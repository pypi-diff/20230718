# Comparing `tmp/fastavro-1.8.0.tar.gz` & `tmp/fastavro-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastavro-1.8.0.tar", last modified: Thu Jul  6 15:53:50 2023, max compression
+gzip compressed data, was "fastavro-1.8.1.tar", last modified: Mon Jul 17 22:03:36 2023, max compression
```

## Comparing `fastavro-1.8.0.tar` & `fastavro-1.8.1.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.594318 fastavro-1.8.0/
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1625 2019-05-08 02:19:05.000000 fastavro-1.8.0/.azure_upload.sh
--rw-r--r--   0 sbelden    (501) staff       (20)       55 2020-12-23 03:10:46.000000 fastavro-1.8.0/.flake8.cython
--rw-r--r--   0 sbelden    (501) staff       (20)    26345 2023-07-06 15:00:48.000000 fastavro-1.8.0/ChangeLog
--rw-r--r--   0 sbelden    (501) staff       (20)      333 2022-10-26 14:14:35.000000 fastavro-1.8.0/Dockerfile
--rw-r--r--   0 sbelden    (501) staff       (20)     1068 2019-05-04 22:05:46.000000 fastavro-1.8.0/LICENSE
--rw-r--r--   0 sbelden    (501) staff       (20)      559 2022-08-11 13:05:27.000000 fastavro-1.8.0/MANIFEST.in
--rw-r--r--   0 sbelden    (501) staff       (20)      812 2022-08-11 13:05:27.000000 fastavro-1.8.0/Makefile
--rw-r--r--   0 sbelden    (501) staff       (20)      563 2019-05-04 22:05:46.000000 fastavro-1.8.0/NOTICE.txt
--rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-07-06 15:53:50.594465 fastavro-1.8.0/PKG-INFO
--rw-r--r--   0 sbelden    (501) staff       (20)     3870 2022-10-26 14:14:35.000000 fastavro-1.8.0/README.md
--rw-r--r--   0 sbelden    (501) staff       (20)      520 2023-05-04 13:14:43.000000 fastavro-1.8.0/developer_requirements.txt
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.494680 fastavro-1.8.0/docs/
--rw-r--r--   0 sbelden    (501) staff       (20)     5578 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/Makefile
--rw-r--r--   0 sbelden    (501) staff       (20)     1456 2019-05-04 22:05:46.000000 fastavro-1.8.0/docs/command_line_script.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     8320 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/conf.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2502 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/index.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.495976 fastavro-1.8.0/docs/io/
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/io/index.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/io/json_decoder.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/io/json_encoder.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       88 2020-02-26 16:33:59.000000 fastavro-1.8.0/docs/json_reader.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       91 2020-02-26 16:33:59.000000 fastavro-1.8.0/docs/json_writer.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     4869 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/logical_types.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      256 2021-03-20 12:25:05.000000 fastavro-1.8.0/docs/reader.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.496914 fastavro-1.8.0/docs/repository/
--rw-r--r--   0 sbelden    (501) staff       (20)      116 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/repository/base.rst
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/repository/index.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      405 2021-02-06 15:15:34.000000 fastavro-1.8.0/docs/schema.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      174 2021-03-13 13:43:47.000000 fastavro-1.8.0/docs/utils.rst
--rw-r--r--   0 sbelden    (501) staff       (20)      149 2019-05-04 22:05:46.000000 fastavro-1.8.0/docs/validation.rst
--rw-r--r--   0 sbelden    (501) staff       (20)     3996 2022-08-11 13:05:27.000000 fastavro-1.8.0/docs/writer.rst
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.531576 fastavro-1.8.0/fastavro/
--rw-r--r--   0 sbelden    (501) staff       (20)     1750 2023-07-06 14:59:31.000000 fastavro-1.8.0/fastavro/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2423 2020-12-23 03:10:46.000000 fastavro-1.8.0/fastavro/__main__.py
--rw-r--r--   0 sbelden    (501) staff       (20)   262056 2023-07-06 15:53:45.000000 fastavro-1.8.0/fastavro/_logical_readers.c
--rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     2792 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     2813 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_logical_readers_py.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)   430913 2023-07-06 15:53:46.000000 fastavro-1.8.0/fastavro/_logical_writers.c
--rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.8.0/fastavro/_logical_writers.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     8427 2022-10-06 12:45:33.000000 fastavro-1.8.0/fastavro/_logical_writers.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     7830 2022-10-06 12:45:33.000000 fastavro-1.8.0/fastavro/_logical_writers_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.8.0/fastavro/_logical_writers_py.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)  1104218 2023-07-06 15:53:46.000000 fastavro-1.8.0/fastavro/_read.c
--rw-r--r--   0 sbelden    (501) staff       (20)     2070 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/_read.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    34172 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/_read.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)      703 2023-04-17 20:07:08.000000 fastavro-1.8.0/fastavro/_read_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    34680 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/_read_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)   704359 2023-07-06 15:53:47.000000 fastavro-1.8.0/fastavro/_schema.c
--rw-r--r--   0 sbelden    (501) staff       (20)      950 2023-02-22 18:29:22.000000 fastavro-1.8.0/fastavro/_schema.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    24103 2023-05-04 14:35:44.000000 fastavro-1.8.0/fastavro/_schema.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)     1421 2021-01-23 16:11:54.000000 fastavro-1.8.0/fastavro/_schema_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    33011 2023-05-04 14:35:44.000000 fastavro-1.8.0/fastavro/_schema_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)   441134 2020-08-18 18:15:09.000000 fastavro-1.8.0/fastavro/_six.c
--rw-r--r--   0 sbelden    (501) staff       (20)      633 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/_validate_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)   390961 2023-07-06 15:53:47.000000 fastavro-1.8.0/fastavro/_validation.c
--rw-r--r--   0 sbelden    (501) staff       (20)      338 2022-08-12 17:49:36.000000 fastavro-1.8.0/fastavro/_validation.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)     9403 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/_validation.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)    10757 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/_validation_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)  1717084 2023-07-06 15:53:49.000000 fastavro-1.8.0/fastavro/_write.c
--rw-r--r--   0 sbelden    (501) staff       (20)     1680 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/_write.pyi
--rw-r--r--   0 sbelden    (501) staff       (20)    26702 2023-04-17 20:07:08.000000 fastavro-1.8.0/fastavro/_write.pyx
--rw-r--r--   0 sbelden    (501) staff       (20)      619 2023-05-03 19:57:13.000000 fastavro-1.8.0/fastavro/_write_common.py
--rw-r--r--   0 sbelden    (501) staff       (20)    26758 2023-04-17 20:07:08.000000 fastavro-1.8.0/fastavro/_write_py.py
--rw-r--r--   0 sbelden    (501) staff       (20)      853 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/const.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.536520 fastavro-1.8.0/fastavro/io/
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-02-26 16:33:59.000000 fastavro-1.8.0/fastavro/io/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4379 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/io/binary_decoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1861 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/io/binary_encoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     6936 2023-07-06 14:53:47.000000 fastavro-1.8.0/fastavro/io/json_decoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     5674 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/io/json_encoder.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4980 2022-02-25 13:49:52.000000 fastavro-1.8.0/fastavro/io/parser.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2321 2021-01-22 04:19:07.000000 fastavro-1.8.0/fastavro/io/symbols.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1603 2023-03-16 19:48:58.000000 fastavro-1.8.0/fastavro/json_read.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2908 2022-08-15 15:33:27.000000 fastavro-1.8.0/fastavro/json_write.py
--rw-r--r--   0 sbelden    (501) staff       (20)      217 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/logical_readers.py
--rw-r--r--   0 sbelden    (501) staff       (20)      217 2020-12-23 03:10:46.000000 fastavro-1.8.0/fastavro/logical_writers.py
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-06-22 15:51:13.000000 fastavro-1.8.0/fastavro/py.typed
--rw-r--r--   0 sbelden    (501) staff       (20)      775 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/read.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.538089 fastavro-1.8.0/fastavro/repository/
--rw-r--r--   0 sbelden    (501) staff       (20)      210 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/repository/__init__.py
--rw-r--r--   0 sbelden    (501) staff       (20)      185 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/repository/base.py
--rw-r--r--   0 sbelden    (501) staff       (20)      764 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/repository/flat_dict.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1030 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/schema.py
--rw-r--r--   0 sbelden    (501) staff       (20)      419 2022-08-11 13:05:27.000000 fastavro-1.8.0/fastavro/types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     7456 2023-02-01 14:56:04.000000 fastavro-1.8.0/fastavro/utils.py
--rw-r--r--   0 sbelden    (501) staff       (20)      422 2020-12-23 03:10:46.000000 fastavro-1.8.0/fastavro/validation.py
--rw-r--r--   0 sbelden    (501) staff       (20)      457 2021-02-27 20:10:59.000000 fastavro-1.8.0/fastavro/write.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.534059 fastavro-1.8.0/fastavro.egg-info/
--rw-r--r--   0 sbelden    (501) staff       (20)     5250 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/PKG-INFO
--rw-r--r--   0 sbelden    (501) staff       (20)     6017 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/SOURCES.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/dependency_links.txt
--rw-r--r--   0 sbelden    (501) staff       (20)       52 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/entry_points.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-07-05 18:01:12.000000 fastavro-1.8.0/fastavro.egg-info/not-zip-safe
--rw-r--r--   0 sbelden    (501) staff       (20)       96 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/requires.txt
--rw-r--r--   0 sbelden    (501) staff       (20)        9 2023-07-06 15:53:50.000000 fastavro-1.8.0/fastavro.egg-info/top_level.txt
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2023-04-17 20:07:08.000000 fastavro-1.8.0/mypy.ini
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1439 2023-07-06 15:52:36.000000 fastavro-1.8.0/publish.sh
--rw-r--r--   0 sbelden    (501) staff       (20)      204 2023-03-08 20:55:48.000000 fastavro-1.8.0/pyproject.toml
--rwxr-xr-x   0 sbelden    (501) staff       (20)       31 2019-05-04 22:05:46.000000 fastavro-1.8.0/pytest.ini
--rw-r--r--   0 sbelden    (501) staff       (20)      710 2022-09-20 17:48:57.000000 fastavro-1.8.0/run-tests.cmd
--rwxr-xr-x   0 sbelden    (501) staff       (20)     1054 2023-07-05 17:54:02.000000 fastavro-1.8.0/run-tests.sh
--rw-r--r--   0 sbelden    (501) staff       (20)      105 2023-07-06 15:53:50.594914 fastavro-1.8.0/setup.cfg
--rw-r--r--   0 sbelden    (501) staff       (20)     2796 2022-10-26 14:14:35.000000 fastavro-1.8.0/setup.py
--rwxr-xr-x   0 sbelden    (501) staff       (20)      169 2023-03-08 22:33:06.000000 fastavro-1.8.0/tag.sh
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.552393 fastavro-1.8.0/tests/
--rw-r--r--   0 sbelden    (501) staff       (20)        0 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/__init__.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.571904 fastavro-1.8.0/tests/avro-files/
--rw-r--r--   0 sbelden    (501) staff       (20)       55 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/Child.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/Child1.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      179 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/Parent.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      130 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/ParentMissingChild.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      447 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/a_triple_pair.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       79 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/bool.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.seperators.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.deflate.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       84 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.plain.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.zerojsonvalues.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3293 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/deflate.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      276 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/double_float.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      234 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/error-type.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     8453 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/java-generated-uuid.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      299 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/lines.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      403 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/m.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      139 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/no-fields.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3285 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/null.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       68 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/org.apache.avro.tool.TestDataFileTools.avro
--rwxr-xr-x   0 sbelden    (501) staff       (20)      321 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/part-00000.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      218 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/recursive.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      162 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/request.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/response.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     3296 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/snappy.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12556 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-0.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-1-A.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-1.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-3-A.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     6112 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-6-B.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-deflate-9.avro
--rw-r--r--   0 sbelden    (501) staff       (20)     6522 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-null-B.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    13289 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-null.avro
--rw-r--r--   0 sbelden    (501) staff       (20)    13677 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test-snappy.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      182 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/test.avro
--rw-r--r--   0 sbelden    (501) staff       (20)       51 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/testDataFileMeta.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      690 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/avro-files/weather-legacy-generated.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      696 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/avro-files/weather-legacy-with-names.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      330 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/weather-snappy.avro
--rwxr-xr-x   0 sbelden    (501) staff       (20)      335 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/weather-sorted.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      358 2019-05-04 22:05:46.000000 fastavro-1.8.0/tests/avro-files/weather.avro
--rw-r--r--   0 sbelden    (501) staff       (20)      999 2021-03-13 13:43:47.000000 fastavro-1.8.0/tests/conftest.py
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.574424 fastavro-1.8.0/tests/load_schema_test/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test/D.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.576920 fastavro-1.8.0/tests/load_schema_test_10/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_10/D.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.578842 fastavro-1.8.0/tests/load_schema_test_11/
--rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       99 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/C.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/D.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_11/E.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.579216 fastavro-1.8.0/tests/load_schema_test_12/
--rw-r--r--   0 sbelden    (501) staff       (20)      143 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/A.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.579969 fastavro-1.8.0/tests/load_schema_test_12/com/
--rw-r--r--   0 sbelden    (501) staff       (20)      137 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      187 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.580693 fastavro-1.8.0/tests/load_schema_test_12/com/namespace/
--rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/namespace/D.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_12/com/namespace/E.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.581558 fastavro-1.8.0/tests/load_schema_test_13/
--rw-r--r--   0 sbelden    (501) staff       (20)        3 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_13/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_13/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.582021 fastavro-1.8.0/tests/load_schema_test_14/
--rw-r--r--   0 sbelden    (501) staff       (20)        8 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_14/A.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.582946 fastavro-1.8.0/tests/load_schema_test_15/
--rw-r--r--   0 sbelden    (501) staff       (20)       10 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_15/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_15/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.0/tests/load_schema_test_15/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.583623 fastavro-1.8.0/tests/load_schema_test_16/
--rw-r--r--   0 sbelden    (501) staff       (20)      225 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/load_schema_test_16/namespace.match.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      120 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/load_schema_test_16/namespace.team.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.584717 fastavro-1.8.0/tests/load_schema_test_2/
--rw-r--r--   0 sbelden    (501) staff       (20)      294 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test_2/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test_2/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.0/tests/load_schema_test_2/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.586139 fastavro-1.8.0/tests/load_schema_test_3/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_3/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_3/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_3/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.587468 fastavro-1.8.0/tests/load_schema_test_4/
--rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_4/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_4/B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_4/C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.588318 fastavro-1.8.0/tests/load_schema_test_5/
--rw-r--r--   0 sbelden    (501) staff       (20)      170 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_5/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_5/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.589348 fastavro-1.8.0/tests/load_schema_test_6/
--rw-r--r--   0 sbelden    (501) staff       (20)      173 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_6/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/load_schema_test_6/B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.590455 fastavro-1.8.0/tests/load_schema_test_7/
--rw-r--r--   0 sbelden    (501) staff       (20)      129 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_7/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      116 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_7/namespace.B.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.591750 fastavro-1.8.0/tests/load_schema_test_8/
--rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_8/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      102 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_8/namespace.B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      110 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_8/namespace.C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.592987 fastavro-1.8.0/tests/load_schema_test_9/
--rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_9/A.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_9/namespace.B.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.8.0/tests/load_schema_test_9/namespace.C.avsc
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.593328 fastavro-1.8.0/tests/repository/
-drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-06 15:53:50.594005 fastavro-1.8.0/tests/repository/flat_dict_test/
--rw-r--r--   0 sbelden    (501) staff       (20)       11 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/repository/flat_dict_test/InvalidJson.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)      111 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/repository/flat_dict_test/Valid.avsc
--rw-r--r--   0 sbelden    (501) staff       (20)     1153 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/repository/test_flat_dict.py
--rw-r--r--   0 sbelden    (501) staff       (20)     3678 2021-03-13 13:43:47.000000 fastavro-1.8.0/tests/test_aliases.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2185 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/test_appendable.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2533 2023-02-01 14:55:54.000000 fastavro-1.8.0/tests/test_block_reader.py
--rw-r--r--   0 sbelden    (501) staff       (20)    14428 2021-01-22 17:21:26.000000 fastavro-1.8.0/tests/test_canonical_form.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4768 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_complex.py
--rw-r--r--   0 sbelden    (501) staff       (20)     5623 2022-08-11 13:05:27.000000 fastavro-1.8.0/tests/test_compression.py
--rw-r--r--   0 sbelden    (501) staff       (20)    98991 2023-07-05 18:24:15.000000 fastavro-1.8.0/tests/test_fastavro.py
--rw-r--r--   0 sbelden    (501) staff       (20)    33787 2021-01-23 16:11:54.000000 fastavro-1.8.0/tests/test_fingerprint.py
--rw-r--r--   0 sbelden    (501) staff       (20)    27597 2023-07-06 14:53:47.000000 fastavro-1.8.0/tests/test_json.py
--rw-r--r--   0 sbelden    (501) staff       (20)    16587 2022-10-26 14:14:35.000000 fastavro-1.8.0/tests/test_logical_types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     3483 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_main_cli.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2229 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_promotion.py
--rw-r--r--   0 sbelden    (501) staff       (20)    40285 2023-05-04 14:35:44.000000 fastavro-1.8.0/tests/test_schema.py
--rw-r--r--   0 sbelden    (501) staff       (20)    22495 2023-02-01 14:56:44.000000 fastavro-1.8.0/tests/test_schema_evolution.py
--rw-r--r--   0 sbelden    (501) staff       (20)     8733 2023-07-06 14:53:47.000000 fastavro-1.8.0/tests/test_schemaless.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1224 2021-03-13 13:43:47.000000 fastavro-1.8.0/tests/test_str_py3.py
--rw-r--r--   0 sbelden    (501) staff       (20)     7148 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_timezone.py
--rw-r--r--   0 sbelden    (501) staff       (20)     2653 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_types.py
--rw-r--r--   0 sbelden    (501) staff       (20)     4503 2022-05-21 05:36:47.000000 fastavro-1.8.0/tests/test_utils.py
--rw-r--r--   0 sbelden    (501) staff       (20)    15273 2022-08-12 17:49:36.000000 fastavro-1.8.0/tests/test_validation.py
--rw-r--r--   0 sbelden    (501) staff       (20)     1653 2020-12-23 03:10:46.000000 fastavro-1.8.0/tests/test_write_block.py
--rw-r--r--   0 sbelden    (501) staff       (20)      253 2022-10-26 15:21:05.000000 fastavro-1.8.0/tox.ini
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.988569 fastavro-1.8.1/
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1625 2019-05-08 02:19:05.000000 fastavro-1.8.1/.azure_upload.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)       55 2020-12-23 03:10:46.000000 fastavro-1.8.1/.flake8.cython
+-rw-r--r--   0 sbelden    (501) staff       (20)    26402 2023-07-17 20:53:23.000000 fastavro-1.8.1/ChangeLog
+-rw-r--r--   0 sbelden    (501) staff       (20)      333 2022-10-26 14:14:35.000000 fastavro-1.8.1/Dockerfile
+-rw-r--r--   0 sbelden    (501) staff       (20)     1068 2019-05-04 22:05:46.000000 fastavro-1.8.1/LICENSE
+-rw-r--r--   0 sbelden    (501) staff       (20)      559 2022-08-11 13:05:27.000000 fastavro-1.8.1/MANIFEST.in
+-rw-r--r--   0 sbelden    (501) staff       (20)      812 2022-08-11 13:05:27.000000 fastavro-1.8.1/Makefile
+-rw-r--r--   0 sbelden    (501) staff       (20)      563 2019-05-04 22:05:46.000000 fastavro-1.8.1/NOTICE.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)     5187 2023-07-17 22:03:36.988699 fastavro-1.8.1/PKG-INFO
+-rw-r--r--   0 sbelden    (501) staff       (20)     3857 2023-07-17 20:43:04.000000 fastavro-1.8.1/README.md
+-rw-r--r--   0 sbelden    (501) staff       (20)      522 2023-07-17 20:52:16.000000 fastavro-1.8.1/developer_requirements.txt
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.875839 fastavro-1.8.1/docs/
+-rw-r--r--   0 sbelden    (501) staff       (20)     5578 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/Makefile
+-rw-r--r--   0 sbelden    (501) staff       (20)     1456 2019-05-04 22:05:46.000000 fastavro-1.8.1/docs/command_line_script.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     8320 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/conf.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2502 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/index.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.877214 fastavro-1.8.1/docs/io/
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/io/index.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/io/json_decoder.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      107 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/io/json_encoder.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       88 2020-02-26 16:33:59.000000 fastavro-1.8.1/docs/json_reader.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       91 2020-02-26 16:33:59.000000 fastavro-1.8.1/docs/json_writer.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     4869 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/logical_types.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      256 2021-03-20 12:25:05.000000 fastavro-1.8.1/docs/reader.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.878061 fastavro-1.8.1/docs/repository/
+-rw-r--r--   0 sbelden    (501) staff       (20)      116 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/repository/base.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/repository/index.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      405 2021-02-06 15:15:34.000000 fastavro-1.8.1/docs/schema.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      174 2021-03-13 13:43:47.000000 fastavro-1.8.1/docs/utils.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)      149 2019-05-04 22:05:46.000000 fastavro-1.8.1/docs/validation.rst
+-rw-r--r--   0 sbelden    (501) staff       (20)     3996 2022-08-11 13:05:27.000000 fastavro-1.8.1/docs/writer.rst
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.919473 fastavro-1.8.1/fastavro/
+-rw-r--r--   0 sbelden    (501) staff       (20)     1750 2023-07-17 20:53:27.000000 fastavro-1.8.1/fastavro/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2423 2020-12-23 03:10:46.000000 fastavro-1.8.1/fastavro/__main__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   262468 2023-07-17 22:03:32.000000 fastavro-1.8.1/fastavro/_logical_readers.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/_logical_readers.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     2792 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/_logical_readers.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     2813 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/_logical_readers_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      131 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/_logical_readers_py.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)   432466 2023-07-17 22:03:33.000000 fastavro-1.8.1/fastavro/_logical_writers.c
+-rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.8.1/fastavro/_logical_writers.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     8427 2022-10-06 12:45:33.000000 fastavro-1.8.1/fastavro/_logical_writers.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     7830 2022-10-06 12:45:33.000000 fastavro-1.8.1/fastavro/_logical_writers_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)       95 2020-06-22 15:51:13.000000 fastavro-1.8.1/fastavro/_logical_writers_py.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)  1105002 2023-07-17 22:03:33.000000 fastavro-1.8.1/fastavro/_read.c
+-rw-r--r--   0 sbelden    (501) staff       (20)     2070 2023-07-06 14:53:47.000000 fastavro-1.8.1/fastavro/_read.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    34172 2023-07-06 14:53:47.000000 fastavro-1.8.1/fastavro/_read.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)      703 2023-04-17 20:07:08.000000 fastavro-1.8.1/fastavro/_read_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    34680 2023-07-17 20:42:23.000000 fastavro-1.8.1/fastavro/_read_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   704771 2023-07-17 22:03:33.000000 fastavro-1.8.1/fastavro/_schema.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      950 2023-02-22 18:29:22.000000 fastavro-1.8.1/fastavro/_schema.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    24103 2023-05-04 14:35:44.000000 fastavro-1.8.1/fastavro/_schema.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)     1421 2021-01-23 16:11:54.000000 fastavro-1.8.1/fastavro/_schema_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    33011 2023-05-04 14:35:44.000000 fastavro-1.8.1/fastavro/_schema_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   441134 2020-08-18 18:15:09.000000 fastavro-1.8.1/fastavro/_six.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      633 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/_validate_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)   391404 2023-07-17 22:03:34.000000 fastavro-1.8.1/fastavro/_validation.c
+-rw-r--r--   0 sbelden    (501) staff       (20)      338 2022-08-12 17:49:36.000000 fastavro-1.8.1/fastavro/_validation.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)     9403 2022-08-15 15:33:27.000000 fastavro-1.8.1/fastavro/_validation.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)    10757 2022-08-15 15:33:27.000000 fastavro-1.8.1/fastavro/_validation_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)  1720429 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro/_write.c
+-rw-r--r--   0 sbelden    (501) staff       (20)     1680 2022-08-15 15:33:27.000000 fastavro-1.8.1/fastavro/_write.pyi
+-rw-r--r--   0 sbelden    (501) staff       (20)    26702 2023-04-17 20:07:08.000000 fastavro-1.8.1/fastavro/_write.pyx
+-rw-r--r--   0 sbelden    (501) staff       (20)      619 2023-05-03 19:57:13.000000 fastavro-1.8.1/fastavro/_write_common.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    26758 2023-04-17 20:07:08.000000 fastavro-1.8.1/fastavro/_write_py.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      853 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/const.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.927098 fastavro-1.8.1/fastavro/io/
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-02-26 16:33:59.000000 fastavro-1.8.1/fastavro/io/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4379 2023-07-06 14:53:47.000000 fastavro-1.8.1/fastavro/io/binary_decoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1861 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/io/binary_encoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     6936 2023-07-06 14:53:47.000000 fastavro-1.8.1/fastavro/io/json_decoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     5674 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/io/json_encoder.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4980 2022-02-25 13:49:52.000000 fastavro-1.8.1/fastavro/io/parser.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2321 2021-01-22 04:19:07.000000 fastavro-1.8.1/fastavro/io/symbols.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1603 2023-03-16 19:48:58.000000 fastavro-1.8.1/fastavro/json_read.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2908 2022-08-15 15:33:27.000000 fastavro-1.8.1/fastavro/json_write.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      217 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/logical_readers.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      217 2020-12-23 03:10:46.000000 fastavro-1.8.1/fastavro/logical_writers.py
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2020-06-22 15:51:13.000000 fastavro-1.8.1/fastavro/py.typed
+-rw-r--r--   0 sbelden    (501) staff       (20)      775 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/read.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.928648 fastavro-1.8.1/fastavro/repository/
+-rw-r--r--   0 sbelden    (501) staff       (20)      210 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/repository/__init__.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      185 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/repository/base.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      764 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/repository/flat_dict.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1030 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/schema.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      419 2022-08-11 13:05:27.000000 fastavro-1.8.1/fastavro/types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     7456 2023-02-01 14:56:04.000000 fastavro-1.8.1/fastavro/utils.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      422 2020-12-23 03:10:46.000000 fastavro-1.8.1/fastavro/validation.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      457 2021-02-27 20:10:59.000000 fastavro-1.8.1/fastavro/write.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.922819 fastavro-1.8.1/fastavro.egg-info/
+-rw-r--r--   0 sbelden    (501) staff       (20)     5187 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro.egg-info/PKG-INFO
+-rw-r--r--   0 sbelden    (501) staff       (20)     6017 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro.egg-info/SOURCES.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro.egg-info/dependency_links.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)       52 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro.egg-info/entry_points.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        1 2023-07-07 19:14:17.000000 fastavro-1.8.1/fastavro.egg-info/not-zip-safe
+-rw-r--r--   0 sbelden    (501) staff       (20)       96 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro.egg-info/requires.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)        9 2023-07-17 22:03:36.000000 fastavro-1.8.1/fastavro.egg-info/top_level.txt
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2023-04-17 20:07:08.000000 fastavro-1.8.1/mypy.ini
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1210 2023-07-17 20:43:04.000000 fastavro-1.8.1/publish.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)      206 2023-07-17 20:43:20.000000 fastavro-1.8.1/pyproject.toml
+-rwxr-xr-x   0 sbelden    (501) staff       (20)       31 2019-05-04 22:05:46.000000 fastavro-1.8.1/pytest.ini
+-rw-r--r--   0 sbelden    (501) staff       (20)      710 2023-07-17 20:43:04.000000 fastavro-1.8.1/run-tests.cmd
+-rwxr-xr-x   0 sbelden    (501) staff       (20)     1050 2023-07-17 20:43:04.000000 fastavro-1.8.1/run-tests.sh
+-rw-r--r--   0 sbelden    (501) staff       (20)      105 2023-07-17 22:03:36.989088 fastavro-1.8.1/setup.cfg
+-rw-r--r--   0 sbelden    (501) staff       (20)     2747 2023-07-17 20:43:04.000000 fastavro-1.8.1/setup.py
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      169 2023-03-08 22:33:06.000000 fastavro-1.8.1/tag.sh
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.944288 fastavro-1.8.1/tests/
+-rw-r--r--   0 sbelden    (501) staff       (20)        0 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/__init__.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.966331 fastavro-1.8.1/tests/avro-files/
+-rw-r--r--   0 sbelden    (501) staff       (20)       55 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/Child.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/Child1.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      179 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/Parent.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      130 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/ParentMissingChild.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      447 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/a_triple_pair.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       79 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/bool.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.seperators.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.deflate.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       84 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.testWrite.plain.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       56 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/class org.apache.avro.tool.TestDataFileTools.zerojsonvalues.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3293 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/deflate.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      276 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/double_float.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      234 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/error-type.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     8453 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/java-generated-uuid.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      299 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/lines.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      403 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/m.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      139 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/no-fields.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3285 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/null.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       68 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/org.apache.avro.tool.TestDataFileTools.avro
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      321 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/part-00000.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      218 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/recursive.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      162 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/request.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       89 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/response.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     3296 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/snappy.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12556 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-deflate-0.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-deflate-1-A.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-deflate-1.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    11906 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-deflate-3-A.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     6112 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-deflate-6-B.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    12546 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-deflate-9.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)     6522 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-null-B.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    13289 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-null.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)    13677 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test-snappy.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      182 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/test.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)       51 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/testDataFileMeta.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      690 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/avro-files/weather-legacy-generated.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      696 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/avro-files/weather-legacy-with-names.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      330 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/weather-snappy.avro
+-rwxr-xr-x   0 sbelden    (501) staff       (20)      335 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/weather-sorted.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      358 2019-05-04 22:05:46.000000 fastavro-1.8.1/tests/avro-files/weather.avro
+-rw-r--r--   0 sbelden    (501) staff       (20)      999 2021-03-13 13:43:47.000000 fastavro-1.8.1/tests/conftest.py
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.968479 fastavro-1.8.1/tests/load_schema_test/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test/D.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.970825 fastavro-1.8.1/tests/load_schema_test_10/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_10/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_10/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_10/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_10/D.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.973046 fastavro-1.8.1/tests/load_schema_test_11/
+-rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_11/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       99 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_11/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      135 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_11/C.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_11/D.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_11/E.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.973464 fastavro-1.8.1/tests/load_schema_test_12/
+-rw-r--r--   0 sbelden    (501) staff       (20)      143 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_12/A.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.974363 fastavro-1.8.1/tests/load_schema_test_12/com/
+-rw-r--r--   0 sbelden    (501) staff       (20)      137 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_12/com/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      187 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_12/com/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.975321 fastavro-1.8.1/tests/load_schema_test_12/com/namespace/
+-rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_12/com/namespace/D.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      140 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_12/com/namespace/E.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.976300 fastavro-1.8.1/tests/load_schema_test_13/
+-rw-r--r--   0 sbelden    (501) staff       (20)        3 2021-04-16 21:12:43.000000 fastavro-1.8.1/tests/load_schema_test_13/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.1/tests/load_schema_test_13/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.976848 fastavro-1.8.1/tests/load_schema_test_14/
+-rw-r--r--   0 sbelden    (501) staff       (20)        8 2021-04-16 21:12:43.000000 fastavro-1.8.1/tests/load_schema_test_14/A.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.978035 fastavro-1.8.1/tests/load_schema_test_15/
+-rw-r--r--   0 sbelden    (501) staff       (20)       10 2021-04-16 21:12:43.000000 fastavro-1.8.1/tests/load_schema_test_15/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.1/tests/load_schema_test_15/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2021-04-16 21:12:43.000000 fastavro-1.8.1/tests/load_schema_test_15/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.978927 fastavro-1.8.1/tests/load_schema_test_16/
+-rw-r--r--   0 sbelden    (501) staff       (20)      225 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/load_schema_test_16/namespace.match.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      120 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/load_schema_test_16/namespace.team.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.980182 fastavro-1.8.1/tests/load_schema_test_2/
+-rw-r--r--   0 sbelden    (501) staff       (20)      294 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test_2/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test_2/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-07-11 18:46:51.000000 fastavro-1.8.1/tests/load_schema_test_2/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.981644 fastavro-1.8.1/tests/load_schema_test_3/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_3/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_3/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_3/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.982732 fastavro-1.8.1/tests/load_schema_test_4/
+-rw-r--r--   0 sbelden    (501) staff       (20)      189 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_4/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_4/B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      126 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_4/C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.983473 fastavro-1.8.1/tests/load_schema_test_5/
+-rw-r--r--   0 sbelden    (501) staff       (20)      170 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_5/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_5/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.984195 fastavro-1.8.1/tests/load_schema_test_6/
+-rw-r--r--   0 sbelden    (501) staff       (20)      173 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_6/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      106 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/load_schema_test_6/B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.984957 fastavro-1.8.1/tests/load_schema_test_7/
+-rw-r--r--   0 sbelden    (501) staff       (20)      129 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_7/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      116 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_7/namespace.B.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.986060 fastavro-1.8.1/tests/load_schema_test_8/
+-rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_8/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      102 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_8/namespace.B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      110 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_8/namespace.C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.987117 fastavro-1.8.1/tests/load_schema_test_9/
+-rw-r--r--   0 sbelden    (501) staff       (20)      165 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_9/A.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_9/namespace.B.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)       65 2021-01-22 04:19:07.000000 fastavro-1.8.1/tests/load_schema_test_9/namespace.C.avsc
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.987449 fastavro-1.8.1/tests/repository/
+drwxr-xr-x   0 sbelden    (501) staff       (20)        0 2023-07-17 22:03:36.988225 fastavro-1.8.1/tests/repository/flat_dict_test/
+-rw-r--r--   0 sbelden    (501) staff       (20)       11 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/repository/flat_dict_test/InvalidJson.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)      111 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/repository/flat_dict_test/Valid.avsc
+-rw-r--r--   0 sbelden    (501) staff       (20)     1153 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/repository/test_flat_dict.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     3678 2021-03-13 13:43:47.000000 fastavro-1.8.1/tests/test_aliases.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2185 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/test_appendable.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2533 2023-02-01 14:55:54.000000 fastavro-1.8.1/tests/test_block_reader.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    14428 2021-01-22 17:21:26.000000 fastavro-1.8.1/tests/test_canonical_form.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4768 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/test_complex.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     5623 2022-08-11 13:05:27.000000 fastavro-1.8.1/tests/test_compression.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    98878 2023-07-17 20:43:04.000000 fastavro-1.8.1/tests/test_fastavro.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    33787 2021-01-23 16:11:54.000000 fastavro-1.8.1/tests/test_fingerprint.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    27597 2023-07-06 14:53:47.000000 fastavro-1.8.1/tests/test_json.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    16587 2022-10-26 14:14:35.000000 fastavro-1.8.1/tests/test_logical_types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     3483 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/test_main_cli.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2229 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/test_promotion.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    40285 2023-05-04 14:35:44.000000 fastavro-1.8.1/tests/test_schema.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    22495 2023-02-01 14:56:44.000000 fastavro-1.8.1/tests/test_schema_evolution.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     8733 2023-07-06 14:53:47.000000 fastavro-1.8.1/tests/test_schemaless.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1224 2021-03-13 13:43:47.000000 fastavro-1.8.1/tests/test_str_py3.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     7148 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/test_timezone.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     2653 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/test_types.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     4503 2022-05-21 05:36:47.000000 fastavro-1.8.1/tests/test_utils.py
+-rw-r--r--   0 sbelden    (501) staff       (20)    15273 2022-08-12 17:49:36.000000 fastavro-1.8.1/tests/test_validation.py
+-rw-r--r--   0 sbelden    (501) staff       (20)     1653 2020-12-23 03:10:46.000000 fastavro-1.8.1/tests/test_write_block.py
+-rw-r--r--   0 sbelden    (501) staff       (20)      248 2023-07-17 20:43:04.000000 fastavro-1.8.1/tox.ini
```

### Comparing `fastavro-1.8.0/.azure_upload.sh` & `fastavro-1.8.1/.azure_upload.sh`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/ChangeLog` & `fastavro-1.8.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-17 version 1.8.1
+* Pin Cython<3 to fix breakage
+
 2023-07-06 version 1.8.0
 * Add ability to override unicode decode errors (@scottbelden in PR #696)
 
 2023-05-04 version 1.7.4
 * Fix parsing of namespaces (@scottbelden in PR #692)
 * Be able to specify a reader schema in the json_reader (@scottbelden in PR #681)
```

### Comparing `fastavro-1.8.0/LICENSE` & `fastavro-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/MANIFEST.in` & `fastavro-1.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/Makefile` & `fastavro-1.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/NOTICE.txt` & `fastavro-1.8.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/PKG-INFO` & `fastavro-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: fastavro
-Version: 1.8.0
+Version: 1.8.1
 Summary: Fast read/write of AVRO files
 Home-page: https://github.com/fastavro/fastavro
 Author: Miki Tebeka
 Author-email: miki.tebeka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: codecs
 Provides-Extra: snappy
 Provides-Extra: zstandard
 Provides-Extra: lz4
 License-File: LICENSE
 License-File: NOTICE.txt
@@ -48,15 +47,14 @@
 library. With regular CPython, `fastavro` uses C extensions which allow it to
 iterate the same 10,000 record file in 1.7 seconds. With PyPy, this drops to 1.5
 seconds (to be fair, the JAVA benchmark is doing some extra JSON
 encoding/decoding).
 
 `fastavro` supports the following Python versions:
 
-* Python 3.7
 * Python 3.8
 * Python 3.9
 * Python 3.10
 * Python 3.11
 * PyPy3
 
 ## Supported Features
```

### Comparing `fastavro-1.8.0/README.md` & `fastavro-1.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 library. With regular CPython, `fastavro` uses C extensions which allow it to
 iterate the same 10,000 record file in 1.7 seconds. With PyPy, this drops to 1.5
 seconds (to be fair, the JAVA benchmark is doing some extra JSON
 encoding/decoding).
 
 `fastavro` supports the following Python versions:
 
-* Python 3.7
 * Python 3.8
 * Python 3.9
 * Python 3.10
 * Python 3.11
 * PyPy3
 
 ## Supported Features
```

### Comparing `fastavro-1.8.0/developer_requirements.txt` & `fastavro-1.8.1/developer_requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pytest-cov
 pytest
 flake8
 check-manifest
-Cython
+Cython<3
 numpy # used in tests
 pandas; platform_python_implementation!='PyPy' # used in tests; not install on pypy as it takes forever
 wheel
 twine
 coverage
 mypy; implementation_name != "pypy"
 black; implementation_name != "pypy"
```

### Comparing `fastavro-1.8.0/docs/Makefile` & `fastavro-1.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/docs/command_line_script.rst` & `fastavro-1.8.1/docs/command_line_script.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/docs/conf.py` & `fastavro-1.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/docs/index.rst` & `fastavro-1.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/docs/logical_types.rst` & `fastavro-1.8.1/docs/logical_types.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/docs/writer.rst` & `fastavro-1.8.1/docs/writer.rst`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/__init__.py` & `fastavro-1.8.1/fastavro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         {u'station': u'012650-99999', u'temp': 111, u'time': 1433275478},
     ]
 
     with open('weather.avro', 'wb') as out:
         writer(out, schema, records)
 """
 
-__version_info__ = (1, 8, 0)
+__version_info__ = (1, 8, 1)
 __version__ = "%s.%s.%s" % __version_info__
 
 
 import fastavro.read
 import fastavro.write
 import fastavro.schema
 import fastavro.validation
```

### Comparing `fastavro-1.8.0/fastavro/__main__.py` & `fastavro-1.8.1/fastavro/__main__.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_logical_readers.c` & `fastavro-1.8.1/fastavro/_logical_readers.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -5571,15 +5577,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5767,15 +5773,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `fastavro-1.8.0/fastavro/_logical_readers.pyx` & `fastavro-1.8.1/fastavro/_logical_readers.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_logical_readers_py.py` & `fastavro-1.8.1/fastavro/_logical_readers_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_logical_writers.c` & `fastavro-1.8.1/fastavro/_logical_writers.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1288,22 +1294,30 @@
 static PyObject* __Pyx_PyInt_AndObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AndObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAnd(op1, op2) : PyNumber_And(op1, op2))
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -6216,22 +6230,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -7712,28 +7725,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -8601,61 +8614,79 @@
     }
     #endif
     return (inplace ? PyNumber_InPlaceAnd : PyNumber_And)(op1, op2);
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -9051,15 +9082,15 @@
                         } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
                             return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9323,15 +9354,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9519,15 +9550,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `fastavro-1.8.0/fastavro/_logical_writers.pyx` & `fastavro-1.8.1/fastavro/_logical_writers.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_logical_writers_py.py` & `fastavro-1.8.1/fastavro/_logical_writers_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_read.c` & `fastavro-1.8.1/fastavro/_read.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -3387,29 +3393,29 @@
       /* "fastavro/_read.pyx":86
  *     else:
  *         # Check for dicts as primitive types are just strings
  *         if isinstance(w_schema, dict):             # <<<<<<<<<<<<<<
  *             w_type = w_schema["type"]
  *         else:
  */
-      goto __pyx_L8;
+      goto __pyx_L9;
     }
 
     /* "fastavro/_read.pyx":89
  *             w_type = w_schema["type"]
  *         else:
  *             w_type = w_schema             # <<<<<<<<<<<<<<
  *         if isinstance(r_schema, dict):
  *             r_type = r_schema["type"]
  */
     /*else*/ {
       __Pyx_INCREF(__pyx_v_w_schema);
       __pyx_v_w_type = __pyx_v_w_schema;
     }
-    __pyx_L8:;
+    __pyx_L9:;
 
     /* "fastavro/_read.pyx":90
  *         else:
  *             w_type = w_schema
  *         if isinstance(r_schema, dict):             # <<<<<<<<<<<<<<
  *             r_type = r_schema["type"]
  *         else:
@@ -3433,29 +3439,29 @@
       /* "fastavro/_read.pyx":90
  *         else:
  *             w_type = w_schema
  *         if isinstance(r_schema, dict):             # <<<<<<<<<<<<<<
  *             r_type = r_schema["type"]
  *         else:
  */
-      goto __pyx_L9;
+      goto __pyx_L10;
     }
 
     /* "fastavro/_read.pyx":93
  *             r_type = r_schema["type"]
  *         else:
  *             r_type = r_schema             # <<<<<<<<<<<<<<
  * 
  *         if w_type == r_type == "map":
  */
     /*else*/ {
       __Pyx_INCREF(__pyx_v_r_schema);
       __pyx_v_r_type = __pyx_v_r_schema;
     }
-    __pyx_L9:;
+    __pyx_L10:;
 
     /* "fastavro/_read.pyx":95
  *             r_type = r_schema
  * 
  *         if w_type == r_type == "map":             # <<<<<<<<<<<<<<
  *             if match_types(w_schema["values"], r_schema["values"]):
  *                 return r_schema
@@ -3512,15 +3518,15 @@
       /* "fastavro/_read.pyx":95
  *             r_type = r_schema
  * 
  *         if w_type == r_type == "map":             # <<<<<<<<<<<<<<
  *             if match_types(w_schema["values"], r_schema["values"]):
  *                 return r_schema
  */
-      goto __pyx_L10;
+      goto __pyx_L11;
     }
 
     /* "fastavro/_read.pyx":98
  *             if match_types(w_schema["values"], r_schema["values"]):
  *                 return r_schema
  *         elif w_type == r_type == "array":             # <<<<<<<<<<<<<<
  *             if match_types(w_schema["items"], r_schema["items"]):
@@ -3578,15 +3584,15 @@
       /* "fastavro/_read.pyx":98
  *             if match_types(w_schema["values"], r_schema["values"]):
  *                 return r_schema
  *         elif w_type == r_type == "array":             # <<<<<<<<<<<<<<
  *             if match_types(w_schema["items"], r_schema["items"]):
  *                 return r_schema
  */
-      goto __pyx_L10;
+      goto __pyx_L11;
     }
 
     /* "fastavro/_read.pyx":101
  *             if match_types(w_schema["items"], r_schema["items"]):
  *                 return r_schema
  *         elif w_type in NAMED_TYPES and r_type in NAMED_TYPES:             # <<<<<<<<<<<<<<
  *             if w_type == r_type == "fixed" and w_schema["size"] != r_schema["size"]:
@@ -3596,23 +3602,23 @@
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_v_w_type, __pyx_t_4, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_10 = (__pyx_t_6 != 0);
     if (__pyx_t_10) {
     } else {
       __pyx_t_5 = __pyx_t_10;
-      goto __pyx_L13_bool_binop_done;
+      goto __pyx_L14_bool_binop_done;
     }
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NAMED_TYPES); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_10 = (__Pyx_PySequence_ContainsTF(__pyx_v_r_type, __pyx_t_4, Py_EQ)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_6 = (__pyx_t_10 != 0);
     __pyx_t_5 = __pyx_t_6;
-    __pyx_L13_bool_binop_done:;
+    __pyx_L14_bool_binop_done:;
     if (__pyx_t_5) {
 
       /* "fastavro/_read.pyx":102
  *                 return r_schema
  *         elif w_type in NAMED_TYPES and r_type in NAMED_TYPES:
  *             if w_type == r_type == "fixed" and w_schema["size"] != r_schema["size"]:             # <<<<<<<<<<<<<<
  *                 raise SchemaResolutionError(
@@ -3624,27 +3630,27 @@
         __pyx_t_4 = PyObject_RichCompare(__pyx_v_r_type, __pyx_n_u_fixed, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
       }
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_6) {
       } else {
         __pyx_t_5 = __pyx_t_6;
-        goto __pyx_L16_bool_binop_done;
+        goto __pyx_L17_bool_binop_done;
       }
       __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_w_schema, __pyx_n_u_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_r_schema, __pyx_n_u_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_8 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_5 = __pyx_t_6;
-      __pyx_L16_bool_binop_done:;
+      __pyx_L17_bool_binop_done:;
       if (unlikely(__pyx_t_5)) {
 
         /* "fastavro/_read.pyx":103
  *         elif w_type in NAMED_TYPES and r_type in NAMED_TYPES:
  *             if w_type == r_type == "fixed" and w_schema["size"] != r_schema["size"]:
  *                 raise SchemaResolutionError(             # <<<<<<<<<<<<<<
  *                     f"Schema mismatch: {w_schema} size is different than {r_schema} size"
@@ -3797,15 +3803,15 @@
  */
       __pyx_t_1 = PyObject_RichCompare(__pyx_v_w_unqual_name, __pyx_v_r_unqual_name, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
       __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (!__pyx_t_6) {
       } else {
         __pyx_t_5 = __pyx_t_6;
-        goto __pyx_L19_bool_binop_done;
+        goto __pyx_L20_bool_binop_done;
       }
       __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_w_schema, __pyx_n_u_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_r_schema, __pyx_n_s_get); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
 
       /* "fastavro/_read.pyx":110
@@ -3873,15 +3879,15 @@
  *             r_unqual_name = r_schema["name"].split(".")[-1]
  *             if w_unqual_name == r_unqual_name or w_schema["name"] in r_schema.get(             # <<<<<<<<<<<<<<
  *                 "aliases", []
  *             ):
  */
       __pyx_t_10 = (__pyx_t_6 != 0);
       __pyx_t_5 = __pyx_t_10;
-      __pyx_L19_bool_binop_done:;
+      __pyx_L20_bool_binop_done:;
       if (__pyx_t_5) {
 
         /* "fastavro/_read.pyx":112
  *                 "aliases", []
  *             ):
  *                 return r_schema             # <<<<<<<<<<<<<<
  *         elif w_type not in AVRO_TYPES and r_type in NAMED_TYPES:
@@ -3904,15 +3910,15 @@
       /* "fastavro/_read.pyx":101
  *             if match_types(w_schema["items"], r_schema["items"]):
  *                 return r_schema
  *         elif w_type in NAMED_TYPES and r_type in NAMED_TYPES:             # <<<<<<<<<<<<<<
  *             if w_type == r_type == "fixed" and w_schema["size"] != r_schema["size"]:
  *                 raise SchemaResolutionError(
  */
-      goto __pyx_L10;
+      goto __pyx_L11;
     }
 
     /* "fastavro/_read.pyx":113
  *             ):
  *                 return r_schema
  *         elif w_type not in AVRO_TYPES and r_type in NAMED_TYPES:             # <<<<<<<<<<<<<<
  *             if match_types(w_type, r_schema["name"]):
@@ -3922,23 +3928,23 @@
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_10 = (__Pyx_PySequence_ContainsTF(__pyx_v_w_type, __pyx_t_9, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_6 = (__pyx_t_10 != 0);
     if (__pyx_t_6) {
     } else {
       __pyx_t_5 = __pyx_t_6;
-      goto __pyx_L21_bool_binop_done;
+      goto __pyx_L22_bool_binop_done;
     }
     __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_NAMED_TYPES); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_v_r_type, __pyx_t_9, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_10 = (__pyx_t_6 != 0);
     __pyx_t_5 = __pyx_t_10;
-    __pyx_L21_bool_binop_done:;
+    __pyx_L22_bool_binop_done:;
     if (__pyx_t_5) {
 
       /* "fastavro/_read.pyx":114
  *                 return r_schema
  *         elif w_type not in AVRO_TYPES and r_type in NAMED_TYPES:
  *             if match_types(w_type, r_schema["name"]):             # <<<<<<<<<<<<<<
  *                 return r_schema["name"]
@@ -3979,15 +3985,15 @@
       /* "fastavro/_read.pyx":113
  *             ):
  *                 return r_schema
  *         elif w_type not in AVRO_TYPES and r_type in NAMED_TYPES:             # <<<<<<<<<<<<<<
  *             if match_types(w_type, r_schema["name"]):
  *                 return r_schema["name"]
  */
-      goto __pyx_L10;
+      goto __pyx_L11;
     }
 
     /* "fastavro/_read.pyx":116
  *             if match_types(w_type, r_schema["name"]):
  *                 return r_schema["name"]
  *         elif match_types(w_type, r_type):             # <<<<<<<<<<<<<<
  *             return r_schema
@@ -4015,15 +4021,15 @@
  *             if match_types(w_type, r_schema["name"]):
  *                 return r_schema["name"]
  *         elif match_types(w_type, r_type):             # <<<<<<<<<<<<<<
  *             return r_schema
  *         raise SchemaResolutionError(error_msg)
  */
     }
-    __pyx_L10:;
+    __pyx_L11:;
 
     /* "fastavro/_read.pyx":118
  *         elif match_types(w_type, r_type):
  *             return r_schema
  *         raise SchemaResolutionError(error_msg)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -19255,15 +19261,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks *__pyx_freelist_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks[8];
 static int __pyx_freecount_8fastavro_5_read___pyx_scope_struct_1__iter_avro_blocks = 0;
 
@@ -19408,15 +19414,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_5_read___pyx_scope_struct_2___iter__ *__pyx_freelist_8fastavro_5_read___pyx_scope_struct_2___iter__[8];
 static int __pyx_freecount_8fastavro_5_read___pyx_scope_struct_2___iter__ = 0;
 
@@ -19525,15 +19531,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"match_types", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_1match_types, METH_VARARGS|METH_KEYWORDS, 0},
   {"match_schemas", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_5_read_3match_schemas, METH_VARARGS|METH_KEYWORDS, 0},
@@ -22736,28 +22742,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -23876,19 +23882,19 @@
     PyErr_Format(PyExc_TypeError,
         "%.200s object is not an iterator", Py_TYPE(iterator)->tp_name);
 }
 static CYTHON_INLINE PyObject *__Pyx_PyIter_Next2(PyObject* iterator, PyObject* defval) {
     PyObject* next;
     iternextfunc iternext = Py_TYPE(iterator)->tp_iternext;
     if (likely(iternext)) {
-#if CYTHON_USE_TYPE_SLOTS
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
         next = iternext(iterator);
         if (likely(next))
             return next;
-        #if PY_VERSION_HEX >= 0x02070000
+        #if PY_VERSION_HEX >= 0x02070000 && CYTHON_COMPILING_IN_CPYTHON
         if (unlikely(iternext == &_PyObject_NextNotImplemented))
             return NULL;
         #endif
 #else
         next = PyIter_Next(iterator);
         if (likely(next))
             return next;
@@ -24716,15 +24722,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -25136,15 +25145,15 @@
                         } else if (8 * sizeof(unsigned char) >= 4 * PyLong_SHIFT) {
                             return (unsigned char) (((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25370,15 +25379,15 @@
                         } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
                             return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25566,15 +25575,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25762,15 +25771,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26896,15 +26905,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `fastavro-1.8.0/fastavro/_read.pyi` & `fastavro-1.8.1/fastavro/_read.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_read.pyx` & `fastavro-1.8.1/fastavro/_read.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_read_common.py` & `fastavro-1.8.1/fastavro/_read_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_read_py.py` & `fastavro-1.8.1/fastavro/_read_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_schema.c` & `fastavro-1.8.1/fastavro/_schema.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -14864,28 +14870,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -16410,15 +16416,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16606,15 +16612,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `fastavro-1.8.0/fastavro/_schema.pyi` & `fastavro-1.8.1/fastavro/_schema.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_schema.pyx` & `fastavro-1.8.1/fastavro/_schema.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_schema_common.py` & `fastavro-1.8.1/fastavro/_schema_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_schema_py.py` & `fastavro-1.8.1/fastavro/_schema_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_six.c` & `fastavro-1.8.1/fastavro/_six.c`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_validate_common.py` & `fastavro-1.8.1/fastavro/_validate_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_validation.c` & `fastavro-1.8.1/fastavro/_validation.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -3797,39 +3803,39 @@
         /* "fastavro/_validation.pyx":193
  *     for s in schema:
  *         try:
  *             ret = _validate(             # <<<<<<<<<<<<<<
  *                 datum,
  *                 schema=s,
  */
-        __pyx_t_4 = __pyx_f_8fastavro_11_validation__validate(__pyx_v_datum, __pyx_v_s, __pyx_v_named_schemas, __pyx_v_parent_ns, __pyx_v_raise_errors, __pyx_v_options, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L15_error)
+        __pyx_t_4 = __pyx_f_8fastavro_11_validation__validate(__pyx_v_datum, __pyx_v_s, __pyx_v_named_schemas, __pyx_v_parent_ns, __pyx_v_raise_errors, __pyx_v_options, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_XDECREF_SET(__pyx_v_ret, __pyx_t_4);
         __pyx_t_4 = 0;
 
         /* "fastavro/_validation.pyx":201
  *                 options=options,
  *             )
  *             if ret:             # <<<<<<<<<<<<<<
  *                 # We exit on the first passing type in Unions
  *                 return True
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_ret); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 201, __pyx_L15_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_ret); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 201, __pyx_L16_error)
         if (__pyx_t_1) {
 
           /* "fastavro/_validation.pyx":203
  *             if ret:
  *                 # We exit on the first passing type in Unions
  *                 return True             # <<<<<<<<<<<<<<
  *         except ValidationError as e:
  *             errors.extend(e.errors)
  */
           __pyx_r = 1;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          goto __pyx_L19_try_return;
+          goto __pyx_L20_try_return;
 
           /* "fastavro/_validation.pyx":201
  *                 options=options,
  *             )
  *             if ret:             # <<<<<<<<<<<<<<
  *                 # We exit on the first passing type in Unions
  *                 return True
@@ -3843,71 +3849,71 @@
  *             ret = _validate(
  *                 datum,
  */
       }
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      goto __pyx_L22_try_end;
-      __pyx_L15_error:;
+      goto __pyx_L23_try_end;
+      __pyx_L16_error:;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
       /* "fastavro/_validation.pyx":204
  *                 # We exit on the first passing type in Unions
  *                 return True
  *         except ValidationError as e:             # <<<<<<<<<<<<<<
  *             errors.extend(e.errors)
  *     if raise_errors:
  */
       __Pyx_ErrFetch(&__pyx_t_4, &__pyx_t_6, &__pyx_t_9);
-      __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_ValidationError); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 204, __pyx_L17_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_ValidationError); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 204, __pyx_L18_except_error)
       __Pyx_GOTREF(__pyx_t_13);
       __pyx_t_14 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_4, __pyx_t_13);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_ErrRestore(__pyx_t_4, __pyx_t_6, __pyx_t_9);
       __pyx_t_4 = 0; __pyx_t_6 = 0; __pyx_t_9 = 0;
       if (__pyx_t_14) {
         __Pyx_AddTraceback("fastavro._validation.validate_union", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_6, &__pyx_t_4) < 0) __PYX_ERR(0, 204, __pyx_L17_except_error)
+        if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_6, &__pyx_t_4) < 0) __PYX_ERR(0, 204, __pyx_L18_except_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_6);
         __pyx_v_e = __pyx_t_6;
         /*try:*/ {
 
           /* "fastavro/_validation.pyx":205
  *                 return True
  *         except ValidationError as e:
  *             errors.extend(e.errors)             # <<<<<<<<<<<<<<
  *     if raise_errors:
  *         raise ValidationError(*errors)
  */
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_e, __pyx_n_s_errors); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 205, __pyx_L29_error)
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_e, __pyx_n_s_errors); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 205, __pyx_L30_error)
           __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_15 = __Pyx_PyList_Extend(__pyx_v_errors, __pyx_t_13); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 205, __pyx_L29_error)
+          __pyx_t_15 = __Pyx_PyList_Extend(__pyx_v_errors, __pyx_t_13); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 205, __pyx_L30_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         }
 
         /* "fastavro/_validation.pyx":204
  *                 # We exit on the first passing type in Unions
  *                 return True
  *         except ValidationError as e:             # <<<<<<<<<<<<<<
  *             errors.extend(e.errors)
  *     if raise_errors:
  */
         /*finally:*/ {
           /*normal exit:*/{
             __Pyx_DECREF(__pyx_v_e);
             __pyx_v_e = NULL;
-            goto __pyx_L30;
+            goto __pyx_L31;
           }
-          __pyx_L29_error:;
+          __pyx_L30_error:;
           /*exception exit:*/{
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
             __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
             if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
             if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20) < 0)) __Pyx_ErrFetch(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
@@ -3930,50 +3936,50 @@
             }
             __Pyx_XGIVEREF(__pyx_t_18);
             __Pyx_XGIVEREF(__pyx_t_19);
             __Pyx_XGIVEREF(__pyx_t_20);
             __Pyx_ErrRestore(__pyx_t_18, __pyx_t_19, __pyx_t_20);
             __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
             __pyx_lineno = __pyx_t_14; __pyx_clineno = __pyx_t_16; __pyx_filename = __pyx_t_17;
-            goto __pyx_L17_except_error;
+            goto __pyx_L18_except_error;
           }
-          __pyx_L30:;
+          __pyx_L31:;
         }
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        goto __pyx_L16_exception_handled;
+        goto __pyx_L17_exception_handled;
       }
-      goto __pyx_L17_except_error;
-      __pyx_L17_except_error:;
+      goto __pyx_L18_except_error;
+      __pyx_L18_except_error:;
 
       /* "fastavro/_validation.pyx":192
  *     cdef list errors = []
  *     for s in schema:
  *         try:             # <<<<<<<<<<<<<<
  *             ret = _validate(
  *                 datum,
  */
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       goto __pyx_L1_error;
-      __pyx_L19_try_return:;
+      __pyx_L20_try_return:;
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       goto __pyx_L0;
-      __pyx_L16_exception_handled:;
+      __pyx_L17_exception_handled:;
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
-      __pyx_L22_try_end:;
+      __pyx_L23_try_end:;
     }
 
     /* "fastavro/_validation.pyx":191
  * 
  *     cdef list errors = []
  *     for s in schema:             # <<<<<<<<<<<<<<
  *         try:
@@ -8554,28 +8560,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -9129,15 +9135,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9325,15 +9331,15 @@
                         } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
                             return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9635,15 +9641,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `fastavro-1.8.0/fastavro/_validation.pyx` & `fastavro-1.8.1/fastavro/_validation.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_validation_py.py` & `fastavro-1.8.1/fastavro/_validation_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_write.c` & `fastavro-1.8.1/fastavro/_write.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -2079,14 +2085,31 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PyObject_GenericGetAttrNoDict.proto */
@@ -2109,22 +2132,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -26257,15 +26288,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -31979,15 +32010,15 @@
   p->value = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_8fastavro_6_write_MemoryIO(PyObject *o) {
   struct __pyx_obj_8fastavro_6_write_MemoryIO *p = (struct __pyx_obj_8fastavro_6_write_MemoryIO *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->value);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
@@ -32063,15 +32094,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_8fastavro_6_write_Writer(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_8fastavro_6_write_Writer *p;
   PyObject *o;
@@ -32094,15 +32125,15 @@
   p->options = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_8fastavro_6_write_Writer(PyObject *o) {
   struct __pyx_obj_8fastavro_6_write_Writer *p = (struct __pyx_obj_8fastavro_6_write_Writer *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->fo);
   Py_CLEAR(p->schema);
   Py_CLEAR(p->validate_fn);
@@ -32435,15 +32466,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_6_write___pyx_scope_struct____pyx_f_8fastavro_6_write_write_union *__pyx_freelist_8fastavro_6_write___pyx_scope_struct____pyx_f_8fastavro_6_write_write_union[8];
 static int __pyx_freecount_8fastavro_6_write___pyx_scope_struct____pyx_f_8fastavro_6_write_write_union = 0;
 
@@ -32553,15 +32584,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_6_write___pyx_scope_struct_1_genexpr *__pyx_freelist_8fastavro_6_write___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_8fastavro_6_write___pyx_scope_struct_1_genexpr = 0;
 
@@ -32666,15 +32697,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_6_write___pyx_scope_struct_2___pyx_f_8fastavro_6_write_write_record *__pyx_freelist_8fastavro_6_write___pyx_scope_struct_2___pyx_f_8fastavro_6_write_write_record[8];
 static int __pyx_freecount_8fastavro_6_write___pyx_scope_struct_2___pyx_f_8fastavro_6_write_write_record = 0;
 
@@ -32784,15 +32815,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_6_write___pyx_scope_struct_3_genexpr *__pyx_freelist_8fastavro_6_write___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_8fastavro_6_write___pyx_scope_struct_3_genexpr = 0;
 
@@ -32897,15 +32928,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8fastavro_6_write___pyx_scope_struct_4__missing_dependency *__pyx_freelist_8fastavro_6_write___pyx_scope_struct_4__missing_dependency[8];
 static int __pyx_freecount_8fastavro_6_write___pyx_scope_struct_4__missing_dependency = 0;
 
@@ -33022,15 +33053,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -33051,15 +33082,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -33214,15 +33245,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -33236,15 +33267,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -33336,15 +33367,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -33367,15 +33398,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -33600,15 +33631,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -33620,15 +33651,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -33749,15 +33780,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"write_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_6_write_1write_data, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8fastavro_6_write_write_data},
   {"write_header", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8fastavro_6_write_3write_header, METH_VARARGS|METH_KEYWORDS, 0},
@@ -34561,14 +34592,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
   __pyx_umethod_PySet_Type_intersection.type = (PyObject*)&PySet_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1000 = PyInt_FromLong(1000); if (unlikely(!__pyx_int_1000)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -34761,37 +34797,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_36(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -36803,28 +36835,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -38993,15 +39025,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -39848,61 +39883,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -41182,15 +41235,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -41416,15 +41469,15 @@
                         } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
                             return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -41612,15 +41665,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -41846,15 +41899,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -42080,15 +42133,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -43214,15 +43267,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `fastavro-1.8.0/fastavro/_write.pyi` & `fastavro-1.8.1/fastavro/_write.pyi`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_write.pyx` & `fastavro-1.8.1/fastavro/_write.pyx`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_write_common.py` & `fastavro-1.8.1/fastavro/_write_common.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/_write_py.py` & `fastavro-1.8.1/fastavro/_write_py.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/const.py` & `fastavro-1.8.1/fastavro/const.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/io/binary_decoder.py` & `fastavro-1.8.1/fastavro/io/binary_decoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/io/binary_encoder.py` & `fastavro-1.8.1/fastavro/io/binary_encoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/io/json_decoder.py` & `fastavro-1.8.1/fastavro/io/json_decoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/io/json_encoder.py` & `fastavro-1.8.1/fastavro/io/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/io/parser.py` & `fastavro-1.8.1/fastavro/io/parser.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/io/symbols.py` & `fastavro-1.8.1/fastavro/io/symbols.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/json_read.py` & `fastavro-1.8.1/fastavro/json_read.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/json_write.py` & `fastavro-1.8.1/fastavro/json_write.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/read.py` & `fastavro-1.8.1/fastavro/read.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/repository/flat_dict.py` & `fastavro-1.8.1/fastavro/repository/flat_dict.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/schema.py` & `fastavro-1.8.1/fastavro/schema.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro/utils.py` & `fastavro-1.8.1/fastavro/utils.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/fastavro.egg-info/PKG-INFO` & `fastavro-1.8.1/fastavro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: fastavro
-Version: 1.8.0
+Version: 1.8.1
 Summary: Fast read/write of AVRO files
 Home-page: https://github.com/fastavro/fastavro
 Author: Miki Tebeka
 Author-email: miki.tebeka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: codecs
 Provides-Extra: snappy
 Provides-Extra: zstandard
 Provides-Extra: lz4
 License-File: LICENSE
 License-File: NOTICE.txt
@@ -48,15 +47,14 @@
 library. With regular CPython, `fastavro` uses C extensions which allow it to
 iterate the same 10,000 record file in 1.7 seconds. With PyPy, this drops to 1.5
 seconds (to be fair, the JAVA benchmark is doing some extra JSON
 encoding/decoding).
 
 `fastavro` supports the following Python versions:
 
-* Python 3.7
 * Python 3.8
 * Python 3.9
 * Python 3.10
 * Python 3.11
 * PyPy3
 
 ## Supported Features
```

### Comparing `fastavro-1.8.0/fastavro.egg-info/SOURCES.txt` & `fastavro-1.8.1/fastavro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/publish.sh` & `fastavro-1.8.1/publish.sh`

 * *Files 24% similar despite different names*

```diff
@@ -18,22 +18,14 @@
 OSes="win_amd64
 macosx_11_0_x86_64
 manylinux_2_17_x86_64.manylinux2014_x86_64
 manylinux_2_17_aarch64.manylinux2014_aarch64
 musllinux_1_1_x86_64
 musllinux_1_1_aarch64"
 
-PyVers="37"
-
-for os in $OSes; do
-    for pyver in $PyVers; do
-        wget -q --directory-prefix=dist/ https://github.com/fastavro/fastavro/releases/download/${ver}/fastavro-${ver}-cp${pyver}-cp${pyver}m-${os}.whl
-    done
-done
-
 PyVers="38
 39
 310
 311"
 
 for os in $OSes; do
     for pyver in $PyVers; do
```

### Comparing `fastavro-1.8.0/run-tests.cmd` & `fastavro-1.8.1/run-tests.cmd`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 del /S *.pyc
 del /S *.pyd
 
 if "%SKIP_BLACK%" == "1" (
 	echo "skipping black"
 ) else (
 	echo "running black"
-	black --target-version py36 --diff fastavro/ tests/ setup.py
-	black --target-version py36 --check fastavro/ tests/ setup.py
+	black --target-version py38 --diff fastavro/ tests/ setup.py
+	black --target-version py38 --check fastavro/ tests/ setup.py
 )
 
 echo "running flake8"
 flake8 --max-line-length=90 --extend-ignore=E203,E501 fastavro tests
 flake8 --config=.flake8.cython fastavro
 
 check-manifest
```

### Comparing `fastavro-1.8.0/run-tests.sh` & `fastavro-1.8.1/run-tests.sh`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 find . -name '*.pyc' -exec rm {} \;
 
 if [[ "$SKIP_BLACK" = "1" ]]; then
 	true
 else
 	echo "running black"
-	black --target-version py36 --diff fastavro/ tests/ setup.py
-	black --target-version py36 --check fastavro/ tests/ setup.py
+	black --target-version py38 --diff fastavro/ tests/ setup.py
+	black --target-version py38 --check fastavro/ tests/ setup.py
 fi
 
 echo "running flake8"
 flake8 --max-line-length=90 --extend-ignore=E203,E501 fastavro tests
 flake8 --config=.flake8.cython fastavro
 
 
@@ -38,11 +38,11 @@
 else
     echo "skipping mypy"
 fi
 
 check-manifest
 
 # Build Cython modules
-# python setup.py build_ext --inplace
-# pip install -e .
+python setup.py build_ext --inplace
+pip install -e .
 
 PYTHONPATH=${PWD} python -m pytest --cov=fastavro -v --cov-report=term-missing --cov-report=html:build/htmlcov $@
```

### Comparing `fastavro-1.8.0/setup.py` & `fastavro-1.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,27 +56,26 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries",
         "Topic :: Scientific/Engineering :: Information Analysis",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     extras_require={
         "codecs": ["python-snappy", "zstandard", "lz4"],
         "snappy": ["python-snappy"],
         "zstandard": ["zstandard"],
         "lz4": ["lz4"],
     },
     package_data={"fastavro": ["py.typed"]},
```

### Comparing `fastavro-1.8.0/tests/avro-files/deflate.avro` & `fastavro-1.8.1/tests/avro-files/deflate.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/java-generated-uuid.avro` & `fastavro-1.8.1/tests/avro-files/java-generated-uuid.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/null.avro` & `fastavro-1.8.1/tests/avro-files/null.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/snappy.avro` & `fastavro-1.8.1/tests/avro-files/snappy.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-deflate-0.avro` & `fastavro-1.8.1/tests/avro-files/test-deflate-0.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-deflate-1-A.avro` & `fastavro-1.8.1/tests/avro-files/test-deflate-1-A.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-deflate-1.avro` & `fastavro-1.8.1/tests/avro-files/test-deflate-1.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-deflate-3-A.avro` & `fastavro-1.8.1/tests/avro-files/test-deflate-3-A.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-deflate-6-B.avro` & `fastavro-1.8.1/tests/avro-files/test-deflate-6-B.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-deflate-9.avro` & `fastavro-1.8.1/tests/avro-files/test-deflate-9.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-null-B.avro` & `fastavro-1.8.1/tests/avro-files/test-null-B.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-null.avro` & `fastavro-1.8.1/tests/avro-files/test-null.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/test-snappy.avro` & `fastavro-1.8.1/tests/avro-files/test-snappy.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/weather-legacy-generated.avro` & `fastavro-1.8.1/tests/avro-files/weather-legacy-generated.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/avro-files/weather-legacy-with-names.avro` & `fastavro-1.8.1/tests/avro-files/weather-legacy-with-names.avro`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/conftest.py` & `fastavro-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/repository/test_flat_dict.py` & `fastavro-1.8.1/tests/repository/test_flat_dict.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_aliases.py` & `fastavro-1.8.1/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_appendable.py` & `fastavro-1.8.1/tests/test_appendable.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_block_reader.py` & `fastavro-1.8.1/tests/test_block_reader.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_canonical_form.py` & `fastavro-1.8.1/tests/test_canonical_form.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_complex.py` & `fastavro-1.8.1/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_compression.py` & `fastavro-1.8.1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_fastavro.py` & `fastavro-1.8.1/tests/test_fastavro.py`

 * *Files 0% similar despite different names*

```diff
@@ -1251,30 +1251,28 @@
         {"time": -(1 << 63)},
     ]
 
     assert records == roundtrip(schema, records)
 
 
 def test_py37_runtime_error():
-    """On Python 3.7 this test would cause the StopIteration to get raised as
+    """On Python 3.7+ this test would cause the StopIteration to get raised as
     a RuntimeError.
 
     See https://www.python.org/dev/peps/pep-0479/
     """
     weather_file = join(data_dir, "weather.avro")
 
     zip_io = BytesIO()
     with zipfile.ZipFile(zip_io, mode="w") as zio:
         zio.write(weather_file, arcname="weather")
 
     with zipfile.ZipFile(zip_io) as zio:
         with zio.open("weather") as fo:
-            # Need to read fo into a bytes buffer for python versions less
-            # than 3.7
-            reader = fastavro.reader(BytesIO(fo.read()))
+            reader = fastavro.reader(fo)
             list(reader)
 
 
 def test_eof_error():
     schema = {
         "type": "record",
         "name": "test_eof_error",
```

### Comparing `fastavro-1.8.0/tests/test_fingerprint.py` & `fastavro-1.8.1/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_json.py` & `fastavro-1.8.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_logical_types.py` & `fastavro-1.8.1/tests/test_logical_types.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_main_cli.py` & `fastavro-1.8.1/tests/test_main_cli.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_promotion.py` & `fastavro-1.8.1/tests/test_promotion.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_schema.py` & `fastavro-1.8.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_schema_evolution.py` & `fastavro-1.8.1/tests/test_schema_evolution.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_schemaless.py` & `fastavro-1.8.1/tests/test_schemaless.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_str_py3.py` & `fastavro-1.8.1/tests/test_str_py3.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_timezone.py` & `fastavro-1.8.1/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_types.py` & `fastavro-1.8.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_utils.py` & `fastavro-1.8.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_validation.py` & `fastavro-1.8.1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `fastavro-1.8.0/tests/test_write_block.py` & `fastavro-1.8.1/tests/test_write_block.py`

 * *Files identical despite different names*

