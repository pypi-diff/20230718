# Comparing `tmp/tuack-0.1.5.1.2.tar.gz` & `tmp/tuack-0.1.5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuack-0.1.5.1.2.tar", last modified: Sun May 28 15:37:45 2023, max compression
+gzip compressed data, was "tuack-0.1.5.1.3.tar", last modified: Tue Jul 18 04:09:01 2023, max compression
```

## Comparing `tuack-0.1.5.1.2.tar` & `tuack-0.1.5.1.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.843270 tuack-0.1.5.1.2/
--rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/LICENSE
--rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      522 2023-05-28 15:37:45.841838 tuack-0.1.5.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 15:37:45.843270 tuack-0.1.5.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1930 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.771806 tuack-0.1.5.1.2/tuack/
--rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/__init__.py
--rw-rw-rw-   0        0        0    34950 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/base.py
--rw-rw-rw-   0        0        0    13348 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/doc.py
--rw-rw-rw-   0        0        0    27596 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/dump.py
--rw-rw-rw-   0        0        0    14486 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/gen.py
--rw-rw-rw-   0        0        0     2334 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/install.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.801724 tuack-0.1.5.1.2/tuack/lex/
--rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1.2/tuack/lex/compile.log
--rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/compile.pyinc
--rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/format-linux
--rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/format-mac
--rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/format-win.exe
--rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1.2/tuack/lex/hehe.log
--rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/lex.l
--rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1.2/tuack/lex/lex.yy.c
--rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1.2/tuack/lex/lex.yy.o
--rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/main.h
--rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1.2/tuack/lex/yacc.tab.c
--rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1.2/tuack/lex/yacc.tab.h
--rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1.2/tuack/lex/yacc.tab.o
--rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/yacc.y
--rw-rw-rw-   0        0        0    12217 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/load.py
--rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/num2chinese.py
--rw-rw-rw-   0        0        0    13010 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/packer.py
--rw-rw-rw-   0        0        0    24499 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/ren.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.812000 tuack-0.1.5.1.2/tuack/sample/
--rw-rw-rw-   0        0        0     7909 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/arbiter_e.noi_linux1.sample
--rw-rw-rw-   0        0        0    23576 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/arbiter_e.sample
--rw-rw-rw-   0        0        0     5586 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/chk.cpp
--rw-rw-rw-   0        0        0      195 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/contest.gitignore
--rw-rw-rw-   0        0        0      266 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/contest.json
--rw-rw-rw-   0        0        0      186 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/day.gitignore
--rw-rw-rw-   0        0        0      207 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/day.json
--rw-rw-rw-   0        0        0      351 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/empty.gitattributes
--rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/empty.gitignore
--rw-rw-rw-   0        0        0      435 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/empty.json
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.827125 tuack-0.1.5.1.2/tuack/sample/precautions/
--rw-rw-rw-   0        0        0       60 2023-05-18 04:27:16.000000 tuack-0.1.5.1.2/tuack/sample/precautions/zh-cn.md
--rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/sample/problem.gitattributes
--rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/problem.gitignore
--rw-rw-rw-   0        0        0      466 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/problem.json
--rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/sample/uoj.json
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.704238 tuack-0.1.5.1.2/tuack/sample-empty/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.812996 tuack-0.1.5.1.2/tuack/sample-empty/statement/
--rw-rw-rw-   0        0        0      411 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-empty/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.748398 tuack-0.1.5.1.2/tuack/sample-problem/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.814487 tuack-0.1.5.1.2/tuack/sample-problem/data/
--rw-rw-rw-   0        0        0       44 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/data/1.ans
--rw-rw-rw-   0        0        0       43 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/data/1.in
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.815846 tuack-0.1.5.1.2/tuack/sample-problem/down/
--rw-rw-rw-   0        0        0       79 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/down/1.ans
--rw-rw-rw-   0        0        0       77 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/down/1.in
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.815846 tuack-0.1.5.1.2/tuack/sample-problem/pre/
--rw-rw-rw-   0        0        0       80 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/pre/1.ans
--rw-rw-rw-   0        0        0       78 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/pre/1.in
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.817337 tuack-0.1.5.1.2/tuack/sample-problem/resources/
--rw-rw-rw-   0        0        0  3293583 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/resources/sample.png
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.822657 tuack-0.1.5.1.2/tuack/sample-problem/solution/
--rw-rw-rw-   0        0        0     1968 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/solution/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.822657 tuack-0.1.5.1.2/tuack/sample-problem/statement/
--rw-rw-rw-   0        0        0     6819 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.825129 tuack-0.1.5.1.2/tuack/sample-problem/tables/
--rw-rw-rw-   0        0        0     1062 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/tables/data.pyinc
--rw-rw-rw-   0        0        0     1227 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/tables/json_data.json
--rw-rw-rw-   0        0        0      205 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/tables/table.json
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.838401 tuack-0.1.5.1.2/tuack/templates/
--rw-rw-rw-   0        0        0      911 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/ccc.tex.jinja
--rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/templates/ccpc.png
--rw-rw-rw-   0        0        0     1240 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/ccpc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.751611 tuack-0.1.5.1.2/tuack/templates/en/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.839397 tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/font.html.jinja
--rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/font.tex.jinja
--rw-rw-rw-   0        0        0      670 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/hand.tex.jinja
--rw-rw-rw-   0        0        0      144 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/image.html.jinja
--rw-rw-rw-   0        0        0      530 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/image.tex.jinja
--rw-rw-rw-   0        0        0     5116 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/problem_base.md.jinja
--rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/table.html.jinja
--rw-rw-rw-   0        0        0      402 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/table.md.jinja
--rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/templates/table.tex.jinja
--rw-rw-rw-   0        0        0     2125 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/template_base.tex.jinja
--rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/template_base.tex.jinja.tex
--rw-rw-rw-   0        0        0     4756 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/tuack.cls
--rw-rw-rw-   0        0        0     8743 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/tuoi.tex.jinja
--rw-rw-rw-   0        0        0     1443 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/tupc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.752802 tuack-0.1.5.1.2/tuack/templates/zh-cn/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.840485 tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3139 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3543 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0    17556 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/test.py
--rw-rw-rw-   0        0        0     3777 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.783624 tuack-0.1.5.1.2/tuack.egg-info/
--rw-rw-rw-   0        0        0      522 2023-05-28 15:37:44.000000 tuack-0.1.5.1.2/tuack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-05-28 15:37:45.000000 tuack-0.1.5.1.2/tuack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 15:37:44.000000 tuack-0.1.5.1.2/tuack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-28 15:37:45.000000 tuack-0.1.5.1.2/tuack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 15:37:45.000000 tuack-0.1.5.1.2/tuack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.363702 tuack-0.1.5.1.3/
+-rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/LICENSE
+-rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      522 2023-07-18 04:09:01.362886 tuack-0.1.5.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1717 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 04:09:01.363702 tuack-0.1.5.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1930 2023-07-18 04:08:34.000000 tuack-0.1.5.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.433805 tuack-0.1.5.1.3/tuack/
+-rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1.3/tuack/__init__.py
+-rw-rw-rw-   0        0        0    34950 2023-05-20 05:40:17.000000 tuack-0.1.5.1.3/tuack/base.py
+-rw-rw-rw-   0        0        0    13348 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/doc.py
+-rw-rw-rw-   0        0        0    27596 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/dump.py
+-rw-rw-rw-   0        0        0    14486 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/gen.py
+-rw-rw-rw-   0        0        0     2334 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/install.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.911376 tuack-0.1.5.1.3/tuack/lex/
+-rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1.3/tuack/lex/compile.log
+-rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/compile.pyinc
+-rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/format-linux
+-rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/format-mac
+-rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/format-win.exe
+-rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1.3/tuack/lex/hehe.log
+-rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/lex.l
+-rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1.3/tuack/lex/lex.yy.c
+-rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1.3/tuack/lex/lex.yy.o
+-rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/main.h
+-rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1.3/tuack/lex/yacc.tab.c
+-rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1.3/tuack/lex/yacc.tab.h
+-rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1.3/tuack/lex/yacc.tab.o
+-rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/lex/yacc.y
+-rw-rw-rw-   0        0        0    12217 2023-05-20 05:40:17.000000 tuack-0.1.5.1.3/tuack/load.py
+-rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/num2chinese.py
+-rw-rw-rw-   0        0        0    13010 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/packer.py
+-rw-rw-rw-   0        0        0    24785 2023-07-18 04:08:34.000000 tuack-0.1.5.1.3/tuack/ren.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.046100 tuack-0.1.5.1.3/tuack/sample/
+-rw-rw-rw-   0        0        0     7909 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/arbiter_e.noi_linux1.sample
+-rw-rw-rw-   0        0        0    23576 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/arbiter_e.sample
+-rw-rw-rw-   0        0        0     5586 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/chk.cpp
+-rw-rw-rw-   0        0        0      195 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/contest.gitignore
+-rw-rw-rw-   0        0        0      266 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/contest.json
+-rw-rw-rw-   0        0        0      186 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/day.gitignore
+-rw-rw-rw-   0        0        0      207 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/day.json
+-rw-rw-rw-   0        0        0      351 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/empty.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/empty.gitignore
+-rw-rw-rw-   0        0        0      435 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/empty.json
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.196387 tuack-0.1.5.1.3/tuack/sample/precautions/
+-rw-rw-rw-   0        0        0       60 2023-05-18 04:27:16.000000 tuack-0.1.5.1.3/tuack/sample/precautions/zh-cn.md
+-rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1.3/tuack/sample/problem.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/problem.gitignore
+-rw-rw-rw-   0        0        0      466 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample/problem.json
+-rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1.3/tuack/sample/uoj.json
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.311531 tuack-0.1.5.1.3/tuack/sample-empty/
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.050103 tuack-0.1.5.1.3/tuack/sample-empty/statement/
+-rw-rw-rw-   0        0        0      411 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-empty/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.311531 tuack-0.1.5.1.3/tuack/sample-problem/
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.070404 tuack-0.1.5.1.3/tuack/sample-problem/data/
+-rw-rw-rw-   0        0        0       44 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/data/1.ans
+-rw-rw-rw-   0        0        0       43 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/data/1.in
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.087562 tuack-0.1.5.1.3/tuack/sample-problem/down/
+-rw-rw-rw-   0        0        0       79 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/down/1.ans
+-rw-rw-rw-   0        0        0       77 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/down/1.in
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.104322 tuack-0.1.5.1.3/tuack/sample-problem/pre/
+-rw-rw-rw-   0        0        0       80 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/pre/1.ans
+-rw-rw-rw-   0        0        0       78 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/pre/1.in
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.121803 tuack-0.1.5.1.3/tuack/sample-problem/resources/
+-rw-rw-rw-   0        0        0  3293583 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/resources/sample.png
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.138116 tuack-0.1.5.1.3/tuack/sample-problem/solution/
+-rw-rw-rw-   0        0        0     1968 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/solution/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.150204 tuack-0.1.5.1.3/tuack/sample-problem/statement/
+-rw-rw-rw-   0        0        0     6819 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.188019 tuack-0.1.5.1.3/tuack/sample-problem/tables/
+-rw-rw-rw-   0        0        0     1062 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/tables/data.pyinc
+-rw-rw-rw-   0        0        0     1227 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/tables/json_data.json
+-rw-rw-rw-   0        0        0      205 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/sample-problem/tables/table.json
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.329149 tuack-0.1.5.1.3/tuack/templates/
+-rw-rw-rw-   0        0        0      911 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/ccc.tex.jinja
+-rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1.3/tuack/templates/ccpc.png
+-rw-rw-rw-   0        0        0     1240 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/ccpc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.311531 tuack-0.1.5.1.3/tuack/templates/en/
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.345378 tuack-0.1.5.1.3/tuack/templates/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/templates/en/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/templates/en/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/templates/font.html.jinja
+-rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/templates/font.tex.jinja
+-rw-rw-rw-   0        0        0      670 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/hand.tex.jinja
+-rw-rw-rw-   0        0        0      144 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/image.html.jinja
+-rw-rw-rw-   0        0        0      530 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/image.tex.jinja
+-rw-rw-rw-   0        0        0     5116 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/problem_base.md.jinja
+-rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/templates/table.html.jinja
+-rw-rw-rw-   0        0        0      402 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/table.md.jinja
+-rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1.3/tuack/templates/table.tex.jinja
+-rw-rw-rw-   0        0        0     2125 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/template_base.tex.jinja
+-rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1.3/tuack/templates/template_base.tex.jinja.tex
+-rw-rw-rw-   0        0        0     4756 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/tuack.cls
+-rw-rw-rw-   0        0        0     8743 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/tuoi.tex.jinja
+-rw-rw-rw-   0        0        0     1443 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/tupc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.315923 tuack-0.1.5.1.3/tuack/templates/zh-cn/
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:01.358587 tuack-0.1.5.1.3/tuack/templates/zh-cn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3139 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3543 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/templates/zh-cn/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0    17556 2023-05-20 05:40:17.000000 tuack-0.1.5.1.3/tuack/test.py
+-rw-rw-rw-   0        0        0     3777 2023-05-18 04:27:25.000000 tuack-0.1.5.1.3/tuack/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:09:00.470202 tuack-0.1.5.1.3/tuack.egg-info/
+-rw-rw-rw-   0        0        0      522 2023-07-18 04:08:59.000000 tuack-0.1.5.1.3/tuack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-07-18 04:09:00.000000 tuack-0.1.5.1.3/tuack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 04:08:59.000000 tuack-0.1.5.1.3/tuack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-18 04:08:59.000000 tuack-0.1.5.1.3/tuack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 04:08:59.000000 tuack-0.1.5.1.3/tuack.egg-info/top_level.txt
```

### Comparing `tuack-0.1.5.1.2/LICENSE` & `tuack-0.1.5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/PKG-INFO` & `tuack-0.1.5.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.1.2
+Version: 0.1.5.1.3
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.1.2/README.md` & `tuack-0.1.5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/setup.py` & `tuack-0.1.5.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	'pyyaml >= 5.1',
 	'rarfile >= 3.0',
 	'requests_toolbelt >= 0.9.1'
 ]
 
 setup(
 	name = 'tuack',
-	version = '0.1.5.1.2',
+	version = '0.1.5.1.3',
 	packages = find_packages(),
 	author = 'Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan',
 	author_email = 'chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn',
 	url = '',
 	license = 'https://git.thusaac.com/publish/tuack/blob/master/LICENSE',
 	description = 'Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.',
 	cmdclass={
```

### Comparing `tuack-0.1.5.1.2/tuack/base.py` & `tuack-0.1.5.1.3/tuack/base.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/doc.py` & `tuack-0.1.5.1.3/tuack/doc.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/dump.py` & `tuack-0.1.5.1.3/tuack/dump.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/gen.py` & `tuack-0.1.5.1.3/tuack/gen.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/install.py` & `tuack-0.1.5.1.3/tuack/install.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/compile.pyinc` & `tuack-0.1.5.1.3/tuack/lex/compile.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/format-linux` & `tuack-0.1.5.1.3/tuack/lex/format-linux`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/format-mac` & `tuack-0.1.5.1.3/tuack/lex/format-mac`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/format-win.exe` & `tuack-0.1.5.1.3/tuack/lex/format-win.exe`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/lex.l` & `tuack-0.1.5.1.3/tuack/lex/lex.l`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/lex.yy.c` & `tuack-0.1.5.1.3/tuack/lex/lex.yy.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/lex.yy.o` & `tuack-0.1.5.1.3/tuack/lex/lex.yy.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/yacc.tab.c` & `tuack-0.1.5.1.3/tuack/lex/yacc.tab.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/yacc.tab.h` & `tuack-0.1.5.1.3/tuack/lex/yacc.tab.h`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/lex/yacc.tab.o` & `tuack-0.1.5.1.3/tuack/lex/yacc.tab.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/load.py` & `tuack-0.1.5.1.3/tuack/load.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/num2chinese.py` & `tuack-0.1.5.1.3/tuack/num2chinese.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/packer.py` & `tuack-0.1.5.1.3/tuack/packer.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/ren.py` & `tuack-0.1.5.1.3/tuack/ren.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,19 +140,28 @@
 				if type(cur) == tuple:
 					cur = cur[0]
 				las = last[j]
 				if type(las) == tuple:
 					las, opt = las
 				else:
 					opt = {}
+				last[j] = las
 				if (not titled or i != 0) and las == cur and not opt.get('no_merge') and options.get('merge') != False:
 					last[j] = None
 				if (opt.get('no_merge') or options.get('merge') == False) and context.get('comp') in work_class['syzoj_like']:
 					last[j] = str(las) + f"<!--{ uuid.uuid4() }-->"
 			last = ret[i]
+		if len(table) > 0:
+			for j in range(len(table[0])):
+				if type(table[0][j]) == tuple:
+					table[0][j] = table[0][j][0]
+		if titled and len(table) > 1:
+			for j in range(len(table[1])):
+				if type(table[1][j]) == tuple:
+					table[1][j] = table[1][j][0]
 		return ret
 	if suf == '.json':
 		res = get_template('table.json', context['prob'].lang()).render(context, options = options)
 		try:
 			table = json.loads(res)
 		except Exception as e:
 			open(pjoin('tmp', 'table.tmp.json'), 'w').write(res)
```

### Comparing `tuack-0.1.5.1.2/tuack/sample/arbiter_e.noi_linux1.sample` & `tuack-0.1.5.1.3/tuack/sample/arbiter_e.noi_linux1.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample/arbiter_e.sample` & `tuack-0.1.5.1.3/tuack/sample/arbiter_e.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample/chk.cpp` & `tuack-0.1.5.1.3/tuack/sample/chk.cpp`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample-problem/resources/sample.png` & `tuack-0.1.5.1.3/tuack/sample-problem/resources/sample.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample-problem/solution/zh-cn.md` & `tuack-0.1.5.1.3/tuack/sample-problem/solution/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample-problem/statement/zh-cn.md` & `tuack-0.1.5.1.3/tuack/sample-problem/statement/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample-problem/tables/data.pyinc` & `tuack-0.1.5.1.3/tuack/sample-problem/tables/data.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/sample-problem/tables/json_data.json` & `tuack-0.1.5.1.3/tuack/sample-problem/tables/json_data.json`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/ccc.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/ccc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/ccpc.png` & `tuack-0.1.5.1.3/tuack/templates/ccpc.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/ccpc.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/ccpc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1.3/tuack/templates/en/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.po` & `tuack-0.1.5.1.3/tuack/templates/en/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/hand.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/hand.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/image.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/image.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/problem_base.md.jinja` & `tuack-0.1.5.1.3/tuack/templates/problem_base.md.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/table.html.jinja` & `tuack-0.1.5.1.3/tuack/templates/table.html.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/table.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/table.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/template_base.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/template_base.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/tuack.cls` & `tuack-0.1.5.1.3/tuack/templates/tuack.cls`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/tuoi.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/tuoi.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/tupc.tex.jinja` & `tuack-0.1.5.1.3/tuack/templates/tupc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1.3/tuack/templates/zh-cn/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.po` & `tuack-0.1.5.1.3/tuack/templates/zh-cn/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/test.py` & `tuack-0.1.5.1.3/tuack/test.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack/tools.py` & `tuack-0.1.5.1.3/tuack/tools.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.2/tuack.egg-info/PKG-INFO` & `tuack-0.1.5.1.3/tuack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.1.2
+Version: 0.1.5.1.3
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.1.2/tuack.egg-info/SOURCES.txt` & `tuack-0.1.5.1.3/tuack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

