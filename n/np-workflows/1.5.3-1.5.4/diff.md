# Comparing `tmp/np_workflows-1.5.3.tar.gz` & `tmp/np_workflows-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_workflows-1.5.3.tar", last modified: Thu Jul 13 02:09:37 2023, max compression
+gzip compressed data, was "np_workflows-1.5.4.tar", last modified: Tue Jul 18 01:28:10 2023, max compression
```

## Comparing `np_workflows-1.5.3.tar` & `np_workflows-1.5.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1614 2023-06-30 17:48:35.853909 np_workflows-1.5.3/README.md
--rw-r--r--   0        0        0     2557 2023-07-13 02:09:37.207147 np_workflows-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.5.3/src/np_workflows/__init__.py
--rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.5.3/src/np_workflows/assets/images/logo_np_hab.png
--rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.5.3/src/np_workflows/assets/images/logo_np_vis.png
--rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.5.3/src/np_workflows/experiments/__init__.py
--rw-r--r--   0        0        0      148 2023-05-18 23:17:52.356257 np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/__init__.py
--rw-r--r--   0        0        0     2737 2023-06-08 01:15:00.774997 np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py
--rw-r--r--   0        0        0     4401 2023-05-11 18:20:25.162316 np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py
--rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py
--rw-r--r--   0        0        0     7621 2023-06-05 04:11:33.975384 np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py
--rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-18 01:58:07.942705 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py
--rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_00.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.949928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_01.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_02.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_03.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_04.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_05.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_06.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.919928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_07.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.889928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_08.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_09.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.859928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_10.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.839929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_11.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.829929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_12.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_13.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.799929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_14.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.789932 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_15.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.769930 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_16.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.759930 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_17.stim
--rw-r--r--   0        0        0      337 2023-03-08 20:59:00.749930 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_18.stim
--rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/flash_250ms.stim
--rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim
--rw-r--r--   0        0        0      340 2023-03-08 20:59:00.949928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/old_stim.stim
--rw-r--r--   0        0        0      334 2023-03-08 20:59:00.959929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed.stim
--rw-r--r--   0        0        0      345 2023-03-08 20:59:00.979929 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_1st.stim
--rw-r--r--   0        0        0      346 2023-03-08 20:59:00.969928 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_2nd.stim
--rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
--rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
--rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
--rw-r--r--   0        0        0     9220 2023-05-18 02:12:21.002654 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
--rw-r--r--   0        0        0     2684 2023-06-08 00:43:09.047204 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
--rw-r--r--   0        0        0     8693 2023-05-24 16:37:52.954146 np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
--rw-r--r--   0        0        0      200 2023-05-19 23:52:58.915202 np_workflows-1.5.3/src/np_workflows/experiments/templeton/__init__.py
--rw-r--r--   0        0        0    12933 2023-07-13 02:06:39.627189 np_workflows-1.5.3/src/np_workflows/experiments/templeton/main_templeton_pilot.py
--rw-r--r--   0        0        0     1779 2023-05-19 23:56:16.341090 np_workflows-1.5.3/src/np_workflows/experiments/templeton/templeton_stim_config.py
--rw-r--r--   0        0        0     2745 2023-07-11 23:54:16.807727 np_workflows-1.5.3/src/np_workflows/experiments/templeton/templeton_widgets.py
--rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.5.3/src/np_workflows/shared/__init__.py
--rw-r--r--   0        0        0    18321 2023-07-13 02:06:35.161196 np_workflows-1.5.3/src/np_workflows/shared/base_experiments.py
--rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.3/src/np_workflows/shared/camstim_scripts/flash_250ms.stim
--rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.3/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim
--rw-r--r--   0        0        0     6258 2023-05-04 01:03:37.729885 np_workflows-1.5.3/src/np_workflows/shared/npxc.py
--rw-r--r--   0        0        0    25914 2023-06-08 00:33:50.617758 np_workflows-1.5.3/src/np_workflows/shared/widgets.py
--rw-r--r--   0        0        0   753021 2023-04-14 19:17:10.939361 np_workflows-1.5.3/tests/logs/debug.log
--rw-r--r--   0        0        0   361698 2023-04-14 19:17:10.939361 np_workflows-1.5.3/tests/logs/warning.log
--rw-r--r--   0        0        0      508 2023-03-17 23:19:28.833208 np_workflows-1.5.3/tests/model_sandbox.py
--rw-r--r--   0        0        0    34554 2023-07-11 18:40:27.336659 np_workflows-1.5.3/tests/widget_sandbox.ipynb
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 np_workflows-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1614 2023-06-30 17:48:35.853909 np_workflows-1.5.4/README.md
+-rw-r--r--   0        0        0     2561 2023-07-18 01:28:10.863089 np_workflows-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-03-07 00:58:26.213008 np_workflows-1.5.4/src/np_workflows/__init__.py
+-rw-r--r--   0        0        0    10071 2023-02-02 02:47:52.020772 np_workflows-1.5.4/src/np_workflows/assets/images/logo_np_hab.png
+-rw-r--r--   0        0        0    19349 2023-02-02 02:47:52.021771 np_workflows-1.5.4/src/np_workflows/assets/images/logo_np_vis.png
+-rw-r--r--   0        0        0       39 2023-02-20 22:40:54.036068 np_workflows-1.5.4/src/np_workflows/experiments/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-18 23:17:52.356257 np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/__init__.py
+-rw-r--r--   0        0        0     2737 2023-06-08 01:15:00.774997 np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py
+-rw-r--r--   0        0        0     4401 2023-05-11 18:20:25.162316 np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py
+-rw-r--r--   0        0        0     7621 2023-06-05 04:11:33.975384 np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py
+-rw-r--r--   0        0        0      114 2023-03-09 03:08:15.270031 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-18 01:58:07.942705 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py
+-rw-r--r--   0        0        0     2094 2023-03-17 23:19:28.822209 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_00.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.949928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_01.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_02.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_03.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.939928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_04.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_05.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.929928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_06.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.919928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_07.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.889928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_08.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.909928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_09.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.859928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_10.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.839929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_11.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.829929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_12.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.819929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_13.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.799929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_14.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.789932 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_15.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.769930 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_16.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.759930 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_17.stim
+-rw-r--r--   0        0        0      337 2023-03-08 20:59:00.749930 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/densely_annotated_18.stim
+-rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/flash_250ms.stim
+-rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim
+-rw-r--r--   0        0        0      340 2023-03-08 20:59:00.949928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/old_stim.stim
+-rw-r--r--   0        0        0      334 2023-03-08 20:59:00.959929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed.stim
+-rw-r--r--   0        0        0      345 2023-03-08 20:59:00.979929 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_1st.stim
+-rw-r--r--   0        0        0      346 2023-03-08 20:59:00.969928 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/shuffle_reversed_2nd.stim
+-rw-r--r--   0        0        0     4004 2023-03-17 23:19:28.824209 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py
+-rw-r--r--   0        0        0     4400 2023-02-23 00:51:23.316978 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py
+-rw-r--r--   0        0        0     6249 2023-02-23 00:09:51.151791 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py
+-rw-r--r--   0        0        0     9220 2023-05-18 02:12:21.002654 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py
+-rw-r--r--   0        0        0     2684 2023-06-08 00:43:09.047204 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py
+-rw-r--r--   0        0        0     8693 2023-05-24 16:37:52.954146 np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py
+-rw-r--r--   0        0        0      200 2023-05-19 23:52:58.915202 np_workflows-1.5.4/src/np_workflows/experiments/templeton/__init__.py
+-rw-r--r--   0        0        0    12723 2023-07-18 01:01:55.386939 np_workflows-1.5.4/src/np_workflows/experiments/templeton/main_templeton_pilot.py
+-rw-r--r--   0        0        0     1779 2023-05-19 23:56:16.341090 np_workflows-1.5.4/src/np_workflows/experiments/templeton/templeton_stim_config.py
+-rw-r--r--   0        0        0     2745 2023-07-11 23:54:16.807727 np_workflows-1.5.4/src/np_workflows/experiments/templeton/templeton_widgets.py
+-rw-r--r--   0        0        0      131 2023-03-07 00:47:58.271771 np_workflows-1.5.4/src/np_workflows/shared/__init__.py
+-rw-r--r--   0        0        0    18321 2023-07-13 02:06:35.161196 np_workflows-1.5.4/src/np_workflows/shared/base_experiments.py
+-rw-r--r--   0        0        0      408 2023-05-18 01:45:39.420251 np_workflows-1.5.4/src/np_workflows/shared/camstim_scripts/flash_250ms.stim
+-rw-r--r--   0        0        0      718 2023-05-18 01:45:17.605960 np_workflows-1.5.4/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim
+-rw-r--r--   0        0        0     6258 2023-05-04 01:03:37.729885 np_workflows-1.5.4/src/np_workflows/shared/npxc.py
+-rw-r--r--   0        0        0    25914 2023-06-08 00:33:50.617758 np_workflows-1.5.4/src/np_workflows/shared/widgets.py
+-rw-r--r--   0        0        0   753021 2023-04-14 19:17:10.939361 np_workflows-1.5.4/tests/logs/debug.log
+-rw-r--r--   0        0        0   361698 2023-04-14 19:17:10.939361 np_workflows-1.5.4/tests/logs/warning.log
+-rw-r--r--   0        0        0      508 2023-03-17 23:19:28.833208 np_workflows-1.5.4/tests/model_sandbox.py
+-rw-r--r--   0        0        0    34554 2023-07-11 18:40:27.336659 np_workflows-1.5.4/tests/widget_sandbox.ipynb
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 np_workflows-1.5.4/PKG-INFO
```

### Comparing `np_workflows-1.5.3/README.md` & `np_workflows-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/pyproject.toml` & `np_workflows-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-workflows"
-version = "1.5.3"
+version = "1.5.4"
 description = "Ecephys and behavior workflows for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 readme = "README.md"
 requires-python = "==3.11.*"
 dependencies = [
@@ -55,15 +55,15 @@
     "src/np_workflows",
 ]
 
 [tool.pdm.scripts]
 ruff = "ruff check src --fix-only"
 blue = "blue src"
 pytest = "pytest --cov"
-bump = "bump -p pyproject.toml"
+bump = "pdm bump -p pyproject.toml"
 
 [tool.pdm.scripts.prebuild]
 composite = [
     "blue",
     "ruff",
     "pytest",
 ]
```

### Comparing `np_workflows-1.5.3/src/np_workflows/assets/images/logo_np_hab.png` & `np_workflows-1.5.4/src/np_workflows/assets/images/logo_np_hab.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/assets/images/logo_np_vis.png` & `np_workflows-1.5.4/src/np_workflows/assets/images/logo_np_vis.png`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py` & `np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/barcode_workflow_widget.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py` & `np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_mapping_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py` & `np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/camstim_scripts/barcode_opto_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py` & `np_workflows-1.5.4/src/np_workflows/experiments/openscope_barcode/main_barcode_pilot.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/make_tt_stims.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/oct22_tt_stim_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/stims/gabor_20_deg_250ms.stim`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_main_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_mapping_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/camstim_scripts/ttn_opto_script.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/main_ttn_pilot.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/ttn_session_widget.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py` & `np_workflows-1.5.4/src/np_workflows/experiments/task_trained_network/ttn_stim_config.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/templeton/main_templeton_pilot.py` & `np_workflows-1.5.4/src/np_workflows/experiments/templeton/main_templeton_pilot.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,38 +143,14 @@
         """For sending to runTask.py"""
         return dict(
                 rigName = str(self.rig).replace('.',''),
                 subjectName = 'sound',
                 taskScript = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/TaskControl.py',
                 taskVersion = 'sound test',
         )
-
-    def initialize_and_test_services(self) -> None:
-        """Configure, initialize (ie. reset), then test all services."""
-        
-        ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/runTask.py'
-        ScriptCamstim.data_root = pathlib.Path('//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/Data') / str(self.mouse)
-
-        MouseDirector.user = self.user.id
-        MouseDirector.mouse = self.mouse.id
-
-        OpenEphys.folder = self.session.folder
-
-        NewScaleCoordinateRecorder.log_root = self.session.npexp_path
-
-        self.configure_services()
-
-        super().initialize_and_test_services()
-
-    def update_state(self) -> None:
-        "Store useful but non-essential info."
-        self.mouse.state['last_session'] = self.session.id
-        self.mouse.state['last_workflow'] = str(self.workflow.name)
-        self.mouse.state['last_task'] = str(self.task_name)
-
     
     def run_script(self, stim: Literal['sound_test', 'mapping', 'task', 'optotagging', 'spontaneous', 'spontaneous_rewards']) -> None:
         ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/runTask.py'
         ScriptCamstim.params = getattr(self, f'{stim.replace(" ", "_")}_params')
 
         with contextlib.suppress(Exception):
             np_logging.web(f'templeton_{self.workflow.name.lower()}').info(f"{stim} started")
@@ -187,48 +163,59 @@
         if isinstance(ScriptCamstim, Finalizable):
             ScriptCamstim.finalize()
 
         with contextlib.suppress(Exception):
             np_logging.web(f'templeton_{self.workflow.name.lower()}').info(f"{stim} complete")
     
     
-    def run_mapping(self) -> None:
-        self.run_script('mapping')    
-            
-    def run_sound_test(self) -> None:
-        self.run_script('sound_test')    
-            
+    run_mapping = functools.partialmethod(run_script, 'mapping')
+    run_sound_test = functools.partialmethod(run_script, 'sound_test')
+    run_optotagging = functools.partialmethod(run_script, 'optotagging')
+    run_spontaneous = functools.partialmethod(run_script, 'spontaneous')
+    run_spontaneous_rewards = functools.partialmethod(run_script, 'spontaneous_rewards')
+    
     def run_task(self) -> None:
         self.update_state()
         self.run_script('task')    
-        
-    def run_optotagging(self) -> None:
-        self.run_script('optotagging')
-        
-    def run_spontaneous(self) -> None:
-        self.run_script('spontaneous')
-                
-    def run_spontaneous_rewards(self) -> None:
-        self.run_script('spontaneous_rewards')
-                
-    def set_grey_desktop_on_stim(self) -> None:
+           
+    def run_stim_desktop_theme_script(self, selection: str) -> None:     
         ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/ben/change_desktop.py'
-        ScriptCamstim.params = {'selection': 'grey'}
-        ScriptCamstim.start()
-        
-    def set_dark_desktop_on_stim(self) -> None:
-        ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/ben/change_desktop.py'
-        ScriptCamstim.params = {'selection': 'dark'}
+        ScriptCamstim.params = {'selection': selection}
         ScriptCamstim.start()
+        while not ScriptCamstim.is_ready_to_start():
+            time.sleep(0.1)
+
+    set_grey_desktop_on_stim = functools.partialmethod(run_stim_desktop_theme_script, 'grey')
+    set_dark_desktop_on_stim = functools.partialmethod(run_stim_desktop_theme_script, 'dark')
+    reset_desktop_on_stim = functools.partialmethod(run_stim_desktop_theme_script, 'reset')
         
-    def reset_desktop_on_stim(self) -> None:
-        ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/ben/change_desktop.py'
-        ScriptCamstim.params = {'selection': 'reset'}
-        ScriptCamstim.start()
+
+    def initialize_and_test_services(self) -> None:
+        """Configure, initialize (ie. reset), then test all services."""
         
+        ScriptCamstim.script = '//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/runTask.py'
+        ScriptCamstim.data_root = pathlib.Path('//allen/programs/mindscope/workgroups/dynamicrouting/DynamicRoutingTask/Data') / str(self.mouse)
+
+        MouseDirector.user = self.user.id
+        MouseDirector.mouse = self.mouse.id
+
+        OpenEphys.folder = self.session.folder
+
+        NewScaleCoordinateRecorder.log_root = self.session.npexp_path
+
+        self.configure_services()
+
+        super().initialize_and_test_services()
+
+    def update_state(self) -> None:
+        "Store useful but non-essential info."
+        self.mouse.state['last_session'] = self.session.id
+        self.mouse.state['last_workflow'] = str(self.workflow.name)
+        self.mouse.state['last_task'] = str(self.task_name)
+
     @functools.cached_property
     def system_camstim_params(self) -> dict[str, Any]:
         "System config on Stim computer, if accessible."
         return camstim_defaults()
     
     def copy_data_files(self) -> None:
         """Copy files from raw data storage to session folder for all services
```

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/templeton/templeton_stim_config.py` & `np_workflows-1.5.4/src/np_workflows/experiments/templeton/templeton_stim_config.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/experiments/templeton/templeton_widgets.py` & `np_workflows-1.5.4/src/np_workflows/experiments/templeton/templeton_widgets.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/shared/base_experiments.py` & `np_workflows-1.5.4/src/np_workflows/shared/base_experiments.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim` & `np_workflows-1.5.4/src/np_workflows/shared/camstim_scripts/gabor_20_deg_250ms.stim`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/shared/npxc.py` & `np_workflows-1.5.4/src/np_workflows/shared/npxc.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/src/np_workflows/shared/widgets.py` & `np_workflows-1.5.4/src/np_workflows/shared/widgets.py`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/tests/logs/debug.log` & `np_workflows-1.5.4/tests/logs/debug.log`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/tests/logs/warning.log` & `np_workflows-1.5.4/tests/logs/warning.log`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/tests/widget_sandbox.ipynb` & `np_workflows-1.5.4/tests/widget_sandbox.ipynb`

 * *Files identical despite different names*

### Comparing `np_workflows-1.5.3/PKG-INFO` & `np_workflows-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-workflows
-Version: 1.5.3
+Version: 1.5.4
 Summary: Ecephys and behavior workflows for the Mindscope Neuropixels team.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

