# Comparing `tmp/pyobs_gui-1.0.7.tar.gz` & `tmp/pyobs_gui-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_gui-1.0.7.tar", max compression
+gzip compressed data, was "pyobs_gui-1.0.8.tar", max compression
```

## Comparing `pyobs_gui-1.0.7.tar` & `pyobs_gui-1.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1099 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/LICENSE
--rw-r--r--   0        0        0      423 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/__init__.py
--rw-r--r--   0        0        0    10966 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/base.py
--rw-r--r--   0        0        0    14024 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/camerawidget.py
--rw-r--r--   0        0        0     1678 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/commandinputwidget.py
--rw-r--r--   0        0        0     2984 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/compassmovewidget.py
--rw-r--r--   0        0        0     2218 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/coolingwidget.py
--rw-r--r--   0        0        0     8641 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/datadisplaywidget.py
--rw-r--r--   0        0        0     6650 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/eventswidget.py
--rw-r--r--   0        0        0     4405 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/filterwidget.py
--rw-r--r--   0        0        0     2429 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/fitsheaderswidget.py
--rw-r--r--   0        0        0     5385 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/focuswidget.py
--rw-r--r--   0        0        0     2763 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/gui.py
--rw-r--r--   0        0        0     2945 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/logmodel.py
--rw-r--r--   0        0        0    15631 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/mainwindow.py
--rw-r--r--   0        0        0     3079 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/modulegui.py
--rw-r--r--   0        0        0        0 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/__init__.py
--rw-r--r--   0        0        0    42397 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/camerawidget.ui
--rw-r--r--   0        0        0    31606 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/camerawidget_ui.py
--rw-r--r--   0        0        0      928 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/compassmoveplugin.py
--rw-r--r--   0        0        0      227 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/compassmovewidget.py
--rw-r--r--   0        0        0     2553 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/compassmovewidget.ui
--rw-r--r--   0        0        0     3229 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/compassmovewidget_ui.py
--rwxr-xr-x   0        0        0      256 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/compile.sh
--rw-r--r--   0        0        0     3547 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/coolingwidget.ui
--rw-r--r--   0        0        0     3925 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/coolingwidget_ui.py
--rw-r--r--   0        0        0      928 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/datadisplayplugin.py
--rw-r--r--   0        0        0      227 2023-07-14 08:12:18.914812 pyobs_gui-1.0.7/pyobs_gui/qt/datadisplaywidget.py
--rw-r--r--   0        0        0     4129 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/datadisplaywidget.ui
--rw-r--r--   0        0        0     4705 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/datadisplaywidget_ui.py
--rwxr-xr-x   0        0        0       43 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/designer.sh
--rw-r--r--   0        0        0     2509 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/eventswidget.ui
--rw-r--r--   0        0        0     2639 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/eventswidget_ui.py
--rw-r--r--   0        0        0     2305 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/filterwidget.ui
--rw-r--r--   0        0        0     2983 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/filterwidget_ui.py
--rw-r--r--   0        0        0     3165 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/fitsheaderswidget.ui
--rw-r--r--   0        0        0     4440 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/fitsheaderswidget_ui.py
--rw-r--r--   0        0        0     5796 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/focuswidget.ui
--rw-r--r--   0        0        0     7130 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/focuswidget_ui.py
--rw-r--r--   0        0        0    10262 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/mainwindow.py
--rw-r--r--   0        0        0    12065 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/mainwindow.ui
--rw-r--r--   0        0        0      502 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrow-alt-circle-down-solid.svg
--rw-r--r--   0        0        0      503 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrow-alt-circle-left-solid.svg
--rw-r--r--   0        0        0      499 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrow-alt-circle-right-solid.svg
--rw-r--r--   0        0        0      493 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrow-alt-circle-up-solid.svg
--rw-r--r--   0        0        0      892 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg
--rw-r--r--   0        0        0     1640 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrows-to-eye-solid.svg
--rw-r--r--   0        0        0      720 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/chart-line-solid.svg
--rw-r--r--   0        0        0      681 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/circle-question-solid.svg
--rw-r--r--   0        0        0     1283 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/cloud-sun-solid.svg
--rw-r--r--   0        0        0      735 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/edit-solid.svg
--rw-r--r--   0        0        0      577 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/search-solid.svg
--rw-r--r--   0        0        0      767 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources/undo-solid.svg
--rw-r--r--   0        0        0      528 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources.qrc
--rw-r--r--   0        0        0    28297 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/resources_rc.py
--rw-r--r--   0        0        0    45953 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/roofwidget.ui
--rw-r--r--   0        0        0    30193 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/roofwidget_ui.py
--rw-r--r--   0        0        0      915 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/shellwidget.ui
--rw-r--r--   0        0        0     1326 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/shellwidget_ui.py
--rw-r--r--   0        0        0    34768 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/spectrographwidget.ui
--rw-r--r--   0        0        0    23247 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/spectrographwidget_ui.py
--rw-r--r--   0        0        0    60514 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/telescopewidget.ui
--rw-r--r--   0        0        0    55903 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/telescopewidget_ui.py
--rw-r--r--   0        0        0     1917 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/temperaturesplotwidget.ui
--rw-r--r--   0        0        0     2769 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/temperaturesplotwidget_ui.py
--rw-r--r--   0        0        0     2114 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/temperatureswidget.ui
--rw-r--r--   0        0        0     2612 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/temperatureswidget_ui.py
--rw-r--r--   0        0        0    40308 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/videowidget.ui
--rw-r--r--   0        0        0    25634 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/videowidget_ui.py
--rw-r--r--   0        0        0     1511 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/weatherwidget.ui
--rw-r--r--   0        0        0     2290 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/qt/weatherwidget_ui.py
--rw-r--r--   0        0        0     2075 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/roofwidget.py
--rw-r--r--   0        0        0    12375 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/shellwidget.py
--rw-r--r--   0        0        0     5392 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/spectrographwidget.py
--rw-r--r--   0        0        0     6608 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/statuswidget.py
--rw-r--r--   0        0        0    27475 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/telescopewidget.py
--rw-r--r--   0        0        0     3350 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/temperaturesplotwidget.py
--rw-r--r--   0        0        0     2577 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/temperatureswidget.py
--rw-r--r--   0        0        0     2255 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/utils.py
--rw-r--r--   0        0        0     8080 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/videowidget.py
--rwxr-xr-x   0        0        0     2419 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/visplot.py
--rw-r--r--   0        0        0     5531 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyobs_gui/weatherwidget.py
--rw-r--r--   0        0        0      681 2023-07-14 08:12:18.918813 pyobs_gui-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 pyobs_gui-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-18 10:31:23.456202 pyobs_gui-1.0.8/LICENSE
+-rw-r--r--   0        0        0      423 2023-07-18 10:31:23.456202 pyobs_gui-1.0.8/pyobs_gui/__init__.py
+-rw-r--r--   0        0        0    10966 2023-07-18 10:31:23.456202 pyobs_gui-1.0.8/pyobs_gui/base.py
+-rw-r--r--   0        0        0    14024 2023-07-18 10:31:23.456202 pyobs_gui-1.0.8/pyobs_gui/camerawidget.py
+-rw-r--r--   0        0        0     1678 2023-07-18 10:31:23.456202 pyobs_gui-1.0.8/pyobs_gui/commandinputwidget.py
+-rw-r--r--   0        0        0     2984 2023-07-18 10:31:23.456202 pyobs_gui-1.0.8/pyobs_gui/compassmovewidget.py
+-rw-r--r--   0        0        0     2218 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/coolingwidget.py
+-rw-r--r--   0        0        0     8641 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/datadisplaywidget.py
+-rw-r--r--   0        0        0     6650 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/eventswidget.py
+-rw-r--r--   0        0        0     4405 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/filterwidget.py
+-rw-r--r--   0        0        0     2429 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/fitsheaderswidget.py
+-rw-r--r--   0        0        0     5385 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/focuswidget.py
+-rw-r--r--   0        0        0     2763 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/gui.py
+-rw-r--r--   0        0        0     2945 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/logmodel.py
+-rw-r--r--   0        0        0    15631 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/mainwindow.py
+-rw-r--r--   0        0        0     3079 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/modulegui.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/__init__.py
+-rw-r--r--   0        0        0    42397 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/camerawidget.ui
+-rw-r--r--   0        0        0    31606 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/camerawidget_ui.py
+-rw-r--r--   0        0        0      928 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/compassmoveplugin.py
+-rw-r--r--   0        0        0      227 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/compassmovewidget.py
+-rw-r--r--   0        0        0     2553 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/compassmovewidget.ui
+-rw-r--r--   0        0        0     3229 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/compassmovewidget_ui.py
+-rwxr-xr-x   0        0        0      256 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/compile.sh
+-rw-r--r--   0        0        0     3547 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/coolingwidget.ui
+-rw-r--r--   0        0        0     3925 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/coolingwidget_ui.py
+-rw-r--r--   0        0        0      928 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/datadisplayplugin.py
+-rw-r--r--   0        0        0      227 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/datadisplaywidget.py
+-rw-r--r--   0        0        0     4129 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/datadisplaywidget.ui
+-rw-r--r--   0        0        0     4705 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/datadisplaywidget_ui.py
+-rwxr-xr-x   0        0        0       43 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/designer.sh
+-rw-r--r--   0        0        0     2509 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/eventswidget.ui
+-rw-r--r--   0        0        0     2639 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/eventswidget_ui.py
+-rw-r--r--   0        0        0     2305 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/filterwidget.ui
+-rw-r--r--   0        0        0     2983 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/filterwidget_ui.py
+-rw-r--r--   0        0        0     3165 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/fitsheaderswidget.ui
+-rw-r--r--   0        0        0     4440 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/fitsheaderswidget_ui.py
+-rw-r--r--   0        0        0     5796 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/focuswidget.ui
+-rw-r--r--   0        0        0     7130 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/focuswidget_ui.py
+-rw-r--r--   0        0        0    10262 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/mainwindow.py
+-rw-r--r--   0        0        0    12065 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/mainwindow.ui
+-rw-r--r--   0        0        0      502 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrow-alt-circle-down-solid.svg
+-rw-r--r--   0        0        0      503 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrow-alt-circle-left-solid.svg
+-rw-r--r--   0        0        0      499 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrow-alt-circle-right-solid.svg
+-rw-r--r--   0        0        0      493 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrow-alt-circle-up-solid.svg
+-rw-r--r--   0        0        0      892 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg
+-rw-r--r--   0        0        0     1640 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrows-to-eye-solid.svg
+-rw-r--r--   0        0        0      720 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/chart-line-solid.svg
+-rw-r--r--   0        0        0      681 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/circle-question-solid.svg
+-rw-r--r--   0        0        0     1283 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/cloud-sun-solid.svg
+-rw-r--r--   0        0        0      735 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/edit-solid.svg
+-rw-r--r--   0        0        0      577 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/search-solid.svg
+-rw-r--r--   0        0        0      767 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources/undo-solid.svg
+-rw-r--r--   0        0        0      528 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources.qrc
+-rw-r--r--   0        0        0    28297 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/resources_rc.py
+-rw-r--r--   0        0        0    45953 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/roofwidget.ui
+-rw-r--r--   0        0        0    30193 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/roofwidget_ui.py
+-rw-r--r--   0        0        0      915 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/shellwidget.ui
+-rw-r--r--   0        0        0     1326 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/shellwidget_ui.py
+-rw-r--r--   0        0        0    34768 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/spectrographwidget.ui
+-rw-r--r--   0        0        0    23247 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/spectrographwidget_ui.py
+-rw-r--r--   0        0        0    60514 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/telescopewidget.ui
+-rw-r--r--   0        0        0    55903 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/telescopewidget_ui.py
+-rw-r--r--   0        0        0     1917 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/temperaturesplotwidget.ui
+-rw-r--r--   0        0        0     2769 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/temperaturesplotwidget_ui.py
+-rw-r--r--   0        0        0     2114 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/temperatureswidget.ui
+-rw-r--r--   0        0        0     2612 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/temperatureswidget_ui.py
+-rw-r--r--   0        0        0    40308 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/videowidget.ui
+-rw-r--r--   0        0        0    25634 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/videowidget_ui.py
+-rw-r--r--   0        0        0     1511 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/weatherwidget.ui
+-rw-r--r--   0        0        0     2290 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/qt/weatherwidget_ui.py
+-rw-r--r--   0        0        0     2075 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/roofwidget.py
+-rw-r--r--   0        0        0    12375 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/shellwidget.py
+-rw-r--r--   0        0        0     5392 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/spectrographwidget.py
+-rw-r--r--   0        0        0     6608 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/statuswidget.py
+-rw-r--r--   0        0        0    27473 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/telescopewidget.py
+-rw-r--r--   0        0        0     3350 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/temperaturesplotwidget.py
+-rw-r--r--   0        0        0     2577 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/temperatureswidget.py
+-rw-r--r--   0        0        0     2255 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/utils.py
+-rw-r--r--   0        0        0     8080 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/videowidget.py
+-rwxr-xr-x   0        0        0     2419 2023-07-18 10:31:23.460202 pyobs_gui-1.0.8/pyobs_gui/visplot.py
+-rw-r--r--   0        0        0     5531 2023-07-18 10:31:23.464203 pyobs_gui-1.0.8/pyobs_gui/weatherwidget.py
+-rw-r--r--   0        0        0      681 2023-07-18 10:31:23.464203 pyobs_gui-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 pyobs_gui-1.0.8/PKG-INFO
```

### Comparing `pyobs_gui-1.0.7/LICENSE` & `pyobs_gui-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/base.py` & `pyobs_gui-1.0.8/pyobs_gui/base.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/camerawidget.py` & `pyobs_gui-1.0.8/pyobs_gui/camerawidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/commandinputwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/commandinputwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/compassmovewidget.py` & `pyobs_gui-1.0.8/pyobs_gui/compassmovewidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/coolingwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/coolingwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/datadisplaywidget.py` & `pyobs_gui-1.0.8/pyobs_gui/datadisplaywidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/eventswidget.py` & `pyobs_gui-1.0.8/pyobs_gui/eventswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/filterwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/filterwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/fitsheaderswidget.py` & `pyobs_gui-1.0.8/pyobs_gui/fitsheaderswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/focuswidget.py` & `pyobs_gui-1.0.8/pyobs_gui/focuswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/gui.py` & `pyobs_gui-1.0.8/pyobs_gui/gui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/logmodel.py` & `pyobs_gui-1.0.8/pyobs_gui/logmodel.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/mainwindow.py` & `pyobs_gui-1.0.8/pyobs_gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/modulegui.py` & `pyobs_gui-1.0.8/pyobs_gui/modulegui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/camerawidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/camerawidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/camerawidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/camerawidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/compassmoveplugin.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/compassmoveplugin.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/compassmovewidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/compassmovewidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/compassmovewidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/compassmovewidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/coolingwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/coolingwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/coolingwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/coolingwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/datadisplayplugin.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/datadisplayplugin.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/datadisplaywidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/datadisplaywidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/datadisplaywidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/datadisplaywidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/eventswidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/eventswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/eventswidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/eventswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/filterwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/filterwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/filterwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/filterwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/fitsheaderswidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/fitsheaderswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/fitsheaderswidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/fitsheaderswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/focuswidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/focuswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/focuswidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/focuswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/mainwindow.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/mainwindow.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/mainwindow.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrow-up-right-from-square-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/arrows-to-eye-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/arrows-to-eye-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/chart-line-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/chart-line-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/circle-question-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/circle-question-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/cloud-sun-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/cloud-sun-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/edit-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/edit-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/search-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/search-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources/undo-solid.svg` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources/undo-solid.svg`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources.qrc` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources.qrc`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/resources_rc.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/resources_rc.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/roofwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/roofwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/roofwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/roofwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/shellwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/shellwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/shellwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/shellwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/spectrographwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/spectrographwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/spectrographwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/spectrographwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/telescopewidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/telescopewidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/telescopewidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/telescopewidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/temperaturesplotwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/temperaturesplotwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/temperaturesplotwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/temperaturesplotwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/temperatureswidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/temperatureswidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/temperatureswidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/temperatureswidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/videowidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/videowidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/videowidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/videowidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/weatherwidget.ui` & `pyobs_gui-1.0.8/pyobs_gui/qt/weatherwidget.ui`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/qt/weatherwidget_ui.py` & `pyobs_gui-1.0.8/pyobs_gui/qt/weatherwidget_ui.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/roofwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/roofwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/shellwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/shellwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/spectrographwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/spectrographwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/statuswidget.py` & `pyobs_gui-1.0.8/pyobs_gui/statuswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/telescopewidget.py` & `pyobs_gui-1.0.8/pyobs_gui/telescopewidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
             tx = -theta * np.sin(psi)
             ty = theta * np.cos(psi)
             heliproj = SkyCoord(tx, ty, obstime=Time.now(), frame=Helioprojective, observer="earth")
 
             # move
             if isinstance(self.module, IPointingHelioprojective):
                 # run it
-                self.run_background(self.module.move_helioprojective, heliproj.Tx.degrees, heliproj.Ty.degrees)
+                self.run_background(self.module.move_helioprojective, heliproj.Tx.degree, heliproj.Ty.degree)
 
             elif isinstance(self.module, IPointingHGS):
                 # alternatively, convert helio projective coordinates to Heliographic Stonyhurst
                 stony = heliproj.transform_to(HeliographicStonyhurst)
                 lon, lat = float(stony.lon.to(u.degree).value), float(stony.lat.to(u.degree).value)
 
                 # run it
```

### Comparing `pyobs_gui-1.0.7/pyobs_gui/temperaturesplotwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/temperaturesplotwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/temperatureswidget.py` & `pyobs_gui-1.0.8/pyobs_gui/temperatureswidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/utils.py` & `pyobs_gui-1.0.8/pyobs_gui/utils.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/videowidget.py` & `pyobs_gui-1.0.8/pyobs_gui/videowidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/visplot.py` & `pyobs_gui-1.0.8/pyobs_gui/visplot.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyobs_gui/weatherwidget.py` & `pyobs_gui-1.0.8/pyobs_gui/weatherwidget.py`

 * *Files identical despite different names*

### Comparing `pyobs_gui-1.0.7/pyproject.toml` & `pyobs_gui-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-gui"
-version = "1.0.7"
+version = "1.0.8"
 description = "A remote GUI for pyobs"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 colour = "^0.1.5"
```

### Comparing `pyobs_gui-1.0.7/PKG-INFO` & `pyobs_gui-1.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-gui
-Version: 1.0.7
+Version: 1.0.8
 Summary: A remote GUI for pyobs
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

