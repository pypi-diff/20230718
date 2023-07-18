# Comparing `tmp/hacapi-0.4.6.tar.gz` & `tmp/hacapi-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hacapi-0.4.6.tar", last modified: Wed Apr  5 19:33:31 2023, max compression
+gzip compressed data, was "hacapi-0.4.7.tar", last modified: Tue Jul 18 18:23:11 2023, max compression
```

## Comparing `hacapi-0.4.6.tar` & `hacapi-0.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 19:33:31.982578 hacapi-0.4.6/
--rw-rw-rw-   0        0        0     1065 2023-04-05 00:04:20.000000 hacapi-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     1264 2023-04-05 19:33:31.980341 hacapi-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      795 2023-04-05 19:29:29.000000 hacapi-0.4.6/README.md
--rw-rw-rw-   0        0        0      557 2023-04-05 19:28:04.000000 hacapi-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 19:33:31.982578 hacapi-0.4.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 19:33:31.873635 hacapi-0.4.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 19:33:31.953429 hacapi-0.4.6/src/hacapi/
--rw-rw-rw-   0        0        0        0 2023-04-05 19:25:58.000000 hacapi-0.4.6/src/hacapi/__init__.py
--rw-rw-rw-   0        0        0     2901 2023-04-04 22:41:20.000000 hacapi-0.4.6/src/hacapi/assignment_grades.py
--rw-rw-rw-   0        0        0     6893 2023-04-05 19:29:05.000000 hacapi-0.4.6/src/hacapi/course_grades.py
--rw-rw-rw-   0        0        0      480 2023-04-04 22:40:16.000000 hacapi-0.4.6/src/hacapi/misc.py
--rw-rw-rw-   0        0        0    26526 2023-04-04 22:40:16.000000 hacapi-0.4.6/src/hacapi/payloads.py
--rw-rw-rw-   0        0        0     1190 2023-04-04 23:51:01.000000 hacapi-0.4.6/src/hacapi/session.py
--rw-rw-rw-   0        0        0     1219 2023-04-04 19:22:07.000000 hacapi-0.4.6/src/hacapi/transcript.py
-drwxrwxrwx   0        0        0        0 2023-04-05 19:33:31.974628 hacapi-0.4.6/src/hacapi.egg-info/
--rw-rw-rw-   0        0        0     1264 2023-04-05 19:33:31.000000 hacapi-0.4.6/src/hacapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-05 19:33:31.000000 hacapi-0.4.6/src/hacapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 19:33:31.000000 hacapi-0.4.6/src/hacapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-05 19:33:31.000000 hacapi-0.4.6/src/hacapi.egg-info/top_level.txt
+drwxr-xr-x   0 iyereshan  (1000) iyereshan  (1000)        0 2023-07-18 18:23:11.233597 hacapi-0.4.7/
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     1065 2023-07-18 17:46:30.000000 hacapi-0.4.7/LICENSE
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     1212 2023-07-18 18:23:11.232597 hacapi-0.4.7/PKG-INFO
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)      756 2023-07-18 17:46:30.000000 hacapi-0.4.7/README.md
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)      537 2023-07-18 18:22:58.000000 hacapi-0.4.7/pyproject.toml
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)       38 2023-07-18 18:23:11.233597 hacapi-0.4.7/setup.cfg
+drwxr-xr-x   0 iyereshan  (1000) iyereshan  (1000)        0 2023-07-18 18:23:11.229597 hacapi-0.4.7/src/
+drwxr-xr-x   0 iyereshan  (1000) iyereshan  (1000)        0 2023-07-18 18:23:11.231597 hacapi-0.4.7/src/hacapi/
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)        0 2023-07-18 17:46:30.000000 hacapi-0.4.7/src/hacapi/__init__.py
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     2785 2023-07-18 17:46:30.000000 hacapi-0.4.7/src/hacapi/assignment_grades.py
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     6643 2023-07-18 18:14:39.000000 hacapi-0.4.7/src/hacapi/course_grades.py
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)      460 2023-07-18 17:46:30.000000 hacapi-0.4.7/src/hacapi/misc.py
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)    26297 2023-07-18 17:46:30.000000 hacapi-0.4.7/src/hacapi/payloads.py
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     7699 2023-07-18 18:22:38.000000 hacapi-0.4.7/src/hacapi/session.py
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     1180 2023-07-18 17:46:30.000000 hacapi-0.4.7/src/hacapi/transcript.py
+drwxr-xr-x   0 iyereshan  (1000) iyereshan  (1000)        0 2023-07-18 18:23:11.232597 hacapi-0.4.7/src/hacapi.egg-info/
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)     1212 2023-07-18 18:23:11.000000 hacapi-0.4.7/src/hacapi.egg-info/PKG-INFO
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)      340 2023-07-18 18:23:11.000000 hacapi-0.4.7/src/hacapi.egg-info/SOURCES.txt
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)        1 2023-07-18 18:23:11.000000 hacapi-0.4.7/src/hacapi.egg-info/dependency_links.txt
+-rw-r--r--   0 iyereshan  (1000) iyereshan  (1000)        7 2023-07-18 18:23:11.000000 hacapi-0.4.7/src/hacapi.egg-info/top_level.txt
```

### Comparing `hacapi-0.4.6/LICENSE` & `hacapi-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hacapi-0.4.6/PKG-INFO` & `hacapi-0.4.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1
-Name: hacapi
-Version: 0.4.6
-Summary: This is a simple API to access the Home Access Center (HAC)
-Author-email: Nazchanel <eshaniyer@duck.com>
-Project-URL: Homepage, https://github.com/Nazchanel/hac-api
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# HAC API
-
-## Introduction
-
-This is a simple API to access the Home Access Center (HAC) of the [Frisco Independent School District](https://www.friscoisd.org/). This API is not affiliated with the school district in any way.
-
----
-
-## Modules
-
-### assignment_grades
-
-* return_quarter_assignments_html(***quarter***)
-* return_quarter_assignments_df(***quarter***)
-* return_current_assignments_df(    )
-* return_current_assignments_html(  )
-
-### course_grades
-
-* return_current_grades(  )
-* return_quarter_grade(***quarter***)
-
-### session
-
-* init(***username***, ***password***)
-* reset(    )
-* return_to_current(    )
-
-### transcript
-
-* return_weighted_gpa(  )
-* return_college_gpa(   )
-
-### misc
-
-* is_updated(***original***, ***new***)
-* get_time( )
-
----
+Metadata-Version: 2.1
+Name: hacapi
+Version: 0.4.7
+Summary: This is a simple API to access the Home Access Center (HAC)
+Author-email: Nazchanel <eshaniyer@duck.com>
+Project-URL: Homepage, https://github.com/Nazchanel/hac-api
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HAC API
+
+## Introduction
+
+This is a simple API to access the Home Access Center (HAC) of the [Frisco Independent School District](https://www.friscoisd.org/). This API is not affiliated with the school district in any way.
+
+---
+
+## Modules
+
+### assignment_grades
+
+* return_quarter_assignments_html(***quarter***)
+* return_quarter_assignments_df(***quarter***)
+* return_current_assignments_df(    )
+* return_current_assignments_html(  )
+
+### course_grades
+
+* return_current_grades(  )
+* return_quarter_grade(***quarter***)
+
+### session
+
+* init(***username***, ***password***)
+* reset(    )
+* return_to_current(    )
+
+### transcript
+
+* return_weighted_gpa(  )
+* return_college_gpa(   )
+
+### misc
+
+* is_updated(***original***, ***new***)
+* get_time( )
+
+---
```

### Comparing `hacapi-0.4.6/README.md` & `hacapi-0.4.7/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# HAC API
-
-## Introduction
-
-This is a simple API to access the Home Access Center (HAC) of the [Frisco Independent School District](https://www.friscoisd.org/). This API is not affiliated with the school district in any way.
-
----
-
-## Modules
-
-### assignment_grades
-
-* return_quarter_assignments_html(***quarter***)
-* return_quarter_assignments_df(***quarter***)
-* return_current_assignments_df(    )
-* return_current_assignments_html(  )
-
-### course_grades
-
-* return_current_grades(  )
-* return_quarter_grade(***quarter***)
-
-### session
-
-* init(***username***, ***password***)
-* reset(    )
-* return_to_current(    )
-
-### transcript
-
-* return_weighted_gpa(  )
-* return_college_gpa(   )
-
-### misc
-
-* is_updated(***original***, ***new***)
-* get_time( )
-
----
+# HAC API
+
+## Introduction
+
+This is a simple API to access the Home Access Center (HAC) of the [Frisco Independent School District](https://www.friscoisd.org/). This API is not affiliated with the school district in any way.
+
+---
+
+## Modules
+
+### assignment_grades
+
+* return_quarter_assignments_html(***quarter***)
+* return_quarter_assignments_df(***quarter***)
+* return_current_assignments_df(    )
+* return_current_assignments_html(  )
+
+### course_grades
+
+* return_current_grades(  )
+* return_quarter_grade(***quarter***)
+
+### session
+
+* init(***username***, ***password***)
+* reset(    )
+* return_to_current(    )
+
+### transcript
+
+* return_weighted_gpa(  )
+* return_college_gpa(   )
+
+### misc
+
+* is_updated(***original***, ***new***)
+* get_time( )
+
+---
```

### Comparing `hacapi-0.4.6/pyproject.toml` & `hacapi-0.4.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-[project]
-name = "hacapi"
-version = "0.4.6"
-authors = [
-  { name="Nazchanel", email="eshaniyer@duck.com" },
-]
-description = "This is a simple API to access the Home Access Center (HAC)"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Nazchanel/hac-api"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+[project]
+name = "hacapi"
+version = "0.4.7"
+authors = [
+  { name="Nazchanel", email="eshaniyer@duck.com" },
+]
+description = "This is a simple API to access the Home Access Center (HAC)"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Nazchanel/hac-api"
```

### Comparing `hacapi-0.4.6/src/hacapi/assignment_grades.py` & `hacapi-0.4.7/src/hacapi/assignment_grades.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import pandas as pd
-from . import session
-from . import payloads
-
-
-def return_quarter_assignments_html(quarter):
-    session_requests = session.session_requests
-
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
-
-    payload = {}
-
-    if quarter == 1:
-        payload = payloads.payload1
-    elif quarter == 2:
-        payload = payloads.payload2
-    elif quarter == 3:
-        payload = payloads.payload3
-    elif quarter == 4:
-        payload = payloads.payload4
-
-    specific_quarter = session_requests.post(urls, data=payload, headers=dict(referer=urls))
-
-    df = pd.read_html(specific_quarter.text)
-    index_list = []
-
-    for i in range(len(df)):
-        if len(df[i].columns) == 10:
-            index_list.append(i)
-
-    html_list = []
-
-    for i in index_list:
-        html_list.append(df[i].to_html())
-
-    return html_list
-
-
-def return_quarter_assignments_df(quarter):
-    session_requests = session.session_requests
-
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
-
-    payload = {}
-    if quarter == 1:
-        payload = payloads.payload1
-    elif quarter == 2:
-        payload = payloads.payload2
-    elif quarter == 3:
-        payload = payloads.payload3
-    elif quarter == 4:
-        payload = payloads.payload4
-
-    specific_quarter = session_requests.post(urls, data=payload, headers=dict(referer=urls))
-    df = pd.read_html(specific_quarter.text)
-
-    index_list = []
-    df_list = []
-
-    for i in range(len(df)):
-        if len(df[i].columns) == 10:
-            index_list.append(i)
-
-    for i in index_list:
-        df_list.append(df[i])
-
-    return df_list
-
-
-def return_current_assignments_df():
-    session_requests = session.session_requests
-    session.return_to_current()
-
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
-
-    result = session_requests.get(urls, headers=dict(referer=urls))
-    df = pd.read_html(result.text)
-
-    index_list = []
-    df_list = []
-
-    for i in range(len(df)):
-        if len(df[i].columns) == 10:
-            index_list.append(i)
-
-    for i in index_list:
-        df_list.append(df[i])
-
-    return df_list
-
-
-def return_current_assignments_html():
-    session_requests = session.session_requests
-    session.return_to_current()
-
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
-
-    result = session_requests.get(urls, headers=dict(referer=urls))
-    df = pd.read_html(result.text)
-
-    index_list = []
-    df_list = []
-
-    for i in range(len(df)):
-        if len(df[i].columns) == 10:
-            index_list.append(i)
-
-    for i in index_list:
-        df_list.append(df[i])
-
-    html_list = []
-
-    for i in index_list:
-        html_list.append(df[i].to_html())
-
-    return html_list
+import pandas as pd
+from . import session
+from . import payloads
+
+
+def return_quarter_assignments_html(quarter):
+    session_requests = session.session_requests
+
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
+
+    payload = {}
+
+    if quarter == 1:
+        payload = payloads.payload1
+    elif quarter == 2:
+        payload = payloads.payload2
+    elif quarter == 3:
+        payload = payloads.payload3
+    elif quarter == 4:
+        payload = payloads.payload4
+
+    specific_quarter = session_requests.post(urls, data=payload, headers=dict(referer=urls))
+
+    df = pd.read_html(specific_quarter.text)
+    index_list = []
+
+    for i in range(len(df)):
+        if len(df[i].columns) == 10:
+            index_list.append(i)
+
+    html_list = []
+
+    for i in index_list:
+        html_list.append(df[i].to_html())
+
+    return html_list
+
+
+def return_quarter_assignments_df(quarter):
+    session_requests = session.session_requests
+
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
+
+    payload = {}
+    if quarter == 1:
+        payload = payloads.payload1
+    elif quarter == 2:
+        payload = payloads.payload2
+    elif quarter == 3:
+        payload = payloads.payload3
+    elif quarter == 4:
+        payload = payloads.payload4
+
+    specific_quarter = session_requests.post(urls, data=payload, headers=dict(referer=urls))
+    df = pd.read_html(specific_quarter.text)
+
+    index_list = []
+    df_list = []
+
+    for i in range(len(df)):
+        if len(df[i].columns) == 10:
+            index_list.append(i)
+
+    for i in index_list:
+        df_list.append(df[i])
+
+    return df_list
+
+
+def return_current_assignments_df():
+    session_requests = session.session_requests
+    session.return_to_current()
+
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
+
+    result = session_requests.get(urls, headers=dict(referer=urls))
+    df = pd.read_html(result.text)
+
+    index_list = []
+    df_list = []
+
+    for i in range(len(df)):
+        if len(df[i].columns) == 10:
+            index_list.append(i)
+
+    for i in index_list:
+        df_list.append(df[i])
+
+    return df_list
+
+
+def return_current_assignments_html():
+    session_requests = session.session_requests
+    session.return_to_current()
+
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
+
+    result = session_requests.get(urls, headers=dict(referer=urls))
+    df = pd.read_html(result.text)
+
+    index_list = []
+    df_list = []
+
+    for i in range(len(df)):
+        if len(df[i].columns) == 10:
+            index_list.append(i)
+
+    for i in index_list:
+        df_list.append(df[i])
+
+    html_list = []
+
+    for i in index_list:
+        html_list.append(df[i].to_html())
+
+    return html_list
```

### Comparing `hacapi-0.4.6/src/hacapi/course_grades.py` & `hacapi-0.4.7/src/hacapi/course_grades.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-from . import session
-from bs4 import BeautifulSoup
-from . import payloads
-
-
-def _return_html():
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
-
-    session_requests = session.session_requests
-
-    result = session_requests.get(urls, headers=dict(referer=urls))
-
-    soup = BeautifulSoup(result.text, "html.parser")
-
-    grades_html = soup.find_all(class_="sg-header-heading sg-right")
-
-    name_html = soup.findAll('a', {"class": ["sg-header-heading"]})
-
-    return grades_html, name_html
-
-
-# Function that only works internally and not meant to be accessed by the user
-def _initialize_classes(grades_html, names_html):
-    class1 = 0
-    try:
-        class1 = str(grades_html[0])
-        class1 = class1[116:121]
-    except IndexError:
-        print("Enter a valid six digit Student ID and password!")
-        exit(0)
-
-    class2 = "0"
-    try:
-        class2 = str(grades_html[1])
-        class2 = class2[116:121]
-        if class2 == "":
-            class2 = "0"
-    except IndexError:
-        pass
-
-    class3 = "0"
-    try:
-        class3 = str(grades_html[2])
-        class3 = class3[116:121]
-        if class3 == "":
-            class3 = "0"
-    except IndexError:
-        pass
-
-    class4 = "0"
-    try:
-        class4 = str(grades_html[3])
-        class4 = class4[116:121]
-        if class4 == "":
-            class4 = "0"
-    except IndexError:
-        pass
-
-    class5 = "0"
-    try:
-        class5 = str(grades_html[4])
-        class5 = class5[116:121]
-        if class5 == "":
-            class5 = "0"
-    except IndexError:
-        pass
-
-    class6 = "0"
-    try:
-        class6 = str(grades_html[5])
-        class6 = class6[116:121]
-        if class6 == "":
-            class6 = "0"
-    except IndexError:
-        pass
-
-    class7 = "0"
-    try:
-        class7 = str(grades_html[6])
-        class7 = class7[116:121]
-        if class7 == "":
-            class7 = "0"
-    except IndexError:
-        pass
-
-    class8 = "0"
-    try:
-        class8 = str(grades_html[7])
-        class8 = class8[116:121]
-        if class8 == "":
-            class8 = "0"
-    except IndexError:
-        pass
-
-    class_name_1 = "No class"
-    try:
-        class_name_1 = (str(names_html[0].text)).strip()
-        index_of_deletion = class_name_1.index("-")
-        class_name_1 = (class_name_1[index_of_deletion + 4:]).strip()
-    except IndexError:
-        pass
-
-    class_name_2 = "No class"
-    try:
-        class_name_2 = (str(names_html[1].text)).strip()
-        index_of_deletion = class_name_2.index("-")
-        class_name_2 = (class_name_2[index_of_deletion + 4:]).strip()
-    except IndexError:
-        pass
-
-    class_name_3 = "No class"
-    try:
-        class_name_3 = (str(names_html[2].text)).strip()
-        index_of_deletion = class_name_3.index("-")
-        class_name_3 = (class_name_3[index_of_deletion + 4:]).strip()
-    except IndexError:
-        pass
-
-    class_name_4 = "No class"
-    try:
-        class_name_4 = (str(names_html[3].text)).strip()
-        index_of_deletion = class_name_4.index("-")
-        class_name_4 = (class_name_4[index_of_deletion + 4:]).strip()
-    except IndexError:
-        pass
-    class_name_5 = "No class"
-    try:
-        class_name_5 = (str(names_html[4].text)).strip()
-        dash_index = class_name_5.index("-")
-        class_name_5 = (class_name_5[dash_index + 4:]).strip()
-    except IndexError:
-        pass
-
-    class_name_6 = "No class"
-    try:
-        class_name_6 = (str(names_html[5].text)).strip()
-        dash_index = class_name_6.index("-")
-        class_name_6 = (class_name_6[dash_index + 4:]).strip()
-    except IndexError:
-        pass
-
-    class_name_7 = "No class"
-    try:
-        class_name_7 = (str(names_html[6].text)).strip()
-        dash_index = class_name_7.index("-")
-        class_name_7 = (class_name_7[dash_index + 4:]).strip()
-    except IndexError:
-        pass
-
-    class_name_8 = "No class"
-    try:
-        class_name_8 = (str(names_html[7].text)).strip()
-        dash_index = class_name_8.index("-")
-        class_name_8 = (class_name_8[dash_index + 4:]).strip()
-    except IndexError:
-        pass
-
-    return [class_name_1, class_name_2, class_name_3, class_name_4, class_name_5, class_name_6, class_name_7,
-            class_name_8], [class1, class2, class3, class4, class5, class6, class7, class8]
-
-
-def return_current_grades():
-    # Creates a session to maintain credentials
-
-    session.return_to_current()
-
-    html = _return_html()
-
-    grades_html = html[0]
-    name_html = html[1]
-
-    classes = _initialize_classes(grades_html, name_html)
-
-    class_names = classes[0]
-    class_grades = classes[1]
-
-    try:
-        class_grades_ = [i.replace("%", "") for i in class_grades]
-    except:
-        class_grades_ = 0
-        print("FAILURE")
-
-    class_grades = []
-    for i in class_grades_:  # type: ignore
-        try:
-            class_grades.append(float(i))
-        except:
-            print("\n" + "ERROR: " + "Could not convert " + i + " to a float." + "\n")
-            class_grades.append(float(0))
-
-    names_ = []
-    grades_ = []
-
-    for i in range(len(class_names)):
-        names_.append(class_names[i])
-        grades_.append(class_grades[i])
-
-    return (names_, grades_)
-
-
-def return_quarter_grade(quarter):
-    session_requests = session.session_requests
-
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
-
-    payload = {}
-    if quarter == 1:
-        payload = payloads.payload1
-    elif quarter == 2:
-        payload = payloads.payload2
-    elif quarter == 3:
-        payload = payloads.payload3
-    elif quarter == 4:
-        payload = payloads.payload4
-
-    specific_quarter = session_requests.post(urls, data=payload, headers=dict(referer=urls))
-
-    soup = BeautifulSoup(specific_quarter.text, "html.parser")
-
-    grades_html = soup.find_all(class_="sg-header-heading sg-right")
-
-    name_html = soup.findAll('a', {"class": ["sg-header-heading"]})
-
-    classes = _initialize_classes(grades_html, name_html)
-
-    class_names = classes[0]
-    class_grades = classes[1]
-
-    try:
-        class_grades_ = [i.replace("%", "") for i in class_grades]
-    except:
-        class_grades_ = 0
-        print("FAILURE")
-
-    class_grades = []
-    for i in class_grades_:  # type: ignore
-        try:
-            class_grades.append(float(i))
-        except:
-            print("\n" + "ERROR: " + "Could not convert " + i + " to a float." + "\n")
-            class_grades.append(float(0))
-
-    names_ = []
-    grades_ = []
-
-    for i in range(len(class_names)):
-        names_.append(class_names[i])
-        grades_.append(class_grades[i])
-
-    return names_, grades_
+from . import session
+from bs4 import BeautifulSoup
+from . import payloads
+
+
+def _return_html():
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
+
+    session_requests = session.session_requests
+
+    result = session_requests.get(urls, headers=dict(referer=urls))
+
+    soup = BeautifulSoup(result.text, "html.parser")
+
+    grades_html = soup.find_all(class_="sg-header-heading sg-right")
+
+    name_html = soup.findAll('a', {"class": ["sg-header-heading"]})
+
+    return grades_html, name_html
+
+
+# Function that only works internally and not meant to be accessed by the user
+def _initialize_classes(grades_html, names_html):
+    class1 = 0
+    try:
+        class1 = str(grades_html[0])
+        class1 = class1[116:121]
+    except IndexError:
+        print("Enter a valid six digit Student ID and password!")
+        exit(0)
+
+    class2 = "0"
+    try:
+        class2 = str(grades_html[1])
+        class2 = class2[116:121]
+        if class2 == "":
+            class2 = "0"
+    except IndexError:
+        pass
+
+    class3 = "0"
+    try:
+        class3 = str(grades_html[2])
+        class3 = class3[116:121]
+        if class3 == "":
+            class3 = "0"
+    except IndexError:
+        pass
+
+    class4 = "0"
+    try:
+        class4 = str(grades_html[3])
+        class4 = class4[116:121]
+        if class4 == "":
+            class4 = "0"
+    except IndexError:
+        pass
+
+    class5 = "0"
+    try:
+        class5 = str(grades_html[4])
+        class5 = class5[116:121]
+        if class5 == "":
+            class5 = "0"
+    except IndexError:
+        pass
+
+    class6 = "0"
+    try:
+        class6 = str(grades_html[5])
+        class6 = class6[116:121]
+        if class6 == "":
+            class6 = "0"
+    except IndexError:
+        pass
+
+    class7 = "0"
+    try:
+        class7 = str(grades_html[6])
+        class7 = class7[116:121]
+        if class7 == "":
+            class7 = "0"
+    except IndexError:
+        pass
+
+    class8 = "0"
+    try:
+        class8 = str(grades_html[7])
+        class8 = class8[116:121]
+        if class8 == "":
+            class8 = "0"
+    except IndexError:
+        pass
+
+    class_name_1 = "No class"
+    try:
+        class_name_1 = (str(names_html[0].text)).strip()
+        index_of_deletion = class_name_1.index("-")
+        class_name_1 = (class_name_1[index_of_deletion + 4:]).strip()
+    except IndexError:
+        pass
+
+    class_name_2 = "No class"
+    try:
+        class_name_2 = (str(names_html[1].text)).strip()
+        index_of_deletion = class_name_2.index("-")
+        class_name_2 = (class_name_2[index_of_deletion + 4:]).strip()
+    except IndexError:
+        pass
+
+    class_name_3 = "No class"
+    try:
+        class_name_3 = (str(names_html[2].text)).strip()
+        index_of_deletion = class_name_3.index("-")
+        class_name_3 = (class_name_3[index_of_deletion + 4:]).strip()
+    except IndexError:
+        pass
+
+    class_name_4 = "No class"
+    try:
+        class_name_4 = (str(names_html[3].text)).strip()
+        index_of_deletion = class_name_4.index("-")
+        class_name_4 = (class_name_4[index_of_deletion + 4:]).strip()
+    except IndexError:
+        pass
+    class_name_5 = "No class"
+    try:
+        class_name_5 = (str(names_html[4].text)).strip()
+        dash_index = class_name_5.index("-")
+        class_name_5 = (class_name_5[dash_index + 4:]).strip()
+    except IndexError:
+        pass
+
+    class_name_6 = "No class"
+    try:
+        class_name_6 = (str(names_html[5].text)).strip()
+        dash_index = class_name_6.index("-")
+        class_name_6 = (class_name_6[dash_index + 4:]).strip()
+    except IndexError:
+        pass
+
+    class_name_7 = "No class"
+    try:
+        class_name_7 = (str(names_html[6].text)).strip()
+        dash_index = class_name_7.index("-")
+        class_name_7 = (class_name_7[dash_index + 4:]).strip()
+    except IndexError:
+        pass
+
+    class_name_8 = "No class"
+    try:
+        class_name_8 = (str(names_html[7].text)).strip()
+        dash_index = class_name_8.index("-")
+        class_name_8 = (class_name_8[dash_index + 4:]).strip()
+    except IndexError:
+        pass
+
+    return [class_name_1, class_name_2, class_name_3, class_name_4, class_name_5, class_name_6, class_name_7,
+            class_name_8], [class1, class2, class3, class4, class5, class6, class7, class8]
+
+
+def return_current_grades():
+    # Creates a session to maintain credentials
+
+    session.return_to_current()
+
+    html = _return_html()
+
+    grades_html = html[0]
+    name_html = html[1]
+
+    classes = _initialize_classes(grades_html, name_html)
+
+    class_names = classes[0]
+    class_grades = classes[1]
+
+    try:
+        class_grades_ = [i.replace("%", "") for i in class_grades]
+    except:
+        class_grades_ = 0
+        print("FAILURE")
+
+    class_grades = []
+    for i in class_grades_:  # type: ignore
+        try:
+            class_grades.append(float(i))
+        except:
+            print("\n" + "ERROR: " + "Could not convert " + i + " to a float." + "\n")
+            class_grades.append(float(0))
+
+    names_ = []
+    grades_ = []
+
+    for i in range(len(class_names)):
+        names_.append(class_names[i])
+        grades_.append(class_grades[i])
+
+    return (names_, grades_)
+
+
+def return_quarter_grade(quarter):
+    session_requests = session.session_requests
+
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Assignments.aspx"
+
+    payload = {}
+    if quarter == 1:
+        payload = payloads.payload1
+    elif quarter == 2:
+        payload = payloads.payload2
+    elif quarter == 3:
+        payload = payloads.payload3
+    elif quarter == 4:
+        payload = payloads.payload4
+
+    specific_quarter = session_requests.post(urls, data=payload, headers=dict(referer=urls))
+
+    soup = BeautifulSoup(specific_quarter.text, "html.parser")
+
+    grades_html = soup.find_all(class_="sg-header-heading sg-right")
+
+    name_html = soup.findAll('a', {"class": ["sg-header-heading"]})
+
+    classes = _initialize_classes(grades_html, name_html)
+
+    class_names = classes[0]
+    class_grades = classes[1]
+
+    try:
+        class_grades_ = [i.replace("%", "") for i in class_grades]
+    except:
+        class_grades_ = 0
+        print("FAILURE")
+
+    class_grades = []
+    for i in class_grades_:  # type: ignore
+        try:
+            class_grades.append(float(i))
+        except:
+            print("\n" + "ERROR: " + "Could not convert " + i + " to a float." + "\n")
+            class_grades.append(float(0))
+
+    names_ = []
+    grades_ = []
+
+    for i in range(len(class_names)):
+        names_.append(class_names[i])
+        grades_.append(class_grades[i])
+
+    return names_, grades_
```

### Comparing `hacapi-0.4.6/src/hacapi/payloads.py` & `hacapi-0.4.7/src/hacapi/payloads.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-payload1 = {
-    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
-    "__EVENTARGUMENT": "",
-    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
-    "__VIEWSTATEGENERATOR": "B0093F3C",
-    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
-    "ctl00$plnMain$hdnValidMHACLicense": "Y",
-    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
-    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
-    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
-    "ctl00$plnMain$hdnTitle": "Classwork",
-    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
-    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
-    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
-    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
-    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
-    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
-    "ctl00$plnMain$hdnCompCourse": "Course",
-    "ctl00$plnMain$hdnCompAssignment": "Assignment",
-    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
-    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
-    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
-    "ctl00$plnMain$hdnCompScore": "Score",
-    "ctl00$plnMain$hdnCompPoints": "Points",
-    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
-    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
-    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
-    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
-    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
-    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
-    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
-    "ctl00$plnMain$hdnCollapse": "Collapse+All",
-    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
-    "ctl00$plnMain$hdnViewFull": "Full+View",
-    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
-    "ctl00$plnMain$hdnViewQuick": "Quick+View",
-    "ctl00$plnMain$hdnExpand": "Expand+All",
-    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
-    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
-    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
-    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
-    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
-    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
-    "ctl00$plnMain$hdnTooltipTitle": "Title",
-    "ctl00$plnMain$hdnCategory": "Category",
-    "ctl00$plnMain$hdnDueDate": "Due+Date",
-    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
-    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
-    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
-    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
-    "ctl00$plnMain$hdnType": "Type",
-    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
-    "ctl00$plnMain$ddlReportCardRuns": "1-2023",
-    "ctl00$plnMain$ddlClasses": "ALL",
-    "ctl00$plnMain$ddlCompetencies": "ALL",
-    "ctl00$plnMain$ddlOrderBy": "Class"
-}
-
-payload2 = {
-    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
-    "__EVENTARGUMENT": "",
-    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
-    "__VIEWSTATEGENERATOR": "B0093F3C",
-    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
-    "ctl00$plnMain$hdnValidMHACLicense": "Y",
-    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
-    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
-    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
-    "ctl00$plnMain$hdnTitle": "Classwork",
-    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
-    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
-    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
-    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
-    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
-    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
-    "ctl00$plnMain$hdnCompCourse": "Course",
-    "ctl00$plnMain$hdnCompAssignment": "Assignment",
-    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
-    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
-    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
-    "ctl00$plnMain$hdnCompScore": "Score",
-    "ctl00$plnMain$hdnCompPoints": "Points",
-    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
-    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
-    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
-    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
-    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
-    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
-    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
-    "ctl00$plnMain$hdnCollapse": "Collapse+All",
-    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
-    "ctl00$plnMain$hdnViewFull": "Full+View",
-    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
-    "ctl00$plnMain$hdnViewQuick": "Quick+View",
-    "ctl00$plnMain$hdnExpand": "Expand+All",
-    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
-    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
-    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
-    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
-    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
-    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
-    "ctl00$plnMain$hdnTooltipTitle": "Title",
-    "ctl00$plnMain$hdnCategory": "Category",
-    "ctl00$plnMain$hdnDueDate": "Due+Date",
-    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
-    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
-    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
-    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
-    "ctl00$plnMain$hdnType": "Type",
-    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
-    "ctl00$plnMain$ddlReportCardRuns": "2-2023",
-    "ctl00$plnMain$ddlClasses": "ALL",
-    "ctl00$plnMain$ddlCompetencies": "ALL",
-    "ctl00$plnMain$ddlOrderBy": "Class"
-}
-payload3 = {
-    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
-    "__EVENTARGUMENT": "",
-    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
-    "__VIEWSTATEGENERATOR": "B0093F3C",
-    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
-    "ctl00$plnMain$hdnValidMHACLicense": "Y",
-    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
-    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
-    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
-    "ctl00$plnMain$hdnTitle": "Classwork",
-    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
-    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
-    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
-    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
-    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
-    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
-    "ctl00$plnMain$hdnCompCourse": "Course",
-    "ctl00$plnMain$hdnCompAssignment": "Assignment",
-    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
-    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
-    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
-    "ctl00$plnMain$hdnCompScore": "Score",
-    "ctl00$plnMain$hdnCompPoints": "Points",
-    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
-    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
-    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
-    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
-    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
-    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
-    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
-    "ctl00$plnMain$hdnCollapse": "Collapse+All",
-    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
-    "ctl00$plnMain$hdnViewFull": "Full+View",
-    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
-    "ctl00$plnMain$hdnViewQuick": "Quick+View",
-    "ctl00$plnMain$hdnExpand": "Expand+All",
-    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
-    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
-    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
-    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
-    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
-    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
-    "ctl00$plnMain$hdnTooltipTitle": "Title",
-    "ctl00$plnMain$hdnCategory": "Category",
-    "ctl00$plnMain$hdnDueDate": "Due+Date",
-    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
-    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
-    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
-    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
-    "ctl00$plnMain$hdnType": "Type",
-    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
-    "ctl00$plnMain$ddlReportCardRuns": "3-2023",
-    "ctl00$plnMain$ddlClasses": "ALL",
-    "ctl00$plnMain$ddlCompetencies": "ALL",
-    "ctl00$plnMain$ddlOrderBy": "Class"
-}
-payload4 = {
-    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
-    "__EVENTARGUMENT": "",
-    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
-    "__VIEWSTATEGENERATOR": "B0093F3C",
-    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
-    "ctl00$plnMain$hdnValidMHACLicense": "Y",
-    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
-    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
-    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
-    "ctl00$plnMain$hdnTitle": "Classwork",
-    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
-    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
-    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
-    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
-    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
-    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
-    "ctl00$plnMain$hdnCompCourse": "Course",
-    "ctl00$plnMain$hdnCompAssignment": "Assignment",
-    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
-    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
-    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
-    "ctl00$plnMain$hdnCompScore": "Score",
-    "ctl00$plnMain$hdnCompPoints": "Points",
-    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
-    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
-    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
-    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
-    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
-    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
-    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
-    "ctl00$plnMain$hdnCollapse": "Collapse+All",
-    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
-    "ctl00$plnMain$hdnViewFull": "Full+View",
-    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
-    "ctl00$plnMain$hdnViewQuick": "Quick+View",
-    "ctl00$plnMain$hdnExpand": "Expand+All",
-    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
-    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
-    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
-    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
-    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
-    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
-    "ctl00$plnMain$hdnTooltipTitle": "Title",
-    "ctl00$plnMain$hdnCategory": "Category",
-    "ctl00$plnMain$hdnDueDate": "Due+Date",
-    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
-    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
-    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
-    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
-    "ctl00$plnMain$hdnType": "Type",
-    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
-    "ctl00$plnMain$ddlReportCardRuns": "4-2023",
-    "ctl00$plnMain$ddlClasses": "ALL",
-    "ctl00$plnMain$ddlCompetencies": "ALL",
-    "ctl00$plnMain$ddlOrderBy": "Class"
-}
+payload1 = {
+    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
+    "__EVENTARGUMENT": "",
+    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
+    "__VIEWSTATEGENERATOR": "B0093F3C",
+    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
+    "ctl00$plnMain$hdnValidMHACLicense": "Y",
+    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
+    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
+    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
+    "ctl00$plnMain$hdnTitle": "Classwork",
+    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
+    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
+    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
+    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
+    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
+    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
+    "ctl00$plnMain$hdnCompCourse": "Course",
+    "ctl00$plnMain$hdnCompAssignment": "Assignment",
+    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
+    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
+    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
+    "ctl00$plnMain$hdnCompScore": "Score",
+    "ctl00$plnMain$hdnCompPoints": "Points",
+    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
+    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
+    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
+    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
+    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
+    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
+    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
+    "ctl00$plnMain$hdnCollapse": "Collapse+All",
+    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
+    "ctl00$plnMain$hdnViewFull": "Full+View",
+    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
+    "ctl00$plnMain$hdnViewQuick": "Quick+View",
+    "ctl00$plnMain$hdnExpand": "Expand+All",
+    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
+    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
+    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
+    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
+    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
+    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
+    "ctl00$plnMain$hdnTooltipTitle": "Title",
+    "ctl00$plnMain$hdnCategory": "Category",
+    "ctl00$plnMain$hdnDueDate": "Due+Date",
+    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
+    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
+    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
+    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
+    "ctl00$plnMain$hdnType": "Type",
+    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
+    "ctl00$plnMain$ddlReportCardRuns": "1-2023",
+    "ctl00$plnMain$ddlClasses": "ALL",
+    "ctl00$plnMain$ddlCompetencies": "ALL",
+    "ctl00$plnMain$ddlOrderBy": "Class"
+}
+
+payload2 = {
+    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
+    "__EVENTARGUMENT": "",
+    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
+    "__VIEWSTATEGENERATOR": "B0093F3C",
+    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
+    "ctl00$plnMain$hdnValidMHACLicense": "Y",
+    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
+    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
+    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
+    "ctl00$plnMain$hdnTitle": "Classwork",
+    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
+    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
+    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
+    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
+    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
+    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
+    "ctl00$plnMain$hdnCompCourse": "Course",
+    "ctl00$plnMain$hdnCompAssignment": "Assignment",
+    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
+    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
+    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
+    "ctl00$plnMain$hdnCompScore": "Score",
+    "ctl00$plnMain$hdnCompPoints": "Points",
+    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
+    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
+    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
+    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
+    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
+    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
+    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
+    "ctl00$plnMain$hdnCollapse": "Collapse+All",
+    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
+    "ctl00$plnMain$hdnViewFull": "Full+View",
+    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
+    "ctl00$plnMain$hdnViewQuick": "Quick+View",
+    "ctl00$plnMain$hdnExpand": "Expand+All",
+    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
+    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
+    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
+    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
+    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
+    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
+    "ctl00$plnMain$hdnTooltipTitle": "Title",
+    "ctl00$plnMain$hdnCategory": "Category",
+    "ctl00$plnMain$hdnDueDate": "Due+Date",
+    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
+    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
+    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
+    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
+    "ctl00$plnMain$hdnType": "Type",
+    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
+    "ctl00$plnMain$ddlReportCardRuns": "2-2023",
+    "ctl00$plnMain$ddlClasses": "ALL",
+    "ctl00$plnMain$ddlCompetencies": "ALL",
+    "ctl00$plnMain$ddlOrderBy": "Class"
+}
+payload3 = {
+    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
+    "__EVENTARGUMENT": "",
+    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
+    "__VIEWSTATEGENERATOR": "B0093F3C",
+    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
+    "ctl00$plnMain$hdnValidMHACLicense": "Y",
+    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
+    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
+    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
+    "ctl00$plnMain$hdnTitle": "Classwork",
+    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
+    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
+    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
+    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
+    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
+    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
+    "ctl00$plnMain$hdnCompCourse": "Course",
+    "ctl00$plnMain$hdnCompAssignment": "Assignment",
+    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
+    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
+    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
+    "ctl00$plnMain$hdnCompScore": "Score",
+    "ctl00$plnMain$hdnCompPoints": "Points",
+    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
+    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
+    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
+    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
+    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
+    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
+    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
+    "ctl00$plnMain$hdnCollapse": "Collapse+All",
+    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
+    "ctl00$plnMain$hdnViewFull": "Full+View",
+    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
+    "ctl00$plnMain$hdnViewQuick": "Quick+View",
+    "ctl00$plnMain$hdnExpand": "Expand+All",
+    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
+    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
+    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
+    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
+    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
+    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
+    "ctl00$plnMain$hdnTooltipTitle": "Title",
+    "ctl00$plnMain$hdnCategory": "Category",
+    "ctl00$plnMain$hdnDueDate": "Due+Date",
+    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
+    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
+    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
+    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
+    "ctl00$plnMain$hdnType": "Type",
+    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
+    "ctl00$plnMain$ddlReportCardRuns": "3-2023",
+    "ctl00$plnMain$ddlClasses": "ALL",
+    "ctl00$plnMain$ddlCompetencies": "ALL",
+    "ctl00$plnMain$ddlOrderBy": "Class"
+}
+payload4 = {
+    "__EVENTTARGET": "ctl00$plnMain$btnRefreshView",
+    "__EVENTARGUMENT": "",
+    "__VIEWSTATE": "LRf+wOXUedofP2GXepyNnLu2T3yZB/hXvZWdk9Kn0FgOOLn2hNRCWcsMGX9i8HXRxFFOllwOBJAo3wNeIUQohA8X2EP15vOa7wouvmmQCtjenb5y+zAYZ+t6X2fJ3ahbROxO9egG/OlMRArr7oDV5zSjMMSS9QHTJZ5JWWBqXMlDAae7x1cDWpoKH9+OWi6bWIBo4FEEui9Yfp8j4ulyv6oD+WGa7206s0QdZIKw/9nYrl/pomeZBR25b4CGQkLkMB9bRBd+bmAIxeIQkz2GySKFLbo0lNcSxsSezNhJFLxjD5C5Bv4sKjAeMXpY3W4ybM4zYk+Nb5JTR8nmVEWTf6ED0yrwdOtyxMAs6i0cQV9G1I1LRxjrunLXRY7HQD+XgCbB0sSqPp2UhmggTc/4cIgnhKrldy8DPNMFPFlxanqrT6s9ly8DGKE/mx0C0bWki46jctPyhdzh2EOMtUZ7EacN/Oy/co+ttEi3jH63X5OFt7ystua1hd8lCvsNBtEBMK73GugoyX5rEmF2dQacZU6GLdeIafj3h0kDHZJ9m8jWcE9in/peQZCbomEqP5FuRXegtNLnG6FICxa+l5gvg7WtJf0PUgNb3B8l1bEA0YML/ceoNXDPcBAHEyUvDMZQAxp3uqoZfp958gD7m1TAH5U3Hkzc3NLcsyLPOUHGOrbv+uC4OBH8Fs3vIXO1csYw9bX/VT3HwGWeS/A/KVmCm6/u8I6+3ddjW4hTLYCG6USFiYzkmWVVYLbh2/G+OTDY0I14ALQycZWgKSTbnKZHj3TeONM049Rcb32iKCOawwuDmDu3FwLveEARuUmyV822Flo1g84kDTn9yq3xQ46WdHtPfmcGQ2OIUizxfRtuMPmtdq+OTVnsVwxrSzez1SnCF2+TLOfCzZqPRdPGdcvv0RFQrO88vfHYXlEHW4Wxdc3bQr4GexJ6upQn2w+XPwPYN/aOjhxRflU2/Llig8lj//IhIIo4SAWP9Hw/+2f3kGZD8BVq3rnLHx/I9hsaco0NEVJCGHh4e1HLtwI6GDRc+pG+LFtsNzHgmzIVPvJR0lFI4dEMlgOmmizFn9jGC/1jBlybTI8VvUlewWy7efKuQHghe/etKvZlXEFN06I9Gtb0go+gGDLOn6Nk9iAbmVhEFVl8idqlgDtmllaAA8mmtxsjJNZDLS6k4+zMHosBCBt6Lr5H7rqWpmkhEDLXBf6leuyQmS7Ss4Nm3fOj3VKz3uPyM4svhsTXtiSetL4otySuXxISGtQSiiDlncVcbuS54dVVr7aYFu98Ig+ceCGwc0aieZ7nQFQzh+ZEF6iQL191cSPhoTv7BjVgykm2sJ+EJiB55oXo6MXJPGtFSSwVL5622tKyoYBJTMyNqPzccWm8pfw7F7faADb8P1DbRzIzAg8tYlgJjhaaZkoVZ5vRjp+muxwibvmcw0muxtsbfabZMNyvKFvEZOcdqryK7bNOZLXMJWCoX9VOa6Ufp23n/H9wm5DVXUHd47nrTpwiZy1YWL9jnHK99+egr3AlfSW4JYo5xg8pvvJrp6+cpxjCFyD9/ncZ1i+iDemikl0xH+WqI0ZdwqXyF4UzCHtoTtqoDZxsQgW6GJSGDXZlkgqvUlj6TW0ifiBrSHLimLsDAymDeeL6OG3Yca/MNTfglFThARPOyPLEti2bwaQcSICbgJBE/rkAjEn2mPRYBfP9aXeva+VhgGTTyMQEumE4wohJdJroKjWUNwQr5Uj81Qyard+232jB3Kj7VpJGnDWVPBEo78Wx6VOgdpBzfjy+DWQ2",
+    "__VIEWSTATEGENERATOR": "B0093F3C",
+    "__EVENTVALIDATION": "DZEJfusFrl7Z1ATA5SedL/JvraKhkPy0z8uzyF0TAZ2CBrL2bhhkxq5Ku4vFOau91V2Dv1XrN0V/Rtdn6aRZfwi6ufwMP0L//GI2cYQdOnM7ku9whPdSxn/XAZJjhb3qoSIWEXn1NXOdSbyqGvYlUQy8oA8ZS68qREtzkUejmFwGpJztKAcS3vdlXicScKFtVt0sPDY87SbenJIloN0M8WhDA5o6e8UgfPF4H2xyZhs00929Qk1MYB/OV7aobj7bGWzWY0tbXN89oiPcrXOHK+n0OEWeSm3KDcEMf8N9wlmniLmbhqKvCerK2SmGa3Ug/boHMBWdIXEv+kJ1gJ7W2WAF5IpGxMql1DFKOSH572eaLMou4AppkB4PYWkVm7bqshougizLS7pLK22N/+rjmFhsdthyqYfVonA00SqTjnI7bkAOxFCG8OPOyYyZzXfuxpIhBEeEG/ala6sftfL5Y3nN9cqhq/4iYF4MjjtmuhWQgikCveCHuB3j2iKUf17ZoB9nuTmciacsA0Sk0v6I/MU8Rub6cb78lR+j6dLei/z+fg4ZCkOCxEgPE8XERCkCrY8zNSfquLBDMoz5lX2ukhdRgZIfITePSSooVsl61e7EDrV0CA6cg4i0gg5btuvK5RNnmnlJRI8nheKlikgw2F4ru+dYMa+i1tR1nWmH0fqmEjF6vTuWWTbBL9EoK5ZKHd5Xm4i4OC3GQWQ4TerRoInIRQDUufmG4IRFCXqsLJiQvmNIeP7HLDUM/FXDVoEdRN2pNCCX56AwdPsGXIsI6I5/Lqwwg3sNHIZ6CoB2Yy8XcaHCtF0vWGedD2h1t7APAYCGwEq+j+hWz5hEGkroFODKGAw82GZ7UvrnSWRBICkapeiWw+Wq6T+8igbtT0iVft52m7khLK5+dZ0fHNM31HBl0nkkGpgJed3DzTWh6GR+hOp3UD4I1xJUJfHDEfGyeHLb9cLMKoP2Kp35mwU5sQzi7wgET6mwU+i6jwRD9YGX28lqaB2qdqJfn1DyurUEZVdbPyXfmhHqz4ulT3gG2ZKundhytRjcCXhuwwKM7Gh7t/mmzDalXIgUFffeF139dWULIjffcpvuU5obcfMILEjG/S/wOFGuXotPNTOxqGbprcT/ThTkx2c5O46V+rgOvLdYSpZFJurayO1h7/9BNdguYsk+zjnMG495qE9gpPJkFXEGVJlYyhYRWh9ut/FQSFbUWMgLJBJkkY/TnbTB4ffyHCJMuoa+dhNQUF7HzBvXu3SeJpOJPMtdhciZWceOnoxwjw9nO1BrkQ+521bsYpoNXLRtmN1OBGG5HIgjEW2dQ7nepSRWPtygCHrpIoNcFcNJ0VF2HVjU6SiWGdS4Z9Fw4Bk8mxjBYqX4dBPsZrZKiPz+/p08uDYSdcwZl1C1kB+HtZ9GH3LgNEU1FZi6iJil6yenKP4Dhr/JFRSWxSNePyb3fFWJe9p3psdBYwnZvvcOkDchRzx6+C8WO/0HtKS5zYUeKg5Ztcx1nAHWuMpuxaB4WnRLmtN9aJJ3XNUetzmqXHsmtK+Jfh7jXZBtVNSk3XltHWMOcBUhQo0U8+PvduFdaaQcUgKZMuVbeU+usA0Yj9+RGMEt2PudFTngmYDm30J6TyYMu+J3yOkKeok=",
+    "ctl00$plnMain$hdnValidMHACLicense": "Y",
+    "ctl00$plnMain$hdnIsVisibleClsWrk": "N",
+    "ctl00$plnMain$hdnIsVisibleCrsAvg": "N",
+    "ctl00$plnMain$hdnJsAlert": "Averages+cannot+be+displayed+when++Report+Card+Run+is+set+to+(All+Runs).",
+    "ctl00$plnMain$hdnTitle": "Classwork",
+    "ctl00$plnMain$hdnLastUpdated": "Last+Updated",
+    "ctl00$plnMain$hdnDroppedCourse": "+This+course+was+dropped+as+of+",
+    "ctl00$plnMain$hdnddlClasses": "(All+Classes)",
+    "ctl00$plnMain$hdnddlCompetencies": "(All+Classes)",
+    "ctl00$plnMain$hdnCompDateDue": "Date+Due",
+    "ctl00$plnMain$hdnCompDateAssigned": "Date+Assigned",
+    "ctl00$plnMain$hdnCompCourse": "Course",
+    "ctl00$plnMain$hdnCompAssignment": "Assignment",
+    "ctl00$plnMain$hdnCompAssignmentLabel": "Assignments+Not+Related+to+Any+Competency",
+    "ctl00$plnMain$hdnCompNoAssignments": "No+assignments+found",
+    "ctl00$plnMain$hdnCompNoClasswork": "Classwork+could+not+be+found+for+this+competency+for+the+selected+report+card+run.",
+    "ctl00$plnMain$hdnCompScore": "Score",
+    "ctl00$plnMain$hdnCompPoints": "Points",
+    "ctl00$plnMain$hdnddlReportCardRuns1": "(All+Runs)",
+    "ctl00$plnMain$hdnddlReportCardRuns2": "(All+Terms)",
+    "ctl00$plnMain$hdnbtnShowAverage": "Show+All+Averages",
+    "ctl00$plnMain$hdnShowAveragesToolTip": "Show+all+student's+averages",
+    "ctl00$plnMain$hdnPrintClassworkToolTip": "Print+all+classwork",
+    "ctl00$plnMain$hdnPrintClasswork": "Print+Classwork",
+    "ctl00$plnMain$hdnCollapseToolTip": "Collapse+all+courses",
+    "ctl00$plnMain$hdnCollapse": "Collapse+All",
+    "ctl00$plnMain$hdnFullToolTip": "Switch+courses+to+Full+View",
+    "ctl00$plnMain$hdnViewFull": "Full+View",
+    "ctl00$plnMain$hdnQuickToolTip": "Switch+courses+to+Quick+View",
+    "ctl00$plnMain$hdnViewQuick": "Quick+View",
+    "ctl00$plnMain$hdnExpand": "Expand+All",
+    "ctl00$plnMain$hdnExpandToolTip": "Expand+all+courses",
+    "ctl00$plnMain$hdnChildCompetencyMessage": "This+competency+is+calculated+as+an+average+of+the+following+competencies",
+    "ctl00$plnMain$hdnCompetencyScoreLabel": "Grade",
+    "ctl00$plnMain$hdnAverageDetailsDialogTitle": "Average+Details",
+    "ctl00$plnMain$hdnAssignmentCompetency": "Assignment+Competency",
+    "ctl00$plnMain$hdnAssignmentCourse": "Assignment+Course",
+    "ctl00$plnMain$hdnTooltipTitle": "Title",
+    "ctl00$plnMain$hdnCategory": "Category",
+    "ctl00$plnMain$hdnDueDate": "Due+Date",
+    "ctl00$plnMain$hdnMaxPoints": "Max+Points",
+    "ctl00$plnMain$hdnCanBeDropped": "Can+Be+Dropped",
+    "ctl00$plnMain$hdnHasAttachments": "Has+Attachments",
+    "ctl00$plnMain$hdnExtraCredit": "Extra+Credit",
+    "ctl00$plnMain$hdnType": "Type",
+    "ctl00$plnMain$hdnAssignmentDataInfo": "Information+could+not+be+found+for+the+assignment",
+    "ctl00$plnMain$ddlReportCardRuns": "4-2023",
+    "ctl00$plnMain$ddlClasses": "ALL",
+    "ctl00$plnMain$ddlCompetencies": "ALL",
+    "ctl00$plnMain$ddlOrderBy": "Class"
+}
```

### Comparing `hacapi-0.4.6/src/hacapi/transcript.py` & `hacapi-0.4.7/src/hacapi/transcript.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from . import session
-import pandas as pd
-import re
-
-
-def return_weighted_gpa():
-    session_requests = session.session_requests
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Transcript.aspx"
-
-    result = session_requests.get(urls, headers=dict(referer=urls))
-
-    df = pd.read_html(result.text)
-
-    gpa_text = df[0].loc[3, 0]
-
-    # Define a regular expression pattern to match the Weighted GPA
-    pattern = r'Weighted GPA\s+(\d+\.\d+)'
-    # Use re.search() to find the first occurrence of the pattern in the string
-    match = re.search(pattern, gpa_text)
-    # If a match was found, return the Weighted GPA as a float; otherwise, return None
-    return float(match.group(1)) if match else None
-
-
-def return_college_gpa():
-    session_requests = session.session_requests
-
-    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Transcript.aspx"
-
-    result = session_requests.get(urls, headers=dict(referer=urls))
-
-    df = pd.read_html(result.text)
-
-    gpa_text = df[0].loc[3, 0]
-    pattern = r'College GPA\s+(\d+\.\d+)'
-    match = re.search(pattern, gpa_text)
-    if match:
-        return float(match.group(1))
-    else:
-        return None
+from . import session
+import pandas as pd
+import re
+
+
+def return_weighted_gpa():
+    session_requests = session.session_requests
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Transcript.aspx"
+
+    result = session_requests.get(urls, headers=dict(referer=urls))
+
+    df = pd.read_html(result.text)
+
+    gpa_text = df[0].loc[3, 0]
+
+    # Define a regular expression pattern to match the Weighted GPA
+    pattern = r'Weighted GPA\s+(\d+\.\d+)'
+    # Use re.search() to find the first occurrence of the pattern in the string
+    match = re.search(pattern, gpa_text)
+    # If a match was found, return the Weighted GPA as a float; otherwise, return None
+    return float(match.group(1)) if match else None
+
+
+def return_college_gpa():
+    session_requests = session.session_requests
+
+    urls = "https://hac.friscoisd.org/HomeAccess/Content/Student/Transcript.aspx"
+
+    result = session_requests.get(urls, headers=dict(referer=urls))
+
+    df = pd.read_html(result.text)
+
+    gpa_text = df[0].loc[3, 0]
+    pattern = r'College GPA\s+(\d+\.\d+)'
+    match = re.search(pattern, gpa_text)
+    if match:
+        return float(match.group(1))
+    else:
+        return None
```

### Comparing `hacapi-0.4.6/src/hacapi.egg-info/PKG-INFO` & `hacapi-0.4.7/src/hacapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1
-Name: hacapi
-Version: 0.4.6
-Summary: This is a simple API to access the Home Access Center (HAC)
-Author-email: Nazchanel <eshaniyer@duck.com>
-Project-URL: Homepage, https://github.com/Nazchanel/hac-api
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# HAC API
-
-## Introduction
-
-This is a simple API to access the Home Access Center (HAC) of the [Frisco Independent School District](https://www.friscoisd.org/). This API is not affiliated with the school district in any way.
-
----
-
-## Modules
-
-### assignment_grades
-
-* return_quarter_assignments_html(***quarter***)
-* return_quarter_assignments_df(***quarter***)
-* return_current_assignments_df(    )
-* return_current_assignments_html(  )
-
-### course_grades
-
-* return_current_grades(  )
-* return_quarter_grade(***quarter***)
-
-### session
-
-* init(***username***, ***password***)
-* reset(    )
-* return_to_current(    )
-
-### transcript
-
-* return_weighted_gpa(  )
-* return_college_gpa(   )
-
-### misc
-
-* is_updated(***original***, ***new***)
-* get_time( )
-
----
+Metadata-Version: 2.1
+Name: hacapi
+Version: 0.4.7
+Summary: This is a simple API to access the Home Access Center (HAC)
+Author-email: Nazchanel <eshaniyer@duck.com>
+Project-URL: Homepage, https://github.com/Nazchanel/hac-api
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HAC API
+
+## Introduction
+
+This is a simple API to access the Home Access Center (HAC) of the [Frisco Independent School District](https://www.friscoisd.org/). This API is not affiliated with the school district in any way.
+
+---
+
+## Modules
+
+### assignment_grades
+
+* return_quarter_assignments_html(***quarter***)
+* return_quarter_assignments_df(***quarter***)
+* return_current_assignments_df(    )
+* return_current_assignments_html(  )
+
+### course_grades
+
+* return_current_grades(  )
+* return_quarter_grade(***quarter***)
+
+### session
+
+* init(***username***, ***password***)
+* reset(    )
+* return_to_current(    )
+
+### transcript
+
+* return_weighted_gpa(  )
+* return_college_gpa(   )
+
+### misc
+
+* is_updated(***original***, ***new***)
+* get_time( )
+
+---
```

