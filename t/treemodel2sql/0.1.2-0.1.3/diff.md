# Comparing `tmp/treemodel2sql-0.1.2.tar.gz` & `tmp/treemodel2sql-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treemodel2sql-0.1.2.tar", last modified: Mon Jul 17 12:57:51 2023, max compression
+gzip compressed data, was "dist/treemodel2sql-0.1.3.tar", last modified: Tue Jul 18 13:11:19 2023, max compression
```

## Comparing `treemodel2sql-0.1.2.tar` & `treemodel2sql-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.editorconfig
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/.github/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      324 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.gitignore
--rw-r--r--   0 ryanzheng   (501) staff       (20)      693 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/.travis.yml
--rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/AUTHORS.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3583 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-07-17 12:54:41.000000 treemodel2sql-0.1.2/HISTORY.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/LICENSE
--rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/MANIFEST.in
--rw-r--r--   0 ryanzheng   (501) staff       (20)     2301 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)    32641 2023-07-17 12:39:53.000000 treemodel2sql-0.1.2/README.md
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/docs/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      614 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/authors.rst
--rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4847 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/conf.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/contributing.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/history.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      310 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/index.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1166 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/installation.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      811 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/make.bat
--rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/readme.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       81 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/docs/usage.rst
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/examples/
--rw-r--r--   0 ryanzheng   (501) staff       (20)   115765 2023-07-17 12:40:38.000000 treemodel2sql-0.1.2/examples/tutorial_code_lightgbm_model_transform_sql.ipynb
--rw-r--r--   0 ryanzheng   (501) staff       (20)   100911 2023-07-17 12:40:39.000000 treemodel2sql-0.1.2/examples/tutorial_code_xgboost_model_transform_sql.ipynb
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/images/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    39768 2023-06-11 07:05:08.000000 treemodel2sql-0.1.2/images/干饭人.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)    27731 2023-06-10 10:02:05.000000 treemodel2sql-0.1.2/images/魔都数据干饭人.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)       26 2023-07-16 14:06:54.000000 treemodel2sql-0.1.2/requirements.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)      430 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/setup.cfg
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1710 2023-07-17 12:54:31.000000 treemodel2sql-0.1.2/setup.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/tests/
--rw-r--r--   0 ryanzheng   (501) staff       (20)       43 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/tests/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)      571 2023-07-15 14:18:03.000000 treemodel2sql-0.1.2/tests/test_treemodel2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      200 2023-07-17 12:54:28.000000 treemodel2sql-0.1.2/treemodel2sql/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4656 2023-07-16 05:19:29.000000 treemodel2sql-0.1.2/treemodel2sql/lgb2sql.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     7583 2023-06-11 02:53:26.000000 treemodel2sql-0.1.2/treemodel2sql/xgboost2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)      898 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       57 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/not-zip-safe
--rw-r--r--   0 ryanzheng   (501) staff       (20)       25 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/requires.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       14 2023-07-17 12:57:51.000000 treemodel2sql-0.1.2/treemodel2sql.egg-info/top_level.txt
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/.editorconfig
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/.github/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      324 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/.gitignore
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      693 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/.travis.yml
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/AUTHORS.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3583 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-07-18 13:09:11.000000 treemodel2sql-0.1.3/HISTORY.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/LICENSE
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/MANIFEST.in
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     2301 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    32641 2023-07-17 12:39:53.000000 treemodel2sql-0.1.3/README.md
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/docs/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      614 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/authors.rst
+-rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4847 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/conf.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/contributing.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/history.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      310 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/index.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1166 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/installation.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      811 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/make.bat
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/readme.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       81 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/docs/usage.rst
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/examples/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   115765 2023-07-17 12:40:38.000000 treemodel2sql-0.1.3/examples/tutorial_code_lightgbm_model_transform_sql.ipynb
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   100911 2023-07-17 12:40:39.000000 treemodel2sql-0.1.3/examples/tutorial_code_xgboost_model_transform_sql.ipynb
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/images/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    39768 2023-06-11 07:05:08.000000 treemodel2sql-0.1.3/images/干饭人.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    27731 2023-06-10 10:02:05.000000 treemodel2sql-0.1.3/images/魔都数据干饭人.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       26 2023-07-16 14:06:54.000000 treemodel2sql-0.1.3/requirements.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      430 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/setup.cfg
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1710 2023-07-18 13:09:07.000000 treemodel2sql-0.1.3/setup.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/tests/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       43 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/tests/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      571 2023-07-15 14:18:03.000000 treemodel2sql-0.1.3/tests/test_treemodel2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      200 2023-07-18 13:09:07.000000 treemodel2sql-0.1.3/treemodel2sql/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     6341 2023-07-18 13:06:12.000000 treemodel2sql-0.1.3/treemodel2sql/lgb2sql.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     9458 2023-07-18 13:07:16.000000 treemodel2sql-0.1.3/treemodel2sql/xgboost2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33383 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      898 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       57 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/not-zip-safe
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       25 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/requires.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       14 2023-07-18 13:11:19.000000 treemodel2sql-0.1.3/treemodel2sql.egg-info/top_level.txt
```

### Comparing `treemodel2sql-0.1.2/.gitignore` & `treemodel2sql-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/.travis.yml` & `treemodel2sql-0.1.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/CONTRIBUTING.rst` & `treemodel2sql-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/LICENSE` & `treemodel2sql-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/Makefile` & `treemodel2sql-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/PKG-INFO` & `treemodel2sql-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treemodel2sql
-Version: 0.1.2
+Version: 0.1.3
 Summary: tree model transform to sql
 Home-page: https://github.com/ZhengRyan/treemodel2sql
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Keywords: treemodel2sql
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `treemodel2sql-0.1.2/README.md` & `treemodel2sql-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/docs/Makefile` & `treemodel2sql-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/docs/conf.py` & `treemodel2sql-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/docs/installation.rst` & `treemodel2sql-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/docs/make.bat` & `treemodel2sql-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/examples/tutorial_code_lightgbm_model_transform_sql.ipynb` & `treemodel2sql-0.1.3/examples/tutorial_code_lightgbm_model_transform_sql.ipynb`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/examples/tutorial_code_xgboost_model_transform_sql.ipynb` & `treemodel2sql-0.1.3/examples/tutorial_code_xgboost_model_transform_sql.ipynb`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/images/干饭人.png` & `treemodel2sql-0.1.3/images/干饭人.png`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/images/魔都数据干饭人.png` & `treemodel2sql-0.1.3/images/魔都数据干饭人.png`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/setup.py` & `treemodel2sql-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     include_package_data=True,
     keywords='treemodel2sql',
     name=NAME,
     packages=find_packages(include=['treemodel2sql', 'treemodel2sql.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZhengRyan/treemodel2sql',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `treemodel2sql-0.1.2/tests/test_treemodel2sql.py` & `treemodel2sql-0.1.3/tests/test_treemodel2sql.py`

 * *Files identical despite different names*

### Comparing `treemodel2sql-0.1.2/treemodel2sql/lgb2sql.py` & `treemodel2sql-0.1.3/treemodel2sql/lgb2sql.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         select {0},
         {3}
         from {4})
         '''
 
     feature_names = []
 
-    def transform(self, lgb_model, keep_columns=['key'], table_name='data_table'):
+    def transform(self, lgb_model, keep_columns=['key'], table_name='data_table', sql_is_format=True):
         """
 
         Args:
             lightgbm_model:训练好的lightgbm模型
             keep_columns:使用sql语句进行预测时，需要保留的列。默认主键保留
             table_name:待预测数据集的表名
 
@@ -43,15 +43,15 @@
         logit = -0.0
 
         # 解析的逻辑
         trees_func_code_l = []
         columns_l = []
 
         for i, tree in enumerate(trees):
-            one_tree_code = self.pre_tree(tree['tree_structure'], 1)
+            one_tree_code = self.pre_tree(tree['tree_structure'], 1, sql_is_format)
             if i == len(trees) - 1:
                 trees_func_code_l.append(
                     '--tree' + str(i) + '\n' + one_tree_code + '\n' + '\t\tas tree_{}_score'.format(i))
             else:
                 trees_func_code_l.append(
                     '--tree' + str(i) + '\n' + one_tree_code + '\n' + '\t\tas tree_{}_score,\n'.format(i))
 
@@ -71,27 +71,27 @@
         Returns:
 
         """
         if isinstance(lgb_model, lightgbm.LGBMClassifier):
             lgb_model = lgb_model._Booster
         return lgb_model.dump_model()
 
-    def pre_tree(self, node, n):
+    def pre_tree(self, node, n, sql_is_format=True):
         """
 
         Args:
             node:树结构
             n:第几层
 
         Returns:
 
         """
         n += 1
         if 'leaf_index' in node:
-            return '\t' * n + str(node['leaf_value'])
+            return '\t' * n + str(node['leaf_value']) if sql_is_format else node['leaf_value']
 
         condition = []
         split_feature = self.feature_names[node['split_feature']]
         is_default_left = node['default_left']
 
         if node['decision_type'] == '<=' or node['decision_type'] == 'no_greater':
             threshold = node['threshold']
@@ -102,19 +102,22 @@
         else:
             threshold = node['threshold']
             if 'e' in str(threshold):
                 threshold = format(threshold, 'f')
             condition.append(
                 f'{split_feature} is null and {str(is_default_left).lower()}==false or {split_feature}=={threshold}')
 
-        left = self.pre_tree(node['left_child'], n)
-        right = self.pre_tree(node['right_child'], n)
+        left = self.pre_tree(node['left_child'], n, sql_is_format)
+        right = self.pre_tree(node['right_child'], n, sql_is_format)
 
-        strformat = '\t' * n
-        return f'{strformat}case when ({condition[0]}) then\n{left}\n{strformat}else\n{right}\n{strformat}end'
+        if sql_is_format:
+            strformat = '\t' * n
+            return f'{strformat}case when ({condition[0]}) then\n{left}\n{strformat}else\n{right}\n{strformat}end'
+        else:
+            return f'case when ({condition[0]}) then {left} else {right} end'
 
     def save(self, filename='lgb_model.sql'):
         """
 
         Args:
             filename:sql语句保存的位置
 
@@ -146,10 +149,43 @@
     ###训练模型
     model = lgb.LGBMClassifier(n_estimators=3)
     model.fit(X_train, y_train)
     lgb.create_tree_digraph(model._Booster, tree_index=0)
 
     ###使用treemodel2sql包将模型转换成的sql语句
     lgb2sql = Lgb2Sql()
-    sql_str = lgb2sql.transform(model)
+    #sql_str = lgb2sql.transform(model)
+    sql_str = lgb2sql.transform(model,sql_is_format=False)
     print(sql_str)
-    lgb2sql.save()
+    #lgb2sql.save()
+
+    import pandas as pd
+
+    pd.set_option('display.float_format', lambda x: '%.9f' % x)
+    ###使用模型对测试数据集进行预测
+    test_pred = model.predict_proba(X_test)[:, 1]
+    test_pred = pd.DataFrame(test_pred, columns=['python_pred_res'])
+    test_pred.reset_index(inplace=True)
+    test_pred.rename(columns={'index': 'key'}, inplace=True)
+    print(test_pred)
+
+    ###使用模型转换成的sql语句对测试数据集进行预测
+    from pyspark.sql import SparkSession
+
+    spark = SparkSession.builder.getOrCreate()
+
+    X_test_df = pd.DataFrame(X_test)
+    X_test_df.columns = X_test_df.columns.map(lambda x: "Column_" + str(x))
+    X_test_df.reset_index(inplace=True)
+    X_test_df.rename(columns={'index': 'key'}, inplace=True)
+    values = X_test_df.values.tolist()
+    columns = X_test_df.columns.tolist()
+    spark_df = spark.createDataFrame(values, columns)
+    spark_df.createOrReplaceTempView('data_table')
+    sql_pred_pysdf = spark.sql(sql_str)
+    sql_pred_df = sql_pred_pysdf.toPandas()
+    sql_pred_df.head(2)
+
+    ###对比python模型预测出来的结果和sql语句预测出来的结果是否一致
+    test_pred_sql_pred_df = test_pred.merge(sql_pred_df, on='key')
+    test_pred_sql_pred_df['diff'] = test_pred_sql_pred_df['python_pred_res'] - test_pred_sql_pred_df['score']
+    print(test_pred_sql_pred_df['diff'].describe())
```

### Comparing `treemodel2sql-0.1.2/treemodel2sql.egg-info/PKG-INFO` & `treemodel2sql-0.1.3/treemodel2sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treemodel2sql
-Version: 0.1.2
+Version: 0.1.3
 Summary: tree model transform to sql
 Home-page: https://github.com/ZhengRyan/treemodel2sql
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Keywords: treemodel2sql
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `treemodel2sql-0.1.2/treemodel2sql.egg-info/SOURCES.txt` & `treemodel2sql-0.1.3/treemodel2sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

