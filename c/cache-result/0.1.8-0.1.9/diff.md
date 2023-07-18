# Comparing `tmp/cache-result-0.1.8.tar.gz` & `tmp/cache-result-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache-result-0.1.8.tar", last modified: Fri Jul 14 12:48:49 2023, max compression
+gzip compressed data, was "cache-result-0.1.9.tar", last modified: Tue Jul 18 02:04:40 2023, max compression
```

## Comparing `cache-result-0.1.8.tar` & `cache-result-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:48:49.360849 cache-result-0.1.8/
--rw-rw-rw-   0        0        0     3032 2023-07-14 12:48:49.359849 cache-result-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2743 2023-07-14 06:08:46.000000 cache-result-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 12:48:49.343850 cache-result-0.1.8/cache_result/
--rw-rw-rw-   0        0        0     3972 2023-07-14 12:18:29.000000 cache-result-0.1.8/cache_result/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:48:49.356850 cache-result-0.1.8/cache_result.egg-info/
--rw-rw-rw-   0        0        0     3032 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-14 12:48:49.000000 cache-result-0.1.8/cache_result.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 12:48:49.360849 cache-result-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-07-14 12:48:02.000000 cache-result-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:04:40.472970 cache-result-0.1.9/
+-rw-rw-rw-   0        0        0     3032 2023-07-18 02:04:40.471967 cache-result-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2743 2023-07-14 06:08:46.000000 cache-result-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 02:04:40.458967 cache-result-0.1.9/cache_result/
+-rw-rw-rw-   0        0        0     4118 2023-07-18 01:58:45.000000 cache-result-0.1.9/cache_result/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:04:40.468971 cache-result-0.1.9/cache_result.egg-info/
+-rw-rw-rw-   0        0        0     3032 2023-07-18 02:04:40.000000 cache-result-0.1.9/cache_result.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-18 02:04:40.000000 cache-result-0.1.9/cache_result.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:04:40.000000 cache-result-0.1.9/cache_result.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 02:04:40.000000 cache-result-0.1.9/cache_result.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-18 02:04:40.000000 cache-result-0.1.9/cache_result.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 02:04:40.469971 cache-result-0.1.9/run_info/
+-rw-rw-rw-   0        0        0     1213 2023-07-16 07:31:15.000000 cache-result-0.1.9/run_info/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:04:40.472970 cache-result-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-07-18 01:57:05.000000 cache-result-0.1.9/setup.py
```

### Comparing `cache-result-0.1.8/PKG-INFO` & `cache-result-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

### Comparing `cache-result-0.1.8/README.md` & `cache-result-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cache-result-0.1.8/cache_result/__init__.py` & `cache-result-0.1.9/cache_result/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import time
 
 from colorama import Fore, Back, Style
 
 def remove_unused_code(source_code):
     # 删除单行注释
     source_code = re.sub(r'#.*$', "", source_code, flags=re.MULTILINE)
+    # 删除多行注释
+    source_code = re.sub(r'""".*?"""', "", source_code, flags=re.MULTILINE | re.DOTALL)
     # 删除print语句
     source_code = re.sub(r'print\(.*\)', "", source_code)
     # 删除注解
-    source_code = re.sub(r'@cache\(.*\)', '', source_code)
+    source_code = re.sub(r'@.*\(.*\)', '', source_code)
     return source_code
 
 def cache(cache_dir, exclude=None, is_print=True):
     """
     缓存函数的装饰器
     :param cache_dir: 缓存目录
     :param exclude: 排除的参数 ['func_name', 'source_code', 'args'] 函数名、源代码、函数参数
@@ -66,29 +68,29 @@
             # 创建缓存目录
             os.makedirs(modified_cache_dir, exist_ok=True)
 
             # 如果缓存文件存在，直接读取并返回结果
             if os.path.exists(file_path):
                 start = time.time()
                 if is_print:
-                    print(Fore.GREEN +f'{func.__name__} Loading from cache', Style.RESET_ALL, end=' ')
+                    print(Fore.GREEN +f'{func.__name__} Loading from cache {file_name}', Style.RESET_ALL, end=' ')
                 with open(file_path, 'rb') as f:
                     try:
                         result = pickle.load(f)
                     except: # 如果pickle文件损坏，重新运行函数
                         result = func(*args, **kwargs)
                         with open(file_path, 'wb') as f:
                             pickle.dump(result, f)
                         if is_print:
-                            print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir), Style.RESET_ALL)
+                            print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir, file_name), Style.RESET_ALL)
                 if is_print:
                     print(Fore.RED +f'{(time.time() - start):.1f}s ok', Style.RESET_ALL)
             else:
                 # 否则，运行函数并保存结果
                 result = func(*args, **kwargs)
                 with open(file_path, 'wb') as f:
                     pickle.dump(result, f)
                 if is_print:
-                    print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir), Style.RESET_ALL)
+                    print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir, file_name), Style.RESET_ALL)
             return result
         return wrapper
     return decorator
```

### Comparing `cache-result-0.1.8/cache_result.egg-info/PKG-INFO` & `cache-result-0.1.9/cache_result.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

### Comparing `cache-result-0.1.8/setup.py` & `cache-result-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # 读取README.md文件的内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cache-result',
-    version='0.1.8',
+    version='0.1.9',
     description='A python decorator for caching the results of functions',
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Source Code': 'https://github.com/glwhappen/cache-result',
     },
     author='glwhappen',
```

