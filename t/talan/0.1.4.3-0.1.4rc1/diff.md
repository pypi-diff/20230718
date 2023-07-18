# Comparing `tmp/talan-0.1.4.3.tar.gz` & `tmp/talan-0.1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talan-0.1.4.3.tar", last modified: Tue Jul 18 16:12:34 2023, max compression
+gzip compressed data, was "talan-0.1.4rc1.tar", last modified: Tue Oct 18 15:47:35 2022, max compression
```

## Comparing `talan-0.1.4.3.tar` & `talan-0.1.4rc1.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-18 16:12:34.227096 talan-0.1.4.3/
--rw-r--r--   0 rstudio   (1001) users      (100)      688 2023-07-18 16:12:34.227096 talan-0.1.4.3/PKG-INFO
--rw-r--r--   0 rstudio   (1001) users      (100)      314 2021-10-14 21:05:42.000000 talan-0.1.4.3/README.md
--rw-r--r--   0 rstudio   (1001) users      (100)       38 2023-07-18 16:12:34.227096 talan-0.1.4.3/setup.cfg
--rw-r--r--   0 rstudio   (1001) users      (100)      975 2023-07-18 16:09:49.000000 talan-0.1.4.3/setup.py
-drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-18 16:12:34.223096 talan-0.1.4.3/talan/
--rwxr-xr-x   0 rstudio   (1001) users      (100)      240 2023-07-05 19:22:10.000000 talan-0.1.4.3/talan/__init__.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    39966 2023-07-04 04:09:16.000000 talan-0.1.4.3/talan/_alan_calc.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    13742 2023-07-03 20:21:58.000000 talan-0.1.4.3/talan/_alan_date.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    14990 2022-05-09 20:38:57.000000 talan-0.1.4.3/talan/_alan_mp4.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    11723 2022-11-22 22:19:42.000000 talan-0.1.4.3/talan/_alan_ohlc_fcs.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     4265 2019-08-01 04:14:12.000000 talan-0.1.4.3/talan/_alan_optparse.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    14976 2021-10-29 01:15:39.000000 talan-0.1.4.3/talan/_alan_pppscf.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    29498 2023-01-23 14:30:39.000000 talan-0.1.4.3/talan/_alan_rmc.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    65801 2023-07-04 02:53:11.000000 talan-0.1.4.3/talan/_alan_str.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    47116 2023-02-09 16:29:37.000000 talan-0.1.4.3/talan/alanapi.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     7501 2023-02-16 02:31:23.000000 talan-0.1.4.3/talan/chatgptAPI.py
--rw-r--r--   0 rstudio   (1001) users      (100)    31949 2022-12-30 20:32:22.000000 talan-0.1.4.3/talan/csv2plotj2ts.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     7100 2021-09-19 20:39:01.000000 talan-0.1.4.3/talan/find_recent_eps.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     3518 2022-10-12 19:28:21.000000 talan-0.1.4.3/talan/fredReader.py
--rw-r--r--   0 rstudio   (1001) users      (100)     2130 2023-07-16 20:30:46.000000 talan-0.1.4.3/talan/get_rq.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6262 2023-01-31 19:25:24.000000 talan-0.1.4.3/talan/headline_calc.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     9876 2020-05-08 19:29:00.000000 talan-0.1.4.3/talan/headline_sts.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6261 2020-05-19 00:26:02.000000 talan-0.1.4.3/talan/iex_peers.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    34234 2022-03-30 17:55:59.000000 talan-0.1.4.3/talan/lsi_daily.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     9822 2021-09-29 19:06:55.000000 talan-0.1.4.3/talan/macro_event_yh.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    41692 2022-12-23 21:01:13.000000 talan-0.1.4.3/talan/plot_templates.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     7703 2023-07-04 20:28:27.000000 talan-0.1.4.3/talan/prc_temp_DN.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    11503 2023-01-31 19:15:38.000000 talan-0.1.4.3/talan/record_hilo.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     1027 2023-07-18 15:56:52.000000 talan-0.1.4.3/talan/talan_wrap.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    14131 2023-01-06 22:09:49.000000 talan-0.1.4.3/talan/theme_list.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6113 2023-02-02 21:45:43.000000 talan-0.1.4.3/talan/ticker2label.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6613 2022-11-07 00:19:24.000000 talan-0.1.4.3/talan/ticker_mapping.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     4825 2021-10-11 19:44:03.000000 talan-0.1.4.3/talan/upd_mapping_ticker.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     8716 2023-07-05 03:31:50.000000 talan-0.1.4.3/talan/webReader.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    42404 2023-07-04 04:49:24.000000 talan-0.1.4.3/talan/yh_chart.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    15454 2022-11-14 21:58:33.000000 talan-0.1.4.3/talan/yh_hist_batch.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     5521 2023-01-31 21:38:37.000000 talan-0.1.4.3/talan/yh_predefined.py
-drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-18 16:12:34.227096 talan-0.1.4.3/talan.egg-info/
--rw-r--r--   0 rstudio   (1001) users      (100)      688 2023-07-18 16:12:34.000000 talan-0.1.4.3/talan.egg-info/PKG-INFO
--rw-r--r--   0 rstudio   (1001) users      (100)      837 2023-07-18 16:12:34.000000 talan-0.1.4.3/talan.egg-info/SOURCES.txt
--rw-r--r--   0 rstudio   (1001) users      (100)        1 2023-07-18 16:12:34.000000 talan-0.1.4.3/talan.egg-info/dependency_links.txt
--rw-r--r--   0 rstudio   (1001) users      (100)       38 2023-07-18 16:12:34.000000 talan-0.1.4.3/talan.egg-info/requires.txt
--rw-r--r--   0 rstudio   (1001) users      (100)        6 2023-07-18 16:12:34.000000 talan-0.1.4.3/talan.egg-info/top_level.txt
+drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2022-10-18 15:47:35.301034 talan-0.1.4rc1/
+-rw-r--r--   0 rstudio   (1001) users      (100)      689 2022-10-18 15:47:35.301034 talan-0.1.4rc1/PKG-INFO
+-rw-r--r--   0 rstudio   (1001) users      (100)      314 2021-10-14 21:05:42.000000 talan-0.1.4rc1/README.md
+-rw-r--r--   0 rstudio   (1001) users      (100)       38 2022-10-18 15:47:35.301034 talan-0.1.4rc1/setup.cfg
+-rw-r--r--   0 rstudio   (1001) users      (100)      977 2022-10-18 15:47:11.000000 talan-0.1.4rc1/setup.py
+drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2022-10-18 15:47:35.297034 talan-0.1.4rc1/talan/
+-rw-r--r--   0 rstudio   (1001) users      (100)      238 2022-10-12 20:09:03.000000 talan-0.1.4rc1/talan/__init__.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    39916 2022-10-10 01:17:35.000000 talan-0.1.4rc1/talan/_alan_calc.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    13070 2022-08-17 17:29:02.000000 talan-0.1.4rc1/talan/_alan_date.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    14990 2022-05-09 20:38:57.000000 talan-0.1.4rc1/talan/_alan_mp4.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    11619 2022-03-30 15:57:05.000000 talan-0.1.4rc1/talan/_alan_ohlc_fcs.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     4265 2019-08-01 04:14:12.000000 talan-0.1.4rc1/talan/_alan_optparse.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    14976 2021-10-29 01:15:39.000000 talan-0.1.4rc1/talan/_alan_pppscf.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    28436 2022-08-19 18:20:19.000000 talan-0.1.4rc1/talan/_alan_rmc.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    64824 2022-09-16 15:56:48.000000 talan-0.1.4rc1/talan/_alan_str.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    46272 2022-09-03 17:19:27.000000 talan-0.1.4rc1/talan/alanapi.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    30625 2022-09-12 18:35:55.000000 talan-0.1.4rc1/talan/csv2plotj2ts.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     7100 2021-09-19 20:39:01.000000 talan-0.1.4rc1/talan/find_recent_eps.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     3518 2022-10-12 19:28:21.000000 talan-0.1.4rc1/talan/fredReader.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6247 2021-07-31 01:13:30.000000 talan-0.1.4rc1/talan/headline_calc.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     9876 2020-05-08 19:29:00.000000 talan-0.1.4rc1/talan/headline_sts.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6261 2020-05-19 00:26:02.000000 talan-0.1.4rc1/talan/iex_peers.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    34234 2022-03-30 17:55:59.000000 talan-0.1.4rc1/talan/lsi_daily.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     9822 2021-09-29 19:06:55.000000 talan-0.1.4rc1/talan/macro_event_yh.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    40055 2022-06-07 20:46:02.000000 talan-0.1.4rc1/talan/plot_templates.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     5752 2021-10-11 19:14:52.000000 talan-0.1.4rc1/talan/prc_temp_DN.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    11228 2020-10-09 14:50:59.000000 talan-0.1.4rc1/talan/record_hilo.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     1027 2022-10-12 19:27:48.000000 talan-0.1.4rc1/talan/talan_wrap.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    14131 2020-07-30 21:48:04.000000 talan-0.1.4rc1/talan/theme_list.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6123 2021-10-07 16:16:03.000000 talan-0.1.4rc1/talan/ticker2label.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6552 2021-10-07 03:41:34.000000 talan-0.1.4rc1/talan/ticker_mapping.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     4825 2021-10-11 19:44:03.000000 talan-0.1.4rc1/talan/upd_mapping_ticker.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6614 2022-10-12 21:00:27.000000 talan-0.1.4rc1/talan/webReader.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    37434 2022-08-10 16:51:40.000000 talan-0.1.4rc1/talan/yh_chart.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    15404 2022-06-03 18:37:28.000000 talan-0.1.4rc1/talan/yh_hist_batch.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     5046 2020-10-29 15:32:34.000000 talan-0.1.4rc1/talan/yh_predefined.py
+drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2022-10-18 15:47:35.301034 talan-0.1.4rc1/talan.egg-info/
+-rw-r--r--   0 rstudio   (1001) users      (100)      689 2022-10-18 15:47:35.000000 talan-0.1.4rc1/talan.egg-info/PKG-INFO
+-rw-r--r--   0 rstudio   (1001) users      (100)      801 2022-10-18 15:47:35.000000 talan-0.1.4rc1/talan.egg-info/SOURCES.txt
+-rw-r--r--   0 rstudio   (1001) users      (100)        1 2022-10-18 15:47:35.000000 talan-0.1.4rc1/talan.egg-info/dependency_links.txt
+-rw-r--r--   0 rstudio   (1001) users      (100)       38 2022-10-18 15:47:35.000000 talan-0.1.4rc1/talan.egg-info/requires.txt
+-rw-r--r--   0 rstudio   (1001) users      (100)        6 2022-10-18 15:47:35.000000 talan-0.1.4rc1/talan.egg-info/top_level.txt
```

### Comparing `talan-0.1.4.3/PKG-INFO` & `talan-0.1.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talan
-Version: 0.1.4.3
+Version: 0.1.4rc1
 Summary: ('Technical ALgorithmic ANalytics',)
 Home-page: https://github.com/beyondbond/talan
 Author: Ted Hong
 Author-email: ted@beyondbond.com
 License: BSD 2-clause
 Description: Utility funcitions for financial analysis
 Platform: UNKNOWN
```

### Comparing `talan-0.1.4.3/setup.py` & `talan-0.1.4rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup,find_packages
-VERSION = '0.1.4.3' 
+VERSION = '0.1.4-rc1' 
 DESCRIPTION = 'Technical ALgorithmic ANalytics',
 LONG_DESCRIPTION = 'Utility funcitions for financial analysis'
 
 # Setting up
 setup(
     name='talan',
     version=VERSION,
```

### Comparing `talan-0.1.4.3/talan/_alan_calc.py` & `talan-0.1.4rc1/talan/_alan_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,27 @@
 def lmap2(f, itr): return [f(x) for x in list(itr)]
 #OR similar run-time efficiency
 lmap = lambda f, itr: list(map(f, itr))
 
 def saferun(func):
 	'''
 	Decorator for try_except to wrap func(...) 
-	`errmsg` default as "" or used-defined
+	Error return is an empty string ""
+
 	Usage of,
 	@saferun 
 	def func(...):
-	or
-	@saferun 
-	def func(...,errmsg=None):
 	----------------------------------------------------------------------
 	'''
 	def wrapped_f(*args, **kwargs):
 		ret=""
 		try:
 			return func(*args, **kwargs)
 		except Exception as e:
-			ret=kwargs.pop('errmsg',ret)
-			sys.stderr.write("**ERROR: {} @ {}\n".format(str(e),func.__name__))
+			sys.stderr.write("**ERROR: {},\nreturn {}\n".format(str(e),ret))
 			return ret
 	wrapped_f.__name__=func.__name__
 	wrapped_f.__doc__=func.__doc__
 	return wrapped_f
 
 class safeRunArg(object):
 	'''
@@ -80,15 +77,15 @@
 		it a single argument, which is the function object.
 		"""
 		#dispatcher = singledispatch(func)
 		def wrapped_f(*args, **kwargs):
 			try:
 				return func(*args, **kwargs)
 			except Exception as e:
-				errMsg="**ERROR: {} @ {}\n{}".format(str(e),func.__name__,self.arg1)
+				errMsg="**ERROR: {}\n{}".format(str(e),self.arg1)
 				sys.stderr.write(errMsg+"\n")
 				return self.arg1
 		#wrapped_f.register = dispatcher.register
 		#update_wrapper(wrapped_f, func)
 		wrapped_f.__name__=func.__name__
 		wrapped_f.__doc__=func.__doc__
 		return wrapped_f
@@ -297,14 +294,15 @@
 				engine = MongoClient(host)[dbname]
 			else:
 				host='{}:{}'.format(hostname,port)
 				engine = MongoClient(host)
 		elif all([hostname,port,dbname]):
 			dbURL='{}{}://{}@{}:{}/{}'.format(dialect,driver,user,hostname,port,dbname)
 			engine = create_engine(dbURL)
+		pqint( "===DB-Driver:",engine, file=sys.stderr)
 	except:
 		pqint( "***DB ERROR:", sys.exc_info()[1], file=sys.stderr)
 	return engine
 
 def conn2mydb(engine=None,dbname=None,hostname="localhost",port=3306,dialect='mysql',driver='',user='sfdbo'):
 	return conn2db(engine=engine,dbname=dbname,hostname=hostname,port=port,dialect=dialect,driver=driver,user=user)
```

### Comparing `talan-0.1.4.3/talan/_alan_date.py` & `talan-0.1.4rc1/talan/_alan_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/env python 
-"""Usage of: _alan_date.py FUNCNAME [JSON]
-----------------------------------------
+"""
 Program: _alan_date.py
-Description: Date functions for ALAN
-Example,
-./_alan_date.py s2dt
-OR
-./_alan_date.py next_month_date 'dict(months=2)'
+Description:
+	Date functions for ALAN,
+	convert daily price into monthly and update to prc_m_hist
 Functions:
 	def s2dt(s=None,dformat=''):
 	def get_start_end(start=None,end=None,dformat='',**kwargs):
 	def str2epoch(s=None,dformat=''):
 	def next_date(d=None,dformat='',dtTF=True,**kwargs):
 	def next_month_date(d=None,months=1):
 	def delta2dates(end,start,dformat="%Y%m%d",fq="D",rounding=0):
@@ -24,18 +21,17 @@
 	def dt2ymd(dt,dformat="%Y%m%d"):
 	def ymd2dt_example():
 	def dt2ymd_example():
 	def freq_d2m(s,fq='M',method='last'):
 	def daily2month(fromSql=None,tablename=None,dbname="ara",hostname="localhost",wmode='fail',fq='M',method='last'):
 	def tg_next2week(pdt,cdt=None,nwk=1):
 	def tg_latest2week(pdt,cdt=None,nwk=1):
-Last mod., Mon 03 Jul 2023 02:19:09 PM EDT
+Last mod., Tue Apr 30 10:32:36 EDT 2019
 Version: 0.70
 """
-__usage__='\n'.join(__doc__.split('\n')[:8])
 import sys
 import numpy as np
 from math import isinf, log
 from datetime import datetime,timedelta,date
 from dateutil import relativedelta
 from _alan_calc import subDict
 
@@ -375,38 +371,14 @@
 
 def utc2local(s,tz1='UTC',tz2='US/Eastern',fmt="%b-%d %I:%M%p %Z"):
 	''' convert datetime-string from `tz1` to `tz2` in format `fmt` 
 	'''
 	import pandas as pd
 	return pd.Timestamp(s,tz=tz1).tz_convert(tz=tz2).strftime(fmt)
 
-def tst101():
+if __name__ == '__main__':
 	fromSql="SELECT * FROM spdr_price_hist WHERE ticker='{}' ORDER BY pbdate"
 	ticker=sys.argv[1] if len(sys.argv)>1 else "IBM"
 	fromSql=fromSql.format(ticker)
 
 	sys.stderr.write("{}\n".format(daily2month(fromSql).tail()))
 	print("20180221-20170320 in months:",delta2dates(20180221,20170320,fq="M"))
-
-def runArgs():
-	if sys.argv[1:]:
-		funcName=sys.argv[1]
-	else:
-		sys.exit(__usage__)
-	opts=eval(sys.argv[2]) if sys.argv[2:] else {}
-	if funcName in globals() and hasattr(globals()[funcName],'__call__'):
-		ret=globals()[funcName](**opts)
-	else:
-		sys.stderr.write("**ERROR: {}() Not Exist\n".format(funcName))
-		ret = __usage__
-	return ret
-
-def mainTst():
-	try:
-		ret = runArgs()
-	except Exception as e:
-		sys.stderr.write("**ERROR: {}\n".format(str(e)))
-		ret = __usage__
-	return ret
-	
-if __name__ == '__main__':
-	sys.exit(mainTst())
```

### Comparing `talan-0.1.4.3/talan/_alan_mp4.py` & `talan-0.1.4rc1/talan/_alan_mp4.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/_alan_ohlc_fcs.py` & `talan-0.1.4rc1/talan/_alan_ohlc_fcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,21 +99,19 @@
 		pqint( "==Input Args:{}".format(optx), file=sys.stderr)
 		pqint( "==df\n:{}".format(vprc.tail()), file=sys.stderr)
 	ret=robj.globalenv['rForecast'](df,asof,debugTF=debugTF,**optx)
 	#ret=robj.globalenv['rForecast'](df,asof,plevel=plevel,funcname=funcname,autoArima=autoArima,debugTF=debugTF,logTF=logTF,difTF=difTF,freq=freq,fcsLst=fcsLst)
 	#return ret
 	if opts['dwmTF'] is True:
 		#dwm=pandas2ri.conversion.rpy2py(ret[1])
-		#dwm=ret[1]
-		dwm=pd.DataFrame({x:y for x,y in ret[1].items()})
+		dwm=ret[1]
 		dwm['ticker']=ticker
 	else:
 		dwm=pd.DataFrame()
-	#dd=ret[0]
-	dd=pd.DataFrame({x:y for x,y in ret[0].items()})
+	dd=ret[0]
 	dd['ticker']=ticker
 	dd['freq']=freq
 	if debugTF:
 		sys.stderr.write("==>dd:\n{}\n==>dwm:\n{}\n==>datax:\n{}\n".format(dd,dwm,datax.tail()))
 	return (dd,dwm,datax)
 
 def convert_data_comment_fcst(ticker,category,df,pgDB=None,lang="cn",mp3YN=True,ts=None,fpTF=False):
```

### Comparing `talan-0.1.4.3/talan/_alan_optparse.py` & `talan-0.1.4rc1/talan/_alan_optparse.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/_alan_pppscf.py` & `talan-0.1.4rc1/talan/_alan_pppscf.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/_alan_rmc.py` & `talan-0.1.4rc1/talan/_alan_rmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 # -*- coding: utf-8 -*-
 '''
 Remote Model Calculation
 
 last mod., Tue Oct 27 17:30:23 EDT 2020
 '''
 import sys
+#sys.path.append("/apps/fafa/pyx/tst/")
 #from __future__ import print_function
 import pandas as pd, numpy as np, json, os, datetime
 import simplejson
 from pandas import Timestamp
 from bson.objectid import ObjectId
 from flask import render_template,Response,make_response
 #from jinja2 import Template as jjTemplate
 from types import *
 from subprocess import Popen, PIPE
 from glob import glob, iglob
 from _alan_str import lsi2nlg_calc,combine_cmd2dict,jj_fmt,sysCall,find_mdb,write2mdb,dtCvt
-from _alan_calc import saferun,safeRunArg,subDict,sqlQuery,getKeyVal,pqint,subDF,subDict,renameDict
+from _alan_calc import subDict,sqlQuery,getKeyVal,pqint,subDF,subDict,renameDict
 from _alan_date import tg_latest2week,tg_next2week,next_date,dt2ymd,ymd2dt,s2dt,utc2local
 from alanapi import run_alanapi,opt_alanapi,search_comment,search_factor,search_quote,search_hist,search_history,search_list,search_allocation,search_mp3,search_ohlc
 #,udfStr,roundUSD
 from _alan_pppscf import batch_pppscf
 from _alan_ohlc_fcs import batch_ohlc_fcs
 from math import *
 import requests
 from importlib import import_module
 if sys.version_info.major == 2:
 	reload(sys)
 	sys.setdefaultencoding('utf8')
+pd.options.display.float_format='{:,.2f}'.format
+
+pd.set_option('display.max_colwidth', -1)
 pd.options.display.float_format = '{:,g}'.format
-#pd.options.display.float_format='{:,.2f}'.format
-#pd.set_option('display.max_colwidth', -1)
 
 def pqrint(*args,**kwargs):
 	return pqint(*args,**kwargs)
 
 def rPost(url='',data={},timeout=5,ret='{}'):
 	try:
 		if len(url)<0:
@@ -57,41 +59,38 @@
 
 def display_page(pathname='index',request=None,**optx):
 	return show_page(pathname=pathname,request=request,**optx)
 
 def show_page(pathname='index',request=None,**optx):
 	sys.stderr.write("===START show_page request:{}\n".format(request))
 	opts=wrap_request(request)
-	opts.update(pathname=pathname)
 	sys.stderr.write(" --opts:{}\n".format(opts))
 	try:
 		pageBase=pathname
 		funcName='page_{}'.format(pageBase)
-		htmlName=optx.pop('html',None)
+		htmlName=opts.pop('html',None)
 
-		sys.stderr.write(" --show_page path:{} func:{} html:{} / opts:\n{}\n".format(pathname,funcName,htmlName,opts))
 		#----------------------------------------------------------------
 		if funcName=='page_api' and htmlName is None:
 			# Run 'page_api' command
 			dd = page_api(**opts)
 			if isinstance(dd,str):
 				if opts.get('output','').lower() in ['html','csv'] and opts.get('outTF',False):
 					return dd
 				ret=Response(dd,mimetype='application/json')
 				return ret
 			ret=Response(simplejson.dumps(dd,ignore_nan=True),mimetype='application/json')
 			return ret
 		elif funcName in globals() and hasattr(globals()[funcName],'__call__'):
 			# Run corresponding funcName like page_???()
 			pass
-		elif "templates/{}".format(htmlName) in glob('templates/*html'):
-			# TBD, newly added @ Sun 22 Jan 2023 01:32:15 PM EST
-			# Process a dynamic page: dlp_???.html without funcName: page_???()
-			sys.stderr.write("++ Process {} with INPUT/opts:\n{}\n".format(htmlName,opts))
-			ret = process_page(htmlName, dd={}, **opts)
+		elif 'templates/{}'.format(htmlName) in glob('templates/*html'):
+			# Newly added @ Sat Oct 24 21:25:43 EDT 2020
+			# Process corresponding html page without funcName like page_???()
+			ret = process_page(htmlName, **opts)
 			return ret
 		else:
 			# Run home page page_index() as default
 			sys.stderr.write("**WARNINGS:{} not found".format(funcName))
 			funcName='page_{}'.format('index')
 			sys.stderr.write(", use:{} instead".format(funcName))
 
@@ -133,45 +132,39 @@
 
 def process_page(htmlName, dd, **opts):
 	# Processing output 
 	from bson import json_util as json
 	#opts.update({"import_module":import_module})
 	#opts.update({"getattr":getattr})
 	opts.update({"exists":os.path.exists})
-
-	sys.stderr.write("===processing page: {}\n".format(htmlName))
-
-	# response datax/mtx/content as JSON.dumps/list/str respectively
-	if isinstance(dd,dict): # response output: `datax` as a `JSON` text
+	if isinstance(dd,dict):
 		datax=json.dumps(dd,default=dtCvt)
-		opts.update(dd)
-		opts.update(datetime=datetime,pd=pd,s2dt=s2dt,utc2local=utc2local,json=json,locals=locals)
-		sys.stderr.write(" --opts: {}".format(opts)[:120]+"\n")
-		sys.stderr.write(" --datax[{}]: {}".format(type(dd),dd)[:200]+"\n")
-		ret= render_template(htmlName,datax=datax,**opts)
-	elif isinstance(dd,list): # response output: `mxt` as a `list` array
-		opts.update(datetime=datetime,pd=pd,s2dt=s2dt,utc2local=utc2local,json=json,locals=locals)
-		sys.stderr.write(" --opts: {}".format(opts)[:120]+"\n")
-		sys.stderr.write(" --mtx[{}]: {}".format(type(dd),dd)[:200]+"\n")
+		dd.update(datetime=datetime,pd=pd,s2dt=s2dt,utc2local=utc2local)
+		ret= render_template(htmlName,datax=datax,**dd)
+	elif isinstance(dd,list):
+		opts.update(datetime=datetime,pd=pd,s2dt=s2dt,utc2local=utc2local)
 		ret= render_template(htmlName,mtx=dd,**opts)
-	else: # response output: `content` as a `string` text
-		opts.update(datetime=datetime,pd=pd,s2dt=s2dt,utc2local=utc2local,json=json,locals=locals)
-		sys.stderr.write(" --opts: {}".format(opts)[:120]+"\n")
-		sys.stderr.write(" --content[{}]: {}".format(type(dd),dd)[:200]+"\n")
+	else:
+		opts.update(datetime=datetime,pd=pd,s2dt=s2dt,utc2local=utc2local)
 		ret= render_template(htmlName, content=dd,**opts)
 
+	sys.stderr.write("===processing page: {}\n".format(htmlName))
+	sys.stderr.write(" --opts: {}".format(opts)[:60]+"\n")
+	sys.stderr.write(" --data: {}".format(dd)[:200]+"\n")
+
 	if isinstance(dd,dict) and 'submit' in dd: 
 		ret = make_response(ret)
 		if dd['submit'] == 'login':
 			ret.set_cookie('userID', dd['user'])
 		elif dd['submit'] == 'logout':
 			ret.delete_cookie('userID')
 		elif dd['submit'] == 'delete':
 			ret.delete_cookie('userID')
 
+
 	return ret
 
 def page_api(**optx):
 	opts={"search":"comment","outTF":False}
 	opts.update(optx)
 	dfTF = opts.pop('dfTF',False)
 	opts.update(debugTF=True)
@@ -188,26 +181,14 @@
 			for x,y in data[j].items():
 				data[j][x]=dtCvt(y)
 		dd=data
 	else:
 		dd=data
 	return dd
 
-@safeRunArg({})
-def page_chat(**optx):
-	from chatgptAPI import chatgptAPI as cg
-	optx.pop("submit",None)
-	prompt=optx.get('prompt','')
-	if not prompt:
-		optx.update(prompt="this is a test")
-	pqint(" -- page_chat INPUT:\n",optx, file=sys.stderr)
-	dd = cg(**optx)
-	dd.update(prompt=optx['prompt']) 
-	return dd
-
 def page_login(**optx):
 	if 'submit' not in optx:
 		return optx
 	pqint(" -- page_login INPUT:\n",optx, file=sys.stderr)
 	submit=optx.pop('submit','login')
 	url = 'http://login.beyondbond.com/'
 	if submit in ['logout','lost-password','reset-password','delete','signup']:
@@ -290,29 +271,33 @@
 
 def page_globalmacro(**optx):
 	return page_api(**optx)
 
 def page_apitest(**optx):
 	return page_api(**optx)
 
-@safeRunArg({})
 def wrap_request(request):
 	dd={}
 	pqint("===request METHOD: {}".format(request.method), file=sys.stderr)
 	optGet = request.args.to_dict()
 	pqint("===request GET Input:\t",optGet, file=sys.stderr)
+	optPost = request.get_json()
+	pqint("===request POST Input:\t",optPost,request.form, file=sys.stderr)
 	user = request.cookies.get('userID')
 	pqint("===request cookies user:{}".format(user) , file=sys.stderr)
-	if request.method=='POST' and request.is_json:
-		optPost = request.get_json(force=True)
-		pqint("===request POST Input:\t",optPost,request.form, file=sys.stderr)
-		if optPost and isinstance(optPost,dict):
+	if request.method=='POST':
+		if optGet is not None:
+			dd.update(optGet)
+		if optPost is not None:
+			dd.update(optPost)
+	else:
+		if optPost is not None:
 			dd.update(optPost)
-	if optGet is not None:
-		dd.update(optGet)
+		if optGet is not None:
+			dd.update(optGet)
 	if request.form is not None:
 		dd.update(request.form.to_dict(flat=True))
 	#if request.form is not None:
 	#	dd.update(request.form)
 	if user is not None:
 		dd.update(user=user)
 	pqint("===request REQUEST Input:\t{}".format(dd) , file=sys.stderr)
```

### Comparing `talan-0.1.4.3/talan/_alan_str.py` & `talan-0.1.4rc1/talan/_alan_str.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 program: _alan_str.py
 Description: ALAN string utility functions for jinja2
 Version: 0.91
-Usage of, 
-python3 -c 'from _alan_str import jj_fmt;r=jj_fmt("daily_macro_cn.j2",fileTF=True,dirname="templates");print(r)' 2> /dev/null
-OR
-python3 -c 'from _alan_str import jjf_fmt;r=jjf_fmt("daily_macro_cn.j2");print(r)' 2> /dev/null
-to run jinjia2 
-
 Functions:
   prerr(e,*args,**kargs):
   str_contains(va=[],subs=[],vb=[],uniqueTF=True):
   str_matches(va=[],subs=[],vb=[],uniqueTF=True):
   clean_punctuation2upper(s,c=' '):
   remove_tags(raw_html):
   unique_set(a):
@@ -120,17 +114,14 @@
 Thu Aug 18 14:23:48 EDT 2022
 + rename upd2mdb() to upd2mdbOLD()
 + add upd2mdb()
 + add upd2many()
 Fri Sep  2 17:35:32 EDT 2022
 + add cgi2dict()
 Fri Sep  9 10:25:12 EDT 2022
-+ update check_latest_macro()
-replace ?_PCTCHG info as default macro data, no longer use `annual_rate` variable
-Fri 23 Dec 2022 04:40:31 PM EST
 """
 
 #from __future__ import print_function
 import sys
 import os
 from jinja2 import Environment as jinEnv, FileSystemLoader
 import jinja2.ext
@@ -149,15 +140,14 @@
 from pandas import Timestamp
 import re
 from subprocess import Popen, PIPE, STDOUT
 from importlib import import_module
 # IMPORT external functions
 from _alan_date import next_date,ymd2dt,dt2ymd,s2dt
 from _alan_calc import saferun,subDict,subDF,subVDict,renameDict,getKeyVal,sqlQuery,conn2mgdb,safeRunArg
-from chatgptAPI import chatgptAPI
 
 if sys.version_info.major == 2:
 	reload(sys)
 	sys.setdefaultencoding('utf8')
 
 def prerr(e,*args,**kargs):
 	'''print error message
@@ -226,33 +216,27 @@
 	from _alan_date import tg_latest2week,ymd2dt
 	xqr="""SELECT  x.value,x.pbdate,y.* from macro_hist_fred x, (SELECT a.vntdate,b.* FROM macro_vintage_date a, mapping_series_label b
 where a.series=b.series and b.freq in ('M','Q') ORDER BY vntdate DESC limit 1) as y
 WHERE x.series=y.series ORDER BY pbdate DESC limit 13 """
 	#df = sqlQuery(open('latest_macro_vintage.sql').read())
 	df = sqlQuery(xqr)
 	in2wTF = tg_latest2week(ymd2dt(df['vntdate'].iloc[0]),cdt=cdt,nwk=nwk)
-	if in2wTF is None or len(in2wTF)<1:
-		return in2wTF
 
 	#=  Check If annualRate is calc when source='deriv' in the 'mapping_series_label' table
-	seriesP=df['series'].iloc[-1]+"_PCTCHG"
-	xqr="""SELECT  x.value,x.pbdate,y.* from macro_hist_fred x, mapping_series_label y
-		WHERE x.series=y.series and x.series='{}' ORDER BY pbdate DESC """.format(seriesP)
-	dg=sqlQuery(xqr)
+	dg=sqlQuery("SELECT * from macro_hist_fred where series='{}' ORDER BY pbdate".format(df['series'].iloc[-1]+"_PCTCHG"))
 	if len(dg)>0:
-		#dg.rename(columns={"value":"annualRate"},inplace=True)
-		#df = df.merge(dg[['annualRate','pbdate']],on='pbdate')
-		#df['pctChange'] = df['annualRate'].diff(-1)
-		df = dg
-		df['pctChange'] = df['value'].pct_change(-1)
+		dg.rename(columns={"value":"annualRate"},inplace=True)
+		df = df.merge(dg[['annualRate','pbdate']],on='pbdate')
+		df['pctChange'] = df['annualRate'].diff(-1)
 	else:
 		df['pctChange'] = df['value'].pct_change(-1)
 
-	in2wTF.update(df.iloc[0].to_dict())
-	in2wTF.update(f=df)
+	if in2wTF is not None and len(in2wTF)>0:
+		in2wTF.update(df.iloc[0].to_dict())
+		in2wTF.update(f=df)
 	return in2wTF
 
 
 def dLst2df(dx,keyName='ticker',valName='pctChange'):
 	'''
 	convert list of dictionay to dataframe
 	'''
@@ -539,19 +523,14 @@
 	if fileTF is False:
 		return(j2Env.from_string(ts).render(**dd))
 		#return jjTemplate(ts).render(**dd)
 		#no loader environment specified for jjTemplate
 	else:
 		return(j2Env.get_template(ts).render(**dd))
 
-def jjf_fmt(ts,dirname='templates',fileTF=True,debugTF=False,j2onlyTF=False,**dd):
-	'''process jinja2 template string from file `{dirname}/{ts}`
-	'''
-	return jj_fmt(ts,dd,dirname=dirname,fileTF=fileTF,debugTF=debugTF,j2onlyTF=j2onlyTF)
-
 def jj2_fmt(ts,dirname='.',fileTF=False,debugTF=False,j2onlyTF=False,**dd):
 	return jj_fmt(ts,dd,dirname=dirname,fileTF=fileTF,debugTF=debugTF,j2onlyTF=j2onlyTF)
 
 def get_arg2func(funcName,**optx):
 
 
 	'''
@@ -1159,15 +1138,15 @@
 		#zobj=loads(dumps(zobj))
 		if limit>0:
 			mbson = dbM[tablename].find(jobj,zobj,sort=zsrt).limit(limit)
 		else:
 			mbson = dbM[tablename].find(jobj,zobj,sort=zsrt)
 		#mobj= json.loads(dumps(mbson))
 		mobj= [x for x in mbson]
-		#clientM.close()
+		clientM.close()
 		msg="success"
 	except Exception as e:
 		msg=str(e)
 		sys.stderr.write("**ERROR: {} @{}.find()\n".format(str(e),tablename))
 	if len(mobj)>0 and len(mobj[0])<1:
 		mobj=[]
 	if dfTF:
@@ -1300,21 +1279,20 @@
 		if getKeyVal(optx,'jsonObjReloadTF',False):
 			jobj = jsonObjReload(jobj)
 			sys.stderr.write(" --{} @ {}\n".format('jsonObjReload','insert_mdb()'))
 		if wmode=='upsert':
 			ret=upd2mdb(jobj,zpk=zpk,mcur=mdb[tablename])
 		else:
 			ret=mdb[tablename].insert_many(jobj,ordered=ordered)
-		errmsg="Success:{}\n".format(len(jobj))
+		errmsg="Success:{}".format(len(ret))
 	except Exception as e:
 		errmsg="**ERROR:{} @{}\n".format(str(e),"insert_mdb:insert_many")
 		sys.stderr.write(errmsg)
 		try:
-			sys.stderr.write("---wmode:{},ordered:{},zpk:{}\n".format(wmode,ordered,zpk))
-			sys.stderr.write("---JOBJ[{}]: {}\n".format(len(jobj),jobj[:2]))
+			sys.stderr.write("---JOBJ[0]:\n{}\n".format(jobj[0]))
 		except:
 			pass
 		return {},None,errmsg
 	return jobj,mdb,errmsg
 
 def save2mgdb(mLst=None,mky=None,dbM=None,tablename="temp",wmode='replace'):
 	if dbM is None or mLst is None:
@@ -1918,15 +1896,15 @@
 		colx=['ranking','ticker','price','volume','change','changePercent','marketCap','dollarValue','Range52Week','pbdt','sector','sector_cn','company','company_cn']
 	df=subDF(df,colx)
 	if nobs>0:
 		return df.iloc[:nobs]
 	else:
 		return df
 
-def ssh2mg(sshUser='rstudio',rhost='api1.beyondbond.com',lhostLst=['bbapi1','api1','api1.beyondbond.com','BHS1','bhs1','bhs1.beyondbond.com'],port=27017,**optx):
+def ssh2mg(sshUser='rstudio',rhost='api1.beyondbond.com',lhostLst=['bbapi1','api1','api1.beyondbond.com'],port=27017,**optx):
 	''' remotely connect to server `rhost` mongoDB via ssh-tunnel
 		local connection rhost="localhost" 
 	'''
 	import subprocess
 	lhost=subprocess.Popen("hostname",stdout=subprocess.PIPE).stdout.read().decode().strip()
 	rhost= rhost if lhost not in lhostLst else 'localhost'
 	return remote2mgdb(sshUser=sshUser,host=rhost,port=port,**optx)
```

### Comparing `talan-0.1.4.3/talan/alanapi.py` & `talan-0.1.4rc1/talan/alanapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 #import matplotlib.pyplot as plt 
 from hashlib import md5
 if sys.version_info.major == 2:
 	reload(sys)
 	sys.setdefaultencoding('utf8')
 
 # set pandas global display formula
-#pd.set_option('display.max_colwidth', -1)
+pd.set_option('display.max_colwidth', -1)
 pd.options.display.float_format='{:,.2f}'.format
 
 # set mongoDB database connection as globals()
 mgDB=conn2mgdb(dbname='ara')
 pgDB=conn2pgdb(dbname='ara')
 currDate=datetime.datetime.now()
 
@@ -311,37 +311,23 @@
 	if 'summary' in opts and opts['summary']:
 		queryObj.update({'summary':{'$regex':opts['summary'],'$options':'i'}})
 	if 'pubdates' in opts and opts['pubdates']:
 		ob = pubdates_ob(opts['pubdates'])
 		queryObj.update(ob)
 	return queryObj
 
-def chatgpt_comment(tkLst,fdLst,**optx):
-	from chatgptAPI import chatgptAPI;
-	vx="dbname,debugTF,end,hostname,instrument,lang,outTF,output,src,start,subtopic,tablename,topic".split(',')
-	for x in vx:
-		del optx[x]
-
-	res=chatgptAPI(**optx) 
-	if 'choices' in res:
-		return res['choices']
-	else:
-		return []
-
 def news_comment(tkLst,fdLst,lang='cn',dbname='ara',hostname='localhost',output='html',limit=200,**optx):
 	print("===@news_comment tkLst:{}, optx: {}".format(tkLst,optx),file=sys.stderr)
 	from _alan_str import ssh2mg
 	serverM,clientM=ssh2mg()
 	sys.stderr.write(" --serverM:{},clientM:{}\n".format(serverM,clientM))
 	from mongo_en2cn import mongo_en2cn as me
 	outTF=optx.pop('outTF',True)
 	tablename='rssNews'
 	jobj={}
-	transource=optx.pop('transource','google')
-	#transource=optx.pop('transource','openai')
 	subtopic=optx.get('subtopic','company')
 	sortLst=['pubDate']
 	data=[]
 	if subtopic=='company' and len(tkLst)>0:
 		ticker=tkLst[0]
 		from rssCompany import run_rssCompany as rrc
 		data = rrc(ticker)
@@ -356,15 +342,15 @@
 			jobj={'link':link}
 		elif not _id:
 			return []
 		else:
 			jobj={'_id':ObjectId(_id)}
 		field={'title','title_cn','summary','summary_cn'}
 		print("===Run Translation:",jobj,tablename,field,src,dest,file=sys.stderr)
-		data = me(jobj,clientM=clientM,tablename=tablename,field=field,src=src,dest=dest,transource=transource)
+		data = me(jobj,clientM=clientM,tablename=tablename,field=field,src=src,dest=dest)
 	else:
 		jobj = get_news_query(jobj,**optx)
 		pqint(" --->news query jobj:\n",jobj,file=sys.stderr)
 
 		field={'_id','ticker','title','title_cn','description','summary','summary_cn','pubDate','link','source'}
 		data,_,_=find_mdb(jobj,clientM=clientM,tablename=tablename,dbname=dbname,field=field,sortLst=sortLst,limit=limit,dfTF=outTF)
 		if isinstance(data,pd.DataFrame):
@@ -444,35 +430,25 @@
 	if len(df)<0:
 		return []
 	if isinstance(df,pd.DataFrame):
 		sys.stderr.write("==OPTS:{},FIELDS:{}, DATA:\n{}".format(opts,fdLst,df.tail(2)))
 	data = df # data = data_output(df,**opts)
 	return data
 
-def industry_comment(tkLst,fdLst,dbname='ara',output=None,**opts):
-	tablename='record_hilo'
-	try:
-		field=['category_cn','ticker','close','pchg','pbdate','label_cn','comment']
-		data,_,err=find_mdb({}, dbname=dbname,tablename=tablename,field=field,sortLst={"category":-1},dfTF=True)
-	except Exception as e:
-		sys.stderr.write("**ERROR: {},{} @{}\n".format(ticker,str(e),'industry_comment'))
-		data=[]
-	return data
-
-def industry_commentOLD(tkLst,fdLst,output=None,**opts):
+def industry_comment(tkLst,fdLst,output=None,**opts):
 	df = getlist_filter(fdLst=fdLst,subtopic='industry')
 	if not (tkLst is None or len(tkLst)<1 or tkLst[0] in ['','*']):
 		df = df[df['ticker'].isin(tkLst)]
 	if len(df)<1:
 		return None
 	data = df # data = data_output(df,output)
 	return data
 
 def search_comment(tkLst,fdLst,**opts):
-	topicLst='hourly|news|report|theme|peers|industry|MFRM|news1|chatgpt'.split('|')
+	topicLst='hourly|news|report|theme|peers|industry|MFRM|news1'.split('|')
 	topic=getKeyVal(opts,'topic','MFRM')
 	if topic not in topicLst:
 		return None
 	argName="{}_comment".format(topic)
 	if topic in topicLst and argName in globals():
 		pqint("==RUNNING {}() Inputs:{}".format(argName,opts),file=sys.stderr)
 		try:
@@ -614,15 +590,15 @@
 	from yh_chart import yh_spark_hist as ysh, runOTF;
 	src = opts.pop('src','iex')
 	src= "yh" if '^' in ticker or '=' in ticker else src
 	sys.stderr.write("---Get minute data {} from WEB::{}\n".format(ticker,src.upper()))
 	if src=='yh':
 		#datax = get_minute_yh(ticker,ranged='1d',tsTF=True,debugTF=False)
 		#d=ysh([ticker],saveDB=False,range='1d',types='chart',interval='5m',debugTF=True)
-		d=runOTF(ticker,ysh,deltaTolerance=900,types='chart',tablename='yh_chart_hist',zpk=['ticker','pbdt'],range='15m',interval='5m',debugTF=True,dbname='ara')
+		d=runOTF(ysh,ticker,deltaTolerance=900,types='chart',tablename='yh_chart_hist',zpk=['ticker','pbdt'],range='15m',interval='5m',debugTF=True,dbname='ara')
 		if len(d)>0:
 			datax=pd.DataFrame(d)
 		else:
 			return []
 	else:
 		datax = get_minute_iex(ticker,ranged='1d',date=None,tsTF=True,debugTF=False)
 	return datax
@@ -676,15 +652,15 @@
 	from _alan_calc import pullStockHistory
 	from yh_chart import yh_spark_hist as ysh, runOTF
 	datax = []
 	try:
 		datax = pullStockHistory(ticker,pgDB=pgDB,**opts)
 		if datax is None or len(datax)<1:
 			sys.stderr.write("**WARNING:{}\n".format("data not found in DB, live pulling"))
-			datax=runOTF(ticker,ysh,deltaTolerance=86400,types='chart',tablename='yh_daily_hist',zpk=['ticker','pbdt'],range='1y',interval='1d',debugTF=True,dbname='ara')
+			datax=runOTF(ysh,ticker,deltaTolerance=86400,types='chart',tablename='yh_daily_hist',zpk=['ticker','pbdt'],range='1y',interval='1d',debugTF=True,dbname='ara')
 			datax=pd.DataFrame(datax)
 	except Exception as e:
 		pqint("**ERROR:{} @ {}, opts:\n{}".format(str(e),'geteach_daily_history',opts) ,file=sys.stderr)
 	return datax
 
 def geteach_history(ticker,fdLst,**opts):
 	# for topic list 'financial','daily','minute'
```

### Comparing `talan-0.1.4.3/talan/csv2plotj2ts.py` & `talan-0.1.4rc1/talan/csv2plotj2ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 # -*- coding: utf-8 -*-
 """ Description: plot time series from a csv file and summarise the graphics
     Usage of:
 	csv2plotj2ts.py file --sep=DELIMITER
     Example:
 	# CPI/PPI historical comparison
 	psql.sh -d ara < cpippi_hist.sql|grep -v row|python3 csv2plotj2ts.py  --columns=series,value,pbdate  --xaxis=pbdate --pivot_group=series --pivot_value=value  --title="CPI/PPI 走勢" --x_fmt='%m/%Y' --extra_xs='pltStyle="classic";renColumns={"PPIFIS_PCTCHG":"PPI","CPIAUCNS_PCTCHG":"CPI"};ylabel="CPI/PPI (%)";endValueTF=True;yfmt="0.2f";' -
-	# treasury spread (10YR-3MO) with 2-YAXIS plot
-	printf 'select tsy_3_mo,tsy_10_yr,ROUND((tsy_10_yr-tsy_3_mo)::numeric,2) as "SPREAD_3MO_10YR", pbdate from tsy_hist where pbdate>=20220101 order by pbdate'|psql.sh -d ara|grep -v row |python3 csv2plotj2ts.py - --xaxis=pbdate --extra_xs='sharXTF=True;columns2="SPREAD_3MO_10YR";kind2="area";color2="lightgray";yfmt=",.2f";endValueTF=True;ylabel="TSY YIELD %";ylabel2="SPREAD %"' --title="TREASURY 10Y - 3MO SPREAD YEAR-TO-DATE" --debug
 	# treasury rates and spread with 2-YAXIS plot
-	printf 'select tsy_2_yr,tsy_10_yr,ROUND((tsy_10_yr-tsy_2_yr)::numeric,2) as "SPREAD_2_10YR", pbdate from tsy_hist where pbdate>=20220101 order by pbdate'|psql.sh -d ara|grep -v row |python3 csv2plotj2ts.py - --xaxis=pbdate --extra_xs='sharXTF=True;columns2="SPREAD_2_10YR";kind2="area";color2="lightgray";yfmt=",.2f";endValueTF=True;ylabel="TSY YIELD %";ylabel2="SPREAD %"' --title="TREASURY 10Y-2Y SPREAD YTD"
+	printf 'select tsy_2_yr,tsy_10_yr,ROUND((tsy_10_yr-tsy_2_yr)::numeric,2) as "SPREAD_2_10YR", pbdate from tsy_hist where pbdate>=20220401 order by pbdate'|psql.sh -d ara|grep -v row |python3 csv2plotj2ts.py - --xaxis=pbdate --extra_xs='sharXTF=True;columns2="SPREAD_2_10YR";kind2="area";color2="lightgray";yfmt=",.2f"' --title="TREASURY 10Y - 2Y SPREAD in Q2/2022"
 	# minute data for 3 major market indices
-	yh_hist_batch.py --range=1d --gap=1m   --no_database_save ^GSPC ^DJI ^IXIC --output=csv | python3 csv2plotj2ts.py  --columns=close,epochs,ticker  --xaxis=epochs --pivot_group=ticker --pivot_value=close  --title="美股行情$(date +'%D %R')" --return_since_inception --x_fmt='%H:%M' --extra_xs='pltStyle="dark_background";renColumns={"^GSPC":"標普500","^DJI":"道瓊指數","^IXIC":"納斯達克指數"};yfmt=",.2f";endValueTF=True'  -
+	yh_hist_batch.py --range=1d --gap=1m   --no_database_save ^GSPC ^DJI ^IXIC --output=csv | python3 csv2plotj2ts.py  --columns=close,epochs,ticker  --xaxis=epochs --pivot_group=ticker --pivot_value=close  --title="美股大盤走勢$(date +%m/%d/%Y)" --return_since_inception --x_fmt='%H:%M' --extra_xs='pltStyle="classic";renColumns={"^GSPC":"標普500","^DJI":"道瓊指數","^IXIC":"納斯達克指數"}' -
 	# daily data since begining of the year for 3 major market indices
 	yh_hist_batch.py --range=20210101, --gap=1d   --no_database_save ^GSPC ^DJI ^IXIC --output=csv | python3 csv2plotj2ts.py  --columns=close,pbdate,ticker  --xaxis=pbdate --pivot_group=ticker --pivot_value=close  --title="美股大盤$(date +%Y)年走勢" --return_since_inception --x_fmt='%m/%d' --extra_xs='pltStyle="classic";renColumns={"^GSPC":"標普500","^DJI":"道瓊指數","^IXIC":"納斯達克指數"}' -
 
 	# OR (directly pulling data)
 	python3 csv2plotj2ts.py TCEHY ^HSI ^GSPC --columns=close,pbdate,ticker  --xaxis=pbdate --pivot_group=ticker --pivot_value=close  --title='騰訊/恆生/標普-2021年初至今報酬率' --interpolate --return_since_inception --x_fmt='%m/%d/%y' --extra_xs='ranged="20210101,20210804";gap="1d";pltStyle="classic";renColumns={"TCEHY":"騰訊","^HSI":"恆生指数","^GSPC":"標普500"}'
 	python3 csv2plotj2ts.py ^GSPC ^DJI ^IXIC --columns=close,epochs,ticker  --xaxis=epochs --pivot_group=ticker --pivot_value=close  --title='美股大盤走勢' --return_since_inception --x_fmt='%H:%M' --extra_xs='ranged="1d";gap="1m";pltStyle="classic";renColumns={"^GSPC":"標普500","^DJI":"道瓊指數","^IXIC":"納斯達克指數"}' 
 	# FROM data file
@@ -76,15 +74,15 @@
 	if reverseTF is True: # invert-match, select non-matching [kyLst] keys 
 		return { ky:myDict[ky] for ky in myDict.keys() if ky not in kyLst }
 	else:
 		return { ky:myDict[ky] for ky in myDict.keys() if ky in kyLst }
 
 def ymd_parser(x,fmt='%Y%m%d'): return datetime.strptime(str(x),fmt)
 
-def epoch_parser(x,s=1000): return pd.Timestamp.fromtimestamp(int(x/s)).round(freq='T')
+def epoch_parser(x,s=1000): return datetime.fromtimestamp(int(x/s))
 
 def extrapolate_series(yo):
 	yg=yo.dropna()
 	#ygi = [int(x) for x in yg.index.values]
 	#fn = interp1d(ygi, yg.values, fill_value='extrapolate')
 	#yoi = [int(x) for x in yo.index.values]
 	#return fn((yoi)
@@ -204,15 +202,15 @@
 				idxpt=[epoch_parser(x) for x in df[pbname]]
 			else:
 				idxpt=[ymd_parser(x,fmt="%Y%m%d") for x in df[pbname]]
 		else:
 			idxpt=[ymd_parser(x,fmt=x_fmt) for x in df[pbname]]
 		df.set_index(pd.DatetimeIndex(idxpt),inplace=True)
 		df.index.rename(idxname,inplace=True)
-		df = df.drop([pbname],axis=1)
+		df = df.drop(pbname,1)
 	elif idxname in df.columns:
 		df[idxname] = pd.to_datetime(df[idxname])
 		df.set_index(idxname,inplace=True)
 	else:
 		df = df.reset_index(drop=True)
 
 
@@ -304,18 +302,14 @@
 		sys.stderr.write("{}\n".format(df.head()))
 		sys.stderr.write("{}\n".format(df.tail()))
 	nobs=len(df.index)
 	nsp = int(nobs/nbins) if nobs>nbins*2 else nobs
 	#ds=[y for j,y in enumerate(df.index) if j%nsp==0]
 	#ax=df.plot(xticks=ds,title=title)
 	colorUD = ['red','green'] if lang=='cn' else ['green','red']
-	if pltStyle[:4]=='dark':
-		colorLst=['yellow','red','cyan','salmon','lightgray','pink']
-	else:
-		colorLst=['blue','red','green','salmon','lightgray','cyan']
 	if ohlcComboTF is True:
 		from alan_plot import plot_candlestickCombo
 		from _alan_calc import run_tech
 		chartType = 'minute' if pbname == 'epochs' else 'chart'
 		#ma1=5;ma2=30
 		ma1,ma2=sma=getKeyVal(kwargs,'sma',[5,30])
 		datax = run_tech(df, pcol='close',winLst=sma,debugTF=debugTF,nanTF=True)
@@ -346,14 +340,15 @@
 		elif 'open' not in df:
 			return df, None, None
 		from alan_plot import plot_candlestick
 		chartType = 'minute' if pbname == 'epochs' else 'chart'
 		ax = plot_candlestick(df,tsidx=df.index,chartType=chartType,title=title,block=False,debugTF=debugTF,ax=ax,trendTF=trendTF,npar=npar,colorUD=colorUD)
 		x_fmt = "%H:%M" if chartType == 'minute' else x_fmt
 	else:
+		colorLst=['blue','red','green','salmon','lightgray','cyan']
 		if len(df.columns)>1 and sharexTF:
 			col2=df.columns[1]
 			df.plot(ax=ax,grid=True,color=colorLst,secondary_y=col2,x_compat=True)
 			ylabel2=getKeyVal(kwargs,'ylabel2',col2)
 			ax.right_ax.set_ylabel(ylabel2,fontproperties=fontProp(size=12))
 		else:
 			df.plot(ax=ax,grid=True,color=colorLst,x_compat=True)
@@ -379,14 +374,20 @@
 			axv.yaxis.set_major_formatter(FuncFormatter(lambda x,pos: '{:{}}'.format(x,yfmt2)))
 			if len(ylabel2)>0:
 				axv.set_ylabel(ylabel2)
 	if len(ylabel)>0:
 		ax.set_ylabel(ylabel,fontproperties=fontProp(size=12))
 	elif rsiYN is True: # calc Returns Since Incept
 		ax.set_ylabel("Returns Since Inception (%)")
+	endValueTF=kwargs.pop('endValueTF',False)
+	if endValueTF:
+		for sx in df:
+			plt.annotate("{:{}}".format(df[sx].iloc[-1],yfmt), xy=(1, df[sx].iloc[-1]), xytext=(8, 0),
+				xycoords=('axes fraction', 'data'), textcoords='offset points')
+	ax.grid(linestyle='dotted',linewidth=0.5)
 	if df.index._typ == "datetimeindex":
 		if debugTF is True:
 			sys.stderr.write("==DF:\n{}\n".format(df.tail()))
 		mddfmt=mdates.DateFormatter(x_fmt)
 		ax.xaxis.set_major_formatter(mddfmt)
 		xtinterval=(df.index[1]-df.index[0])
 		if xtinterval.days < 7 and  xtinterval.days>=1 : # daily data
@@ -416,15 +417,14 @@
 			locator.intervald[5] = [0,5,10,15,20,25,30,35,40,45,55]
 			mddfmt = mdates.AutoDateFormatter(locator)
 			mddfmt.scaled[1/(24.*60.)] = '%M:%S' 
 			ax.xaxis.set_major_locator(locator)
 			ax.xaxis.set_major_formatter(mddfmt)
 			sys.stderr.write("{} {}\n".format( "Second data use AutoDateLocator",xtinterval.seconds))
 		elif xtinterval.seconds and xtinterval.seconds < 100 : # minute data
-			ax.set_xlim(df.index[0], df.index[-1])
 			bym = [0,15,30,45] if nobs<=120 else [0,30] if nobs<=360 else [0]
 			xlocator = mdates.MinuteLocator(byminute=bym, interval = 1)
 			ax.xaxis.set_major_locator(xlocator)
 			sys.stderr.write("{} {}\n".format( "Minute data use MinuteLocator",xtinterval.days))
 		else: # periodic data
 			sys.stderr.write("{} {}\n".format( "Periodic data use DayLocator",nsp))
 			#ax.xaxis.set_major_locator(mdates.DayLocator(interval=nsp))
@@ -438,32 +438,14 @@
 		h1, l1 = ax.get_legend_handles_labels()
 		h2, l2 = ax.right_ax.get_legend_handles_labels()
 		if len(ylabel)<1 and len(l1)>0:
 			ylabel=l1[0]
 		ax.legend(h1+h2, [ylabel]+[ylabel2], loc="upper left",prop=prop)
 	elif len(df.columns)>0 and sharexTF is False and ohlcTF is False:
 		ax.legend(df.columns,loc="upper left",prop=prop)
-	endValueTF=kwargs.pop('endValueTF',False)
-	if endValueTF:
-		for j,sx in enumerate(df):
-			try:
-				xl=mdates.date2num(df.index[-1])
-				cx=colorLst[j]
-				ax.annotate("{:{}}".format(df[sx].iloc[-1],yfmt), xy=(1, df[sx].iloc[-1]), xytext=(-25,25+15*j),
-					xycoords=('axes fraction', 'data'), textcoords='offset points', 
-					arrowprops=dict(arrowstyle='-|>',color=cx),size=10,color=cx)#,ha=('right'), va='bottom')
-			except Exception as e:
-				sys.stderr.write("**ERROR:{}. {} {!r:}\n".format(j,sx,str(e)))
-				continue
-		lgx=["{}: {:{}}%".format(x,y,yfmt) for x,y in zip(df.columns,df.iloc[-1])]
-		ax.legend(lgx,loc="upper left",prop=prop)
-		if debugTF:
-			sys.stderr.write(" --endValue List:\n{}\n{}\n".format(df.columns,df.iloc[-1].values))
-		sys.stderr.write(" --endValue List:\n{}\n{}\n".format(df.columns,df.iloc[-1].values))
-	ax.grid(linestyle='dotted',linewidth=0.5)
 	#ax.legend().set_visible(False)
 	#logo = mimage.imread("aicaas_icon.png")
 	#plt.figimage(logo, xo=20,yo=420)
 	plt.subplots_adjust(left=0.1,bottom=0.30)
 	if pngname is not None and len(pngname)>4:
 		plt.savefig(pngname)#, bbox_inches='tight',dpi=1000)
 		sys.stderr.write("Save chart {} to {}\n".format(title,pngname))
```

### Comparing `talan-0.1.4.3/talan/find_recent_eps.py` & `talan-0.1.4rc1/talan/find_recent_eps.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/fredReader.py` & `talan-0.1.4rc1/talan/fredReader.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/headline_calc.py` & `talan-0.1.4rc1/talan/headline_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
 	return dd
 
 def find_hiloRecord(ticker='^GSPC',end=None,days=366,debugTF=False):
 	#from record_hilo import find_record_hilo as frh
 	from record_hilo import recordHiLo as frh
 	from _alan_calc import pull_stock_data as psd
-	df=psd(ticker,end=end,days=days,pchgTF=True,searchDB=False)
+	df=psd(ticker,end=end,days=days,pchgTF=True)
 	endDT=df.index[-1]
 	jobj=frh(df,endDT,ticker,debugTF=debugTF)
 	hiloRecord = jobj['YTD'] if jobj['YTD'] else {}
 	return(hiloRecord)
 
 import numpy as np
 import datetime
```

### Comparing `talan-0.1.4.3/talan/headline_sts.py` & `talan-0.1.4rc1/talan/headline_sts.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/iex_peers.py` & `talan-0.1.4rc1/talan/iex_peers.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/lsi_daily.py` & `talan-0.1.4rc1/talan/lsi_daily.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/macro_event_yh.py` & `talan-0.1.4rc1/talan/macro_event_yh.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/plot_templates.py` & `talan-0.1.4rc1/talan/plot_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,27 +88,24 @@
 	plot daily_peers by marketcap barh
 	'''
 	sys.stderr.write("===start:{}()\n".format("plot_daily_conclusion"))
 	ticker = getKeyVal(optx,'ticker')
 	if backend is not None:
 		plt.switch_backend(backend)
 	chartpath,chartname = gen_chartpath(**optx)
-	if 'snsStyle' in optx:
-		sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-	else:
-		plt.style.use(optx.pop('pltStyle',"dark_background"))
+	sns.set(style="whitegrid")
+
 	# define plot
 	if fig is None:
 		fig, ax = plt.subplots(figsize=figsize)
-	#ax.grid(False, axis='y')
-	ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+	ax.grid(False, axis='y')
 	ax.spines['right'].set_color('none')
 	ax.spines['top'].set_color('none')
-	#ax.spines['bottom'].set_color('none')
-	#ax.spines['left'].set_color('none')
+	ax.spines['bottom'].set_color('none')
+	ax.spines['left'].set_color('none')
 
 	bottom=optx['bottom'] if 'bottom' in optx else 0.25
 
 	#da.plot(ax=ax,kind=kind,position=position,width=width)
 	da = da[['comment','pchg']].sort_values(by='pchg',ascending=False).iloc[0:10,:]
 	plt.title('指標變化百分比',fontproperties=fontProp(size=15))
 	da['comment'] = [ xstr.strip('[,.，。]') for xstr in da['comment'].values ]
@@ -155,15 +152,15 @@
 	sys.stderr.write("===start:{}()\n".format("plot_intraday_headline"))
 	bottom=optx['bottom'] if 'bottom' in optx else 0.2
 	chartpath = getKeyVal(optx,'chartpath','')
 	chartname = getKeyVal(optx,'chartname','')    
 	x_fmt = getKeyVal(optx,'x_fmt','%H:%M')    
 	#chartpath,chartname = gen_chartpath(**optx)    
 	from csv2plotj2ts import get_csv2plot,get_csvdata,subDict
-	opts ={'debugTF': True,'pngname': None, 'debugTF': True, 'rsiYN': True, 'renColumns': {'^IXIC': '納斯達克指數', '^DJI': '道瓊指數', '^GSPC': '標普500'}, 'colLst': 'change,pchg,close,epochs,ticker', 'hdrLst': None, 'npar': 15, 'days': 730, 'j2ts': None, 'start': None, 'pivot_group': 'ticker', 'gap': '1m', 'trendTF': False, 'ohlcTF': False, 'src': 'yh', 'pivot_value': 'close', 'pchgTF':True, 'end': None, 'title': '美股大盤走勢2019-09-17', 'lang': 'cn', 'backend': 'tkAgg', 'nbins': 6, 'tsTF': True, 'ranged': '1d', 'ohlcComboTF': False, 'sep': '|', 'interpolateYN': False, 'xaxis': 'epochs', 'pltStyle': 'dark_background', 'x_fmt': '%H:%M'}
+	opts ={'debugTF': True,'pngname': None, 'debugTF': True, 'rsiYN': True, 'renColumns': {'^IXIC': '納斯達克指數', '^DJI': '道瓊指數', '^GSPC': '標普500'}, 'colLst': 'change,pchg,close,epochs,ticker', 'hdrLst': None, 'npar': 15, 'days': 730, 'j2ts': None, 'start': None, 'pivot_group': 'ticker', 'gap': '1m', 'trendTF': False, 'ohlcTF': False, 'src': 'yh', 'pivot_value': 'close', 'pchgTF':True, 'end': None, 'title': '美股大盤走勢2019-09-17', 'lang': 'cn', 'backend': 'tkAgg', 'nbins': 6, 'tsTF': True, 'ranged': '1d', 'ohlcComboTF': False, 'sep': '|', 'interpolateYN': False, 'xaxis': 'epochs', 'pltStyle': 'classic', 'x_fmt': '%H:%M'}
 	if len(tkLst)<1:
 		tkLst= ['^GSPC', '^DJI', '^IXIC']
 	if len(chartpath)>5:
 		optx.update(pngname=chartpath)
 	opts.update(**optx)
 	renColumns = opts['renColumns']
 	gkys=['sep','src','days','start','end','colLst','hdrLst','debugTF','ranged','gap','tsTF','pchgTF','searchDB']
@@ -186,36 +183,32 @@
 	
 	max_num = da.values.max()
 	min_num = da.values.min()
 	min_index = np.min(da.index)
 
 	try:
 		plt.rcParams.update(plt.rcParamsDefault)
-		if 'snsStyle' in opts:
-			sns.set_style(opts.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-		else:
-			plt.style.use(opts.pop('pltStyle',"dark_background"))
+		sns.set_style("whitegrid",{'grid.linestyle':'--'})
 		fig, ax=plt.subplots(figsize=figsize)
 		fig.autofmt_xdate()
 		if(opts['gap'][-1:]=='m'):
 			x_lim = min_index.replace(hour=16, minute =0 )    
 			plt.xlim(min_index-timedelta(minutes=5), x_lim+timedelta(minutes=5))
 		##plt.ylim(min_num-(max_num-min_num)/2, max_num+(max_num-min_num)/5)
 		#plt.xlabel('Time',fontsize=15)
 		#plt.ylabel('price',fontsize=15)
 		#hours = mdates.HourLocator(interval = 1)
 		h_fmt = mdates.DateFormatter(x_fmt)
 		#ax.xaxis.set_major_locator(hours)
 		ax.xaxis.set_major_formatter(h_fmt)
-		#ax.grid(False, axis='x')
-		ax.grid(opts.get('grid',True),linestyle='dotted',linewidth=0.5)
+		ax.grid(False, axis='x')                        
 		ax.spines['right'].set_color('none')
 		ax.spines['top'].set_color('none')
-		#ax.spines['bottom'].set_color('none')
-		#ax.spines['left'].set_color('none')
+		ax.spines['bottom'].set_color('none')
+		ax.spines['left'].set_color('none')
 		#ax.set_ylabel('Returns Since Previous Close in %')
 		ax.set_ylabel('自前日收盤價報酬率%',fontproperties=fontProp())
 		plt.title(title,fontproperties=fontProp(size=15))
 		#laLst=('標普500','道瓊指數','納斯達克指數')
 		#for j,xlabel in enumerate(laLst):
 		for j,tkX in enumerate(tkLst):
 			xlabel = renColumns[tkX]
@@ -250,15 +243,15 @@
 		ticker=df
 		from _alan_calc import pullStockHistory as psd
 		ranged = getKeyVal(optx,'ranged','1d')
 		gap = getKeyVal(optx,'gap','1m')
 		datax = psd(ticker,gap=gap,ranged=ranged,days=1500,src=src)
 		datax.rename(columns={'close':ticker}, inplace=True)
 		df = datax[[ticker]]
-		if src=='fred' and ticker[-7:]!='_PCTCHG':
+		if src=='fred':
 			tk2=ticker+'_PCTCHG'
 			dx2 = psd(tk2,src=src,days=1500)
 			if len(dx2)>0:
 				dv = datax[[ticker]]
 				df = dx2[['close']]
 		elif 'volume' in datax:
 			dv = datax[['volume']]
@@ -274,25 +267,21 @@
 	chartpath,chartname = gen_chartpath(**optx)
 	try:
 		from _alan_pppscf import vertex_locator
 		if not isinstance(df,pd.DataFrame):
 			df = pd.DataFrame(data=df)
 		if fig is None:
 			plt.rcParams.update(plt.rcParamsDefault)            
-			if 'snsStyle' in optx:
-				sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-			else:
-				plt.style.use(optx.pop('pltStyle',"dark_background"))
+			sns.set_style("whitegrid",{'grid.linestyle':'--'})                 
 			fig, ax=plt.subplots(figsize=figsize)
-			#ax.grid(False, axis='x')                        
-			ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+			ax.grid(False, axis='x')                        
 			ax.spines['right'].set_color('none')
 			ax.spines['top'].set_color('none')
-			#ax.spines['bottom'].set_color('none')
-			#ax.spines['left'].set_color('none')            
+			ax.spines['bottom'].set_color('none')
+			ax.spines['left'].set_color('none')            
 		if debugTF:
 			sys.stderr.write("===== DF:\n{}\n".format(df.tail()))
 		#ax.plot(df.index,df[ticker])
 		#df.plot(ax=ax)
 		ax.plot(df.index,df.iloc[:,0])
 		x_fmt = getKeyVal(optx,'x_fmt','') 
 		yunit=['','1,000','Million','Billion','Trillion']
@@ -357,28 +346,24 @@
 	plot daily_peers by marketcap barh
 	'''
 	sys.stderr.write("===start:{}()\n".format("plot_daily_mostactive"))
 	ticker = getKeyVal(optx,'ticker')
 	if backend is not None:
 		plt.switch_backend(backend)
 	chartpath,chartname = gen_chartpath(**optx)
-	if 'snsStyle' in optx:
-		sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-	else:
-		plt.style.use(optx.pop('pltStyle',"dark_background"))
+	sns.set(style="whitegrid")
 
 	# define plot
 	if fig is None:
 		fig, ax = plt.subplots(figsize=figsize)
-	#ax.grid(False, axis='y')
-	ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+	ax.grid(False, axis='y')
 	ax.spines['right'].set_color('none')
 	ax.spines['top'].set_color('none')
-	#ax.spines['bottom'].set_color('none')
-	#ax.spines['left'].set_color('none')
+	ax.spines['bottom'].set_color('none')
+	ax.spines['left'].set_color('none')
 
 	bottom=optx['bottom'] if 'bottom' in optx else 0.3
 
 	#da.plot(ax=ax,kind=kind,position=position,width=width)
 
 	#xmax = da['changePercent'].max()
 	#ndg = max(int(math.log(xmax,10)/3),1)
@@ -470,36 +455,32 @@
 			#print(dh)            
 		else:
 			dh={}
 		if not isinstance(df,pd.DataFrame):
 			df = pd.DataFrame(data=df)
 		if fig is None:
 			plt.rcParams.update(plt.rcParamsDefault)            
-			if 'snsStyle' in optx:
-				sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-			else:
-				plt.style.use(optx.pop('pltStyle',"dark_background"))
+			sns.set_style("whitegrid",{'grid.linestyle':'--'})                 
 			fig, ax=plt.subplots(figsize=figsize)
 			fig.autofmt_xdate()
 			ax.yaxis.set_major_formatter(StrMethodFormatter('{x:,.0f}'))
 			plt.xlim(min_index-timedelta(minutes=5), x_lim+timedelta(minutes=5))
 			plt.ylim(min_ylim-(max_ylim-min_ylim)/2, max_ylim+(max_ylim-min_ylim)/5)
 			plt.subplots_adjust(bottom=0.2)
 			#plt.xlabel('Time',fontsize=15)
 			#plt.ylabel('price',fontsize=15)
 			#hours = mdates.HourLocator(interval = 1)
 			h_fmt = mdates.DateFormatter(x_fmt)
 			#ax.xaxis.set_major_locator(hours)
 			ax.xaxis.set_major_formatter(h_fmt)
-			#ax.grid(False, axis='x')                        
-			ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+			ax.grid(False, axis='x')                        
 			ax.spines['right'].set_color('none')
 			ax.spines['top'].set_color('none')
-			#ax.spines['bottom'].set_color('none')
-			#ax.spines['left'].set_color('none')
+			ax.spines['bottom'].set_color('none')
+			ax.spines['left'].set_color('none')
 			plt.title(title,fontproperties=fontProp(size=15))
 			plt.legend(frameon=False)            
 		plt.plot(df.index, df['close'])
 		plt.plot([min_index,x_lim],[xprice,xprice],'k--',lw=1)# plot open dash line
 		plt.plot([curr_num_date,curr_num_date],[xprice,curr_num],'k--',lw=1)# plot day pchg vertical line
 		#plt.annotate('{}%'.format(round((curr_num/open_num-1)*100,2)), xy=(curr_num_date,open_num+(curr_num-open_num)/2),xytext=(0,6),fontsize=10,annotation_clip=True, textcoords="offset points",ha=('left'), va='center') # plot pchg number        
 		plt.scatter(max_num_date,max_num,s=20,color = 'g',zorder = 19)#plot max point
@@ -552,28 +533,24 @@
 		return {},{},{}   
 	ticker = getKeyVal(optx,'ticker')
 	title  = getKeyVal(optx,'title','MarketCap')
 	sys.stderr.write(" --title: {}, ticker:{}\n".format(title,ticker))
 	if backend is not None:
 		plt.switch_backend(backend)
 	chartpath,chartname = gen_chartpath(**optx)
-	if 'snsStyle' in optx:
-		sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-	else:
-		plt.style.use(optx.pop('pltStyle',"dark_background"))
+	sns.set(style="whitegrid")
 
 	# define plot
 	if fig is None:
 		fig, ax = plt.subplots(figsize=figsize)
-	#ax.grid(False, axis='y')
-	ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+	ax.grid(False, axis='y')
 	ax.spines['right'].set_color('none')
 	ax.spines['top'].set_color('none')
-	#ax.spines['bottom'].set_color('none')
-	#ax.spines['left'].set_color('none')
+	ax.spines['bottom'].set_color('none')
+	ax.spines['left'].set_color('none')
 
 	bottom=optx['bottom'] if 'bottom' in optx else 0.3
 
 	#da.plot(ax=ax,kind=kind,position=position,width=width)
 
 	xmax = da['marketcap'].max()
 	ndg = max(int(math.log(xmax,10)/3),1)
@@ -605,18 +582,15 @@
 	if chartname is not None and len(chartname)>5:
 		plt.savefig(chartpath, format=chartformat)
 	elif backend is not None and backend.lower()=='tkagg': 
 		plt.show()
 	return chartpath,ax,fig
 
 def plot_peers_performance(df,fig=None,ax=None,figsize=(11,6),backend='Agg',title='',chartformat='svg',debugTF=False,**optx):
-	if 'snsStyle' in optx:
-		sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-	else:
-		plt.style.use(optx.pop('pltStyle',"dark_background"))
+	sns.set(style="whitegrid")
 	df['pchg']=df['pchg']*100
 	if 'ticker' in df and 'peRatio' in df:
 		df = pd.DataFrame(df.sort_values(by='peRatio').set_index('ticker',drop=True))
 	elif 'ticker' in df:
 		df = pd.DataFrame(df.set_index('ticker',drop=True))
 	ngrid = df.shape[1]
 	kind = getKeyVal(optx,'kind','barh')
@@ -697,28 +671,24 @@
 	'''
 	plot daily_peers by marketcap barh
 	'''
 	ticker = getKeyVal(optx,'ticker')
 	if backend is not None:
 		plt.switch_backend(backend)
 	chartpath,chartname = gen_chartpath(**optx)
-	if 'snsStyle' in optx:
-		sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-	else:
-		plt.style.use(optx.pop('pltStyle',"dark_background"))
+	sns.set(style="whitegrid")
 
 	# define plot
 	if fig is None:
 		fig, ax = plt.subplots(figsize=figsize)
-	#ax.grid(False, axis='x')
-	ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+	ax.grid(False, axis='x')
 	ax.spines['right'].set_color('none')
 	ax.spines['top'].set_color('none')
-	#ax.spines['bottom'].set_color('none')
-	#ax.spines['left'].set_color('none')
+	ax.spines['bottom'].set_color('none')
+	ax.spines['left'].set_color('none')
 
 	bottom=optx['bottom'] if 'bottom' in optx else 0.3
 	da['pbdate'] = da.index.astype(str)
 	da = da.sort_index(ascending=True)
 	#da.index = pd.to_datetime(da.index)    
 	#plt.ylim(,da['actualEPS'].max()*1.2)
 	plt.title('EPS')
@@ -799,25 +769,21 @@
 	bottom=optx['bottom'] if 'bottom' in optx else 0.35
 	chartpath,chartname = gen_chartpath(**optx)
 	try:
 		from _alan_pppscf import vertex_locator
 		if not isinstance(df,pd.DataFrame):
 			df = pd.DataFrame(data=df)
 		if fig is None:
-			if 'snsStyle' in optx:
-				sns.set_style(optx.pop('snsStyle',"whitegrid"),{'grid.linestyle':'--'})
-			else:
-				plt.style.use(optx.pop('pltStyle',"dark_background"))
+			sns.set_style("whitegrid",{'grid.linestyle':'--'})            
 			fig, ax=plt.subplots(figsize=figsize)
-			#ax.grid(False, axis='x')
-			ax.grid(optx.get('grid',True),linestyle='dotted',linewidth=0.5)
+			ax.grid(False, axis='x')
 			ax.spines['right'].set_color('none')
 			ax.spines['top'].set_color('none')
-			#ax.spines['bottom'].set_color('none')
-			#ax.spines['left'].set_color('none')            
+			ax.spines['bottom'].set_color('none')
+			ax.spines['left'].set_color('none')            
 		plt.plot(df.index,df.iloc[:,0])
 		plt.title(title,fontproperties=fontProp(size=30))
 		x_fmt = getKeyVal(optx,'x_fmt','') 
 		yunit=['','1,000','Million','Billion','Trillion']
 		ymax = abs(df.iloc[:,0]).max()
 		ndg = max(int(math.log(ymax,10)/3),1)
 		nadj = (ndg-1)*3
```

### Comparing `talan-0.1.4.3/talan/record_hilo.py` & `talan-0.1.4rc1/talan/record_hilo.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 record_hilo.py --extra_xs='nlookback=200' 'GC=F'
 OR
 record_hilo.py --extra_xs='nlookback=200' 'CNY=X'
 OR
 record_hilo.py --extra_xs='nlookback=200;colx="close";"' 'CNY=X'
 OR
 record_hilo.py --extra_xs='nlookback=200;colx="close";";mthLst=[-1,-3]' 'CNY=X'
-OR
-python3 -c "from record_hilo import get_titlehead as gt;d=gt(tablename='record_hilo');print(d)"
 '''
 
 import sys
 import numpy as np
 from _alan_calc import pull_stock_data as psd,getKeyVal,conn2mgdb
 from _alan_str import write2mdb,upsert_mdb
 from _alan_date import next_date,delta2dates
@@ -40,17 +38,14 @@
 		startDT=next_date(dx.index[-1],**nd_args)
 	ds = dx.loc[dx.index>=startDT,colx]
 	mnxTF,hilo,idxmnx = find_hilo(ds)
 	startAT=ds.index[0] # actual startDate in datetime
 	#sys.stderr.write("===Act:{}, Start:{}, Args:{}\n".format(startAT,startDT,nd_args))
 	return mnxTF,hilo,idxmnx,startDT,startAT
 
-def hilo(v):
-	return 1 if v[::-1].argmax()==0 else (-1 if v[::-1].argmin()==0 else 0)
-
 def find_hilo(ds):
 	'''
 	find hilo of pandas.Series 'ds'
 	'''
 	if len(ds)<1:
 		return False,ds.iloc[-1]>0,None
 	idxmnx=ds.index[-1]
@@ -226,17 +221,16 @@
 			jobj = funcArg(dx,endDT=xd,ticker=ticker,colx=colx,colLst=colLst,mthLst=mthLst)
 			if debugTF==True:
 				sys.stderr.write("{}\n".format(dx.iloc[-1]))
 			#if any([jobj['MTD'],jobj['YTD']]):
 			if jobj['YTD']:
 				sys.stderr.write("{}\n".format(jobj['YTD']))
 				if tablename is not None:
-					#zpk={"ticker","pbdate"}
-					zpk={"ticker"}
-					mobj,clientM,msg = upsert_mdb(jobj,clientM,tablename=tablename,zpk=zpk)
+					zpk={"ticker","pbdate"}
+					mobj,clientM,msg = write2mdb(jobj,clientM,tablename=tablename,zpk=zpk)
 		except Exception as e:
 			continue
 	return jobj
 
 def titlehead_tst(opts={},**optx):
 	ds = titlehead_backtest(opts,**optx)
 	sys.stderr.write( "ds:\n{}\n".format(ds.to_string()))
@@ -270,15 +264,14 @@
 	ds=[]
 	for lkbx in range(nlookback):
 		dm=[]
 		for jx in range(len(dLst)):
 			ticker,freq,src,label_cn,category_cn = dLst[['series','freq','source','label_cn','category_cn']].iloc[jx]
 			if freq != 'D':
 				continue
-			searchDB = (False if src=='yahoo' else True)
 			df = psd(ticker,days=days,src=src,debugTF=debugTF,pchgTF=True,searchDB=searchDB)
 			try:
 				dx = df.iloc[:-lkbx] if lkbx>0 else df
 				ret=recordHiLo2(dx,ticker=ticker)
 				if len(ret['YTD'])>0:
 					dd=dLst.iloc[jx].to_dict()
 					dd.update(ret['YTD'])
@@ -299,16 +292,15 @@
 				sys.stderr.write("**ERROR:{}:{}:{}\n".format(jx,ticker,str(e)))
 				continue
 		if len(dm)<1:	
 			continue
 		dm = pd.DataFrame(dm)
 		ds = dm.sort_values(by=['days','category_seq','category_label_seq'],ascending =[False,True,True])
 		if tablename is not None:
-			#zpk={"ticker","pbdate"}
-			zpk={"ticker"}
+			zpk={"ticker","pbdate"}
 			sys.stderr.write("Save to {}:\n{}\n".format(tablename,dm))
 			mobj,clientM,msg = upsert_mdb(dm,tablename=tablename,dbname=dbname,zpk=zpk)
 	return ds
 
 if __name__ == '__main__':
 	description="""Find record high/low returns, e.g., record_hilo.py SPY --extra_xs=nlookback=100"""
 	fx = lambda ky,va,m: m[ky] if ky in m and m[ky] in globals() else va
```

### Comparing `talan-0.1.4.3/talan/talan_wrap.py` & `talan-0.1.4rc1/talan/talan_wrap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import sys,os
 sys.path.append(os.path.dirname(__file__))
 from _alan_calc import *
 from _alan_date import *
 from _alan_str import *
 from _alan_pppscf import batch_pppscf,vertex_locator,vertex_mnmx
 from yh_chart import *
-from webReader import webReader,streamReader, yhReader
 from yh_hist_batch import *
 from yh_predefined import bb_predefined
 from find_recent_eps import find_recent_eps
 from headline_calc import find_hiloRecord,headline_calc
 from headline_sts import headline_hist
 from iex_peers import iex_peers,peers_performance,ticker2sectorRanking
 from macro_event_yh import run_macro_event_yh
 from plot_templates import plot_templates
 from record_hilo import get_titlehead
 from ticker2label import ticker2label,t2l
-from get_rq import get_rq,prn_df
+from webReader import webReader,streamReader,yhReader
+from fredReader import fredReader
 import types
 unLst=['popen','Call','OLD','TBD','_DEPRECATED','Popen','__']
 talan_vars = {k:v for (k,v) in globals().items() if callable(v) and not any(map(k.__contains__,unLst)) and isinstance(v,types.FunctionType) and v.__doc__} 
 for k in ['unLst']:
 	globals().pop(k,None)
```

### Comparing `talan-0.1.4.3/talan/theme_list.py` & `talan-0.1.4rc1/talan/theme_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
 def add_sector_industry(df=[]):
 	from yh_chart import runOTF
 	from _alan_calc import subDict
 	if len(df)<1:
 		return []
 	tkLst=df['ticker'].values
-	datax=runOTF(list(df['ticker'].values),'yh_financials',modules="summaryProfile",dbname='ara',tablename="yh_summaryProfile",zpk={'ticker'},deltaTolerance=8640000)
+	datax=runOTF('yh_financials',list(df['ticker'].values),modules="summaryProfile",dbname='ara',tablename="yh_summaryProfile",zpk={'ticker'},deltaTolerance=8640000)
 	if len(datax)<1:
 		return df
 	dg =  subDict(pd.DataFrame(datax),['ticker','sector','industry'])
 	df = df.merge(dg,on='ticker',how='left')
 	return df
 
 def nasdaq_ipos(hostname='localhost',dbname='ara',tablename='nasdaq_ipos',tab='filing',month='',debugTF=False,**kwargs):
```

### Comparing `talan-0.1.4.3/talan/ticker2label.py` & `talan-0.1.4rc1/talan/ticker2label.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3.8
+#!/usr/bin/env python3
 ''' get basic info from a list of tickers 'tkLst'
 required tables:
   mapping_ticker_cik (pgDB)
   spdr_sector
   sector_alias_industry
   yh_curr_quote
   yh_summaryProfile
@@ -20,26 +20,26 @@
 if sys.version_info.major == 2:
 	reload(sys)
 	sys.setdefaultencoding('utf8')
 
 def tk2infoM(ticker='',tablename='yh_curr_quote',colx='ticker',dbname='ara',clientM=None,**optx):
 	from yh_chart import runOTF,yh_financials,yh_quote_comparison;
 	from _alan_str import find_mdb
-	funcN,zpk,deltaTolerance=getKeyVal(optx,["funcN","zpk","deltaTolerance"],['yh_financials',{'ticker'},1800])
+	funcArg,zpk,deltaTolerance=getKeyVal(optx,["funcArg","zpk","deltaTolerance"],['yh_financials',{'ticker'},1800])
 	modules = optx.pop('modules','')
 	jobj = {colx:ticker}
 	df=[]
 	try:
 		df=find_mdb(jobj,clientM=clientM,dbname=dbname,tablename=tablename,dfTF=True)[0]
 		if len(df)>0 and isinstance(df,pd.DataFrame):
 			sys.stderr.write(" --{} found in {}:\n{}\n".format(ticker,tablename,df)[:100]+"\n")
 			return df
 		else:
-			datax=runOTF(ticker,funcN,deltaTolerance=deltaTolerance,modules=modules,dbname=dbname,tablename=tablename,zpk=zpk)
-			#datax=locals()[funcN](ticker,deltaTolerance=deltaTolerance,modules=modules,dbname=dbname,tablename=tablename,zpk=zpk)
+			datax=runOTF(funcArg,ticker,deltaTolerance=deltaTolerance,modules=modules,dbname=dbname,tablename=tablename,zpk=zpk)
+			#datax=locals()[funcArg](ticker,deltaTolerance=deltaTolerance,modules=modules,dbname=dbname,tablename=tablename,zpk=zpk)
 			if len(datax)<1:
 				sys.stderr.write(" --{} not found via {} @{}\n".format(ticker,modules,'tk2infoM'))
 				return []
 			df= pd.DataFrame(datax)
 			sys.stderr.write(" --{} found in {}:\n{}\n".format(ticker,modules,df)[:100]+"\n")
 			return df
 	except:
@@ -56,21 +56,21 @@
 	sys.stderr.write(" --find {} from SQL:\n{}\n".format(ticker,xqr))
 	df= sqlQuery(xqr,engine=pgDB)
 	if len(df)>0 and isinstance(df,pd.DataFrame):
 		return df
 	else:
 		return []
        
-def en2cn(e='Metropolitan Bank Holding Corp'):
+def en2cnOLD(e='Metropolitan Bank Holding Corp'):
 	from googletrans import Translator
 	c = Translator().translate(e,src='en',dest='zh-tw')
 	sys.stderr.write(" --Translate: {} -> {}\n".format(e,c.text))
 	return c.text
 
-def en2cnOLD(e='Metropolitan Bank Holding Corp',src='en',dest='zh-TW'):
+def en2cn(e='Metropolitan Bank Holding Corp',src='en',dest='zh-TW'):
 	from google_trans_new import google_translator as Translator
 	import html
 	dscr =html.unescape(e)
 	dscr = str(dscr.strip()+"\n")
 	if len(dscr)<1:
 		return dscr
 	try:
@@ -104,15 +104,15 @@
 def t2l(ticker='',output='dict',quoteTF=True,dbname='ara'):
 	''' get basic info from ticker
 	'''
 	if isinstance(ticker,list):
 		return batch_t2l(tkLst=ticker,output=output,quoteTF=quoteTF,dbname=dbname)
 
 	#- GET summaryProfile from mDB:yh_summaryProfile or onTheFly
-	dg = tk2infoM(ticker,tablename="yh_summaryProfile",funcN='yh_financials',modules="summaryProfile",zpk={'ticker'},deltaTolerance=864000)
+	dg = tk2infoM(ticker,tablename="yh_summaryProfile",funcArg='yh_financials',modules="summaryProfile",zpk={'ticker'},deltaTolerance=864000)
 	dg = renameDict(dg,{"sector":"sector_alias"})
 
 	#- GET basic ticker info from pgDB:mapping_ticker_cik 
 	pgDB = conn2pgdb(dbname=dbname)
 	df = tk2info(ticker,tablename='mapping_ticker_cik',pgDB=pgDB)
 	if all([len(df),len(dg)]):
 		df = df.merge(dg,on='ticker')
@@ -144,15 +144,15 @@
 		dg = tk2info(df['industry'].values[0],tablename='sector_alias_industry',colx='industry',pgDB=pgDB)
 		if len(dg):
 			df = df.merge(dg[['industry','industry_cn']],on='industry')
 		else:
 			df['industry_cn'] = df['industry'].values
 
 	#- GET summaryProfile from mDB:yh_quote_curr or onTheFly
-	dg = tk2infoM(ticker,tablename='yh_quote_curr',funcN='yh_quote_comparison',zpk={'ticker'},deltaTolerance=900)
+	dg = tk2infoM(ticker,tablename='yh_quote_curr',funcArg='yh_quote_comparison',zpk={'ticker'},deltaTolerance=900)
 	if all([len(df),len(dg)]):
 		df = df.merge(dg,on='ticker')
 		if 'trailingPE' in df:
 			df['peRatio']=df['trailingPE']
 	elif len(dg)>0:
 		df=dg
```

### Comparing `talan-0.1.4.3/talan/ticker_mapping.py` & `talan-0.1.4rc1/talan/ticker_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 '''
-DEPRECATED, use ticker2cik.py for sec.gov edgar related info
 Get [CIK,SIC,Company] info from [TICKER] via
 http://www.sec.gov/cgi-bin/browse-edgar?CIK={ticker}&Find=Search&owner=exclude&action=getcompany&output=atom
 Get GIC [Sector] via
 https://query2.finance.yahoo.com/v11/finance/quoteSummary/{ticker}?modules=summaryProfile'
 Convert chinese [company_cn] via tencent site: http://qt.gtimg.cn/q=usAAPL
 http://qt.gtimg.cn/q=us{ticker}
```

### Comparing `talan-0.1.4.3/talan/upd_mapping_ticker.py` & `talan-0.1.4rc1/talan/upd_mapping_ticker.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.3/talan/webReader.py` & `talan-0.1.4rc1/talan/webReader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,57 @@
 #!/usr/bin/env python3
 '''Read data from WEB via `requests` [GET|POST] method
 Usage of,
-./webReader.py URL [JSON]
-OR
-./webReader.py AAPL 'dict(funcName="yhReader")'
-
-Where:
-JSON default value:
-{ "funcName":"webReader",
-  "opts": { "rtype":"json", "method":"get" }
-}
+./webReader.py URL [JSON] [RTYPE] [METHOD]
 
 Example,
 #----- To read web data from FRED
 ./webReader.py 'https://api.stlouisfed.org/fred/series/observations?file_type=json&series_id=CPIAUCNS' $(cat ~/.fredapi.json)
 #----- OR 
 api_key=$(jq ".api_key" ~/.fredapi.json)
 ./webReader.py 'https://api.stlouisfed.org/fred/series/observations?' '{"api_key":'\"${api_key}\"',"file_type":"json","series_id":"CPIAUCNS","observation_start":"2022-07-01"}'
 #----- OR to read web data from yahoo-finance
-./webReader.py 'https://query2.finance.yahoo.com/v7/finance/spark?range=1d&interval=30m&indicators=close&includeTimestamps=false&includePrePost=false&corsDomain=finance.yahoo.com&.tsrc=finance' '{"symbols":"AAPL,IBM"}'
+./webReader.py 'https://query1.finance.yahoo.com/v7/finance/spark?range=1d&interval=30m&indicators=close&includeTimestamps=false&includePrePost=false&corsDomain=finance.yahoo.com&.tsrc=finance' '{"symbols":"AAPL,IBM"}'
 #----- OR 
-./webReader.py 'https://query2.finance.yahoo.com/v7/finance/spark' '{"symbols":"AAPL","range":"1d","interval":"60m"}'
+./webReader.py 'https://query1.finance.yahoo.com/v7/finance/spark' '{"symbols":"AAPL","range":"1d","interval":"60m"}'
 #----- OR to load a streaming file 
 ./webReader.py http://api1.beyondbond.com/downloads/grimm10-49_1.png {} stream get "${user},${pswd}"
-#----- OR to load stock spark prices 
-./webReader.py AAPL,TSM 'dict(funcName="yhReader")'
 #----- OR 
 python3 -c "from webReader import yhReader;df=yhReader(['AAPL','AMD'],types='spark');print(df)"
 #----- OR 
 python3 -c "from webReader import yhReader;df=yhReader(['AAPL','AMD'],types='chart');print(df)"
-#----- OR 
-python3 -c "from webReader import yhReader;df=yhReader(['AAPL','AMD'],types='quote');print(df)"
 
 Last Mod.,
-Sun 02 Jul 2023 06:52:03 PM EDT
+Tue 11 Oct 2022 10:40:10 PM EDT
 '''
-__usage__='\n'.join(__doc__.split('\n')[:11])
 import sys
 import requests
 from requests.auth import HTTPBasicAuth as HA
 import pandas as pd
 
-headers={'Content-Type': 'text/html', 'Accept': 'application/json', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36'}
-
-credentials={}
-
-apiBase = 'https://query2.finance.yahoo.com'
-
-def getCredentials(cookieUrl='https://fc.yahoo.com', crumbUrl=apiBase+'/v1/test/getcrumb'):
-	cookies = requests.get(cookieUrl).cookies
-	crumb = requests.get(url=crumbUrl, cookies=cookies, headers=headers).text
-	return {'cookies': cookies, 'crumb': crumb}
+hds={'Content-Type': 'text/html', 'Accept': 'application/json', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36'}
 
 def chart_json2df(res):
 	jx=res["chart"]["result"][0]
-	ticker=jx["meta"]["symbol"]
 	epoch=jx["timestamp"]
-	dlst=jx["indicators"]["quote"][0]
-	dlst.update(epoch=jx["timestamp"])
+	close=jx["indicators"]["quote"][0]["close"]
+	if "open" in jx["indicators"]["quote"][0]:
+		open=jx["indicators"]["quote"][0]["open"]
+	if "high" in jx["indicators"]["quote"][0]:
+		high=jx["indicators"]["quote"][0]["high"]
+	if "low" in jx["indicators"]["quote"][0]:
+		low=jx["indicators"]["quote"][0]["low"]
+	if "volume" in jx["indicators"]["quote"][0]:
+		volume=jx["indicators"]["quote"][0]["volume"]
+	ticker=jx["meta"]["symbol"]
 	if "adjclose" in jx["indicators"]:
 		adjusted=jx["indicators"]["adjclose"][0]["adjclose"]
 	else:
-		adjusted=dlst["close"]
-	dlst.update(epoch=epoch,adjusted=adjusted)
-	dx=pd.DataFrame(data=dlst)
-	dx['ticker']=ticker
+		adjusted=close
+	dx=pd.DataFrame(data=dict(epoch=epoch,close=close,open=open,high=high,low=low,volume=volume,adjusted=adjusted,ticker=ticker))
 	dx.set_index(pd.DatetimeIndex(dx['epoch'].apply(pd.Timestamp.fromtimestamp)),inplace=True)
 	return dx
 
 def spark_json2df(res):
 	jlst=res["spark"]["result"]
 	df=pd.DataFrame()	
 	for jx in jlst:
@@ -80,167 +63,116 @@
 		df = pd.concat([df,dx])
 	df.index.name="DATE"
 	df=df.drop(["epoch"],axis=1)
 	df["pbdate"]=pd.Series((df.index)).apply(lambda x: pd.Timestamp.strftime(x,"%Y%m%d")).values
 	return df
 
 def yh_chart(tkLst=['AAPL'],debugTF=False,**opts):
-	if debugTF:
-		sys.stderr.write("==yh_chart inputs:{}\n".format(locals()))
-	urx="https://query2.finance.yahoo.com/v8/finance/chart/{}"
-	parat=dict(interval='1d',range='7d')
-	pLst=['interval','range','fields','period1','period2','includeAdjustedClose']
-	parax={k:v for k,v in opts.items() if k in pLst}
-	parat.update(parax)
+	urx="https://query1.finance.yahoo.com/v8/finance/chart/{}"
+	param=dict(interval='1d',range='7d')
+	pLst=['interval','range','fields','period1','period2']
+	data={k:v for k,v in opts.items() if k in pLst}
+	param.update(data)
 	df=pd.DataFrame()	
 	for tx in tkLst:
 		url=urx.format(tx)
-		res=webReader(url,pjson=parat,debugTF=debugTF,**opts)
+		res=webReader(url,data=param,debugTF=debugTF,**opts)
 		dx = chart_json2df(res)
 		df = pd.concat([df,dx])
 	df.index.name="DATE"
 	df=df.drop(["epoch"],axis=1)
 	df["pbdate"]=pd.Series((df.index)).apply(lambda x: pd.Timestamp.strftime(x,"%Y%m%d")).values
-	if parat.get('interval','')[-1:]=="m":
-		df["epochs"]=pd.Series((df.index)).apply(lambda x: pd.Timestamp.strftime(x,"%s000")).values
-	if not opts.get('dfTF',False):
-		return df.to_dict(orient='records')
 	return df
 
 def yh_spark(tkLst=['AAPL'],debugTF=False,**opts):
-	if debugTF:
-		sys.stderr.write("==yh_spark inputs:{}\n".format(locals()))
-	url="https://query2.finance.yahoo.com/v7/finance/spark?"
-	parat=dict(symbols=",".join(tkLst),interval='1d',range='7d')
-	pLst=['symbols','interval','range','fields','indicators','period1','period2']
-	parax={k:v for k,v in opts.items() if k in pLst}
-	parat.update(parax)
-	res=webReader(url,pjson=parat,debugTF=debugTF,**opts)
+	url="https://query1.finance.yahoo.com/v7/finance/spark?"
+	param=dict(symbols=",".join(tkLst),interval='1d',range='7d')
+	pLst=['symbols','interval','range','fields','period1','period2']
+	data={k:v for k,v in opts.items() if k in pLst}
+	param.update(data)
+	res=webReader(url,data=param,debugTF=debugTF,**opts)
 	df=spark_json2df(res)
-	if parat.get('interval','')[-1:]=="m":
-		df["epochs"]=pd.Series((df.index)).apply(lambda x: pd.Timestamp.strftime(x,"%s000")).values
 	return df
 
 def yh_quote(tkLst=['AAPL'],debugTF=False,**opts):
-	if debugTF:
-		sys.stderr.write("==yh_quote inputs:{}\n".format(locals()))
-	url="https://query2.finance.yahoo.com/v7/finance/quote?"
-	parat=dict(symbols=",".join(tkLst))
-	pLst=['symbols','fields','formatted']
-	parax={k:v for k,v in opts.items() if k in pLst}
-	parat.update(parax)
-	res=webReader(url,pjson=parat,debugTF=debugTF,**opts)
+	url="https://query1.finance.yahoo.com/v7/finance/quote?"
+	param=dict(symbols=",".join(tkLst))
+	res=webReader(url,data=param,debugTF=debugTF,**opts)
 	jlst=res["quoteResponse"]["result"]
-	if opts.get('dfTF',False):
-		return pd.DataFrame(jlst)
-	else:
-		return jlst
+	return pd.DataFrame(jlst)
 
-def yhReader(tkLst,types='spark',debugTF=False,**opts):
-	if isinstance(tkLst,str):
-		tkLst=tkLst.split(',')
+def yhReader(tkLst=['AAPL'],types='spark',debugTF=False,**opts):
 	typ=types.lower()
 	if typ =='chart':
 		return yh_chart(tkLst=tkLst,debugTF=debugTF,**opts)
 	elif typ =='spark':
 		return yh_spark(tkLst=tkLst,debugTF=debugTF,**opts)
 	elif typ =='quote':
 		return yh_quote(tkLst=tkLst,debugTF=debugTF,**opts)
 	return {}
 
-def webReader(url,pjson={},rtype='json',method='get',sessionTF=True,debugTF=False,**opts):
-	global credentials
+def webReader(url,data=None,rtype='json',method='get',headers=hds,sessionTF=True,user='',pswd='',**opts):
 	if not url:
 		return {}
-	user, pswd = [opts.pop(x,'') for x in ['user','pswd'] ]
-	if debugTF:
-		sys.stderr.write("==webReader inputs:{}\n".format(locals()))
 	rq = requests.Session() if sessionTF else requests
 	rqOpts={}
-	if 'quote' in url and 'quoteS' not in url:
-		if not credentials:
-			credentials=getCredentials()
-		crumb,cookies = (credentials['crumb'],credentials['cookies'])
-		pjson.update(crumb=crumb)
-		rqOpts.update(cookies=cookies)
 	if (user and pswd):
 		rqOpts.update(auth=HA(user,pswd))
-	if debugTF:
-		sys.stderr.write(" --requests URL:{}\n --params:{}\n --rqOpts:{}\n".format(url,pjson,rqOpts))
 	if method.lower()=='post':
-		ret = rq.post(url,data=pjson,headers=headers,**rqOpts)
+		ret = rq.post(url,data=data,headers=headers,**rqOpts)
 	else:
-		ret = rq.get(url,params=pjson,headers=headers,**rqOpts)
+		ret = rq.get(url,params=data,headers=headers,**rqOpts)
 	res = ret.json() if rtype.lower()=='json' else ret.text
 	return res
 	
-def streamReader(url,pjson={},rtype='json',method='get',sessionTF=True,debugTF=False,**opts):
+def streamReader(url,data=None,rtype='json',method='get',headers=hds,sessionTF=True,stream=True,filepath='',user='',pswd='',**opts):
 	from urllib.parse import urlparse
 	import shutil
 	if not url:
 		return {}
-	stream = opts.pop('stream',True)
-	user, pswd,filepath = [opts.pop(x,'') for x in ['user','pswd','filepath'] ]
-	if debugTF:
-		sys.stderr.write("==streamReader inputs:{}\n".format(locals()))
 	if not filepath:
 		o=urlparse(url)
 		filepath=o.path.split('/')[-1]
 	rq = requests.Session() if sessionTF else requests
 	rqOpts={}
 	if stream:
 		rqOpts.update(stream=stream)
 	if (user and pswd):
 		rqOpts.update(auth=HA(user,pswd))
-	if debugTF:
-		sys.stderr.write(" --requests URL:{}\n --params:{}\n --rqOpts:{}\n".format(url,pjson,rqOpts))
 	if method.lower()=='post':
-		ret = rq.post(url,data=pjson,headers=headers,**rqOpts)
+		ret = rq.post(url,data=data,headers=headers,**rqOpts)
 	else:
-		ret = rq.get(url,params=pjson,headers=headers,**rqOpts)
+		ret = rq.get(url,params=data,headers=headers,**rqOpts)
 	if ret.status_code == 200:
 		with open(filepath, 'wb') as f:
 			ret.raw.decode_content = True
 			shutil.copyfileobj(ret.raw, f)  
 	else:
 		print(ret.status_code,ret.raise_for_status(),file=sys.stderr)
 	del ret
 	return filepath
 	
-def mainTst():
-	pjson={}
+if __name__ == '__main__' :
+	import json;
 	argc=len(sys.argv)
 	if argc>1:
 		url = sys.argv[1]
 	else:
-		sys.exit(__usage__)
+		sys.stderr.write(__doc__)
+		exit(1)
 	try:
-		pjson=eval(sys.argv[2]) if sys.argv[2:] else {}
+		print(sys.argv[2])
+		data   = json.loads(sys.argv[2]) if argc>2 else None
 	except Exception as e:
-		sys.stderr.write("**ERROR: Invalid JSON, {}\n".format(e))
-	opts = pjson.pop('opts',{})
-	funcName = pjson.pop('funcName','webReader')
-	if funcName in globals() and hasattr(globals()[funcName],'__call__'):
-		funcArg=globals()[funcName]
+		sys.stderr.write("**ERROR: {}\n".format(e))
+		data   = None
+	rtype = sys.argv[3] if argc>3 else 'json'
+	method = sys.argv[4] if argc>4 else 'get'
+	user,pswd = (sys.argv[5] if argc>5 else ',').split(',')
+	if rtype == 'stream':	
+		res=streamReader(url,data=data,method=method,rtype=rtype,user=user,pswd=pswd)
 	else:
-		sys.stderr.write("**WARNINGS: Invalid function:{}\n".format(funcName))
-		sys.exit(__usage__)
-
-	if funcArg in [streamReader,webReader]:
-		res=funcArg(url,pjson=pjson,**opts)
+		res=webReader(url,data=data,method=method,rtype=rtype,user=user,pswd=pswd)
 		if 'spark' in url:
-			res = spark_json2df(res)
-		elif 'chart' in url:
-			res = chart_json2df(res)
-	else:
-		if opts:
-			pjson.update(opts)
-		res=funcArg(url,**pjson)
-	return res
-
-if __name__ == '__main__' :
-	try:
-		sys.exit(mainTst())
-	except Exception as e:
-		sys.stderr.write("**ERROR: mainTst {}\n".format(e))
-		sys.exit(__usage__)
-
+			df = spark_json2df(res)
+			print(df)
+	print(res,file=sys.stderr)
```

### Comparing `talan-0.1.4.3/talan/yh_chart.py` & `talan-0.1.4rc1/talan/yh_chart.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python3
-'''Stock feed from yahoo finance
-Usage of,
-./yh_chart.py TICKER[,TICKER2, ...] [JSON]
-Example,
-./yh_chart.py IBM,AAPL --no_database_save
-OR
-./yh_chart.py AAPL,IBM '{"types":"spark","dfTF":True,"saveDB":False}' --funcname=yh_spark_hist
--------------------------------------------
+''' Live datafeed from yahoo quotes
 Update tables:
 mDB: ara::yh_spark_hist, ara::yh_quote_curr
 pgDB: ara::yh_quote_curr (isEoD=True)
 
+Usage of:
++ From commandline: 
+python3 yh_chart.py IBM,AAPL
+python3 yh_chart.py IBM AAPL
+echo "IBM AAPL" | python3 yh_chart.py -
 
 #-------------------------------------------------------------------------
 + For a list of tickers 'tkLst' with direct function call for pricing data
   -- To run Intraday for yh_spark_hist (CRON every 15 minutes 930-1600 M-F)
 python3 -c "from yh_chart import yh_spark_hist as ysh;ysh(ranged='15m',interval='5m',debugTF=True)"
   -- To run EoD yh_quote_curr and yh_spark_hist (CRON at 1600 M-F)
 python3 -c "from yh_chart import yh_spark_hist as ysh;ysh(types='quote',isEoD=True,debugTF=True)"
@@ -22,36 +20,36 @@
 python3 -c "from yh_chart import yh_spark_hist as ysh;ysh(types='quote',debugTF=True)"
   -- To run intraday yh_quote_market
 printf "^GSPC ^IXIC ^DJI ^SOX" | python3 -c "import sys;from yh_chart import yh_spark_hist as ysh;ysh(sys.stdin.read().split(),t2='market_indicator_quote',types='quote',debugTF=True)"
 
 #-------------------------------------------------------------------------
 + For specific 'ticker' of either non-existed ticker or if not updated in the last 'deltaTolerance' seconds
   -- To setup onTheFly stock quote for non-existed ticker or if not updated in the last 'deltaTolerance' seconds
-python3 -c "ticker='AAPL';from yh_chart import yh_quote_comparison as yqc, runOTF;ret=runOTF(ticker,yqc,deltaTolerance=3600,tablename='yh_quote_curr',zpk=['ticker']);"
+python3 -c "ticker='AAPL';from yh_chart import yh_quote_comparison as yqc, runOTF;ret=runOTF(yqc,ticker,deltaTolerance=3600,tablename='yh_quote_curr',zpk=['ticker']);"
   -- To setup onTheFly stock intra-day spark history for non-existed ticker or if not updated in the last 'deltaTolerance' seconds
-python3 -c "tkLst='AAPL';from yh_chart import yh_spark_hist as ysh, runOTF;ret=runOTF(ticker,ysh,deltaTolerance=900,tablename='yh_spark_hist',zpk=['ticker','pbdt'],ranged='15m',interval='5m',debugTF=True,dbname='test');"
+python3 -c "tkLst='AAPL';from yh_chart import yh_spark_hist as ysh, runOTF;ret=runOTF(ysh,ticker,deltaTolerance=900,tablename='yh_spark_hist',zpk=['ticker','pbdt'],ranged='15m',interval='5m',debugTF=True,dbname='test');"
   -- To setup onTheFly financials 'modules' for non-existed ticker or if not updated in the last 'deltaTolerance' seconds (86400 for 1-day)
-python3 -c "ticker='AAPL';from yh_chart import runOTF, yh_financials as yh;ret=runOTF(ticker,yh,deltaTolerance=86400,modules='incomeStatementHistoryQuarterly',tablename='yh_financials',dbname='yh',zpkChk=['ticker','module'],zpk=['ticker','module','pbdate']);"
+python3 -c "ticker='AAPL';from yh_chart import runOTF, yh_financials as yh;ret=runOTF(yh,ticker,deltaTolerance=86400,modules='incomeStatementHistoryQuarterly',tablename='yh_financials',dbname='yh',zpkChk=['ticker','module'],zpk=['ticker','module','pbdate']);"
   -- To setup onTheFly stock intra-day chart history for non-existed ticker or if not updated in the last 'deltaTolerance' seconds (TBD)
-python3 -c "tkLst='AAPL';from yh_chart import yh_spark_hist as ysh, runOTF;ret=runOTF(ticker,ysh,deltaTolerance=900,types='chart',tablename='yh_chart_hist',zpk=['ticker','pbdt'],ranged='15m',interval='5m',debugTF=True,dbname='ara');"
+python3 -c "tkLst='AAPL';from yh_chart import yh_spark_hist as ysh, runOTF;ret=runOTF(ysh,ticker,deltaTolerance=900,types='chart',tablename='yh_chart_hist',zpk=['ticker','pbdt'],ranged='15m',interval='5m',debugTF=True,dbname='ara');"
 
 #-------------------------------------------------------------------------
 + From Direct function call for financial keyStatistics
 python3 -c "from yh_chart import qS_keyStatistics as yks;yks(saveDB=True,debugTF=True)"
   -- To run Quarterly income_statement
-python3 -c "from yh_chart import yh_financialsubatch as yf;yf(modules='incomeStatementHistoryQuarterly',tablename='yh_IS_Q',zpk={'ticker','pbdate'});"
+python3 -c "from yh_chart import yh_financials_batch as yf;yf(modules='incomeStatementHistoryQuarterly',tablename='yh_IS_Q',zpk={'ticker','pbdate'});"
 python3 -c "from yh_chart import yh_financials_batch as yf;yf(modules='incomeStatementHistoryQuarterly',tablename='yh_IS_Q',zpk={'ticker','pbdate'},useDB=True);"
   -- To run Annual income_statement
 python3 -c "from yh_chart import yh_financials_batch as yf;yf(modules='incomeStatementHistory',tablename='yh_IS_A',zpk={'ticker','pbdate'});"
 + NOTE:
   -- below 3 calls are equivalent (1st one perferred, see onTheFlyDB_tst for better reference)
-python3 -c "ticker='DAL';from yh_chart import runOTF, yh_financials as yh;ret=runOTF(ticker,yh,deltaTolerance=86400,modules='incomeStatementHistoryQuarterly',tablename='yh_financials',dbname='yh',zpkChk=['ticker','module'],zpk=['ticker','module','pbdate']);"
+python3 -c "ticker='DAL';from yh_chart import runOTF, yh_financials as yh;ret=runOTF(yh,ticker,deltaTolerance=86400,modules='incomeStatementHistoryQuarterly',tablename='yh_financials',dbname='yh',zpkChk=['ticker','module'],zpk=['ticker','module','pbdate']);"
 python3 -c "tkLst=['DAL'];from yh_chart import func2mdb as yhb;dd=yhb(tkLst,dbname='test',tablename='test1',funcN='yh_batchTypes',zpk={'ticker','pbdate'},types='quoteSummary',modules='incomeStatementHistoryQuarterly',debugTF=True);print(dd)"
 python3 -c "tkLst=['DAL'];from yh_chart import yh_financials_batch as yf;yf(tkLst,modules='incomeStatementHistory',dbname='test',tablename='test1',zpk={'ticker','module','pbdate'});"
-python3 -c "ticker=['AAPL','DAL'];from yh_chart import runOTF, yh_financials as yf;ret=runOTF(ticker,yf,deltaTolerance=86400*90,modules='"summaryProfile"',tablename='"yh_summaryProfile"',dbname='ara',zpkChk=['ticker','module'],zpk=['ticker','module','pbdate']);"
+python3 -c "ticker=['AAPL','DAL'];from yh_chart import runOTF, yh_financials as yf;ret=runOTF(yf,ticker,deltaTolerance=86400*90,modules='"summaryProfile"',tablename='"yh_summaryProfile"',dbname='ara',zpkChk=['ticker','module'],zpk=['ticker','module','pbdate']);"
 
   -- To run summaryProfile  and save to MDB: yh_summaryProfile table
 python3 -c "tkLst=['SHAK'];from yh_chart import func2mdb as yhb;dd=yhb(tkLst,tablename='yh_summaryProfile',funcN='yh_batchTypes',zpk=['ticker'],types='quoteSummary',modules='summaryProfile',debugTF=True);print(dd)"
 
   -- To run summaryProfile and show output
 python3 -c "tkLst=['SHAK'];from yh_chart import yh_batchTypes as yhb;dd=yhb(tkLst,types='quoteSummary',modules='summaryProfile',debugTF=True);print(dd)"
   -- To run defaultKeyStatistics and show output
@@ -64,34 +62,24 @@
 python3 -c "from yh_chart import func2mdb as yhq; yhq(['XLRE'],tablename='yh_quote_curr',dbname='ara',funcN='yh_quote_comparison',zpk={'ticker'});"
 python3 -c "from yh_chart import yh_hist_query as yhq;d=yhq(['AAPL'],types='spark');print(d)"
 python3 -c "from yh_chart import yh_hist_query as yhq;d=yhq(['AAPL'],types='quote');print(d)"
 python3 -c "from yh_chart import yh_quote_comparison as yqc;print(yqc(['AAPL']))"
 
 Last mod.,
 Wed May 27 10:20:54 EDT 2020
-----------------------------------------------------------------------------------------
+-----------------------------------------------------------------------------------------------------
 '''
-__usage__='\n'.join(__doc__.split('\n')[:8])
-import sys, datetime, re
+import sys, datetime
 import requests
 import numpy as np
 import pandas as pd
 from pandas.io.json import json_normalize
 from _alan_str import write2mdb,find_mdb,insert_mdb,upsert_mdb,get_arg2func
 from _alan_calc import getKeyVal,conn2pgdb,conn2mgdb,renameDict,subDict,subDF,saferun,safeRunArg
-
 headers={'Content-Type': 'text/html', 'Accept': 'application/json', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36'}
-credentials={}
-apiBase = 'https://query2.finance.yahoo.com'
-
-def getCredentials(cookieUrl='https://fc.yahoo.com', crumbUrl=apiBase+'/v1/test/getcrumb'):
-	cookies = requests.get(cookieUrl).cookies
-	crumb = requests.get(url=crumbUrl, cookies=cookies, headers=headers).text
-	return {'cookies': cookies, 'crumb': crumb}
-
 
 def epoch_parser(x,s=1000): return datetime.datetime.fromtimestamp(int(x/s))
 
 def pull_act_tickers(sql=None,engine=None):
 	if not sql:
 		sql="select ticker from mapping_ticker_cik where act_code=1 ORDER BY ticker"
 	try:
@@ -105,50 +93,43 @@
 	''' partition an array 'v' into arrays limit to 'n' elements
 	'''
 	import numpy as np
 	return [v[i:i+max(1,n)] for i in np.arange(0, len(v), n)]
 
 
 def yh_spark_hist(tkLst=None,**optx):
-	debugTF=optx.get('debugTF',False)
-	if debugTF:
-		sys.stderr.write("===optx in yh_spark_hist():\n{}\n".format(optx))
+	sys.stderr.write("++yh_spark_hist():optx: {}\n".format(optx))
 	dd = yh_batchSpark(tkLst=tkLst,**optx)
 	if optx.pop('dfTF',False) and not isinstance(dd,pd.DataFrame):
 		dd = pd.DataFrame(dd)
 	if optx.pop('tsTF',False) and isinstance(dd,pd.DataFrame) and \
 		not isinstance(dd.index,(datetime.date, datetime.datetime)):
 		if 'pbdt' in dd.columns:
 			dd.set_index('pbdt',drop=True,inplace=True)
 		elif 'epochs' in dd.columns:
 			pbdt = np.vectorize(epoch_parser)(dd['epochs'])
 			dd.set_index(pd.DatetimeIndex(pbdt),inplace=True)
 		dd.index.name='date'
-	if debugTF:
-		sys.stderr.write("===END yh_spark_hist():\n{}".format(dd)[:256]+" ...\n")
 	return dd
 
 def useWeb(jobj={'ticker':'^GSPC'},colx='pbdt',dbname='ara',tablename='yh_quote_curr',mmGap=30,**optx):
 	'''return [True|Flase] action for using web or DB
 	based on 'tablename' 'colx' field
 
 	'''
 	from _alan_calc import conn2mgdb
-	if not tablename:
-		return True
 	debugTF=getKeyVal(optx,'debugTF',False)
 	webTF=optx.pop('webTF',None)
 	if webTF is not None and isinstance(webTF,bool):
 		return webTF
-	currDt=pd.Timestamp.now(tz='US/Eastern')
-	cdt=getKeyVal(optx,'cdt',currDt)
+	cdt=getKeyVal(optx,'cdt',datetime.datetime.now())
 	mgDB=conn2mgdb(dbname=dbname)
 
 	dc = mgDB[tablename].find_one({"$query":jobj,"$orderby":{colx:-1}},{colx:1,"_id":0})
-	if dc is None or len(dc)<1:
+	if len(dc)<1:
 		return True
 	pdt=dc[colx]
 	mmPassed=pd.Timedelta(cdt - pdt).total_seconds() / 60.0
 	webTF = mmPassed>mmGap
 	if debugTF is True:
 		sys.stderr.write("{}|{}|{}|{}|{}\n".format("webTF","cdt","pdt","mmPassed","mmGap"))
 		sys.stderr.write("{}|{}|{}|{:.0f}|{}\n".format(webTF,cdt,pdt,mmPassed,mmGap))
@@ -158,27 +139,27 @@
 	'''
 	create yh_quote_curr table
 	'''
 	if tkLst is None or len(tkLst)<1:
 		from _alan_calc import sqlQuery
 		tkDF=sqlQuery('select ticker from mapping_ticker_cik where act_code=1')
 		tkLst=list(tkDF['ticker'])
-	d=[]
 	try:
 		jobj=dict(ticker=tkLst[0])
 		if webTF is None:
 			webTF = useWeb(jobj=jobj,dbname=dbname,tablename=tablename,**optx)
 		if not webTF:
 			jobj = {'ticker':{'$in':tkLst}}
 			d,_,_ = find_mdb(jobj,dbname=dbname,tablename=tablename,dfTF=True)
 			sys.stderr.write("===Using data from {}::{}\n".format(dbname,tablename))
 			return d
 		d=yh_quote_comparison(tkLst,screenerTF=screenerTF,dbname=dbname,tablename=tablename,zpk=zpk,**optx)
 	except Exception as e:
-		sys.stderr.write("**ERROR: {}@{}:{}\n".format("yh_quote_curr()","yh_quote_comparison",str(e)))
+		sys.stderr.write("**ERROR: {}:{}:{}\n".format("yh_quote_curr()","@ yh_quote_comparison",str(e)))
+		d=[]
 	saveDB=optx.pop('saveDB',False)
 	if not saveDB:
 		return d
 	try:
 		if m2pTF:
 			from mongo2psql import mongo2psql
 			mongo2psql(tablename,dbname)
@@ -186,32 +167,30 @@
 	except Exception as e:
 		sys.stderr.write("**ERROR: {}:{}:{}\n".format("yh_quote_curr()","mongo2psql ...",str(e)))
 
 	# Save yh_quote_curr To yh_quote_hist
 	try:
 		dbM = conn2mgdb(dbname=dbname)
 		tablename = tablename.replace('curr','hist')
-		if isinstance(d,pd.DataFrame):
-			d = d.to_dict(orient='records')
-		ret=dbM[tablename].insert_many(d,ordered=False)
+		ret=dbM[tablename].insert_many(d.to_dict(orient='records'),ordered=False)
 		sys.stderr.write("===Saving history: {dbname}::{tablename}".format(**locals()))
 	except Exception as e:
 		sys.stderr.write("**ERROR: {}:{}:{}\n".format("yh_quote_curr()","MDB saving...",str(e)))
 	return d
 
 def qS_keyStatistics(tkLst=[],tablename='qS_keyStatistics',saveDB=False,debugTF=True,**optx):
 	''' pull defaultKeyStatistics from yahoo and save to qS_keyStatistics
 	e.g.,
 	python3 -c "from yh_chart import qS_keyStatistics as yks;yks(['AAPL']);"
 	
 	'''
 	if tkLst is None or len(tkLst)<1:
 		tkLst = list(pull_act_tickers()['ticker'])
 	dbM=None
-	pbdt=pd.Timestamp.now(tz='US/Eastern')
+	pbdt=datetime.datetime.now()
 	jdM=yh_batchTypes(tkLst,types='quoteSummary',modules='defaultKeyStatistics',debugTF=debugTF)
 	for jx in jdM:
 		jx['pbdt']=pbdt
 	if saveDB is True:
 		zpk=optx.pop('zpk',{"ticker"})
 		m,dbM,err=upsert_mdb(jdM,clientM=dbM,tablename=tablename,zpk=zpk,**optx)
 		sys.stderr.write("=== {} of {} saved to {}\n".format(tkLst,jdM[-1],tablename))
@@ -315,28 +294,17 @@
 	jdTmp = ret.json()
 	return jdTmp
 
 def yh_batchRaw(tkLst=[],filter='*',types='spark',ranged='5m',interval='1m',debugTF=False,**optx):
 	'''
 	Pulling finance.yahoo data based on the 'types' of [spark|quote|chart]
 	'''
-	global credentials
 	if tkLst is None or len(tkLst)<1:
 		return {}
-	if types in ['quote']:
-		if not credentials:
-			credentials=getCredentials()
-			if debugTF:
-				sys.stderr.write("==GET CREDENTIALS: {}\n".format(credentials))
-
-		crumb,cookies = (credentials['crumb'],credentials['cookies'])
-		utmp = 'https://query1.finance.yahoo.com/v7/finance/{}?corsDomain=finance.yahoo.com&.tsrc=finance&'
-		urx = utmp + 'symbols={}&crumb={}'
-		url = urx.format(types,','.join(tkLst),crumb)
-	elif types in ['spark']:
+	if types in ['spark','quote']:
 		utmp = 'https://query1.finance.yahoo.com/v7/finance/{}?corsDomain=finance.yahoo.com&.tsrc=finance&'
 		urx = utmp + 'symbols={}&range={}&interval={}'
 		url = urx.format(types,','.join(tkLst),ranged,interval)
 	else:
 		utmp = 'https://query1.finance.yahoo.com/v8/finance/{}/{}?corsDomain=finance.yahoo.com&.tsrc=finance&'
 		urx = utmp + 'range={}&interval={}'
 		tkX = tkLst[0] if isinstance(tkLst,(list,tuple)) else tkLst
@@ -346,18 +314,17 @@
 	url += "&includeTimestamps={}&includePrePost={}".format(includeTimestamps,includePrePost)
 	if filter != '*' and types=='quote':
 		ftx="&fields={}".format(filter)
 		url += ftx
 	elif filter != '*':
 		ftx="&indicators={}".format(filter)
 		url += ftx
-	if types=='quote':
-		res=requests.Session().get(url,headers=headers,cookies=cookies)
-	else:
-		res=requests.Session().get(url,headers=headers)
+	if debugTF is True:
+		sys.stderr.write("==URL:\n{}\n".format(url))
+	res=requests.Session().get(url,headers=headers)
 	#res=requests.get(url,timeout=5)
 	if debugTF:
 		sys.stderr.write("=====URL STATUS:{}\n{}\n{}\n".format(res.status_code,tkLst,url))
 	if res.status_code!=200:
 		return {}
 	try:
 		jdTmp = res.json()
@@ -527,16 +494,16 @@
 			else:
 				jdM = batchSpark_sparkConv(jdLst,**optx)
 			if len(jdM)<1:
 				continue
 			if saveDB is True:
 				m,dbM,err=insert_mdb(jdM,clientM=dbM,tablename=tablename,zpk=zpk,**optx)
 				if debugTF:
-					sys.stderr.write("++yh_batchSpark(optx): {}\n".format(optx))
-					sys.stderr.write("=== SAVE {} data({}) {} to {}\n".format(tkM,len(jdM),jdM[-1],tablename))
+					sys.stderr.write("++optx: {}\n".format(optx))
+					sys.stderr.write("=== {} of {} saved to {}\n".format(tkM,jdM[-1],tablename))
 			jdN.extend(jdM)
 		else: # for case of types.lower()=='quote'
 			jdLst = jdTmp['quoteResponse']['result']
 			jdQC = batchSpark_quoteConv(jdLst,**optx)
 			if len(jdQC)<1:
 				continue
 			jdM = subDict(jdQC,colX)
@@ -660,23 +627,21 @@
 					jD=proc_summaryQuote(modObj,ticker=tkM,xmod=xmod)
 				jdX=[jD] if not isinstance(jD,list) else jD
 			elif types=='quote':
 				jdX = jdTmp['quoteResponse']['result']
 			else:
 				jdX = jdTmp[types]['result']
 			if debugTF:
-				sys.stderr.write("\n==={}.{}\n".format(j,tkM))
-				sys.stderr.write("---jdTmp: {}".format(jdTmp)[:80]+" ...\n")
-				sys.stderr.write("---jdX: {}".format(jdX[-1])[:80]+" ...\n\n")
+				sys.stderr.write("==={}.{}\njdTmp\n{}\njdX\n{}\n".format(j,tkM,jdTmp,jdX[-1]))
 		except Exception as e:
 			sys.stderr.write("**ERROR: {}:{}\n".format(types,str(e)))
 			continue
 		jdM.extend(jdX)
 	if debugTF:
-		sys.stderr.write("===jdM:\n{}".format(jdM)[:128]+" ...\n")
+		sys.stderr.write("===jdM:\n{}".format(jdM))
 	return jdM
 
 # DEPRECATED
 def raw2screener_output_1(jobj):
 	d = dict(ticker=jobj['symbol'])
 	d.update(changePercent=jobj['regularMarketChangePercent'])
 	if 'marketCap' in jobj:
@@ -698,15 +663,14 @@
 	return ds
 
 def yh_hist_query(tkLst=[],filter='*',types='quote',nchunk=20,rawTF=False,screenerTF=False,dfTF=False,debugTF=False,dbname=None,tablename=None,**optx):
 	'''
 	Pull minute ohlc pricing data from Yahoo but use marketVolume as volume
 	since market data has 15-minute delay, latest 15 marketVolumes become 0 
 	'''
-	saveDB=optx.get('saveDB',False)
 	if len(tkLst)<1:
 		tkLst = list(pull_act_tickers()['ticker'])
 	jdLst = yh_batchTypes(tkLst,filter=filter,types=types,nchunk=nchunk,debugTF=debugTF,**optx)
 	colX = ["ticker","open","high","low","close","volume","xclose","change","pchg","epochs",'hhmm',"pbdate","pbdt"]
 	dLst=[]
 	df=pd.DataFrame()
 	clientM=None
@@ -728,27 +692,28 @@
 				jdTmp['epochs']=jdTmp['regularMarketTime']*1000
 				jdTmp['pbdt'] = datetime.datetime.fromtimestamp(jdTmp['regularMarketTime'])
 				jdTmp['pbdate'] = int(jdTmp['pbdt'].strftime('%Y%m%d'))
 				newNames={"symbol":"ticker","regularMarketPrice":"close","regularMarketChange":"change","regularMarketChangePercent":"changePercent","regularMarketOpen":"open","regularMarketDayHigh":"high","regularMarketDayLow":"low","regularMarketVolume":"volume","regularMarketPreviousClose":"xclose","regularMarketTime":"epoch"}
 				if rawTF:
 					renameDict(jdTmp,mapper=newNames)
 					if debugTF:
-						sys.stderr.write("===jdTmp:\n{}".format(jdTmp)[:128]+" ...\n")
+						sys.stderr.write("{}\n".format(jdTmp))
 					if screenerTF==True:
 						colx=["change","changePercent","company","marketCap","close","ticker","volume","epochs","pbdt"]
 						#ds=raw2screener_output_1(jdTmp)
 						ds =  subDict(jdTmp,colx)
 						renameDict(ds,{"close":"price"})
 					elif screenerTF>0: # original False case
 						colx=list( set(newNames.values()).union(['epochs','pbdt','hhmm','pbdate','marketCap']) )
 						ds =  subDict(jdTmp,colx)
 					else:
 						ds = jdTmp 
-					if all([dbname,tablename,saveDB]):
+					if all([dbname,tablename]):
 						zpk=getKeyVal(optx,'zpk',['ticker','epochs'])
+						#mobj,clientM,err_msg = write2mdb(ds,clientM,dbname=dbname,tablename=tablename,zpk=zpk)
 						mobj,clientM,err_msg = insert_mdb(ds,clientM,dbname=dbname,tablename=tablename,zpk=zpk)
 						if debugTF:
 							sys.stderr.write("{}\nSave to {}::{}\n".format(ds,dbname,tablename))
 					dLst.append(ds)
 					continue
 				#- for 'spark' and 'chart' parsing
 				dx=pd.DataFrame([jdTmp])
@@ -830,190 +795,109 @@
 		#	dbM[tablename].create_index([(k,v) for k,v in zip(zpk,zsrt)],unique=True)
 		#ret=dbM[tablename].insert_many(df,ordered=ordered)
 		dbM=None;zpk=zpk
 		mobj,dbM,err_msg =upsert_mdb(df,dbM,dbname=dbname,tablename=tablename,zpk=zpk,insertOnly=True)
 	except Exception as e:
 		sys.stderr.write("**ERROR: {}:{}\n".format("func2mdb()",str(e)))
 	return df	
-
 def renewChk(pbdtCurr,pbdtMod,deltaTolerance=86400):
 	deltaPassed=pd.Timedelta(pbdtCurr - pbdtMod).total_seconds()
 	sys.stderr.write(" --curr:{},last:{}:deltaPassed:{}\n".format(pbdtCurr,pbdtMod,deltaPassed))
 	return deltaPassed>deltaTolerance
 
 def lastRunChk(objChk={},tableChk='',deltaTolerance=43200,clientM=None,dbname='ara',**optx):
-	pbdtCurr=pd.Timestamp.now(tz='US/Eastern')
+	pbdtCurr=pd.datetime.now()
 	lastObj,clientM,_=find_mdb(objChk,clientM=clientM,dbname=dbname,tablename=tableChk,limit=1)
 	if not lastObj:
 		pbdtMod=pbdtCurr
 		renewTF=True
 	else:
 		pbdtMod=lastObj[0]['pbdt']
 		renewTF=renewChk(pbdtCurr,pbdtMod,deltaTolerance)
 		if renewTF:
 			pbdtMod=pbdtCurr
 	objChk.update(pbdt=pbdtMod)
 	return renewTF,objChk,clientM
 
-def batchOTF(tkLst=[],**optx):
+def batchOTF(funcArg,tkLst=[],tableChk='',zpkChk=["ticker"],deltaTolerance=43200,**optx):
 	for ticker in tkLst: 
-		sys.stderr.write("==Batch Running:{} on {}\n".format(ticker,optx))
-		runOTF(ticker,**optx)
+		sys.stderr.write("==Batch Running:{} on {}\n".format(ticker,funcArg))
+		runOTF(funcArg,ticker,tableChk,zpkChk=zpkChk,deltaTolerance=deltaTolerance,**optx)
 
 @safeRunArg([])
-def runOTF(ticker='',funcN='',tableChk='',zpkChk=["ticker"],deltaTolerance=43200,**optx):
-	'''Fetch data from web/DB based on `deltaTolerance` in seconds
-	Required valid inputs: ticker, funcN, tablename
+def runOTF(funcArg,ticker='',tableChk='',zpkChk=["ticker"],deltaTolerance=43200,**optx):
 	'''
-	debugTF=optx.get('debugTF',False)
+	To  ticker='AAPL'
+	where real-time data is only grab based on 'deltaTolerance' in seconds
+	current setup is half-days
+	'''
+
 	if isinstance(ticker,list):
 		tkLst=ticker
+		dLst=[]
 		for tkX in tkLst: 
-			sys.stderr.write("==BATCH runOTF:{} on {}\n".format(ticker,funcN))
-			dd = runOTF(tkX,funcN,tableChk,zpkChk=zpkChk,deltaTolerance=deltaTolerance,**optx)
-		return dd
+			sys.stderr.write("==BATCH Running:{} on {}\n".format(ticker,funcArg))
+			dd = runOTF(funcArg,tkX,tableChk,zpkChk=zpkChk,deltaTolerance=deltaTolerance,**optx)
+			if isinstance(dd,list):
+				dLst.extend(dd)
+			else:
+				dLst.extend([dd])
+		return dLst
 
-	if isinstance(funcN,str) and funcN in globals() and hasattr(globals()[funcN],'__call__'):
-			funcArg =  globals()[funcN]
-	elif funcN in globals().values() and hasattr(funcN,'__call__'):
-			funcArg =funcN
-	else:
+	if isinstance(funcArg,str):
+		if funcArg in globals() and hasattr(globals()[funcArg],'__call__'):
+			funcArg =  globals()[funcArg]
+		else:
 			return []
-	sys.stderr.write("==START runOTF:{} on {}\n".format(ticker,funcArg))
-	if not optx.get('saveDB',False):
-		retObj = funcArg(ticker,**optx)
-		return retObj
+	sys.stderr.write("==START Running:{} on {}\n".format(ticker,funcArg))
 	dbname=getKeyVal(optx,'dbname','ara')
 	optx.update({'dbname':dbname})
 	tablename=getKeyVal(optx,'tablename','')
 	if not all([tablename, ticker]):
 		return []
 		
 	if 'modules' in optx:
 		objChk=dict(ticker=ticker,module=optx['modules'])
 	else:
 		objChk=dict(ticker=ticker)
 	if not tableChk:
 		tableChk=tablename+'_chk'
 	renewTF,objChk,clientM = lastRunChk(objChk=objChk,tableChk=tableChk,deltaTolerance=deltaTolerance,**optx)
-	if debugTF:
-		sys.stderr.write("==tableChk:{}".format(tableChk))
-		sys.stderr.write(": {} {} {}\n".format(renewTF,objChk,clientM))
 	if renewTF:
-		sys.stderr.write("==Data outdated or never run, Running:{}\n".format(funcN))
+		sys.stderr.write("==Data outdated or never run, Running:{}\n".format(funcArg))
 		retObj = funcArg(ticker,**optx)
-		if len(retObj)<1 and debugTF:
-			sys.stderr.write("**WARNING:{}({},{}) @runOTF:\n".format(funcN,ticker,optx))
 		if len(retObj)<1:
 			return []
-		if isinstance(retObj,pd.DataFrame):
-			retObj=retObj.to_dict(orient='records')
+
 		xChk={ky:val for ky,val in retObj[0].items() if ky in zpkChk}
 		objChk.update(xChk)
-		sys.stderr.write(" --Updating {} to {}\n".format(objChk,tableChk))
 		retObj,clientM,errChk = upsert_mdb(retObj,**optx)
+		sys.stderr.write(" --Update {} to {}\n".format(objChk,tableChk))
 		objChk,clientM,errChk = upsert_mdb(objChk,clientM=clientM,tablename=tableChk,zpk=zpkChk)
 	else:
 		sys.stderr.write("==Data exist, LoadFromTable:{}\n".format(tablename))
 		objChk.pop('pbdt',None)
 		optx.get('zpk',None)
 		retObj,clientM,errMsg = find_mdb(objChk,clientM=clientM,**optx)
 	return retObj
 
-from optparse import OptionParser
-def get_opts(argv,retParser=False):
-	""" command-line options initial setup
-	    Arguments:
-		argv:   list arguments, usually passed from sys.argv
-		retParser:      OptionParser class return flag, default to False
-	    Return: (options, args) tuple if retParser is False else OptionParser class
-	"""
-	parser = OptionParser(usage="usage: %prog [option] SYMBOL1[,...] [JSON]", version="%prog 0.01",
-		description="Pull Price History from YAHOO")
-	parser.add_option("","--types",action="store",dest="types",default='quote',
-		help="list of types:[chart,spark,quote] (default: quote)")
-	parser.add_option("","--funcname",action="store",dest="funcname",default="yh_quote_curr",
-		help="access function [yh_quote_curr|yh_hist_querry]  (default: yh_quote_curr)")
-	parser.add_option("","--range",action="store",dest="ranged",default='1d',
-		help="range period from now (default: 1d)")
-	parser.add_option("","--gap",action="store",dest="gap",default='1m',
-		help="interval GAP of data frequency (default: 1m)")
-	parser.add_option("-d","--database",action="store",dest="dbname",default="ara",
-		help="database (default: ara)")
-	parser.add_option("","--host",action="store",dest="hostname",default="localhost",
-		help="db host (default: localhost)")
-	parser.add_option("-t","--table",action="store",dest="tablename",
-		help="db tablename (default: None)")
-	parser.add_option("-w","--wmode",action="store",dest="wmode",default="replace",
-		help="db table write-mode [replace|append] (default: replace)")
-	parser.add_option("-o","--output",action="store",dest="output",
-		help="OUTPUT type [csv|html|json] (default: no output)")
-	parser.add_option("","--no_datetimeindex",action="store_false",dest="tsTF",default=True,
-		help="no datetime index (default: use datetime)")
-	parser.add_option("","--show_index",action="store_true",dest="indexTF",default=False,
-		help="show index (default: False) Note, OUTPUT ONLY")
-	parser.add_option("-s","--sep",action="store",dest="sep",default="|",
-		help="output field separator (default: |) Note, OUTPUT ONLY")
-	parser.add_option("","--no_database_save",action="store_false",dest="saveDB",default=True,
-		help="no save to database (default: save to database)")
-	parser.add_option("","--extra_js",action="store",dest="extraJS",
-		help="extra JSON in DICT format.")
-	parser.add_option("","--extra_qs",action="store",dest="extraQS",
-		help="extra GET string format like k1=v1&k2=v2; ")
-	parser.add_option("","--extra_xs",action="store",dest="extraXS",
-		help="extra excutable string like k1=v1;k2=v2; ")
-	parser.add_option("","--debug",action="store_true",dest="debugTF",default=False,
-		help="debugging (default: False)")
-	(options, args) = parser.parse_args(argv[1:])
-	try:
-		from _alan_str import extra_opts
-		opts = vars(options)
-		extra_opts(opts,xkey='extraJS',method='JS',updTF=True)
-		extra_opts(opts,xkey='extraQS',method='QS',updTF=True)
-		extra_opts(opts,xkey='extraXS',method='XS',updTF=True)
-		opts.update(args=args,narg=len(args))
-	except Exception as e:
-		sys.stderr.write(str(e)+"\n")
-	if retParser is True:
-		return parser
-	return (opts, args)
-
-def runArgs():
-	# GET options
-	(opts, args)=get_opts(sys.argv)
-	if not opts.get('tablename',None):
-		opts.pop('tablename')
-		#opts.update(saveDB=False)
-
-	funcName=opts.pop('funcname','yh_quote_curr')
-
-	# PROCESS arguments
+def main_tst():
+	args = sys.argv[1:]
 	if len(args)<1:
-		return __usage__
-	tkLst = args[0].split(',')
-	if tkLst[0]=='-':
-		tkLst = re.split('[\s,]',sys.stdin.read().strip())
-	optj=eval(args[1]) if args[1:] else {}
-	kLst=["args","narg","extraJS","extraQS","extraXS"]
-	keys_to_remove = set(kLst).intersection(set(opts.keys()))
-	for k in keys_to_remove:
-		del opts[k]
-	opts.update(optj)
-
-	# RUN 
-	if funcName in globals() and hasattr(globals()[funcName],'__call__'):
-		ret=globals()[funcName](tkLst,**opts)
-	else:
-		sys.stderr.write("**ERROR: {}() Not Exist\n".format(funcName))
-		return __usage__
-	return ret
+		#exit(0)
+		args=['AAPL','IBM']
+	elif len(args)==1 and ',' in args[0]:
+		args = args[0].split(',')
+	elif len(args)==1 and '-' in args[0]:
+		args = sys.stdin.read().strip().split()
+	#df = yh_spark_hist(args)
+	#df = yh_hist_query(args,types='spark',ranged='1d',pchgTF=False)
+	#df = yh_hist_query(args,types='quote',pchgTF=False,filter='symbol,regularMarketPrice,regularMarketChange,regularMarketOpen,regularMarketDayHigh,regularMarketDayLow,regularMarketVolume')
+	#df = yh_hist_query(args,types='quote')
+	df = yh_quote_curr(args)
+	if isinstance(df,list):
+		sys.stderr.write("\n{}".format(df))
+	else:
+		sys.stderr.write("\n{}".format(df.to_string()))
 
-def mainTst():
-	try:
-		ret = runArgs()
-	except Exception as e:
-		sys.stderr.write("**ERROR: runArgs:{}\n".format(str(e)))
-		ret = __usage__
-	return ret
-	
 if __name__ == '__main__':
-	sys.exit(mainTst())
+	main_tst()
```

### Comparing `talan-0.1.4.3/talan/yh_hist_batch.py` & `talan-0.1.4rc1/talan/yh_hist_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,14 @@
 		colv=['open','high','low','close','volume','adjusted','pbdate','name']
 	else:
 		colv=['open','high','low','close','volume','epochs','ticker']
 	if pchgTF:
 		colv += ['xclose','change','pchg']
 	colx = [x for x in colv if x in clx ]
 	sys.stderr.write("{}\n{}\n{}\n".format(colx,colv,clx))
-	sys.stderr.write("{}\n".format(dx[colx].head()))
 	sys.stderr.write("{}\n".format(dx[colx].tail()))
 	return dx[colx]
 
 def batch_yh_hist(tkLst=[],opts=None,**optx):
 	#- Set input parameters
 	if opts is None or len(opts)<1:
 		opts, _ = opt_yh_hist([])
```

### Comparing `talan-0.1.4.3/talan/yh_predefined.py` & `talan-0.1.4rc1/talan/yh_predefined.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 Usage of:
 python yh_predefined.py [ day_gainers | day_losers | most_actives ]
 
 RUN _actives in 'volume'
 python yh_predefined.py --no_database_save
 
 OR yh_predefined_query() call 
-python3 -c "from yh_predefined import yh_predefined_query as ypq;print(ypq())"
+python -c "from yh_predefined import yh_predefined_query as ypq;print(ypq())"
 
 OR bb_predefined() call most_actives in 'volume' and '>3% price change'
 python -c "from yh_predefined import bb_predefined as ypq;df=ypq('most_actives',addiFilter=1);print(df)"
 
 Last Mod., Fri Jul 26 23:34:16 EDT 2019
 '''
 import sys
 import requests
 import pandas as pd
 from _alan_str import write2mdb,find_mdb
 from _alan_date import s2dt
 from _alan_calc import sqlQuery
 from _alan_optparse import parse_opt, subDict
-hds={'Content-Type': 'text/html', 'Accept': 'application/json', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36'}
-
 
 def bb_predefined(scrIds='most_actives',dbname='ara',saveDB=True,mappingTF=True,mmGap=30,addiFilter=1,debugTF=False,**optx):
 	''' 
 	return a ticker list based on the combo of
 	yahoo 'scrIds' list and BB internal tracking tickers
 	where
 	  mappingTF: apply list on in the [mapping_ticker_cik] table
@@ -54,17 +52,15 @@
 			if mmPassed>mmGap: # check if DB info is winthin last 'mmGap' (30-minute)
 				df=[]
 		else:
 			df=[]
 		if len(df)>0:
 			if debugTF:
 				sys.stderr.write("===Use {} from MDB:{}\n".format(scrIds,tablename))
-			if 'changePercent' in df:
-				df = df.loc[abs(df['changePercent']).sort_values(ascending=False).index].reset_index(drop=False)
-			return df.iloc[:6]
+			return df
 		df=yh_predefined_query(scrIds,dfTF=True)
 		if len(df)<1: # using whatever in the DB if live pulling failed
 			df,_,_ = find_mdb(dbname=dbname,tablename=tablename,dfTF=True)
 			return df
 		df['pbdt'] = cdt
 		if mappingTF:
 			secInfo=sqlQuery('select * from mapping_ticker_cik where act_code=1')
@@ -87,16 +83,14 @@
 		if saveDB:
 			clientM=None
 			mobj, clientM, _ = write2mdb(df,clientM,dbname=dbname,tablename=tablename,zpk={'*'})
 			sys.stderr.write("Data saved to {}::{}".format(clientM,tablename))
 	except Exception as e:
 		sys.stderr.write("**ERROR: bb_predefined(): {}\n".format(str(e)))
 		df=[]
-	if 'changePercent' in df:
-		df = df.loc[abs(df['changePercent']).sort_values(ascending=False).index].reset_index(drop=False)
 	return df.iloc[:6]
 
 def screener_output_1(jobj):
 	d = dict(ticker=jobj['symbol'])
 	d.update(changePercent=jobj['regularMarketChangePercent']['raw'])
 	if 'marketCap' in jobj:
 		d.update(marketCap=jobj['marketCap']['raw'])
@@ -110,15 +104,15 @@
 
 def yh_predefined(scrIds='most_actives',debugTF=False,**optx):
 	''' 
 	return yahoo screener info in JSON based on 'scrIds'
 	'''
 	urx = 'https://query2.finance.yahoo.com/v1/finance/screener/predefined/saved?formatted=true&lang=en-US&region=US&scrIds={scrIds}&start=0&count=25&co'
 	url=urx.format(scrIds=scrIds)
-	ret = requests.get(url,headers=hds,timeout=3)
+	ret = requests.get(url,timeout=3)
 	jdTmp = ret.json()
 	return jdTmp
 
 
 def yh_predefined_query(scrIds='most_actives',dfTF=False,saveDB=False,screenerTF=True,debugTF=False,**optx):
 	''' 
 	return yahoo screener DictList/DataFrame relavant info based on 'scrIds'
```

### Comparing `talan-0.1.4.3/talan.egg-info/PKG-INFO` & `talan-0.1.4rc1/talan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talan
-Version: 0.1.4.3
+Version: 0.1.4rc1
 Summary: ('Technical ALgorithmic ANalytics',)
 Home-page: https://github.com/beyondbond/talan
 Author: Ted Hong
 Author-email: ted@beyondbond.com
 License: BSD 2-clause
 Description: Utility funcitions for financial analysis
 Platform: UNKNOWN
```

### Comparing `talan-0.1.4.3/talan.egg-info/SOURCES.txt` & `talan-0.1.4rc1/talan.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 talan/_alan_mp4.py
 talan/_alan_ohlc_fcs.py
 talan/_alan_optparse.py
 talan/_alan_pppscf.py
 talan/_alan_rmc.py
 talan/_alan_str.py
 talan/alanapi.py
-talan/chatgptAPI.py
 talan/csv2plotj2ts.py
 talan/find_recent_eps.py
 talan/fredReader.py
-talan/get_rq.py
 talan/headline_calc.py
 talan/headline_sts.py
 talan/iex_peers.py
 talan/lsi_daily.py
 talan/macro_event_yh.py
 talan/plot_templates.py
 talan/prc_temp_DN.py
```

