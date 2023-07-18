# Comparing `tmp/gmsofttest-0.0.8.tar.gz` & `tmp/gmsofttest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gmsofttest-0.0.8.tar", last modified: Sat Jun  3 03:57:19 2023, max compression
+gzip compressed data, was "dist\gmsofttest-0.0.9.tar", last modified: Tue Jul 18 07:44:26 2023, max compression
```

## Comparing `gmsofttest-0.0.8.tar` & `gmsofttest-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1407 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-06-03 03:57:15.000000 gmsofttest-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-06-03 03:55:43.000000 gmsofttest-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.8/src/gmsofttest/__init__.py
--rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.8/src/gmsofttest/china_address.py
--rw-rw-rw-   0        0        0     3327 2023-05-24 03:07:23.000000 gmsofttest-0.0.8/src/gmsofttest/gm_assert_utils.py
--rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.8/src/gmsofttest/gm_excel_utils.py
--rw-rw-rw-   0        0        0     3382 2023-06-03 03:54:28.000000 gmsofttest-0.0.8/src/gmsofttest/gm_parse_response_utils.py
--rw-rw-rw-   0        0        0     2170 2023-06-02 00:58:44.000000 gmsofttest-0.0.8/src/gmsofttest/gm_randomdata_utils.py
--rw-rw-rw-   0        0        0     1806 2023-05-24 02:44:27.000000 gmsofttest-0.0.8/src/gmsofttest/gm_request_utils.py
--rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.8/src/gmsofttest/gm_sqlconn_utils.py
--rw-rw-rw-   0        0        0      877 2023-05-23 08:40:42.000000 gmsofttest-0.0.8/src/gmsofttest/gm_stock_enum.py
--rw-rw-rw-   0        0        0     4322 2023-06-02 06:56:24.000000 gmsofttest-0.0.8/src/gmsofttest/gm_sucreditcode_utils.py
--rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.8/src/gmsofttest/gm_timestamp_utils.py
--rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.8/src/gmsofttest/gm_yaml_process_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/
--rw-rw-rw-   0        0        0     1407 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1431 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      937 2023-07-18 07:42:33.000000 gmsofttest-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-07-18 07:44:22.000000 gmsofttest-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/gmsofttest/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.9/src/gmsofttest/__init__.py
+-rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.9/src/gmsofttest/china_address.py
+-rw-rw-rw-   0        0        0     3333 2023-07-18 07:37:35.000000 gmsofttest-0.0.9/src/gmsofttest/gm_assert_utils.py
+-rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.9/src/gmsofttest/gm_excel_utils.py
+-rw-rw-rw-   0        0        0     2451 2023-07-18 07:35:34.000000 gmsofttest-0.0.9/src/gmsofttest/gm_parse_response_utils.py
+-rw-rw-rw-   0        0        0     2200 2023-07-18 07:41:07.000000 gmsofttest-0.0.9/src/gmsofttest/gm_randomdata_utils.py
+-rw-rw-rw-   0        0        0     1807 2023-06-04 07:13:18.000000 gmsofttest-0.0.9/src/gmsofttest/gm_request_utils.py
+-rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.9/src/gmsofttest/gm_sqlconn_utils.py
+-rw-rw-rw-   0        0        0      953 2023-06-19 05:54:21.000000 gmsofttest-0.0.9/src/gmsofttest/gm_stock_enum.py
+-rw-rw-rw-   0        0        0     4322 2023-06-02 06:56:24.000000 gmsofttest-0.0.9/src/gmsofttest/gm_sucreditcode_utils.py
+-rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.9/src/gmsofttest/gm_timestamp_utils.py
+-rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.9/src/gmsofttest/gm_yaml_process_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/gmsofttest.egg-info/
+-rw-rw-rw-   0        0        0     1431 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/gmsofttest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/gmsofttest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/gmsofttest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 07:44:26.000000 gmsofttest-0.0.9/src/gmsofttest.egg-info/top_level.txt
```

### Comparing `gmsofttest-0.0.8/LICENSE` & `gmsofttest-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/PKG-INFO` & `gmsofttest-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.8
+Version: 0.0.9
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 License-File: LICENSE
 
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
+v0.0.9
+  demo演示
+
 v0.0.8
  修改gm_prase_response的调用名称为gm_extract_json
  增加gm_sucreditcode_utils，用于生成企业社会信用代码
 
 v0.0.6 
  修改gm_request_utils的请求参数verfiy的默认值,由NONE调整成False
```

### Comparing `gmsofttest-0.0.8/README.md` & `gmsofttest-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
+v0.0.9
+  demo演示
+
 v0.0.8
  修改gm_prase_response的调用名称为gm_extract_json
  增加gm_sucreditcode_utils，用于生成企业社会信用代码
 
 v0.0.6 
  修改gm_request_utils的请求参数verfiy的默认值,由NONE调整成False
```

### Comparing `gmsofttest-0.0.8/setup.py` & `gmsofttest-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gmsofttest",
-    version="0.0.8",
+    version="0.0.9",
     author="ronaldsu",
     author_email="uph4rmt@dingtalk.com",
     description="大家软件内部测试技术线支撑工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.gec123.com",
     project_urls={
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest/china_address.py` & `gmsofttest-0.0.9/src/gmsofttest/china_address.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_assert_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_assert_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,18 +69,20 @@
     try:
         return to_type(value)
     except (ValueError, TypeError):
         return default
 
 
 if __name__ == '__main__':
-    gm_assert_equal(2, '2', int)  # 将第1和第2个参数转换成int型比较
-    gm_assert_multiple_values_equal([3, 3, '3'], int)
-    first_value = 'ok'
-    # second_value = '{"code":20000,"message":"ok","description":"","data":{"todoRationalNum":18,"todoAuditNum":1,"todoEleGuaranteeNum":1,"todoAbolishEleGuaranteeNum":0}}'
-    types = 'str'
-    second_value = 'okok'
-    # gm_assert_in(first_value,second_value, types)
-    # print(second_value)
-    # print(type(second_value))
-    gm_assert_equal('str', 'str1', str)
-    # print(s)
+    print(gm_assert_equal(2, '2', int))
+    print(gm_assert_equal(2, '2', str))
+
+    # gm_assert_multiple_values_equal([3, 3, '3'], int)
+    # first_value = 'ok'
+    # # second_value = '{"code":20000,"message":"ok","description":"","data":{"todoRationalNum":18,"todoAuditNum":1,"todoEleGuaranteeNum":1,"todoAbolishEleGuaranteeNum":0}}'
+    # types = 'str'
+    # second_value = 'okok'
+    # # gm_assert_in(first_value,second_value, types)
+    # # print(second_value)
+    # # print(type(second_value))
+    # gm_assert_equal('str', 'str1', str)
+
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_excel_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_excel_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_parse_response_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_parse_response_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,79 +12,43 @@
 def gm_extract_json(text, jsonpath_expression):
     """使用jsonpath工具类解析请求返回值"""
     try:
         # 判断是否
         if isinstance(text, dict):
             data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
         elif isinstance(text, str):
-            data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
+            text1 = json.loads(text)
+            data = jsonpath(text1, jsonpath_expression)  # 使用jsonpath进行解析
         elif isinstance(text, list):
             data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
         else:
             json_text = json.loads(text)  # 如果是非dict、str、list类型，则转换成python对象
             data = jsonpath(json_text, jsonpath_expression)  # 使用jsonpath进行解析
         return data
     except TypeError as e:
-        print("入参{}的类型错误，请检查,{}".format(text, e))
+        print("入参类型：{}，入参数据：{}，请检查错误:{}".format(type(text), text, e))
 
 
 if __name__ == '__main__':
-    json_data = """
-    { "store": {
-        "book": [
-          { "category": "reference",
-            "author": "Nigel Rees",
-            "title": "Sayings of the Century",
-            "price": 8.95
-          },
-          { "category": "fiction",
-            "author": "Evelyn Waugh",
-            "title": "Sword of Honour",
-            "price": 12.99
-          },
-          { "category": "fiction",
-            "author": "Herman Melville",
-            "title": "Moby Dick",
-            "isbn": "0-553-21311-3",
-            "price": 8.99
-          },
-          { "category": "fiction",
-            "author": "J. R. R. Tolkien",
-            "title": "The Lord of the Rings",
-            "isbn": "0-395-19395-8",
-            "price": 22.99
-          }
-        ],
-        "bicycle": {
-          "color": "red",
-          "price": 19.95
-        }
-      }
-    }
-    """
-
-    import jsonpath
-
-    json_data = json.loads(json_data)
-    store = jsonpath.jsonpath(json_data, '$.store')
-    isbn_book = jsonpath.jsonpath(json_data, '$..book[?(@.isbn)]')  # 正则查询book节点下含 isbn 关键字的，并列出对应book子节点数据；
-    price_book = jsonpath.jsonpath(json_data, '$..book[?(@.price<10)]')  # 正则查询book节点下 Price<10的，并列出对应book子节点数据；
-    category = jsonpath.jsonpath(json_data, '$...isbn')  # 直接查找isbn
-    price = jsonpath.jsonpath(json_data, '$.store..price')  # store节点下所有的price值
-    three_price = jsonpath.jsonpath(json_data, '$.store.book[0].price')  # store节点第1部书的price值，索引从0开始
-    last_book = jsonpath.jsonpath(json_data, '$.store.book[(@.length-1)]')  # 最后一本书
-
-    print(store)
-    print(isbn_book)
-    print(price_book)
-    print(category)
-    print(price)
-    print(three_price)
-    print(last_book)
-    print(type(last_book))
-    print(jsonpath.jsonpath(json_data, '$..book[-2:]'))  # 最后两本书)
-
-    s = """{"code":20000,"message":"ok","description":"",
-    "data":{"todoRationalNum":18,"todoAuditNum":1,"todoEleGuaranteeNum":1,"todoAbolishEleGuaranteeNum":0}}"""
-    s = json.loads(s)
-    s1 = jsonpath.jsonpath(s, '$.code')
-    print(s1[0])
+    s = """{ "store": 
+                { "book": 
+                    [
+                        { "category": "reference", "author": "Nigel Rees", "title": "Sayings of the Century", "price": 8.95 },
+                        { "category": "fiction", "author": "Evelyn Waugh", "title": "Sword of Honour", "price": 12.99 }, 
+                        { "category": "fiction", "author": "Herman Melville", "title": "Moby Dick", "isbn": "0-553-21311-3", "price": 8.99 }, 
+                        { "category": "fiction", "author": "J. R. R. Tolkien", "title": "The Lord of the Rings", "isbn": "0-395-19395-8", "price": 22.99 } 
+                    ], 
+                "bicycle": { "color": "red", "price": 19.95 } 
+                } 
+            }"""
+    print(gm_extract_json(s, '$.store.book'))
+    print(gm_extract_json(s, '$.store.book[0]'))
+    print(gm_extract_json(s, '$.store.book[0,3]'))
+    print(gm_extract_json(s, '$.store.book[*].author'))
+    print(gm_extract_json(s, '$.store.book[(@.length-1)].title'))
+    print(gm_extract_json(s, '$.store.book[3].title'))
+    print(gm_extract_json(s, '$.store.book[?(@.price<10)].price'))
+
+
+    print([i*2 for i in gm_extract_json(s, '$.store.book[*].author')])
+
+
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_randomdata_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_randomdata_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,7 +89,8 @@
 if __name__ == '__main__':
     print(getMobile())
     print(getCityName())
     print(getInt())
     print(getCompany())
     print(getProfile())
     print(getIDcard())
+    print(getLinuxTimestamp())
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_request_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_request_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,11 +31,11 @@
     return response
 
 def send_options_request(request, url, headers=None, params=None, data=None, json=None, verify=False):
     response = request.options(url=url, headers=headers, params=params, data=data, json=json,
                                verify=verify)
     return response
 
-def send_head_request(request, url, headers=None, params=None, data=None, json=None, verify=False):
+def send_head_request(request, url, headers=None, params=None, data=None, json=None, verify=False ):
     response = request.head(url=url, headers=headers, params=params, data=data, json=json,
                                verify=verify)
     return response
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_sqlconn_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_sqlconn_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_stock_enum.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_stock_enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,7 +25,11 @@
     SERVERCATEGORY = 313  # 服务类别
     ACCOUNT = 314  # 管理账号
     UNIT = 321  # 计量单位
     GOODS = '货物类'
     ENGINEERING = '工程类'
     SERVICES = '服务类'
 
+
+class EOpenBidHallEnum(Enum):
+    CHOOSEEVAL = 37
+    CHOOSEOPENBID = 36
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_sucreditcode_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_sucreditcode_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_timestamp_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/src/gmsofttest/gm_yaml_process_utils.py` & `gmsofttest-0.0.9/src/gmsofttest/gm_yaml_process_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.8/src/gmsofttest.egg-info/PKG-INFO` & `gmsofttest-0.0.9/src/gmsofttest.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.8
+Version: 0.0.9
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 License-File: LICENSE
 
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
+v0.0.9
+  demo演示
+
 v0.0.8
  修改gm_prase_response的调用名称为gm_extract_json
  增加gm_sucreditcode_utils，用于生成企业社会信用代码
 
 v0.0.6 
  修改gm_request_utils的请求参数verfiy的默认值,由NONE调整成False
```

### Comparing `gmsofttest-0.0.8/src/gmsofttest.egg-info/SOURCES.txt` & `gmsofttest-0.0.9/src/gmsofttest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

