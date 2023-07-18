# Comparing `tmp/tainstcalorimetry-0.1.8.tar.gz` & `tmp/tainstcalorimetry-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tainstcalorimetry-0.1.8.tar", max compression
+gzip compressed data, was "tainstcalorimetry-0.1.9.tar", max compression
```

## Comparing `tainstcalorimetry-0.1.8.tar` & `tainstcalorimetry-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    35821 2022-12-30 15:49:02.340925 tainstcalorimetry-0.1.8/LICENSE
--rw-r--r--   0        0        0     1563 2023-03-20 15:50:18.177975 tainstcalorimetry-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7323 2023-03-20 15:26:22.033699 tainstcalorimetry-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-01-25 17:11:07.300092 tainstcalorimetry-0.1.8/TAInstCalorimetry/__init__.py
--rw-r--r--   0        0        0  2012712 2023-01-25 17:11:07.295105 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/c3a.csv
--rw-r--r--   0        0        0   435544 2023-02-19 17:35:10.285212 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_1.csv
--rw-r--r--   0        0        0   580847 2023-02-17 15:50:49.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_2.csv
--rw-r--r--   0        0        0   434569 2023-02-19 17:35:10.279229 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_3.csv
--rw-r--r--   0        0        0  2053989 2023-02-17 15:50:49.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_4.csv
--rw-r--r--   0        0        0  2057263 2023-02-17 15:50:49.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_5.csv
--rw-r--r--   0        0        0    99788 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp1.csv
--rw-r--r--   0        0        0    93604 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp2.csv
--rw-r--r--   0        0        0    99923 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp3.csv
--rw-r--r--   0        0        0    93849 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp4.csv
--rw-r--r--   0        0        0    93666 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp5.csv
--rw-r--r--   0        0        0    93920 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp6.csv
--rw-r--r--   0        0        0    93554 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp7.csv
--rw-r--r--   0        0        0    93848 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp8.csv
--rw-r--r--   0        0        0   575488 2023-01-25 17:11:07.283137 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/OPC_1.xls
--rw-r--r--   0        0        0   380416 2023-01-25 17:11:07.286129 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/OPC_2.xls
--rw-r--r--   0        0        0   587043 2023-01-25 17:11:07.299095 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/opc_3.csv
--rw-r--r--   0        0        0   939164 2023-02-18 08:43:35.343646 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/TEST_CALO_Gen1+2.csv
--rw-r--r--   0        0        0   425872 2023-02-19 17:34:54.786627 tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/TEST_CALO_Gen3.csv
--rw-r--r--   0        0        0    45341 2023-03-20 15:50:24.106211 tainstcalorimetry-0.1.8/TAInstCalorimetry/tacalorimetry.py
--rw-r--r--   0        0        0      471 2023-03-10 17:55:17.564094 tainstcalorimetry-0.1.8/TAInstCalorimetry/utils.py
--rw-r--r--   0        0        0     8277 1970-01-01 00:00:00.000000 tainstcalorimetry-0.1.8/setup.py
--rw-r--r--   0        0        0     8337 1970-01-01 00:00:00.000000 tainstcalorimetry-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35821 2022-12-30 15:49:02.340925 tainstcalorimetry-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1563 2023-05-23 17:16:29.060924 tainstcalorimetry-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9716 2023-03-20 16:38:03.841613 tainstcalorimetry-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-01-25 17:11:07.300092 tainstcalorimetry-0.1.9/TAInstCalorimetry/__init__.py
+-rw-r--r--   0        0        0  2012712 2023-01-25 17:11:07.295105 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/c3a.csv
+-rw-r--r--   0        0        0   435544 2023-02-19 17:35:10.285212 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_1.csv
+-rw-r--r--   0        0        0   580847 2023-02-17 15:50:49.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_2.csv
+-rw-r--r--   0        0        0   434569 2023-02-19 17:35:10.279229 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_3.csv
+-rw-r--r--   0        0        0  2053989 2023-02-17 15:50:49.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_4.csv
+-rw-r--r--   0        0        0  2057263 2023-02-17 15:50:49.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_5.csv
+-rw-r--r--   0        0        0    99788 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp1.csv
+-rw-r--r--   0        0        0    93604 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp2.csv
+-rw-r--r--   0        0        0    99923 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp3.csv
+-rw-r--r--   0        0        0    93849 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp4.csv
+-rw-r--r--   0        0        0    93666 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp5.csv
+-rw-r--r--   0        0        0    93920 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp6.csv
+-rw-r--r--   0        0        0    93554 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp7.csv
+-rw-r--r--   0        0        0    93848 2023-03-17 16:06:12.000000 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp8.csv
+-rw-r--r--   0        0        0   575488 2023-01-25 17:11:07.283137 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/OPC_1.xls
+-rw-r--r--   0        0        0   380416 2023-01-25 17:11:07.286129 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/OPC_2.xls
+-rw-r--r--   0        0        0   587043 2023-01-25 17:11:07.299095 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/opc_3.csv
+-rw-r--r--   0        0        0   939164 2023-02-18 08:43:35.343646 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/TEST_CALO_Gen1+2.csv
+-rw-r--r--   0        0        0   425872 2023-02-19 17:34:54.786627 tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/TEST_CALO_Gen3.csv
+-rw-r--r--   0        0        0    49112 2023-05-23 17:00:30.363392 tainstcalorimetry-0.1.9/TAInstCalorimetry/tacalorimetry.py
+-rw-r--r--   0        0        0      471 2023-03-10 17:55:17.564094 tainstcalorimetry-0.1.9/TAInstCalorimetry/utils.py
+-rw-r--r--   0        0        0    10678 1970-01-01 00:00:00.000000 tainstcalorimetry-0.1.9/PKG-INFO
```

### Comparing `tainstcalorimetry-0.1.8/LICENSE` & `tainstcalorimetry-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/pyproject.toml` & `tainstcalorimetry-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TAInstCalorimetry"
-version = "0.1.8"
+version = "0.1.9"
 description = "Handling TAM Air calorimetry files made easy."
 authors = [
     "mj-hofmann <aCodingChemist@gmail.com>",
     "tgaedt <torben.gaedt@tum.de>"
 ]
 license = "GNU GENERAL PUBLIC LICENSE"
```

### Comparing `tainstcalorimetry-0.1.8/README.md` & `tainstcalorimetry-0.1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ## Table of Contents  
 - [Example Usage](#example-usage)<br>
   - [Basic plotting](#basic-plotting)<br>
   - [Getting cumulated heat values](#getting-cumulated-heat-values)<br>
   - [Identifying peaks](#identifying-peaks)<br>
   - [Identifying peak onsets](#identifying-peak-onsets)<br>
+  - [Plotting by Category](#plotting-by-category)<br>
 - [Installation](#installation)<br>
 - [Contributing](#contributing)
 
 ## Example Usage
 
 Import the ```tacalorimetry``` module from **TAInstCalorimetry**.
 
@@ -144,14 +145,65 @@
     exclude_discarded_time=True,
     show_plot=True,
     regex="OPC"
 )
 ```
 ![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-01-26%20174524.png?raw=true)
 
+### Plotting by Category
+
+For introducing the idea of plotting calorimetry data "by category" another set of experimental data will be introduced. Next to the calorimetry data alone, information on investigated samples is supplied via an additional source file. In the present example via the file ```mini_metadata.csv```.
+
+To begin with, a ```TAInstCalorimetry.tacalorimetry.Measurement```-object is initialized for selected files from the specified ````path```.
+
+```python
+import pathlib
+from TAInstCalorimetry import tacalorimetry
+
+# path to experimental calorimetry files
+path = pathlib.Path().cwd().parent / "TAInstCalorimetry" / "DATA"
+
+# initialize TAInstCalorimetry.tacalorimetry.Measurement object
+tam_II = tacalorimetry.Measurement(
+    path, regex="myexp.*", show_info=True, cold_start=True, auto_clean=False
+)
+```
+
+Next, we need to connect the previously defined object to our metadata provided by the ```mini_metadata.csv```-file. To establish this mapping between experimental results and metadata, the file location, i.e. path, and the column name containing the exact(!) names of the calorimetry files needs to be passed to the ```add_metadata_source```-method. In our case, we declare the column ```experiment_nr``` for this purpose
+
+```python
+# add metadata
+tam.add_metadata_source("mini_metadata.csv", "experiment_nr")
+```
+
+Finally, a plotting by category can be carried out by one or multiple categories as shown in the following.
+
+```python
+# define action by one category
+categorize_by = "cement_name"  # 'date', 'cement_amount_g', 'water_amount_g'
+
+# # define action by two or more categories
+categorize_by = ["date", "cement_name"]
+
+# loop through plots via generator
+for this_plot in tam.plot_by_category(categorize_by):
+    # extract parts obtained from generator
+    category_value, ax = this_plot
+    # fine tuning of plot/cosmetics
+    ax.set_ylim(0, 3)
+    # show plot
+    tacalorimetry.plt.show()
+```
+
+This yields plots of the following kind.
+
+![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-03-20%20170659.png?raw=true)
+
+![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-03-20%20170711.png?raw=true)
+
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install TAInstCalorimetry.
 
 ```bash
 pip install TAInstCalorimetry
 ```
```

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/c3a.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/c3a.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_1.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_1.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_2.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_2.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_3.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_3.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_4.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_4.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/calorimetry_data_5.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/calorimetry_data_5.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp1.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp1.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp2.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp2.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp3.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp3.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp4.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp4.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp5.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp5.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp6.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp6.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp7.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp7.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/myexp8.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/myexp8.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/OPC_1.xls` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/OPC_1.xls`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/OPC_2.xls` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/OPC_2.xls`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/opc_3.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/opc_3.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/TEST_CALO_Gen1+2.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/TEST_CALO_Gen1+2.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/DATA/TEST_CALO_Gen3.csv` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/DATA/TEST_CALO_Gen3.csv`

 * *Files identical despite different names*

### Comparing `tainstcalorimetry-0.1.8/TAInstCalorimetry/tacalorimetry.py` & `tainstcalorimetry-0.1.9/TAInstCalorimetry/tacalorimetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -820,21 +820,42 @@
         for s, d in self.iter_samples():
             # define pattern
             if regex:
                 if not re.findall(rf"{regex}", os.path.basename(s)):
                     # go to next
                     continue
             # plot
-            plt.plot(
-                d["time_s"] * x_factor,
-                d[y_column] * y_factor,
-                label=os.path.basename(d["sample"].tolist()[0])
-                .split(".xls")[0]
-                .split(".csv")[0],
-            )
+            try:
+                # attempt mean and std plot
+                # mean plot
+                p_mean = plt.plot(
+                    d["time_s"] * x_factor,
+                    d[y_column, "mean"] * y_factor,
+                    label=os.path.basename(d["sample"].tolist()[0])
+                    .split(".xls")[0]
+                    .split(".csv")[0],
+                )
+                # std plot of "fill_between" type
+                plt.fill_between(
+                    d["time_s"] * x_factor,
+                    (d[y_column, "mean"] - d[y_column, "std"]) * y_factor,
+                    (d[y_column, "mean"] + d[y_column, "std"]) * y_factor,
+                    color=p_mean[0].get_color(),
+                    alpha=0.4,
+                    label=None,
+                )
+            except Exception:
+                # "standard plot"
+                plt.plot(
+                    d["time_s"] * x_factor,
+                    d[y_column] * y_factor,
+                    label=os.path.basename(d["sample"].tolist()[0])
+                    .split(".xls")[0]
+                    .split(".csv")[0],
+                )
 
         # legend
         plt.legend(loc="center left", bbox_to_anchor=(1, 0.5), frameon=False)
 
         # limits
         plt.xlim(left=0)
         plt.ylim(bottom=0)
@@ -1484,7 +1505,96 @@
         -------
         list
             list of categories avaialble for grouping by.
         """
 
         # get list based on column names of "_metadata"
         return self._metadata.columns.tolist()
+
+    #
+    # average by metadata
+    #
+    def average_by_metadata(
+        self,
+        group_by: str,
+        meta_id="experiment_nr",
+        data_id="sample_short",
+        time_average_window_s=60,
+        get_time_from="left",
+    ):
+        """
+
+
+        Parameters
+        ----------
+        group_by : str | list[str]
+            DESCRIPTION.
+        meta_id : TYPE, optional
+            DESCRIPTION. The default is "experiment_nr".
+        data_id : TYPE, optional
+            DESCRIPTION. The default is "sample_short".
+        time_average_window_s : TYPE, optional
+            DESCRIPTION. The default is 60.
+        get_time_from : TYPE, optional
+            DESCRIPTION. The default is "left". further options: # "mid" "right"
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # get metadata
+        meta, meta_id = self.get_metadata()
+
+        # get data
+        df = self._data
+
+        # rename sample in "data" by metadata grouping options
+        for value, group in meta.groupby(group_by):
+            # if one grouping level is used
+            if isinstance(value, str) or isinstance(value, int):
+                # modify data --> replace "sample_short" with metadata group name
+                _idx_to_replace = df[data_id].isin(group[meta_id])
+                df.loc[_idx_to_replace, data_id] = str(value)
+            # if multiple grouping levels are used
+            elif isinstance(value, tuple):
+                # modify data --> replace "sample_short" with metadata group name
+                _idx_to_replace = df[data_id].isin(group[meta_id])
+                df.loc[_idx_to_replace, data_id] = " | ".join([str(x) for x in value])
+            else:
+                pass
+
+        # sort experimentally detected times to "bins"
+        df["BIN"] = pd.cut(
+            df["time_s"], np.arange(0, 2 * 24 * 60 * 60, time_average_window_s)
+        )
+
+        # calculate average and std
+        df = (
+            df.groupby([data_id, "BIN"])
+            .agg(
+                {
+                    "normalized_heat_flow_w_g": ["mean", "std"],
+                    "normalized_heat_j_g": ["mean", "std"],
+                }
+            )
+            .dropna(thresh=2)
+            .reset_index()
+        )
+
+        # regain "time_s" columns
+        if get_time_from == "left":
+            df["time_s"] = [i.left for i in df["BIN"]]
+        elif get_time_from == "mid":
+            df["time_s"] = [i.mid for i in df["BIN"]]
+        elif get_time_from == "right":
+            df["time_s"] = [i.right for i in df["BIN"]]
+
+        # remove "BIN" auxiliary column
+        del df["BIN"]
+
+        # copy information to "sample" column --> needed for plotting
+        df["sample"] = df[data_id]
+
+        # overwrite data
+        self._data = df
```

### Comparing `tainstcalorimetry-0.1.8/setup.py` & `tainstcalorimetry-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,259 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tainstcalorimetry
+Version: 0.1.9
+Summary: Handling TAM Air calorimetry files made easy.
+Home-page: https://github.com/mj-hofmann/TAInstCalorimetry
+License: GNU GENERAL PUBLIC LICENSE
+Keywords: calorimetry,TAM Air,TA Instruments,analysis,vizualisation
+Author: mj-hofmann
+Author-email: aCodingChemist@gmail.com
+Requires-Python: >=3.7,<3.12
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
+Requires-Dist: mypy (>=0.991,<0.992)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pysnooper (>=1.1.1,<2.0.0)
+Requires-Dist: pytest (>=7.2.0,<8.0.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/mj-hofmann/TAInstCalorimetry
+Description-Content-Type: text/markdown
 
-packages = \
-['tainstcalorimetry']
+![Logo](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/icon/icon.png?raw=true)
 
-package_data = \
-{'': ['*'], 'tainstcalorimetry': ['DATA/*']}
+# Interfacing with experimental results file from TAM Air calorimeters made easy.
 
-install_requires = \
-['matplotlib>=3.6.3,<4.0.0',
- 'mypy>=0.991,<0.992',
- 'pandas>=1.5.3,<2.0.0',
- 'pysnooper>=1.1.1,<2.0.0',
- 'pytest-cov>=4.0.0,<5.0.0',
- 'pytest>=7.2.0,<8.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'scipy>=1.10.0,<2.0.0',
- 'xlrd>=2.0.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'tainstcalorimetry',
-    'version': '0.1.8',
-    'description': 'Handling TAM Air calorimetry files made easy.',
-    'long_description': '![Logo](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/icon/icon.png?raw=true)\n\n# Interfacing with experimental results file from TAM Air calorimeters made easy.\n\nAfter collecting multiple experimental results files from a TAM Air calorimeter you will be left with multiple *.xls*-files obtained as exports from the device control software. To achieve a side by side comparison of theses results and some basic extraction of relevant parameters, **TAInstCalorimetry** is here to get this done smoothly.\n\n*Note: **TAInstCalorimetry** has been developed without involvement of **TA Instruments** and is thus independent from the company and its software.*\n\n## Info / Downloads\n\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/tainstcalorimetry.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pepy.tech/project/tainstcalorimetry)\n[![PyPI - Downloads](https://static.pepy.tech/personalized-badge/tainstcalorimetry?period=total&units=none&left_color=black&right_color=grey&left_text=Downloads)](https://pepy.tech/project/tainstcalorimetry)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tainstcalorimetry.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/tainstcalorimetry/) \n\n## Table of Contents  \n- [Example Usage](#example-usage)<br>\n  - [Basic plotting](#basic-plotting)<br>\n  - [Getting cumulated heat values](#getting-cumulated-heat-values)<br>\n  - [Identifying peaks](#identifying-peaks)<br>\n  - [Identifying peak onsets](#identifying-peak-onsets)<br>\n- [Installation](#installation)<br>\n- [Contributing](#contributing)\n\n## Example Usage\n\nImport the ```tacalorimetry``` module from **TAInstCalorimetry**.\n\n```python\n# import\nimport os\nfrom TAInstCalorimetry import tacalorimetry\n```\n\nNext, we define where the exported files are stored. With this information at hand, a ```Measurement``` is initialized. Experimental raw data and the metadata passed in the course of the measurement are retrieved by the methods ```get_data()``` and ```get_information()```, respectively.\n\n```python\n# define data path\n# "mycalodata" is the subfoldername where the calorimetry\n# data files (both .csv or .xlsx) are stored\n\npathname = os.path.dirname(os.path.realpath(__file__))\npath_to_data = pathname + os.sep + "mycalodata"\n\n# Example: if projectfile is at "C:\\Users\\myname\\myproject\\myproject.py", then "mydata"\n# refers to "C:\\Users\\myname\\myproject\\mycalodata" where the data is stored\n\n# load experiments via class, i.e. instantiate tacalorimetry object with data\ntam = tacalorimetry.Measurement(folder=path_to_data)\n\n# get sample and information\ndata = tam.get_data()\ninfo = tam.get_information()\n```\n\n### Basic plotting\n\nFurthermore, the ```Measurement``` features a ```plot()```-method for readily visualizing the collected results.\n\n```python\n# make plot\ntam.plot()\n# show plot\ntacalorimetry.plt.show()\n```\n\nWithout further options specified, the ```plot()```-method yields the following.\n\n![enter image description here](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202022-08-08%20112743.png?raw=true)\n\nThe ```plot()```-method can also be tuned to show the temporal course of normalized heat. On the one hand, this "tuning" refers to the specification of further keyword arguments such as ```t_unit``` and ```y```. On the other hand, the ```plot()```-method returns an object of type ```matplotlib.axes._subplots.AxesSubplot```, which can be used to further customize the plot. In the following, a guide-to-the-eye line is introduced next to adjuting the axes limts, which is not provided for via the ```plot()```-method\'s signature.\n\n```python\n# show cumulated heat plot\nax = tam.plot(\n    t_unit="h",\n    y=\'normalized_heat\',\n    y_unit_milli=False\n)\n\n# define target time\ntarget_h = 1.5\n\n# guide to the eye line\nax.axvline(target_h, color="gray", alpha=0.5, linestyle=":")\n\n# set upper limits\nax.set_ylim(top=250)\nax.set_xlim(right=6)\n# show plot\ntacalorimetry.plt.show()\n```\nThe following plot is obtained:\n\n![enter image description here](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202022-08-19%20085928.png?raw=true)\n\n### Getting cumulated heat values\n\nThe cumulated heat after a certain period of time ```target_h``` from starting the measurement is a relevant quantity for answering different types of questions. For this purpose, the method ```get_cumulated_heat_at_hours``` returns an overview of this parameter for all the samples in the specified folder.\n\n```python\n# get table of cumulated heat at certain age\ncumulated_heats = tam.get_cumulated_heat_at_hours(\n          target_h=target_h,\n          cutoff_min=10\n          )\n          \n# show result\nprint(cumulated_heats)\n```\n\nThe return value of the method, ```cumulated_heats``` is a ```pd.DataFrame```.\n\n### Identifying peaks\n\nNext to cumulated heat values detected after a certain time frame from starting the reaction, peaks characteristics can be obtained from the experimental data via the ```get_peaks```-method.\n\n```python\n# get peaks\npeaks = tam.get_peaks(\n    show_plot=True,\n    prominence=0.00001,  # "sensitivity of peak picking"\n    cutoff_min=60,  # how much to discard at the beginning of the measurement\n    plt_right_s=4e5,\n    plt_top=1e-2,\n    regex=".*_\\d"  # filter samples\n    )\n```\n\nTweaking some of the available keyword arguments, the following plot is obtained:\n\n![Identified peaks for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-01-25%20193222.png?raw=true)\n\nPlease keep in mind, that in particular for samples of ordinary Portland cement (OPC) a clear and unambiguous identification/assigment of peaks remains a challenging task which cannot be achieved in each and every case by **TAInstCalorimetry**. It is left to the user draw meaningful scientific conclusions from the characteristics derived from this method.\n\n### Identifying peak onsets\n\nSimilarly, the peak onset characteristics are accessible via the ```get_peak_onsets```-method. The resulting plot is shown below.\n\n```python\n# get onsets\nonsets = tam.get_peak_onsets(\n    gradient_threshold=0.000001,\n    rolling=10,\n    exclude_discarded_time=True,\n    show_plot=True,\n    regex="OPC"\n)\n```\n![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-01-26%20174524.png?raw=true)\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install TAInstCalorimetry.\n\n```bash\npip install TAInstCalorimetry\n```\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\nList of contributors:\n- [mj-hofmann](https://github.com/mj-hofmann)\n- [tgaedt](https://github.com/tgaedt)\n\n## License\n[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/#)\n\n\n## Test\n![Tests](https://github.com/mj-hofmann/TAInstCalorimetry/actions/workflows/run-tests.yml/badge.svg)\n\n## Code Styling\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n',
-    'author': 'mj-hofmann',
-    'author_email': 'aCodingChemist@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mj-hofmann/TAInstCalorimetry',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.12',
-}
+After collecting multiple experimental results files from a TAM Air calorimeter you will be left with multiple *.xls*-files obtained as exports from the device control software. To achieve a side by side comparison of theses results and some basic extraction of relevant parameters, **TAInstCalorimetry** is here to get this done smoothly.
 
+*Note: **TAInstCalorimetry** has been developed without involvement of **TA Instruments** and is thus independent from the company and its software.*
+
+## Info / Downloads
+
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/tainstcalorimetry.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pepy.tech/project/tainstcalorimetry)
+[![PyPI - Downloads](https://static.pepy.tech/personalized-badge/tainstcalorimetry?period=total&units=none&left_color=black&right_color=grey&left_text=Downloads)](https://pepy.tech/project/tainstcalorimetry)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tainstcalorimetry.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/tainstcalorimetry/) 
+
+## Table of Contents  
+- [Example Usage](#example-usage)<br>
+  - [Basic plotting](#basic-plotting)<br>
+  - [Getting cumulated heat values](#getting-cumulated-heat-values)<br>
+  - [Identifying peaks](#identifying-peaks)<br>
+  - [Identifying peak onsets](#identifying-peak-onsets)<br>
+  - [Plotting by Category](#plotting-by-category)<br>
+- [Installation](#installation)<br>
+- [Contributing](#contributing)
+
+## Example Usage
+
+Import the ```tacalorimetry``` module from **TAInstCalorimetry**.
+
+```python
+# import
+import os
+from TAInstCalorimetry import tacalorimetry
+```
+
+Next, we define where the exported files are stored. With this information at hand, a ```Measurement``` is initialized. Experimental raw data and the metadata passed in the course of the measurement are retrieved by the methods ```get_data()``` and ```get_information()```, respectively.
+
+```python
+# define data path
+# "mycalodata" is the subfoldername where the calorimetry
+# data files (both .csv or .xlsx) are stored
+
+pathname = os.path.dirname(os.path.realpath(__file__))
+path_to_data = pathname + os.sep + "mycalodata"
+
+# Example: if projectfile is at "C:\Users\myname\myproject\myproject.py", then "mydata"
+# refers to "C:\Users\myname\myproject\mycalodata" where the data is stored
+
+# load experiments via class, i.e. instantiate tacalorimetry object with data
+tam = tacalorimetry.Measurement(folder=path_to_data)
+
+# get sample and information
+data = tam.get_data()
+info = tam.get_information()
+```
+
+### Basic plotting
+
+Furthermore, the ```Measurement``` features a ```plot()```-method for readily visualizing the collected results.
+
+```python
+# make plot
+tam.plot()
+# show plot
+tacalorimetry.plt.show()
+```
+
+Without further options specified, the ```plot()```-method yields the following.
+
+![enter image description here](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202022-08-08%20112743.png?raw=true)
+
+The ```plot()```-method can also be tuned to show the temporal course of normalized heat. On the one hand, this "tuning" refers to the specification of further keyword arguments such as ```t_unit``` and ```y```. On the other hand, the ```plot()```-method returns an object of type ```matplotlib.axes._subplots.AxesSubplot```, which can be used to further customize the plot. In the following, a guide-to-the-eye line is introduced next to adjuting the axes limts, which is not provided for via the ```plot()```-method's signature.
+
+```python
+# show cumulated heat plot
+ax = tam.plot(
+    t_unit="h",
+    y='normalized_heat',
+    y_unit_milli=False
+)
+
+# define target time
+target_h = 1.5
+
+# guide to the eye line
+ax.axvline(target_h, color="gray", alpha=0.5, linestyle=":")
+
+# set upper limits
+ax.set_ylim(top=250)
+ax.set_xlim(right=6)
+# show plot
+tacalorimetry.plt.show()
+```
+The following plot is obtained:
+
+![enter image description here](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202022-08-19%20085928.png?raw=true)
+
+### Getting cumulated heat values
+
+The cumulated heat after a certain period of time ```target_h``` from starting the measurement is a relevant quantity for answering different types of questions. For this purpose, the method ```get_cumulated_heat_at_hours``` returns an overview of this parameter for all the samples in the specified folder.
+
+```python
+# get table of cumulated heat at certain age
+cumulated_heats = tam.get_cumulated_heat_at_hours(
+          target_h=target_h,
+          cutoff_min=10
+          )
+          
+# show result
+print(cumulated_heats)
+```
+
+The return value of the method, ```cumulated_heats``` is a ```pd.DataFrame```.
+
+### Identifying peaks
+
+Next to cumulated heat values detected after a certain time frame from starting the reaction, peaks characteristics can be obtained from the experimental data via the ```get_peaks```-method.
+
+```python
+# get peaks
+peaks = tam.get_peaks(
+    show_plot=True,
+    prominence=0.00001,  # "sensitivity of peak picking"
+    cutoff_min=60,  # how much to discard at the beginning of the measurement
+    plt_right_s=4e5,
+    plt_top=1e-2,
+    regex=".*_\d"  # filter samples
+    )
+```
+
+Tweaking some of the available keyword arguments, the following plot is obtained:
+
+![Identified peaks for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-01-25%20193222.png?raw=true)
+
+Please keep in mind, that in particular for samples of ordinary Portland cement (OPC) a clear and unambiguous identification/assigment of peaks remains a challenging task which cannot be achieved in each and every case by **TAInstCalorimetry**. It is left to the user draw meaningful scientific conclusions from the characteristics derived from this method.
+
+### Identifying peak onsets
+
+Similarly, the peak onset characteristics are accessible via the ```get_peak_onsets```-method. The resulting plot is shown below.
+
+```python
+# get onsets
+onsets = tam.get_peak_onsets(
+    gradient_threshold=0.000001,
+    rolling=10,
+    exclude_discarded_time=True,
+    show_plot=True,
+    regex="OPC"
+)
+```
+![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-01-26%20174524.png?raw=true)
+
+### Plotting by Category
+
+For introducing the idea of plotting calorimetry data "by category" another set of experimental data will be introduced. Next to the calorimetry data alone, information on investigated samples is supplied via an additional source file. In the present example via the file ```mini_metadata.csv```.
+
+To begin with, a ```TAInstCalorimetry.tacalorimetry.Measurement```-object is initialized for selected files from the specified ````path```.
+
+```python
+import pathlib
+from TAInstCalorimetry import tacalorimetry
+
+# path to experimental calorimetry files
+path = pathlib.Path().cwd().parent / "TAInstCalorimetry" / "DATA"
+
+# initialize TAInstCalorimetry.tacalorimetry.Measurement object
+tam_II = tacalorimetry.Measurement(
+    path, regex="myexp.*", show_info=True, cold_start=True, auto_clean=False
+)
+```
+
+Next, we need to connect the previously defined object to our metadata provided by the ```mini_metadata.csv```-file. To establish this mapping between experimental results and metadata, the file location, i.e. path, and the column name containing the exact(!) names of the calorimetry files needs to be passed to the ```add_metadata_source```-method. In our case, we declare the column ```experiment_nr``` for this purpose
+
+```python
+# add metadata
+tam.add_metadata_source("mini_metadata.csv", "experiment_nr")
+```
+
+Finally, a plotting by category can be carried out by one or multiple categories as shown in the following.
+
+```python
+# define action by one category
+categorize_by = "cement_name"  # 'date', 'cement_amount_g', 'water_amount_g'
+
+# # define action by two or more categories
+categorize_by = ["date", "cement_name"]
+
+# loop through plots via generator
+for this_plot in tam.plot_by_category(categorize_by):
+    # extract parts obtained from generator
+    category_value, ax = this_plot
+    # fine tuning of plot/cosmetics
+    ax.set_ylim(0, 3)
+    # show plot
+    tacalorimetry.plt.show()
+```
+
+This yields plots of the following kind.
+
+![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-03-20%20170659.png?raw=true)
+
+![Identified peak onsets for one sample.](https://github.com/mj-hofmann/TAInstCalorimetry/blob/main/tests/plots/Figure%202023-03-20%20170711.png?raw=true)
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install TAInstCalorimetry.
+
+```bash
+pip install TAInstCalorimetry
+```
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+List of contributors:
+- [mj-hofmann](https://github.com/mj-hofmann)
+- [tgaedt](https://github.com/tgaedt)
+
+## License
+[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/#)
+
+
+## Test
+![Tests](https://github.com/mj-hofmann/TAInstCalorimetry/actions/workflows/run-tests.yml/badge.svg)
+
+## Code Styling
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-setup(**setup_kwargs)
```

