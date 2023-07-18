# Comparing `tmp/md2site-0.0.7.tar.gz` & `tmp/md2site-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2site-0.0.7.tar", max compression
+gzip compressed data, was "md2site-0.0.8.tar", max compression
```

## Comparing `md2site-0.0.7.tar` & `md2site-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.7/LICENSE.md
--rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.7/md2site/__init__.py
--rw-r--r--   0        0        0     4048 2023-07-04 11:00:46.653809 md2site-0.0.7/md2site/generator.py
--rw-r--r--   0        0        0     2464 2023-07-04 10:39:56.386981 md2site-0.0.7/md2site/post.py
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.7/md2site/py.typed
--rw-r--r--   0        0        0     3021 2023-07-07 10:53:39.298260 md2site-0.0.7/md2site/renderer.py
--rw-r--r--   0        0        0      419 2023-07-01 10:42:34.126426 md2site-0.0.7/md2site/site.py
--rw-r--r--   0        0        0     1015 2023-07-07 10:54:40.025457 md2site-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.8/md2site/__init__.py
+-rw-r--r--   0        0        0     4179 2023-07-18 04:49:59.319984 md2site-0.0.8/md2site/generator.py
+-rw-r--r--   0        0        0     2655 2023-07-18 04:36:20.493524 md2site-0.0.8/md2site/post.py
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.8/md2site/py.typed
+-rw-r--r--   0        0        0     3021 2023-07-07 10:53:39.298260 md2site-0.0.8/md2site/renderer.py
+-rw-r--r--   0        0        0      419 2023-07-01 10:42:34.126426 md2site-0.0.8/md2site/site.py
+-rw-r--r--   0        0        0     1015 2023-07-18 04:52:57.587331 md2site-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.8/PKG-INFO
```

### Comparing `md2site-0.0.7/LICENSE.md` & `md2site-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `md2site-0.0.7/md2site/generator.py` & `md2site-0.0.8/md2site/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 import shutil
 
 import jinja2
 import toml
 
-from md2site.post import Post, name_to_slug
+from md2site.post import Post, name_to_url
 from md2site.site import PostMetaData, Site
 
 from md2site.renderer import Parser, Renderer, extract_wikilinks
 
 
 def prepare_output_folder():
     output_folder = Path("dist")
@@ -25,19 +25,19 @@
     return Site(base_url, name)
 
 
 def parse_markdown(markdown: str) -> str:
     return markdown
 
 
-def load_post_files() -> list[Post]:
+def load_post_files(site: Site) -> list[Post]:
     posts = list()
     for child in Path("posts").iterdir():
         if child.name.endswith(".md"):
-            posts.append(Post.from_file(child))
+            posts.append(Post.from_file(child, site.base_url))
     posts.sort(key=lambda p: p.created_at, reverse=True)
     return posts
 
 
 def write_html(site: Site, post: Post, template: jinja2.Template):
     with open(f"dist/{post.slug}.html", "w", encoding="utf-8") as file:
         html = template.render(post=post, site=site)
@@ -67,18 +67,14 @@
             continue
         backlinks = []
         for name in backlink_map[post.name]:
             backlinks.append({"title": name, "url": name_to_url(name, base_url)})
         post.backlinks = backlinks
 
 
-def name_to_url(name: str, base_url: str) -> str:
-    return f"{base_url}/{name_to_slug(name)}.html"
-
-
 def populate_prev_next_links(posts: list[Post], base_url: str):
     for index, post in enumerate(posts):
         if index > 0:
             prev_post = posts[index - 1]
             post.prev_post = PostMetaData(
                 prev_post.name,
                 prev_post.title,
@@ -124,16 +120,22 @@
         shutil.copyfile(file, output_folder / file.name)
 
 
 def generate():
     prepare_output_folder()
     copy_static_files()
     site = load_config()
-    posts = load_post_files()
+    all_posts = load_post_files(site)
+    special_posts = [p for p in all_posts if is_special(p)]
+    posts = [p for p in all_posts if not is_special(p)]
     site.link_map = build_link_map(posts)
     site.recent_posts = [
         PostMetaData(p.name, p.title, p.created_at, name_to_url(p.name, site.base_url))
         for p in posts[:10]
     ]
     populate_backlinks(posts, site.base_url)
     populate_prev_next_links(posts, site.base_url)
-    build_posts(posts, site)
+    build_posts(posts + special_posts, site)
+
+
+def is_special(post: Post) -> bool:
+    return post.name == "index"
```

### Comparing `md2site-0.0.7/md2site/post.py` & `md2site-0.0.8/md2site/post.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,41 +24,44 @@
 
     name: str
     title: str
     content: str
     summary: str
     created_at: datetime
     slug: str
+    url: str
     prev_post: PostMetaData | None = None
     next_post: PostMetaData | None = None
     backlinks: list[str] = field(default_factory=list)
 
     @classmethod
-    def from_file(cls, filepath: Path) -> Post:
+    def from_file(cls, filepath: Path, base_url: str) -> Post:
         with open(filepath, "r", encoding="utf-8") as f:
             content = separate_frontmatter(f)
             name = filepath.stem
             if "title" in content.frontmatter:
                 title = content.frontmatter["title"]
             else:
                 title = name
 
             if "date" in content.frontmatter:
-                created_at = content.frontmatter["date"]
+                created_at: datetime = content.frontmatter["date"]
             else:
                 created_at = datetime.fromtimestamp(os.path.getctime(filepath)).replace(
                     tzinfo=timezone.utc
                 )
+
             return Post(
                 name=name,
                 title=title,
                 content=content.body,
                 summary=content.body[:140],
                 created_at=created_at,
                 slug=name_to_slug(name),
+                url=name_to_url(name, base_url),
             )
 
 
 def parse_frontmatter(yaml_text: str) -> dict[str, str]:
     parsed = yaml.safe_load(yaml_text)
     if parsed is not None:
         return parsed
@@ -85,7 +88,11 @@
     frontmatter = parse_frontmatter("".join(frontmatter_lines))
     body = "".join(body_lines)
     return MarkdownContent(frontmatter, body)
 
 
 def name_to_slug(name: str) -> str:
     return name.lower().replace(" ", "-")
+
+
+def name_to_url(name: str, base_url: str) -> str:
+    return f"{base_url}/{name_to_slug(name)}.html"
```

### Comparing `md2site-0.0.7/md2site/renderer.py` & `md2site-0.0.8/md2site/renderer.py`

 * *Files identical despite different names*

### Comparing `md2site-0.0.7/pyproject.toml` & `md2site-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md2site"
-version = "0.0.7"
+version = "0.0.8"
 description = "A static site generator with bare-minimum functionality."
 license = "GPL-3.0-or-later"
 authors = ["Yoonseop Kang <e0engoon@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/e0en/md2site"
 repository = "https://github.com/e0en/md2site"
 classifiers = [
```

### Comparing `md2site-0.0.7/PKG-INFO` & `md2site-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2site
-Version: 0.0.7
+Version: 0.0.8
 Summary: A static site generator with bare-minimum functionality.
 Home-page: https://github.com/e0en/md2site
 License: GPL-3.0-or-later
 Author: Yoonseop Kang
 Author-email: e0engoon@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 1 - Planning
```

