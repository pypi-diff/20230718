# Comparing `tmp/envisionriskraas-0.1.0.tar.gz` & `tmp/envisionriskraas-0.2.0.tar.gz`

## Comparing `envisionriskraas-0.1.0.tar` & `envisionriskraas-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    88302 2020-02-02 00:00:00.000000 envisionriskraas-0.1.0/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-0.1.0/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 envisionriskraas-0.1.0/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 envisionriskraas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    86296 2020-02-02 00:00:00.000000 envisionriskraas-0.2.0/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-0.2.0/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 envisionriskraas-0.2.0/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 envisionriskraas-0.2.0/PKG-INFO
```

### Comparing `envisionriskraas-0.1.0/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-0.2.0/src/EnvisionRiskRaaS/RAAS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1777,16 +1777,16 @@
             "base_cur": base_cur,
             "signif_level": signif_level
         }
         params = {k: v for k, v in params.items() if v is not None}
 
         res_out = envrsk_post(url=api_url, access_token=get_access_token(), params=params, body=backtestdata)
 
-        if result_backtest["status_code"] == 200:
-            out_raw = result_backtest["content"]
+        if res_out["status_code"] == 200:
+            out_raw = res_out["content"]
 
             backtestdata_in = out_raw["Input"]["BacktestData"]
             dt_backtestdata_in = pd.DataFrame.from_dict(backtestdata_in, orient='columns')        
 
             backtestdata_out = out_raw["Output"]
             dt_backtestdata_out = pd.DataFrame.from_dict(backtestdata_out, orient='columns')        
             
@@ -1930,56 +1930,7 @@
                 },
                 "UnMappedSymbols": pd.DataFrame(out_raw["Output"]["UnmappedSymbols"])
             }
         else:
             return res_out
 
         return out
-
-#******************************************************************************
-#### Miscellaneous ####
-#******************************************************************************
-def envrsk_decorate_portfolio_with_product_type(positions, simplify=True):
-    """
-    Function to enrich portfolio position data with additional information based on position ID.
-
-    Parameters:
-    positions (pd.DataFrame): A list of positions to be enriched with additional information.
-    simplify (bool, optional): Logical, indicating whether to simplify the output.
-
-    Returns:
-    pd.DataFrame or requests.Response: If the API call is successful, a dataframe containing the 
-                                       enriched positions is returned. If the API call is unsuccessful, 
-                                       the original API response is returned.
-
-    Examples:
-    dt_positions_without_product_type = pd.DataFrame({
-        "symbol": ["AAPL.US", "DANSKE.CO", "CashUSD", "AGG.US"],
-        "quantity": [129, 768, 69000, 89]
-    })
-    dt_positions = envrsk_decorate_portfolio_with_product_type(positions=dt_positions_without_product_type)
-    """
-    if os.getenv("LOGGED_IN") != 'Yes':
-        return {"message": "Please login before using the functionality - use 'envrsk_auth_log_in()' or 'envrsk_auth_log_in_interactively()'"}
-    else:
-        end_point = "decorate-position-id"
-        api_url = get_api_url(end_point)
-
-        res_out = requests.post(
-            url=api_url,
-            headers={"Authorization": f"Bearer {get_access_token()}"},
-            json=positions.to_dict()
-        )
-
-        if res_out["status_code]" == 200:
-            
-            out = res_out["content"]
-
-            if "Output" in out:
-                out["Output"] = pd.DataFrame(out["Output"])
-
-            if simplify:
-                return out["Output"]
-            else:
-                return out
-        else:
-            return res_out
```

### Comparing `envisionriskraas-0.1.0/LICENSE.txt` & `envisionriskraas-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-0.1.0/README.md` & `envisionriskraas-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `envisionriskraas-0.1.0/pyproject.toml` & `envisionriskraas-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "EnvisionRiskRaas"
-version = "0.1.0"
+name = "EnvisionRiskRaaS"
+version = "0.2.0"
 authors = [
   { name="Jonas Hal", email="jonas.hal@envisionrisk.com" },
 ]
 description = "EnvisionRisk's Risk as a service package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `envisionriskraas-0.1.0/PKG-INFO` & `envisionriskraas-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: EnvisionRiskRaas
-Version: 0.1.0
+Name: EnvisionRiskRaaS
+Version: 0.2.0
 Summary: EnvisionRisk's Risk as a service package
 Project-URL: Homepage, https://www.envisionrisk.com/
 Project-URL: GitHub profile, https://github.com/EnvisionRisk
 Author-email: Jonas Hal <jonas.hal@envisionrisk.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

