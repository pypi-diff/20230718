# Comparing `tmp/tools_wzy-0.0.4.tar.gz` & `tmp/tools_wzy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools_wzy-0.0.4.tar", last modified: Tue Jul 18 02:52:08 2023, max compression
+gzip compressed data, was "tools_wzy-0.0.5.tar", last modified: Tue Jul 18 03:28:15 2023, max compression
```

## Comparing `tools_wzy-0.0.4.tar` & `tools_wzy-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:52:08.464372 tools_wzy-0.0.4/
--rw-rw-rw-   0        0        0      308 2023-07-18 02:52:08.463375 tools_wzy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 02:52:08.464372 tools_wzy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-07-18 02:51:21.000000 tools_wzy-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:52:08.460385 tools_wzy-0.0.4/tools_wzy/
--rw-rw-rw-   0        0        0        0 2023-07-13 09:07:59.000000 tools_wzy-0.0.4/tools_wzy/__init__.py
--rw-rw-rw-   0        0        0     9507 2023-07-17 06:15:57.000000 tools_wzy-0.0.4/tools_wzy/node_coverage.py
--rw-rw-rw-   0        0        0     5157 2023-07-18 02:41:09.000000 tools_wzy-0.0.4/tools_wzy/yolo_need.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:52:08.463375 tools_wzy-0.0.4/tools_wzy.egg-info/
--rw-rw-rw-   0        0        0      308 2023-07-18 02:52:08.000000 tools_wzy-0.0.4/tools_wzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-18 02:52:08.000000 tools_wzy-0.0.4/tools_wzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:52:08.000000 tools_wzy-0.0.4/tools_wzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 02:52:08.000000 tools_wzy-0.0.4/tools_wzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 02:52:08.000000 tools_wzy-0.0.4/tools_wzy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:15.534023 tools_wzy-0.0.5/
+-rw-rw-rw-   0        0        0      308 2023-07-18 03:28:15.533026 tools_wzy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 03:28:15.534023 tools_wzy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-07-18 03:27:45.000000 tools_wzy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:15.530036 tools_wzy-0.0.5/tools_wzy/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:07:59.000000 tools_wzy-0.0.5/tools_wzy/__init__.py
+-rw-rw-rw-   0        0        0     9507 2023-07-17 06:15:57.000000 tools_wzy-0.0.5/tools_wzy/node_coverage.py
+-rw-rw-rw-   0        0        0     5153 2023-07-18 03:25:19.000000 tools_wzy-0.0.5/tools_wzy/yolo_need.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:15.533026 tools_wzy-0.0.5/tools_wzy.egg-info/
+-rw-rw-rw-   0        0        0      308 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/top_level.txt
```

### Comparing `tools_wzy-0.0.4/setup.py` & `tools_wzy-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2023-07-18
 #############################################
 
 from setuptools import setup, find_packages            #这个包没有的可以pip一下
 
 setup(
     name = "tools_wzy",      #这里是pip项目发布的名称
-    version = "0.0.4",  #版本号，数值大的会优先被pip
+    version = "0.0.5",  #版本号，数值大的会优先被pip
     keywords = ["pip", "tools_wzy"],
     description = "Some python tools for work from Zhiyuan",
     long_description = "Some python tools for work from Zhiyuan",
     license = "MIT Licence",
 
     url = "https://gitee.com/Zhiyuan_WZY",     #项目相关文件地址，一般是github
     author = "Zhiyuan Wang",
```

### Comparing `tools_wzy-0.0.4/tools_wzy/node_coverage.py` & `tools_wzy-0.0.5/tools_wzy/node_coverage.py`

 * *Files identical despite different names*

### Comparing `tools_wzy-0.0.4/tools_wzy/yolo_need.py` & `tools_wzy-0.0.5/tools_wzy/yolo_need.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,19 @@
 def split_train_val(xmls_folder, trainval_proportion=0.9, train_proportion=0.8):
     # trainval_proportion: 训练集和验证集占总体的比例，剩下的是测试集
     # train_proportion: 训练集占train_val比例，可自己进行调整
 
     # 创建label文件夹
     up_folder = os.path.dirname(xmls_folder)
     split_folder = up_folder + '/dataSet_path'
+    images_folder = up_folder + '/images'
     os.makedirs(split_folder, exist_ok=True)
 
-    # 读取所有xml文件的绝对路径
-    xmls_names = [os.path.join(xmls_folder, f.name) for f in os.scandir(xmls_folder) if f.is_file()]
+    # 读取所有xml文件名，拼接到
+    xmls_names = [os.path.join(images_folder, f.name[:-4]+'.jpg') for f in os.scandir(xmls_folder) if f.is_file()]
     # 随机划分
     num = len(xmls_names)
     list_index = range(num)
     tv = int(num * trainval_proportion)
     tr = int(tv * train_proportion)
     trainval = random.sample(list_index, tv)
     train = random.sample(trainval, tr)
@@ -134,14 +135,13 @@
         yaml.dump(params, f, sort_keys=False)
     print("data yaml文件生成成功：" + yaml_path)
     return yaml_path
 
 if __name__ == '__main__':
     xmls_folder = r'F:\Zhiyuan\pic_annotations_data\Annotations'
     class_list = ["person"]
-    images_path = r'F:\Zhiyuan\pic_annotations_data\images'
     labels_folder = xmls_to_yolo(xmls_folder, class_list)
     dataSet_folder = split_train_val(xmls_folder, 0.5, 0.5)
     yaml_path = gen_yaml(dataSet_folder, class_list, 'test.yaml')
```

