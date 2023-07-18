# Comparing `tmp/pyuploadcare-4.0.0.tar.gz` & `tmp/pyuploadcare-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuploadcare-4.0.0.tar", max compression
+gzip compressed data, was "pyuploadcare-4.1.0.tar", max compression
```

## Comparing `pyuploadcare-4.0.0.tar` & `pyuploadcare-4.1.0.tar`

### file list

```diff
@@ -1,62 +1,61 @@
--rw-r--r--   0        0        0     1082 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/LICENSE
--rw-r--r--   0        0        0     2820 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/README.md
--rw-r--r--   0        0        0     2331 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      439 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/__init__.py
--rw-r--r--   0        0        0      205 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/__init__.py
--rw-r--r--   0        0        0     3412 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/addon_entities.py
--rw-r--r--   0        0        0    17717 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/api.py
--rw-r--r--   0        0        0     2901 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/auth.py
--rw-r--r--   0        0        0     8261 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/base.py
--rw-r--r--   0        0        0     8512 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/client.py
--rw-r--r--   0        0        0     5772 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/entities.py
--rw-r--r--   0        0        0     1001 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/metadata.py
--rw-r--r--   0        0        0     2205 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/responses.py
--rw-r--r--   0        0        0      447 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/api/utils.py
--rw-r--r--   0        0        0    28141 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/client.py
--rw-r--r--   0        0        0      841 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/conf.py
--rw-r--r--   0        0        0      193 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/dj/__init__.py
--rw-r--r--   0        0        0      472 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/dj/client.py
--rw-r--r--   0        0        0     1510 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/dj/conf.py
--rw-r--r--   0        0        0     3611 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/dj/forms.py
--rw-r--r--   0        0        0     6211 2022-12-26 11:30:04.030620 pyuploadcare-4.0.0/pyuploadcare/dj/models.py
--rw-r--r--   0        0        0   384057 2022-12-26 11:30:04.034620 pyuploadcare-4.0.0/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js
--rw-r--r--   0        0        0   296023 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/dj/static/uploadcare/uploadcare.min.js
--rw-r--r--   0        0        0     2160 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/dj/subclassing.py
--rw-r--r--   0        0        0     1904 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/exceptions.py
--rw-r--r--   0        0        0     1288 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/helpers.py
--rw-r--r--   0        0        0        0 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/__init__.py
--rw-r--r--   0        0        0     2816 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/base.py
--rw-r--r--   0        0        0    18812 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/file.py
--rw-r--r--   0        0        0     6434 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/file_group.py
--rw-r--r--   0        0        0     2241 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/file_list.py
--rw-r--r--   0        0        0     1400 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/group_list.py
--rw-r--r--   0        0        0      730 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/resources/utils.py
--rw-r--r--   0        0        0     2336 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/secure_url.py
--rw-r--r--   0        0        0        0 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/transformations/__init__.py
--rw-r--r--   0        0        0     1305 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/transformations/base.py
--rw-r--r--   0        0        0      729 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/transformations/document.py
--rw-r--r--   0        0        0    10674 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/transformations/image.py
--rw-r--r--   0        0        0     1711 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/transformations/video.py
--rwxr-xr-x   0        0        0        0 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/__init__.py
--rw-r--r--   0        0        0     1394 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/convert_document.py
--rw-r--r--   0        0        0     1048 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/convert_video.py
--rw-r--r--   0        0        0      539 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/create_group.py
--rw-r--r--   0        0        0     1028 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/create_webhook.py
--rw-r--r--   0        0        0      984 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/delete_files.py
--rw-r--r--   0        0        0      398 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/delete_webhook.py
--rw-r--r--   0        0        0      439 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/get_file.py
--rw-r--r--   0        0        0      455 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/get_project.py
--rw-r--r--   0        0        0     3255 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/helpers.py
--rw-r--r--   0        0        0     1406 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/list_files.py
--rw-r--r--   0        0        0      934 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/list_groups.py
--rw-r--r--   0        0        0      450 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/list_webhooks.py
--rw-r--r--   0        0        0     1186 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/store_files.py
--rw-r--r--   0        0        0     8801 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/sync.py
--rw-r--r--   0        0        0     1484 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/update_webhook.py
--rw-r--r--   0        0        0     1456 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/upload.py
--rw-r--r--   0        0        0     2987 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/upload_from_url.py
--rw-r--r--   0        0        0     3928 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/main.py
--rw-r--r--   0        0        0     2282 2022-12-26 11:30:04.038620 pyuploadcare-4.0.0/pyuploadcare/ucare_cli/settings.py
--rw-r--r--   0        0        0     4386 1970-01-01 00:00:00.000000 pyuploadcare-4.0.0/setup.py
--rw-r--r--   0        0        0     4576 1970-01-01 00:00:00.000000 pyuploadcare-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/LICENSE
+-rw-r--r--   0        0        0     2996 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/README.md
+-rw-r--r--   0        0        0     2587 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/__init__.py
+-rw-r--r--   0        0        0     3412 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/addon_entities.py
+-rw-r--r--   0        0        0    18400 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/api.py
+-rw-r--r--   0        0        0     2901 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/auth.py
+-rw-r--r--   0        0        0     8261 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/base.py
+-rw-r--r--   0        0        0     8512 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/client.py
+-rw-r--r--   0        0        0     5772 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/entities.py
+-rw-r--r--   0        0        0     1001 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/metadata.py
+-rw-r--r--   0        0        0     2205 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/responses.py
+-rw-r--r--   0        0        0      447 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/api/utils.py
+-rw-r--r--   0        0        0    29560 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/client.py
+-rw-r--r--   0        0        0      841 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/conf.py
+-rw-r--r--   0        0        0      193 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/dj/__init__.py
+-rw-r--r--   0        0        0      472 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/dj/client.py
+-rw-r--r--   0        0        0     1510 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/dj/conf.py
+-rw-r--r--   0        0        0     3611 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/dj/forms.py
+-rw-r--r--   0        0        0     6211 2023-07-18 11:28:35.189646 pyuploadcare-4.1.0/pyuploadcare/dj/models.py
+-rw-r--r--   0        0        0   384057 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js
+-rw-r--r--   0        0        0   296023 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.min.js
+-rw-r--r--   0        0        0     2160 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/dj/subclassing.py
+-rw-r--r--   0        0        0     2224 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/exceptions.py
+-rw-r--r--   0        0        0     1288 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/resources/__init__.py
+-rw-r--r--   0        0        0     2816 2023-07-18 11:28:35.193646 pyuploadcare-4.1.0/pyuploadcare/resources/base.py
+-rw-r--r--   0        0        0    18812 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/resources/file.py
+-rw-r--r--   0        0        0     6882 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/resources/file_group.py
+-rw-r--r--   0        0        0     2241 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/resources/file_list.py
+-rw-r--r--   0        0        0     1400 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/resources/group_list.py
+-rw-r--r--   0        0        0      730 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/resources/utils.py
+-rw-r--r--   0        0        0     2336 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/secure_url.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/transformations/__init__.py
+-rw-r--r--   0        0        0     1305 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/transformations/base.py
+-rw-r--r--   0        0        0      729 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/transformations/document.py
+-rw-r--r--   0        0        0    10674 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/transformations/image.py
+-rw-r--r--   0        0        0     1711 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/transformations/video.py
+-rwxr-xr-x   0        0        0        0 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1394 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/convert_document.py
+-rw-r--r--   0        0        0     1048 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/convert_video.py
+-rw-r--r--   0        0        0      539 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/create_group.py
+-rw-r--r--   0        0        0     1028 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/create_webhook.py
+-rw-r--r--   0        0        0      984 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/delete_files.py
+-rw-r--r--   0        0        0      398 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/delete_webhook.py
+-rw-r--r--   0        0        0      439 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/get_file.py
+-rw-r--r--   0        0        0      455 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/get_project.py
+-rw-r--r--   0        0        0     3255 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/helpers.py
+-rw-r--r--   0        0        0     1406 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/list_files.py
+-rw-r--r--   0        0        0      934 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/list_groups.py
+-rw-r--r--   0        0        0      450 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/list_webhooks.py
+-rw-r--r--   0        0        0     1186 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/store_files.py
+-rw-r--r--   0        0        0     8801 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/sync.py
+-rw-r--r--   0        0        0     1484 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/update_webhook.py
+-rw-r--r--   0        0        0     1456 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/upload.py
+-rw-r--r--   0        0        0     2987 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/upload_from_url.py
+-rw-r--r--   0        0        0     3928 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/main.py
+-rw-r--r--   0        0        0     2282 2023-07-18 11:28:35.197646 pyuploadcare-4.1.0/pyuploadcare/ucare_cli/settings.py
+-rw-r--r--   0        0        0     4551 1970-01-01 00:00:00.000000 pyuploadcare-4.1.0/PKG-INFO
```

### Comparing `pyuploadcare-4.0.0/LICENSE` & `pyuploadcare-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/README.md` & `pyuploadcare-4.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,26 @@
         <th style="vertical-align: center; border: none;">
             <h1>PyUploadcare: a Python library for Uploadcare</h1>
         </th>
     </tr>
 </table>
 
 <p>
-  <img src="https://badge.fury.io/py/pyuploadcare.svg" height="25" />
-  <img src="https://github.com/uploadcare/pyuploadcare/actions/workflows/test.yml/badge.svg" height="25" /> 
-  <img src="https://readthedocs.org/projects/pyuploadcare/badge/?version=latest" height="25" />
-  <img src="https://coveralls.io/repos/github/uploadcare/pyuploadcare/badge.svg?branch=master" height="25" />
-  <img src="https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat" height="25" />
+  <a href="https://pypi.org/project/pyuploadcare/">
+    <img src="https://badge.fury.io/py/pyuploadcare.svg" height="25" />
+  </a>
+  <a href="https://github.com/uploadcare/pyuploadcare/actions?query=branch%3Amain+workflow%3ATests++">
+    <img src="https://github.com/uploadcare/pyuploadcare/actions/workflows/test.yml/badge.svg" height="25" />
+  </a>
+  <a href="https://pyuploadcare.readthedocs.io/">
+    <img src="https://readthedocs.org/projects/pyuploadcare/badge/?version=latest" height="25" />
+  </a>
+  <a href="https://stackshare.io/uploadcare">
+    <img src="https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat" height="25" />
+  </a>
 </p>
 
 Uploadcare Python & Django integrations handle uploads and further operations
 with files by wrapping Upload and REST APIs.
 
 Simple file uploads for the web are of most importance for us. Today, everyone
 is used to the routine of allowing users to upload their pics or attach resumes.
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
 [https://ucarecdn.com/2f4864b7-ed0e- ****** PyUploadcare: a Python library for
 4411-965b-8148623aa680/-/inline/yes/ Uploadcare ******
 uploadcare-logo-mark.svg]
 [https://badge.fury.io/py/pyuploadcare.svg] [https://github.com/uploadcare/
 pyuploadcare/actions/workflows/test.yml/badge.svg] [https://readthedocs.org/
-projects/pyuploadcare/badge/?version=latest] [https://coveralls.io/repos/
-github/uploadcare/pyuploadcare/badge.svg?branch=master] [https://
-img.shields.io/badge/tech-stack-0690fa.svg?style=flat]
+projects/pyuploadcare/badge/?version=latest] [https://img.shields.io/badge/
+tech-stack-0690fa.svg?style=flat]
 Uploadcare Python & Django integrations handle uploads and further operations
 with files by wrapping Upload and REST APIs. Simple file uploads for the web
 are of most importance for us. Today, everyone is used to the routine of
 allowing users to upload their pics or attach resumes. The routine covers it
 all: installing image processing libraries, adjusting permissions, ensuring
 servers never go down, and enabling CDN. This library consists of the
 Uploadcare API interface and a couple of Django goodies. Simple as that,
```

### Comparing `pyuploadcare-4.0.0/pyproject.toml` & `pyuploadcare-4.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "pyuploadcare"
-version = "4.0.0"
+version = "4.1.0"
 description = "Python library for Uploadcare.com"
 authors = ["Uploadcare Inc <hello@uploadcare.com>"]
 readme = "README.md"
 homepage = "https://uploadcare.com"
 repository = "https://github.com/uploadcare/pyuploadcare"
 classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/uploadcare/pyuploadcare/issues"
 
 [tool.poetry.scripts]
 ucare = 'pyuploadcare.ucare_cli.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 httpx = [
   {version = "^0.18.2", python = ">=3.6,<3.7"},
-  {version = "^0.23.0", python = "^3.7"}
+  {version = "^0.24.1", python = "^3.7"}
 ]
 pydantic = {extras = ["email"], version = "^1.8.2"}
 python-dateutil = "^2.8.2"
 pytz = "^2022.4"
 typing-extensions = [
     {version = "^3.10.0", python = ">=3.6,<3.7"},
     {version = "^4.3.0", python = "^3.7"}
@@ -50,15 +51,23 @@
 tox = "^3.24.1"
 black = "^22.3.0"
 isort = "^5.9.3"
 flake8 = "^3.9.2"
 mypy = "^0.910"
 flake8-print = "^4.0.0"
 pytest-vcr = "^1.0.2"
+yarl = [
+    {version = "^1.7.2", python = ">=3.6,<3.7"},
+    {version = "^1.9.2", python = "^3.7"}
+]
 Django = "^3.2.7"
+coverage = [
+    {version = "^6.2", python = ">=3.6,<3.7"},
+    {version = "^7.2.5", python = "^3.7"}
+]
 pytest-cov = "^2.12.1"
 python-coveralls = "^2.9.3"
 tox-pyenv = "^1.1.0"
 types-python-dateutil = "^2.8.0"
 types-pytz = "^2021.1.2"
 Sphinx = "^4.2.0"
 sphinx-argparse = "^0.3.1"
```

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/addon_entities.py` & `pyuploadcare-4.1.0/pyuploadcare/api/addon_entities.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/api.py` & `pyuploadcare-4.1.0/pyuploadcare/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ListCountMixin,
     ListMixin,
     RetrieveMixin,
     UpdateMixin,
 )
 from pyuploadcare.exceptions import (
     APIError,
+    DuplicateFileError,
     InvalidRequestError,
     WebhookIsNotUnique,
 )
 
 from .entities import UUIDEntity
 from .metadata import validate_meta_key, validate_meta_value, validate_metadata
 from .utils import flatten_dict
@@ -341,22 +342,24 @@
             "uuid": str(uuid),
             "UPLOADCARE_PUB_KEY": self.public_key,
         }
         url = self._build_url(base="multipart/complete")
         document = self._client.post(url, data=data)
         return document.json()
 
-    def upload_from_url(
+    def upload_from_url(  # noqa: max-complexity: 8
         self,
         source_url,
         store="auto",
         filename=None,
         metadata: Optional[Dict] = None,
         secure_upload: bool = False,
         expire: Optional[int] = None,
+        check_duplicates: Optional[bool] = None,
+        save_duplicates: Optional[bool] = None,
     ) -> str:
         data = {
             "source_url": source_url,
             "store": store,
             "pub_key": self.public_key,
         }
         if filename:
@@ -374,18 +377,30 @@
             )
 
             data["expire"] = str(expire)
             data["signature"] = self._generate_secure_signature(
                 self.secret_key, expire  # type: ignore
             )
 
+        if check_duplicates is not None:
+            data["check_URL_duplicates"] = "1" if check_duplicates else "0"
+
+        if save_duplicates is not None:
+            data["save_URL_duplicates"] = "1" if save_duplicates else "0"
+
         url = self._build_url(base="/from_url")
         document = self._client.post(url, data=data)
         response = document.json()
         if "token" not in response:
+            if check_duplicates and response["type"] == "file_info":
+                file_id = response["file_id"]
+                raise DuplicateFileError(
+                    f"The file is a duplicate of a previously uploaded file ({file_id})",
+                    file_id=file_id,
+                )
             raise APIError(f"could not find token in result: {response}")
         return response["token"]
 
     def get_upload_from_url_status(self, token: str) -> Dict[str, Any]:
         query_parameters = {
             "token": token,
         }
```

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/auth.py` & `pyuploadcare-4.1.0/pyuploadcare/api/auth.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/base.py` & `pyuploadcare-4.1.0/pyuploadcare/api/base.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/client.py` & `pyuploadcare-4.1.0/pyuploadcare/api/client.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/entities.py` & `pyuploadcare-4.1.0/pyuploadcare/api/entities.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/metadata.py` & `pyuploadcare-4.1.0/pyuploadcare/api/metadata.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/api/responses.py` & `pyuploadcare-4.1.0/pyuploadcare/api/responses.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/client.py` & `pyuploadcare-4.1.0/pyuploadcare/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     UploadAPI,
     VideoConvertAPI,
     WebhooksAPI,
 )
 from pyuploadcare.api.auth import UploadcareAuth
 from pyuploadcare.api.client import Client
 from pyuploadcare.api.entities import ProjectInfo, Webhook
-from pyuploadcare.exceptions import InvalidParamError
+from pyuploadcare.exceptions import DuplicateFileError, InvalidParamError
 from pyuploadcare.helpers import (
     extracts_uuids,
     get_file_size,
     guess_mime_type,
     iterate_over_batches,
 )
 from pyuploadcare.resources.file import FileFromUrl, UploadProgress
@@ -447,29 +447,40 @@
 
             chunk = file_obj.read(self.multipart_chunk_size)
 
         file_info: Dict = self.upload_api.multipart_complete(multipart_uuid)
         return self.file(file_info["uuid"], file_info)
 
     def upload_from_url(
-        self, url, store=None, filename=None, metadata=None
+        self,
+        url,
+        store=None,
+        filename=None,
+        metadata=None,
+        check_duplicates: Optional[bool] = None,
+        save_duplicates: Optional[bool] = None,
     ) -> FileFromUrl:
         """Uploads file from given url and returns ``FileFromUrl`` instance.
 
         Args:
             - url (str): URL of file to upload to
             - store (Optional[bool]): Should the file be automatically stored
                 upon upload. Defaults to None.
                 - False - do not store file
                 - True - store file (can result in error if autostore
                                is disabled for project)
                 - None - use project settings
             - filename (Optional[str]): Name of the uploaded file. If this not
                 specified the filename will be obtained from response headers
                 or source URL. Defaults to None.
+            - check_duplicates (Optional[bool]): Enables duplicate uploads
+                prevention. If a file with the same source URL has been
+                previously uploaded this method will raise DuplicateFileError.
+            - save_duplicates (Optional[bool]): Indicates if the URL should be
+                stored by Uploadcare future check_duplicates usages.
 
         Returns:
             ``FileFromUrl`` instance
 
         """
         if store is None:
             store = "auto"
@@ -481,28 +492,32 @@
         token = self.upload_api.upload_from_url(
             source_url=url,
             store=store,
             filename=filename,
             metadata=metadata,
             secure_upload=self.signed_uploads,
             expire=self.signed_uploads_ttl,
+            check_duplicates=check_duplicates,
+            save_duplicates=save_duplicates,
         )
         file_from_url = FileFromUrl(token, self)
         return file_from_url
 
     def upload_from_url_sync(
         self,
         url,
         timeout=30,
         interval=0.3,
         metadata=None,
         until_ready=False,
         store=None,
         filename=None,
         callback: Optional[Callable[[UploadProgress], Any]] = None,
+        check_duplicates: Optional[bool] = None,
+        save_duplicates: Optional[bool] = None,
     ) -> File:
         """Uploads file from given url and returns ``File`` instance.
 
         Args:
             - url (str): URL of file to upload to
             - store (Optional[bool]): Should the file be automatically stored
                 upon upload. Defaults to None.
@@ -517,29 +532,45 @@
                 Defaults to 30.
             - interval (Optional[float]): interval between upload status checks.
                 Defaults to 0.3.
             - until_ready (Optional[bool]): should we wait until file is
                 available via CDN. Defaults to False.
             - callback (Optional[Callable[[UploadProgress], Any]]): Optional callback
                 accepting ``UploadProgress`` to track uploading progress.
+            - check_duplicates (Optional[bool]): Enables duplicate uploads
+                prevention. If a file with the same source URL has been
+                previously uploaded this method will return the previously
+                uploaded file.
+            - save_duplicates (Optional[bool]): Indicates if the URL should be
+                stored by Uploadcare future check_duplicates usages.
 
         Returns:
             ``File`` instance
 
         Raises:
             ``TimeoutError`` if file wasn't uploaded in time
 
         """
-        ffu = self.upload_from_url(url, store, filename, metadata=metadata)
-        return ffu.wait(
-            timeout=timeout,
-            interval=interval,
-            until_ready=until_ready,
-            callback=callback,
-        )
+        try:
+            ffu = self.upload_from_url(
+                url,
+                store,
+                filename,
+                metadata=metadata,
+                check_duplicates=check_duplicates,
+                save_duplicates=save_duplicates,
+            )
+            return ffu.wait(
+                timeout=timeout,
+                interval=interval,
+                until_ready=until_ready,
+                callback=callback,
+            )
+        except DuplicateFileError as e:
+            return self.file(e.file_id)
 
     def _extract_uuids(
         self, files: Iterable[Union[str, File, UUID]]
     ) -> List[str]:
         """Convert various resource representation into string-based."""
         file_generator = (
             file_ if isinstance(file_, File) else File(file_, self)
@@ -566,15 +597,15 @@
                 List of file UUIDs, CND urls or ``File`` instances.
         """
         uuids = self._extract_uuids(files)
 
         for chunk in iterate_over_batches(uuids, self.batch_chunk_size):
             self.files_api.batch_store(chunk)
 
-    def delete_files(self, files: Iterable[Union[str, "File"]]) -> None:
+    def delete_files(self, files: Iterable[Union[str, UUID, "File"]]) -> None:
         """Deletes multiple files by requesting Uploadcare API.
 
         Usage example::
 
             >>> uploadcare = Uploadcare(public_key='<public-key>', secret_key='<secret-key>')
             >>> files = [
             ... '6c5e9526-b0fe-4739-8975-72e8d5ee6342',
@@ -631,15 +662,15 @@
         stored: Optional[bool] = None,
         removed: Optional[bool] = None,
     ) -> FileList:
         """List files.
 
         Returns ``FileList`` instance providing iteration over all uploaded files.
 
-        Args:m
+        Args:
             - ``starting_point`` -- a starting point for filtering files.
               It is reflects a ``from`` parameter from REST API.
             - ``ordering`` -- a string with name of the field what must be used
               for sorting files. The actual list of supported fields you can find in
               documentation: http://uploadcare.com/documentation/rest/#file-files
             - ``limit`` -- a total number of objects to be iterated.
               If not specified, all available objects are iterated;
```

### Comparing `pyuploadcare-4.0.0/pyuploadcare/conf.py` & `pyuploadcare-4.1.0/pyuploadcare/conf.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/dj/conf.py` & `pyuploadcare-4.1.0/pyuploadcare/dj/conf.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/dj/forms.py` & `pyuploadcare-4.1.0/pyuploadcare/dj/forms.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/dj/models.py` & `pyuploadcare-4.1.0/pyuploadcare/dj/models.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js` & `pyuploadcare-4.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.full.min.js`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/dj/static/uploadcare/uploadcare.min.js` & `pyuploadcare-4.1.0/pyuploadcare/dj/static/uploadcare/uploadcare.min.js`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/dj/subclassing.py` & `pyuploadcare-4.1.0/pyuploadcare/dj/subclassing.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/exceptions.py` & `pyuploadcare-4.1.0/pyuploadcare/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,14 +55,27 @@
     It raises when user wants to wait the result of::
 
         $ ucare upload_from_url --wait http://path.to/file.jpg
 
     """
 
 
+class DuplicateFileError(UploadError):
+    """
+    Raised within UploadAPI.upload_from_url if check_duplicates is True
+    and file was already been uploaded before)
+    """
+
+    file_id: str
+
+    def __init__(self, message: str, file_id: str) -> None:
+        super().__init__(message)
+        self.file_id = file_id
+
+
 class DefaultResponseClassNotDefined(Exception):
     def __init__(self) -> None:
         super().__init__("Need define default response class for API.")
 
 
 class MetadataValidationError(UploadcareException):
     """
```

### Comparing `pyuploadcare-4.0.0/pyuploadcare/helpers.py` & `pyuploadcare-4.1.0/pyuploadcare/helpers.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/resources/base.py` & `pyuploadcare-4.1.0/pyuploadcare/resources/base.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/resources/file.py` & `pyuploadcare-4.1.0/pyuploadcare/resources/file.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/resources/file_group.py` & `pyuploadcare-4.1.0/pyuploadcare/resources/file_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import re
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, Optional
 
 import dateutil.parser
 
 from pyuploadcare.exceptions import InvalidParamError
 from pyuploadcare.resources.utils import (
     coerce_to_optional_datetime,
     max_for_optional_datetimes,
 )
 
 
 if TYPE_CHECKING:
     from pyuploadcare.client import Uploadcare
+    from pyuploadcare.resources.file import File
 
 
 GROUP_ID_REGEX = re.compile(
     r"""
     (?P<group_id>
         [a-z0-9]{8}-(?:[a-z0-9]{4}-){3}[a-z0-9]{12}
         ~
         (?P<files_qty>\d+)
     )
 """,
     re.VERBOSE,
 )
 
 
-class FileGroup:
+class FileGroup(Iterable):
     """File Group resource for working with user-uploaded group of files.
 
     It can take group id or group CDN url::
 
         >>> file_group = uploadcare.file_group('0513dda0-582f-447d-846f-096e5df9e2bb~2')
 
     You can iterate ``file_group`` or get ``File`` instance by key::
@@ -88,14 +89,20 @@
         if isinstance(key, slice):
             raise TypeError("slicing is not supported")
         else:
             file_info = self.info["files"][key]
             if file_info is not None:
                 return self._client.file(file_info["uuid"], file_info)
 
+    def __iter__(self) -> Iterator["File"]:
+        for i in range(len(self)):
+            file_ = self[i]
+            if file_:
+                yield file_
+
     @property
     def cdn_url(self):
         """Returns group's CDN url.
 
         Usage example::
 
             >>> file_group = uploadcare.file_group('0513dda0-582f-447d-846f-096e5df9e2bb~2')
@@ -209,17 +216,23 @@
         """Returns ``True`` if group is deleted.
 
         It makes no API call
 
         """
         return self._is_deleted
 
-    def delete(self):
+    def delete(self, delete_files: bool = False):
         """Delete group itself, left files unchanged
 
         Added in API v. 0.7.0
+
+        Args:
+            - ``delete_files`` -- ``True`` do also delete files in this group.
         """
         if self._is_deleted:
             return
 
+        if delete_files:
+            self._client.delete_files(file_ for file_ in self)
+
         self._client.groups_api.delete(self.id)
         self._is_deleted = True
```

### Comparing `pyuploadcare-4.0.0/pyuploadcare/resources/file_list.py` & `pyuploadcare-4.1.0/pyuploadcare/resources/file_list.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/resources/group_list.py` & `pyuploadcare-4.1.0/pyuploadcare/resources/group_list.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/resources/utils.py` & `pyuploadcare-4.1.0/pyuploadcare/resources/utils.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/secure_url.py` & `pyuploadcare-4.1.0/pyuploadcare/secure_url.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/transformations/base.py` & `pyuploadcare-4.1.0/pyuploadcare/transformations/base.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/transformations/document.py` & `pyuploadcare-4.1.0/pyuploadcare/transformations/document.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/transformations/image.py` & `pyuploadcare-4.1.0/pyuploadcare/transformations/image.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/transformations/video.py` & `pyuploadcare-4.1.0/pyuploadcare/transformations/video.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/convert_document.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/convert_document.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/convert_video.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/convert_video.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/create_group.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/create_group.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/create_webhook.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/create_webhook.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/delete_files.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/delete_files.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/helpers.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/list_files.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/list_files.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/list_groups.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/list_groups.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/store_files.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/store_files.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/sync.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/update_webhook.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/update_webhook.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/upload.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/commands/upload_from_url.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/commands/upload_from_url.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/main.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/main.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/pyuploadcare/ucare_cli/settings.py` & `pyuploadcare-4.1.0/pyuploadcare/ucare_cli/settings.py`

 * *Files identical despite different names*

### Comparing `pyuploadcare-4.0.0/setup.py` & `pyuploadcare-4.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,275 +1,285 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2770 7975 706c 6f61 6463 6172   \.['pyuploadcar
-00000050: 6527 2c0a 2027 7079 7570 6c6f 6164 6361  e',. 'pyuploadca
-00000060: 7265 2e61 7069 272c 0a20 2770 7975 706c  re.api',. 'pyupl
-00000070: 6f61 6463 6172 652e 646a 272c 0a20 2770  oadcare.dj',. 'p
-00000080: 7975 706c 6f61 6463 6172 652e 7265 736f  yuploadcare.reso
-00000090: 7572 6365 7327 2c0a 2027 7079 7570 6c6f  urces',. 'pyuplo
-000000a0: 6164 6361 7265 2e74 7261 6e73 666f 726d  adcare.transform
-000000b0: 6174 696f 6e73 272c 0a20 2770 7975 706c  ations',. 'pyupl
-000000c0: 6f61 6463 6172 652e 7563 6172 655f 636c  oadcare.ucare_cl
-000000d0: 6927 2c0a 2027 7079 7570 6c6f 6164 6361  i',. 'pyuploadca
-000000e0: 7265 2e75 6361 7265 5f63 6c69 2e63 6f6d  re.ucare_cli.com
-000000f0: 6d61 6e64 7327 5d0a 0a70 6163 6b61 6765  mands']..package
-00000100: 5f64 6174 6120 3d20 5c0a 7b27 273a 205b  _data = \.{'': [
-00000110: 272a 275d 2c20 2770 7975 706c 6f61 6463  '*'], 'pyuploadc
-00000120: 6172 652e 646a 273a 205b 2773 7461 7469  are.dj': ['stati
-00000130: 632f 7570 6c6f 6164 6361 7265 2f2a 275d  c/uploadcare/*']
-00000140: 7d0a 0a69 6e73 7461 6c6c 5f72 6571 7569  }..install_requi
-00000150: 7265 7320 3d20 5c0a 5b27 7079 6461 6e74  res = \.['pydant
-00000160: 6963 5b65 6d61 696c 5d3e 3d31 2e38 2e32  ic[email]>=1.8.2
-00000170: 2c3c 322e 302e 3027 2c0a 2027 7079 7468  ,<2.0.0',. 'pyth
-00000180: 6f6e 2d64 6174 6575 7469 6c3e 3d32 2e38  on-dateutil>=2.8
-00000190: 2e32 2c3c 332e 302e 3027 2c0a 2027 7079  .2,<3.0.0',. 'py
-000001a0: 747a 3e3d 3230 3232 2e34 2c3c 3230 3233  tz>=2022.4,<2023
-000001b0: 2e30 275d 0a0a 6578 7472 6173 5f72 6571  .0']..extras_req
-000001c0: 7569 7265 203d 205c 0a7b 273a 7079 7468  uire = \.{':pyth
-000001d0: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2233  on_version >= "3
-000001e0: 2e36 2220 616e 6420 7079 7468 6f6e 5f76  .6" and python_v
-000001f0: 6572 7369 6f6e 203c 2022 332e 3722 273a  ersion < "3.7"':
-00000200: 205b 2768 7474 7078 3e3d 302e 3138 2e32   ['httpx>=0.18.2
-00000210: 2c3c 302e 3139 2e30 272c 0a20 2020 2020  ,<0.19.0',.     
-00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000250: 2020 2020 2774 7970 696e 672d 6578 7465      'typing-exte
-00000260: 6e73 696f 6e73 3e3d 332e 3130 2e30 2c3c  nsions>=3.10.0,<
-00000270: 342e 302e 3027 5d2c 0a20 273a 7079 7468  4.0.0'],. ':pyth
-00000280: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2233  on_version >= "3
-00000290: 2e37 2220 616e 6420 7079 7468 6f6e 5f76  .7" and python_v
-000002a0: 6572 7369 6f6e 203c 2022 342e 3022 273a  ersion < "4.0"':
-000002b0: 205b 2768 7474 7078 3e3d 302e 3233 2e30   ['httpx>=0.23.0
-000002c0: 2c3c 302e 3234 2e30 272c 0a20 2020 2020  ,<0.24.0',.     
-000002d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000300: 2020 2020 2774 7970 696e 672d 6578 7465      'typing-exte
-00000310: 6e73 696f 6e73 3e3d 342e 332e 302c 3c35  nsions>=4.3.0,<5
-00000320: 2e30 2e30 275d 2c0a 2027 646a 616e 676f  .0.0'],. 'django
-00000330: 273a 205b 2744 6a61 6e67 6f3e 3d31 2e31  ': ['Django>=1.1
-00000340: 3127 5d7d 0a0a 656e 7472 795f 706f 696e  1']}..entry_poin
-00000350: 7473 203d 205c 0a7b 2763 6f6e 736f 6c65  ts = \.{'console
-00000360: 5f73 6372 6970 7473 273a 205b 2775 6361  _scripts': ['uca
-00000370: 7265 203d 2070 7975 706c 6f61 6463 6172  re = pyuploadcar
-00000380: 652e 7563 6172 655f 636c 692e 6d61 696e  e.ucare_cli.main
-00000390: 3a6d 6169 6e27 5d7d 0a0a 7365 7475 705f  :main']}..setup_
-000003a0: 6b77 6172 6773 203d 207b 0a20 2020 2027  kwargs = {.    '
-000003b0: 6e61 6d65 273a 2027 7079 7570 6c6f 6164  name': 'pyupload
-000003c0: 6361 7265 272c 0a20 2020 2027 7665 7273  care',.    'vers
-000003d0: 696f 6e27 3a20 2734 2e30 2e30 272c 0a20  ion': '4.0.0',. 
-000003e0: 2020 2027 6465 7363 7269 7074 696f 6e27     'description'
-000003f0: 3a20 2750 7974 686f 6e20 6c69 6272 6172  : 'Python librar
-00000400: 7920 666f 7220 5570 6c6f 6164 6361 7265  y for Uploadcare
-00000410: 2e63 6f6d 272c 0a20 2020 2027 6c6f 6e67  .com',.    'long
-00000420: 5f64 6573 6372 6970 7469 6f6e 273a 2027  _description': '
-00000430: 5c6e 3c74 6162 6c65 3e5c 6e20 2020 203c  \n<table>\n    <
-00000440: 7472 2073 7479 6c65 3d22 626f 7264 6572  tr style="border
-00000450: 3a20 6e6f 6e65 3b22 3e5c 6e20 2020 2020  : none;">\n     
-00000460: 2020 203c 7464 2073 7479 6c65 3d22 626f     <td style="bo
-00000470: 7264 6572 3a20 6e6f 6e65 3b22 3e5c 6e20  rder: none;">\n 
-00000480: 2020 2020 2020 2020 2020 203c 696d 6720             <img 
-00000490: 7372 633d 2268 7474 7073 3a2f 2f75 6361  src="https://uca
-000004a0: 7265 6364 6e2e 636f 6d2f 3266 3438 3634  recdn.com/2f4864
-000004b0: 6237 2d65 6430 652d 3434 3131 2d39 3635  b7-ed0e-4411-965
-000004c0: 622d 3831 3438 3632 3361 6136 3830 2f2d  b-8148623aa680/-
-000004d0: 2f69 6e6c 696e 652f 7965 732f 7570 6c6f  /inline/yes/uplo
-000004e0: 6164 6361 7265 2d6c 6f67 6f2d 6d61 726b  adcare-logo-mark
-000004f0: 2e73 7667 2220 7461 7267 6574 3d22 2220  .svg" target="" 
-00000500: 7769 6474 683d 2236 3422 2068 6569 6768  width="64" heigh
-00000510: 743d 2236 3422 3e5c 6e20 2020 2020 2020  t="64">\n       
-00000520: 203c 2f74 643e 5c6e 2020 2020 2020 2020   </td>\n        
-00000530: 3c74 6820 7374 796c 653d 2276 6572 7469  <th style="verti
-00000540: 6361 6c2d 616c 6967 6e3a 2063 656e 7465  cal-align: cente
-00000550: 723b 2062 6f72 6465 723a 206e 6f6e 653b  r; border: none;
-00000560: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-00000570: 3c68 313e 5079 5570 6c6f 6164 6361 7265  <h1>PyUploadcare
-00000580: 3a20 6120 5079 7468 6f6e 206c 6962 7261  : a Python libra
-00000590: 7279 2066 6f72 2055 706c 6f61 6463 6172  ry for Uploadcar
-000005a0: 653c 2f68 313e 5c6e 2020 2020 2020 2020  e</h1>\n        
-000005b0: 3c2f 7468 3e5c 6e20 2020 203c 2f74 723e  </th>\n    </tr>
-000005c0: 5c6e 3c2f 7461 626c 653e 5c6e 5c6e 3c70  \n</table>\n\n<p
-000005d0: 3e5c 6e20 203c 696d 6720 7372 633d 2268  >\n  <img src="h
-000005e0: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
-000005f0: 792e 696f 2f70 792f 7079 7570 6c6f 6164  y.io/py/pyupload
-00000600: 6361 7265 2e73 7667 2220 6865 6967 6874  care.svg" height
-00000610: 3d22 3235 2220 2f3e 5c6e 2020 3c69 6d67  ="25" />\n  <img
-00000620: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-00000630: 7468 7562 2e63 6f6d 2f75 706c 6f61 6463  thub.com/uploadc
-00000640: 6172 652f 7079 7570 6c6f 6164 6361 7265  are/pyuploadcare
-00000650: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000660: 7773 2f74 6573 742e 796d 6c2f 6261 6467  ws/test.yml/badg
-00000670: 652e 7376 6722 2068 6569 6768 743d 2232  e.svg" height="2
-00000680: 3522 202f 3e20 5c6e 2020 3c69 6d67 2073  5" /> \n  <img s
-00000690: 7263 3d22 6874 7470 733a 2f2f 7265 6164  rc="https://read
-000006a0: 7468 6564 6f63 732e 6f72 672f 7072 6f6a  thedocs.org/proj
-000006b0: 6563 7473 2f70 7975 706c 6f61 6463 6172  ects/pyuploadcar
-000006c0: 652f 6261 6467 652f 3f76 6572 7369 6f6e  e/badge/?version
-000006d0: 3d6c 6174 6573 7422 2068 6569 6768 743d  =latest" height=
-000006e0: 2232 3522 202f 3e5c 6e20 203c 696d 6720  "25" />\n  <img 
-000006f0: 7372 633d 2268 7474 7073 3a2f 2f63 6f76  src="https://cov
-00000700: 6572 616c 6c73 2e69 6f2f 7265 706f 732f  eralls.io/repos/
-00000710: 6769 7468 7562 2f75 706c 6f61 6463 6172  github/uploadcar
-00000720: 652f 7079 7570 6c6f 6164 6361 7265 2f62  e/pyuploadcare/b
-00000730: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000740: 6d61 7374 6572 2220 6865 6967 6874 3d22  master" height="
-00000750: 3235 2220 2f3e 5c6e 2020 3c69 6d67 2073  25" />\n  <img s
-00000760: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000770: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000780: 2f74 6563 682d 7374 6163 6b2d 3036 3930  /tech-stack-0690
-00000790: 6661 2e73 7667 3f73 7479 6c65 3d66 6c61  fa.svg?style=fla
-000007a0: 7422 2068 6569 6768 743d 2232 3522 202f  t" height="25" /
-000007b0: 3e5c 6e3c 2f70 3e5c 6e5c 6e55 706c 6f61  >\n</p>\n\nUploa
-000007c0: 6463 6172 6520 5079 7468 6f6e 2026 2044  dcare Python & D
-000007d0: 6a61 6e67 6f20 696e 7465 6772 6174 696f  jango integratio
-000007e0: 6e73 2068 616e 646c 6520 7570 6c6f 6164  ns handle upload
-000007f0: 7320 616e 6420 6675 7274 6865 7220 6f70  s and further op
-00000800: 6572 6174 696f 6e73 5c6e 7769 7468 2066  erations\nwith f
-00000810: 696c 6573 2062 7920 7772 6170 7069 6e67  iles by wrapping
-00000820: 2055 706c 6f61 6420 616e 6420 5245 5354   Upload and REST
-00000830: 2041 5049 732e 5c6e 5c6e 5369 6d70 6c65   APIs.\n\nSimple
-00000840: 2066 696c 6520 7570 6c6f 6164 7320 666f   file uploads fo
-00000850: 7220 7468 6520 7765 6220 6172 6520 6f66  r the web are of
-00000860: 206d 6f73 7420 696d 706f 7274 616e 6365   most importance
-00000870: 2066 6f72 2075 732e 2054 6f64 6179 2c20   for us. Today, 
-00000880: 6576 6572 796f 6e65 5c6e 6973 2075 7365  everyone\nis use
-00000890: 6420 746f 2074 6865 2072 6f75 7469 6e65  d to the routine
-000008a0: 206f 6620 616c 6c6f 7769 6e67 2075 7365   of allowing use
-000008b0: 7273 2074 6f20 7570 6c6f 6164 2074 6865  rs to upload the
-000008c0: 6972 2070 6963 7320 6f72 2061 7474 6163  ir pics or attac
-000008d0: 6820 7265 7375 6d65 732e 5c6e 5468 6520  h resumes.\nThe 
-000008e0: 726f 7574 696e 6520 636f 7665 7273 2069  routine covers i
-000008f0: 7420 616c 6c3a 2069 6e73 7461 6c6c 696e  t all: installin
-00000900: 6720 696d 6167 6520 7072 6f63 6573 7369  g image processi
-00000910: 6e67 206c 6962 7261 7269 6573 2c20 6164  ng libraries, ad
-00000920: 6a75 7374 696e 675c 6e70 6572 6d69 7373  justing\npermiss
-00000930: 696f 6e73 2c20 656e 7375 7269 6e67 2073  ions, ensuring s
-00000940: 6572 7665 7273 206e 6576 6572 2067 6f20  ervers never go 
-00000950: 646f 776e 2c20 616e 6420 656e 6162 6c69  down, and enabli
-00000960: 6e67 2043 444e 2e5c 6e5c 6e54 6869 7320  ng CDN.\n\nThis 
-00000970: 6c69 6272 6172 7920 636f 6e73 6973 7473  library consists
-00000980: 206f 6620 7468 6520 5570 6c6f 6164 6361   of the Uploadca
-00000990: 7265 2041 5049 2069 6e74 6572 6661 6365  re API interface
-000009a0: 2061 6e64 2061 2063 6f75 706c 6520 6f66   and a couple of
-000009b0: 2044 6a61 6e67 6f5c 6e67 6f6f 6469 6573   Django\ngoodies
-000009c0: 2e5c 6e5c 6e53 696d 706c 6520 6173 2074  .\n\nSimple as t
-000009d0: 6861 742c 2055 706c 6f61 6463 6172 6520  hat, Uploadcare 
-000009e0: 6049 6d61 6765 4669 656c 6460 2063 616e  `ImageField` can
-000009f0: 2062 6520 6164 6465 6420 746f 2061 6e5c   be added to an\
-00000a00: 6e65 7869 7374 696e 6720 446a 616e 676f  nexisting Django
-00000a10: 2070 726f 6a65 6374 2069 6e20 6a75 7374   project in just
-00000a20: 2061 2063 6f75 706c 6520 6f66 205b 7369   a couple of [si
-00000a30: 6d70 6c65 2073 7465 7073 5d28 6874 7470  mple steps](http
-00000a40: 733a 2f2f 7079 7570 6c6f 6164 6361 7265  s://pyuploadcare
-00000a50: 2e72 6561 6474 6865 646f 6373 2e6f 7267  .readthedocs.org
-00000a60: 2f65 6e2f 6c61 7465 7374 2f71 7569 636b  /en/latest/quick
-00000a70: 7374 6172 742e 6874 6d6c 292e 5c6e 5468  start.html).\nTh
-00000a80: 6973 2077 696c 6c20 656e 6162 6c65 2079  is will enable y
-00000a90: 6f75 7220 7573 6572 7320 746f 2073 6565  our users to see
-00000aa0: 2074 6865 2075 706c 6f61 6420 7072 6f67   the upload prog
-00000ab0: 7265 7373 2c20 7069 636b 2066 696c 6573  ress, pick files
-00000ac0: 5c6e 6672 6f6d 2047 6f6f 676c 6520 4472  \nfrom Google Dr
-00000ad0: 6976 6520 6f72 2049 6e73 7461 6772 616d  ive or Instagram
-00000ae0: 2c20 616e 6420 6564 6974 2061 2066 6f72  , and edit a for
-00000af0: 6d20 7768 696c 6520 6669 6c65 7320 6172  m while files ar
-00000b00: 655c 6e62 6569 6e67 2075 706c 6f61 6465  e\nbeing uploade
-00000b10: 6420 6173 796e 6368 726f 6e6f 7573 6c79  d asynchronously
-00000b20: 2e5c 6e5c 6e59 6f75 2063 616e 2066 696e  .\n\nYou can fin
-00000b30: 6420 616e 2065 7861 6d70 6c65 2070 726f  d an example pro
-00000b40: 6a65 6374 205b 6865 7265 5d28 6874 7470  ject [here](http
-00000b50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f75  s://github.com/u
-00000b60: 706c 6f61 6463 6172 652f 7079 7570 6c6f  ploadcare/pyuplo
-00000b70: 6164 6361 7265 2d65 7861 6d70 6c65 292e  adcare-example).
-00000b80: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e5c  \n\n```python\n\
-00000b90: 6e20 2020 2066 726f 6d20 646a 616e 676f  n    from django
-00000ba0: 2069 6d70 6f72 7420 666f 726d 735c 6e20   import forms\n 
-00000bb0: 2020 2066 726f 6d20 646a 616e 676f 2e64     from django.d
-00000bc0: 6220 696d 706f 7274 206d 6f64 656c 735c  b import models\
-00000bd0: 6e5c 6e20 2020 2066 726f 6d20 7079 7570  n\n    from pyup
-00000be0: 6c6f 6164 6361 7265 2e64 6a2e 6d6f 6465  loadcare.dj.mode
-00000bf0: 6c73 2069 6d70 6f72 7420 496d 6167 6546  ls import ImageF
-00000c00: 6965 6c64 5c6e 2020 2020 6672 6f6d 2070  ield\n    from p
-00000c10: 7975 706c 6f61 6463 6172 652e 646a 2e66  yuploadcare.dj.f
-00000c20: 6f72 6d73 2069 6d70 6f72 7420 4669 6c65  orms import File
-00000c30: 5769 6467 6574 2c20 496d 6167 6546 6965  Widget, ImageFie
-00000c40: 6c64 2061 7320 496d 6167 6546 6f72 6d46  ld as ImageFormF
-00000c50: 6965 6c64 5c6e 5c6e 5c6e 2020 2020 636c  ield\n\n\n    cl
-00000c60: 6173 7320 4361 6e64 6964 6174 6528 6d6f  ass Candidate(mo
-00000c70: 6465 6c73 2e4d 6f64 656c 293a 5c6e 2020  dels.Model):\n  
-00000c80: 2020 2020 2020 7068 6f74 6f20 3d20 496d        photo = Im
-00000c90: 6167 6546 6965 6c64 2862 6c61 6e6b 3d54  ageField(blank=T
-00000ca0: 7275 652c 206d 616e 7561 6c5f 6372 6f70  rue, manual_crop
-00000cb0: 3d22 2229 5c6e 5c6e 5c6e 2020 2020 2320  ="")\n\n\n    # 
-00000cc0: 6f70 7469 6f6e 616c 2e20 7072 6f76 6964  optional. provid
-00000cd0: 6520 6164 7661 6e63 6564 2077 6964 6765  e advanced widge
-00000ce0: 7420 6f70 7469 6f6e 733a 2068 7474 7073  t options: https
-00000cf0: 3a2f 2f75 706c 6f61 6463 6172 652e 636f  ://uploadcare.co
-00000d00: 6d2f 646f 6373 2f75 706c 6f61 6473 2f77  m/docs/uploads/w
-00000d10: 6964 6765 742f 636f 6e66 6967 2f23 6f70  idget/config/#op
-00000d20: 7469 6f6e 735c 6e20 2020 2063 6c61 7373  tions\n    class
-00000d30: 2043 616e 6469 6461 7465 466f 726d 2866   CandidateForm(f
-00000d40: 6f72 6d73 2e46 6f72 6d29 3a5c 6e20 2020  orms.Form):\n   
-00000d50: 2020 2020 2070 686f 746f 203d 2049 6d61       photo = Ima
-00000d60: 6765 466f 726d 4669 656c 6428 7769 6467  geFormField(widg
-00000d70: 6574 3d46 696c 6557 6964 6765 7428 6174  et=FileWidget(at
-00000d80: 7472 733d 7b5c 6e20 2020 2020 2020 2020  trs={\n         
-00000d90: 2020 205c 2764 6174 612d 6364 6e2d 6261     \'data-cdn-ba
-00000da0: 7365 5c27 3a20 5c27 6874 7470 733a 2f2f  se\': \'https://
-00000db0: 6364 6e2e 7375 7065 722d 6361 6e64 6964  cdn.super-candid
-00000dc0: 6174 6573 2e63 6f6d 5c27 2c5c 6e20 2020  ates.com\',\n   
-00000dd0: 2020 2020 2020 2020 205c 2764 6174 612d           \'data-
-00000de0: 696d 6167 652d 7368 7269 6e6b 5c27 3a20  image-shrink\': 
-00000df0: 5c27 3130 3234 7831 3032 345c 272c 5c6e  \'1024x1024\',\n
-00000e00: 2020 2020 2020 2020 7d29 295c 6e5c 6e60          }))\n\n`
-00000e10: 6060 5c6e 5c6e 215b 5d28 6874 7470 733a  ``\n\n![](https:
-00000e20: 2f2f 7563 6172 6563 646e 2e63 6f6d 2f64  //ucarecdn.com/d
-00000e30: 6262 3430 3231 652d 6232 3065 2d34 3066  bb4021e-b20e-40f
-00000e40: 612d 3930 3762 2d33 6461 3061 3466 3865  a-907b-3da0a4f8e
-00000e50: 6437 302f 2d2f 7265 7369 7a65 2f38 3030  d70/-/resize/800
-00000e60: 2f6d 616e 7561 6c5f 6372 6f70 2e70 6e67  /manual_crop.png
-00000e70: 295c 6e5c 6e23 2320 446f 6375 6d65 6e74  )\n\n## Document
-00000e80: 6174 696f 6e5c 6e5c 6e44 6574 6169 6c65  ation\n\nDetaile
-00000e90: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
-00000ea0: 6973 2061 7661 696c 6162 6c65 205b 6f6e  is available [on
-00000eb0: 2052 5444 5d28 6874 7470 733a 2f2f 7079   RTD](https://py
-00000ec0: 7570 6c6f 6164 6361 7265 2e72 6561 6474  uploadcare.readt
-00000ed0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000ee0: 6573 742f 292e 5c6e 5c6e 2323 2046 6565  est/).\n\n## Fee
-00000ef0: 6462 6163 6b5c 6e5c 6e49 7373 7565 7320  dback\n\nIssues 
-00000f00: 616e 6420 5052 7320 6172 6520 7765 6c63  and PRs are welc
-00000f10: 6f6d 652e 2059 6f75 2063 616e 2070 726f  ome. You can pro
-00000f20: 7669 6465 2079 6f75 7220 6665 6564 6261  vide your feedba
-00000f30: 636b 206f 7220 6472 6f70 2075 7320 6120  ck or drop us a 
-00000f40: 7375 7070 6f72 745c 6e72 6571 7565 7374  support\nrequest
-00000f50: 2061 7420 5b68 656c 6c6f 4075 706c 6f61   at [hello@uploa
-00000f60: 6463 6172 652e 636f 6d5d 2868 656c 6c6f  dcare.com](hello
-00000f70: 4075 706c 6f61 6463 6172 652e 636f 6d29  @uploadcare.com)
-00000f80: 2e5c 6e27 2c0a 2020 2020 2761 7574 686f  .\n',.    'autho
-00000f90: 7227 3a20 2755 706c 6f61 6463 6172 6520  r': 'Uploadcare 
-00000fa0: 496e 6327 2c0a 2020 2020 2761 7574 686f  Inc',.    'autho
-00000fb0: 725f 656d 6169 6c27 3a20 2768 656c 6c6f  r_email': 'hello
-00000fc0: 4075 706c 6f61 6463 6172 652e 636f 6d27  @uploadcare.com'
-00000fd0: 2c0a 2020 2020 276d 6169 6e74 6169 6e65  ,.    'maintaine
-00000fe0: 7227 3a20 274e 6f6e 6527 2c0a 2020 2020  r': 'None',.    
-00000ff0: 276d 6169 6e74 6169 6e65 725f 656d 6169  'maintainer_emai
-00001000: 6c27 3a20 274e 6f6e 6527 2c0a 2020 2020  l': 'None',.    
-00001010: 2775 726c 273a 2027 6874 7470 733a 2f2f  'url': 'https://
-00001020: 7570 6c6f 6164 6361 7265 2e63 6f6d 272c  uploadcare.com',
-00001030: 0a20 2020 2027 7061 636b 6167 6573 273a  .    'packages':
-00001040: 2070 6163 6b61 6765 732c 0a20 2020 2027   packages,.    '
-00001050: 7061 636b 6167 655f 6461 7461 273a 2070  package_data': p
-00001060: 6163 6b61 6765 5f64 6174 612c 0a20 2020  ackage_data,.   
-00001070: 2027 696e 7374 616c 6c5f 7265 7175 6972   'install_requir
-00001080: 6573 273a 2069 6e73 7461 6c6c 5f72 6571  es': install_req
-00001090: 7569 7265 732c 0a20 2020 2027 6578 7472  uires,.    'extr
-000010a0: 6173 5f72 6571 7569 7265 273a 2065 7874  as_require': ext
-000010b0: 7261 735f 7265 7175 6972 652c 0a20 2020  ras_require,.   
-000010c0: 2027 656e 7472 795f 706f 696e 7473 273a   'entry_points':
-000010d0: 2065 6e74 7279 5f70 6f69 6e74 732c 0a20   entry_points,. 
-000010e0: 2020 2027 7079 7468 6f6e 5f72 6571 7569     'python_requi
-000010f0: 7265 7327 3a20 273e 3d33 2e36 2e32 2c3c  res': '>=3.6.2,<
-00001100: 342e 302e 3027 2c0a 7d0a 0a0a 7365 7475  4.0.0',.}...setu
-00001110: 7028 2a2a 7365 7475 705f 6b77 6172 6773  p(**setup_kwargs
-00001120: 290a                                     ).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7570  : 2.1.Name: pyup
+00000020: 6c6f 6164 6361 7265 0a56 6572 7369 6f6e  loadcare.Version
+00000030: 3a20 342e 312e 300a 5375 6d6d 6172 793a  : 4.1.0.Summary:
+00000040: 2050 7974 686f 6e20 6c69 6272 6172 7920   Python library 
+00000050: 666f 7220 5570 6c6f 6164 6361 7265 2e63  for Uploadcare.c
+00000060: 6f6d 0a48 6f6d 652d 7061 6765 3a20 6874  om.Home-page: ht
+00000070: 7470 733a 2f2f 7570 6c6f 6164 6361 7265  tps://uploadcare
+00000080: 2e63 6f6d 0a41 7574 686f 723a 2055 706c  .com.Author: Upl
+00000090: 6f61 6463 6172 6520 496e 630a 4175 7468  oadcare Inc.Auth
+000000a0: 6f72 2d65 6d61 696c 3a20 6865 6c6c 6f40  or-email: hello@
+000000b0: 7570 6c6f 6164 6361 7265 2e63 6f6d 0a52  uploadcare.com.R
+000000c0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+000000d0: 3e3d 332e 362e 322c 3c34 2e30 2e30 0a43  >=3.6.2,<4.0.0.C
+000000e0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
+000000f0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000100: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+00000110: 5374 6162 6c65 0a43 6c61 7373 6966 6965  Stable.Classifie
+00000120: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000130: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000140: 7273 0a43 6c61 7373 6966 6965 723a 204c  rs.Classifier: L
+00000150: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000160: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000170: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
+00000180: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000190: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001d0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000200: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
+00000210: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000220: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000230: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000240: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000260: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000270: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000280: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000290: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+000002a0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002c0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
+000002d0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002f0: 2050 7974 686f 6e20 3a3a 2033 2e36 0a50   Python :: 3.6.P
+00000300: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
+00000310: 6a61 6e67 6f0a 5265 7175 6972 6573 2d44  jango.Requires-D
+00000320: 6973 743a 2044 6a61 6e67 6f20 283e 3d31  ist: Django (>=1
+00000330: 2e31 3129 203b 2065 7874 7261 203d 3d20  .11) ; extra == 
+00000340: 2264 6a61 6e67 6f22 0a52 6571 7569 7265  "django".Require
+00000350: 732d 4469 7374 3a20 6874 7470 7820 283e  s-Dist: httpx (>
+00000360: 3d30 2e31 382e 322c 3c30 2e31 392e 3029  =0.18.2,<0.19.0)
+00000370: 203b 2070 7974 686f 6e5f 7665 7273 696f   ; python_versio
+00000380: 6e20 3e3d 2022 332e 3622 2061 6e64 2070  n >= "3.6" and p
+00000390: 7974 686f 6e5f 7665 7273 696f 6e20 3c20  ython_version < 
+000003a0: 2233 2e37 220a 5265 7175 6972 6573 2d44  "3.7".Requires-D
+000003b0: 6973 743a 2068 7474 7078 2028 3e3d 302e  ist: httpx (>=0.
+000003c0: 3234 2e31 2c3c 302e 3235 2e30 2920 3b20  24.1,<0.25.0) ; 
+000003d0: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
+000003e0: 3d20 2233 2e37 2220 616e 6420 7079 7468  = "3.7" and pyth
+000003f0: 6f6e 5f76 6572 7369 6f6e 203c 2022 342e  on_version < "4.
+00000400: 3022 0a52 6571 7569 7265 732d 4469 7374  0".Requires-Dist
+00000410: 3a20 7079 6461 6e74 6963 5b65 6d61 696c  : pydantic[email
+00000420: 5d20 283e 3d31 2e38 2e32 2c3c 322e 302e  ] (>=1.8.2,<2.0.
+00000430: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000440: 3a20 7079 7468 6f6e 2d64 6174 6575 7469  : python-dateuti
+00000450: 6c20 283e 3d32 2e38 2e32 2c3c 332e 302e  l (>=2.8.2,<3.0.
+00000460: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000470: 3a20 7079 747a 2028 3e3d 3230 3232 2e34  : pytz (>=2022.4
+00000480: 2c3c 3230 3233 2e30 290a 5265 7175 6972  ,<2023.0).Requir
+00000490: 6573 2d44 6973 743a 2074 7970 696e 672d  es-Dist: typing-
+000004a0: 6578 7465 6e73 696f 6e73 2028 3e3d 332e  extensions (>=3.
+000004b0: 3130 2e30 2c3c 342e 302e 3029 203b 2070  10.0,<4.0.0) ; p
+000004c0: 7974 686f 6e5f 7665 7273 696f 6e20 3e3d  ython_version >=
+000004d0: 2022 332e 3622 2061 6e64 2070 7974 686f   "3.6" and pytho
+000004e0: 6e5f 7665 7273 696f 6e20 3c20 2233 2e37  n_version < "3.7
+000004f0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000500: 2074 7970 696e 672d 6578 7465 6e73 696f   typing-extensio
+00000510: 6e73 2028 3e3d 342e 332e 302c 3c35 2e30  ns (>=4.3.0,<5.0
+00000520: 2e30 2920 3b20 7079 7468 6f6e 5f76 6572  .0) ; python_ver
+00000530: 7369 6f6e 203e 3d20 2233 2e37 2220 616e  sion >= "3.7" an
+00000540: 6420 7079 7468 6f6e 5f76 6572 7369 6f6e  d python_version
+00000550: 203c 2022 342e 3022 0a50 726f 6a65 6374   < "4.0".Project
+00000560: 2d55 524c 3a20 4275 6720 5472 6163 6b65  -URL: Bug Tracke
+00000570: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
+00000580: 622e 636f 6d2f 7570 6c6f 6164 6361 7265  b.com/uploadcare
+00000590: 2f70 7975 706c 6f61 6463 6172 652f 6973  /pyuploadcare/is
+000005a0: 7375 6573 0a50 726f 6a65 6374 2d55 524c  sues.Project-URL
+000005b0: 3a20 5265 706f 7369 746f 7279 2c20 6874  : Repository, ht
+000005c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000005d0: 2f75 706c 6f61 6463 6172 652f 7079 7570  /uploadcare/pyup
+000005e0: 6c6f 6164 6361 7265 0a44 6573 6372 6970  loadcare.Descrip
+000005f0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000600: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000610: 0a0a 0a3c 7461 626c 653e 0a20 2020 203c  ...<table>.    <
+00000620: 7472 2073 7479 6c65 3d22 626f 7264 6572  tr style="border
+00000630: 3a20 6e6f 6e65 3b22 3e0a 2020 2020 2020  : none;">.      
+00000640: 2020 3c74 6420 7374 796c 653d 2262 6f72    <td style="bor
+00000650: 6465 723a 206e 6f6e 653b 223e 0a20 2020  der: none;">.   
+00000660: 2020 2020 2020 2020 203c 696d 6720 7372           <img sr
+00000670: 633d 2268 7474 7073 3a2f 2f75 6361 7265  c="https://ucare
+00000680: 6364 6e2e 636f 6d2f 3266 3438 3634 6237  cdn.com/2f4864b7
+00000690: 2d65 6430 652d 3434 3131 2d39 3635 622d  -ed0e-4411-965b-
+000006a0: 3831 3438 3632 3361 6136 3830 2f2d 2f69  8148623aa680/-/i
+000006b0: 6e6c 696e 652f 7965 732f 7570 6c6f 6164  nline/yes/upload
+000006c0: 6361 7265 2d6c 6f67 6f2d 6d61 726b 2e73  care-logo-mark.s
+000006d0: 7667 2220 7461 7267 6574 3d22 2220 7769  vg" target="" wi
+000006e0: 6474 683d 2236 3422 2068 6569 6768 743d  dth="64" height=
+000006f0: 2236 3422 3e0a 2020 2020 2020 2020 3c2f  "64">.        </
+00000700: 7464 3e0a 2020 2020 2020 2020 3c74 6820  td>.        <th 
+00000710: 7374 796c 653d 2276 6572 7469 6361 6c2d  style="vertical-
+00000720: 616c 6967 6e3a 2063 656e 7465 723b 2062  align: center; b
+00000730: 6f72 6465 723a 206e 6f6e 653b 223e 0a20  order: none;">. 
+00000740: 2020 2020 2020 2020 2020 203c 6831 3e50             <h1>P
+00000750: 7955 706c 6f61 6463 6172 653a 2061 2050  yUploadcare: a P
+00000760: 7974 686f 6e20 6c69 6272 6172 7920 666f  ython library fo
+00000770: 7220 5570 6c6f 6164 6361 7265 3c2f 6831  r Uploadcare</h1
+00000780: 3e0a 2020 2020 2020 2020 3c2f 7468 3e0a  >.        </th>.
+00000790: 2020 2020 3c2f 7472 3e0a 3c2f 7461 626c      </tr>.</tabl
+000007a0: 653e 0a0a 3c70 3e0a 2020 3c61 2068 7265  e>..<p>.  <a hre
+000007b0: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+000007c0: 6f72 672f 7072 6f6a 6563 742f 7079 7570  org/project/pyup
+000007d0: 6c6f 6164 6361 7265 2f22 3e0a 2020 2020  loadcare/">.    
+000007e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000007f0: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000800: 7079 2f70 7975 706c 6f61 6463 6172 652e  py/pyuploadcare.
+00000810: 7376 6722 2068 6569 6768 743d 2232 3522  svg" height="25"
+00000820: 202f 3e0a 2020 3c2f 613e 0a20 203c 6120   />.  </a>.  <a 
+00000830: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000840: 7468 7562 2e63 6f6d 2f75 706c 6f61 6463  thub.com/uploadc
+00000850: 6172 652f 7079 7570 6c6f 6164 6361 7265  are/pyuploadcare
+00000860: 2f61 6374 696f 6e73 3f71 7565 7279 3d62  /actions?query=b
+00000870: 7261 6e63 6825 3341 6d61 696e 2b77 6f72  ranch%3Amain+wor
+00000880: 6b66 6c6f 7725 3341 5465 7374 732b 2b22  kflow%3ATests++"
+00000890: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+000008a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000008b0: 6f6d 2f75 706c 6f61 6463 6172 652f 7079  om/uploadcare/py
+000008c0: 7570 6c6f 6164 6361 7265 2f61 6374 696f  uploadcare/actio
+000008d0: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+000008e0: 742e 796d 6c2f 6261 6467 652e 7376 6722  t.yml/badge.svg"
+000008f0: 2068 6569 6768 743d 2232 3522 202f 3e0a   height="25" />.
+00000900: 2020 3c2f 613e 0a20 203c 6120 6872 6566    </a>.  <a href
+00000910: 3d22 6874 7470 733a 2f2f 7079 7570 6c6f  ="https://pyuplo
+00000920: 6164 6361 7265 2e72 6561 6474 6865 646f  adcare.readthedo
+00000930: 6373 2e69 6f2f 223e 0a20 2020 203c 696d  cs.io/">.    <im
+00000940: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000950: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
+00000960: 726f 6a65 6374 732f 7079 7570 6c6f 6164  rojects/pyupload
+00000970: 6361 7265 2f62 6164 6765 2f3f 7665 7273  care/badge/?vers
+00000980: 696f 6e3d 6c61 7465 7374 2220 6865 6967  ion=latest" heig
+00000990: 6874 3d22 3235 2220 2f3e 0a20 203c 2f61  ht="25" />.  </a
+000009a0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+000009b0: 7073 3a2f 2f73 7461 636b 7368 6172 652e  ps://stackshare.
+000009c0: 696f 2f75 706c 6f61 6463 6172 6522 3e0a  io/uploadcare">.
+000009d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000009e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000009f0: 732e 696f 2f62 6164 6765 2f74 6563 682d  s.io/badge/tech-
+00000a00: 7374 6163 6b2d 3036 3930 6661 2e73 7667  stack-0690fa.svg
+00000a10: 3f73 7479 6c65 3d66 6c61 7422 2068 6569  ?style=flat" hei
+00000a20: 6768 743d 2232 3522 202f 3e0a 2020 3c2f  ght="25" />.  </
+00000a30: 613e 0a3c 2f70 3e0a 0a55 706c 6f61 6463  a>.</p>..Uploadc
+00000a40: 6172 6520 5079 7468 6f6e 2026 2044 6a61  are Python & Dja
+00000a50: 6e67 6f20 696e 7465 6772 6174 696f 6e73  ngo integrations
+00000a60: 2068 616e 646c 6520 7570 6c6f 6164 7320   handle uploads 
+00000a70: 616e 6420 6675 7274 6865 7220 6f70 6572  and further oper
+00000a80: 6174 696f 6e73 0a77 6974 6820 6669 6c65  ations.with file
+00000a90: 7320 6279 2077 7261 7070 696e 6720 5570  s by wrapping Up
+00000aa0: 6c6f 6164 2061 6e64 2052 4553 5420 4150  load and REST AP
+00000ab0: 4973 2e0a 0a53 696d 706c 6520 6669 6c65  Is...Simple file
+00000ac0: 2075 706c 6f61 6473 2066 6f72 2074 6865   uploads for the
+00000ad0: 2077 6562 2061 7265 206f 6620 6d6f 7374   web are of most
+00000ae0: 2069 6d70 6f72 7461 6e63 6520 666f 7220   importance for 
+00000af0: 7573 2e20 546f 6461 792c 2065 7665 7279  us. Today, every
+00000b00: 6f6e 650a 6973 2075 7365 6420 746f 2074  one.is used to t
+00000b10: 6865 2072 6f75 7469 6e65 206f 6620 616c  he routine of al
+00000b20: 6c6f 7769 6e67 2075 7365 7273 2074 6f20  lowing users to 
+00000b30: 7570 6c6f 6164 2074 6865 6972 2070 6963  upload their pic
+00000b40: 7320 6f72 2061 7474 6163 6820 7265 7375  s or attach resu
+00000b50: 6d65 732e 0a54 6865 2072 6f75 7469 6e65  mes..The routine
+00000b60: 2063 6f76 6572 7320 6974 2061 6c6c 3a20   covers it all: 
+00000b70: 696e 7374 616c 6c69 6e67 2069 6d61 6765  installing image
+00000b80: 2070 726f 6365 7373 696e 6720 6c69 6272   processing libr
+00000b90: 6172 6965 732c 2061 646a 7573 7469 6e67  aries, adjusting
+00000ba0: 0a70 6572 6d69 7373 696f 6e73 2c20 656e  .permissions, en
+00000bb0: 7375 7269 6e67 2073 6572 7665 7273 206e  suring servers n
+00000bc0: 6576 6572 2067 6f20 646f 776e 2c20 616e  ever go down, an
+00000bd0: 6420 656e 6162 6c69 6e67 2043 444e 2e0a  d enabling CDN..
+00000be0: 0a54 6869 7320 6c69 6272 6172 7920 636f  .This library co
+00000bf0: 6e73 6973 7473 206f 6620 7468 6520 5570  nsists of the Up
+00000c00: 6c6f 6164 6361 7265 2041 5049 2069 6e74  loadcare API int
+00000c10: 6572 6661 6365 2061 6e64 2061 2063 6f75  erface and a cou
+00000c20: 706c 6520 6f66 2044 6a61 6e67 6f0a 676f  ple of Django.go
+00000c30: 6f64 6965 732e 0a0a 5369 6d70 6c65 2061  odies...Simple a
+00000c40: 7320 7468 6174 2c20 5570 6c6f 6164 6361  s that, Uploadca
+00000c50: 7265 2060 496d 6167 6546 6965 6c64 6020  re `ImageField` 
+00000c60: 6361 6e20 6265 2061 6464 6564 2074 6f20  can be added to 
+00000c70: 616e 0a65 7869 7374 696e 6720 446a 616e  an.existing Djan
+00000c80: 676f 2070 726f 6a65 6374 2069 6e20 6a75  go project in ju
+00000c90: 7374 2061 2063 6f75 706c 6520 6f66 205b  st a couple of [
+00000ca0: 7369 6d70 6c65 2073 7465 7073 5d28 6874  simple steps](ht
+00000cb0: 7470 733a 2f2f 7079 7570 6c6f 6164 6361  tps://pyuploadca
+00000cc0: 7265 2e72 6561 6474 6865 646f 6373 2e6f  re.readthedocs.o
+00000cd0: 7267 2f65 6e2f 6c61 7465 7374 2f71 7569  rg/en/latest/qui
+00000ce0: 636b 7374 6172 742e 6874 6d6c 292e 0a54  ckstart.html)..T
+00000cf0: 6869 7320 7769 6c6c 2065 6e61 626c 6520  his will enable 
+00000d00: 796f 7572 2075 7365 7273 2074 6f20 7365  your users to se
+00000d10: 6520 7468 6520 7570 6c6f 6164 2070 726f  e the upload pro
+00000d20: 6772 6573 732c 2070 6963 6b20 6669 6c65  gress, pick file
+00000d30: 730a 6672 6f6d 2047 6f6f 676c 6520 4472  s.from Google Dr
+00000d40: 6976 6520 6f72 2049 6e73 7461 6772 616d  ive or Instagram
+00000d50: 2c20 616e 6420 6564 6974 2061 2066 6f72  , and edit a for
+00000d60: 6d20 7768 696c 6520 6669 6c65 7320 6172  m while files ar
+00000d70: 650a 6265 696e 6720 7570 6c6f 6164 6564  e.being uploaded
+00000d80: 2061 7379 6e63 6872 6f6e 6f75 736c 792e   asynchronously.
+00000d90: 0a0a 596f 7520 6361 6e20 6669 6e64 2061  ..You can find a
+00000da0: 6e20 6578 616d 706c 6520 7072 6f6a 6563  n example projec
+00000db0: 7420 5b68 6572 655d 2868 7474 7073 3a2f  t [here](https:/
+00000dc0: 2f67 6974 6875 622e 636f 6d2f 7570 6c6f  /github.com/uplo
+00000dd0: 6164 6361 7265 2f70 7975 706c 6f61 6463  adcare/pyuploadc
+00000de0: 6172 652d 6578 616d 706c 6529 2e0a 0a60  are-example)...`
+00000df0: 6060 7079 7468 6f6e 0a0a 2020 2020 6672  ``python..    fr
+00000e00: 6f6d 2064 6a61 6e67 6f20 696d 706f 7274  om django import
+00000e10: 2066 6f72 6d73 0a20 2020 2066 726f 6d20   forms.    from 
+00000e20: 646a 616e 676f 2e64 6220 696d 706f 7274  django.db import
+00000e30: 206d 6f64 656c 730a 0a20 2020 2066 726f   models..    fro
+00000e40: 6d20 7079 7570 6c6f 6164 6361 7265 2e64  m pyuploadcare.d
+00000e50: 6a2e 6d6f 6465 6c73 2069 6d70 6f72 7420  j.models import 
+00000e60: 496d 6167 6546 6965 6c64 0a20 2020 2066  ImageField.    f
+00000e70: 726f 6d20 7079 7570 6c6f 6164 6361 7265  rom pyuploadcare
+00000e80: 2e64 6a2e 666f 726d 7320 696d 706f 7274  .dj.forms import
+00000e90: 2046 696c 6557 6964 6765 742c 2049 6d61   FileWidget, Ima
+00000ea0: 6765 4669 656c 6420 6173 2049 6d61 6765  geField as Image
+00000eb0: 466f 726d 4669 656c 640a 0a0a 2020 2020  FormField...    
+00000ec0: 636c 6173 7320 4361 6e64 6964 6174 6528  class Candidate(
+00000ed0: 6d6f 6465 6c73 2e4d 6f64 656c 293a 0a20  models.Model):. 
+00000ee0: 2020 2020 2020 2070 686f 746f 203d 2049         photo = I
+00000ef0: 6d61 6765 4669 656c 6428 626c 616e 6b3d  mageField(blank=
+00000f00: 5472 7565 2c20 6d61 6e75 616c 5f63 726f  True, manual_cro
+00000f10: 703d 2222 290a 0a0a 2020 2020 2320 6f70  p="")...    # op
+00000f20: 7469 6f6e 616c 2e20 7072 6f76 6964 6520  tional. provide 
+00000f30: 6164 7661 6e63 6564 2077 6964 6765 7420  advanced widget 
+00000f40: 6f70 7469 6f6e 733a 2068 7474 7073 3a2f  options: https:/
+00000f50: 2f75 706c 6f61 6463 6172 652e 636f 6d2f  /uploadcare.com/
+00000f60: 646f 6373 2f75 706c 6f61 6473 2f77 6964  docs/uploads/wid
+00000f70: 6765 742f 636f 6e66 6967 2f23 6f70 7469  get/config/#opti
+00000f80: 6f6e 730a 2020 2020 636c 6173 7320 4361  ons.    class Ca
+00000f90: 6e64 6964 6174 6546 6f72 6d28 666f 726d  ndidateForm(form
+00000fa0: 732e 466f 726d 293a 0a20 2020 2020 2020  s.Form):.       
+00000fb0: 2070 686f 746f 203d 2049 6d61 6765 466f   photo = ImageFo
+00000fc0: 726d 4669 656c 6428 7769 6467 6574 3d46  rmField(widget=F
+00000fd0: 696c 6557 6964 6765 7428 6174 7472 733d  ileWidget(attrs=
+00000fe0: 7b0a 2020 2020 2020 2020 2020 2020 2764  {.            'd
+00000ff0: 6174 612d 6364 6e2d 6261 7365 273a 2027  ata-cdn-base': '
+00001000: 6874 7470 733a 2f2f 6364 6e2e 7375 7065  https://cdn.supe
+00001010: 722d 6361 6e64 6964 6174 6573 2e63 6f6d  r-candidates.com
+00001020: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00001030: 6461 7461 2d69 6d61 6765 2d73 6872 696e  data-image-shrin
+00001040: 6b27 3a20 2731 3032 3478 3130 3234 272c  k': '1024x1024',
+00001050: 0a20 2020 2020 2020 207d 2929 0a0a 6060  .        }))..``
+00001060: 600a 0a21 5b5d 2868 7474 7073 3a2f 2f75  `..![](https://u
+00001070: 6361 7265 6364 6e2e 636f 6d2f 6462 6234  carecdn.com/dbb4
+00001080: 3032 3165 2d62 3230 652d 3430 6661 2d39  021e-b20e-40fa-9
+00001090: 3037 622d 3364 6130 6134 6638 6564 3730  07b-3da0a4f8ed70
+000010a0: 2f2d 2f72 6573 697a 652f 3830 302f 6d61  /-/resize/800/ma
+000010b0: 6e75 616c 5f63 726f 702e 706e 6729 0a0a  nual_crop.png)..
+000010c0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
+000010d0: 0a0a 4465 7461 696c 6564 2064 6f63 756d  ..Detailed docum
+000010e0: 656e 7461 7469 6f6e 2069 7320 6176 6169  entation is avai
+000010f0: 6c61 626c 6520 5b6f 6e20 5254 445d 2868  lable [on RTD](h
+00001100: 7474 7073 3a2f 2f70 7975 706c 6f61 6463  ttps://pyuploadc
+00001110: 6172 652e 7265 6164 7468 6564 6f63 732e  are.readthedocs.
+00001120: 696f 2f65 6e2f 6c61 7465 7374 2f29 2e0a  io/en/latest/)..
+00001130: 0a23 2320 4665 6564 6261 636b 0a0a 4973  .## Feedback..Is
+00001140: 7375 6573 2061 6e64 2050 5273 2061 7265  sues and PRs are
+00001150: 2077 656c 636f 6d65 2e20 596f 7520 6361   welcome. You ca
+00001160: 6e20 7072 6f76 6964 6520 796f 7572 2066  n provide your f
+00001170: 6565 6462 6163 6b20 6f72 2064 726f 7020  eedback or drop 
+00001180: 7573 2061 2073 7570 706f 7274 0a72 6571  us a support.req
+00001190: 7565 7374 2061 7420 5b68 656c 6c6f 4075  uest at [hello@u
+000011a0: 706c 6f61 6463 6172 652e 636f 6d5d 2868  ploadcare.com](h
+000011b0: 656c 6c6f 4075 706c 6f61 6463 6172 652e  ello@uploadcare.
+000011c0: 636f 6d29 2e0a 0a                        com)...
```

