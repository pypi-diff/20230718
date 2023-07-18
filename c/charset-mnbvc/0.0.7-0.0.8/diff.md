# Comparing `tmp/charset_mnbvc-0.0.7.tar.gz` & `tmp/charset_mnbvc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charset_mnbvc-0.0.7.tar", last modified: Thu Jun  8 01:59:34 2023, max compression
+gzip compressed data, was "charset_mnbvc-0.0.8.tar", last modified: Tue Jul 18 06:25:52 2023, max compression
```

## Comparing `charset_mnbvc-0.0.7.tar` & `charset_mnbvc-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-06-08 01:59:34.334869 charset_mnbvc-0.0.7/
--rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.7/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)    12261 2023-06-08 01:59:34.334678 charset_mnbvc-0.0.7/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)    11621 2023-06-08 01:44:43.000000 charset_mnbvc-0.0.7/README.md
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-06-08 01:59:34.333996 charset_mnbvc-0.0.7/charset_mnbvc/
--rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.7/charset_mnbvc/__init__.py
--rw-r--r--   0 alan       (501) staff       (20)     4674 2023-06-05 07:27:58.000000 charset_mnbvc-0.0.7/charset_mnbvc/api.py
--rw-r--r--   0 alan       (501) staff       (20)      453 2023-05-26 03:45:39.000000 charset_mnbvc-0.0.7/charset_mnbvc/common_utils.py
--rw-r--r--   0 alan       (501) staff       (20)     2902 2023-03-27 14:46:45.000000 charset_mnbvc-0.0.7/charset_mnbvc/constant.py
--rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.7/charset_mnbvc/verify.py
--rw-r--r--   0 alan       (501) staff       (20)       70 2023-06-08 01:59:32.000000 charset_mnbvc-0.0.7/charset_mnbvc/version.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-06-08 01:59:34.334493 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)    12261 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      326 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       14 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/top_level.txt
--rw-r--r--   0 alan       (501) staff       (20)       38 2023-06-08 01:59:34.334986 charset_mnbvc-0.0.7/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.7/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-18 06:25:52.625591 charset_mnbvc-0.0.8/
+-rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.8/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)    12352 2023-07-18 06:25:52.625405 charset_mnbvc-0.0.8/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)    11712 2023-07-07 03:47:36.000000 charset_mnbvc-0.0.8/README.md
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-18 06:25:52.624462 charset_mnbvc-0.0.8/charset_mnbvc/
+-rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.8/charset_mnbvc/__init__.py
+-rw-r--r--   0 alan       (501) staff       (20)     6375 2023-07-18 06:24:28.000000 charset_mnbvc-0.0.8/charset_mnbvc/api.py
+-rw-r--r--   0 alan       (501) staff       (20)      453 2023-07-07 02:45:15.000000 charset_mnbvc-0.0.8/charset_mnbvc/common_utils.py
+-rw-r--r--   0 alan       (501) staff       (20)     3211 2023-07-07 03:34:44.000000 charset_mnbvc-0.0.8/charset_mnbvc/constant.py
+-rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.8/charset_mnbvc/verify.py
+-rw-r--r--   0 alan       (501) staff       (20)       70 2023-06-20 03:19:29.000000 charset_mnbvc-0.0.8/charset_mnbvc/version.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-18 06:25:52.625230 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)    12352 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      326 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       14 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/top_level.txt
+-rw-r--r--   0 alan       (501) staff       (20)       38 2023-07-18 06:25:52.625631 charset_mnbvc-0.0.8/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.8/setup.py
```

### Comparing `charset_mnbvc-0.0.7/LICENSE` & `charset_mnbvc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.7/PKG-INFO` & `charset_mnbvc-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charset_mnbvc
-Version: 0.0.7
+Version: 0.0.8
 Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 Home-page: https://github.com/alanshi/charset_mnbvc
 Author: Alan Shi
 Author-email: alan.shi86@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
 Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
@@ -70,14 +70,22 @@
     source_data=source_data,
     source_encoding="gbk",
     target_encoding="utf-8",
 )
 print(ret)
 ```
 
+###### 尝试修复乱码数据
+```
+from charset_mnbvc import api
+data_1 = "变巨"
+
+result_1 = api.fix_data(s=data_1)
+print(f"修复测试1: {result_1}")
+```
 
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
 2: 将文本使用utf-8格式覆盖到test.txt
@@ -184,15 +192,15 @@
 No, Windows code pages must be either one byte (SBCS) or a mix of one and two bytes (DBCS). This requirement is reflected throughout our code e.g. in data structures, program interfaces, network protocols and applications. The existing code page for Simplified Chinese, CP936, is a double byte code page. GB18030 is a four–byte code page i.e. every character is represented by one, two or four bytes. To replace CP936 with GB18030 would require rewriting much of the system. Even if we were to do this, such a system would not run regular applications nor interoperate with regular Windows.
 ```
 
 
 解决这个问题最简单的方式就是使用MS936来处理这种有问题的文件(Windows Code page 936 (abbreviated MS936, Windows-936 or (ambiguously) CP936))。不过遗憾的是Python语言暂时没有独立支持MS936或者CP936，而是把它们统一作为GBK处理了。https://docs.python.org/3/library/codecs.html。
 因此目前单纯使用Python对文件内容进行decode无法正确处理这些特殊符号。
 
-最后我用Java写了一段代码验证，可以顺利的用MS936解析出文件中的欧元符号。
+最后我用Java写了一段代码验证，可以顺利的用MS936解析出文件中的欧元符号，目前计划把Java对于MS936的支持翻译成Python代码作为本项目的一部分。
 ![iZAjIJ.png](https://i.328888.xyz/2023/03/23/iZAjIJ.png)
 
 
 ```
 import java.io.BufferedReader;
 import java.io.File;
 import java.io.FileInputStream;
@@ -224,15 +232,7 @@
         }
         return sb.toString();
     }
 }
 ```
 
 
-现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
-
-
-
-
-
-
-
```

### Comparing `charset_mnbvc-0.0.7/README.md` & `charset_mnbvc-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,22 @@
     source_data=source_data,
     source_encoding="gbk",
     target_encoding="utf-8",
 )
 print(ret)
 ```
 
+###### 尝试修复乱码数据
+```
+from charset_mnbvc import api
+data_1 = "变巨"
+
+result_1 = api.fix_data(s=data_1)
+print(f"修复测试1: {result_1}")
+```
 
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
 2: 将文本使用utf-8格式覆盖到test.txt
@@ -167,15 +175,15 @@
 No, Windows code pages must be either one byte (SBCS) or a mix of one and two bytes (DBCS). This requirement is reflected throughout our code e.g. in data structures, program interfaces, network protocols and applications. The existing code page for Simplified Chinese, CP936, is a double byte code page. GB18030 is a four–byte code page i.e. every character is represented by one, two or four bytes. To replace CP936 with GB18030 would require rewriting much of the system. Even if we were to do this, such a system would not run regular applications nor interoperate with regular Windows.
 ```
 
 
 解决这个问题最简单的方式就是使用MS936来处理这种有问题的文件(Windows Code page 936 (abbreviated MS936, Windows-936 or (ambiguously) CP936))。不过遗憾的是Python语言暂时没有独立支持MS936或者CP936，而是把它们统一作为GBK处理了。https://docs.python.org/3/library/codecs.html。
 因此目前单纯使用Python对文件内容进行decode无法正确处理这些特殊符号。
 
-最后我用Java写了一段代码验证，可以顺利的用MS936解析出文件中的欧元符号。
+最后我用Java写了一段代码验证，可以顺利的用MS936解析出文件中的欧元符号，目前计划把Java对于MS936的支持翻译成Python代码作为本项目的一部分。
 ![iZAjIJ.png](https://i.328888.xyz/2023/03/23/iZAjIJ.png)
 
 
 ```
 import java.io.BufferedReader;
 import java.io.File;
 import java.io.FileInputStream;
@@ -205,15 +213,7 @@
                 sb.append(line).append(System.lineSeparator());
             }
         }
         return sb.toString();
     }
 }
 ```
-
-
-现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
-
-
-
-
-
```

### Comparing `charset_mnbvc-0.0.7/charset_mnbvc/api.py` & `charset_mnbvc-0.0.8/charset_mnbvc/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,78 @@
 import os
 import sys
+import re
 from re import compile
 
 import cchardet
 import tqdm
 
 from .constant import (
     REGEX_FEATURE_ALL,
     REGEX_FEATURE,
     CHUNK_SIZE,
     ENCODINGS,
+    EXT_ENCODING,
     CCHARDECT_ENCODING_MAP
 )
 
 
 # compile makes it more efficient
 re_char_check = compile(REGEX_FEATURE_ALL)
 
 
+def has_control_characters(text):
+    """
+    :param text: text
+    :return: bool
+    """
+    pattern = r'[\u0000-\u001f\u007f-\u009f]'
+    match = re.search(pattern, text)
+    return match is not None
+
+
+def fix_data(s: str) -> list:
+    """
+    :param s: text
+    :return: list
+    """
+
+    result = []
+
+    for item in EXT_ENCODING:
+        guess_text = s.encode(encoding=item, errors='replace')
+        for target in EXT_ENCODING:
+            if item == target:
+                continue
+            fixed_text = guess_text.decode(encoding=target, errors='replace')
+            dic = {"origin": s, "guess": fixed_text, "from": item, "to": target}
+            result.append(dic)
+
+    return result
+
+
 def from_data(data, mode) -> str:
     """
     :param data: data
     :param mode: 1: use mnbvc, 2: use cchardet
     :return: encoding
     """
-    coding_name = get_cn_charset(source_data=data, mode=mode, source_type="data")
+    coding_name = get_cn_charset(
+        source_data=data, mode=mode, source_type="data")
     return coding_name
 
 
 def from_file(file_path, mode):
     """
     :param file_path: file path
     :param mode: 1: use mnbvc, 2: use cchardet
     :return: encoding
     """
-    coding_name = get_cn_charset(source_data=file_path, mode=mode, source_type="file")
+    coding_name = get_cn_charset(
+        source_data=file_path, mode=mode, source_type="file")
     return file_path, coding_name
 
 
 def from_dir(folder_path, mode):
     """
     :param folder_path: folder path
     :param mode: 1: use mnbvc, 2: use cchardet
@@ -46,15 +80,16 @@
     """
     results = []
     sub_folders, files = scan_dir(folder_path)
     file_count = len(files)
     for idx in tqdm.tqdm(range(file_count), "编码检测进度"):
         file_path = files[idx]
 
-        coding_name = get_cn_charset(source_data=file_path, mode=mode, source_type="file")
+        coding_name = get_cn_charset(
+            source_data=file_path, mode=mode, source_type="file")
         if not coding_name:
             coding_name = "None"
 
         results.append(
             (file_path, coding_name)
         )
 
@@ -149,20 +184,38 @@
     """
     encoding = None
     try:
         data = ""
         if source_type == "file":
             with open(source_data, 'rb') as fp:
                 data = fp.read()
+
                 if not data:
-                    return "Empty File"
+                    return None
         else:
             data = source_data
 
-        encoding = check_by_mnbvc(data=data) if mode == 1 else check_by_cchardect(data=data)
+        try:
+
+            # 内容中是否包含 null 字符（二进制文件通常包含 null 字符）
+            # if b'\x00' in data:
+            #     return None
+
+            if 'ufffd' in data.decode().encode("unicode_escape").decode():
+                return "UNKNOWN"
+
+            # 内容是否包含 unicode控制符
+            # if has_control_characters(data.decode("unicode_escape")):
+            #     return "UNKNOWN"
+
+        except Exception as err:
+            pass
+
+        encoding = check_by_mnbvc(
+            data=data) if mode == 1 else check_by_cchardect(data=data)
 
     except Exception as err:
         sys.stderr.write(f"Error: {str(err)}\n")
 
     return encoding
 
 
@@ -171,16 +224,28 @@
     :param source_data: data
     :param source_encoding: input encoding
     :param target_encoding: output encoding
     :return: data
     """
     try:
         data = source_data.decode(encoding=source_encoding)
-        data = data.encode(encoding=target_encoding).decode(encoding=target_encoding)
+        data = data.encode(encoding=target_encoding).decode(
+            encoding=target_encoding)
     except Exception as err:
-        sys.stderr.write(f"Error: {str(err)}\n")
-        data = source_data
+        if source_encoding == "big5":
+            try:
+                source_encoding = "cp950"
+                data = source_data.decode(encoding=source_encoding)
+                data = data.encode(encoding=target_encoding).decode(
+                    encoding=target_encoding)
+            except Exception as err:
+                sys.stderr.write(f"Error: {str(err)}\n")
+                data = source_data
+        else:
+            sys.stderr.write(f"Error: {str(err)}\n")
+            data = source_data
 
     return data
 
+
 def test():
     print("test")
```

### Comparing `charset_mnbvc-0.0.7/charset_mnbvc/constant.py` & `charset_mnbvc-0.0.8/charset_mnbvc/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,27 @@
                     r'\u5206\u8fd8\u8fdb\u597d\u5c0f\u90e8\u5176\u4e9b\u4e3b\u6837\u7406\u5fc3\u5979' \
                     r'\u672c\u524d\u5f00\u4f46\u56e0\u53ea\u4ece\u60f3\u5b9e]'
 
 ENCODINGS = [
     'utf_8',
     'utf_16',
     'gb18030',
-    'big5'
+    'big5',
+]
+
+EXT_ENCODING = [
+    'utf-8',
+    'gbk', # 简体中文 (GB2312)
+    'gb18030', # 简体中文 (GB2312)
+    'BIG5', # 繁体中文 (BIG5)
+    'shift_jis', # 日本語 (cp932)
+    'euc_kr', # 한국어 (cp949)
+    'ascii', # ASCII
+    'utf_16', # Unicode (UTF-16)
+    'cp1252', # Western European (Windows)
 ]
 
 CCHARDECT_ENCODING_MAP = {
     "UTF-8": "utf_8",
     "UTF-16": "utf_16",
     "UTF-8-SIG": "utf_8_sig",
     "UTF-16BE": "utf_16_be",
@@ -66,8 +78,7 @@
     "ISO-8859-10": "iso_8859_10",
     "KOI8-R": "koi8_r",
     "MAC-CYRILLIC": "mac_cyrillic",
     "IBM866": "ibm866",
     "IBM855": "ibm855",
     "M": "m"
 }
-
```

### Comparing `charset_mnbvc-0.0.7/charset_mnbvc/verify.py` & `charset_mnbvc-0.0.8/charset_mnbvc/verify.py`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.7/charset_mnbvc.egg-info/PKG-INFO` & `charset_mnbvc-0.0.8/charset_mnbvc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charset-mnbvc
-Version: 0.0.7
+Version: 0.0.8
 Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 Home-page: https://github.com/alanshi/charset_mnbvc
 Author: Alan Shi
 Author-email: alan.shi86@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
 Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
@@ -70,14 +70,22 @@
     source_data=source_data,
     source_encoding="gbk",
     target_encoding="utf-8",
 )
 print(ret)
 ```
 
+###### 尝试修复乱码数据
+```
+from charset_mnbvc import api
+data_1 = "变巨"
+
+result_1 = api.fix_data(s=data_1)
+print(f"修复测试1: {result_1}")
+```
 
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
 2: 将文本使用utf-8格式覆盖到test.txt
@@ -184,15 +192,15 @@
 No, Windows code pages must be either one byte (SBCS) or a mix of one and two bytes (DBCS). This requirement is reflected throughout our code e.g. in data structures, program interfaces, network protocols and applications. The existing code page for Simplified Chinese, CP936, is a double byte code page. GB18030 is a four–byte code page i.e. every character is represented by one, two or four bytes. To replace CP936 with GB18030 would require rewriting much of the system. Even if we were to do this, such a system would not run regular applications nor interoperate with regular Windows.
 ```
 
 
 解决这个问题最简单的方式就是使用MS936来处理这种有问题的文件(Windows Code page 936 (abbreviated MS936, Windows-936 or (ambiguously) CP936))。不过遗憾的是Python语言暂时没有独立支持MS936或者CP936，而是把它们统一作为GBK处理了。https://docs.python.org/3/library/codecs.html。
 因此目前单纯使用Python对文件内容进行decode无法正确处理这些特殊符号。
 
-最后我用Java写了一段代码验证，可以顺利的用MS936解析出文件中的欧元符号。
+最后我用Java写了一段代码验证，可以顺利的用MS936解析出文件中的欧元符号，目前计划把Java对于MS936的支持翻译成Python代码作为本项目的一部分。
 ![iZAjIJ.png](https://i.328888.xyz/2023/03/23/iZAjIJ.png)
 
 
 ```
 import java.io.BufferedReader;
 import java.io.File;
 import java.io.FileInputStream;
@@ -224,15 +232,7 @@
         }
         return sb.toString();
     }
 }
 ```
 
 
-现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
-
-
-
-
-
-
-
```

### Comparing `charset_mnbvc-0.0.7/setup.py` & `charset_mnbvc-0.0.8/setup.py`

 * *Files identical despite different names*

