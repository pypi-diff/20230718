# Comparing `tmp/check_changelog-0.3.0-py3-none-any.whl.zip` & `tmp/check_changelog-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 9152 bytes, number of entries: 10
+Zip file size: 11972 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx      160 b- defN 16-Jan-01 00:00 check_changelog/__init__.py
--rw-rw-r--  2.0 unx     3702 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
--rw-rw-r--  2.0 unx     8027 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
+-rw-rw-r--  2.0 unx     3301 b- defN 16-Jan-01 00:00 check_changelog/__main__.py
+-rw-rw-r--  2.0 unx     8388 b- defN 16-Jan-01 00:00 check_changelog/changelog.py
 -rw-rw-r--  2.0 unx     2011 b- defN 16-Jan-01 00:00 check_changelog/git.py
+-rw-rw-r--  2.0 unx      979 b- defN 16-Jan-01 00:00 check_changelog/misc.py
+-rw-rw-r--  2.0 unx     5580 b- defN 16-Jan-01 00:00 check_changelog/release.py
 -rw-rw-r--  2.0 unx       21 b- defN 16-Jan-01 00:00 check_changelog/__version__.py
-?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/WHEEL
-?rw-------  2.0 unx     4385 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/licenses/LICENSE
-?rw-------  2.0 unx      854 b- defN 16-Jan-01 00:00 check_changelog-0.3.0.dist-info/RECORD
-10 files, 20415 bytes uncompressed, 7680 bytes compressed:  62.4%
+?rw-------  2.0 unx       65 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/WHEEL
+?rw-------  2.0 unx     4896 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/licenses/LICENSE
+?rw-------  2.0 unx     1016 b- defN 16-Jan-01 00:00 check_changelog-0.4.0.dist-info/RECORD
+12 files, 27607 bytes uncompressed, 10250 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -6,26 +6,32 @@
 
 Filename: check_changelog/changelog.py
 Comment: 
 
 Filename: check_changelog/git.py
 Comment: 
 
+Filename: check_changelog/misc.py
+Comment: 
+
+Filename: check_changelog/release.py
+Comment: 
+
 Filename: check_changelog/__version__.py
 Comment: 
 
-Filename: check_changelog-0.3.0.dist-info/entry_points.txt
+Filename: check_changelog-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_changelog-0.3.0.dist-info/WHEEL
+Filename: check_changelog-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: check_changelog-0.3.0.dist-info/METADATA
+Filename: check_changelog-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: check_changelog-0.3.0.dist-info/licenses/LICENSE
+Filename: check_changelog-0.4.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: check_changelog-0.3.0.dist-info/RECORD
+Filename: check_changelog-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_changelog/__main__.py

```diff
@@ -17,14 +17,16 @@
 
 import pydevkit.log.config  # noqa: F401
 from pydevkit.argparse import ArgumentParser
 
 from . import __version__
 from .changelog import check_changelog_main
 from .git import git_check_tags
+from .misc import run_task
+from .release import do_release
 
 log = logging.getLogger(__name__)
 
 bool_yes_no = ["yes", "no"]
 
 
 def get_args():
@@ -38,14 +40,22 @@
     p.add_argument(
         "--install",
         help=("if value is 'yes', installs git 'pre-push' hook"),
         choices=bool_yes_no,
         default="no",
     )
     p.add_argument(
+        "--release",
+        help=(
+            "if value is 'new', ensures CHANGELOG.md exists and has [Unreleased]"
+            " section. Otherwise, create new release with this name."
+            " based on [Unreleased] content"
+        ),
+    )
+    p.add_argument(
         "--tags",
         help=(
             "check that specified git tags are documented. "
             "Value can be 'hook' to read tag "
             "refs from stdin as pre-push hook would do. Or it can be "
             "'history:N' for N latest tags, or 'history' to all tags."
         ),
@@ -55,70 +65,34 @@
     p.add_argument(
         "--file", help="changelog file to check", default="CHANGELOG.md"
     )
 
     return p.parse_known_args()
 
 
-def task_status(ttype, tname, status):
-    clrs = {
-        "norm": "\033[0m",
-        "ok": "\033[32;1m",
-        "fail": "\033[31;1m",
-        "starting": "\033[32;1m",
-    }
-    msg = ""
-    rc = {
-        "clr-off": clrs["norm"],
-        "clr-on": clrs[status],
-        "type": ttype,
-        "name": tname,
-        "status": status,
-    }
-    fmt = "%(clr-on)s%(type)s%(clr-off)s %(name)s: %(clr-on)s%(status)s%(clr-off)s"
-    msg += fmt % rc
-    return msg
-
-
-def run_task(ttype, tname, func, *args):
-    _norm = "\033[0m"
-    _ok = "\033[32;1m"
-    _fail = "\033[31;1m"
-    log.info("%s", task_status(ttype, tname, "starting"))
-    try:
-        rc = func(*args)
-    except Exception as exc:
-        rc = False
-        log.error("%s", exc)
-    if rc:
-        log.info("%s", task_status(ttype, tname, "ok"))
-    else:
-        log.error("%s", task_status(ttype, tname, "fail"))
-    return rc
-
-
 def run_all_tasks(args):
+    log.info("read %s", args.file)
     text = open(args.file, "r").read()
-    rcs = []
+    rcs = {}
     if args.check == "yes":
         rc = run_task(
             "task",
             "check changelog structure",
             check_changelog_main,
             args.file,
             text,
         )
-        rcs.append(rc)
+        rcs["check"] = rc
 
     if args.tags:
         rc = run_task(
             "task", "check tags documentation", git_check_tags, text, args.tags
         )
-        rcs.append(rc)
-
+        rcs["tags"] = rc
+    log.debug("run_all_tasks: %s", rcs)
     return all(rcs)
 
 
 def install_git_hook():
     path = ".git/hooks/pre-push"
     if os.path.exists(path):
         log.warning("remove current '%s'", path)
@@ -138,15 +112,17 @@
         try:
             log.info("working dir '%s'", args.topdir)
             os.chdir(args.topdir)
         except Exception as exp:
             log.error("%s", exp)
             sys.exit(1)
 
-    if args.install == "yes":
+    if args.release:
+        rc = run_task("release", args.release, do_release, args)
+    elif args.install == "yes":
         rc = run_task("hook", "install pre-push", install_git_hook)
     else:
         rc = run_task("file", args.file, run_all_tasks, args)
     sys.exit(0 if rc else 1)
 
 
 if __name__ == "__main__":
```

## check_changelog/changelog.py

```diff
@@ -5,14 +5,15 @@
 """
 
 import inspect
 import logging
 import re
 
 from markdown_it import MarkdownIt
+from pydevkit.log import prettify
 
 log = logging.getLogger(__name__)
 logging.getLogger("markdown_it").setLevel(logging.INFO)
 
 
 class Tokens(list):
     def __init__(self, *args, **kwargs):
@@ -86,19 +87,37 @@
     pass
 
 
 class CLPartiallyFoundError(CLError):
     pass
 
 
+xdata = []
+
+
 def run(func, narg):
-    log.debug("func %s, narg %s", func, narg)
+    data_len = len(xdata)
+    xdata.append({})
+    try:
+        run_real(func, narg)
+        rc = xdata[data_len]
+        log.debug("func %s, narg %s: exit %s", func, narg, rc)
+        return rc
+    except Exception:
+        raise
+    finally:
+        log.debug("func %s, narg %s: cleanup", func, narg)
+        del xdata[data_len:]
+
+
+def run_real(func, narg):
     count = 0
     while True:
         try:
+            log.debug("func %s, narg %s: enter", func, narg)
             func()
         except CLSyntaxError:
             raise
         except CLNotFoundError as exp:
             if narg == "?" or narg == "*":
                 return
             if narg == "+" and count > 0:
@@ -138,45 +157,41 @@
     tokens.consume_until(
         lambda x: x.tag == tag
         and x.type == tag2type[tag] + "_close"
         and x.level == t.level
     )
 
 
-ctx = {}
-
-
 def title():
-    log.debug("%s", func_name())
     msg = "expected 'Changelog'"
 
     def _validate(msg):
         t = tokens.next()
         log.info("title: %s", t.content)
         if t.content != "Changelog":
             m1 = "bad title"
             raise CLSyntaxError(m1, t, msg)
+        xdata[-1]["title"] = t.content
 
     do_item("h1", msg, _validate)
 
 
 def notes():
-    log.debug("%s", func_name())
-
     def _validate(msg):  # noqa: ARG001
         t = tokens.next()
         t.content.replace("\n", " ")
-        tlen = len(t.content) + ctx.get("notes", 0)
-        ctx["notes"] = tlen
+        obj = xdata[-1]
+        size = obj.get("notes", 0)
+        size += len(t.content)
+        obj["notes"] = size
 
     do_item("p", "", _validate)
 
 
 def release_header():
-    log.debug("%s", func_name())
     msg = "expected '[Unreleased]' or '[ver] - YYYY-MM-DD'"
     msgr = "expected '[ver] - YYYY-MM-DD'"
 
     def _validate(msg):
         t = tokens.next()
         log.info("release: %s", t.content)
         kids_num_unreleased = 3
@@ -189,48 +204,48 @@
             m1 = "no link for release"
             raise CLSyntaxError(m1, t)
         rname = t.children[1].content
         log.debug("rname '%s'", rname)
         if rname is None:
             m1 = "bad release title"
             raise CLSyntaxError(m1, t, msg)
+        xdata[-1]["name"] = rname
 
         if rname == "Unreleased":
             if len(t.children) != kids_num_unreleased:
                 m1 = "bad release title"
                 raise CLSyntaxError(m1, t, msg)
             return
         if len(t.children) != kids_num_released:
             m1 = "bad release title"
             raise CLSyntaxError(m1, t, msg)
         rdate = t.children[3].content
         log.debug("rdate '%s'", rdate)
         if not re.search("^ - \\d\\d\\d\\d-\\d\\d-\\d\\d$", rdate):
             m1 = "bad release date"
             raise CLSyntaxError(m1, t, msgr)
+        xdata[-1]["date"] = rdate.split()[-1]
 
     do_item("h2", msg, _validate)
 
 
 def change():
-    log.debug("%s", func_name())
     msg = "expecting list item"
-    idx = ctx["changes"]["idx"]
     do_item("li", msg, None)
-    count = ctx["changes"].get(idx, 0)
-    ctx["changes"][idx] = count + 1
+    count = xdata[-1].get("num", 0)
+    xdata[-1]["num"] = count + 1
 
 
 def change_list():
-    log.debug("%s", func_name())
     msg = "expecting unordered list"
 
     def _validate(msg):  # noqa: ARG001
         tokens.next()
-        run(change, narg="+")
+        rc = run(change, narg="+")
+        xdata[-1].update(rc)
 
     do_item("ul", msg, _validate)
 
 
 change_type_names = [
     "Added",
     "Changed",
@@ -239,75 +254,73 @@
     "Fixed",
     "Security",
 ]
 change_type_len = max([len(k) for k in change_type_names])
 
 
 def change_type():
-    log.debug("%s", func_name())
     msg = "expecting '### <Change Type>'"
 
     def _validate(msg):
         t = tokens.next()
         log.debug("change type: %s", t.content)
         msg += "; got '%s'" % t.content
         if t.content not in change_type_names:
             m1 = "bad change type"
             raise CLSyntaxError(m1, t, "expected one of %s" % change_type_names)
-        ctx["changes"]["idx"] = t.content
+        xdata[-1]["type"] = t.content.lower()
 
     do_item("h3", msg, _validate)
 
 
 def change_block():
-    log.debug("%s", func_name())
-    run(change_type, narg=1)
+    rc = run(change_type, narg=1)
     try:
-        run(change_list, narg="+")
+        rc.update(run(change_list, narg="+"))
     except CLNotFoundError as exp:
         raise CLSyntaxError(exp.msg, exp.token) from exp
+    log.debug("change_block rc: %s", rc)
+    num = xdata[-1].get(rc["type"], 0)
+    xdata[-1][rc["type"]] = rc["num"] + num
 
 
 def release():
-    log.debug("%s", func_name())
-    run(release_header, narg=1)
-
-    ctx["notes"] = 0
-    run(notes, narg="*")
-    nnotes = ctx.get("notes")
-    if nnotes:
-        log.info("  notes: %d chars", nnotes)
-    del ctx["notes"]
-
-    ctx["changes"] = {"idx": "none"}
-    run(change_block, narg="*")
-    del ctx["changes"]["idx"]
-    keys = ctx["changes"].keys()
-    if keys:
-        fmt = "  %%-%ds: %%s" % change_type_len
-        for k, v in ctx["changes"].items():
-            log.info(fmt, k.lower(), v)
+    rel = {}
+    rc = run(release_header, narg=1)
+    rel.update(rc)
+
+    rc = run(notes, narg="*")
+    rel.update(rc)
+
+    rc = run(change_block, narg="*")
+    rel["changes"] = rc
+    log.debug("release: %s", rel)
+    arr = xdata[-1].get("rels", [])
+    arr.append(rel)
+    xdata[-1]["rels"] = arr
 
 
 def check_changelog(text):
-    log.debug("%s", func_name())
     md = MarkdownIt("commonmark", {"breaks": True, "html": True})
     global tokens  # noqa: PLW0603
     tokens = Tokens(md.parse(text))
 
-    run(title, narg=1)
-    run(notes, narg="*")
-    nnotes = ctx.get("notes")
-    if nnotes:
-        log.info("  notes: %d chars", nnotes)
-        del ctx["notes"]
-    run(release, narg="+")
+    xdata.append({"releases": []})
+    rc = run(title, narg=1)
+    xdata[-1].update(rc)
+    rc = run(notes, narg="*")
+    xdata[-1].update(rc)
+    rc = run(release, narg="+")
+    xdata[-1]["releases"] += rc["rels"]
+    log.debug("xdata: %s", xdata)
+    rc = xdata.pop()
+    log.debug("final rc: %s", prettify(rc))
 
     if tokens.is_empty() or tokens.get().tag == "hr":
-        return True
+        return rc
     msg = "out of context"
     raise CLSyntaxError(msg, tokens.get())
 
 
 def check_changelog_main(fname, text):
     try:
         return check_changelog(text)
```

## check_changelog/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.3.0'
+__version__ = '0.4.0'
```

## Comparing `check_changelog-0.3.0.dist-info/METADATA` & `check_changelog-0.4.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: check-changelog
-Version: 0.3.0
+Version: 0.4.0
 Summary: check that changelog conforms to 'Keep A Changelog' style
 Author-email: Anatoly Asviyan <aanatoly@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Dist: markdown-it-py
 Requires-Dist: pydevkit<4.0.0,>=3.1.2
+Requires-Dist: toml
 Project-URL: Homepage, https://github.com/aanatoly/check-changelog
 Project-URL: Repository, https://github.com/aanatoly/check-changelog
 Description-Content-Type: text/markdown
 
 # check-changelog
 
 [![pkg - version][pkg-version]][pkg-link]
@@ -28,66 +29,111 @@
 ---
 The project's aims are:
  - validate `CHANGELOG.md`. Check that it conforms to
    [Keep A Changelog][kacl] and [Common Changelog][ccl] styles.
  - ensure git tags are documented in `CHANGELOG.md`
  - block pushing tags without changelog. See [git pre-push](#git-pre-push-hook) section
 
-Main features:
- - check that changelog conforms to [Keep A Changelog][kacl] style
- - allow release notes. Add them between the release header and change list
+The supported changelog style is [Keep A Changelog][kacl] style with these
+additions:
+
+ - allow changelog notes
+
+   ```markdown
+   # Changelog
+   Changelog notes
+
+   ## [Unreleased]
+   ```
+
+ - allow release notes
    ([Common Changelog][ccl] addition)
 
    ```markdown
    ## [1.0.0] - 2023-05-05
    Release notes
 
    ### Added
     - add feature ...
    ```
 
- - allow custom footer to keep things from being verified. Useful for legal
-   notes, text used by other scripts, HTML comments, etc
+ - allow custom footer to separate tech stuff from changelog content.
+   Useful for legal notes, text used by other scripts, HTML comments, etc
 
    ```markdown
    -----
    Linter will ignore this section.
    <!--- message for some script -->
    [my site]: http://mysite.com
    ```
 
- - `gcc` style error reports
-   ```text
-   CHANGELOG.md:10: bad release title: [0.2.1]; expected '[Unreleased]' or '[ver] - YYYY-MM-DD'
-   CHANGELOG.md:12: bad change type: Changed2; expected one of ['Added', 'Changed', ...]
-    ```
-
 ## Installation
 
 ```sh
 pip install check-changelog
 ```
 
 ## Usage
-From command line
+
+### From command line
+
+Check changelog style
+
+```sh
+check-changelog --check=yes
+```
+
+Ensure git tags are documented in a changelog
 
 ```sh
-# check CHANGELOG.md in a current dir
-check-changelog
-check-changelog --check=yes --tags=   # default settings
-# check CHANGELOG.md and git tags
-check-changelog --check=yes --tags=history
+check-changelog --tags=history
+```
+
+Add `Unreleased` section to a changelog, create a new changelog if needed
+
+```sh
+check-changelog --release=new
+```
+
+Create release `3.3.3` from current `Unreleased` section
+
+```sh
+check-changelog --release="3.3.3"
+```
+
+```diff
+--- CHANGELOG.md
++++ CHANGELOG.md
+@@ -2,6 +2,8 @@
+
+ ## [Unreleased]
+
++## [3.3.3] - 2023-07-17
++
+ ### Changed
+
+  - some change
+@@ -20,6 +22,7 @@
+ ## [0.1.0] - 2023-07-11
+
+ [Unreleased]: https://github.com/aanatoly/check-changelog
++[3.3.3]: https://github.com/aanatoly/check-changelog/releases/tag/3.3.3
+ [0.3.0]: https://github.com/aanatoly/check-changelog/releases/tag/0.3.0
+ [0.2.1]: https://github.com/aanatoly/check-changelog/releases/tag/0.2.1
+
+
 ```
 
+### pre-commit hook
 As a [pre-commit](https://pre-commit.com/) hook.
 Add this section to your `.pre-commit-config.yaml`
 
 ```yml
 - repo: https://github.com/aanatoly/check-changelog
-  rev: '0.3.0'
+  rev: '0.4.0'
   hooks:
     - id: check-changelog
 ```
 
 ### git pre-push hook
 As a git `pre-push` hook, `check-changelog` can block `git` from pushing
 tags without changelog. To install it that way, run the following commmands
```

## Comparing `check_changelog-0.3.0.dist-info/licenses/LICENSE` & `check_changelog-0.4.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

