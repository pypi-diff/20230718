# Comparing `tmp/vgis_utils-1.0.8.tar.gz` & `tmp/vgis_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.8.tar", last modified: Thu Jul  6 07:12:14 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.0.9.tar", last modified: Tue Jul 11 10:45:28 2023, max compression
```

## Comparing `vgis_utils-1.0.8.tar` & `vgis_utils-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.495675 vgis_utils-1.0.8/
--rw-rw-rw-   0        0        0     1034 2023-07-06 07:12:14.494671 vgis_utils-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 07:12:14.495675 vgis_utils-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2200 2023-07-06 07:10:53.000000 vgis_utils-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.462638 vgis_utils-1.0.8/vgis_utils/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.8/vgis_utils/commonTools.py
--rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.8/vgis_utils/iteratorTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.473639 vgis_utils-1.0.8/vgis_utils/vgis_datetime/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_datetime/__init__.py
--rw-rw-rw-   0        0        0     8245 2023-07-06 07:08:32.000000 vgis_utils-1.0.8/vgis_utils/vgis_datetime/datetimeTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.475650 vgis_utils-1.0.8/vgis_utils/vgis_file/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_file/__init__.py
--rw-rw-rw-   0        0        0     8364 2023-07-06 02:09:51.000000 vgis_utils-1.0.8/vgis_utils/vgis_file/fileTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.478639 vgis_utils-1.0.8/vgis_utils/vgis_http/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_http/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.8/vgis_utils/vgis_http/httpTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.481639 vgis_utils-1.0.8/vgis_utils/vgis_image/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_image/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.8/vgis_utils/vgis_image/imageTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.484638 vgis_utils-1.0.8/vgis_utils/vgis_list/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/vgis_list/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-06-27 06:37:50.000000 vgis_utils-1.0.8/vgis_utils/vgis_list/listTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.487638 vgis_utils-1.0.8/vgis_utils/vgis_money/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/vgis_money/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.0.8/vgis_utils/vgis_money/moneyTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.490665 vgis_utils-1.0.8/vgis_utils/vgis_string/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.8/vgis_utils/vgis_string/__init__.py
--rw-rw-rw-   0        0        0     3238 2023-07-06 07:09:21.000000 vgis_utils-1.0.8/vgis_utils/vgis_string/stringTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.493640 vgis_utils-1.0.8/vgis_utils/vgis_video/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.8/vgis_utils/vgis_video/__init__.py
--rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.8/vgis_utils/vgis_video/videoTools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:12:14.470640 vgis_utils-1.0.8/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 07:12:14.000000 vgis_utils-1.0.8/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.177571 vgis_utils-1.0.9/
+-rw-rw-rw-   0        0        0     1034 2023-07-11 10:45:28.176571 vgis_utils-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:45:28.177571 vgis_utils-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2200 2023-07-11 10:44:52.000000 vgis_utils-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:27.992243 vgis_utils-1.0.9/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.9/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.9/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.028210 vgis_utils-1.0.9/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     8245 2023-07-06 07:08:32.000000 vgis_utils-1.0.9/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.050211 vgis_utils-1.0.9/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8345 2023-07-10 02:56:16.000000 vgis_utils-1.0.9/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.072210 vgis_utils-1.0.9/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.9/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.093238 vgis_utils-1.0.9/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.9/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.110211 vgis_utils-1.0.9/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-07-11 10:42:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.113211 vgis_utils-1.0.9/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.0.9/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.135058 vgis_utils-1.0.9/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/vgis_string/__init__.py
+-rw-rw-rw-   0        0        0     3353 2023-07-07 09:32:52.000000 vgis_utils-1.0.9/vgis_utils/vgis_string/stringTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.160573 vgis_utils-1.0.9/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.9/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.025211 vgis_utils-1.0.9/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.8/PKG-INFO` & `vgis_utils-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.8/setup.py` & `vgis_utils-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.8",  # Required 发布版本号
+    version="1.0.9",  # Required 发布版本号
     description="A libary for common operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisUtils",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_utils-1.0.8/vgis_utils/commonTools.py` & `vgis_utils-1.0.9/vgis_utils/commonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils/iteratorTools.py` & `vgis_utils-1.0.9/vgis_utils/iteratorTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_datetime/datetimeTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_datetime/datetimeTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_file/fileTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_file/fileTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,31 @@
 
 
 class FileHelper:
     # 初始化
     def __init__(self):
         pass
 
-
     # 根据路径创建文件夹
     @staticmethod
     def mkdir(path):
         folder = os.path.exists(path)
         # 判断是否存在文件夹如果不存在则创建为文件夹
         if not folder:
             # 创建文件时如果路径不存在会创建这个路径
             os.makedirs(path)
 
     # 清空路径文件夹下所有文件
     @staticmethod
-    def rmdir( img_dir):
+    def rmdir(img_dir):
         images = os.listdir(img_dir)
         for name in images:
             img_path = os.path.join(img_dir, name)
             os.remove(img_path)
 
-
     # 删除临时目录，包括其下面的文件
     @staticmethod
     def delete_tmp_dir(dir_path):
         common_utity = CommonHelper()
         for i in os.listdir(dir_path):
             file_data = dir_path + common_utity.get_dash_in_system()
             if os.path.isfile(file_data) is True:
@@ -62,15 +60,15 @@
             if os.path.isdir(c_path):
                 FileHelper.del_file(c_path)
             else:
                 os.remove(c_path)
 
     # 用于复制目录下所有文件到另一个目录
     @staticmethod
-    def copy_allfiles( src, dest):
+    def copy_allfiles(src, dest):
         src_files = os.listdir(src)
 
         # 创建输出目录
         FileHelper.mkdir(dest)
 
         for file_name in src_files:
             full_file_name = os.path.join(src, file_name)
@@ -81,64 +79,63 @@
     @staticmethod
     def get_file_name(orgin_file_path):
         (file_pre_path, temp_filename) = os.path.split(orgin_file_path)
         return temp_filename
 
     # 得到文件名称的前缀
     @staticmethod
-    def get_file_name_prefix( orgin_file_path):
+    def get_file_name_prefix(orgin_file_path):
         (file_pre_path, temp_filename) = os.path.split(orgin_file_path)
         (shot_name, file_ext) = os.path.splitext(temp_filename)
         return shot_name
 
     # 得到文件名称的后缀
     @staticmethod
-    def get_file_name_suffix( orgin_file_path):
+    def get_file_name_suffix(orgin_file_path):
         (file_pre_path, temp_filename) = os.path.split(orgin_file_path)
         (shot_name, file_ext) = os.path.splitext(temp_filename)
         return file_ext
 
     # 为文件增加副本，按照给出的后缀名
     @staticmethod
-    def get_new_file_path_add_suffix( orgin_file_path, suffix_name):
+    def get_new_file_path_add_suffix(orgin_file_path, suffix_name):
         (file_pre_path, temp_filename) = os.path.split(orgin_file_path)
         (shot_name, file_ext) = os.path.splitext(temp_filename)
         common_utity = CommonHelper()
         bak_file_path = file_pre_path + common_utity.get_dash_in_system() + shot_name + "_" + suffix_name + file_ext
         return bak_file_path
 
-
     # 在目标文件路径下创建临时目录,并返回路径
     @staticmethod
-    def make_tmp_dir_onside_file( dest_file_path):
+    def make_tmp_dir_onside_file(dest_file_path):
         common_utity = CommonHelper()
         (file_pre_path, temp_filename) = os.path.split(dest_file_path)
         tmp_path = file_pre_path + common_utity.get_dash_in_system() + common_utity.get_uuid()
         # print("创建临时文件夹{}".format(tmp_path))
         os.makedirs(tmp_path)
         return tmp_path
 
     # 在目标文件路径下创建临时目录,并返回路径、
     @staticmethod
-    def make_tmp_dir_under_dir( dest_dir_path):
+    def make_tmp_dir_under_dir(dest_dir_path):
         common_utity = CommonHelper()
         tmp_path = dest_dir_path + common_utity.get_dash_in_system() + common_utity.get_uuid()
         # print("创建临时文件夹{}".format(tmp_path))
         os.makedirs(tmp_path)
         return tmp_path
 
     # 得到文件路径中的最后一级目录名
     @staticmethod
     def get_last_dir_name_in_file_path(orgin_file_path):
         (file_pre_path, temp_filename) = os.path.split(orgin_file_path)
         return FileHelper.get_last_dir_name_in_dir_path(file_pre_path)
 
     # 获取目录路径中的最后一级目录名
     @staticmethod
-    def get_last_dir_name_in_dir_path( dir_path):
+    def get_last_dir_name_in_dir_path(dir_path):
         common_utity = CommonHelper()
         last_dir_name = dir_path[dir_path.rindex(common_utity.get_dash_in_system()) + len(
             common_utity.get_dash_in_system()):]
         return last_dir_name
 
     # 得到文件路径中的完整目录路径
     @staticmethod
@@ -153,15 +150,14 @@
         for temp in file_names:
             file = os.path.join(file_dir_path, temp)
             fname, ext = os.path.splitext(file)
             base_name = os.path.basename(fname)
             new_n = base_name + add_sub + ext
             os.rename(os.path.join(file_dir_path, temp), os.path.join(file_dir_path, new_n))
 
-
     # 清除文件内容
     @staticmethod
     def clear_file_content(file_path):
         with open(file_path, "w") as file:
             file.truncate(0)
 
     @staticmethod
@@ -186,18 +182,17 @@
                     # print('Copy %s'% filepath +' To ' + destinationfile)
                     # print('Delet %s to recycle bin.' % filepath)
                     # # 删除文件
                     # send2trash.send2trash(filepath)
                     # 复制该文件到指定目录
                     shutil.copy(filepath, destinationfile)
 
-
     # 创建zip文件
     @staticmethod
-    def make_zip( source_dir, output_filename):
+    def make_zip(source_dir, output_filename):
         zipf = zipfile.ZipFile(output_filename, 'w')
         pre_len = len(os.path.dirname(source_dir))
         for parent, dirnames, filenames in os.walk(source_dir):
             for filename in filenames:
                 pathfile = os.path.join(parent, filename)
                 arcname = pathfile[pre_len:].strip(os.path.sep)  # 相对路径
                 zipf.write(pathfile, arcname)
```

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_http/httpTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_http/httpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_image/imageTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_image/imageTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_list/listTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_list/listTools.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,8 +81,16 @@
     def convert_all_list_into_one_list( all_data_record_list):
         result_data_list = []
         for each_data_record_list in all_data_record_list:
             for data_field_value_obj in each_data_record_list:
                 result_data_list.append(data_field_value_obj)
         return result_data_list
 
+    @staticmethod
+    def get_number_str_by_list(num_list):
+        number_str = ""
+        for num in num_list:
+            number_str = number_str + str(num) + ","
+        number_str = number_str.rstrip(",")
+        return number_str
+
```

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_money/moneyTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_money/moneyTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_string/stringTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_string/stringTools.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,13 +86,18 @@
         # 利用正则匹配\x开头的特殊字符
         result = re.findall(r'\\x[a-f0-9]{2}', content)
         for x in result:
             # 替换找的的特殊字符
             content = content.replace(x, '')
         # 最后再解码
         content = content.encode('utf-8').decode('unicode_escape')
-        return content
+        return
+
+    @staticmethod
+    # 首字母小写
+    def decapitalize(string):
+        return string[:1].lower() + string[1:]
 
 if __name__ == '__main__':
     input_str = "中故宫eee中工"
     input_str = StringHelper.convert_hanzi_to_pinyin_in_str(input_str)
     print(input_str)
```

### Comparing `vgis_utils-1.0.8/vgis_utils/vgis_video/videoTools.py` & `vgis_utils-1.0.9/vgis_utils/vgis_video/videoTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.8/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.0.9/vgis_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.8/vgis_utils.egg-info/SOURCES.txt` & `vgis_utils-1.0.9/vgis_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

