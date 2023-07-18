# Comparing `tmp/TinetApiRequest-0.1.9.tar.gz` & `tmp/TinetApiRequest-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-0.1.9.tar", last modified: Fri Jul 14 02:57:09 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-0.1.9.1.tar", last modified: Tue Jul 18 07:10:42 2023, max compression
```

## Comparing `TinetApiRequest-0.1.9.tar` & `TinetApiRequest-0.1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/
--rw-rw-rw-   0        0        0      272 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3690 2023-06-28 10:50:15.000000 TinetApiRequest-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      272 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      653 2023-07-14 02:56:37.000000 TinetApiRequest-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/tinet/
--rw-rw-rw-   0        0        0    21866 2023-07-14 02:51:06.000000 TinetApiRequest-0.1.9/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-06-28 10:40:40.000000 TinetApiRequest-0.1.9/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-0.1.9/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-0.1.9/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/
+-rw-rw-rw-   0        0        0      274 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-0.1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-07-18 07:04:56.000000 TinetApiRequest-0.1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/tinet/
+-rw-rw-rw-   0        0        0    21950 2023-07-18 07:04:01.000000 TinetApiRequest-0.1.9.1/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-0.1.9.1/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9.1/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9.1/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9.1/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-0.1.9.1/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-0.1.9.1/tinet/__init__.py
```

### Comparing `TinetApiRequest-0.1.9/README.md` & `TinetApiRequest-0.1.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## 项目名称
 
 API自动化测试框架,封装requests库.使用Yaml文件管理测试用例,支持数据驱动,支持多环境配置,支持多线程执行,支持测试报告生成.
 
-当前版本 v0.1.0
+当前版本 https://pypi.org/project/TinetApiRequest/
 ## 项目结构
 
 ```angular2html
 ├── dist # 打包目录 版本发布
 ├── test # 测试目录 测试类
 ├── tinet # 源码目录 框架源码
 ```
```

### Comparing `TinetApiRequest-0.1.9/setup.py` & `TinetApiRequest-0.1.9.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="0.1.9",
+    version="0.1.9.1",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-0.1.9/tinet/APIRequest.py` & `TinetApiRequest-0.1.9.1/tinet/APIRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                     allure.attach(f"{ass.get('status_code')}  ,response结果: {response.status_code}", name=f"断言status_code结束", attachment_type=allure.attachment_type.TEXT)
                     self.assertChoose(str(response.status_code) == str(ass.get('status_code')), f"status_code断言失败: {ass.get('status_code')}  ,response结果: {response.status_code}", failType)
                     continue
             jsonpathResults = jsonpath.jsonpath(response.json(), ass.get(key)[0])
             if jsonpathResults is False:
                 log.info(f'提取{ass.get(key)[0]}失败，请检查格式')
                 allure.attach(f"提取{ass.get(key)[0]}失败，请检查格式", name=f"提取{ass.get(key)[0]}失败，请检查格式", attachment_type=allure.attachment_type.TEXT)
-                self.assertChoose(1 > 2, f"提取response失败，断言失败", failType)
+                self.assertChoose(1 > 2, f"提取{ass.get(key)[0]}失败，断言失败, response结果: {json.dumps(response.text, indent=4, ensure_ascii=False)}", failType)
                 continue
             if 'eq' in ass:
                 # 相等判断 都转为str进行判断
                 expectedResults = PlaceholderYaml(attrObj=bean, reString=ass.get('eq')[1]).replace().replaced_str
                 # 判断 expectedResults 是否在 jsonpathResults list中  判断类型
                 assResults = str(expectedResults) in [str(item) for item in jsonpathResults]
                 self.assertChoose(assResults is True, f"eq断言失败: {jsonpathResults} 不等于 {expectedResults}", failType)
```

### Comparing `TinetApiRequest-0.1.9/tinet/ApiConfig.py` & `TinetApiRequest-0.1.9.1/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9/tinet/LogUtil.py` & `TinetApiRequest-0.1.9.1/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9/tinet/RequestUtil.py` & `TinetApiRequest-0.1.9.1/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9/tinet/SignUtil.py` & `TinetApiRequest-0.1.9.1/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9/tinet/YamlUtil.py` & `TinetApiRequest-0.1.9.1/tinet/YamlUtil.py`

 * *Files identical despite different names*

