# Comparing `tmp/DyLoPro-0.1.0.tar.gz` & `tmp/DyLoPro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DyLoPro-0.1.0.tar", last modified: Wed Jun 28 16:58:26 2023, max compression
+gzip compressed data, was "DyLoPro-0.1.1.tar", last modified: Tue Jul 18 15:33:39 2023, max compression
```

## Comparing `DyLoPro-0.1.0.tar` & `DyLoPro-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 16:58:26.141895 DyLoPro-0.1.0/
--rw-rw-rw-   0        0        0      138 2023-06-28 14:58:32.000000 DyLoPro-0.1.0/AUTHORS.md
--rw-rw-rw-   0        0        0     3038 2023-06-28 15:52:03.000000 DyLoPro-0.1.0/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2023-06-28 16:58:26.094021 DyLoPro-0.1.0/DyLoPro/
--rw-rw-rw-   0        0        0    93085 2023-06-14 13:56:31.000000 DyLoPro-0.1.0/DyLoPro/DynamicLogPlotting.py
--rw-rw-rw-   0        0        0      880 2023-06-27 11:47:01.000000 DyLoPro-0.1.0/DyLoPro/__init__.py
--rw-rw-rw-   0        0        0    33331 2023-06-14 13:56:31.000000 DyLoPro-0.1.0/DyLoPro/check_args.py
--rw-rw-rw-   0        0        0     4276 2023-06-14 13:56:31.000000 DyLoPro-0.1.0/DyLoPro/plot_components.py
--rw-rw-rw-   0        0        0    30364 2023-06-14 13:56:31.000000 DyLoPro-0.1.0/DyLoPro/plotting_utils.py
--rw-rw-rw-   0        0        0    15204 2023-06-21 13:04:53.000000 DyLoPro-0.1.0/DyLoPro/preprocess_utils.py
--rw-rw-rw-   0        0        0   226284 2023-06-14 13:56:31.000000 DyLoPro-0.1.0/DyLoPro/univariate_plots.py
--rw-rw-rw-   0        0        0    22813 2023-06-14 13:56:31.000000 DyLoPro-0.1.0/DyLoPro/validate_methods.py
-drwxrwxrwx   0        0        0        0 2023-06-28 16:58:26.130923 DyLoPro-0.1.0/DyLoPro.egg-info/
--rw-rw-rw-   0        0        0     2301 2023-06-28 16:58:25.000000 DyLoPro-0.1.0/DyLoPro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      729 2023-06-28 16:58:25.000000 DyLoPro-0.1.0/DyLoPro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 16:58:25.000000 DyLoPro-0.1.0/DyLoPro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-28 16:58:25.000000 DyLoPro-0.1.0/DyLoPro.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       59 2023-06-28 16:58:25.000000 DyLoPro-0.1.0/DyLoPro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-28 16:58:25.000000 DyLoPro-0.1.0/DyLoPro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-06-27 16:03:29.000000 DyLoPro-0.1.0/HISTORY.md
--rw-rw-rw-   0        0        0     1573 2023-06-21 08:44:35.000000 DyLoPro-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      251 2023-06-28 16:03:20.000000 DyLoPro-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2301 2023-06-28 16:58:26.141895 DyLoPro-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1155 2023-06-28 16:01:27.000000 DyLoPro-0.1.0/README.md
--rw-rw-rw-   0        0        0      450 2023-06-28 16:58:26.144886 DyLoPro-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1794 2023-06-28 16:50:16.000000 DyLoPro-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 16:58:26.140898 DyLoPro-0.1.0/tests/
--rw-rw-rw-   0        0        0       38 2023-06-21 08:44:35.000000 DyLoPro-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      577 2023-06-21 08:44:35.000000 DyLoPro-0.1.0/tests/test_DyLoPro.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:39:08.000000 DyLoPro-0.1.0/tests/test_DynamicLogPlotting.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:39:19.000000 DyLoPro-0.1.0/tests/test_check_args.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:39:28.000000 DyLoPro-0.1.0/tests/test_plot_components.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:39:40.000000 DyLoPro-0.1.0/tests/test_plotting_utils.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:40:22.000000 DyLoPro-0.1.0/tests/test_preprocess_utils.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:40:32.000000 DyLoPro-0.1.0/tests/test_univariate_plots.py
--rw-rw-rw-   0        0        0        0 2023-06-27 15:40:47.000000 DyLoPro-0.1.0/tests/test_validate_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:33:39.256402 DyLoPro-0.1.1/
+-rw-rw-rw-   0        0        0      138 2023-06-28 14:58:32.000000 DyLoPro-0.1.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     3177 2023-07-06 15:36:36.000000 DyLoPro-0.1.1/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2023-07-18 15:33:39.176639 DyLoPro-0.1.1/DyLoPro/
+-rw-rw-rw-   0        0        0   101418 2023-07-18 15:20:12.000000 DyLoPro-0.1.1/DyLoPro/DynamicLogPlotting.py
+-rw-rw-rw-   0        0        0      880 2023-07-06 16:35:25.000000 DyLoPro-0.1.1/DyLoPro/__init__.py
+-rw-rw-rw-   0        0        0    33331 2023-06-14 13:56:31.000000 DyLoPro-0.1.1/DyLoPro/check_args.py
+-rw-rw-rw-   0        0        0     3973 2023-07-05 08:15:02.000000 DyLoPro-0.1.1/DyLoPro/plot_components.py
+-rw-rw-rw-   0        0        0    33276 2023-07-05 10:55:14.000000 DyLoPro-0.1.1/DyLoPro/plotting_utils.py
+-rw-rw-rw-   0        0        0    15204 2023-06-21 13:04:53.000000 DyLoPro-0.1.1/DyLoPro/preprocess_utils.py
+-rw-rw-rw-   0        0        0   226284 2023-06-14 13:56:31.000000 DyLoPro-0.1.1/DyLoPro/univariate_plots.py
+-rw-rw-rw-   0        0        0    22813 2023-06-14 13:56:31.000000 DyLoPro-0.1.1/DyLoPro/validate_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:33:39.227502 DyLoPro-0.1.1/DyLoPro.egg-info/
+-rw-rw-rw-   0        0        0    16839 2023-07-18 15:33:38.000000 DyLoPro-0.1.1/DyLoPro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      729 2023-07-18 15:33:38.000000 DyLoPro-0.1.1/DyLoPro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:33:38.000000 DyLoPro-0.1.1/DyLoPro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 15:33:38.000000 DyLoPro-0.1.1/DyLoPro.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       59 2023-07-18 15:33:38.000000 DyLoPro-0.1.1/DyLoPro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 15:33:38.000000 DyLoPro-0.1.1/DyLoPro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      690 2023-07-05 12:42:17.000000 DyLoPro-0.1.1/HISTORY.md
+-rw-rw-rw-   0        0        0     1556 2023-06-29 14:28:52.000000 DyLoPro-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-06-28 16:03:20.000000 DyLoPro-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    16839 2023-07-18 15:33:39.257399 DyLoPro-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15052 2023-07-18 15:25:58.000000 DyLoPro-0.1.1/README.md
+-rw-rw-rw-   0        0        0      450 2023-07-18 15:33:39.259394 DyLoPro-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1794 2023-07-06 16:35:25.000000 DyLoPro-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:33:39.255402 DyLoPro-0.1.1/tests/
+-rw-rw-rw-   0        0        0       38 2023-06-21 08:44:35.000000 DyLoPro-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-06-21 08:44:35.000000 DyLoPro-0.1.1/tests/test_DyLoPro.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:39:08.000000 DyLoPro-0.1.1/tests/test_DynamicLogPlotting.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:39:19.000000 DyLoPro-0.1.1/tests/test_check_args.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:39:28.000000 DyLoPro-0.1.1/tests/test_plot_components.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:39:40.000000 DyLoPro-0.1.1/tests/test_plotting_utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:40:22.000000 DyLoPro-0.1.1/tests/test_preprocess_utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:40:32.000000 DyLoPro-0.1.1/tests/test_univariate_plots.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:40:47.000000 DyLoPro-0.1.1/tests/test_validate_methods.py
```

### Comparing `DyLoPro-0.1.0/CONTRIBUTING.md` & `DyLoPro-0.1.1/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 
 If you are reporting a bug, please include:
 
 - Your operating system name and version.
 - Any details about your local setup that might be helpful in troubleshooting.
 - Detailed steps to reproduce the bug.
 
+### Write Test Functions 
+
+
+Currently, the test folder contains empty test modules. These test modules 
+are still to be developed. 
+
 ### Fix Bugs
 
 
 Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
 wanted" is open to whoever wants to implement it.
 
 ### Implement Features
```

### Comparing `DyLoPro-0.1.0/DyLoPro/DynamicLogPlotting.py` & `DyLoPro-0.1.1/DyLoPro/DynamicLogPlotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,37 +85,43 @@
             Column name (in `event_log`) containing the binary case 
             outcome values (if present). By default `None`. Should be of 
             an integer dtype. See Notes for more details on how an 
             outcome column should be formatted.
 
         Notes
         -----
-        Formatting requirements specified columns in `event_log`: 
-        - `categorical_casefeatures` : Every column in `event_log` 
-        specified in this list has to be of one of the following dtypes: 
-        category, object, boolean. Furthermore, every event (row) 
-        pertaining to the same case (i.e. same case ID specified in the 
-        `case_id_key` column) should share the exact same value for each 
-        case feature. 
-        - `numerical_casefeatures` : Every column in `event_log` 
-        specified in this list has to be of a numerical dtype. 
-        Furthermore, every event (row) pertaining to the same case (i.e. 
-        same case ID specified in the `case_id_key` column) should share 
-        the exact same value for each case feature. 
-        - `categorical_eventfeatures` : Every column in `event_log` 
-        specified in this list has to be of one of the following dtypes: 
-        category, object, boolean. 
-        - `numerical_eventfeatures` : Every column in `event_log` 
-        specified in this list has to be of a numerical dtype. 
-        - `outcome`: An outcome column in `event_log` should be of an 
-        integer dtype, only contain the values `1` (positive cases) and 
-        `0` (negative cases). We regard outcome as case outcomes, and 
-        hence every event (row) pertaining to the same case (i.e. 
-        same case ID specified in the `case_id_key` column) should share 
-        the exact same value for the outcome. 
+        Formatting requirements specified columns in `event_log`:
+
+        * `categorical_casefeatures` : Every column in `event_log` 
+          specified in this list has to be of one of the following dtypes: 
+          category, object, boolean. Furthermore, every event (row) 
+          pertaining to the same case (i.e. same case ID specified in the 
+          `case_id_key` column) should share the exact same value for each 
+          case feature.
+
+        * `numerical_casefeatures` : Every column in `event_log` 
+          specified in this list has to be of a numerical dtype. 
+          Furthermore, every event (row) pertaining to the same case (i.e. 
+          same case ID specified in the `case_id_key` column) should share 
+          the exact same value for each case feature.
+
+        * `categorical_eventfeatures` : Every column in `event_log` 
+          specified in this list has to be of one of the following dtypes: 
+          category, object, boolean.
+
+        * `numerical_eventfeatures` : Every column in `event_log` 
+          specified in this list has to be of a numerical dtype.
+
+        * `outcome`: An outcome column in `event_log` should be of an 
+          integer dtype, only contain the values `1` (positive cases) and 
+          `0` (negative cases). We regard outcome as case outcomes, and 
+          hence every event (row) pertaining to the same case (i.e. 
+          same case ID specified in the `case_id_key` column) should share 
+          the exact same value for the outcome.
+
         """
         log = event_log.copy()
         valm._verify_initial(log, case_id_key, activity_key, timestamp_key, categorical_casefeatures, 
                     numerical_casefeatures, categorical_eventfeatures, numerical_eventfeatures, outcome, start_date, end_date)
 
         if case_id_key != 'case:concept:name':
             log.rename(columns = {case_id_key: 'case:concept:name'}, inplace = True)
@@ -143,28 +149,28 @@
         self.variant_df.columns = ['variant', 'variant count']
 
 
 
     # Plotting methods
         
     def topK_dfr_evol(self, time_unit = 'days', frequency = 'weekly', case_assignment = 'first_event', plt_type = 'univariate', numeric_agg = 'mean', max_k = 10, xtr_outlier_rem = True):
-        """Plot the time series of the requested aggregations for each of the 'max_k' 
+        """Plot the time series of the requested aggregations for each of the ``max_k`` 
         most frequently occurring Directly-Follows Relations (DFRs).
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. The requested DFR evolutions plotted are arranged in 
+        ``plt_type`` argument. The requested DFR evolutions plotted are arranged in 
         descending order of the number of occurrences of the DFRs.
 
         For readability, the DFRs are encoded with a number with DFR 1 being the most 
-        frequently occurring DFR, and DFR '`max_k`' being the max_k'th most occurring 
+        frequently occurring DFR, and DFR ``max_k`` being the max_k'th most occurring 
         DFR. To retrieve a dataframe that maps these DFR numbers to the actual 
-        activity pairs, the `get_DFR_df()` method of the `DynamicLogPlots` class can 
+        activity pairs, the ``get_DFR_df()`` method of the ``DynamicLogPlots`` class can 
         be called upon. 
 
         Parameters
         ----------
         time_unit : {'microseconds', 'milliseconds', 'seconds', 'minutes', 'hours', 'days', 'weeks'}
             Time unit in which the throughput time of cases is specified, by default `'days'`.
         frequency : {'minutely', '5-minutely', '10-minutely', 'half-hourly', 'hourly' '2-hourly', 
@@ -187,103 +193,119 @@
         xtr_outlier_rem : bool, optional
             If True, the vertical ranges of the plots are only determined by regular 
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
             its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
             its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
             case to the first time interval. 
-        - `plt_type` can take one of the following five values:
-            - `'univariate'`: For each DFR, the evolutions of the periodically aggregated 
+
+        * ``plt_type`` can take one of the following five values:
+
+          * `'univariate'`: For each DFR, the evolutions of the periodically aggregated 
             amount of occurrences per case, as well as the fraction of cases containing
             at least one occurance of of that DFR, are plotted. 
-            - `'type_tt'`: For each DFR, next to the univariate plots, also the evolutions of 
+
+          * `'type_tt'`: For each DFR, next to the univariate plots, also the evolutions of 
             the periodically aggregated Throughput Time (TT) for cases with vs. cases 
             without that DFR are plotted. 
-            - `'type_events_case'`: For each DFR, next to the univariate plots, also the evolutions of 
+
+          * `'type_events_case'`: For each DFR, next to the univariate plots, also the evolutions of 
             the periodically aggregated case length (in number of events per case (NEPC)) for cases 
             with vs. cases without that DFR are plotted. 
-            - `'type_outcome'`: For each DFR, next to the univariate plots, also the evolutions of 
+
+          * `'type_outcome'`: For each DFR, next to the univariate plots, also the evolutions of 
             the periodic fractions of cases with a positive outcome ('outcome=1') for cases with
             vs. cases without that DFR, are plotted. (Only applicable if an outcome is already 
             specified upon initialization of the `DynamicLogPlots` instance, or with the 
-            `set_outcomeColumn(outcome)` method.)
-            - `'type_dfr_performance'`: For each DFR, next to the univariate plots, also the 
+            ``set_outcomeColumn(outcome)`` method.)
+
+          * `'type_dfr_performance'`: For each DFR, next to the univariate plots, also the 
             evolution of the periodically aggregated DFR performance is plotted. The DFR 
-            performance refers to the time elapsed between the first and last activity of
+            performance refers to the time elapsed between the first and last activity of 
             that DFR. The time unit in which these periodic performance aggregations are 
-            expressed, is automatically determined based on their magnitude. __NOTE__ that 
+            expressed, is automatically determined based on their magnitude. **NOTE** that 
             the `'type_dfr_performance'` representation type is a special case, as it is 
             the only representation type in which cases can deliver more than one measure 
             for a certain DFR. I.e. cases that contain more than one occurrence of a 
             certain DFR will also deliver more than one value for the DFR performance to 
             be aggregated over. 
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='univariate'`, for each time interval, 
             and for each of the `max_k` DFRs, the mean amount of occurrences per case 
             is computed. The fraction of cases containing at least one occurrence of a 
             certain DFR is simply computed by, for each time interval, computing the 
             amount of cases with at least one occurrence, and dividing it by the total 
             amount of cases assigned to that time interval. 
-            - `'median'` : The requested time series are computed by taking the median for  
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` DFRs, the median amount of occurrences per case, 
             the median TT for cases with at least one occurrence of that DFR, and the 
             median TT for all other cases (without an occurrence of that DFR) are 
             computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
             and for each of the `max_k` DFRs, the minimum amount of occurrences per case, 
             the minimum NEPC for cases with at least one occurrence of that DFR, and the 
             minimum NEPC for all other cases (without an occurrence of that DFR) are 
             computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_dfr_performance'`, for each 
             time interval, and for each of the `max_k` DFRs, the maximum amount of 
             occurrences per case and the maximum DFR performance (i.e. the maximum 
             time elapsed between the occurrence of the first and second activity of 
             that DFR) are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_dfr_performance'`, 
             for each time interval, and for each of the `max_k` DFRs, the standard deviation 
             of amount of occurrences per case as and the standard deviation of the DFR 
             performances are computed. 
+
         """
         valm._verify_topKdfr(outcome = self.outcome, time_unit = time_unit, frequency= frequency, 
                             case_assignment= case_assignment, plt_type= plt_type, numeric_agg= numeric_agg,
                              max_k= max_k, xtr_outlier_rem = xtr_outlier_rem)
         top_k_dfr = self.dfrelations[:max_k]
         up.topK_dfr_evol(log = self.log, top_k_dfr = top_k_dfr, outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment,
                         type = plt_type, numeric_agg = numeric_agg, max_k = max_k, xtr_outlier_rem = xtr_outlier_rem)
     
     def dfr_evol(self, directly_follows_relations, time_unit='days', frequency='weekly', case_assignment = 'first_event', plt_type= 'univariate', numeric_agg= 'mean', xtr_outlier_rem=True):
         """Plot the time series of the requested aggregations for the 
-        Directly-Follows Relations (DFRs) specified in the 'directly_follows_relations' list.
+        Directly-Follows Relations (DFRs) specified in the ``directly_follows_relations`` list.
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. The requested DFR evolutions plotted are arranged in 
+        ``plt_type`` argument. The requested DFR evolutions plotted are arranged in 
         descending order of the number of occurrences of the DFRs.
 
-        For readability, the DFRs in `directly_follows_relations` are encoded with a 
+        For readability, the DFRs in ``directly_follows_relations`` are encoded with a 
         number, with DFR 1 being the most frequently occurring DFR, DFR 2 being 
         the second most occurring DFR, and so on. To retrieve a dataframe that maps these 
-        DFR numbers to the actual activity pairs, the `get_DFR_df()` method of the 
-        `DynamicLogPlots` class can be called upon. 
+        DFR numbers to the actual activity pairs, the ``get_DFR_df()`` method of the 
+        ``DynamicLogPlots`` class can be called upon. 
 
         Parameters
         ----------
         directly_follows_relations : list of tuple
             The DFRs for which the requested time series will be plotted. Each DFR needs to 
             be specified as a tuple that contains 2 strings, referring to the 2 activities in 
             the DFR, e.g. ('activity_a', 'activity_b').
@@ -307,105 +329,121 @@
         xtr_outlier_rem : bool, optional
             If True, the vertical ranges of the plots are only determined by regular  
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following five values:
-            - `'univariate'`: For each DFR, the evolutions of the periodically aggregated 
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following five values:
+
+          * `'univariate'`: For each DFR, the evolutions of the periodically aggregated 
             amount of occurrences per case, as well as the fraction of cases containing
-            at least one occurance of of that DFR, are plotted. 
-            - `'type_tt'`: For each DFR, next to the univariate plots, also the evolutions of 
+            at least one occurance of of that DFR, are plotted.
+
+          * `'type_tt'`: For each DFR, next to the univariate plots, also the evolutions of 
             the periodically aggregated Throughput Time (TT) for cases with vs. cases 
-            without that DFR are plotted. 
-            - `'type_events_case'`: For each DFR, next to the univariate plots, also the evolutions of 
+            without that DFR are plotted.
+
+          * `'type_events_case'`: For each DFR, next to the univariate plots, also the evolutions of 
             the periodically aggregated case length (in number of events per case (NEPC)) for cases 
-            with vs. cases without that DFR are plotted. 
-            - `'type_outcome'`: For each DFR, next to the univariate plots, also the evolutions of 
+            with vs. cases without that DFR are plotted.
+
+          * `'type_outcome'`: For each DFR, next to the univariate plots, also the evolutions of 
             the periodic fractions of cases with a positive outcome ('outcome=1') for cases with
             vs. cases without that DFR, are plotted. (Only applicable if an outcome is already 
             specified upon initialization of the `DynamicLogPlots` instance, or with the 
-            `set_outcomeColumn(outcome)` method.)
-            - `'type_dfr_performance'`: For each DFR, next to the univariate plots, also the 
+            ``set_outcomeColumn(outcome)`` method.)
+
+          * `'type_dfr_performance'`: For each DFR, next to the univariate plots, also the 
             evolution of the periodically aggregated DFR performance is plotted. The DFR 
             performance refers to the time elapsed between the first and last activity of
             that DFR. The time unit in which these periodic performance aggregations are 
-            expressed, is automatically determined based on their magnitude. __NOTE__ that 
+            expressed, is automatically determined based on their magnitude. **NOTE** that 
             the `'type_dfr_performance'` representation type is a special case, as it is 
             the only representation type in which cases can deliver more than one measure 
             for a certain DFR. I.e. cases that contain more than one occurrence of a 
             certain DFR will also deliver more than one value for the DFR performance to 
-            be aggregated over. 
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            be aggregated over.
+        
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='univariate'`, for each time interval, 
             and for each of the DFRs specified in `directly_follows_relations`, the 
             mean amount of occurrences per case is computed. The fraction of cases 
             containing at least one occurrence of a certain DFR is simply computed by, 
             for each time interval, computing the amount of cases with at least one 
             occurrence, and dividing it by the total amount of cases assigned to 
-            that time interval. 
-            - `'median'` : The requested time series are computed by taking the median for  
+            that time interval.
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the DFRs specified in `directly_follows_relations`, the median 
             amount of occurrences per case, the median TT for cases with at least one 
             occurrence of that DFR, and the median TT for all other cases 
-            (without an occurrence of that DFR) are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            (without an occurrence of that DFR) are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
             and for each of the DFRs specified in `directly_follows_relations`, the 
             minimum amount of occurrences per case, the minimum NEPC for cases with 
             at least one occurrence of that DFR, and the minimum NEPC for all other 
-            cases (without an occurrence of that DFR) are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            cases (without an occurrence of that DFR) are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_dfr_performance'`, for each 
             time interval, and for each of the DFRs specified in `directly_follows_relations`, 
             the maximum amount of occurrences per case and the maximum DFR performance 
             (i.e. the maximum time elapsed between the occurrence of the first and second 
-            activity of that DFR) are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
+            activity of that DFR) are computed.
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_dfr_performance'`, 
             for each time interval, and for each of the DFRs specified in `directly_follows_relations`, 
             the standard deviation of amount of occurrences per case as and the standard 
-            deviation of the DFR performances are computed. 
+            deviation of the DFR performances are computed.
+
         """
 
         valm._verify_dfr(dfrelations = self.dfrelations, directly_follows_relations = directly_follows_relations, outcome = self.outcome, 
                         time_unit = time_unit, frequency = frequency, case_assignment = case_assignment, plt_type = plt_type, 
                         numeric_agg = numeric_agg, xtr_outlier_rem= xtr_outlier_rem)
 
         up.dfr_evol(   log = self.log, directly_follows_relations = directly_follows_relations, outcome = self.outcome, time_unit = time_unit, frequency = frequency,
                     case_assignment = case_assignment, type = plt_type, numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem)
 
 
     def topK_variants_evol(self, time_unit='days', frequency='weekly', case_assignment = 'first_event', plt_type= 'univariate', numeric_agg= 'mean', max_k= 10, xtr_outlier_rem = True):
-        """Plot the time series of the requested aggregations for each of the 'max_k' 
+        """Plot the time series of the requested aggregations for each of the ``max_k`` 
         most frequently occurring variants.
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. The requested variant time series plotted are arranged in 
+        ``plt_type`` argument. The requested variant time series plotted are arranged in 
         descending order of the number of occurrences of the variants.
 
         For readability, the variants are encoded with a number, with variant 1 being the most 
-        frequently occurring variant, and variant '`max_k`' being the max_k'th most occurring 
+        frequently occurring variant, and variant ``max_k`` being the max_k'th most occurring 
         variant. To retrieve a dataframe that maps these variant numbers to the actual 
-        activity sequences, the `get_var_df()` method of the `DynamicLogPlots` class can 
+        activity sequences, the ``get_var_df()`` method of the ``DynamicLogPlots`` class can 
         be called upon. 
 
         Parameters
         ----------
         time_unit : {'microseconds', 'milliseconds', 'seconds', 'minutes', 'hours', 'days', 'weeks'}
             Time unit in which the throughput time of cases is specified, by default `'days'`.
         frequency : {'minutely', '5-minutely', '10-minutely', 'half-hourly', 'hourly' '2-hourly', 
@@ -422,89 +460,103 @@
             Determines how periodic quantities are aggregated, by default `'mean'`. The specified
             aggregation function will be applied to all the requested time series, except for 
             those quantities that express fractions or counts (if any). For a more detailed 
             explanation of the different `numeric_agg` options, see Notes.
         max_k : int, optional
             Only the max_k most frequently occurring variants are considered, by default 10. 
         xtr_outlier_rem : bool, optional
-            If True, the vertical ranges of the plots are only determined by regular  
+            If True, the vertical ranges of the plots are only determined by regular 
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs. 
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following three values:
-            - `'univariate'`: For each variant, plots the evolution of the periodic fraction
-            of cases for accounted for by that variant. 
-            - `'type_tt'`: For each variant, next to the univariate plots, also the evolutions of 
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following three values:
+
+          * `'univariate'`: For each variant, plots the evolution of the periodic fraction
+            of cases for accounted for by that variant.
+
+          * `'type_tt'`: For each variant, next to the univariate plots, also the evolutions of 
             the periodically aggregated Throughput Time (TT) for cases belonging to that variant vs. 
-            all other cases (not belonging to that variant), are plotted. 
-            - `'type_outcome'`: For each variant, next to the univariate plots, also the evolutions 
+            all other cases (not belonging to that variant), are plotted.
+
+          * `'type_outcome'`: For each variant, next to the univariate plots, also the evolutions 
             of the periodic fractions of cases with a positive outcome ('outcome=1') for cases 
             belonging to that variant vs. all other cases (not belonging to that variant),
             are plotted. (Only applicable if an outcome is already specified upon initialization 
-            of the `DynamicLogPlots` instance, or with the `set_outcomeColumn(outcome)` method.)
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            of the `DynamicLogPlots` instance, or with the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` variants, the mean TT for cases belonging to 
             that variant, and the mean TT for all other cases (belonging to other 
-            variants) are computed. 
-            - `'median'` : The requested time series are computed by taking the median for  
+            variants) are computed.
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` variants, the median TT for cases belonging to 
             that variant, and the median TT for all other cases (belonging to other 
-            variants) are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            variants) are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` variants, the minimum TT among cases belonging 
             to that variant, and the minimum TT among all other cases (belonging to other 
-            variants) are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            variants) are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` variants, the maximum TT among cases belonging 
             to that variant, and the maximum TT among all other cases (belonging to other 
-            variants) are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
+            variants) are computed.
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_tt'`, 
             for each time interval, and for each of the `max_k` variants, the standard  
             deviation of the TT for cases belonging to that variant, and the standard 
-            deviation of the TT for all other cases (belonging to other variants) are computed. 
+            deviation of the TT for all other cases (belonging to other variants) are computed.
+
         """
         valm._verify_topKvariants(outcome = self.outcome, time_unit = time_unit, frequency = frequency, 
                                     case_assignment = case_assignment, plt_type = plt_type, numeric_agg = numeric_agg,
                                     max_k = max_k, xtr_outlier_rem = xtr_outlier_rem)
         top_k_vars = self.all_vars[:max_k]
         up.topK_variants_evol(log = self.log, top_k_vars = top_k_vars, outcome = self.outcome, time_unit= time_unit, frequency= frequency, 
                             case_assignment = case_assignment, type= plt_type, numeric_agg= numeric_agg, max_k= max_k, xtr_outlier_rem = xtr_outlier_rem)
 
     def variants_evol(self, variants, time_unit='days', frequency='weekly', case_assignment = 'first_event', plt_type= 'univariate', numeric_agg= 'mean', xtr_outlier_rem = True):
         """Plot the time series of the requested aggregations for the 
-        variants specified in the 'variants' list.
+        variants specified in the ``variants`` list.
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. The requested variant time series plotted are arranged in 
+        ``plt_type`` argument. The requested variant time series plotted are arranged in 
         descending order of the number of occurrences of the variants.
 
         For readability, the variants are encoded with a number, with variant 1 being the most 
         frequently occurring variant, variant 2 being the second most occurring 
         variant, and so on. To retrieve a dataframe that maps these variant numbers to the actual 
-        activity sequences, the `get_var_df()` method of the `DynamicLogPlots` class can 
+        activity sequences, the ``get_var_df()`` method of the ``DynamicLogPlots`` class can 
         be called upon. 
 
         Parameters
         ----------
         variants : list of tuple
             The variants for which the requested time series will be plotted. Each variant needs to 
             be specified as a tuple that contains N strings, referring to the N activities that 
@@ -529,80 +581,94 @@
         xtr_outlier_rem : bool, optional
             If True, the vertical ranges of the plots are only determined by regular  
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following three values:
-            - `'univariate'`: For each variant, plots the evolution of the periodic fraction
-            of cases accounted for by that variant. 
-            - `'type_tt'`: For each variant, next to the univariate plots, also the evolutions of 
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following three values:
+
+          * `'univariate'`: For each variant, plots the evolution of the periodic fraction
+            of cases accounted for by that variant.
+
+          * `'type_tt'`: For each variant, next to the univariate plots, also the evolutions of 
             the periodically aggregated Throughput Time (TT) for cases belonging to that variant vs. 
-            all other cases (not belonging to that variant), are plotted. 
-            - `'type_outcome'`: For each variant, next to the univariate plots, also the evolutions 
+            all other cases (not belonging to that variant), are plotted.
+
+          * `'type_outcome'`: For each variant, next to the univariate plots, also the evolutions 
             of the periodic fractions of cases with a positive outcome ('outcome=1') for cases 
             belonging to that variant vs. all other cases (not belonging to that variant),
             are plotted. (Only applicable if an outcome is already specified upon initialization 
-            of the `DynamicLogPlots` instance, or with the `set_outcomeColumn(outcome)` method.)
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            of the `DynamicLogPlots` instance, or with the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each variant specified in `variants`, the mean TT for cases belonging to 
             that variant, and the mean TT for all other cases (belonging to other 
-            variants) are computed. 
-            - `'median'` : The requested time series are computed by taking the median for  
+            variants) are computed.
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each variant specified in `variants`, the median TT for cases belonging to 
             that variant, and the median TT for all other cases (belonging to other 
-            variants) are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            variants) are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each variant specified in `variants`, the minimum TT among cases belonging 
             to that variant, and the minimum TT among all other cases (belonging to other 
-            variants) are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            variants) are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each variant specified in `variants`, the maximum TT among cases belonging 
             to that variant, and the maximum TT among all other cases (belonging to other 
-            variants) are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
+            variants) are computed.
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_tt'`, 
             for each time interval, and for each variant specified in `variants`, the standard  
             deviation of the TT for cases belonging to that variant, and the standard 
-            deviation of the TT for all other cases (belonging to other variants) are computed. 
+            deviation of the TT for all other cases (belonging to other variants) are computed.
+
         """
         valm._verify_variants(all_vars = self.all_vars, variants = variants, outcome = self.outcome, time_unit = time_unit, 
                                 frequency = frequency, case_assignment = case_assignment, plt_type = plt_type, 
                                 numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem)
 
         up.variants_evol(log = self.log, variants = variants, outcome = self.outcome, time_unit = time_unit,
                             frequency = frequency, case_assignment = case_assignment, type= plt_type, 
                             numeric_agg= numeric_agg, xtr_outlier_rem = xtr_outlier_rem)
 
     def topK_categorical_caseftr_evol(self, case_feature, time_unit = 'days', frequency = 'weekly', case_assignment = 'first_event', plt_type = 'univariate', numeric_agg = 'mean', max_k = 10, xtr_outlier_rem = True):
-        """Plot the time series of the requested aggregations for each of the 'max_k' 
+        """Plot the time series of the requested aggregations for each of the ``max_k`` 
         most frequently occurring levels of categorical case feature 'case_feature'.
-        If 'max_k' is greater than or equal to the cardinality of that feature, the 
+        If ``max_k`` is greater than or equal to the cardinality of that feature, the 
         requested time series for all levels are plotted. 
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. The requested level time series plotted are arranged in 
+        ``plt_type`` argument. The requested level time series plotted are arranged in 
         descending order of the number of occurrences of the levels. 
 
         Parameters
         ----------
         case_feature : str
             Column name of the categorical case feature. The case feature already has to be 
             specified, either upon initalization of the `DynamicLogPlots` object, or with 
@@ -624,89 +690,105 @@
             aggregation function will be applied to all the requested time series, except for 
             those quantities that express fractions or counts (if any). For a more detailed 
             explanation of the different `numeric_agg` options, see Notes.
         max_k : int, optional
             Only the max_k most frequently occurring levels of 'case_feature' are considered, 
             by default 10.
         xtr_outlier_rem : bool, optional
-            If True, the vertical ranges of the plots are only determined by regular  
+            If True, the vertical ranges of the plots are only determined by regular 
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following four values:
-            - `'univariate'`: For each level, plots the evolution of the periodic fraction
-            of cases for which `case_feature='level'`. 
-            - `'type_tt'`: For each level, next to the univariate plots, also the evolutions of 
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following four values:
+
+          * `'univariate'`: For each level, plots the evolution of the periodic fraction
+            of cases for which `case_feature='level'`.
+
+          * `'type_tt'`: For each level, next to the univariate plots, also the evolutions of 
             the periodically aggregated Throughput Time (TT) for cases with `case_feature='level'` vs. 
-            all other cases (`case_feature!='level'`), are plotted. 
-            - `'type_events_case'`: For each level, next to the univariate plots, also the evolutions of 
+            all other cases (`case_feature!='level'`), are plotted.
+
+          * `'type_events_case'`: For each level, next to the univariate plots, also the evolutions of 
             the periodically aggregated case length (in Number of Events Per Case (NEPC)) for cases 
-            with `case_feature='level'` vs. all other cases (`case_feature!='level'`), are plotted. 
-            - `'type_outcome'`: For each level, next to the univariate plots, also the evolutions 
+            with `case_feature='level'` vs. all other cases (`case_feature!='level'`), are plotted.
+
+          * `'type_outcome'`: For each level, next to the univariate plots, also the evolutions 
             of the periodic fractions of cases with a positive outcome ('outcome=1') for cases 
             with `case_feature='level'` vs. all other cases (`case_feature!='level'`), are plotted. 
             (Only applicable if an outcome is already specified upon initialization 
-            of the `DynamicLogPlots` instance, or with the `set_outcomeColumn(outcome)` method.)
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            of the `DynamicLogPlots` instance, or with the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` levels of `case_feature`, the mean TT for cases with 
             `case_feature='level'`, and the mean TT for all other cases (with 
-            `case_feature!='level'`) are computed. 
-            - `'median'` : The requested time series are computed by taking the median for  
+            `case_feature!='level'`) are computed.
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
             and for each of the `max_k` levels of `case_feature`, the median NEPC for cases with 
             `case_feature='level'`, and the median NEPC for all other cases (with 
-            `case_feature!='level'`) are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            `case_feature!='level'`) are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
             and for each of the `max_k` levels of `case_feature`, the minimum NEPC among cases with 
             `case_feature='level'`, and the minimum NEPC among all other cases (with 
-            `case_feature!='level'`) are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            `case_feature!='level'`) are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` levels of `case_feature`, the maximum TT among cases 
             with `case_feature='level'`, and the maximum TT among all other cases (with 
-            `case_feature!='level'`) are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
+            `case_feature!='level'`) are computed.
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` levels of `case_feature`, the standard deviation of the 
             TT among cases with `case_feature='level'`, and the standard deviation of the TT of all 
-            other cases (with `case_feature!='level'`) are computed. 
+            other cases (with `case_feature!='level'`) are computed.
+
         """
 
         valm._verify_topKcatFt(feature = case_feature, ftr_type = 'case', feature_list = self.categorical_casefeatures, 
                                     outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment, 
                                     plt_type = plt_type, numeric_agg = numeric_agg, max_k = max_k, xtr_outlier_rem = xtr_outlier_rem)
 
         up.topK_categorical_caseftr_evol(log = self.log, case_feature = case_feature, outcome = self.outcome, time_unit = time_unit, 
                                         frequency = frequency, case_assignment = case_assignment, type = plt_type, 
                                         numeric_agg = numeric_agg, max_k = max_k, xtr_outlier_rem = xtr_outlier_rem)
 
 
     def num_casefts_evol(self, numeric_case_list, time_unit='days', frequency='weekly', case_assignment = 'first_event', plt_type = 'univariate', numeric_agg= 'mean', xtr_outlier_rem = True):
         """ Plots the time series of the requested aggregations over time for the numerical 
-        event features specified in the 'numeric_case_list' argument.
+        event features specified in the ``numeric_case_list`` argument.
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument.
+        ``plt_type`` argument.
 
         Parameters
         ----------
         numeric_case_list : list of str
             Column names of the numerical case features. All case features already have to be 
             specified, either upon initalization of the `DynamicLogPlots` object, or with 
             the `.add_numerical_caseft(case_feature)` class method. 
@@ -730,85 +812,101 @@
         xtr_outlier_rem : bool, optional
             If True, the vertical ranges of the plots are only determined by regular  
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following four values:
-            - `'univariate'`: For each numerical case feature, plots the evolution of its 
-            periodical aggregations. 
-            - `'type_tt'`: For each numerical case feature, next to the univariate plots, also the
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following four values:
+
+          * `'univariate'`: For each numerical case feature, plots the evolution of its 
+            periodical aggregations.
+
+          * `'type_tt'`: For each numerical case feature, next to the univariate plots, also the
             evolution of the periodically aggregated ratio of Throughput Time (TT) needed per 
             unit of that feature is plotted. The time unit of these periodic ratio aggregations 
-            (time unit / unit of feature) is automatically determined based on their magnitude. 
-            - `'type_events_case'`: For each numerical case feature, next to the univariate plots, 
+            (time unit / unit of feature) is automatically determined based on their magnitude.
+
+          * `'type_events_case'`: For each numerical case feature, next to the univariate plots, 
             also the evolution of the periodically aggregated ratio of Number of Events Per Case 
             (NEPC) needed per 10^(x) units of that feature is plotted. The exponent 'x' is automatically 
-            determined based on their magnitude. 
-            - `'type_outcome'`: For each numerical case feature, next to the univariate plots, also 
+            determined based on their magnitude.
+
+          * `'type_outcome'`: For each numerical case feature, next to the univariate plots, also 
             the two evolutions of the feature's periodical aggregations for cases with a positive 
             outcome ('outcome=1') vs. cases with a negative outcome ('outcome=1') are plotted. 
             (Only applicable if an outcome is already specified upon initialization 
-            of the `DynamicLogPlots` instance, or with the `set_outcomeColumn(outcome)` method.)
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            of the `DynamicLogPlots` instance, or with the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='univariate'`, for each time interval, 
             and for each numeric case feature specified in `numeric_case_list`, the mean 
-            of all case feature values is is computed. 
-            - `'median'` : The requested time series are computed by taking the median for 
+            of all case feature values is is computed.
+
+          * `'median'` : The requested time series are computed by taking the median for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each numeric case feature specified in `numeric_case_list`, the median 
-            of all case feature values as well as the median of all TT ratios are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            of all case feature values as well as the median of all TT ratios are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_events_case'`, for each time 
             interval, and for each numeric case feature specified in `numeric_case_list`, 
             both the minimum of all case feature values and the minimum of all NEPC ratios 
-            are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_outcome'`, for each time 
             interval, and for each numeric case feature specified in `numeric_case_list`, 
             the maximum of all case feature values, the maximum of all case feature values 
             for cases with a positive outcome and the maximum of all values for cases 
             with a negative outcome are computed.
-            - `'std'` : The requested time series are computed by taking the standard 
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_tt'`, for each 
             time interval, and for each numeric case feature specified in `numeric_case_list`, 
             the standard deviation of all case feature values as well as the standard deviation 
-            of all TT ratios are computed. 
+            of all TT ratios are computed.
+
         """
 
         valm._verify_numFt(features = numeric_case_list, ftr_type = 'case', feature_list = self.numerical_casefeatures, 
                             outcome = self.outcome, time_unit = time_unit, frequency = frequency, 
                             case_assignment= case_assignment, plt_type = plt_type, numeric_agg = numeric_agg, xtr_outlier_rem= xtr_outlier_rem)
         up.num_casefts_evol(log = self.log, numeric_case_list = numeric_case_list, outcome = self.outcome, time_unit = time_unit, 
                                 frequency = frequency, case_assignment = case_assignment, type = plt_type, 
                                 numeric_agg= numeric_agg, xtr_outlier_rem= xtr_outlier_rem)
 
 
     def topK_categorical_eventftr_evol(self, event_feature, time_unit = 'days', frequency = 'weekly', case_assignment = 'first_event', plt_type = 'univariate', numeric_agg = 'mean', max_k = 10, xtr_outlier_rem = True):
-        """Plot the time series of the requested aggregations for each of the 'max_k' 
-        most frequently occurring levels of categorical event feature 'event_feature'.
-        If 'max_k' is greater than or equal to the cardinality of that feature, the 
+        """Plot the time series of the requested aggregations for each of the ``max_k`` 
+        most frequently occurring levels of categorical event feature ``event_feature``.
+        If ``max_k`` is greater than or equal to the cardinality of that feature, the 
         requested time series for all levels are plotted. 
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. The requested level time series plotted are arranged in 
+        ``plt_type`` argument. The requested level time series plotted are arranged in 
         descending order of the number of occurrences of each level.
 
         Parameters
         ----------
         event_feature : str
             Column name of the categorical event feature. The event feature already has to be 
             specified, either upon initalization of the `DynamicLogPlots` object, or with 
@@ -836,93 +934,108 @@
         xtr_outlier_rem : bool, optional
             If True, the vertical ranges of the plots are only determined by regular  
             values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
             when determining the vertical range, by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following four values:
-            - `'univariate'`: For each level, plots the evolution of the periodic fraction
-            of cases for which . 
-            - `'type_tt'`: For each level, next to the univariate plots, also the evolutions of 
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following four values:
+
+          * `'univariate'`: For each level, plots the evolution of the periodic fraction
+            of cases for which at least one event satisfies `event_feature='level'`. 
+          * `'type_tt'`: For each level, next to the univariate plots, also the evolutions of 
             the periodically aggregated Throughput Time (TT) for cases with at least one  
-            occurrence of  vs. all other cases (`event_feature!='level'` for all 
-            events), are plotted. 
-            - `'type_events_case'`: For each level, next to the univariate plots, also the evolutions of 
+            occurrence of `event_feature='level'` vs. all other cases (`event_feature!='level'` for all 
+            events), are plotted.
+
+          * `'type_events_case'`: For each level, next to the univariate plots, also the evolutions of 
             the periodically aggregated case length (in Number of Events Per Case (NEPC)) for cases 
-            with at least one occurrence of  vs. all other cases 
-            (`event_feature!='level'` for all events), are plotted. 
-            - `'type_outcome'`: For each level, next to the univariate plots, also the evolutions 
+            with at least one occurrence of `event_feature='level'` vs. all other cases 
+            (`event_feature!='level'` for all events), are plotted.
+
+          * `'type_outcome'`: For each level, next to the univariate plots, also the evolutions 
             of the periodic fractions of cases with a positive outcome ('outcome=1') for cases 
             with at least one occurrence of `event_feature='level'` vs. all other cases 
             (`event_feature!='level'` for all events), are plotted. (Only applicable if an outcome 
             is already specified upon initialization of the `DynamicLogPlots` instance, or with 
-            the `set_outcomeColumn(outcome)` method.)
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` levels of `event_feature`, the mean TT for cases with 
             at least one occurrence of `event_feature='level'`, and the mean TT for all other cases 
-            (with `event_feature!='level'` for all events) are computed. 
-            - `'median'` : The requested time series are computed by taking the median for  
+            (with `event_feature!='level'` for all events) are computed.
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
             and for each of the `max_k` levels of `event_feature`, the median NEPC for cases with 
             at least one occurrence of `event_feature='level'`, and the median NEPC for all other cases  
-            (with `event_feature!='level'` for all events) are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            (with `event_feature!='level'` for all events) are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
             and for each of the `max_k` levels of `event_feature`, the minimum NEPC among cases with 
             at least one occurrence of `event_feature='level'`, and the minimum NEPC among all other 
-            cases (with `event_feature!='level'` for all events) are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            cases (with `event_feature!='level'` for all events) are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` levels of `event_feature`, the maximum TT among cases 
             with at least one occurrence of `event_feature='level'`, and the maximum TT among all 
-            other cases (with `event_feature!='level'` for all events) are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
+            other cases (with `event_feature!='level'` for all events) are computed.
+
+          * `'std'` : The requested time series are computed by taking the standard 
             deviation for each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each of the `max_k` levels of `event_feature`, the standard deviation of the 
             TT among cases with at least one occurrence of `event_feature='level'`, and the standard 
             deviation of the TT of all other cases (with `event_feature!='level'` for all events) are 
-            computed. 
+            computed.
+
         """
         valm._verify_topKcatFt(feature = event_feature, ftr_type = 'event', feature_list = self.categorical_eventfeatures,
                                 outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment,
                                 plt_type = plt_type, numeric_agg = numeric_agg, max_k = max_k, xtr_outlier_rem = xtr_outlier_rem)
 
         up.topK_categorical_eventftr_evol(log = self.log, event_feature = event_feature, outcome = self.outcome, time_unit = time_unit,
                                 frequency = frequency, case_assignment = case_assignment, plt_type = plt_type, numeric_agg = numeric_agg,
                                 max_k = max_k, xtr_outlier_rem = xtr_outlier_rem)
 
 
     def num_eventfts_evol(self, numeric_event_list, time_unit = 'days', frequency = 'weekly', case_assignment = 'first_event', 
                           plt_type = 'univariate', numeric_agg = 'mean', xtr_outlier_rem = True, numEventFt_transform = 'last'):
         """Plot the evolution of the requested aggregations over time for the numerical 
-        event features specified in the numeric_event_list argument. 
+        event features specified in the ``numeric_event_list`` argument. 
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         holistically combined with different performance measures by specifying the 
-        `plt_type` argument. 
+        ``plt_type`` argument. 
 
         In contrast to the numerical case features, numerical event features can take on 
         different values for one and the same case. Therefore, to visualize case-level 
         characteristics over time, an additional abstraction method is needed to project a 
         trace's sequence of numerical event feature values to a single numeric value. This
-        transformation can be specified by means of the `numEventFt_transform` parameter. 
+        transformation can be specified by means of the ``numEventFt_transform`` parameter. 
         
         Parameters
         ----------
         numeric_event_list : list of str
             Column names of the numerical event features. All event features already have to be 
             specified, either upon initalization of the `DynamicLogPlots` object, or with 
             the `.add_numerical_eventft(event_feature)` class method. 
@@ -952,101 +1065,136 @@
             determines the way in which these numerical event features are transformed to the 
             case level. By default `'last'`. For a more detailed explanation of the different 
             `numEventFt_transform` options, see Notes.
 
         
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - ``plt_type`` can take one of the following four values:
-            - `'univariate'`: For each numerical event feature, plots the evolution of its 
-            periodical aggregations. 
-            - `'type_tt'`: For each numerical event feature, next to the univariate plots, also the
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following four values:
+
+          * `'univariate'`: For each numerical event feature, plots the evolution of its 
+            periodical aggregations.
+
+          * `'type_tt'`: For each numerical event feature, next to the univariate plots, also the
             evolution of the periodically aggregated ratio of Throughput Time (TT) needed per 
             unit of that feature is plotted. The time unit of these periodic ratio aggregations 
-            (time unit / unit of feature) is automatically determined based on their magnitude. 
-            - `'type_events_case'`: For each numerical event feature, next to the univariate plots, 
+            (time unit / unit of feature) is automatically determined based on their magnitude.
+
+          * `'type_events_case'`: For each numerical event feature, next to the univariate plots, 
             also the evolution of the periodically aggregated ratio of Number of Events Per Case 
             (NEPC) needed per 10^(x) units of that feature is plotted. The exponent 'x' is automatically 
-            determined based on their magnitude. 
-            - `'type_outcome'`: For each numerical event feature, next to the univariate plots, also 
+            determined based on their magnitude.
+
+          * `'type_outcome'`: For each numerical event feature, next to the univariate plots, also 
             the two evolutions of the feature's periodical aggregations for cases with a positive 
             outcome ('outcome=1') vs. cases with a negative outcome ('outcome=1') are plotted. 
             (Only applicable if an outcome is already specified upon initialization 
-            of the `DynamicLogPlots` instance, or with the `set_outcomeColumn(outcome)` method.)
-        - ``numeric_agg`` can take on the following five values:
-            - `'mean'` : The requested time series are computed by taking the mean for each 
+            of the `DynamicLogPlots` instance, or with the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
             time interval. E.g. for `plt_type='univariate'`, for each time interval, 
             and for each numeric event feature, the mean of all (transformed) values is 
-            is computed. 
-            - `'median'` : The requested time series are computed by taking the median for  
+            is computed.
+
+          * `'median'` : The requested time series are computed by taking the median for  
             each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
             and for each numeric event feature, the median of all (transformed) event 
-            feature values as well as the median of all TT ratios are computed. 
-            - `'min'` : The requested time series are computed by taking the minimum for 
+            feature values as well as the median of all TT ratios are computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
             each time interval. E.g. for `plt_type='type_events_case'`, for each time  
             interval, and for each numeric event feature, both the minimum of all 
-            (transformed) values and the minimum of all NEPC ratios are computed. 
-            - `'max'` : The requested time series are computed by taking the maximum for 
+            (transformed) values and the minimum of all NEPC ratios are computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
             each time interval. E.g. for `plt_type='type_outcome'`, for each time  
             interval, and for each numeric event feature, both the maximum of all 
             (transformed) values, the maximum of all (transformed) values for cases 
             with a positive outcome and the maximum of all (transformed) values for 
-            cases with a negative outcome are computed. 
-            - `'std'` : The requested time series are computed by taking the standard 
-            deviation for each time interval. E.g. for `plt_type='type_tt'`, for each  
+            cases with a negative outcome are computed.
+
+          * `'std'` : The requested time series are computed by taking the standard 
+            deviation for each time interval. E.g. for `plt_type='type_tt'`, for each 
             time interval, and for each numeric event feature, the standard deviation 
             of all (transformed) event feature values as well as the standard deviation 
-            of all TT ratios are computed. 
-        - 'numEventFt_transform' determines, for each numerical event feature contained in 
-        `numeric_event_list`, how each trace's sequence of numerical event feature values 
-        are projected to a single numeric value. It can take on the following eight values: 
-            - `'last'` : Each case is assigned the last non-null entry a numerical event feature. 
-            - `'first'` : Each case is assigned the first non-null entry of a numerical event feature. 
-            - `'mean'` : Each case is assigned the mean value over all its non-null entries of a 
-            numerical event feature. 
-            - `'median'` : Each case is assigned the median value over all its non-null entries of a 
-            numerical event feature. 
-            - `'sum'` : Each case is assigned the sum over all its non-null entries of a 
-            numerical event feature. 
-            - `'prod'` : Each case is assigned the product over all its non-null entries of a 
-            numerical event feature. 
-            - `'min'` : Each case is assigned the minimum value over all its non-null entries of a 
-            numerical event feature. 
-            - `'max'` : Each case is assigned the maximum value over all its non-null entries of a 
-            numerical event feature. 
+            of all TT ratios are computed.
+
+        * 'numEventFt_transform' determines, for each numerical event feature contained in 
+          `numeric_event_list`, how each trace's sequence of numerical event feature values 
+          are projected to a single numeric value. It can take on the following eight values:
+
+          * `'last'` : Each case is assigned the last non-null entry a numerical event feature.
+
+          * `'first'` : Each case is assigned the first non-null entry of a numerical event feature.
+
+          * `'mean'` : Each case is assigned the mean value over all its non-null entries of a 
+            numerical event feature.
+
+          * `'median'` : Each case is assigned the median value over all its non-null entries of a 
+            numerical event feature.
+
+          * `'sum'` : Each case is assigned the sum over all its non-null entries of a 
+            numerical event feature.
+
+          * `'prod'` : Each case is assigned the product over all its non-null entries of a 
+            numerical event feature.
+
+          * `'min'` : Each case is assigned the minimum value over all its non-null entries of a 
+            numerical event feature.
+
+          * `'max'` : Each case is assigned the maximum value over all its non-null entries of a 
+            numerical event feature.
+
         """
 
         valm._verify_numFt(features = numeric_event_list, ftr_type = 'event', feature_list = self.numerical_eventfeatures,
                             outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment,
                             plt_type = plt_type, numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem, 
                             numEventFt_transform = numEventFt_transform)
                             
         up.num_eventfts_evol(log = self.log, numeric_event_list = numeric_event_list, outcome = self.outcome, time_unit = time_unit,
                             frequency = frequency, case_assignment = case_assignment, type = plt_type, numeric_agg = numeric_agg, 
                             xtr_outlier_rem = xtr_outlier_rem, numEventFt_transform = numEventFt_transform)
 
 
     def distinct_variants_evol(self, time_unit='days', frequency='weekly', case_assignment = 'first_event', plt_type= 'univariate', numeric_agg= 'mean', xtr_outlier_rem = True, cases_initialized = True):
-        """Plots the number of distinct variants over time, as well as the number of 
+        """
+        **Deprecated**
+
+        .. deprecated:: 0.1.1
+          ``distinct_variants_evol()`` method will be removed in DyLoPro 0.2.0 
+          because it duplicates part of the visualization capabilities 
+          offered by the ``distinct_variants_AdvancedEvol()`` method. 
+          Use the more extensive ``distinct_variants_AdvancedEvol()`` 
+          visualization method instead.
+        
+        Plots the number of distinct variants over time, as well as the number of 
         distinct previously unseen / distinct new variants over time.
 
         All cases are grouped into time intervals of which the length is determined by the 
-        `frequency` argument. The condition that determines the time interval to which a 
-        certain case is assigned, is determined by the `case_assignment` argument. Can be 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
         combined with different performance measures by specifying the 
-        `plt_type` argument.
+        ``plt_type`` argument.
 
         Parameters
         ----------
         time_unit : {'microseconds', 'milliseconds', 'seconds', 'minutes', 'hours', 'days', 'weeks'}
             Time unit in which the throughput time of cases is specified, by default `'days'`.
         frequency : {'minutely', '5-minutely', '10-minutely', 'half-hourly', 'hourly' '2-hourly', 
                     '12-hourly', 'daily', 'weekly', '2-weekly', 'monthly', 'quarterly', 'half-yearly'}
@@ -1072,60 +1220,199 @@
             the evolution of the number of cases initialized in each period 
             on the same graph as the one foreseen for either the Throughput Time 
             (`plt_type='type_tt'`), the Number of Events Per Case (`plt_type='type_events_case'`) 
             or the fraction of positive cases (`plt_type='type_outcome'`), by default `True`.
 
         Notes
         -----
-        - ``case_assignment`` can take on the following three values:
-            - `'first_event'`: Each case is assigned to the time interval in which 
-            its first event occurs. 
-            - `'last_event'`: Each case is assigned to the time interval in which 
-            its last event occurs
-            - `'max_events'`: Out of all the time intervals in which the events of a 
+        
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
             particular case occur, the case is assigned to the interval in which most 
             of its events occur. Ties among time intervals are broken by assigning the 
-            case to the first time interval. 
-        - `plt_type` can take one of the following four values:
-            - `'univariate'`: Plots the evolution of the amount of distinct variants present in each time period, 
+            case to the first time interval.
+            
+        * ``plt_type`` can take one of the following four values:
+
+          * `'univariate'`: Plots the evolution of the amount of distinct variants present in each time period, 
             as well as the amount of distinct new variants introduced in each time period.
-            - `'type_tt'`: Next ot the univariate plots, also plots the evolution of the periodically aggregated 
+
+          * `'type_tt'`: Next ot the univariate plots, also plots the evolution of the periodically aggregated 
             Throughput Time (TT) (in the time unit specified by the 'time_unit' argument).
-            - `'type_events_case'`: Next to the univariate plots, also plots the evolution of the periodically aggregated 
+
+          * `'type_events_case'`: Next to the univariate plots, also plots the evolution of the periodically aggregated 
             Number of Events Per Case (NEPC).
-            - `'type_outcome'`: Next to the univariate plots, also plots the evolution of the periodically aggregated 
+
+          * `'type_outcome'`: Next to the univariate plots, also plots the evolution of the periodically aggregated 
             fraction of cases with outcome = True. (Only applicable if an outcome is already specified upon initialization 
-            of the `DynamicLogPlots` instance, or with the `set_outcomeColumn(outcome)` method.)
+            of the `DynamicLogPlots` instance, or with the ``set_outcomeColumn(outcome)`` method.)
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
+            time interval.
+
+          * `'median'` : The requested time series are computed by taking the median for  
+            each time interval.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
+            each time interval.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
+            each time interval.
+
+          * `'std'` : The requested time series are computed by taking the standard 
+            deviation for each time interval.
+
         """
         valm._verify_distinctvars(outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment, plt_type = plt_type, 
                                     numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem, cases_initialized = cases_initialized)
         
         up.distinct_variants_evol(log = self.log, outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment, 
                                     type = plt_type, numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem, cases_initialized = cases_initialized)
 
 
     def distinct_variants_AdvancedEvol(self, time_unit='days', frequency='weekly', case_assignment = 'first_event', plt_type= 'univariate', numeric_agg= 'mean', xtr_outlier_rem = True, cases_initialized = True):
-        """Documentation COMING SOON...
+        """Plot the evolution of the requested aggregations over time for:
+
+        #. cases belonging to variants already seen in previous time periods
+        #. cases belonging to variants first observed in each time period
+
+        All cases are grouped into time intervals of which the length is determined by the 
+        ``frequency`` argument. The condition that determines the time interval to which a 
+        certain case is assigned, is determined by the ``case_assignment`` argument. Can be 
+        holistically combined with different performance measures by specifying the 
+        ``plt_type`` argument. 
 
         Parameters
         ----------
-        time_unit : str, optional
-            _description_, by default `'days'`
-        frequency : str, optional
-            _description_, by default `'weekly'`
-        case_assignment : str, optional
-            _description_, by default `'first_event'`
-        plt_type : str, optional
-            _description_, by default `'univariate'`
-        numeric_agg : str, optional
-            _description_, by default `'mean'`
+        time_unit : {'microseconds', 'milliseconds', 'seconds', 'minutes', 'hours', 'days', 'weeks'}
+            Time unit in which the throughput time of cases is specified, by default `'days'`.
+        frequency : {'minutely', '5-minutely', '10-minutely', 'half-hourly', 'hourly' '2-hourly', 
+                    '12-hourly', 'daily', 'weekly', '2-weekly', 'monthly', 'quarterly', 'half-yearly'}
+            Frequency by which the observations are grouped together, by default `'weekly'`.
+        case_assignment : {'first_event', 'last_event', 'max_events'}
+            Determines the condition upon which each case is assigned to a certain 
+            period, by default `'first_event'`. For a more detailed explanation 
+            of the different `case_assignment` options, see Notes.
+        plt_type : {'univariate', 'type_tt', 'type_events_case', 'type_outcome'}
+            Determines which time series are constructed and visualized, by default `'univariate'`.
+            For a more detailed explanation of the different `plt_type` options, see Notes.
+        numeric_agg : {'mean', 'median', 'min', 'max', 'std'}
+            Determines how periodic quantities are aggregated, by default `'mean'`. The specified
+            aggregation function will be applied to all the requested time series, except for 
+            those quantities that express fractions or counts (if any). For a more detailed 
+            explanation of the different `numeric_agg` options, see Notes.
         xtr_outlier_rem : bool, optional
-            _description_, by default `True`
+            If True, the vertical ranges of the plots are only determined by regular  
+            values, i.e. extreme outliers (>q3 + 3*iqr) in the time series are neglected 
+            when determining the vertical range, by default `True`.
         cases_initialized : bool, optional
-            _description_, by default `True`
+            If True, and `plt_type!='univariate'`, then the method also plots 
+            the evolution of the number of cases initialized in each period 
+            on the same graph as the one foreseen for either the Throughput Time 
+            (`plt_type='type_tt'`), the Number of Events Per Case (`plt_type='type_events_case'`) 
+            or the fraction of positive cases (`plt_type='type_outcome'`), by default `True`.
+
+        Notes
+        -----
+        
+        * ``case_assignment`` can take on the following three values:
+
+          * `'first_event'`: Each case is assigned to the time interval in which 
+            its first event occurs.
+
+          * `'last_event'`: Each case is assigned to the time interval in which 
+            its last event occurs.
+
+          * `'max_events'`: Out of all the time intervals in which the events of a 
+            particular case occur, the case is assigned to the interval in which most 
+            of its events occur. Ties among time intervals are broken by assigning the 
+            case to the first time interval.
+
+        * ``plt_type`` can take one of the following four values:
+
+          * `'univariate'`: Plots the periodic evolution of
+
+            #. the absolute amount of distinct variants present in each time period
+
+            #. the absolute amount of distinct new variants introduced in each time period
+
+            #. the fraction of cases belonging to variants already seen in previous time periods
+
+            #. the fraction of cases belonging to variants first observed in each time period
+
+          * `'type_tt'`: Next ot the univariate plots, also plots the periodic evolution of
+
+            #. the aggregated throughput time of cases pertaining to existing variants 
+               in each time period
+            
+            #. the aggregated throughput time of cases pertaining to new 
+               variants in each time period
+
+          * `'type_events_case'`: Next to the univariate plots, also plots 
+            the periodic evolution of
+          
+            #. the aggregated Number of Events Per Case (NEPC) of cases 
+               pertaining to existing variants in each time period
+            
+            #. the aggregated Number of Events Per Case (NEPC) of cases 
+               pertaining to new variants in each time period
+
+          * `'type_outcome'`: (Only applicable if an outcome is already 
+            specified upon initialization of the `DynamicLogPlots` instance, 
+            or with the ``set_outcomeColumn(outcome)`` method.) Next to the 
+            univariate plots, also plots the periodic evolution of
+
+            #. the fraction of cases with `outcome=True` of cases 
+               pertaining to existing variants in each time period 
+            
+            #. the fraction of cases with `outcome=True` of cases 
+               pertaining to new variants in each time period
+
+        * ``numeric_agg`` can take on the following five values:
+
+          * `'mean'` : The requested time series are computed by taking the mean for each 
+            time period. E.g. for `plt_type='type_tt'`, for each time interval, 
+            the mean throughput time (TT) of cases pertaining to already 
+            existing variants, and the mean TT of cases pertaining 
+            to newly introduced variants is computed.
+
+          * `'median'` : The requested time series are computed by taking the median for  
+            each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
+            the median case length (in Number of Events Per Case, aka NEPC) 
+            of cases pertaining to already existing variants, and the median 
+            NEPC of cases pertaining to newly introduced variants is computed.
+
+          * `'min'` : The requested time series are computed by taking the minimum for 
+            each time interval. E.g. for `plt_type='type_events_case'`, for each time interval, 
+            the minimum case length (in Number of Events Per Case, aka NEPC) 
+            of cases pertaining to already existing variants, and the minimum 
+            NEPC of cases pertaining to newly introduced variants is computed.
+
+          * `'max'` : The requested time series are computed by taking the maximum for 
+            each time interval. E.g. for `plt_type='type_tt'`, for each time interval, 
+            the maximum throughput time (TT) of cases pertaining to already 
+            existing variants, and the maximum TT of cases pertaining 
+            to newly introduced variants is computed.
+
+          * `'std'` : The requested time series are computed by taking the 
+            standard deviation for each time interval. E.g. for 
+            `plt_type='type_tt'`, for each time interval, the standard 
+            deviation of the throughput time (TT) of cases pertaining to 
+            already existing variants, and the standard deviation of the TT 
+            of cases pertaining to newly introduced variants is computed.
+
         """
         valm._verify_distinctvars(outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment, plt_type = plt_type, 
                                     numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem, cases_initialized = cases_initialized)
         
         up.distinct_variants_AdvancedEvol(log = self.log, outcome = self.outcome, time_unit = time_unit, frequency = frequency, case_assignment = case_assignment, 
                                     type = plt_type, numeric_agg = numeric_agg, xtr_outlier_rem = xtr_outlier_rem, cases_initialized = cases_initialized)
```

### Comparing `DyLoPro-0.1.0/DyLoPro/__init__.py` & `DyLoPro-0.1.1/DyLoPro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 temporary or permanent changes and trends of interest
 from different perspectives, which upon identification 
 could be further analyzed in a manner deemed appropriate 
 by the user.
 """
 __author__ = """Brecht Wuyts """
 __email__ = 'brecht.wuyts@kuleuven.be'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 from DyLoPro.DynamicLogPlotting import DynamicLogPlots
```

### Comparing `DyLoPro-0.1.0/DyLoPro/check_args.py` & `DyLoPro-0.1.1/DyLoPro/check_args.py`

 * *Files identical despite different names*

### Comparing `DyLoPro-0.1.0/DyLoPro/plotting_utils.py` & `DyLoPro-0.1.1/DyLoPro/plotting_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 import numpy as np
 
-def select_string_column(log, case_agg, col, case_id_key = 'case:concept:name'):
+def select_string_column(log, 
+                         case_agg, 
+                         col, 
+                         case_id_key = 'case:concept:name'):
     """
-    Extract N columns (for N different attribute values; hotencoding) for the features 
-    dataframe for the given string attribute.
+    Extract N columns (for N different attribute values; hotencoding) for 
+    the features dataframe for the given string attribute.
 
     Code of this function inspired by source code of PM4PY. 
 
     Parameters
     --------------
     log
         Dataframe
@@ -38,29 +41,35 @@
             case_agg[new_col] = case_agg[case_id_key].copy().isin(filt_log_cases)
             case_agg[new_col] = case_agg[new_col].copy().astype("int")
     return case_agg
 
 def select_number_column(log, case_agg, col, numEventFt_transform, 
                          case_id_key = 'case:concept:name') -> pd.DataFrame:
     """
-    Extract a column for the features dataframe for the given numeric attribute.
+    Extract a column for the features dataframe for the given numeric 
+    attribute.
 
     Code of this function inspired by source code of PM4PY. 
 
     Parameters
     ----------
     log : pandas.DataFrame
-        Event log. 
+        Event log.
+
     case_agg
-        Feature dataframe
+        Feature dataframe.
+
     col
-        Numeric column
-    numEventFt_transform : {'last', 'first', 'mean', 'median', 'sum', 'prod', 'min', 'max'}
-        Determines the way in which these numerical event features are transformed to the 
-        case level. By default 'last'. 
+        Numeric column.
+
+    numEventFt_transform : {'last', 'first', 'mean', 'median', 'sum', 'prod', 
+                            'min', 'max'}
+        Determines the way in which these numerical event features are 
+        transformed to the case level. By default 'last'.
+        
     case_id_key
         Case ID key
 
     Returns
     ----------
     case_agg
         Feature dataframe (desidered output)
@@ -69,31 +78,37 @@
     log_agg = log.dropna(subset=[col]).groupby(case_id_key, sort=False)[col].agg(numEventFt_transform).reset_index().copy()
     case_agg = case_agg.merge(log_agg, on=[case_id_key], how="left", suffixes=('', '_y'))
     return case_agg
 
 def get_features_df(log: pd.DataFrame, column_list,
                     case_id_key = 'case:concept:name', numEventFt_transform = 'last') -> pd.DataFrame:
     """
-    Given a dataframe and a list of columns, performs an automatic feature extraction
+    Given a dataframe and a list of columns, performs an automatic feature 
+    extraction.
 
     Code of this function inspired by source code of PM4PY. 
 
     Parameters
     ----------
     log : pandas.DataFrame
-        Event log. 
+        Event log.
+
     column_list : list of str
-        The column names (in 'log') for which the event features need to be elevated 
-        to the case level. 
+        The column names (in 'log') for which the event features need to be 
+        elevated to the case level.
+
     case_id_key : str, optional
-        Column name (in 'log') that contains the case ID. By default 'case:concept:name'.
-    numEventFt_transform : {'last', 'first', 'mean', 'median', 'sum', 'prod', 'min', 'max'}
-        If any numeric event features contained in 'column_list', 'numEventFt_transform' 
-        determines the way in which these numerical event features are transformed to the 
-        case level. By default 'last'. 
+        Column name (in 'log') that contains the case ID. By default 
+        'case:concept:name'.
+
+    numEventFt_transform : {'last', 'first', 'mean', 'median', 'sum', 'prod', 
+                            'min', 'max'}
+        If any numeric event features contained in ``column_list``, 
+        ``numEventFt_transform`` determines the way in which these numerical 
+        event features are transformed to the case level. By default 'last'.
 
     Returns
     ----------
     case_agg
         Feature dataframe (desidered output)
     """
     case_agg = pd.DataFrame({case_id_key: list(log[case_id_key].unique())})
@@ -101,69 +116,88 @@
         data_tp = str(log[col].dtype)
         if "obj" in data_tp or "str" in data_tp or "bool" in data_tp or "categ" in data_tp:
             case_agg = select_string_column(log, case_agg, col, case_id_key=case_id_key)
         elif "float" in data_tp or "int" in data_tp:
             case_agg = select_number_column(log, case_agg, col, numEventFt_transform, case_id_key=case_id_key)
     return case_agg
 
-def _event_fts_to_tracelvl(log, event_features, numEventFt_transform = 'last'):
+def _event_fts_to_tracelvl(log, 
+                           event_features, 
+                           numEventFt_transform = 'last'):
     """Transforms categorical and numerical event features to the trace level.
 
     Parameters
     ----------
     log : pandas.DataFrame
-        Current event log. 
+        Current event log.
+
     event_features : list of str
-        Column names of the event features that need to be elevated to the trace level. 
-    numEventFt_transform : {'last', 'first', 'mean', 'median', 'sum', 'prod', 'min', 'max'}
-        If any numeric event features contained in 'event_features', 'numEventFt_transform' 
-        determines the way in which these numerical event features are transformed to the 
+        Column names of the event features that need to be elevated to the 
+        trace level.
+
+    numEventFt_transform : {'last', 'first', 'mean', 'median', 'sum', 'prod', 
+                            'min', 'max'}
+        If any numeric event features contained in ``event_features``, 
+        ``numEventFt_transform`` determines the way in which these 
+        numerical event features are transformed to the 
         case level. By default 'last'. 
 
     Returns
     -------
-    _type_
-        _description_
+    log : pd.DataFrame
+        Enhanced event log in which the event features are transformed to the 
+        trace level. 
+
+        For:
+
+        * numeric event features: For each trace, all **non-null** 
+          occurences of that feature are aggregated into a single case 
+          measure based on the ``numEventFt_transform`` argument. If a 
+          case only contains null values for that feature, it is 
+          assigned an NaN value. 
+
+        * categorical event features: A binary column (0-1) is added for each 
+          level of that feature. For each case, a value of 1 is assigned if 
+          that level occurs at least in one of its events, and 0 otherwise. 
+          It is important to note that, for categorical event features, this 
+          function is only called with a reduced event log, in which only the 
+          levels of interest for a certain categorical event feature are 
+          retained, while all other levels are discarded. In that way, 
+          high-level categoricals do not cause memory overload and / or 
+          computational bottlenecks. As such, for categorical event features, 
+          this function is only called for one feature at a time. 
+
     """
-    '''Transforms categorical and numeric event features to the trace level.
-        args:
-            - log               : pd.DataFrame
-            - event_features    : list of strings, containing the column names of the event features to be preprocessed. 
-
-        returns:
-            - log: enhanced pd.DataFrame in which the event features are transformed to the trace level:
-                    - numeric event features: last recorded (non-null) value for each trace taken; name= [original name]+'_trace'
-                    - categorical event features: binary column (0 - 1) added for each level; names = [original name]+'_'+[level name]
-    '''
     feature_table = get_features_df(log, event_features, numEventFt_transform = numEventFt_transform)
     log = log.merge(feature_table, on='case:concept:name', how='left', suffixes=("","_trace"))
     return log
 
 
 def determine_time_col(frequency, case_assignment):
     """Determine the time period column ('time_col') that indicates 
     to which time period each case should be assigned too. 
 
     Parameters
     ----------
-    frequency : {'minutely', '5-minutely', '10-minutely', 
-                'half-hourly', 'hourly' '2-hourly', '12-hourly', 'daily', 
-                'weekly', '2-weekly', 'monthly', 'quarterly', 'half-yearly'}
+
+    frequency : {'minutely', '5-minutely', '10-minutely', 'half-hourly', 'hourly' '2-hourly', '12-hourly', 'daily', 'weekly', '2-weekly', 'monthly', 'quarterly', 'half-yearly'}
         Determines the intervals of time periods to which cases are 
         assigned.
+
     case_assignment : {'first_event', 'last_event', 'max_events'}
         Given the time intervals determined by 'frequency', 
         'case_assigment' determines the the condition upon which
         each case is assigned to a certain time period. 
 
     Returns
     -------
     time_col : str
         Time period column that contains for each case the time period
-        it should be assigned to. 
+        it should be assigned to.
+
     """
     frequencies = ['minutely', '5-minutely', '10-minutely', 'half-hourly', 
                    'hourly', '2-hourly', '12-hourly', 'daily', 'weekly', 
                    '2-weekly', 'monthly', 'quarterly', 'half-yearly']
     
     periodic_timestamps = ['1min_timestamp', '5min_timestamp', '10min_timestamp', 
                            '30min_timestamp', 'hourly_timestamp', '2hour_timestamp', 
@@ -180,38 +214,58 @@
 
     cassi_idx = case_assignments.index(case_assignment)
     time_col = time_col + assignment_suffixes[cassi_idx]
 
     return time_col 
 
 def determine_tt_col(time_unit):
-    '''
-        args: 
-            - time_unit: string = 'microseconds', 'milliseconds', 'seconds', 'minutes', 'hours', 'days' or 'weeks'; time unit for Throughput Time 
-
-        returns:
-            - tt_col: string ; name of the throughput time (tt) column with correct time unit. 
-    '''
+    """Determine the appropriate time unit column for the throughput time 
+    based on the ``time_unit`` argument specified by the user. 
+
+    Parameters
+    ----------
+
+    time_unit : {'microseconds', 'milliseconds', 'seconds', 'minutes', 
+                'hours', 'days', 'weeks'}
+        Time unit for the throughput time specified by the user. 
+
+    Returns
+    -------
+    tt_col : str
+        Column name throughput time with correct unit in the preprocessed 
+        event log. 
+    """
     tt_cols = ['tt_microseconds', 'tt_milliseconds', 'tt_seconds', 'tt_minutes', 'tt_hours', 'tt_days', 'tt_weeks']
     time_unit_list = ['microseconds', 'milliseconds', 'seconds', 'minutes', 'hours', 'days', 'weeks']
     time_unit_idx = time_unit_list.index(time_unit)
     tt_col = tt_cols[time_unit_idx]
     
     return tt_col
 
 def get_outcome_percentage(filtered_log, outcome, time_col):
-    ''' Computes the periodic percentage of cases with outcome == 1 for a filtered log
-        args:
-            - filtered_log: pd.DataFrame; case log (i.e. log with 1 row per case) that is filtered based on a condition.
-            - outcome:      string of the outcome column. (Has to be a binary outcome column with 0 and 1's)
-            - time_col:     string of the periodic timestamp column.
-
-        returns:
-            - periodic % of (the filtered) cases with outcome == 1 
-    '''
+    """Compute for each time bucket the fraction of cases with 
+    ``outcome=1`` for the cases in ``filtered_log``. 
+
+    Parameters
+    ----------
+    filtered_log : pd.DataFrame
+        FIltered event log. The case filtering is performed by the plotting 
+        functions calling this util function, and depends on the purpose and 
+        arguments of these plotting functions. 
+    outcome : str
+        Name of the outcome column in ``filtered_log``.
+    time_col : str
+        The time column of interest in the event log. Determined in the 
+        plotting functions calling this util function. 
+
+    Returns
+    -------
+    pd.DataFrame
+        Periodic fraction of cases with ``outcome=1``. 
+    """
     # Periodic number of cases in the filtered log. (I.e. periodic number of cases that satisfy the condition on which you have filtered.)
     per_counts = filtered_log.pivot_table(values= 'case:concept:name',index= time_col, aggfunc='count', fill_value=0)
     per_counts.columns = ['total']
     # Filtering the filtered cases on outcome == 1
     filtered_case = filtered_log[filtered_log[outcome]==1]
     # Periodic number of those filtered cases with outcome == 0 and outcome == 1
     per_true = filtered_case.pivot_table("case:concept:name",index= time_col, aggfunc="count", fill_value=0)
@@ -223,24 +277,54 @@
         per_counts = per_counts.merge(per_true, left_index = True, right_index = True, how='left')
 
     per_counts['prc_true'] = per_counts['num_true'] / per_counts['total']
 
     return per_counts[['prc_true']]
 
 def get_dfr_time(log, case_log, dfr_list, time_col, numeric_agg):
-    ''' For each case: computes the performance (time between) for each occurance of the given dfr (if any).
-        args: 
-            - log: pd.DataFrame 
-            - dfr_list: list of tuples; [('activity_string_1', 'activity_string_2'), ...]
-
-        returns: 
-            - period_dfr_perf:  pd.DataFrame; aggregated periodic performances (time between) for each of the given dfr's in dfr_list
-            - perf_units_cols:  list of strings; indicating the automatically determined time_unit for each of the columns / dfr's. The possibilities
-                                are 'days', 'hours', 'minutes', 'seconds', 'milliseconds' and 'microseconds'. 
-    '''
+    """Compute, for each case, the DFR performance (i.e. time elapsed 
+    between the occurrence of the first and second activity of a given 
+    Directly-Follows Relationship (DFR)) for each occurrence of each 
+    DFR in ``dfr_list``. Then, the cases are grouped into discrete 
+    time buckets, producing for each DFR a set of DFR performances. 
+    Finally, for each of the DFRs in ``dfr_list``, an aggregate 
+    DFR perforamnce is computed for each time bucket, with the 
+    aggregation function being determined by the ``numeric_agg`` 
+    parameter. 
+
+    Parameters
+    ----------
+    log : pd.DataFrame
+        The (preprocessed) event log. 
+    case_log : pd.DataFrame
+        Dataframe containing only one row for each case. 
+    dfr_list : list of tuple 
+        The Directly-Follows Relations for which the periodically aggregated 
+        DFR performances are computed. Should be formatted as follows: 
+        [('activity_string_1', 'activity_string_2'), ...].
+        _description_
+    time_col : str
+        The time column of interest in the event log. Determined in the 
+        plotting functions calling this util function. 
+    numeric_agg : str
+        How the DFRs assigned to each time bucket should be aggregated 
+        towards one aggregated measure. 
+
+    Returns
+    -------
+    period_dfr_perf : pd.DataFrame 
+        Dataframe with on the rows the chronologically ordered time buckets, 
+        and with each column being the aggregated DFR performances for one of 
+        of the DFRs listed in ``dfr_list``.
+    perf_units_cols : list of string
+        The most suitable time units are, for each requested DFR separately, 
+        determined automatically. This list contains these time units in the 
+        correct order, such that the appropriate time units can be displayed 
+        in the visualizations. 
+    """
 
     time_products = [1, 24, 1440, 86400, 86400000, 86400000000]
     perf_units = ['days', 'hours', 'minutes', 'seconds', 'milliseconds', 'microseconds']
 
     
     log_loc = log.copy()
     log_loc['next:concept:name'] = log_loc.groupby(['case:concept:name'])['concept:name'].shift(-1)
@@ -272,59 +356,89 @@
     time_prods_resbc = np.broadcast_to(time_prods_res[None, :], (period_dfr_perf.shape[0], num_cols))
     period_dfr_perf = np.multiply(period_dfr_perf[col_strings], time_prods_resbc)
     perf_units_cols = [perf_units[idx] for idx in time_indices] # (num_cols, )
 
     return period_dfr_perf, perf_units_cols 
 
 def get_maxrange(agg_df):
-    ''' Computes for each of the given arrays / pd Series the maximum y-range, by neglecting extreme outliers (values > q3 + 3*iqr). 
-        args:
-            - agg_df: (num periods, num series) - shaped dataframe, containing the series for which outliers should be accounted for before plotting. 
-        
-        returns: 
-            - max_values:   (num series, ) - shaped np.ndarray, containing the max y-values < q3 + 3*iqr for each of the columns / series in agg_df. 
-    '''
+    """Compute for each of the given arrays / pd.Series the maximum value 
+    that should not be considered as an extreme outlier (i.e. < q3 + 3 x iqr).
+
+    Parameters
+    ----------
+    agg_df : pd.DatFrame
+        Shape (num periods, num series), with num periods being the amount of 
+        time buckets, and num series being the amount of time series for 
+        which outliers should be accounted for. 
+
+    Returns
+    -------
+    max_values : np.ndarray
+        The 'num series' maximum values not to be considered as extreme 
+        outliers.
+    """
 
     q1 = np.quantile(agg_df, 0.25, axis = 0) # shape (num series, )
     q3 = np.quantile(agg_df, 0.75, axis = 0) # shape (num series, )
     iqr = q3 - q1 
     upper_bound = q3 + (3*iqr)
     # Replacing the extreme outliers in each column by NaN:
     agg_df_MinusFliers = np.where(agg_df>upper_bound[None,:], np.nan, agg_df) # shape (num periods, num series)
 
     return np.nanmax(agg_df_MinusFliers, axis=0)  # max_values: shape (num series, )
 
 
 def get_variant_case(log):
-    ''' Takes the whole log as input, and returns a pd.DataFrame with the case id in column 0, and the variant (as a tuple) in column 1
-        
-        args:
-            - log: pd.DataFrame
+    """Return a pd.Dataframe with a row row for each case, containing the 
+    unique case ID and the corresponding variant (as a tuple) in its columns.
 
-        returns:
-            - case_variant: pd.DataFrame with 1 row for each case and 2 columns: 'case:concept:name' and 'variant'. 
-    '''
+    Parameters
+    ----------
+    log : pd.DataFrame
+        The event log.
+
+    Returns
+    -------
+    case_variant : pd.DataFrame
+        Dataframe with one row for each case and two columns, 
+        'case:concept:name' and 'variant'.
+    """
     log_loc = log[['case:concept:name', 'concept:name']].copy()
     case_variant = log_loc.groupby(['case:concept:name'], as_index = False, sort = False).agg({'concept:name': ','.join})
     case_variant.columns = ['case:concept:name', 'variant']
     case_variant['variant'] = case_variant['variant'].apply(lambda x: tuple(x.split(',')))
     return case_variant
 
 def get_tt_ratios(log, num_fts_list, time_col, numeric_agg):
-    ''' Computes the periodic ratio of throughput time over numerical feature and automatically determines the most appropriate time unit for that ratio 
-        for each of the numerical features in num_fts_list simultaneously. 
-        args: 
-            - log               :   pd.DataFrame 
-            - num_fts_list      :   list of strings; containing the column names of the numerical features. 
-
-        returns: 
-            - period_ttr        :   pd.DataFrame; aggregated periodic ratios for each of the given numerical features in num_fts_list
-            - perf_units_cols   :   list of strings; indicating the automatically determined time_unit for each of the columns / given numerical features. The possibilities
-                                    are 'days', 'hours', 'minutes', 'seconds', 'milliseconds' and 'microseconds'. 
-    '''
+    """Compute the periodic ratio of throughput time over numerical feature 
+    and automatically determine the most appropriate time unit for that ratio 
+    for each of the numerical features in ``num_fts_list`` simultaneously. 
+
+    Parameters
+    ----------
+    log : pd.DataFrame
+        The event log.
+    num_fts_list : list of str
+        Column names of numeric features of interest.
+    time_col : str
+        The time column of interest in the event log. Determined in the 
+        plotting functions calling this util function. 
+    numeric_agg : str
+        How the ratios assigned to each time bucket should be aggregated 
+        towards one aggregated measure. 
+
+    Returns
+    -------
+    period_ttr : pd.DataFrame
+        Periodically aggregated TT ratios for each of the numeric features 
+        given in `num_fts_list`.
+    perf_units_cols : list of str
+        Indicating the automatically determined time unit for each of the 
+        requested numeric features.
+    """
     log_loc = log.copy()
     case_log_cop = log_loc.drop_duplicates(subset = 'case:concept:name').copy()
     time_products = [1, 24, 1440, 86400, 86400000, 86400000000]
     ratio_units = ['days', 'hours', 'minutes', 'seconds', 'milliseconds', 'microseconds']
     num_units = 6
 
     fts_list_ext = num_fts_list.copy()
@@ -356,23 +470,29 @@
     time_prods_resbc = np.broadcast_to(time_prods_res[None, :], (period_ttr.shape[0], num_cols))
     period_ttr = np.multiply(period_ttr[col_strings], time_prods_resbc)
     ratio_units_cols = [ratio_units[idx] for idx in time_indices] # (num_cols, )
 
     return period_ttr, ratio_units_cols 
 
 def get_sorted_DFRs(log):
-    ''' Retrieves all the Directly-Follows Relations (DFRs) in the log, sorts them from highest to lowest frequency, 
-        and returns them as a list of tupples. E.g. [('act_1_dfr_1', 'act_2_dfr_1'), ('act_1_dfr_2', 'act_2_dfr_2'), ...]
+    """Retrieve all the Directly-Follows Relations (DFRs) in the log, sort
+    them from highest to lowest frequency, and return them as a list of 
+    tuples. E.g. [('act_1_dfr_1', 'act_2_dfr_1'), ('act_1_dfr_2', 'act_2_dfr_2'), 
+    ...].
 
-        args:
-            - log       :   pd.DataFrame
-        
-        returns:
-            - list_dfr  :   sorted list of all the DFRs, as specified here above. 
-    '''
+    Parameters
+    ----------
+    log : pd.DataFrame
+        The event log.
+
+    Returns
+    -------
+    list_dfr : str of tuple
+        Sorted list of DFRs (in descending order of frequency).
+    """
     locallog = log[['case:concept:name', 'concept:name']].copy()
     locallog['next:concept:name'] = locallog.groupby('case:concept:name')['concept:name'].shift(-1)
     locallog = locallog.dropna(subset='next:concept:name').copy()
     locallog['dfr_start'] = list(zip(locallog['concept:name'], locallog['next:concept:name']))
     dfr_df = pd.DataFrame(locallog['dfr_start'].value_counts()).reset_index()
     dfr_df.columns = ['DFR', 'DFR count']
     list_dfr = list(locallog['dfr_start'].value_counts().index)
@@ -488,28 +608,37 @@
     if counts: 
         return filtered_var_df
     
     return filtered_var_df[['variant']]
     
 
 def get_uniq_varcounts(log, time_col):
-    ''' Computes the number of distinct variants in each time bucket, as well as the number of distinct previously 
-        unseen / distinct new variants in each time bucket. 
+    """Compute the number of distinct variants in each consecutive time 
+    bucket, as well as the number of distinct previously unseen variants 
+    in each time bucket.
+
+    Parameters
+    ----------
+    log : pd.DataFrame
+        Event log that is already enhanced, prior to this function being 
+        called, with an additional 'variant' column containing the variant 
+        of each case. 
+    time_col : str
+        The time column of interest in the event log. Determined in the 
+        plotting functions calling this util function. 
+
+    Returns
+    -------
+    periodic_varcounts : pd.DataFrame
+        Containing the chronologically ordered time buckets as the indices, 
+        and two columns, containing for each time bucket the number of 
+        distinct variants, and the number of distinct variants not seen in 
+        any of the preceding periods, respectively. 
+    """
 
-        args:
-            - log               :   pd.DataFrame, already enhanced with a column that contains the variant of that case. 
-            - time_col          :   string; indicating the column in which the 'periodic group' of that case is documented.
-        
-        returns:
-            - period_varcounts  :   pd.DataFrame containing:
-                                    -   the sorted time periods / buckets as the indices
-                                    -   the number of distinct variants in each time bucket / period as the 'num_distinct_vars' column
-                                    -   the number of distinct previously unseen / dinstinct new variants in each time bucket as the
-                                        'num_NEW_distinct_vars' column 
-    '''
     # First the amount of distinct variants (not per se unseen) in each period:
     local_log = log[['case:concept:name', time_col, 'variant']].copy()
     local_log = local_log.drop_duplicates(subset= 'case:concept:name')
     period_numDistinctvars = local_log.pivot_table(values ='variant', index = time_col, aggfunc = pd.Series.nunique, fill_value = 0)
 
     local_log = local_log.sort_values(time_col)
     local_log = local_log.drop_duplicates(subset = 'variant')
@@ -521,26 +650,37 @@
     period_numDistinctvars.columns = ['num_distinct_vars']
     period_numUnseenVars.columns = ['num_NEW_distinct_vars']
     period_varcounts = period_numDistinctvars.merge(period_numUnseenVars, left_index = True, right_index = True, how = 'left').fillna(0)
 
     return period_varcounts
 
 def get_ordered_variantMap(case_log, time_col):
-    ''' Computes a variant mapping that maps the tuple representation of a variant to a unique string. The mapping is ordered. 
+    """Computes a variant mapping that maps the tuple representation of a 
+    variant to a unique string. The mapping is ordered. Only used by the 
+    ``get_neVar_cases()`` util function in this same module.
 
-        args:
-            - case_log          :   pd.DataFrame, 1 row per case, already enhanced with a column that contains the variant of that case. 
-            - time_col          :   string; indicating the column in which the 'periodic group' of that case is documented.
-        
-        returns:
-            - case_log               :   pd.DataFrame containing an additional column: variant_str'
-            - periodic_newvars  :   pd.DataFrame containing 2 columns: 1st column containing the unique periodic timestamps (determined by time_col),
-                                    and the 2nd column containing the tuple of (mapped) variant strings containing the previously unseen variants that
-                                    occurred for the first time in that time period. 
-    '''
+    Parameters
+    ----------
+    case_log : pd.DataFrame
+        Event log containing only one row for each case. Already enhanced with 
+        a column that contains the variant of that case.
+    time_col : str
+        Column name specifying the relevant time bucket each case should be 
+        assigned to. 
+
+    Returns
+    -------
+    case_log : pd.DataFrame
+        case_log containing an additional column 'variant_str'.
+    periodic_newvars : pd.DataFrame 
+        Contains two columns, the chronologically ordered unique periodic 
+        timestamps / time buckets, and a tuple of mapped variant strings in 
+        the second column containing the variants that were first observed 
+        in the corresponding time bucket. 
+    """
     local_log = case_log[['case:concept:name', 'time:timestamp', time_col, 'variant']].copy()
     local_log = local_log.drop_duplicates(subset = 'case:concept:name')
     local_log = local_log.sort_values([time_col, 'time:timestamp'])
     local_log = local_log.drop_duplicates(subset = 'variant')
     local_log.loc[:,'variant_str'] = ['Variant_{}'.format(i) for i in range(len(local_log))]
     variant_map = local_log[['variant', 'variant_str']]
     case_log = case_log.merge(variant_map, on = 'variant', how = 'left')
@@ -550,26 +690,39 @@
     periodic_newvars = local_log.groupby([time_col], as_index = False, sort = False).agg({'variant_str': ','.join})
     periodic_newvars.columns = [time_col, 'new_variants']
     periodic_newvars.loc[:, 'new_variants'] = periodic_newvars.loc[:, 'new_variants'].apply(lambda x: tuple(x.split(',')))
     
     return case_log, periodic_newvars
 
 def get_newVar_cases(log, time_col):
-    ''' Determines which cases belong to variants that were introduced for the first time during its corresponding periodic timestamp (determined by time_col). 
+    """Determines for each consecutive time period / time bucket the cases 
+    pertaining to variants that were first observed in that time period. 
+    
+    Only called by the ``distinct_variants_AdvancedEvol()`` plotting method. 
 
-        args:
-            - log               :   pd.DataFrame, already enhanced with a column that contains the variant of that case. 
-            - time_col          :   string; indicating the column in which the 'periodic group' of that case is documented.
-        
-        returns:
-            - log               :   pd.DataFrame containing an additional column: variant_str'
-            - periodic_newvars  :   pd.DataFrame containing 2 columns: 1st column containing the unique periodic timestamps (determined by time_col),
-                                    and the 2nd column containing the tuple of (mapped) variant strings containing the previously unseen variants that
-                                    occurred for the first time in that time period. 
-    '''
+    Parameters
+    ----------
+    log : pd.DataFrame 
+        Event log that is already enhanced, prior to this function being 
+        called, with an additional 'variant' column containing the variant 
+        of each case. 
+    time_col : str
+        The time column of interest in the event log. Determined in the 
+        plotting functions calling this util function. 
+
+    Returns
+    -------
+    log : pd.DataFrame
+        Event log containing additional column 'variant_str'.
+    periodic_newvars : pd.DataFrame 
+        Contains two columns, the chronologically ordered unique periodic 
+        timestamps / time buckets, and a tuple of mapped variant strings in 
+        the second column containing the variants that were first observed 
+        in the corresponding time bucket. 
+    """
     loc_log = log.drop_duplicates(subset = 'case:concept:name').copy()
     case_id_log = loc_log[['case:concept:name']].copy()
     enhanced_log, periodic_newvars = get_ordered_variantMap(case_log = loc_log, time_col = time_col)
     time_col_list = periodic_newvars[time_col].unique()
     newVar_cases = []
     for period in time_col_list:
         new_vars = periodic_newvars.loc[periodic_newvars[time_col]==period,'new_variants'].item()
```

### Comparing `DyLoPro-0.1.0/DyLoPro/preprocess_utils.py` & `DyLoPro-0.1.1/DyLoPro/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `DyLoPro-0.1.0/DyLoPro/univariate_plots.py` & `DyLoPro-0.1.1/DyLoPro/univariate_plots.py`

 * *Files identical despite different names*

### Comparing `DyLoPro-0.1.0/DyLoPro/validate_methods.py` & `DyLoPro-0.1.1/DyLoPro/validate_methods.py`

 * *Files identical despite different names*

### Comparing `DyLoPro-0.1.0/DyLoPro.egg-info/SOURCES.txt` & `DyLoPro-0.1.1/DyLoPro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DyLoPro-0.1.0/LICENSE` & `DyLoPro-0.1.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007
 
-    To be filled in later...
+    DyLoPro
     Copyright (C) 2023  Brecht Wuyts 
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
```

### Comparing `DyLoPro-0.1.0/setup.py` & `DyLoPro-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='DyLoPro',
     name='DyLoPro',
     packages=find_packages(include=['DyLoPro', 'DyLoPro.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/BrechtWts/DyLoPro',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `DyLoPro-0.1.0/tests/test_DyLoPro.py` & `DyLoPro-0.1.1/tests/test_DyLoPro.py`

 * *Files identical despite different names*

