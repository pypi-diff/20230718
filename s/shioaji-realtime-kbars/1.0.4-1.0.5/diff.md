# Comparing `tmp/shioaji_realtime_kbars-1.0.4.tar.gz` & `tmp/shioaji_realtime_kbars-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_realtime_kbars-1.0.4.tar", last modified: Mon Jul 17 15:53:21 2023, max compression
+gzip compressed data, was "shioaji_realtime_kbars-1.0.5.tar", last modified: Tue Jul 18 16:47:37 2023, max compression
```

## Comparing `shioaji_realtime_kbars-1.0.4.tar` & `shioaji_realtime_kbars-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:21.002124 shioaji_realtime_kbars-1.0.4/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.4/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4313 2023-07-17 15:53:21.002124 shioaji_realtime_kbars-1.0.4/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3719 2023-07-17 15:52:52.000000 shioaji_realtime_kbars-1.0.4/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.4/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      764 2023-07-17 15:53:21.006124 shioaji_realtime_kbars-1.0.4/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:20.994124 shioaji_realtime_kbars-1.0.4/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:20.998124 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5228 2023-07-17 15:51:45.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-17 15:53:21.002124 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4313 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       21 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-07-17 15:53:20.000000 shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.5/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5851 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5257 2023-07-18 16:47:01.000000 shioaji_realtime_kbars-1.0.5/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.5/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      764 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.592853 shioaji_realtime_kbars-1.0.5/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.596853 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5398 2023-07-18 16:35:18.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-18 16:47:37.600853 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5851 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       21 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-07-18 16:47:37.000000 shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/top_level.txt
```

### Comparing `shioaji_realtime_kbars-1.0.4/PKG-INFO` & `shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji_realtime_kbars
-Version: 1.0.4
+Name: shioaji-realtime-kbars
+Version: 1.0.5
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
   <p align="center">
     An Extensions help you streaming with real-time data
     <br/>
     <br/>
   </p>
 </p>
 
-![Contributors](https://img.shields.io/github/contributors/NickLin910221/Shioaji_Realtime_Kline?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/NickLin910221/Shioaji_Realtime_Kline?style=social) ![Issues](https://img.shields.io/github/issues/NickLin910221/Shioaji_Realtime_Kline) 
+![Contributors](https://img.shields.io/github/contributors/NickLin910221/Shioaji_Realtime_Kline?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/NickLin910221/Shioaji_Realtime_Kline?style=social) ![Issues](https://img.shields.io/github/issues/NickLin910221/Shioaji_Realtime_Kline) [![PyPI Latest Release](https://img.shields.io/pypi/v/shioaji-realtime-kbars.svg)](https://pypi.org/project/shioaji-realtime-kbars/) [![PyPI Downloads](https://img.shields.io/pypi/dm/shioaji-realtime-kbars.svg?label=PyPI%20downloads)](https://pypi.org/project/shioaji-realtime-kbars/)
 
 ## Table Of Contents
 
 * [About the Project](#about-the-project)
 * [Description](#description)
 * [Getting Started](#getting-started)
 * [Usage](#usage)
@@ -75,14 +75,15 @@
 
 ```sh
 pip install shioaji_realtime_kbars
 ```
 
 ## Usage
 
+### kbars
 Refer to the [shioaji sample](https://sinotrade.github.io/tutor/market_data/historical/#kbar)
 
 ```
 import pandas as pd
 kbars = api.kbars(
     contract=api.Contracts.Stocks["2330"], 
     start="2023-01-15", 
@@ -114,17 +115,62 @@
     print(df.tail(2), end = "\n")
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
+### Callback funtion
+shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe?
+
+Signature:
+shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe(
+    contract: List[Union[shioaji.contracts.Option, shioaji.contracts.Future, shioaji.contracts.Stock, shioaji.contracts.Index]],
+    last_days: int = 0,
+    cb: Any = List[[callback_function, period]]
+) -> None
+
+### Example
+If you want to clearly write your strategy. You can refer to example
+
+```
+def strategy(period, kbars):
+    print(period)
+    df = pd.DataFrame({**kbars}, columns = ["ts", "Open", "High", "Low", "Close", "Volume", "Amount"])
+    df.ts = pd.to_datetime(df.ts)
+
+    ### Write your strategy here ###
+
+    print(df.tail(5), end = "\n")
+
+if __name__ == "__main__":
+
+    api = sj.Shioaji(simulation = True)
+
+    api.login(
+        api_key=config.API_KEY, 
+        secret_key=config.API_SECRET
+    )
+
+    Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
+    Contracts.subscribe(api.Contracts.Futures.MXF.MXFR1, last_days = 3, cb = [[strategy, "1min"], [strategy, "5min"]])
+
+    @api.on_tick_fop_v1()
+    def callback(exchange : Exchange, tick : TickFOPv1):
+        Contracts.update(tick, "fop")
+
+    Event().wait()
+```
+
+
 ## Version
+### v1.0.5 (2023/7/19)
+#### * Add callback function
 ### v1.0.4 (2023/7/17)
-#### * Fix resamplind will have some NaN rows
+#### * Fix resampling will have some NaN rows
 ### v1.0.3 (2023/6/30)
 ### v1.0.2 (2023/6/30)
 #### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
```

### Comparing `shioaji_realtime_kbars-1.0.4/README.md` & `shioaji_realtime_kbars-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+Metadata-Version: 2.1
+Name: shioaji_realtime_kbars
+Version: 1.0.5
+Summary: An Extensions help you streaming with real-time data
+Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
+Author: NickLin910221
+Author-email: nicklin910221@gmail.com
+Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
+Keywords: shioaji
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <br/>
 <p align="center">
   <h3 align="center">Shioaji Realtime Kline Extension
 </h3>
 
   <p align="center">
     An Extensions help you streaming with real-time data
     <br/>
     <br/>
   </p>
 </p>
 
-![Contributors](https://img.shields.io/github/contributors/NickLin910221/Shioaji_Realtime_Kline?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/NickLin910221/Shioaji_Realtime_Kline?style=social) ![Issues](https://img.shields.io/github/issues/NickLin910221/Shioaji_Realtime_Kline) 
+![Contributors](https://img.shields.io/github/contributors/NickLin910221/Shioaji_Realtime_Kline?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/NickLin910221/Shioaji_Realtime_Kline?style=social) ![Issues](https://img.shields.io/github/issues/NickLin910221/Shioaji_Realtime_Kline) [![PyPI Latest Release](https://img.shields.io/pypi/v/shioaji-realtime-kbars.svg)](https://pypi.org/project/shioaji-realtime-kbars/) [![PyPI Downloads](https://img.shields.io/pypi/dm/shioaji-realtime-kbars.svg?label=PyPI%20downloads)](https://pypi.org/project/shioaji-realtime-kbars/)
 
 ## Table Of Contents
 
 * [About the Project](#about-the-project)
 * [Description](#description)
 * [Getting Started](#getting-started)
 * [Usage](#usage)
@@ -59,14 +75,15 @@
 
 ```sh
 pip install shioaji_realtime_kbars
 ```
 
 ## Usage
 
+### kbars
 Refer to the [shioaji sample](https://sinotrade.github.io/tutor/market_data/historical/#kbar)
 
 ```
 import pandas as pd
 kbars = api.kbars(
     contract=api.Contracts.Stocks["2330"], 
     start="2023-01-15", 
@@ -98,17 +115,62 @@
     print(df.tail(2), end = "\n")
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
+### Callback funtion
+shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe?
+
+Signature:
+shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe(
+    contract: List[Union[shioaji.contracts.Option, shioaji.contracts.Future, shioaji.contracts.Stock, shioaji.contracts.Index]],
+    last_days: int = 0,
+    cb: Any = List[[callback_function, period]]
+) -> None
+
+### Example
+If you want to clearly write your strategy. You can refer to example
+
+```
+def strategy(period, kbars):
+    print(period)
+    df = pd.DataFrame({**kbars}, columns = ["ts", "Open", "High", "Low", "Close", "Volume", "Amount"])
+    df.ts = pd.to_datetime(df.ts)
+
+    ### Write your strategy here ###
+
+    print(df.tail(5), end = "\n")
+
+if __name__ == "__main__":
+
+    api = sj.Shioaji(simulation = True)
+
+    api.login(
+        api_key=config.API_KEY, 
+        secret_key=config.API_SECRET
+    )
+
+    Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
+    Contracts.subscribe(api.Contracts.Futures.MXF.MXFR1, last_days = 3, cb = [[strategy, "1min"], [strategy, "5min"]])
+
+    @api.on_tick_fop_v1()
+    def callback(exchange : Exchange, tick : TickFOPv1):
+        Contracts.update(tick, "fop")
+
+    Event().wait()
+```
+
+
 ## Version
+### v1.0.5 (2023/7/19)
+#### * Add callback function
 ### v1.0.4 (2023/7/17)
-#### * Fix resamplind will have some NaN rows
+#### * Fix resampling will have some NaN rows
 ### v1.0.3 (2023/6/30)
 ### v1.0.2 (2023/6/30)
 #### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
```

### Comparing `shioaji_realtime_kbars-1.0.4/setup.cfg` & `shioaji_realtime_kbars-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_realtime_kbars
-version = 1.0.4
+version = 1.0.5
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you streaming with real-time data
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/Shioaji_Realtime_Kline
```

### Comparing `shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py` & `shioaji_realtime_kbars-1.0.5/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,22 +38,23 @@
                            Close = kbars_df["Close"].values.tolist(), 
                            Volume = kbars_df["Volume"].values.tolist(), 
                            Amount = kbars_df["Amount"].values.tolist())
         return kbars
 
 class Contracts:
 
-    __slots__ = ["api", "contract", "last_days", "kbars", "cache"]
+    __slots__ = ["api", "contract", "last_days", "kbars", "cache", "cb"]
 
-    def __init__(self, api, contract, last_days = 0):
+    def __init__(self, api, contract, cb, last_days = 0):
         self.api = api
         self.contract = contract
         self.last_days = last_days
         self.fetchdata()
         self.subscribe()
+        self.cb = cb
 
     def fetchdata(self):
         res = self.api.kbars(
             contract = self.contract, 
             start = dt.datetime.strftime(dt.datetime.today() - dt.timedelta(days = self.last_days), "%Y-%m-%d"), 
             end = dt.datetime.strftime(dt.datetime.now(), "%Y-%m-%d")
         )
@@ -64,35 +65,38 @@
             contract = self.contract,
             quote_type = sj.constant.QuoteType.Tick,
             version = sj.constant.QuoteVersion.v1
         )
 
     def update(self, tick):
         self.kbars.update({"ts" : (math.floor(int(tick.datetime.replace(tzinfo=dt.timezone.utc).timestamp() * 1000000000) / 60000000000) + 1) * 60000000000, "Open" : float(tick.open), "High" : float(tick.high), "Low" : float(tick.low), "Close" : float(tick.close), "Volume" :  tick.volume, "Amount" : float(tick.amount)})
+        for cb, period in self.cb:
+            print(cb, period)
+            cb(period, self.getklines(period))
 
     def getklines(self, period):
         return self.kbars.getKlines(period)
     
 class ShioajiRealtimeKbars():
 
     __slots__ = ["api", "stk_Contracts", "fop_Contracts"]
 
     def __init__(self, api):
         self.api = api
         self.stk_Contracts, self.fop_Contracts = [], []
 
-    def subscribe(self, contract, last_days = 0):
+    def subscribe(self, contract, last_days = 0, cb = []):
         if contract.__class__ is sj.contracts.Stock:
             for _contract_ in self.stk_Contracts:
                 if contract.code == _contract_.contract.code: return
-            self.stk_Contracts.append(Contracts(self.api, contract, last_days = last_days))    
+            self.stk_Contracts.append(Contracts(self.api, contract, last_days = last_days, cb = cb))    
         elif contract.__class__ is sj.contracts.Future or contract.__class__ is sj.contracts.Option:
             for _contract_ in self.fop_Contracts:
                 if contract.target_code == _contract_.contract.target_code or contract.code == _contract_.contract.code: return
-            self.fop_Contracts.append(Contracts(self.api, contract, last_days = last_days))
+            self.fop_Contracts.append(Contracts(self.api, contract, last_days = last_days, cb = cb))
             
     def update(self, tick, type):
         if type == "stk":
             for _contract_ in self.stk_Contracts:
                 if tick.code == _contract_.contract.code: _contract_.update(tick)
         elif type == "fop":
             for _contract_ in self.fop_Contracts:
```

### Comparing `shioaji_realtime_kbars-1.0.4/src/shioaji_realtime_kbars.egg-info/PKG-INFO` & `shioaji_realtime_kbars-1.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 2.1
-Name: shioaji-realtime-kbars
-Version: 1.0.4
-Summary: An Extensions help you streaming with real-time data
-Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
-Author: NickLin910221
-Author-email: nicklin910221@gmail.com
-Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
-Keywords: shioaji
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <br/>
 <p align="center">
   <h3 align="center">Shioaji Realtime Kline Extension
 </h3>
 
   <p align="center">
     An Extensions help you streaming with real-time data
     <br/>
     <br/>
   </p>
 </p>
 
-![Contributors](https://img.shields.io/github/contributors/NickLin910221/Shioaji_Realtime_Kline?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/NickLin910221/Shioaji_Realtime_Kline?style=social) ![Issues](https://img.shields.io/github/issues/NickLin910221/Shioaji_Realtime_Kline) 
+![Contributors](https://img.shields.io/github/contributors/NickLin910221/Shioaji_Realtime_Kline?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/NickLin910221/Shioaji_Realtime_Kline?style=social) ![Issues](https://img.shields.io/github/issues/NickLin910221/Shioaji_Realtime_Kline) [![PyPI Latest Release](https://img.shields.io/pypi/v/shioaji-realtime-kbars.svg)](https://pypi.org/project/shioaji-realtime-kbars/) [![PyPI Downloads](https://img.shields.io/pypi/dm/shioaji-realtime-kbars.svg?label=PyPI%20downloads)](https://pypi.org/project/shioaji-realtime-kbars/)
 
 ## Table Of Contents
 
 * [About the Project](#about-the-project)
 * [Description](#description)
 * [Getting Started](#getting-started)
 * [Usage](#usage)
@@ -75,14 +59,15 @@
 
 ```sh
 pip install shioaji_realtime_kbars
 ```
 
 ## Usage
 
+### kbars
 Refer to the [shioaji sample](https://sinotrade.github.io/tutor/market_data/historical/#kbar)
 
 ```
 import pandas as pd
 kbars = api.kbars(
     contract=api.Contracts.Stocks["2330"], 
     start="2023-01-15", 
@@ -114,17 +99,62 @@
     print(df.tail(2), end = "\n")
     MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
     df = pd.DataFrame({**MXFR1_5K })
     df.ts = pd.to_datetime(df.ts)
     print(df.tail(2), end = "\n")
 ```
 
+### Callback funtion
+shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe?
+
+Signature:
+shioaji_realtime_kbars.ShioajiRealtimeKbars.subscribe(
+    contract: List[Union[shioaji.contracts.Option, shioaji.contracts.Future, shioaji.contracts.Stock, shioaji.contracts.Index]],
+    last_days: int = 0,
+    cb: Any = List[[callback_function, period]]
+) -> None
+
+### Example
+If you want to clearly write your strategy. You can refer to example
+
+```
+def strategy(period, kbars):
+    print(period)
+    df = pd.DataFrame({**kbars}, columns = ["ts", "Open", "High", "Low", "Close", "Volume", "Amount"])
+    df.ts = pd.to_datetime(df.ts)
+
+    ### Write your strategy here ###
+
+    print(df.tail(5), end = "\n")
+
+if __name__ == "__main__":
+
+    api = sj.Shioaji(simulation = True)
+
+    api.login(
+        api_key=config.API_KEY, 
+        secret_key=config.API_SECRET
+    )
+
+    Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
+    Contracts.subscribe(api.Contracts.Futures.MXF.MXFR1, last_days = 3, cb = [[strategy, "1min"], [strategy, "5min"]])
+
+    @api.on_tick_fop_v1()
+    def callback(exchange : Exchange, tick : TickFOPv1):
+        Contracts.update(tick, "fop")
+
+    Event().wait()
+```
+
+
 ## Version
+### v1.0.5 (2023/7/19)
+#### * Add callback function
 ### v1.0.4 (2023/7/17)
-#### * Fix resamplind will have some NaN rows
+#### * Fix resampling will have some NaN rows
 ### v1.0.3 (2023/6/30)
 ### v1.0.2 (2023/6/30)
 #### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
```

