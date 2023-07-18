# Comparing `tmp/yhgit-2.9.0.tar.gz` & `tmp/yhgit-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yhgit-2.9.0.tar", last modified: Thu Apr 20 11:31:08 2023, max compression
+gzip compressed data, was "yhgit-2.9.1.tar", last modified: Tue Jul 18 01:07:54 2023, max compression
```

## Comparing `yhgit-2.9.0.tar` & `yhgit-2.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-04-20 11:31:08.264033 yhgit-2.9.0/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     1062 2022-11-04 01:44:48.000000 yhgit-2.9.0/LICENSE.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-04-20 11:31:08.264222 yhgit-2.9.0/PKG-INFO
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     3709 2023-03-22 10:57:10.000000 yhgit-2.9.0/README.md
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       79 2023-04-20 11:31:08.264809 yhgit-2.9.0/setup.cfg
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     2113 2023-04-20 11:30:58.000000 yhgit-2.9.0/setup.py
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-04-20 11:31:08.260862 yhgit-2.9.0/yhgit/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       13 2023-01-11 03:34:32.000000 yhgit-2.9.0/yhgit/__init__.py
--rw-r--r--   0 fanguohuijack   (501) staff       (20)    62547 2023-04-20 11:29:46.000000 yhgit-2.9.0/yhgit/yhgit.py
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-04-20 11:31:08.263524 yhgit-2.9.0/yhgit.egg-info/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/PKG-INFO
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      249 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/SOURCES.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)        1 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/dependency_links.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       44 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/entry_points.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      116 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/requires.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)        6 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/top_level.txt
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-07-18 01:07:54.110069 yhgit-2.9.1/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     1062 2022-11-04 01:44:48.000000 yhgit-2.9.1/LICENSE.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-07-18 01:07:54.110317 yhgit-2.9.1/PKG-INFO
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     3709 2023-03-22 10:57:10.000000 yhgit-2.9.1/README.md
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       79 2023-07-18 01:07:54.111070 yhgit-2.9.1/setup.cfg
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     2113 2023-07-18 01:06:33.000000 yhgit-2.9.1/setup.py
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-07-18 01:07:54.107267 yhgit-2.9.1/yhgit/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       13 2023-01-11 03:34:32.000000 yhgit-2.9.1/yhgit/__init__.py
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)    62680 2023-07-18 01:06:13.000000 yhgit-2.9.1/yhgit/yhgit.py
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-07-18 01:07:54.109794 yhgit-2.9.1/yhgit.egg-info/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-07-18 01:07:54.000000 yhgit-2.9.1/yhgit.egg-info/PKG-INFO
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      249 2023-07-18 01:07:54.000000 yhgit-2.9.1/yhgit.egg-info/SOURCES.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)        1 2023-07-18 01:07:54.000000 yhgit-2.9.1/yhgit.egg-info/dependency_links.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       44 2023-07-18 01:07:54.000000 yhgit-2.9.1/yhgit.egg-info/entry_points.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      116 2023-07-18 01:07:54.000000 yhgit-2.9.1/yhgit.egg-info/requires.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)        6 2023-07-18 01:07:54.000000 yhgit-2.9.1/yhgit.egg-info/top_level.txt
```

### Comparing `yhgit-2.9.0/LICENSE.txt` & `yhgit-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yhgit-2.9.0/PKG-INFO` & `yhgit-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yhgit
-Version: 2.9.0
+Version: 2.9.1
 Summary: yh branch git manager util
 Home-page: http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git
 Author: yonghuifan21
 Author-email: jackfan1@yonghui.com
 License: MIT
 Download-URL: https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz
 Keywords: yhgit,git,yh
```

### Comparing `yhgit-2.9.0/README.md` & `yhgit-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `yhgit-2.9.0/setup.py` & `yhgit-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     packages=find_packages(),
     entry_points={
           'console_scripts': [
               'yhgit = yhgit.yhgit:main'
           ]
     },
     python_requires='>=3.7',
-    version='2.9.0',  # Start with a small number and increase it with every change you make
+    version='2.9.1',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='yh branch git manager util',  # Give a short description about your library
     author='yonghuifan21',  # Type in your name
     author_email='jackfan1@yonghui.com',  # Type in your E-Mail
     url='http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git',
     download_url='https://files.pythonhosted.org/packages/08/7d'
                  '/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz',  # I explain this
```

### Comparing `yhgit-2.9.0/yhgit/yhgit.py` & `yhgit-2.9.1/yhgit/yhgit.py`

 * *Files 1% similar despite different names*

```diff
@@ -999,15 +999,16 @@
     return pull_result
 
 
 # 基于podfileModule，提交模块开发分支代码
 def release_branch(module_list, include_list, tag_path, c_path, f_branch):
     """
     基于模块列表，合并对应开发分支代码到master并打新的tag
-    :param module_list: 模块列表
+    :param module_list: 所有模块列表
+    :param include_list: release的模块列表
     :param tag_path:  这些模块排除在外，不提交n_branch代码
     :param c_path: 当前运行分支
     :param f_branch: 配置的全局统一分支，每个模块可以单独配置分支
     :return: 返回操作成功的分支
     """
 
     index = 0
@@ -1243,14 +1244,16 @@
             debugInfo("本地modules为空，无法查看组件的状态")
             return
         if not os.path.exists(local_yaml_path):
             debugInfo("本地local_yaml_path为空，无法查看组件的状态")
             return
         podfile_module_data = yaml_data(local_yaml_path)
         local_dependenceList = podfile_module_data["dependencies"]
+        if local_dependenceList is None:
+            local_dependenceList = []
         # 转换成模型数组
         module_list = load_yaml(local_dependenceList)
         status_result = []
         invert_list = module_list
         if len(include_modules) > 0:
             invert_list = [i for i in module_list if i.module in include_modules]
```

### Comparing `yhgit-2.9.0/yhgit.egg-info/PKG-INFO` & `yhgit-2.9.1/yhgit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yhgit
-Version: 2.9.0
+Version: 2.9.1
 Summary: yh branch git manager util
 Home-page: http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git
 Author: yonghuifan21
 Author-email: jackfan1@yonghui.com
 License: MIT
 Download-URL: https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz
 Keywords: yhgit,git,yh
```

