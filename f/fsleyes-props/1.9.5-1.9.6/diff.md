# Comparing `tmp/fsleyes-props-1.9.5.tar.gz` & `tmp/fsleyes-props-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsleyes-props-1.9.5.tar", last modified: Thu Jul  6 15:55:01 2023, max compression
+gzip compressed data, was "fsleyes-props-1.9.6.tar", last modified: Mon Jul 10 16:27:37 2023, max compression
```

## Comparing `fsleyes-props-1.9.5.tar` & `fsleyes-props-1.9.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:55:01.845344 fsleyes-props-1.9.5/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/COPYRIGHT
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4464 2023-07-06 15:55:01.845344 fsleyes-props-1.9.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3721 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:55:01.835344 fsleyes-props-1.9.5/doc/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.bindable.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.build.rst
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.build_parts.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.callqueue.rst
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.cli.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.properties.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.properties_types.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.properties_value.rst
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.serialise.rst
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.suppress.rst
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.syncable.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.trace.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets_boolean.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets_bounds.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets_choice.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets_list.rst
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets_number.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/fsleyes_props.widgets_point.rst
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/doc/mock_modules.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:55:01.840344 fsleyes-props-1.9.5/fsleyes_props/
--rw-rw-rw-   0 root         (0) root         (0)    12129 2023-07-06 15:48:33.000000 fsleyes-props-1.9.5/fsleyes_props/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30475 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/bindable.py
--rw-rw-rw-   0 root         (0) root         (0)    34075 2023-07-06 11:21:24.000000 fsleyes-props-1.9.5/fsleyes_props/build.py
--rw-rw-rw-   0 root         (0) root         (0)    15466 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/build_parts.py
--rw-rw-rw-   0 root         (0) root         (0)     5109 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9936 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/callqueue.py
--rw-rw-rw-   0 root         (0) root         (0)    28752 2023-02-20 16:04:14.000000 fsleyes-props-1.9.5/fsleyes_props/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    40536 2023-03-20 10:37:32.000000 fsleyes-props-1.9.5/fsleyes_props/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    58616 2023-02-21 11:25:17.000000 fsleyes-props-1.9.5/fsleyes_props/properties_types.py
--rw-rw-rw-   0 root         (0) root         (0)    48238 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/properties_value.py
--rw-rw-rw-   0 root         (0) root         (0)     5591 2023-02-20 16:02:09.000000 fsleyes-props-1.9.5/fsleyes_props/serialise.py
--rw-rw-rw-   0 root         (0) root         (0)     3627 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/suppress.py
--rw-rw-rw-   0 root         (0) root         (0)    20161 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/syncable.py
--rw-rw-rw-   0 root         (0) root         (0)     8462 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/trace.py
--rw-rw-rw-   0 root         (0) root         (0)    27887 2023-02-20 16:02:09.000000 fsleyes-props-1.9.5/fsleyes_props/widgets.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-06 15:48:33.000000 fsleyes-props-1.9.5/fsleyes_props/widgets_boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     8027 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/widgets_bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     8619 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/widgets_choice.py
--rw-rw-rw-   0 root         (0) root         (0)     8868 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/widgets_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8934 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/widgets_number.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/fsleyes_props/widgets_point.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:55:01.841344 fsleyes-props-1.9.5/fsleyes_props.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4464 2023-07-06 15:55:01.000000 fsleyes-props-1.9.5/fsleyes_props.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2061 2023-07-06 15:55:01.000000 fsleyes-props-1.9.5/fsleyes_props.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:55:01.000000 fsleyes-props-1.9.5/fsleyes_props.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-06 15:55:01.000000 fsleyes-props-1.9.5/fsleyes_props.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-06 15:55:01.000000 fsleyes-props-1.9.5/fsleyes_props.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-02-20 16:02:09.000000 fsleyes-props-1.9.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-06 15:55:01.846344 fsleyes-props-1.9.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2965 2023-03-15 13:47:40.000000 fsleyes-props-1.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:55:01.845344 fsleyes-props-1.9.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3315 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3890 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5763 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_callqueue.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-03-20 10:51:40.000000 fsleyes-props-1.9.5/tests/test_hasprops.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_importall.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_properties_value.py
--rw-rw-rw-   0 root         (0) root         (0)     7127 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_property_number.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_property_overwritten.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_property_string.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_property_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_suppress.py
--rw-rw-rw-   0 root         (0) root         (0)     7166 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_syncable.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_widget_boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_widget_bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_widget_number.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/test_widget_point.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:55:01.845344 fsleyes-props-1.9.5/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)     1289 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/testdata/false.png
--rw-rw-rw-   0 root         (0) root         (0)     3608 2023-02-07 19:05:55.000000 fsleyes-props-1.9.5/tests/testdata/true.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:27:37.714590 fsleyes-props-1.9.6/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/COPYRIGHT
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4464 2023-07-10 16:27:37.716591 fsleyes-props-1.9.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3721 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:27:37.698590 fsleyes-props-1.9.6/doc/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.bindable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.build.rst
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.build_parts.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.callqueue.rst
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.properties.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.properties_types.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.properties_value.rst
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.serialise.rst
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.suppress.rst
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.syncable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.trace.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets_boolean.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets_bounds.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets_choice.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets_list.rst
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets_number.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/fsleyes_props.widgets_point.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/doc/mock_modules.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:27:37.705590 fsleyes-props-1.9.6/fsleyes_props/
+-rw-rw-rw-   0 root         (0) root         (0)    12129 2023-07-10 16:06:11.000000 fsleyes-props-1.9.6/fsleyes_props/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30475 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/bindable.py
+-rw-rw-rw-   0 root         (0) root         (0)    34075 2023-07-06 11:21:24.000000 fsleyes-props-1.9.6/fsleyes_props/build.py
+-rw-rw-rw-   0 root         (0) root         (0)    15466 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/build_parts.py
+-rw-rw-rw-   0 root         (0) root         (0)     5109 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9936 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/callqueue.py
+-rw-rw-rw-   0 root         (0) root         (0)    28752 2023-02-20 16:04:14.000000 fsleyes-props-1.9.6/fsleyes_props/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    40536 2023-03-20 10:37:32.000000 fsleyes-props-1.9.6/fsleyes_props/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    58093 2023-07-10 16:09:15.000000 fsleyes-props-1.9.6/fsleyes_props/properties_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    48501 2023-07-10 16:06:11.000000 fsleyes-props-1.9.6/fsleyes_props/properties_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     5591 2023-02-20 16:02:09.000000 fsleyes-props-1.9.6/fsleyes_props/serialise.py
+-rw-rw-rw-   0 root         (0) root         (0)     3627 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/suppress.py
+-rw-rw-rw-   0 root         (0) root         (0)    20161 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/syncable.py
+-rw-rw-rw-   0 root         (0) root         (0)     8462 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/trace.py
+-rw-rw-rw-   0 root         (0) root         (0)    27887 2023-02-20 16:02:09.000000 fsleyes-props-1.9.6/fsleyes_props/widgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-06 15:48:33.000000 fsleyes-props-1.9.6/fsleyes_props/widgets_boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     8027 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/widgets_bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     8619 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/widgets_choice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8868 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/widgets_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8934 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/widgets_number.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/fsleyes_props/widgets_point.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:27:37.708590 fsleyes-props-1.9.6/fsleyes_props.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4464 2023-07-10 16:27:37.000000 fsleyes-props-1.9.6/fsleyes_props.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-07-10 16:27:37.000000 fsleyes-props-1.9.6/fsleyes_props.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:27:37.000000 fsleyes-props-1.9.6/fsleyes_props.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-10 16:27:37.000000 fsleyes-props-1.9.6/fsleyes_props.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-10 16:27:37.000000 fsleyes-props-1.9.6/fsleyes_props.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-02-20 16:02:09.000000 fsleyes-props-1.9.6/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-10 16:27:37.716591 fsleyes-props-1.9.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2965 2023-03-15 13:47:40.000000 fsleyes-props-1.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:27:37.714590 fsleyes-props-1.9.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3890 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5763 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_callqueue.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-03-20 10:51:40.000000 fsleyes-props-1.9.6/tests/test_hasprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_importall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_properties_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     7127 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_property_number.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_property_overwritten.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_property_string.py
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-07-10 16:06:11.000000 fsleyes-props-1.9.6/tests/test_property_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_suppress.py
+-rw-rw-rw-   0 root         (0) root         (0)     7166 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_syncable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_widget_boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_widget_bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_widget_number.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/test_widget_point.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:27:37.714590 fsleyes-props-1.9.6/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/testdata/false.png
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2023-02-07 19:05:55.000000 fsleyes-props-1.9.6/tests/testdata/true.png
```

### Comparing `fsleyes-props-1.9.5/LICENSE` & `fsleyes-props-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/PKG-INFO` & `fsleyes-props-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsleyes-props
-Version: 1.9.5
+Version: 1.9.6
 Summary: [wx]Python event programming framework
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsleyes/props
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `fsleyes-props-1.9.5/README.rst` & `fsleyes-props-1.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/doc/conf.py` & `fsleyes-props-1.9.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/doc/fsleyes_props.rst` & `fsleyes-props-1.9.6/doc/fsleyes_props.rst`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/doc/index.rst` & `fsleyes-props-1.9.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/__init__.py` & `fsleyes-props-1.9.6/fsleyes_props/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 ^^^^^^^^^^^^^
 
 The :func:`.suppress` module provides some context managers allowing
 notification of properties to be suppressed in a ``with`` statement.
 """
 
 
-__version__ = '1.9.5'
+__version__ = '1.9.6'
 
 
 import sys
 import logging
 
 
 log = logging.getLogger(__name__)
```

### Comparing `fsleyes-props-1.9.5/fsleyes_props/bindable.py` & `fsleyes-props-1.9.6/fsleyes_props/bindable.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/build.py` & `fsleyes-props-1.9.6/fsleyes_props/build.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/build_parts.py` & `fsleyes-props-1.9.6/fsleyes_props/build_parts.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/cache.py` & `fsleyes-props-1.9.6/fsleyes_props/cache.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/callqueue.py` & `fsleyes-props-1.9.6/fsleyes_props/callqueue.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/cli.py` & `fsleyes-props-1.9.6/fsleyes_props/cli.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/properties.py` & `fsleyes-props-1.9.6/fsleyes_props/properties.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/properties_types.py` & `fsleyes-props-1.9.6/fsleyes_props/properties_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1615,22 +1615,14 @@
     """A property which represents a ``numpy`` array. Each array is
     encapsulated within an :class:`ArrayProxy` instance.
     """
 
     def __init__(self, dtype=None, shape=None, resizable=True, **kwargs):
         """Create an ``Array`` property.
 
-        .. warning:: If you set a ``default`` value here (see
-                     :meth:`.PropertyBase.__init__`), *do not* use a ``numpy``
-                     array - use a regular python list. It will be converted
-                     in a ``numpy`` array internally. An equality test is made
-                     on the ``default`` attribute, so if you use a ``numpy``
-                     array, a :exc:`ValueError` will be raised, as ``numpy``
-                     performs equality tests on an element-wise basis.
-
         :arg dtype:     ``numpy`` data type.
 
         :arg shape:     Initial shape of the array.
 
         :arg resizable: Defaults to ``True``. If ``False``, the array size
                         will be fixed to the ``shape`` specified
                         here. Different sized arrays will still be allowed, if
```

### Comparing `fsleyes-props-1.9.5/fsleyes_props/properties_value.py` & `fsleyes-props-1.9.6/fsleyes_props/properties_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,15 +493,23 @@
         """Sets the named attribute to the given value, and notifies any
         registered attribute listeners of the change.
         """
         oldVal = self._attributes.get(name, None)
 
         self._attributes[name] = value
 
-        if oldVal == value: return
+        # Use the type-specific equalty function
+        # for the "default" attribute (see
+        # PropertyBase.__init__).
+        if name == 'default':
+            if self._equalityFunc(oldVal, value):
+                return
+        else:
+            if oldVal == value:
+                return
 
         log.debug('Attribute on %s.%s (%s) changed: %s = %s',
             self._context().__class__.__name__,
             self._name,
             id(self),
             name,
             value)
```

### Comparing `fsleyes-props-1.9.5/fsleyes_props/serialise.py` & `fsleyes-props-1.9.6/fsleyes_props/serialise.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/suppress.py` & `fsleyes-props-1.9.6/fsleyes_props/suppress.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/syncable.py` & `fsleyes-props-1.9.6/fsleyes_props/syncable.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/trace.py` & `fsleyes-props-1.9.6/fsleyes_props/trace.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets_boolean.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets_boolean.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets_bounds.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets_bounds.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets_choice.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets_choice.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets_list.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets_list.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets_number.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets_number.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props/widgets_point.py` & `fsleyes-props-1.9.6/fsleyes_props/widgets_point.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/fsleyes_props.egg-info/PKG-INFO` & `fsleyes-props-1.9.6/fsleyes_props.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsleyes-props
-Version: 1.9.5
+Version: 1.9.6
 Summary: [wx]Python event programming framework
 Home-page: https://git.fmrib.ox.ac.uk/fsl/fsleyes/props
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `fsleyes-props-1.9.5/fsleyes_props.egg-info/SOURCES.txt` & `fsleyes-props-1.9.6/fsleyes_props.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/setup.py` & `fsleyes-props-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/__init__.py` & `fsleyes-props-1.9.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_cache.py` & `fsleyes-props-1.9.6/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_callqueue.py` & `fsleyes-props-1.9.6/tests/test_callqueue.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_importall.py` & `fsleyes-props-1.9.6/tests/test_importall.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_properties_value.py` & `fsleyes-props-1.9.6/tests/test_properties_value.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_property_number.py` & `fsleyes-props-1.9.6/tests/test_property_number.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_suppress.py` & `fsleyes-props-1.9.6/tests/test_suppress.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_syncable.py` & `fsleyes-props-1.9.6/tests/test_syncable.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_widget_boolean.py` & `fsleyes-props-1.9.6/tests/test_widget_boolean.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_widget_bounds.py` & `fsleyes-props-1.9.6/tests/test_widget_bounds.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_widget_number.py` & `fsleyes-props-1.9.6/tests/test_widget_number.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/test_widget_point.py` & `fsleyes-props-1.9.6/tests/test_widget_point.py`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/testdata/false.png` & `fsleyes-props-1.9.6/tests/testdata/false.png`

 * *Files identical despite different names*

### Comparing `fsleyes-props-1.9.5/tests/testdata/true.png` & `fsleyes-props-1.9.6/tests/testdata/true.png`

 * *Files identical despite different names*

