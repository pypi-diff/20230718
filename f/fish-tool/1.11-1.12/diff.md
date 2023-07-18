# Comparing `tmp/fish_tool-1.11.tar.gz` & `tmp/fish_tool-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_tool-1.11.tar", last modified: Mon Mar 27 07:07:02 2023, max compression
+gzip compressed data, was "dist/fish_tool-1.12.tar", last modified: Tue Jul 18 00:19:15 2023, max compression
```

## Comparing `fish_tool-1.11.tar` & `fish_tool-1.12.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 07:07:02.260849 fish_tool-1.11/
--rw-rw-rw-   0        0        0      297 2023-03-27 07:07:02.259874 fish_tool-1.11/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-02-10 15:15:12.000000 fish_tool-1.11/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 07:07:02.217980 fish_tool-1.11/fish_tool/
--rw-rw-rw-   0        0        0      459 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:07:02.239889 fish_tool-1.11/fish_tool/ai/
--rw-rw-rw-   0        0        0        0 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/__init__.py
--rw-rw-rw-   0        0        0     7140 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/attentions.py
--rw-rw-rw-   0        0        0   988443 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/echarts_tool.py
--rw-rw-rw-   0        0        0     2272 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/group_list.py
--rw-rw-rw-   0        0        0     1553 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/laboratory.py
--rw-rw-rw-   0        0        0     3148 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/scorers.py
--rw-rw-rw-   0        0        0    17016 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/ai/torch_tool.py
--rw-rw-rw-   0        0        0     1285 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/config_base.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:07:02.253033 fish_tool-1.11/fish_tool/db/
--rw-rw-rw-   0        0        0        0 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/db/__init__.py
--rw-rw-rw-   0        0        0    50278 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/db/es_tool.py
--rw-rw-rw-   0        0        0     1196 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/db/mysql_tool.py
--rw-rw-rw-   0        0        0     3249 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/db/neo_tool.py
--rw-rw-rw-   0        0        0     5959 2023-03-27 06:55:53.000000 fish_tool-1.11/fish_tool/db/sqlite_tool.py
--rw-rw-rw-   0        0        0     1562 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/db/xmind_tool.py
--rw-rw-rw-   0        0        0     1545 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/db/zip_tool.py
--rw-rw-rw-   0        0        0     4717 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/log_tool.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:07:02.258836 fish_tool-1.11/fish_tool/net/
--rw-rw-rw-   0        0        0        0 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/net/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/net/api_tool.py
--rw-rw-rw-   0        0        0     2567 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/net/proxy_16yun.py
--rw-rw-rw-   0        0        0     4941 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/net/spider_tool.py
--rw-rw-rw-   0        0        0     2854 2023-02-10 07:51:37.000000 fish_tool-1.11/fish_tool/register.py
--rw-rw-rw-   0        0        0    21100 2023-02-10 12:07:35.000000 fish_tool-1.11/fish_tool/sys_tool.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:07:02.224933 fish_tool-1.11/fish_tool.egg-info/
--rw-rw-rw-   0        0        0      297 2023-03-27 07:07:02.000000 fish_tool-1.11/fish_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2023-03-27 07:07:02.000000 fish_tool-1.11/fish_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 07:07:02.000000 fish_tool-1.11/fish_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-03-27 07:07:02.000000 fish_tool-1.11/fish_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-27 07:07:02.000000 fish_tool-1.11/fish_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 07:07:02.260849 fish_tool-1.11/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-03-27 06:57:36.000000 fish_tool-1.11/setup.py
+drwxrwxr-x   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:19:15.493547 fish_tool-1.12/
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)      284 2023-07-18 00:19:15.493547 fish_tool-1.12/PKG-INFO
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)       39 2023-07-18 00:03:04.000000 fish_tool-1.12/README.md
+drwxrwxr-x   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:19:15.489547 fish_tool-1.12/fish_tool/
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)      459 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/__init__.py
+drwxrwxr-x   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:19:15.489547 fish_tool-1.12/fish_tool/ai/
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/ai/__init__.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     7140 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/ai/attentions.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)   988443 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/ai/echarts_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     2272 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/ai/group_list.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     1553 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/ai/laboratory.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     3148 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/ai/scorers.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)    17608 2023-07-18 00:10:23.000000 fish_tool-1.12/fish_tool/ai/torch_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     1285 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/config_base.py
+drwxrwxr-x   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:19:15.489547 fish_tool-1.12/fish_tool/db/
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/__init__.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)    50278 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/es_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     1196 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/mysql_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     3249 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/neo_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     5959 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/sqlite_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     1562 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/xmind_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     1545 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/db/zip_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     4717 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/log_tool.py
+drwxrwxr-x   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:19:15.493547 fish_tool-1.12/fish_tool/net/
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/net/__init__.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     2513 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/net/api_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     2567 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/net/proxy_16yun.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     4941 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/net/spider_tool.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)     2854 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/register.py
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)    21100 2023-07-18 00:03:04.000000 fish_tool-1.12/fish_tool/sys_tool.py
+drwxrwxr-x   0 fish1     (1000) fish1     (1000)        0 2023-07-18 00:19:15.489547 fish_tool-1.12/fish_tool.egg-info/
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)      284 2023-07-18 00:19:15.000000 fish_tool-1.12/fish_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)      772 2023-07-18 00:19:15.000000 fish_tool-1.12/fish_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)        1 2023-07-18 00:19:15.000000 fish_tool-1.12/fish_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)      126 2023-07-18 00:19:15.000000 fish_tool-1.12/fish_tool.egg-info/requires.txt
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)       10 2023-07-18 00:19:15.000000 fish_tool-1.12/fish_tool.egg-info/top_level.txt
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)       38 2023-07-18 00:19:15.493547 fish_tool-1.12/setup.cfg
+-rw-rw-r--   0 fish1     (1000) fish1     (1000)      925 2023-07-18 00:16:39.000000 fish_tool-1.12/setup.py
```

### Comparing `fish_tool-1.11/fish_tool/ai/attentions.py` & `fish_tool-1.12/fish_tool/ai/attentions.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/ai/echarts_tool.py` & `fish_tool-1.12/fish_tool/ai/echarts_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/ai/group_list.py` & `fish_tool-1.12/fish_tool/ai/group_list.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/ai/laboratory.py` & `fish_tool-1.12/fish_tool/ai/laboratory.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/ai/scorers.py` & `fish_tool-1.12/fish_tool/ai/scorers.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/ai/torch_tool.py` & `fish_tool-1.12/fish_tool/ai/torch_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             self._value = value
         else:
             new_value = self.beta * self._value + (1 - self.beta) * value
             if math.isnan(new_value):
                 logs.tmp.error(f'value={value}  old={self._value}  new={new_value}')
             else:
                 self._value = new_value
+        return self._value
 
 
 class SentencePieceVocab:
     def __init__(self, sp_path):
         if not os.path.isfile(sp_path):
             logs.brief.warning(f'sp_path文件不存在： {sp_path}')
         self.sp = sentencepiece.SentencePieceProcessor()
@@ -233,31 +234,47 @@
     big += add
     weight = [big / t for t in counts_pad]
     weight = torch.tensor(weight, dtype=torch.float, device=device)
     return weight
 
 
 def save_model(model, path):
+    if hasattr(model, 'module'):
+        model = getattr(model, 'module')  # torch.nn.parallel.DistributedDataParallel
     path = os.path.abspath(path)
     save_dir = os.path.dirname(path)
     if not os.path.isdir(save_dir):
         os.makedirs(save_dir)
     torch.save(model.state_dict(), path)
     return model
 
 
 def load_cpu_model(model, path):
+    # 之后废弃掉
     if isinstance(path, bytes):
         # 如果是二进制 则已经读取了 要包装一下
         path = io.BytesIO(path)
     model_state = torch.load(path, map_location=torch.device('cpu'))
     model.load_state_dict(model_state)
     return model
 
 
+def load_model(model, path, device=None):
+    if isinstance(path, bytes):
+        # 如果是二进制 则已经读取了 要包装一下
+        path = io.BytesIO(path)
+    if device is None:
+        device = torch.device('cpu')
+    elif isinstance(device, int):
+        device = torch.device("cuda", device)
+    model_state = torch.load(path, map_location=device)
+    model.load_state_dict(model_state)
+    return model
+
+
 def model_save_zip(model, path, name='model.pth'):
     # 把模型存储到zip文件中 注意存储过程很慢
     save_dir = os.path.dirname(os.path.abspath(path))
     if not os.path.isdir(save_dir):
         os.makedirs(save_dir)
     zip = zip_tool.ZipTool(path)
     if zip.is_exist(name):
```

### Comparing `fish_tool-1.11/fish_tool/config_base.py` & `fish_tool-1.12/fish_tool/config_base.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/db/es_tool.py` & `fish_tool-1.12/fish_tool/db/es_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/db/mysql_tool.py` & `fish_tool-1.12/fish_tool/db/mysql_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/db/neo_tool.py` & `fish_tool-1.12/fish_tool/db/neo_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/db/sqlite_tool.py` & `fish_tool-1.12/fish_tool/db/sqlite_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/db/xmind_tool.py` & `fish_tool-1.12/fish_tool/db/xmind_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/db/zip_tool.py` & `fish_tool-1.12/fish_tool/db/zip_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/log_tool.py` & `fish_tool-1.12/fish_tool/log_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/net/api_tool.py` & `fish_tool-1.12/fish_tool/net/api_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/net/proxy_16yun.py` & `fish_tool-1.12/fish_tool/net/proxy_16yun.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/net/spider_tool.py` & `fish_tool-1.12/fish_tool/net/spider_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/register.py` & `fish_tool-1.12/fish_tool/register.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool/sys_tool.py` & `fish_tool-1.12/fish_tool/sys_tool.py`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/fish_tool.egg-info/SOURCES.txt` & `fish_tool-1.12/fish_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fish_tool-1.11/setup.py` & `fish_tool-1.12/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fish_tool",
-    version="1.11",
+    version="1.12",
     author="aifish",
     url="https://gitee.com/laowangzi/fish_tool",
     author_email="ofyu@163.com",
     description="some tool code",
     packages=find_packages(),
     install_requires=[
         'pyyaml>=6.0',
@@ -36,8 +36,9 @@
 twine upload dist/*
 """
 """
 更新内容
 1.1 2023.03.22 db/sqlite_tool.py 增加字段功能
 
 1.11 2023年3月27日 db/sqlite_tool.py 增加scroll功能
+1.12 2023年7月18日 ai/torch_tool.py 增加load_model(model, path, device=None)
 """
```

