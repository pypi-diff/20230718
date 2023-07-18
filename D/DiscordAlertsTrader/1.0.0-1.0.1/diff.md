# Comparing `tmp/DiscordAlertsTrader-1.0.0.tar.gz` & `tmp/DiscordAlertsTrader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiscordAlertsTrader-1.0.0.tar", last modified: Sun Jul 16 16:55:49 2023, max compression
+gzip compressed data, was "DiscordAlertsTrader-1.0.1.tar", last modified: Tue Jul 18 10:54:19 2023, max compression
```

## Comparing `DiscordAlertsTrader-1.0.0.tar` & `DiscordAlertsTrader-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.888747 DiscordAlertsTrader-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.783184 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/
--rw-rw-rw-   0        0        0       47 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-07-15 20:38:48.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_generator.py
--rw-rw-rw-   0        0        0    14034 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_tracker.py
--rw-rw-rw-   0        0        0    74192 2023-07-16 16:41:57.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_trader.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.833262 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/
--rw-rw-rw-   0        0        0    12837 2023-07-13 14:38:05.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/TDA_api.py
--rw-rw-rw-   0        0        0     2800 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/__init__.py
--rw-rw-rw-   0        0        0    23709 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/eTrade_api.py
--rw-rw-rw-   0        0        0    17459 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/weBull_api.py
--rw-rw-rw-   0        0        0     3813 2023-06-20 16:07:36.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/calc_stats.py
--rw-rw-rw-   0        0        0    12181 2023-07-13 14:23:53.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/calc_strat.py
--rw-rw-rw-   0        0        0     4807 2023-07-16 16:19:10.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/configurator.py
--rw-rw-rw-   0        0        0    15905 2023-07-16 15:56:29.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/discord_bot.py
--rw-rw-rw-   0        0        0     2345 2023-06-08 13:42:28.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/fend_bot.py
--rw-rw-rw-   0        0        0    15655 2023-07-16 15:15:51.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui.py
--rw-rw-rw-   0        0        0    23375 2023-07-15 18:44:04.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_generator.py
--rw-rw-rw-   0        0        0    15051 2023-07-16 15:11:55.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_layouts.py
--rw-rw-rw-   0        0        0     1834 2023-05-28 17:46:50.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/load_chn_hist.py
--rw-rw-rw-   0        0        0    18352 2023-07-15 16:03:06.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/message_parser.py
--rw-rw-rw-   0        0        0    15335 2023-07-15 18:48:55.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/port_sim.py
--rw-rw-rw-   0        0        0    20395 2023-07-04 15:50:18.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/tem_etrades.py
--rw-rw-rw-   0        0        0      327 2023-07-13 15:28:14.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/test_trader.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.810191 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/
--rw-rw-rw-   0        0        0     9294 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-16 16:55:49.000000 DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1545 2023-05-17 00:51:47.000000 DiscordAlertsTrader-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9294 2023-07-16 16:55:49.887747 DiscordAlertsTrader-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8432 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 16:55:49.888747 DiscordAlertsTrader-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:55:49.886747 DiscordAlertsTrader-1.0.0/tests/
--rw-rw-rw-   0        0        0      119 2023-03-28 13:47:06.000000 DiscordAlertsTrader-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2694 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/mock_discord_message.py
--rw-rw-rw-   0        0        0      974 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_AlertsTracker.py
--rw-rw-rw-   0        0        0    12801 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_AlertsTrader.py
--rw-rw-rw-   0        0        0     7396 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_AlertsTrader_exits.py
--rw-rw-rw-   0        0        0     5157 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_TDA.py
--rw-rw-rw-   0        0        0     1062 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_configurator.py
--rw-rw-rw-   0        0        0     4680 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.0/tests/test_discord_bot.py
--rw-rw-rw-   0        0        0     4964 2023-07-15 17:47:09.000000 DiscordAlertsTrader-1.0.0/tests/test_msg_parsed.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:54:19.700771 DiscordAlertsTrader-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-18 10:54:19.660771 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/
+-rw-rw-rw-   0        0        0       47 2023-07-18 10:54:11.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/__init__.py
+-rw-rw-rw-   0        0        0     2426 2023-07-15 20:38:48.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/alerts_generator.py
+-rw-rw-rw-   0        0        0    14034 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/alerts_tracker.py
+-rw-rw-rw-   0        0        0    74184 2023-07-18 10:50:46.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/alerts_trader.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:54:19.688772 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/
+-rw-rw-rw-   0        0        0    12837 2023-07-13 14:38:05.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/TDA_api.py
+-rw-rw-rw-   0        0        0     2800 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/__init__.py
+-rw-rw-rw-   0        0        0    23709 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/eTrade_api.py
+-rw-rw-rw-   0        0        0    17459 2023-07-11 17:52:40.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/weBull_api.py
+-rw-rw-rw-   0        0        0     3813 2023-06-20 16:07:36.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/calc_stats.py
+-rw-rw-rw-   0        0        0    12181 2023-07-18 10:50:46.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/calc_strat.py
+-rw-rw-rw-   0        0        0     4807 2023-07-16 16:19:10.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/configurator.py
+-rw-rw-rw-   0        0        0    15905 2023-07-16 15:56:29.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/discord_bot.py
+-rw-rw-rw-   0        0        0     2345 2023-06-08 13:42:28.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/fend_bot.py
+-rw-rw-rw-   0        0        0    15653 2023-07-18 10:50:46.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/gui.py
+-rw-rw-rw-   0        0        0    23671 2023-07-18 10:50:46.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/gui_generator.py
+-rw-rw-rw-   0        0        0    15051 2023-07-16 15:11:55.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/gui_layouts.py
+-rw-rw-rw-   0        0        0     1834 2023-05-28 17:46:50.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/load_chn_hist.py
+-rw-rw-rw-   0        0        0    18619 2023-07-18 10:50:46.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/message_parser.py
+-rw-rw-rw-   0        0        0    15335 2023-07-15 18:48:55.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/port_sim.py
+-rw-rw-rw-   0        0        0    20395 2023-07-04 15:50:18.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/tem_etrades.py
+-rw-rw-rw-   0        0        0      327 2023-07-13 15:28:14.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/test_trader.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:54:19.683771 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/
+-rw-rw-rw-   0        0        0     9801 2023-07-18 10:54:19.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-07-18 10:54:19.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:54:19.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-18 10:54:19.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-07-18 10:54:19.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-18 10:54:19.000000 DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1545 2023-05-17 00:51:47.000000 DiscordAlertsTrader-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     9801 2023-07-18 10:54:19.699772 DiscordAlertsTrader-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8939 2023-07-18 10:50:46.000000 DiscordAlertsTrader-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:54:19.700771 DiscordAlertsTrader-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-18 10:53:59.000000 DiscordAlertsTrader-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:54:19.698770 DiscordAlertsTrader-1.0.1/tests/
+-rw-rw-rw-   0        0        0      119 2023-03-28 13:47:06.000000 DiscordAlertsTrader-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2694 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/mock_discord_message.py
+-rw-rw-rw-   0        0        0      974 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/test_AlertsTracker.py
+-rw-rw-rw-   0        0        0    12801 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/test_AlertsTrader.py
+-rw-rw-rw-   0        0        0     7396 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/test_AlertsTrader_exits.py
+-rw-rw-rw-   0        0        0     5157 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/test_TDA.py
+-rw-rw-rw-   0        0        0     1062 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/test_configurator.py
+-rw-rw-rw-   0        0        0     4680 2023-07-11 17:52:41.000000 DiscordAlertsTrader-1.0.1/tests/test_discord_bot.py
+-rw-rw-rw-   0        0        0     4964 2023-07-15 17:47:09.000000 DiscordAlertsTrader-1.0.1/tests/test_msg_parsed.py
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_generator.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/alerts_generator.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_tracker.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/alerts_tracker.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/alerts_trader.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/alerts_trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1060,15 +1060,15 @@
                         exit_plan = eval(trade["exit_plan"])                        
                         PT, SL = self.cfg['shorting']['BTC_EOD_PT_SL'].split(",")
                         SL, PT = eval(SL)/100, eval(PT)/100
                         
                         # check if not already updated, assume 5-10% exits are the updated 
                         # percentage_difference = round(abs(exit_plan['SL'] - exit_plan['PT1']) / exit_plan['PT1'], 2)
                         # if abs(percentage_difference - (SL+PT)) <= 0.03:  # accept 3% rounding error
-                        if self.EOD.get(trade["Symbol"]) is not "15min":
+                        if self.EOD.get(trade["Symbol"]) != "15min":
                             quote = self.price_now(trade["Symbol"], "BTC", 1)
                             exit_plan = {
                                 "PT1": round(quote - PT * quote, 2),
                                 "PT2": None,
                                 "PT3": None,
                                 "SL": round(quote + SL * quote, 2)
                                 }
@@ -1077,15 +1077,15 @@
                             str_msg = f'updating exits option {trade["Symbol"]} 15 min before EOD with {SL*100}% SL and {PT*100}% PT'
                             print(Back.GREEN + str_msg)
                             self.queue_prints.put([str_msg, "", "green"])
                             self.exit_percent_to_price(i)
                             self.EOD[trade["Symbol"]] = "15min"
                 # Close position 5 min to close
                 elif time_now >= time_five.time() and time_now < time_closed.time() \
-                    and self.EOD.get(trade["Symbol"]) is not "5min":
+                    and self.EOD.get(trade["Symbol"]) != "5min":
                     print(f'closing option {trade["Symbol"]} 5 min before EOD')
                     quote = self.price_now(trade["Symbol"], "BTC", 1)
                     
                     # Close and send lim order
                     self.close_open_exit_orders(i)       
                     order = {}
                     order['action'] = "BTC"
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/TDA_api.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/TDA_api.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/__init__.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/__init__.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/eTrade_api.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/eTrade_api.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/brokerages/weBull_api.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/brokerages/weBull_api.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/calc_stats.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/calc_stats.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/calc_strat.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/calc_strat.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,27 +266,27 @@
     return res
 
 
 
 port, no_quote, param = calc_returns(
     fname_port= cfg['portfolio_names']['tracker_portfolio_name'],
     dir_quotes= cfg['general']['data_dir'] + '/live_quotes',
-    last_days= 17,
+    last_days= 60,
     max_underlying_price= 500,
     min_price= 50,
     max_dte= 10,
     min_dte= 0,
     exclude_traders= [ 'SPY', 'enhancedmarket'],
     exclude_symbols= ['SPX'],
     exclude_channs = "",
-    PT=50,
+    PT=100,
     TS=0,
     SL=40,
     TS_buy= 10,
-    max_margin = 22900
+    max_margin = None
     )
 
 # print(port[['Date','Symbol','Trader', 'STC-PnL', 'STC-PnL-current', 'strategy-PnL','STC-PnL$', 'STC-PnL$-current',
 #                 'strategy-PnL$','strategy-entry','strategy-exit', 'strategy-close_date']])
 sport = port[['Date','Symbol','Trader', 'PnL', 'PnL-actual', 'PnL$', 'PnL$-actual', 'strategy-PnL',
                'strategy-PnL$','strategy-entry','strategy-exit', 'strategy-close_date', 'reason_skip']]
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/configurator.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/configurator.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/discord_bot.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/discord_bot.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/fend_bot.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/fend_bot.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
     alistner.run(cfg['discord']['discord_token'])
 
 
 def gui():   
     client_thread = threading.Thread(target=run_client, daemon=True)
 
     # start the threads
-    # client_thread.start()
+    client_thread.start()
     run_gui()
 
     # close the GUI window
     window.close()
     alistner.close_bot()
     exit()
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_generator.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/gui_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Created on Fri Apr  9 09:53:44 2021
 
 @author: adonay
 """
 import math
 import os.path as op
 import pandas as pd
-from datetime import datetime
+from datetime import datetime, date
 import numpy as np
 from .configurator import cfg
 from .alerts_tracker import calc_stc_prices
 from .port_sim import filter_data
 
 def short_date(datestr, infrm="%Y-%m-%d %H:%M:%S.%f", outfrm="%m/%d/%Y %H:%M"):
     return datetime.strptime(datestr, infrm).strftime(outfrm)
@@ -99,23 +99,22 @@
                             filt_date_frm=port_filt_date_frm,
                             filt_date_to=port_filt_date_to,
                             filt_sym=port_filt_sym,
                             filt_chn=port_filt_chn,
                             exc_author=port_exc_author,
                             exc_chn=port_exc_chn
                             )
-   
     except Exception as e:
         print("error during portfolio filter data", e)
         pass
     
     live_col = False
     data['Live'] = np.nan
     if not exclude.get("live PnL", False):
-        data =  get_live_quotes(data)
+        data =  get_live_quotes(data, trader_port=True)
         if 'Live' in data.columns:
             live_col = True
 
     data['STC-Qty'] = data[['STC1-Qty', 'STC2-Qty', 'STC3-Qty']].sum(axis=1)
     data['Price-actual'] = data['Price-actual']
     
     for price in ['Price', 'Price-alert', 'Price-actual']:
@@ -150,15 +149,15 @@
                 "PnL", "PnL$","PnL-alert", "PnL$-alert","PnL-actual","PnL$-actual", 
                 "STC-Price", "STC-Price-actual", "STC-Price-alert", 
                 ]
     
     for cfrm in frm_cols:
         data[cfrm] = pd_col_str_frmt(data[cfrm])
 
-    cols = ['isOpen', "PnL", "PnL$", 'Date', 'Symbol', 'Trader', 'BTO-Status', 'Price',
+    cols = ['isOpen', "PnL", "PnL$", 'Date', 'Symbol', 'Trader', 'BTO-Status', 'Type','Price',
             'Price-alert', "Price-actual", 'Qty', 'filledQty', 'N Alerts',"PnL-alert",
             "PnL$-alert","PnL-actual","PnL$-actual", 
             "STC-Price", "STC-Price-actual", "STC-Price-alert",
             "STC-Prices","STC-Prices-actual", "STC-Prices-alert",
             'STC1-Status','STC1-Qty', 'STC2-Status', 'STC2-Qty', 'STC3-Status',  'STC3-Qty',                      
             ]
     cols = ['Live'] + cols
@@ -204,26 +203,26 @@
                             exc_author=track_exc_author,
                             exc_chn=track_exc_chn
                         )
     except Exception as e:
         print("error during tracker filter data", e)
         pass
     
-    data['Date'] = data['Date'].apply(lambda x: short_date(x))
-    data["isOpen"] = data["isOpen"].map({1:"Yes", 0:"No"})
-    data["N Alerts"]= data['Avged']
-    data['Trader'] = data['Trader'].apply(lambda x: x.split('(')[0].split('#')[0])
-    
     live_col = False
     data['Live'] = np.nan
     if not exclude.get("live PnL", False):
         data =  get_live_quotes(data)
         if 'Live' in data.columns:
             live_col = True
-
+    
+    data['Date'] = data['Date'].apply(lambda x: short_date(x))
+    data["isOpen"] = data["isOpen"].map({1:"Yes", 0:"No"})
+    data["N Alerts"]= data['Avged']
+    data['Trader'] = data['Trader'].apply(lambda x: x.split('(')[0].split('#')[0])
+    
     frm_cols = ['Qty', 'N Alerts', 'STC-Qty','STC-Price','STC-Price-actual','PnL','PnL-actual',
                 'PnL$','PnL$-actual', 'Price', 'Price-actual']
     for cfrm in frm_cols:
         data[cfrm] = pd_col_str_frmt(data[cfrm])
     
     if live_col:
         data['Live'] = pd_col_str_frmt(data['Live'])
@@ -325,15 +324,18 @@
     header_list = [d.replace('STC-', '') for d in header_list]
     data = result_td.values.tolist()
     return data, header_list
 
 
 def get_live_quotes(portfolio, trader_port=False):
     dir_quotes = cfg['general']['data_dir'] + '/live_quotes'
-    track_symb = portfolio.loc[portfolio['isOpen']=='Yes', 'Symbol'].to_list()
+    
+    msk = (pd.to_datetime(portfolio['Date']).dt.date == date.today()) | (portfolio['isOpen']==1)
+    
+    track_symb = portfolio.loc[msk, 'Symbol'].to_list()
     
     quotes_sym = {}
     for sym in track_symb: 
         fquote = f"{dir_quotes}/{sym}.csv"
         if not op.exists(fquote):
             continue
         
@@ -343,41 +345,47 @@
         timestamp, quote = quotes[-1].split(',')  # in ms
         quotes_sym[sym] = float(quote.replace('\n', '').replace(' ', ''))
     
     for sym in quotes_sym:
         live_price = quotes_sym[sym]
         if live_price == 0:
             continue
-        msk = (portfolio['Symbol']==sym) & (portfolio['isOpen']=='Yes')
+        msk = portfolio['Symbol']==sym
         trades = portfolio.loc[msk]
         
         for ix, trade in trades.iterrows():
+            portfolio.loc[ix, 'Live'] = live_price
+            if trade['isOpen'] == 0:
+                continue
             order= {
                 "Qty": trade['Qty'] if pd.isnull(trade.get("STC-Qty")) else trade['Qty']- trade["STC-Qty"],
                 "price": live_price,
                 "Actual Cost": live_price,
                 } 
-            portfolio.loc[ix, 'Live'] = live_price
+
             if trader_port:
                 trade = compute_live_trader_port(trade, order)
                 portfolio.loc[ix] = trade
             else:                 
                 stc_info = calc_stc_prices(trade, order)
                 for k, v in stc_info.items():
                     if k == "STC-Qty":
                         continue
                     portfolio.loc[msk,k] = v
+            # portfolio.loc[ix, 'Live'] = live_price
     return portfolio
 
 
 def compute_live_trader_port(trade, order):
     "Workaround to get live trade Pnl for trader portfolio"
     stc_price = order['price']
 
     bto_price = trade["Price"]
+    if pd.isnull(bto_price):
+        return trade 
     bto_price_alert = trade["Price-alert"]
     bto_price_actual = trade["Price-actual"]
 
     if trade["Type"] == "BTO":
         stc_PnL = float((stc_price - bto_price)/bto_price) *100
     elif trade["Type"] == "STO":
         stc_PnL = float((bto_price - stc_price)/bto_price) *100
@@ -390,14 +398,15 @@
             break
 
     #Log portfolio
     trade[ STC + "-Price"] = stc_price
     trade[ STC + "-Price-alert"] = stc_price
     trade[ STC + "-Price-actual"] = stc_price
     trade[ STC + "-PnL"] = stc_PnL
+    trade[ STC + "-Qty"] = order['Qty']
 
     sold_tot = np.nansum([trade[f"STC{i}-Qty"] for i in range(1,4)])
     stc_PnL_all = np.nansum([trade[f"STC{i}-PnL"]*trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
     trade[ "PnL"] = stc_PnL_all
 
     if trade[ "Type"] == "BTO":
         stc_PnL_all_alert =  np.nansum([(float((trade[f"STC{i}-Price-alert"] - bto_price_alert)/bto_price_alert) *100) * trade[f"STC{i}-Qty"] for i in range(1,4)])/sold_tot
@@ -409,15 +418,14 @@
     trade[ "PnL-alert"] = stc_PnL_all_alert
     trade[ "PnL-actual"] = stc_PnL_all_curr
 
     mutipl = 1 if trade['Asset'] == "option" else .01  # pnl already in %
     trade[ "PnL$"] =  stc_PnL_all* bto_price *mutipl*sold_tot
     trade[ "PnL$-alert"] =  stc_PnL_all_alert* bto_price_alert *mutipl*sold_tot
     trade[ "PnL$-actual"] =  stc_PnL_all_curr* bto_price_actual *mutipl*sold_tot
-
     return trade
 
 def get_hist_msgs(filt_author='', filt_date_frm='', filt_date_to='',
                   filt_cont='', chan_name="option_alerts", **kwargs):
     # Provide arguments to filter
     data = pd.read_csv(op.join(cfg['general']['data_dir'] , f"{chan_name}_message_history.csv"),
                        usecols=['Author', 'Date', 'Content', 'Parsed'])
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/gui_layouts.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/gui_layouts.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/load_chn_hist.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/load_chn_hist.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/message_parser.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/message_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,22 +50,29 @@
         if action.upper() in ["BTO", "STO"]:
             if "avg" in msg.lower() or "average" in msg.lower():
                 avg_price, _ = parse_avg(msg)
                 pars = pars + f"AVG to {avg_price} "
                 order["avg"] = avg_price
             else:
                 order["avg"] = None
-            pt1_v, pt2_v, pt3_v, sl_v = parse_exits(msg)
-            n_pts = 3 if pt3_v else 2 if pt2_v else 1 if pt1_v else 0
-            pts_qty = set_pt_qts(n_pts)
-            order, pars = make_order_exits(order, msg, pars, asset_type)
+            try:
+                pt1_v, pt2_v, pt3_v, sl_v = parse_exits(msg)
+                n_pts = 3 if pt3_v else 2 if pt2_v else 1 if pt1_v else 0
+                pts_qty = set_pt_qts(n_pts)
+                order, pars = make_order_exits(order, msg, pars, asset_type)
+                order["n_PTs"] = n_pts
+                order["PTs_Qty"] = pts_qty
+            except:
+                order["PT1"] =  None
+                order["PT2"] = None
+                order["PT3"] = None
+                order["SL"] = None            
             sl_mental = True if "mental" in msg.lower() else False
             if sl_mental: order["SL_mental"] = True
-            order["n_PTs"] = n_pts
-            order["PTs_Qty"] = pts_qty
+            
 
         elif action.upper() in ["STC", "BTC"]:
             xamnt = parse_sell_ratio_amount(msg, asset_type)
             if order["Qty"] is None:
                 pars = pars + f" xamount: {xamnt}"
             order["xQty"] = xamnt
         
@@ -395,15 +402,15 @@
     re_comp= re.compile("\s" +expr + "[:]?[ ]*[$]*(\d*[\.]*[\d]*[%]?)(TS[\d+\.]*[%]?)?", re.IGNORECASE) 
     exit_inf = re_comp.search(msg) 
 
     if exit_inf is None:
         re_comp= re.compile("(" + expr.lower() + "[:]?[ ]*[$]*(\d*[\.]*[\d]*[%]?))", re.IGNORECASE)
         exit_inf = re_comp.search(msg)        
 
-        if exit_inf is None:
+        if exit_inf is None or exit_inf.groups()[-1] =='':
             return None
         elif "%" in exit_inf.groups()[-1]:
             return exit_inf.groups()[-1]
         return float(exit_inf.groups()[-1].replace("..", ""))
     exit_v = exit_inf.group(1) + (exit_inf.group(2) if exit_inf.group(2) else "")
     return exit_v
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/port_sim.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/port_sim.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader/tem_etrades.py` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader/tem_etrades.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/PKG-INFO` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiscordAlertsTrader
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for automating discord trade alerts in TDA or eTrade.
 Home-page: 
 Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
 Author: Adonay Nunes
 Author-email: adonays.nunes@gmail.com
 License: BSD (3-clause)
 Classifier: License :: OSI Approved :: BSD License
@@ -17,19 +17,20 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/t/AdoNunes/DiscordAlertsTrader?color=red)
 ![PyPI](https://img.shields.io/pypi/v/DiscordAlertsTrader)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/DiscordAlertsTrader)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/DiscordAlertsTrader)
 ![GitHub](https://img.shields.io/github/license/AdoNunes/DiscordAlertsTrader)
-[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Zb4ymtF "realtime support / chat with the community and the team.")
+[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/9ejghcjpar "realtime support / chat with the community and the team.")
 
 
 A Python package to automate trades from alerts shared in a Discord channel by analysts.
 The package parses these messages and executes trades from traders specified in the configuration file. 
 It tracks messages from all the channels, generates a portfolio from analysts and from trades executed, 
 provides live quotes to see actual alert profits (rather than prices stated in the alert), and can trigger
 an alert to open long or short a position, close it or update exits (target profit, stop loss).
@@ -48,21 +49,22 @@
 - Tracking performance with real-time actual prices and returns.
 - Opening, closing, and updating trades through the GUI.
 - Calculate analysts' stats and provide options to test stats with maximum capital 
 - Checking order and account status, and accessing current ticker prices.
 - Supporting manual trade execution through prompts if `auto_trade` is set to False in `config.ini`.
 
 
-Supports any Discord channel with structured alerts BTO and STC as message contents (not embedded)
+**Current Discord servers being used**:
+- TradeProElite (good timing, profitable strategies): [invite link](https://tradeproelite.memberful.com/referral/vedpmz8)
+- BullTrades (good for shorting, see historical trades in the package): [invite link](https://bulltrades.net/?ref=ndrjogi)
 
-**Currently, version control for analysts portfolio is from server BullTrades.[you can see all historical stats]** 
-  - Invite link to BullTrades: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
+Supports any Discord channel with structured BTP/STC alerts as message contents (not embedded, yet)
 
 
-Let me know if you find the package useful or need support by dropping me an email or visiting the [discord server](https://discord.gg/9ejghcjpar)
+Let me know if you find the package useful or need support by dropping me a DM @MinkysTradus or visiting the [discord server](https://discord.gg/9ejghcjpar)
 
  ________________________
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
 <img src="media/xtrader_console.png" alt="Console with discord messages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
@@ -71,14 +73,17 @@
  ## Discord user token and channel IDs
  ______________________________
 
 It requires a user discord token, once installed the package saves the token in config.ini[discord], as well as the channel ID where alerts are posted.
 To get the discord token follow the instructions: https://www.androidauthority.com/get-discord-token-3149920/
 To get the channel ID, in Discord right click on the channel and click "Copy Channel ID"
 
+**Automation of user accounts is against Discord ToS. This package only read alerts and Discord can not detect automation behavior,
+however, if you want to follow Discords ToS, do not provide a user token and manually input the alerts at the bottom of the GUI to
+manually trigger the alerts ;)**
 
 ## Installation and Setup
  ______________________________
 
 1. Install Python:
    - For Windows, open PowerShell and run the following command, verify that it prints out "Hello World!":
      ```powershell
```

### Comparing `DiscordAlertsTrader-1.0.0/DiscordAlertsTrader.egg-info/SOURCES.txt` & `DiscordAlertsTrader-1.0.1/DiscordAlertsTrader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/LICENSE` & `DiscordAlertsTrader-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/PKG-INFO` & `DiscordAlertsTrader-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiscordAlertsTrader
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for automating discord trade alerts in TDA or eTrade.
 Home-page: 
 Download-URL: https://github.com/AdoNunes/DiscordAlertsTrader
 Author: Adonay Nunes
 Author-email: adonays.nunes@gmail.com
 License: BSD (3-clause)
 Classifier: License :: OSI Approved :: BSD License
@@ -17,19 +17,20 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/t/AdoNunes/DiscordAlertsTrader?color=red)
 ![PyPI](https://img.shields.io/pypi/v/DiscordAlertsTrader)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/DiscordAlertsTrader)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/DiscordAlertsTrader)
 ![GitHub](https://img.shields.io/github/license/AdoNunes/DiscordAlertsTrader)
-[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Zb4ymtF "realtime support / chat with the community and the team.")
+[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/9ejghcjpar "realtime support / chat with the community and the team.")
 
 
 A Python package to automate trades from alerts shared in a Discord channel by analysts.
 The package parses these messages and executes trades from traders specified in the configuration file. 
 It tracks messages from all the channels, generates a portfolio from analysts and from trades executed, 
 provides live quotes to see actual alert profits (rather than prices stated in the alert), and can trigger
 an alert to open long or short a position, close it or update exits (target profit, stop loss).
@@ -48,21 +49,22 @@
 - Tracking performance with real-time actual prices and returns.
 - Opening, closing, and updating trades through the GUI.
 - Calculate analysts' stats and provide options to test stats with maximum capital 
 - Checking order and account status, and accessing current ticker prices.
 - Supporting manual trade execution through prompts if `auto_trade` is set to False in `config.ini`.
 
 
-Supports any Discord channel with structured alerts BTO and STC as message contents (not embedded)
+**Current Discord servers being used**:
+- TradeProElite (good timing, profitable strategies): [invite link](https://tradeproelite.memberful.com/referral/vedpmz8)
+- BullTrades (good for shorting, see historical trades in the package): [invite link](https://bulltrades.net/?ref=ndrjogi)
 
-**Currently, version control for analysts portfolio is from server BullTrades.[you can see all historical stats]** 
-  - Invite link to BullTrades: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
+Supports any Discord channel with structured BTP/STC alerts as message contents (not embedded, yet)
 
 
-Let me know if you find the package useful or need support by dropping me an email or visiting the [discord server](https://discord.gg/9ejghcjpar)
+Let me know if you find the package useful or need support by dropping me a DM @MinkysTradus or visiting the [discord server](https://discord.gg/9ejghcjpar)
 
  ________________________
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
 <img src="media/xtrader_console.png" alt="Console with discord messages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
@@ -71,14 +73,17 @@
  ## Discord user token and channel IDs
  ______________________________
 
 It requires a user discord token, once installed the package saves the token in config.ini[discord], as well as the channel ID where alerts are posted.
 To get the discord token follow the instructions: https://www.androidauthority.com/get-discord-token-3149920/
 To get the channel ID, in Discord right click on the channel and click "Copy Channel ID"
 
+**Automation of user accounts is against Discord ToS. This package only read alerts and Discord can not detect automation behavior,
+however, if you want to follow Discords ToS, do not provide a user token and manually input the alerts at the bottom of the GUI to
+manually trigger the alerts ;)**
 
 ## Installation and Setup
  ______________________________
 
 1. Install Python:
    - For Windows, open PowerShell and run the following command, verify that it prints out "Hello World!":
      ```powershell
```

### Comparing `DiscordAlertsTrader-1.0.0/README.md` & `DiscordAlertsTrader-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # DiscordAlertsTrader: *Discord Alerts Trader Bot*
 ________________________
+![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/t/AdoNunes/DiscordAlertsTrader?color=red)
 ![PyPI](https://img.shields.io/pypi/v/DiscordAlertsTrader)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/DiscordAlertsTrader)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/DiscordAlertsTrader)
 ![GitHub](https://img.shields.io/github/license/AdoNunes/DiscordAlertsTrader)
-[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Zb4ymtF "realtime support / chat with the community and the team.")
+[![Discord](https://img.shields.io/discord/1123242366980075570.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/9ejghcjpar "realtime support / chat with the community and the team.")
 
 
 A Python package to automate trades from alerts shared in a Discord channel by analysts.
 The package parses these messages and executes trades from traders specified in the configuration file. 
 It tracks messages from all the channels, generates a portfolio from analysts and from trades executed, 
 provides live quotes to see actual alert profits (rather than prices stated in the alert), and can trigger
 an alert to open long or short a position, close it or update exits (target profit, stop loss).
@@ -27,21 +28,22 @@
 - Tracking performance with real-time actual prices and returns.
 - Opening, closing, and updating trades through the GUI.
 - Calculate analysts' stats and provide options to test stats with maximum capital 
 - Checking order and account status, and accessing current ticker prices.
 - Supporting manual trade execution through prompts if `auto_trade` is set to False in `config.ini`.
 
 
-Supports any Discord channel with structured alerts BTO and STC as message contents (not embedded)
+**Current Discord servers being used**:
+- TradeProElite (good timing, profitable strategies): [invite link](https://tradeproelite.memberful.com/referral/vedpmz8)
+- BullTrades (good for shorting, see historical trades in the package): [invite link](https://bulltrades.net/?ref=ndrjogi)
 
-**Currently, version control for analysts portfolio is from server BullTrades.[you can see all historical stats]** 
-  - Invite link to BullTrades: [https://discord.gg/bulltrades](https://bulltrades.net/?ref=ndrjogi)
+Supports any Discord channel with structured BTP/STC alerts as message contents (not embedded, yet)
 
 
-Let me know if you find the package useful or need support by dropping me an email or visiting the [discord server](https://discord.gg/9ejghcjpar)
+Let me know if you find the package useful or need support by dropping me a DM @MinkysTradus or visiting the [discord server](https://discord.gg/9ejghcjpar)
 
  ________________________
 <img src="media/GUI_analysts_portfolio.PNG" alt="Analysts Portfolio" width="500" height="300">
 <img src="media/GUI_messages.PNG" alt="Channel message history" width="500" height="300">
 (older version shots)
 <img src="media/xtrader_console.png" alt="Console with discord messages" width="500" height="300">
 <img src="media/xtrader_portfolio.png" alt="Portfolio" width="500" height="300">
@@ -50,14 +52,17 @@
  ## Discord user token and channel IDs
  ______________________________
 
 It requires a user discord token, once installed the package saves the token in config.ini[discord], as well as the channel ID where alerts are posted.
 To get the discord token follow the instructions: https://www.androidauthority.com/get-discord-token-3149920/
 To get the channel ID, in Discord right click on the channel and click "Copy Channel ID"
 
+**Automation of user accounts is against Discord ToS. This package only read alerts and Discord can not detect automation behavior,
+however, if you want to follow Discords ToS, do not provide a user token and manually input the alerts at the bottom of the GUI to
+manually trigger the alerts ;)**
 
 ## Installation and Setup
  ______________________________
 
 1. Install Python:
    - For Windows, open PowerShell and run the following command, verify that it prints out "Hello World!":
      ```powershell
```

### Comparing `DiscordAlertsTrader-1.0.0/setup.py` & `DiscordAlertsTrader-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     for line in (line.strip() for line in fid):
         if line.startswith('__version__'):
             version = line.split('=')[1].strip().strip('\'')
             break
 
 setup(
     name='DiscordAlertsTrader',
-    version='1.0.0',
+    version='1.0.1',
     author='Adonay Nunes',
     author_email='adonays.nunes@gmail.com',
     description='Package for automating discord trade alerts in TDA or eTrade.',
     license='BSD (3-clause)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='',
```

### Comparing `DiscordAlertsTrader-1.0.0/tests/mock_discord_message.py` & `DiscordAlertsTrader-1.0.1/tests/mock_discord_message.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_AlertsTracker.py` & `DiscordAlertsTrader-1.0.1/tests/test_AlertsTracker.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_AlertsTrader.py` & `DiscordAlertsTrader-1.0.1/tests/test_AlertsTrader.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_AlertsTrader_exits.py` & `DiscordAlertsTrader-1.0.1/tests/test_AlertsTrader_exits.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_TDA.py` & `DiscordAlertsTrader-1.0.1/tests/test_TDA.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_configurator.py` & `DiscordAlertsTrader-1.0.1/tests/test_configurator.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_discord_bot.py` & `DiscordAlertsTrader-1.0.1/tests/test_discord_bot.py`

 * *Files identical despite different names*

### Comparing `DiscordAlertsTrader-1.0.0/tests/test_msg_parsed.py` & `DiscordAlertsTrader-1.0.1/tests/test_msg_parsed.py`

 * *Files identical despite different names*

