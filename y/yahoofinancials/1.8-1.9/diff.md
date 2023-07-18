# Comparing `tmp/yahoofinancials-1.8.tar.gz` & `tmp/yahoofinancials-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yahoofinancials-1.8.tar", last modified: Tue Jan 10 04:04:44 2023, max compression
+gzip compressed data, was "dist/yahoofinancials-1.9.tar", last modified: Sat Jan 14 07:10:19 2023, max compression
```

## Comparing `yahoofinancials-1.8.tar` & `yahoofinancials-1.9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-10 04:04:44.000000 yahoofinancials-1.8/
--rw-r--r--   0 alt       (1000) alt       (1000)       19 2019-01-12 19:28:20.000000 yahoofinancials-1.8/MANIFEST.in
-drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/
--rw-r--r--   0 alt       (1000) alt       (1000)    31879 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/PKG-INFO
--rw-r--r--   0 alt       (1000) alt       (1000)        1 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/dependency_links.txt
--rw-r--r--   0 alt       (1000) alt       (1000)        1 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/not-zip-safe
--rw-r--r--   0 alt       (1000) alt       (1000)      320 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/SOURCES.txt
--rw-r--r--   0 alt       (1000) alt       (1000)       48 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/requires.txt
--rw-r--r--   0 alt       (1000) alt       (1000)       16 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials.egg-info/top_level.txt
--rw-r--r--   0 alt       (1000) alt       (1000)       38 2023-01-10 04:04:44.000000 yahoofinancials-1.8/setup.cfg
--rw-r--r--   0 alt       (1000) alt       (1000)    31879 2023-01-10 04:04:44.000000 yahoofinancials-1.8/PKG-INFO
-drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-10 04:04:44.000000 yahoofinancials-1.8/yahoofinancials/
--rw-r--r--   0 alt       (1000) alt       (1000)    41014 2023-01-10 04:04:00.000000 yahoofinancials-1.8/yahoofinancials/__init__.py
--rw-r--r--   0 alt       (1000) alt       (1000)     1585 2023-01-10 04:04:00.000000 yahoofinancials-1.8/setup.py
--rw-r--r--   0 alt       (1000) alt       (1000)    24692 2023-01-10 04:04:00.000000 yahoofinancials-1.8/README.rst
-drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-10 04:04:44.000000 yahoofinancials-1.8/test/
--rw-r--r--   0 alt       (1000) alt       (1000)     5324 2023-01-10 04:04:00.000000 yahoofinancials-1.8/test/test_yahoofinancials.py
+drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-14 07:10:19.000000 yahoofinancials-1.9/
+-rw-r--r--   0 alt       (1000) alt       (1000)       19 2019-01-12 19:28:20.000000 yahoofinancials-1.9/MANIFEST.in
+drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/
+-rw-r--r--   0 alt       (1000) alt       (1000)    34537 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/PKG-INFO
+-rw-r--r--   0 alt       (1000) alt       (1000)        1 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/dependency_links.txt
+-rw-r--r--   0 alt       (1000) alt       (1000)        1 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/not-zip-safe
+-rw-r--r--   0 alt       (1000) alt       (1000)      392 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/SOURCES.txt
+-rw-r--r--   0 alt       (1000) alt       (1000)       63 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/requires.txt
+-rw-r--r--   0 alt       (1000) alt       (1000)       16 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials.egg-info/top_level.txt
+-rw-r--r--   0 alt       (1000) alt       (1000)       38 2023-01-14 07:10:19.000000 yahoofinancials-1.9/setup.cfg
+-rw-r--r--   0 alt       (1000) alt       (1000)    34537 2023-01-14 07:10:19.000000 yahoofinancials-1.9/PKG-INFO
+drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-14 07:10:19.000000 yahoofinancials-1.9/yahoofinancials/
+-rw-r--r--   0 alt       (1000) alt       (1000)      699 2023-01-14 07:02:01.000000 yahoofinancials-1.9/yahoofinancials/calcs.py
+-rw-r--r--   0 alt       (1000) alt       (1000)    15595 2023-01-14 07:02:01.000000 yahoofinancials-1.9/yahoofinancials/__init__.py
+-rw-r--r--   0 alt       (1000) alt       (1000)    31158 2023-01-14 07:02:01.000000 yahoofinancials-1.9/yahoofinancials/etl.py
+-rw-r--r--   0 alt       (1000) alt       (1000)     1183 2023-01-14 07:02:01.000000 yahoofinancials-1.9/yahoofinancials/maps.py
+-rw-r--r--   0 alt       (1000) alt       (1000)     1695 2023-01-14 07:07:09.000000 yahoofinancials-1.9/setup.py
+-rw-r--r--   0 alt       (1000) alt       (1000)    26779 2023-01-14 07:02:01.000000 yahoofinancials-1.9/README.rst
+drwxr-xr-x   0 alt       (1000) alt       (1000)        0 2023-01-14 07:10:19.000000 yahoofinancials-1.9/test/
+-rw-r--r--   0 alt       (1000) alt       (1000)     6155 2023-01-14 07:02:01.000000 yahoofinancials-1.9/test/test_yahoofinancials.py
```

### Comparing `yahoofinancials-1.8/yahoofinancials.egg-info/PKG-INFO` & `yahoofinancials-1.9/yahoofinancials.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 Metadata-Version: 1.1
 Name: yahoofinancials
-Version: 1.8
+Version: 1.9
 Summary: A powerful financial data module used for pulling both fundamental and technical data from Yahoo Finance
 Home-page: https://github.com/JECSand/yahoofinancials
 Author: Connor Sanders
 Author-email: connor@exceleri.com
 License: MIT
-Download-URL: https://github.com/JECSand/yahoofinancials/archive/1.8.tar.gz
+Download-URL: https://github.com/JECSand/yahoofinancials/archive/1.9.tar.gz
 Description-Content-Type: UNKNOWN
 Description: ===============
         yahoofinancials
         ===============
         
         A python module that returns stock, cryptocurrency, forex, mutual fund, commodity futures, ETF, and US Treasury financial data from Yahoo Finance.
         
         .. image:: https://github.com/JECSand/yahoofinancials/actions/workflows/test.yml/badge.svg?branch=master
             :target: https://github.com/JECSand/yahoofinancials/actions/workflows/test.yml
         
-        Current Version: v1.8
+        Current Version: v1.9
         
-        Version Released: 01/09/2023
+        Version Released: 01/14/2023
         
         Report any bugs by opening an issue here: https://github.com/JECSand/yahoofinancials/issues
         
         Overview
         --------
         A powerful financial data module used for pulling both fundamental and technical data from Yahoo Finance.
         
-        - As of Version 0.10, Yahoo Financials now returns historical pricing data for commodity futures, cryptocurrencies, ETFs, mutual funds, U.S. Treasuries, currencies, indexes, and stocks.
+        - As of Version 1.9, YahooFinancials supports optional parameters for asynchronous execution, proxies, and international requests.
+        
+        .. code-block:: python
+        
+            from yahoofinancials import YahooFinancials
+            tickers = ['AAPL', 'GOOG', 'C']
+            yahoo_financials = YahooFinancials(tickers, concurrent=True, max_workers=8, country="US")
+            balance_sheet_data_qt = yahoo_financials.get_financial_stmts('quarterly', 'balance')
+            print(balance_sheet_data_qt)
+        
+            proxy_addresses = [ "mysuperproxy.com:5000", "mysuperproxy.com:5001"]
+            yahoo_financials = YahooFinancials(tickers, concurrent=True, proxies=proxy_addresses)
+            balance_sheet_data_qt = yahoo_financials.get_financial_stmts('quarterly', 'balance')
+            print(balance_sheet_data_qt)
+        
+        - New methods in Version 1.9:
+            - get_stock_profile_data()
+            - get_financial_data()
+        
         
         Installation
         -------------
-        - yahoofinancials runs on Python 3.6, 3.7, 3.8, 3.9, and 3.10.
-        - This package depends on beautifulsoup4, pytz, and cryptography to work.
+        - yahoofinancials runs on Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
+        - This package depends on beautifulsoup4, pytz, requests, and cryptography to work.
         
         1. Installation using pip:
         
         - Linux/Mac:
         
         .. code-block:: bash
         
@@ -72,15 +90,15 @@
             $ cd yahoofinancials
             $ python test/test_yahoofinancials.py
         
         Module Methods
         --------------
         - The financial data from all methods is returned as JSON.
         - You can run multiple symbols at once using an inputted array or run an individual symbol using an inputted string.
-        - YahooFinancials works with Python 3.6, 3.7, 3.8, 3.9, and 3.10 and runs on all operating systems. (Windows, Mac, Linux).
+        - YahooFinancials works with Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11 and runs on all operating systems. (Windows, Mac, Linux).
         
         Featured Methods
         ^^^^^^^^^^^^^^^^
         1. get_financial_stmts(frequency, statement_type, reformat=True)
         
            - frequency can be either 'annual' or 'quarterly'.
            - statement_type can be 'income', 'balance', 'cash' or a list of several.
@@ -152,14 +170,16 @@
         - get_price_to_sales()
         - get_exdividend_date()
         - get_book_value()
         - get_ebit()
         - get_net_income()
         - get_earnings_per_share()
         - get_key_statistics_data()
+        - get_stock_profile_data()
+        - get_financial_data()
         
         Usage Examples
         --------------
         - The class constructor can take either a single ticker or a list of tickers as it's parameter.
         - This makes it easy to initiate multiple classes for different groupings of financial assets.
         - Quarterly statement data returns the last 4 periods of data, while annual returns the last 3.
         
@@ -755,14 +775,59 @@
                         "date": 586445400,
                         "formatted_date": "1988-08-01",
                         "amount": 0.3344
                     }
                 ]
             }
         
+        13. Apple key Financial Data:
+        
+        
+        .. code-block:: python
+        
+            yahoo_financials = YahooFinancials("AAPL")
+            print(yahoo_financials.get_financial_data())
+        
+        
+        .. code-block:: javascript
+        
+            {
+                'AAPL': {
+                    'ebitdaMargins': 0.29395,
+                    'profitMargins': 0.21238,
+                    'grossMargins': 0.37818,
+                    'operatingCashflow': 69390999552,
+                    'revenueGrowth': 0.018,
+                    'operatingMargins': 0.24572,
+                    'ebitda': 76476997632,
+                    'targetLowPrice': 150,
+                    'recommendationKey': 'buy',
+                    'grossProfits': 98392000000,
+                    'freeCashflow': 42914250752,
+                    'targetMedianPrice': 270,
+                    'currentPrice': 261.78,
+                    'earningsGrowth': 0.039,
+                    'currentRatio': 1.54,
+                    'returnOnAssets': 0.11347,
+                    'numberOfAnalystOpinions': 40,
+                    'targetMeanPrice': 255.51,
+                    'debtToEquity': 119.405,
+                    'returnOnEquity': 0.55917,
+                    'targetHighPrice': 300,
+                    'totalCash': 100556996608,
+                    'totalDebt': 108046999552,
+                    'totalRevenue': 260174004224,
+                    'totalCashPerShare': 22.631,
+                    'financialCurrency': 'USD',
+                    'maxAge': 86400,
+                    'revenuePerShare': 56.341,
+                    'quickRatio': 1.384,
+                    'recommendationMean': 2.2
+                }
+            }
         
 Keywords: finance data,stocks,commodities,cryptocurrencies,currencies,forex,yahoo finance
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Office/Business :: Financial :: Investment
@@ -770,7 +835,8 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yahoofinancials-1.8/PKG-INFO` & `yahoofinancials-1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 Metadata-Version: 1.1
 Name: yahoofinancials
-Version: 1.8
+Version: 1.9
 Summary: A powerful financial data module used for pulling both fundamental and technical data from Yahoo Finance
 Home-page: https://github.com/JECSand/yahoofinancials
 Author: Connor Sanders
 Author-email: connor@exceleri.com
 License: MIT
-Download-URL: https://github.com/JECSand/yahoofinancials/archive/1.8.tar.gz
+Download-URL: https://github.com/JECSand/yahoofinancials/archive/1.9.tar.gz
 Description-Content-Type: UNKNOWN
 Description: ===============
         yahoofinancials
         ===============
         
         A python module that returns stock, cryptocurrency, forex, mutual fund, commodity futures, ETF, and US Treasury financial data from Yahoo Finance.
         
         .. image:: https://github.com/JECSand/yahoofinancials/actions/workflows/test.yml/badge.svg?branch=master
             :target: https://github.com/JECSand/yahoofinancials/actions/workflows/test.yml
         
-        Current Version: v1.8
+        Current Version: v1.9
         
-        Version Released: 01/09/2023
+        Version Released: 01/14/2023
         
         Report any bugs by opening an issue here: https://github.com/JECSand/yahoofinancials/issues
         
         Overview
         --------
         A powerful financial data module used for pulling both fundamental and technical data from Yahoo Finance.
         
-        - As of Version 0.10, Yahoo Financials now returns historical pricing data for commodity futures, cryptocurrencies, ETFs, mutual funds, U.S. Treasuries, currencies, indexes, and stocks.
+        - As of Version 1.9, YahooFinancials supports optional parameters for asynchronous execution, proxies, and international requests.
+        
+        .. code-block:: python
+        
+            from yahoofinancials import YahooFinancials
+            tickers = ['AAPL', 'GOOG', 'C']
+            yahoo_financials = YahooFinancials(tickers, concurrent=True, max_workers=8, country="US")
+            balance_sheet_data_qt = yahoo_financials.get_financial_stmts('quarterly', 'balance')
+            print(balance_sheet_data_qt)
+        
+            proxy_addresses = [ "mysuperproxy.com:5000", "mysuperproxy.com:5001"]
+            yahoo_financials = YahooFinancials(tickers, concurrent=True, proxies=proxy_addresses)
+            balance_sheet_data_qt = yahoo_financials.get_financial_stmts('quarterly', 'balance')
+            print(balance_sheet_data_qt)
+        
+        - New methods in Version 1.9:
+            - get_stock_profile_data()
+            - get_financial_data()
+        
         
         Installation
         -------------
-        - yahoofinancials runs on Python 3.6, 3.7, 3.8, 3.9, and 3.10.
-        - This package depends on beautifulsoup4, pytz, and cryptography to work.
+        - yahoofinancials runs on Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
+        - This package depends on beautifulsoup4, pytz, requests, and cryptography to work.
         
         1. Installation using pip:
         
         - Linux/Mac:
         
         .. code-block:: bash
         
@@ -72,15 +90,15 @@
             $ cd yahoofinancials
             $ python test/test_yahoofinancials.py
         
         Module Methods
         --------------
         - The financial data from all methods is returned as JSON.
         - You can run multiple symbols at once using an inputted array or run an individual symbol using an inputted string.
-        - YahooFinancials works with Python 3.6, 3.7, 3.8, 3.9, and 3.10 and runs on all operating systems. (Windows, Mac, Linux).
+        - YahooFinancials works with Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11 and runs on all operating systems. (Windows, Mac, Linux).
         
         Featured Methods
         ^^^^^^^^^^^^^^^^
         1. get_financial_stmts(frequency, statement_type, reformat=True)
         
            - frequency can be either 'annual' or 'quarterly'.
            - statement_type can be 'income', 'balance', 'cash' or a list of several.
@@ -152,14 +170,16 @@
         - get_price_to_sales()
         - get_exdividend_date()
         - get_book_value()
         - get_ebit()
         - get_net_income()
         - get_earnings_per_share()
         - get_key_statistics_data()
+        - get_stock_profile_data()
+        - get_financial_data()
         
         Usage Examples
         --------------
         - The class constructor can take either a single ticker or a list of tickers as it's parameter.
         - This makes it easy to initiate multiple classes for different groupings of financial assets.
         - Quarterly statement data returns the last 4 periods of data, while annual returns the last 3.
         
@@ -755,14 +775,59 @@
                         "date": 586445400,
                         "formatted_date": "1988-08-01",
                         "amount": 0.3344
                     }
                 ]
             }
         
+        13. Apple key Financial Data:
+        
+        
+        .. code-block:: python
+        
+            yahoo_financials = YahooFinancials("AAPL")
+            print(yahoo_financials.get_financial_data())
+        
+        
+        .. code-block:: javascript
+        
+            {
+                'AAPL': {
+                    'ebitdaMargins': 0.29395,
+                    'profitMargins': 0.21238,
+                    'grossMargins': 0.37818,
+                    'operatingCashflow': 69390999552,
+                    'revenueGrowth': 0.018,
+                    'operatingMargins': 0.24572,
+                    'ebitda': 76476997632,
+                    'targetLowPrice': 150,
+                    'recommendationKey': 'buy',
+                    'grossProfits': 98392000000,
+                    'freeCashflow': 42914250752,
+                    'targetMedianPrice': 270,
+                    'currentPrice': 261.78,
+                    'earningsGrowth': 0.039,
+                    'currentRatio': 1.54,
+                    'returnOnAssets': 0.11347,
+                    'numberOfAnalystOpinions': 40,
+                    'targetMeanPrice': 255.51,
+                    'debtToEquity': 119.405,
+                    'returnOnEquity': 0.55917,
+                    'targetHighPrice': 300,
+                    'totalCash': 100556996608,
+                    'totalDebt': 108046999552,
+                    'totalRevenue': 260174004224,
+                    'totalCashPerShare': 22.631,
+                    'financialCurrency': 'USD',
+                    'maxAge': 86400,
+                    'revenuePerShare': 56.341,
+                    'quickRatio': 1.384,
+                    'recommendationMean': 2.2
+                }
+            }
         
 Keywords: finance data,stocks,commodities,cryptocurrencies,currencies,forex,yahoo finance
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Office/Business :: Financial :: Investment
@@ -770,7 +835,8 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yahoofinancials-1.8/yahoofinancials/__init__.py` & `yahoofinancials-1.9/yahoofinancials/etl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,76 @@
-"""
-==============================
-The Yahoo Financials Module
-Version: 1.8
-==============================
-
-Author: Connor Sanders
-Email: sandersconnor1@gmail.com
-Version Released: 01/09/2023
-Tested on Python 3.6, 3.7, 3.8, 3.9, and 3.10
-
-Copyright (c) 2023 Connor Sanders
-MIT License
-
-List of Included Functions:
-
-1) get_financial_stmts(frequency, statement_type, reformat=True)
-   - frequency can be either 'annual' or 'quarterly'.
-   - statement_type can be 'income', 'balance', 'cash'.
-   - reformat optional value defaulted to true. Enter False for unprocessed raw data from Yahoo Finance.
-2) get_stock_price_data(reformat=True)
-   - reformat optional value defaulted to true. Enter False for unprocessed raw data from Yahoo Finance.
-3) get_stock_earnings_data(reformat=True)
-   - reformat optional value defaulted to true. Enter False for unprocessed raw data from Yahoo Finance.
-4) get_summary_data(reformat=True)
-   - reformat optional value defaulted to true. Enter False for unprocessed raw data from Yahoo Finance.
-5) get_stock_quote_type_data()
-6) get_historical_price_data(start_date, end_date, time_interval)
-   - Gets historical price data for currencies, stocks, indexes, cryptocurrencies, and commodity futures.
-   - start_date should be entered in the 'YYYY-MM-DD' format. First day that financial data will be pulled.
-   - end_date should be entered in the 'YYYY-MM-DD' format. Last day that financial data will be pulled.
-   - time_interval can be either 'daily', 'weekly', or 'monthly'. Parameter determines the time period interval.
-
-Usage Examples:
-from yahoofinancials import YahooFinancials
-#tickers = 'AAPL'
-#or
-tickers = ['AAPL', 'WFC', 'F', 'JPY=X', 'XRP-USD', 'GC=F']
-yahoo_financials = YahooFinancials(tickers)
-balance_sheet_data = yahoo_financials.get_financial_stmts('quarterly', 'balance')
-earnings_data = yahoo_financials.get_stock_earnings_data()
-historical_prices = yahoo_financials.get_historical_price_data('2015-01-15', '2017-10-15', 'weekly')
-"""
-
-import sys
 import calendar
-import re
-from json import loads
-import time
-from bs4 import BeautifulSoup
 import datetime
-import pytz
-import random
-try:
-    from urllib import FancyURLopener
-except:
-    from urllib.request import FancyURLopener
 import hashlib
-from base64 import b64decode
-from cryptography.hazmat.primitives import padding
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 import json
+import logging
+import random
+import re
+import time
+from base64 import b64decode
+from functools import partial
+from json import loads
+from multiprocessing import Pool
+
+import pytz
+import requests as requests
+from bs4 import BeautifulSoup
+
+from yahoofinancials.maps import COUNTRY_MAP
 
+usePycryptodome = False
+if usePycryptodome:
+    from Crypto.Cipher import AES
+    from Crypto.Util.Padding import unpad
+else:
+    from cryptography.hazmat.primitives import padding
+    from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 # track the last get timestamp to add a minimum delay between gets - be nice!
 _lastget = 0
 
 
+# logger = log_to_stderr(logging.DEBUG)
+
+
 # Custom Exception class to handle custom error
 class ManagedException(Exception):
     pass
 
 
-# Class used to open urls for financial data
-class UrlOpener(FancyURLopener):
-    version = 'w3m/0.5.3+git20180125'
+# Class used to get data from urls
+class UrlOpener:
+    user_agent_headers = {
+        'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
+    }
+
+    def __init__(self, session=None):
+        self._session = session or requests
+
+    def open(self, url, user_agent_headers=None, params=None, proxy=None, timeout=30):
+        response = self._session.get(
+            url=url,
+            params=params,
+            proxies=proxy,
+            timeout=timeout,
+            headers=user_agent_headers or self.user_agent_headers
+        )
+        return response
 
 
 def decrypt_cryptojs_aes(data):
     encrypted_stores = data['context']['dispatcher']['stores']
-    _cs = data["_cs"]
-    _cr = data["_cr"]
-    _cr = b"".join(int.to_bytes(i, length=4, byteorder="big", signed=True) for i in json.loads(_cr)["words"])
-    password = hashlib.pbkdf2_hmac("sha1", _cs.encode("utf8"), _cr, 1, dklen=32).hex()
+    if "_cs" in data and "_cr" in data:
+        _cs = data["_cs"]
+        _cr = data["_cr"]
+        _cr = b"".join(int.to_bytes(i, length=4, byteorder="big", signed=True) for i in json.loads(_cr)["words"])
+        password = hashlib.pbkdf2_hmac("sha1", _cs.encode("utf8"), _cr, 1, dklen=32).hex()
+    else:
+        password_key = next(key for key in data.keys() if key not in ["context", "plugins"])
+        password = data[password_key]
     encrypted_stores = b64decode(encrypted_stores)
     assert encrypted_stores[0:8] == b"Salted__"
     salt = encrypted_stores[8:16]
     encrypted_stores = encrypted_stores[16:]
 
     def EVPKDF(password, salt, keySize=32, ivSize=16, iterations=1, hashAlgorithm="md5") -> tuple:
         """OpenSSL EVP Key Derivation Function
@@ -94,15 +79,14 @@
             salt (Union[bytes, bytearray]): Salt to use.
             keySize (int, optional): Output key length in bytes. Defaults to 32.
             ivSize (int, optional): Output Initialization Vector (IV) length in bytes. Defaults to 16.
             iterations (int, optional): Number of iterations to perform. Defaults to 1.
             hashAlgorithm (str, optional): Hash algorithm to use for the KDF. Defaults to 'md5'.
         Returns:
             key, iv: Derived key and Initialization Vector (IV) bytes.
-
         Taken from: https://gist.github.com/rafiibrahim8/0cd0f8c46896cafef6486cb1a50a16d3
         OpenSSL original code: https://github.com/openssl/openssl/blob/master/crypto/evp/evp_key.c#L78
         """
         assert iterations > 0, "Iterations can not be less than 1."
         if isinstance(password, str):
             password = password.encode("utf-8")
         final_length = keySize + ivSize
@@ -118,29 +102,40 @@
             for _ in range(1, iterations):
                 block = hashlib.new(hashAlgorithm, block).digest()
             key_iv += block
         key, iv = key_iv[:keySize], key_iv[keySize:final_length]
         return key, iv
 
     key, iv = EVPKDF(password, salt, keySize=32, ivSize=16, iterations=1, hashAlgorithm="md5")
-    cipher = Cipher(algorithms.AES(key), modes.CBC(iv))
-    decryptor = cipher.decryptor()
-    plaintext = decryptor.update(encrypted_stores) + decryptor.finalize()
-    unpadder = padding.PKCS7(128).unpadder()
-    plaintext = unpadder.update(plaintext) + unpadder.finalize()
-    plaintext = plaintext.decode("utf-8")
+    if usePycryptodome:
+        cipher = AES.new(key, AES.MODE_CBC, iv=iv)
+        plaintext = cipher.decrypt(encrypted_stores)
+        plaintext = unpad(plaintext, 16, style="pkcs7")
+    else:
+        cipher = Cipher(algorithms.AES(key), modes.CBC(iv))
+        decryptor = cipher.decryptor()
+        plaintext = decryptor.update(encrypted_stores) + decryptor.finalize()
+        unpadder = padding.PKCS7(128).unpadder()
+        plaintext = unpadder.update(plaintext) + unpadder.finalize()
+        plaintext = plaintext.decode("utf-8")
     decoded_stores = json.loads(plaintext)
     return decoded_stores
 
 
-# Class containing Yahoo Finance ETL Functionality
 class YahooFinanceETL(object):
 
-    def __init__(self, ticker):
+    def __init__(self, ticker, **kwargs):
         self.ticker = ticker.upper() if isinstance(ticker, str) else [t.upper() for t in ticker]
+        self.country = kwargs.get("country", "US")
+        if self.country.upper() not in COUNTRY_MAP.keys():
+            raise ReferenceError("invalid country: " + self.country)
+        self.concurrent = kwargs.get("concurrent", False)
+        self.max_workers = kwargs.get("max_workers", 8)
+        self.timeout = kwargs.get("timeout", 30)
+        self.proxies = kwargs.get("proxies")
         self._cache = {}
 
     # Minimum interval between Yahoo Finance requests for this instance
     _MIN_INTERVAL = 7
 
     # Meta-data dictionaries for the classes to use
     YAHOO_FINANCIAL_TYPES = {
@@ -185,53 +180,78 @@
         utc = pytz.utc
         eastern = pytz.timezone('US/Eastern')
         date_ = datetime.datetime.strptime(date.replace(" 0:", " 12:"), mask)
         date_eastern = eastern.localize(date_, is_dst=None)
         date_utc = date_eastern.astimezone(utc)
         return date_utc.strftime('%Y-%m-%d %H:%M:%S %Z%z')
 
+    # _get_proxy randomly picks a proxy in the proxies list if not None
+    def _get_proxy(self):
+        if self.proxies:
+            proxy_str = self.proxies
+            if isinstance(self.proxies, list):
+                proxy_str = random.choice(self.proxies)
+            return {"https": proxy_str}
+        return None
+
+    # Private method that determines number of workers to use in a process
+    def _get_worker_count(self):
+        workers = self.max_workers
+        if len(self.ticker) < workers:
+            workers = len(self.ticker)
+        return workers
+
+    # Private method to execute a web scrape request and decrypt the return
+    def _request_handler(self, url):
+        urlopener = UrlOpener()
+        # Try to open the URL up to 10 times sleeping random time if something goes wrong
+        max_retry = 10
+        for i in range(0, max_retry):
+            response = urlopener.open(url, proxy=self._get_proxy(), timeout=self.timeout)
+            if response.status_code != 200:
+                time.sleep(random.randrange(10, 20))
+                response.close()
+            else:
+                soup = BeautifulSoup(response.content, "html.parser")
+                re_script = soup.find("script", string=re.compile("root.App.main")).text
+                if re_script is not None:
+                    re_data = loads(re.search("root.App.main\s+=\s+(\{.*\})", re_script).group(1))
+                    if "context" in re_data and "dispatcher" in re_data["context"]:
+                        data = re_data['context']['dispatcher']['stores']
+                        if "QuoteSummaryStore" not in data:
+                            data = decrypt_cryptojs_aes(re_data)
+                        try:
+                            if data.get("QuoteSummaryStore"):
+                                self._cache[url] = data
+                                break
+                        except AttributeError:
+                            time.sleep(random.randrange(10, 20))
+                            continue
+                else:
+                    time.sleep(random.randrange(10, 20))
+            if i == max_retry - 1:
+                # Raise a custom exception if we can't get the web page within max_retry attempts
+                raise ManagedException("Server replied with HTTP " + str(response.status_code) +
+                                       " code while opening the url: " + str(url))
+
     # Private method to scrape data from yahoo finance
     def _scrape_data(self, url, tech_type, statement_type):
         global _lastget
+        country_ent = COUNTRY_MAP.get(self.country.upper())
+        meta_str = '&lang=' + country_ent.get("lang", "en-US") + '&region=' + country_ent.get("region", "US")
+        url += meta_str
         if not self._cache.get(url):
             now = int(time.time())
             if _lastget and now - _lastget < self._MIN_INTERVAL:
                 time.sleep(self._MIN_INTERVAL - (now - _lastget) + 1)
                 now = int(time.time())
             _lastget = now
-            urlopener = UrlOpener()
-            # Try to open the URL up to 10 times sleeping random time if something goes wrong
-            max_retry = 10
-            for i in range(0, max_retry):
-                response = urlopener.open(url)
-                if response.getcode() != 200:
-                    time.sleep(random.randrange(10, 20))
-                else:
-                    response_content = response.read()
-                    soup = BeautifulSoup(response_content, "html.parser")
-                    re_script = soup.find("script", text=re.compile("root.App.main"))
-                    if re_script is not None:
-                        script = re_script.text
-                        # bs4 4.9.0 changed so text from scripts is no longer considered text
-                        if not script:
-                            script = re_script.string
-                        self._cache[url] = loads(re.search("root.App.main\s+=\s+(\{.*\})", script).group(1))
-                        response.close()
-                        break
-                    else:
-                        time.sleep(random.randrange(10, 20))
-                if i == max_retry - 1:
-                    # Raise a custom exception if we can't get the web page within max_retry attempts
-                    raise ManagedException("Server replied with HTTP " + str(response.getcode()) +
-                                           " code while opening the url: " + str(url))
+            self._request_handler(url)
         data = self._cache[url]
-        if "_cs" in data and "_cr" in data:
-            data = decrypt_cryptojs_aes(data)
         if "context" in data and "dispatcher" in data["context"]:
-            # Keep old code, just in case
             data = data['context']['dispatcher']['stores']
         if tech_type == '' and statement_type != 'history':
             stores = data["QuoteSummaryStore"]
         elif tech_type != '' and statement_type != 'history':
             stores = data["QuoteSummaryStore"][tech_type]
         else:
             stores = data["HistoricalPriceStore"]
@@ -245,32 +265,30 @@
         else:
             numerical_val = None
         return numerical_val
 
     # Private method to format date serial string to readable format and vice versa
     def _format_time(self, in_time):
         form_date_time = datetime.datetime.fromtimestamp(int(in_time)).strftime('%Y-%m-%d %H:%M:%S')
-        utc_dt = self._convert_to_utc(form_date_time)
-        return utc_dt
+        return self._convert_to_utc(form_date_time)
 
     # Private method to return a sub dictionary entry for the earning report cleaning
     def _get_cleaned_sub_dict_ent(self, key, val_list):
         sub_list = []
         for rec in val_list:
             sub_sub_dict = {}
             for k, v in rec.items():
                 if k == 'date':
                     sub_sub_dict_ent = {k: v}
                 else:
                     numerical_val = self._determine_numeric_value(v)
                     sub_sub_dict_ent = {k: numerical_val}
                 sub_sub_dict.update(sub_sub_dict_ent)
             sub_list.append(sub_sub_dict)
-        sub_ent = {key: sub_list}
-        return sub_ent
+        return {key: sub_list}
 
     # Private method to process raw earnings data and clean
     def _clean_earnings_data(self, raw_data):
         cleaned_data = {}
         earnings_key = 'earningsData'
         financials_key = 'financialsData'
         for k, v in raw_data.items():
@@ -371,32 +389,39 @@
                 dict_ent = {k: sub_dict_list}
             else:
                 dict_ent = {k: v}
             data.update(dict_ent)
         return data
 
     # Private Static Method to build API url for GET Request
-    @staticmethod
-    def _build_api_url(hist_obj, up_ticker):
-        base_url = "https://query1.finance.yahoo.com/v8/finance/chart/"
+    def _build_api_url(self, hist_obj, up_ticker, v="2", events=None):
+        if events is None:
+            events = [" div", "split", "earn"]
+        event_str = ''
+        for idx, s in enumerate(events, start=1):
+            if idx < len(events):
+                event_str += s + "|"
+            elif idx == len(events):
+                event_str += s
+        base_url = "https://query" + v + ".finance.yahoo.com/v8/finance/chart/"
         api_url = base_url + up_ticker + '?symbol=' + up_ticker + '&period1=' + str(hist_obj['start']) + '&period2=' + \
                   str(hist_obj['end']) + '&interval=' + hist_obj['interval']
-        api_url += '&events=div|split|earn&lang=en-US&region=US'
+        country_ent = COUNTRY_MAP.get(self.country.upper())
+        meta_str = '&lang=' + country_ent.get("lang", "en-US") + '&region=' + country_ent.get("region", "US")
+        api_url += '&events=' + event_str + meta_str
         return api_url
 
     # Private Method to get financial data via API Call
     def _get_api_data(self, api_url, tries=0):
         urlopener = UrlOpener()
-        response = urlopener.open(api_url)
-        if response.getcode() == 200:
-            res_content = response.read()
+        response = urlopener.open(api_url, proxy=self._get_proxy(), timeout=self.timeout)
+        if response.status_code == 200:
+            res_content = response.text
             response.close()
-            if sys.version_info < (3, 0):
-                return loads(res_content)
-            return loads(res_content.decode('utf-8'))
+            return loads(res_content)
         else:
             if tries < 5:
                 time.sleep(random.randrange(10, 20))
                 tries += 1
                 return self._get_api_data(api_url, tries)
             else:
                 return None
@@ -439,30 +464,36 @@
                 price_dict.update({'adjclose': adj_close_list[i]})
                 prices_list.append(price_dict)
                 i += 1
             ret_obj.update({'prices': prices_list})
         return ret_obj
 
     # Private Method to Handle Recursive API Request
-    def _recursive_api_request(self, hist_obj, up_ticker, i=0):
-        api_url = self._build_api_url(hist_obj, up_ticker)
-        re_data = self._clean_api_data(api_url)
-        cleaned_re_data = self._clean_historical_data(re_data)
-        if cleaned_re_data is not None:
-            return cleaned_re_data
-        else:
-            if i < 3:
-                i += 1
-                return self._recursive_api_request(hist_obj, up_ticker, i)
-            else:
-                return self._clean_historical_data(re_data, True)
+    def _recursive_api_request(self, hist_obj, up_ticker, clean=True, i=0):
+        v = "2"
+        if i == 3:  # After 3 tries querying against 'query2.finance.yahoo.com' try 'query1.finance.yahoo.com' instead
+            v = "1"
+        if clean:
+            re_data = self._clean_api_data(self._build_api_url(hist_obj, up_ticker, v))
+            cleaned_re_data = self._clean_historical_data(re_data)
+            if cleaned_re_data is not None:
+                return cleaned_re_data
+        else:
+            re_data = self._get_api_data(self._build_api_url(hist_obj, up_ticker, v))
+            if re_data is not None:
+                return re_data
+        if i < 6:
+            i += 1
+            return self._recursive_api_request(hist_obj, up_ticker, clean, i)
+        elif clean:
+            return self._clean_historical_data(re_data, True)
 
-    # Private Method to take scrapped data and build a data dictionary with
+    # Private Method to take scrapped data and build a data dictionary with, used by get_stock_data()
     def _create_dict_ent(self, up_ticker, statement_type, tech_type, report_name, hist_obj):
-        YAHOO_URL = self._BASE_YAHOO_URL + up_ticker + '/' + self.YAHOO_FINANCIAL_TYPES[statement_type][0] + '?p=' +\
+        YAHOO_URL = self._BASE_YAHOO_URL + up_ticker + '/' + self.YAHOO_FINANCIAL_TYPES[statement_type][0] + '?p=' + \
                     up_ticker
         if tech_type == '' and statement_type != 'history':
             try:
                 re_data = self._scrape_data(YAHOO_URL, tech_type, statement_type)
                 dict_ent = {up_ticker: re_data[u'' + report_name], 'dataType': report_name}
             except KeyError:
                 re_data = None
@@ -535,85 +566,105 @@
     # Public Method to get stock data
     def get_stock_data(self, statement_type='income', tech_type='', report_name='', hist_obj={}):
         data = {}
         if isinstance(self.ticker, str):
             dict_ent = self._create_dict_ent(self.ticker, statement_type, tech_type, report_name, hist_obj)
             data.update(dict_ent)
         else:
-            for tick in self.ticker:
-                try:
-                    dict_ent = self._create_dict_ent(tick, statement_type, tech_type, report_name, hist_obj)
-                    data.update(dict_ent)
-                except ManagedException:
-                    print("Warning! Ticker: " + str(tick) + " error - " + str(ManagedException))
-                    print("The process is still running...")
-                    continue
+            if self.concurrent:
+                with Pool(self._get_worker_count()) as pool:
+                    dict_ents = pool.map(partial(self._create_dict_ent,
+                                                 statement_type=statement_type,
+                                                 tech_type=tech_type,
+                                                 report_name=report_name,
+                                                 hist_obj=hist_obj), self.ticker)
+                    for dict_ent in dict_ents:
+                        data.update(dict_ent)
+            else:
+                for tick in self.ticker:
+                    try:
+                        dict_ent = self._create_dict_ent(tick, statement_type, tech_type, report_name, hist_obj)
+                        data.update(dict_ent)
+                    except ManagedException:
+                        logging.warning("yahoofinancials ticker: %s error getting %s - %s\n\tContinuing extraction...",
+                                        str(tick), statement_type, str(ManagedException))
+                        continue
         return data
 
     # Public Method to get technical stock data
     def get_stock_tech_data(self, tech_type):
         if tech_type == 'defaultKeyStatistics':
             return self.get_stock_data(statement_type='keystats', tech_type=tech_type)
         else:
             return self.get_stock_data(tech_type=tech_type)
 
     # Public Method to get reformatted statement data
     def get_reformatted_stmt_data(self, raw_data, statement_type):
-        data_dict = {}
-        sub_dict = {}
+        sub_dict, data_dict = {}, {}
         data_type = raw_data['dataType']
         if isinstance(self.ticker, str):
             sub_dict_ent = self._get_sub_dict_ent(self.ticker, raw_data, statement_type)
             sub_dict.update(sub_dict_ent)
             dict_ent = {data_type: sub_dict}
             data_dict.update(dict_ent)
         else:
-            for tick in self.ticker:
-                sub_dict_ent = self._get_sub_dict_ent(tick, raw_data, statement_type)
-                sub_dict.update(sub_dict_ent)
+            if self.concurrent:
+                with Pool(self._get_worker_count()) as pool:
+                    sub_dict_ents = pool.map(partial(self._get_sub_dict_ent,
+                                                     raw_data=raw_data,
+                                                     statement_type=statement_type), self.ticker)
+                    for dict_ent in sub_dict_ents:
+                        sub_dict.update(dict_ent)
+            else:
+                for tick in self.ticker:
+                    sub_dict_ent = self._get_sub_dict_ent(tick, raw_data, statement_type)
+                    sub_dict.update(sub_dict_ent)
             dict_ent = {data_type: sub_dict}
             data_dict.update(dict_ent)
         return data_dict
 
+    # Public method to get cleaned report data
+    def _clean_data_process(self, tick, report_type, raw_report_data):
+        if report_type == 'earnings':
+            try:
+                cleaned_data = self._clean_earnings_data(raw_report_data[tick])
+            except:
+                cleaned_data = None
+        else:
+            try:
+                cleaned_data = self._clean_reports(raw_report_data[tick])
+            except:
+                cleaned_data = None
+        return cleaned_data
+
     # Public method to get cleaned summary and price report data
     def get_clean_data(self, raw_report_data, report_type):
         cleaned_data_dict = {}
         if isinstance(self.ticker, str):
-            if report_type == 'earnings':
-                try:
-                    cleaned_data = self._clean_earnings_data(raw_report_data[self.ticker])
-                except:
-                    cleaned_data = None
-            else:
-                try:
-                    cleaned_data = self._clean_reports(raw_report_data[self.ticker])
-                except:
-                    cleaned_data = None
+            cleaned_data = self._clean_data_process(self.ticker, report_type, raw_report_data)
             cleaned_data_dict.update({self.ticker: cleaned_data})
         else:
-            for tick in self.ticker:
-                if report_type == 'earnings':
-                    try:
-                        cleaned_data = self._clean_earnings_data(raw_report_data[tick])
-                    except:
-                        cleaned_data = None
-                else:
-                    try:
-                        cleaned_data = self._clean_reports(raw_report_data[tick])
-                    except:
-                        cleaned_data = None
-                cleaned_data_dict.update({tick: cleaned_data})
+            if self.concurrent:
+                with Pool(self._get_worker_count()) as pool:
+                    cleaned_data_list = pool.map(partial(self._clean_data_process,
+                                                         report_type=report_type,
+                                                         raw_report_data=raw_report_data), self.ticker)
+                    for idx, cleaned_data in enumerate(cleaned_data_list):
+                        cleaned_data_dict.update({self.ticker[idx]: cleaned_data})
+            else:
+                for tick in self.ticker:
+                    cleaned_data = self._clean_data_process(tick, report_type, raw_report_data)
+                    cleaned_data_dict.update({tick: cleaned_data})
         return cleaned_data_dict
 
     # Private method to handle dividend data requests
     def _handle_api_dividend_request(self, cur_ticker, start, end, interval):
         re_dividends = []
-        test_url = 'https://query1.finance.yahoo.com/v8/finance/chart/' + cur_ticker + \
-                   '?period1=' + str(start) + '&period2=' + str(end) + '&interval=' + interval + '&events=div'
-        div_dict = self._get_api_data(test_url)['chart']['result'][0]['events']['dividends']
+        hist_obj = {"start": start, "end": end, "interval": interval}
+        div_dict = self._recursive_api_request(hist_obj, cur_ticker, False)['chart']['result'][0]['events']['dividends']
         for div_time_key, div_obj in div_dict.items():
             dividend_obj = {
                 'date': div_obj['date'],
                 'formatted_date': self.format_date(int(div_obj['date'])),
                 'amount': div_obj.get('amount', None)
             }
             re_dividends.append(dividend_obj)
@@ -625,331 +676,23 @@
         if isinstance(self.ticker, str):
             try:
                 return {self.ticker: self._handle_api_dividend_request(self.ticker, start, end, interval_code)}
             except:
                 return {self.ticker: None}
         else:
             re_data = {}
-            for tick in self.ticker:
-                try:
-                    div_data = self._handle_api_dividend_request(tick, start, end, interval_code)
-                    re_data.update({tick: div_data})
-                except:
-                    re_data.update({tick: None})
-            return re_data
-
-
-# Class containing methods to create stock data extracts
-class YahooFinancials(YahooFinanceETL):
-
-    # Private method that handles financial statement extraction
-    def _run_financial_stmt(self, statement_type, report_num, reformat):
-        report_name = self.YAHOO_FINANCIAL_TYPES[statement_type][report_num]
-        if reformat:
-            raw_data = self.get_stock_data(statement_type, report_name=report_name)
-            data = self.get_reformatted_stmt_data(raw_data, statement_type)
-        else:
-            data = self.get_stock_data(statement_type, report_name=report_name)
-        return data
-
-    # Public Method for the user to get financial statement data
-    def get_financial_stmts(self, frequency, statement_type, reformat=True):
-        report_num = self.get_report_type(frequency)
-        if isinstance(statement_type, str):
-            data = self._run_financial_stmt(statement_type, report_num, reformat)
-        else:
-            data = {}
-            for stmt_type in statement_type:
-                re_data = self._run_financial_stmt(stmt_type, report_num, reformat)
-                data.update(re_data)
-        return data
-
-    # Public Method for the user to get stock price data
-    def get_stock_price_data(self, reformat=True):
-        if reformat:
-            return self.get_clean_data(self.get_stock_tech_data('price'), 'price')
-        else:
-            return self.get_stock_tech_data('price')
-
-    # Public Method for the user to return key-statistics data
-    def get_key_statistics_data(self, reformat=True):
-        if reformat:
-            return self.get_clean_data(self.get_stock_tech_data('defaultKeyStatistics'), 'defaultKeyStatistics')
-        else:
-            return self.get_stock_tech_data('defaultKeyStatistics')
-
-    # Public Method for the user to get stock earnings data
-    def get_stock_earnings_data(self, reformat=True):
-        if reformat:
-            return self.get_clean_data(self.get_stock_tech_data('earnings'), 'earnings')
-        else:
-            return self.get_stock_tech_data('earnings')
-
-    # Public Method for the user to get stock summary data
-    def get_summary_data(self, reformat=True):
-        if reformat:
-            return self.get_clean_data(self.get_stock_tech_data('summaryDetail'), 'summaryDetail')
-        else:
-            return self.get_stock_tech_data('summaryDetail')
-
-    # Public Method for the user to get the yahoo summary url
-    def get_stock_summary_url(self):
-        if isinstance(self.ticker, str):
-            return self._BASE_YAHOO_URL + self.ticker
-        return {t: self._BASE_YAHOO_URL + t for t in self.ticker}
-
-    # Public Method for the user to get stock quote data
-    def get_stock_quote_type_data(self):
-        return self.get_stock_tech_data('quoteType')
-
-    # Public Method for user to get historical price data with
-    def get_historical_price_data(self, start_date, end_date, time_interval):
-        interval_code = self.get_time_code(time_interval)
-        start = self.format_date(start_date)
-        end = self.format_date(end_date)
-        hist_obj = {'start': start, 'end': end, 'interval': interval_code}
-        return self.get_stock_data('history', hist_obj=hist_obj)
-
-    # Private Method for Functions needing stock_price_data
-    def _stock_price_data(self, data_field):
-        if isinstance(self.ticker, str):
-            if self.get_stock_price_data()[self.ticker] is None:
-                return None
-            return self.get_stock_price_data()[self.ticker].get(data_field, None)
-        else:
-            ret_obj = {}
-            for tick in self.ticker:
-                if self.get_stock_price_data()[tick] is None:
-                    ret_obj.update({tick: None})
-                else:
-                    ret_obj.update({tick: self.get_stock_price_data()[tick].get(data_field, None)})
-            return ret_obj
-
-    # Private Method for Functions needing stock_price_data
-    def _stock_summary_data(self, data_field):
-        if isinstance(self.ticker, str):
-            if self.get_summary_data()[self.ticker] is None:
-                return None
-            return self.get_summary_data()[self.ticker].get(data_field, None)
-        else:
-            ret_obj = {}
-            for tick in self.ticker:
-                if self.get_summary_data()[tick] is None:
-                    ret_obj.update({tick: None})
-                else:
-                    ret_obj.update({tick: self.get_summary_data()[tick].get(data_field, None)})
-            return ret_obj
-
-    # Private Method for Functions needing financial statement data
-    def _financial_statement_data(self, stmt_type, stmt_code, field_name, freq):
-        re_data = self.get_financial_stmts(freq, stmt_type)[stmt_code]
-        if isinstance(self.ticker, str):
-            try:
-                date_key = re_data[self.ticker][0].keys()[0]
-            except (IndexError, AttributeError, TypeError):
-                date_key = list(re_data[self.ticker][0])[0]
-            data = re_data[self.ticker][0][date_key][field_name]
-        else:
-            data = {}
-            for tick in self.ticker:
-                try:
-                    date_key = re_data[tick][0].keys()[0]
-                except:
+            if self.concurrent:
+                with Pool(self._get_worker_count()) as pool:
+                    div_data_list = pool.map(partial(self._handle_api_dividend_request,
+                                                     start=start,
+                                                     end=end,
+                                                     interval=interval_code), self.ticker)
+                    for idx, div_data in enumerate(div_data_list):
+                        re_data.update({self.ticker[idx]: div_data})
+            else:
+                for tick in self.ticker:
                     try:
-                        date_key = list(re_data[tick][0].keys())[0]
+                        div_data = self._handle_api_dividend_request(tick, start, end, interval_code)
+                        re_data.update({tick: div_data})
                     except:
-                        date_key = None
-                if date_key is not None:
-                    sub_data = re_data[tick][0][date_key][field_name]
-                    data.update({tick: sub_data})
-                else:
-                    data.update({tick: None})
-        return data
-
-    # Public method to get daily dividend data
-    def get_daily_dividend_data(self, start_date, end_date):
-        start = self.format_date(start_date)
-        end = self.format_date(end_date)
-        return self.get_stock_dividend_data(start, end, 'daily')
-
-    # Public Price Data Methods
-    def get_current_price(self):
-        return self._stock_price_data('regularMarketPrice')
-
-    def get_current_change(self):
-        return self._stock_price_data('regularMarketChange')
-
-    def get_current_percent_change(self):
-        return self._stock_price_data('regularMarketChangePercent')
-
-    def get_current_volume(self):
-        return self._stock_price_data('regularMarketVolume')
-
-    def get_prev_close_price(self):
-        return self._stock_price_data('regularMarketPreviousClose')
-
-    def get_open_price(self):
-        return self._stock_price_data('regularMarketOpen')
-
-    def get_ten_day_avg_daily_volume(self):
-        return self._stock_price_data('averageDailyVolume10Day')
-
-    def get_three_month_avg_daily_volume(self):
-        return self._stock_price_data('averageDailyVolume3Month')
-
-    def get_stock_exchange(self):
-        return self._stock_price_data('exchangeName')
-
-    def get_market_cap(self):
-        return self._stock_price_data('marketCap')
-
-    def get_daily_low(self):
-        return self._stock_price_data('regularMarketDayLow')
-
-    def get_daily_high(self):
-        return self._stock_price_data('regularMarketDayHigh')
-
-    def get_currency(self):
-        return self._stock_price_data('currency')
-
-    # Public Summary Data Methods
-    def get_yearly_high(self):
-        return self._stock_summary_data('fiftyTwoWeekHigh')
-
-    def get_yearly_low(self):
-        return self._stock_summary_data('fiftyTwoWeekLow')
-
-    def get_dividend_yield(self):
-        return self._stock_summary_data('dividendYield')
-
-    def get_annual_avg_div_yield(self):
-        return self._stock_summary_data('trailingAnnualDividendYield')
-
-    def get_five_yr_avg_div_yield(self):
-        return self._stock_summary_data('fiveYearAvgDividendYield')
-
-    def get_dividend_rate(self):
-        return self._stock_summary_data('dividendRate')
-
-    def get_annual_avg_div_rate(self):
-        return self._stock_summary_data('trailingAnnualDividendRate')
-
-    def get_50day_moving_avg(self):
-        return self._stock_summary_data('fiftyDayAverage')
-
-    def get_200day_moving_avg(self):
-        return self._stock_summary_data('twoHundredDayAverage')
-
-    def get_beta(self):
-        return self._stock_summary_data('beta')
-
-    def get_payout_ratio(self):
-        return self._stock_summary_data('payoutRatio')
-
-    def get_pe_ratio(self):
-        return self._stock_summary_data('trailingPE')
-
-    def get_price_to_sales(self):
-        return self._stock_summary_data('priceToSalesTrailing12Months')
-
-    def get_exdividend_date(self):
-        return self._stock_summary_data('exDividendDate')
-
-    # Financial Statement Data Methods
-    def get_book_value(self):
-        return self._financial_statement_data('balance', 'balanceSheetHistoryQuarterly',
-                                              'totalStockholderEquity', 'quarterly')
-
-    def get_ebit(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'ebit', 'annual')
-
-    def get_net_income(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'netIncome', 'annual')
-
-    def get_interest_expense(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'interestExpense', 'annual')
-
-    def get_operating_income(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'operatingIncome', 'annual')
-
-    def get_total_operating_expense(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'totalOperatingExpenses', 'annual')
-
-    def get_total_revenue(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'totalRevenue', 'annual')
-
-    def get_cost_of_revenue(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'costOfRevenue', 'annual')
-
-    def get_income_before_tax(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'incomeBeforeTax', 'annual')
-
-    def get_income_tax_expense(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'incomeTaxExpense', 'annual')
-
-    def get_gross_profit(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'grossProfit', 'annual')
-
-    def get_net_income_from_continuing_ops(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory',
-                                              'netIncomeFromContinuingOps', 'annual')
-
-    def get_research_and_development(self):
-        return self._financial_statement_data('income', 'incomeStatementHistory', 'researchDevelopment', 'annual')
-
-    # Calculated Financial Methods
-    def get_earnings_per_share(self):
-        price_data = self.get_current_price()
-        pe_ratio = self.get_pe_ratio()
-        if isinstance(self.ticker, str):
-            if price_data is not None and pe_ratio is not None:
-                return price_data / pe_ratio
-            else:
-                return None
-        else:
-            ret_obj = {}
-            for tick in self.ticker:
-                if price_data[tick] is not None and pe_ratio[tick] is not None:
-                    ret_obj.update({tick: price_data[tick] / pe_ratio[tick]})
-                else:
-                    ret_obj.update({tick: None})
-            return ret_obj
-
-    def get_num_shares_outstanding(self, price_type='current'):
-        today_low = self._stock_summary_data('dayHigh')
-        today_high = self._stock_summary_data('dayLow')
-        cur_market_cap = self._stock_summary_data('marketCap')
-        if isinstance(self.ticker, str):
-            if cur_market_cap is not None:
-                if price_type == 'current':
-                    current = self.get_current_price()
-                    if current is not None:
-                        today_average = current
-                    else:
-                        return None
-                else:
-                    if today_high is not None and today_low is not None:
-                        today_average = (today_high + today_low) / 2
-                    else:
-                        return None
-                return cur_market_cap / today_average
-            else:
-                return None
-        else:
-            ret_obj = {}
-            for tick in self.ticker:
-                if cur_market_cap[tick] is not None:
-                    if price_type == 'current':
-                        current = self.get_current_price()
-                        if current[tick] is not None:
-                            ret_obj.update({tick: cur_market_cap[tick] / current[tick]})
-                        else:
-                            ret_obj.update({tick: None})
-                    else:
-                        if today_low[tick] is not None and today_high[tick] is not None:
-                            today_average = (today_high[tick] + today_low[tick]) / 2
-                            ret_obj.update({tick: cur_market_cap[tick] / today_average})
-                        else:
-                            ret_obj.update({tick: None})
-                else:
-                    ret_obj.update({tick: None})
-            return ret_obj
+                        re_data.update({tick: None})
+            return re_data
```

### Comparing `yahoofinancials-1.8/setup.py` & `yahoofinancials-1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,38 +6,41 @@
 
 
 with codecs.open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='yahoofinancials',
-    version='1.8',
+    version='1.9',
     description='A powerful financial data module used for pulling both fundamental and technical data from Yahoo Finance',
     long_description=long_description,
     url='https://github.com/JECSand/yahoofinancials',
-    download_url='https://github.com/JECSand/yahoofinancials/archive/1.8.tar.gz',
+    download_url='https://github.com/JECSand/yahoofinancials/archive/1.9.tar.gz',
     author='Connor Sanders',
     author_email='connor@exceleri.com',
     license='MIT',
     keywords=['finance data', 'stocks', 'commodities', 'cryptocurrencies', 'currencies', 'forex', 'yahoo finance'],
     packages=['yahoofinancials'],
     install_requires=[
         "beautifulsoup4>=4.11.1",
         "pytz",
-        "cryptography>=3.3.2"
+        "cryptography>=3.3.2",
+        # "pycryptodome>=3.6.6"
+        "requests>=2.26",
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Financial and Insurance Industry',
         'Topic :: Office/Business :: Financial :: Investment',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     zip_safe=False
 )
```

### Comparing `yahoofinancials-1.8/README.rst` & `yahoofinancials-1.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,48 @@
 ===============
 
 A python module that returns stock, cryptocurrency, forex, mutual fund, commodity futures, ETF, and US Treasury financial data from Yahoo Finance.
 
 .. image:: https://github.com/JECSand/yahoofinancials/actions/workflows/test.yml/badge.svg?branch=master
     :target: https://github.com/JECSand/yahoofinancials/actions/workflows/test.yml
 
-Current Version: v1.8
+Current Version: v1.9
 
-Version Released: 01/09/2023
+Version Released: 01/14/2023
 
 Report any bugs by opening an issue here: https://github.com/JECSand/yahoofinancials/issues
 
 Overview
 --------
 A powerful financial data module used for pulling both fundamental and technical data from Yahoo Finance.
 
-- As of Version 0.10, Yahoo Financials now returns historical pricing data for commodity futures, cryptocurrencies, ETFs, mutual funds, U.S. Treasuries, currencies, indexes, and stocks.
+- As of Version 1.9, YahooFinancials supports optional parameters for asynchronous execution, proxies, and international requests.
+
+.. code-block:: python
+
+    from yahoofinancials import YahooFinancials
+    tickers = ['AAPL', 'GOOG', 'C']
+    yahoo_financials = YahooFinancials(tickers, concurrent=True, max_workers=8, country="US")
+    balance_sheet_data_qt = yahoo_financials.get_financial_stmts('quarterly', 'balance')
+    print(balance_sheet_data_qt)
+
+    proxy_addresses = [ "mysuperproxy.com:5000", "mysuperproxy.com:5001"]
+    yahoo_financials = YahooFinancials(tickers, concurrent=True, proxies=proxy_addresses)
+    balance_sheet_data_qt = yahoo_financials.get_financial_stmts('quarterly', 'balance')
+    print(balance_sheet_data_qt)
+
+- New methods in Version 1.9:
+    - get_stock_profile_data()
+    - get_financial_data()
+
 
 Installation
 -------------
-- yahoofinancials runs on Python 3.6, 3.7, 3.8, 3.9, and 3.10.
-- This package depends on beautifulsoup4, pytz, and cryptography to work.
+- yahoofinancials runs on Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11.
+- This package depends on beautifulsoup4, pytz, requests, and cryptography to work.
 
 1. Installation using pip:
 
 - Linux/Mac:
 
 .. code-block:: bash
 
@@ -62,15 +80,15 @@
     $ cd yahoofinancials
     $ python test/test_yahoofinancials.py
 
 Module Methods
 --------------
 - The financial data from all methods is returned as JSON.
 - You can run multiple symbols at once using an inputted array or run an individual symbol using an inputted string.
-- YahooFinancials works with Python 3.6, 3.7, 3.8, 3.9, and 3.10 and runs on all operating systems. (Windows, Mac, Linux).
+- YahooFinancials works with Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11 and runs on all operating systems. (Windows, Mac, Linux).
 
 Featured Methods
 ^^^^^^^^^^^^^^^^
 1. get_financial_stmts(frequency, statement_type, reformat=True)
 
    - frequency can be either 'annual' or 'quarterly'.
    - statement_type can be 'income', 'balance', 'cash' or a list of several.
@@ -142,14 +160,16 @@
 - get_price_to_sales()
 - get_exdividend_date()
 - get_book_value()
 - get_ebit()
 - get_net_income()
 - get_earnings_per_share()
 - get_key_statistics_data()
+- get_stock_profile_data()
+- get_financial_data()
 
 Usage Examples
 --------------
 - The class constructor can take either a single ticker or a list of tickers as it's parameter.
 - This makes it easy to initiate multiple classes for different groupings of financial assets.
 - Quarterly statement data returns the last 4 periods of data, while annual returns the last 3.
 
@@ -745,7 +765,52 @@
                 "date": 586445400,
                 "formatted_date": "1988-08-01",
                 "amount": 0.3344
             }
         ]
     }
 
+13. Apple key Financial Data:
+
+
+.. code-block:: python
+
+    yahoo_financials = YahooFinancials("AAPL")
+    print(yahoo_financials.get_financial_data())
+
+
+.. code-block:: javascript
+
+    {
+        'AAPL': {
+            'ebitdaMargins': 0.29395,
+            'profitMargins': 0.21238,
+            'grossMargins': 0.37818,
+            'operatingCashflow': 69390999552,
+            'revenueGrowth': 0.018,
+            'operatingMargins': 0.24572,
+            'ebitda': 76476997632,
+            'targetLowPrice': 150,
+            'recommendationKey': 'buy',
+            'grossProfits': 98392000000,
+            'freeCashflow': 42914250752,
+            'targetMedianPrice': 270,
+            'currentPrice': 261.78,
+            'earningsGrowth': 0.039,
+            'currentRatio': 1.54,
+            'returnOnAssets': 0.11347,
+            'numberOfAnalystOpinions': 40,
+            'targetMeanPrice': 255.51,
+            'debtToEquity': 119.405,
+            'returnOnEquity': 0.55917,
+            'targetHighPrice': 300,
+            'totalCash': 100556996608,
+            'totalDebt': 108046999552,
+            'totalRevenue': 260174004224,
+            'totalCashPerShare': 22.631,
+            'financialCurrency': 'USD',
+            'maxAge': 86400,
+            'revenuePerShare': 56.341,
+            'quickRatio': 1.384,
+            'recommendationMean': 2.2
+        }
+    }
```

### Comparing `yahoofinancials-1.8/test/test_yahoofinancials.py` & `yahoofinancials-1.9/test/test_yahoofinancials.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-# YahooFinancials Unit Tests v1.7
-# Version Released: 01/01/2023
+# YahooFinancials Unit Tests v1.9
+# Version Released: 01/14/2023
 # Author: Connor Sanders
-# Tested on Python 3.6, 3.7, 3.8, 3.9, and 3.10
+# Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10, and 3.11
 # Copyright (c) 2023 Connor Sanders
 # MIT License
 
-import sys
-from yahoofinancials import YahooFinancials
-
-if sys.version_info < (2, 7):
-    from unittest2 import main as test_main, SkipTest, TestCase
-else:
-    from unittest import main as test_main, SkipTest, TestCase
+from unittest import main as test_main, TestCase
 
+from yahoofinancials import YahooFinancials
 
 # Test Configuration Variables
 stocks = ['AAPL', 'MSFT', 'C', 'IL&FSTRANS.NS']
 currencies = ['EURUSD=X', 'JPY=X', 'GBPUSD=X']
 us_treasuries = ['^TNX', '^IRX', '^TYX']
 
 
@@ -25,35 +20,36 @@
     if test_type == 'bal':
         if 'balanceSheetHistoryQuarterly' in test_data and test_data['balanceSheetHistoryQuarterly']['C'] is not None:
             return True
         else:
             return False
     elif test_type == 'inc':
         if 'incomeStatementHistoryQuarterly' in test_data and \
-                        test_data['incomeStatementHistoryQuarterly']['C'] is not None:
+                test_data['incomeStatementHistoryQuarterly']['C'] is not None:
             return True
         else:
             return False
     elif test_type == 'all':
         if 'balanceSheetHistoryQuarterly' in test_data and 'incomeStatementHistoryQuarterly' in test_data and \
-                        'cashflowStatementHistoryQuarterly' in test_data:
+                'cashflowStatementHistoryQuarterly' in test_data:
             return True
         else:
             return False
 
 
 # Main Test Module Class
 class TestModule(TestCase):
 
     def setUp(self):
         self.test_yf_stock_single = YahooFinancials('C')
         self.test_yf_stock_multi = YahooFinancials(stocks)
         self.test_yf_treasuries_single = YahooFinancials('^IRX')
         self.test_yf_treasuries_multi = YahooFinancials(us_treasuries)
         self.test_yf_currencies = YahooFinancials(currencies)
+        self.test_yf_concurrent = YahooFinancials(stocks, concurrent=True)
 
     # Fundamentals Test
     def test_yf_fundamentals(self):
         # Single stock test
         single_balance_sheet_data_qt = self.test_yf_stock_single.get_financial_stmts('quarterly', 'balance')
         single_income_statement_data_qt = self.test_yf_stock_single.get_financial_stmts('quarterly', 'income')
         single_all_statement_data_qt = self.test_yf_stock_single.get_financial_stmts('quarterly',
@@ -110,10 +106,25 @@
             self.assertEqual(False, True)
         # Treasuries
         if isinstance(self.test_yf_treasuries_single.get_current_price(), float):
             self.assertEqual(True, True)
         else:
             self.assertEqual(False, True)
 
+    # Test concurrent functionality of module
+    def test_yf_concurrency(self):
+        # Multi stock test
+        multi_balance_sheet_data_qt = self.test_yf_concurrent.get_financial_stmts('quarterly', 'balance')
+        multi_income_statement_data_qt = self.test_yf_concurrent.get_financial_stmts('quarterly', 'income')
+        multi_all_statement_data_qt = self.test_yf_concurrent.get_financial_stmts('quarterly',
+                                                                                  ['income', 'cash', 'balance'])
+        # Multi stock check
+        result = check_fundamental(multi_balance_sheet_data_qt, 'bal')
+        self.assertEqual(result, True)
+        result = check_fundamental(multi_income_statement_data_qt, 'inc')
+        self.assertEqual(result, True)
+        result = check_fundamental(multi_all_statement_data_qt, 'all')
+        self.assertEqual(result, True)
+
 
 if __name__ == "__main__":
     test_main()
```

