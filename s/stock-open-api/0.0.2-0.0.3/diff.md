# Comparing `tmp/stock-open-api-0.0.2.tar.gz` & `tmp/stock-open-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-0.0.2.tar", last modified: Mon Jul 17 10:09:47 2023, max compression
+gzip compressed data, was "dist/stock-open-api-0.0.3.tar", last modified: Tue Jul 18 14:41:57 2023, max compression
```

## Comparing `stock-open-api-0.0.2.tar` & `stock-open-api-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,47 @@
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/
--rwxr-xr-x   0 hina       (501) staff       (20)      414 2023-07-17 03:13:13.000000 stock-open-api-0.0.2/MANIFEST.in
--rw-r--r--   0 hina       (501) staff       (20)     4951 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)     2833 2023-07-17 09:05:44.000000 stock-open-api-0.0.2/README.md
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/requirements/
--rw-r--r--   0 hina       (501) staff       (20)        9 2023-07-17 03:10:06.000000 stock-open-api-0.0.2/requirements/production.txt
--rw-r--r--   0 hina       (501) staff       (20)       38 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/setup.cfg
--rwxr-xr-x   0 hina       (501) staff       (20)     3181 2023-07-17 10:08:42.000000 stock-open-api-0.0.2/setup.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/
--rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 02:58:35.000000 stock-open-api-0.0.2/stock_open_api/__init__.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/api/
--rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 06:54:43.000000 stock-open-api-0.0.2/stock_open_api/api/__init__.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/
--rw-r--r--   0 hina       (501) staff       (20)      136 2023-07-17 03:07:42.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)     6384 2023-07-17 07:46:00.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 hina       (501) staff       (20)     3495 2023-07-17 07:04:03.000000 stock-open-api-0.0.2/stock_open_api/api/eastmoney/hk_stock_config.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/api/sse/
--rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 07:14:57.000000 stock-open-api-0.0.2/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)     2972 2023-07-17 07:43:31.000000 stock-open-api-0.0.2/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 hina       (501) staff       (20)     1471 2023-07-17 07:18:17.000000 stock-open-api-0.0.2/stock_open_api/api/sse/sh_stock_config.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/items/
--rw-r--r--   0 hina       (501) staff       (20)      102 2023-07-17 06:55:24.000000 stock-open-api-0.0.2/stock_open_api/items/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      333 2023-07-17 07:00:59.000000 stock-open-api-0.0.2/stock_open_api/items/list_item.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api/utils/
--rw-r--r--   0 hina       (501) staff       (20)       79 2023-07-17 03:33:51.000000 stock-open-api-0.0.2/stock_open_api/utils/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      263 2023-07-17 03:39:39.000000 stock-open-api-0.0.2/stock_open_api/utils/time_util.py
--rw-r--r--   0 hina       (501) staff       (20)      209 2023-07-17 03:42:26.000000 stock-open-api-0.0.2/stock_open_api/utils/ua_util.py
--rw-r--r--   0 hina       (501) staff       (20)       95 2023-07-17 09:55:34.000000 stock-open-api-0.0.2/stock_open_api/version.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/
--rw-r--r--   0 hina       (501) staff       (20)     4951 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)      772 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 hina       (501) staff       (20)        9 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 hina       (501) staff       (20)       21 2023-07-17 10:09:47.000000 stock-open-api-0.0.2/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2023-07-17 07:07:04.000000 stock-open-api-0.0.2/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 14:41:47.000000 stock-open-api-0.0.3/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:41:57.000000 stock-open-api-0.0.3/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-0.0.2/setup.py` & `stock-open-api-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.2/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 """
 @File    : hk_stock.py
 @Date    : 2023-07-17
 港股相关接口
 """
 import json
 
-import requests
-
 from stock_open_api.api.eastmoney import hk_stock_config
 from stock_open_api.items.list_item import ListItem
-from stock_open_api.utils import time_util
+from stock_open_api.utils import time_util, request_util
 
 
 def get_list(page=1, size=20):
     """
     港股列表
     东方财富网 > 行情中心 > 港股市场 > 全部港股
     http://quote.eastmoney.com/center/gridlist.html#hk_stocks
@@ -57,15 +55,15 @@
         'fid': 'f3',
         'fs': 'm:128 t:3,m:128 t:4,m:128 t:1,m:128 t:2',
         'fields': 'f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f12,f13,f14,f15,f16,f17,f18,f19,f20,f21,f23,f24,f25,f26,f22,f33,f11,f62,f128,f136,f115,f152',
         # '_': 1689562954034
         '_': time_util.get_timespan_13()
     }
 
-    res = requests.get(url, params, headers=hk_stock_config.headers)
+    res = request_util.get(url, params)
 
     data = res.json()
 
     list_item = ListItem()
     if data['data'] is None:
         return list_item
 
@@ -73,15 +71,16 @@
 
     items = []
     for row in data['data']['diff']:
         item = {}
 
         for map_item in hk_stock_config.list_key_map:
             item[map_item['title']] = row.get(map_item['key'])
-            items.append(item)
+
+        items.append(item)
 
     list_item.items = items
     return list_item
 
 
 def get_list_iter(size=100):
     """
@@ -101,15 +100,17 @@
         yield data
 
 
 def get_org_profile(code):
     """
     公司资料
     http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile
-    :param code: str
+
+    :param code: str eg: 00491
+
     :return:
     {
       "证券代码": "00491.HK",
       "公司名称": "英皇文化产业集团有限公司",
       "英文名称": "Emperor Culture Group Limited",
       "注册地": "Bermuda 百慕大",
       "注册地址": "Clarendon House, 2 Church Street, Hamilton, Bermuda",
@@ -141,15 +142,15 @@
         'sortTypes': '',
         'sortColumns': '',
         'source': 'F10',
         'client': 'PC',
         'v': '05607491999280683',
     }
 
-    res = requests.get(url, params, headers=hk_stock_config.headers)
+    res = request_util.get(url, params)
 
     data = res.json()['result']['data'][0]
 
     item = {}
     for row in hk_stock_config.org_profile_key_map:
         value = data.get(row['key'])
         if isinstance(value, str):
@@ -160,15 +161,17 @@
     return item
 
 
 def get_security_info(code):
     """
     证券资料
     http://emweb.securities.eastmoney.com/PC_HKF10/pages/home/index.html?code=00491&type=web&color=w#/CompanyProfile
-    :param code: str
+
+    :param code: str  eg: 00491
+
     :return:
     {
       "证券代码": "00491.HK",
       "证券简称": "英皇文化产业",
       "上市日期": "1992-06-10 00:00:00",
       "证券类型": "非H股",
       "交易所": "香港交易所",
@@ -191,15 +194,15 @@
         'sortTypes': '',
         'sortColumns': '',
         'source': 'F10',
         'client': 'PC',
         'v': '05299608968630529',
     }
 
-    res = requests.get(url, params, headers=hk_stock_config.headers)
+    res = request_util.get(url, params)
 
     data = res.json()['result']['data'][0]
 
     item = {}
     for row in hk_stock_config.security_info_key_map:
         value = data.get(row['key'])
         if isinstance(value, str):
```

### Comparing `stock-open-api-0.0.2/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-0.0.3/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @File    : hk_stocks_config.py
 @Date    : 2023-07-17
 """
-from stock_open_api.utils import ua_util
-
-headers = {
-    'User-Agent': ua_util.User_Agent
-}
 
 # 配置数据
 # http://quote.eastmoney.com/center/js/gridlist.js
 # 港股--全部
 
 list_key_map = [
     {
```

### Comparing `stock-open-api-0.0.2/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 """
 sh_stock.py
 上海证券交易所
 """
 import json
 import re
 import time
-import requests
 
 from stock_open_api.api.sse import sh_stock_config
+from stock_open_api.log import logger
+from stock_open_api.utils import request_util
 
 
 def get_company_info(stock_code):
     """
     股票概况 / 公司信息 / 公司概况
 
     页面地址
         eg: http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE=688001
 
     :param stock_code: eg 688001
+
     :return:
     {
       "公司代码": "688001",
       "上市日-A": "",
       "代码-A": "688001",
       "简称-A": "华兴源创",
       "代码-B": "-",
@@ -55,15 +57,17 @@
       "是否境外上市": "-",
       "境外上市地": "-"
     }
 
     """
     url = "http://query.sse.com.cn/commonQuery.do"
     detail_url = f'http://www.sse.com.cn/assortment/stock/list/info/company/index.shtml?COMPANY_CODE={stock_code}'
-    # print('Referer', detail_url)
+    # print()
+
+    logger.debug('Referer: %s', detail_url)
 
     params = {
         'jsonCallBack': 'jsonpCallback22015',
         'isPagination': 'false',
         'sqlId': 'COMMON_SSE_ZQPZ_GP_GPLB_C',
         'productid': stock_code,
         '_': int(time.time() * 1000),
@@ -76,21 +80,21 @@
         'Cache-Control': 'no-cache',
         'Connection': 'keep-alive',
         'Pragma': 'no-cache',
         'Referer': detail_url,
         'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36',
     }
 
-    response = requests.get(url, params, headers=headers)
+    response = request_util.get(url, params, headers=headers)
 
     ret = re.match("jsonpCallback22015\((.*)\)", response.text)
     data = json.loads(ret.group(1))['result'][0]
 
     item = {}
     for key, value in sh_stock_config.company_info_key_map.items():
         item[key] = data.get(value, '').strip()
 
     return item
 
 
 if __name__ == '__main__':
-    print(json.dumps(get_company_info(688001), indent=2, ensure_ascii=False))
+    print(json.dumps(get_company_info(688627), indent=2, ensure_ascii=False))
```

### Comparing `stock-open-api-0.0.2/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-0.0.3/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-0.0.2/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-0.0.3/stock_open_api.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 MANIFEST.in
 README.md
 setup.py
 requirements/production.txt
 stock_open_api/__init__.py
+stock_open_api/log.py
 stock_open_api/version.py
 stock_open_api.egg-info/PKG-INFO
 stock_open_api.egg-info/SOURCES.txt
 stock_open_api.egg-info/dependency_links.txt
 stock_open_api.egg-info/requires.txt
 stock_open_api.egg-info/top_level.txt
 stock_open_api.egg-info/zip-safe
 stock_open_api/api/__init__.py
 stock_open_api/api/eastmoney/__init__.py
+stock_open_api/api/eastmoney/company.py
+stock_open_api/api/eastmoney/company_config.py
 stock_open_api/api/eastmoney/hk_stock.py
 stock_open_api/api/eastmoney/hk_stock_config.py
+stock_open_api/api/eastmoney/kcb_stock.py
+stock_open_api/api/eastmoney/kcb_stock_config.py
+stock_open_api/api/eastmoney/neeq_stock.py
+stock_open_api/api/eastmoney/neeq_stock_config.py
+stock_open_api/api/eastmoney/sz_stock.py
+stock_open_api/api/eastmoney/us_chinese_stock.py
+stock_open_api/api/eastmoney/us_chinese_stock_config.py
 stock_open_api/api/sse/__init__.py
 stock_open_api/api/sse/sh_stock.py
 stock_open_api/api/sse/sh_stock_config.py
 stock_open_api/items/__init__.py
 stock_open_api/items/list_item.py
 stock_open_api/utils/__init__.py
+stock_open_api/utils/json_util.py
+stock_open_api/utils/request_util.py
 stock_open_api/utils/time_util.py
 stock_open_api/utils/ua_util.py
```

