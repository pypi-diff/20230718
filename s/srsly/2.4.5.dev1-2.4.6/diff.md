# Comparing `tmp/srsly-2.4.5.dev1.tar.gz` & `tmp/srsly-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srsly-2.4.5.dev1.tar", last modified: Mon Oct 17 08:49:04 2022, max compression
+gzip compressed data, was "srsly-2.4.6.tar", last modified: Tue Feb 28 12:33:53 2023, max compression
```

## Comparing `srsly-2.4.5.dev1.tar` & `srsly-2.4.6.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.388756 srsly-2.4.5.dev1/
--rw-r--r--   0 vsts      (1001) docker     (121)     1103 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)    17421 2022-10-17 08:49:04.388756 srsly-2.4.5.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    16279 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     1654 2022-10-17 08:49:04.392756 srsly-2.4.5.dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     4309 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.376756 srsly-2.4.5.dev1/srsly/
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5599 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/_json_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/_msgpack_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)      631 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/_pickle_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3773 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/_yaml_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/about.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.376756 srsly-2.4.5.dev1/srsly/cloudpickle/
--rw-r--r--   0 vsts      (1001) docker     (121)      292 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/cloudpickle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    35137 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/cloudpickle/cloudpickle.py
--rw-r--r--   0 vsts      (1001) docker     (121)    34114 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 vsts      (1001) docker     (121)      508 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/cloudpickle/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.380756 srsly-2.4.5.dev1/srsly/msgpack/
--rw-r--r--   0 vsts      (1001) docker     (121)     2573 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      493 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/_ext_type.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2717 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/_msgpack_numpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)   408630 2022-10-17 08:49:03.000000 srsly-2.4.5.dev1/srsly/msgpack/_packer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13850 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/_packer.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)   414515 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly/msgpack/_unpacker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19218 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/_unpacker.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/_version.py
--rw-r--r--   0 vsts      (1001) docker     (121)      661 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/buff_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1081 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2628 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/pack.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20708 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/pack_template.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6464 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/sysdep.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8070 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/unpack.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2372 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/unpack_define.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14888 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/unpack_template.h
--rw-r--r--   0 vsts      (1001) docker     (121)      301 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/msgpack/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.380756 srsly-2.4.5.dev1/srsly/ruamel_yaml/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      104 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      501 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/anchor.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    35006 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/comments.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     8594 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/compat.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     8355 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/composer.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      351 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/configobjwalker.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    64802 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/constructor.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6567 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/cyaml.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6570 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/dumper.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    64676 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/emitter.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     9104 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/error.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3902 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/events.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2597 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/loader.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    53946 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/main.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3716 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/nodes.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    33818 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/parser.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    11177 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/reader.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    49193 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/representer.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    15456 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/resolver.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1520 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarbool.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4515 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarfloat.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4681 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarint.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4463 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarstring.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    72758 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/scanner.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     8531 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/serializer.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      939 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/timestamp.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     7471 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/tokens.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6098 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ruamel_yaml/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.384756 srsly-2.4.5.dev1/srsly/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.384756 srsly-2.4.5.dev1/srsly/tests/cloudpickle/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/cloudpickle/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3244 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/cloudpickle/cloudpickle_file_test.py
--rw-r--r--   0 vsts      (1001) docker     (121)   105620 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/cloudpickle/cloudpickle_test.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7466 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/cloudpickle/testutils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.384756 srsly-2.4.5.dev1/srsly/tests/msgpack/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      709 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_buffer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2846 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_case.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1682 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_except.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2575 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_extension.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2052 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_format.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3123 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_limits.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2581 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_memoryview.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2604 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_newspec.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8609 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_numpy.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4733 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_pack.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1800 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_read_size.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1125 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_seq.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3632 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_sequnpack.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1781 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_stricttype.py
--rw-r--r--   0 vsts      (1001) docker     (121)      375 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_subtype.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/msgpack/test_unpack.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.388756 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     9490 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/roundtrip.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1125 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_a_dedent.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5347 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_add_xxx.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    14428 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_anchor.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6980 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_api_change.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     7680 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_appliance.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3340 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_class_register.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      508 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_collections.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    14843 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_comment_manipulation.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    20299 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_comments.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2804 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_contextmanager.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3651 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_copy.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3787 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_datetime.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      353 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_deprecation.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1827 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_documents.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6290 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_fail.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2130 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_float.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      487 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_flowsequencekey.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     8512 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_indentation.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      907 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_int.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    23514 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_issues.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1452 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_json_numbers.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2106 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_line_col.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     7787 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_literal.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1428 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_none.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      488 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_numpy.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1869 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_program_config.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5880 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_spec_examples.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5603 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_string.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     3619 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_tag.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4343 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_version.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     5897 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_yamlfile.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2513 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_yamlobject.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      891 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_z_check_debug_leftovers.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     7319 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_z_data.py
--rw-r--r--   0 vsts      (1001) docker     (121)     6440 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/test_json_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3568 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/test_msgpack_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)      870 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/test_pickle_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3162 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/test_yaml_api.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.388756 srsly-2.4.5.dev1/srsly/tests/ujson/
--rw-r--r--   0 vsts      (1001) docker     (121)    29345 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ujson/334-reproducer.json
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ujson/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    33468 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/ujson/test_ujson.py
--rw-r--r--   0 vsts      (1001) docker     (121)      415 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.388756 srsly-2.4.5.dev1/srsly/ujson/
--rw-r--r--   0 vsts      (1001) docker     (121)     6361 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/JSONtoObj.c
--rw-r--r--   0 vsts      (1001) docker     (121)       74 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.388756 srsly-2.4.5.dev1/srsly/ujson/lib/
--rw-r--r--   0 vsts      (1001) docker     (121)     2038 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/lib/dconv_wrapper.cc
--rw-r--r--   0 vsts      (1001) docker     (121)     9792 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/lib/ultrajson.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21708 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/lib/ultrajsondec.c
--rw-r--r--   0 vsts      (1001) docker     (121)    26333 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/lib/ultrajsonenc.c
--rw-r--r--   0 vsts      (1001) docker     (121)    22961 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/objToJSON.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2365 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/py_defines.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4748 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/ujson.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1999 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/ujson/version.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1098 2022-10-17 08:48:49.000000 srsly-2.4.5.dev1/srsly/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-17 08:49:04.376756 srsly-2.4.5.dev1/srsly.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)    17421 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     4750 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      172 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       24 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-17 08:49:04.000000 srsly-2.4.5.dev1/srsly.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.900413 srsly-2.4.6/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1103 2023-02-28 12:33:43.000000 srsly-2.4.6/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       96 2023-02-28 12:33:43.000000 srsly-2.4.6/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    20009 2023-02-28 12:33:53.900413 srsly-2.4.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    18872 2023-02-28 12:33:43.000000 srsly-2.4.6/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-02-28 12:33:43.000000 srsly-2.4.6/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1654 2023-02-28 12:33:53.904413 srsly-2.4.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     4309 2023-02-28 12:33:43.000000 srsly-2.4.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.884413 srsly-2.4.6/srsly/
+-rw-r--r--   0 vsts      (1001) docker     (122)      591 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7068 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/_json_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1855 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/_msgpack_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      631 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/_pickle_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3773 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/_yaml_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/about.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.884413 srsly-2.4.6/srsly/cloudpickle/
+-rw-r--r--   0 vsts      (1001) docker     (122)      292 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/cloudpickle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35137 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/cloudpickle/cloudpickle.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34114 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      508 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/cloudpickle/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.888413 srsly-2.4.6/srsly/msgpack/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2573 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      493 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/_ext_type.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2717 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/_msgpack_numpy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   408600 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly/msgpack/_packer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    13850 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/_packer.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)   414516 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly/msgpack/_unpacker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)    19218 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/_unpacker.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)       20 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/buff_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1081 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2628 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/pack.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20708 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/pack_template.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6464 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/sysdep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8070 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/unpack.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2372 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/unpack_define.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    14888 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/unpack_template.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      301 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/msgpack/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.892413 srsly-2.4.6/srsly/ruamel_yaml/
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      104 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      501 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/anchor.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    35006 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/comments.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     8594 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/compat.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     8355 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/composer.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      351 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/configobjwalker.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    64802 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/constructor.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6567 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/cyaml.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6570 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/dumper.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    64676 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/emitter.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     9104 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/error.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3902 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/events.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2597 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/loader.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    53946 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/main.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3716 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/nodes.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    33818 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/parser.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    11177 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/reader.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    49193 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/representer.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    15456 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/resolver.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1520 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/scalarbool.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4515 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/scalarfloat.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4681 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/scalarint.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4463 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/scalarstring.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    72758 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/scanner.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     8531 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/serializer.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      939 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/timestamp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     7471 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/tokens.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6098 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ruamel_yaml/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.892413 srsly-2.4.6/srsly/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.892413 srsly-2.4.6/srsly/tests/cloudpickle/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/cloudpickle/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3244 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/cloudpickle/cloudpickle_file_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   106164 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/cloudpickle/cloudpickle_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7466 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/cloudpickle/testutils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.896413 srsly-2.4.6/srsly/tests/msgpack/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      709 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_buffer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2846 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_case.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_except.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2575 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_extension.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2052 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_format.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3123 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_limits.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2581 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_memoryview.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_newspec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8609 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_numpy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4733 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_pack.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1800 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_read_size.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1125 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_seq.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3632 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_sequnpack.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1781 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_stricttype.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      375 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_subtype.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1820 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/msgpack/test_unpack.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.900413 srsly-2.4.6/srsly/tests/ruamel_yaml/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     9490 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/roundtrip.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1125 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_a_dedent.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5347 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_add_xxx.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    14428 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_anchor.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6980 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_api_change.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     7680 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_appliance.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3340 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_class_register.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      508 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_collections.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    14843 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_comment_manipulation.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    20299 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_comments.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2804 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_contextmanager.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3651 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_copy.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3787 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_datetime.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      353 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_deprecation.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1827 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_documents.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6290 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_fail.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2130 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_float.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      487 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_flowsequencekey.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     8512 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_indentation.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      907 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_int.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)    23514 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_issues.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1452 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_json_numbers.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2106 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_line_col.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     7787 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_literal.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1428 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_none.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      488 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_numpy.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1869 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_program_config.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5880 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_spec_examples.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5603 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_string.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3619 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_tag.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     4343 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_version.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5897 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_yamlfile.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2513 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_yamlobject.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      891 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_z_check_debug_leftovers.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     7319 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ruamel_yaml/test_z_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8291 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/test_json_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3568 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/test_msgpack_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/test_pickle_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3162 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/test_yaml_api.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.900413 srsly-2.4.6/srsly/tests/ujson/
+-rw-r--r--   0 vsts      (1001) docker     (122)    29345 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ujson/334-reproducer.json
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ujson/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    33468 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/ujson/test_ujson.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      415 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.900413 srsly-2.4.6/srsly/ujson/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6361 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/JSONtoObj.c
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.900413 srsly-2.4.6/srsly/ujson/lib/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2038 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/lib/dconv_wrapper.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9792 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/lib/ultrajson.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    21708 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/lib/ultrajsondec.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    26333 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/lib/ultrajsonenc.c
+-rw-r--r--   0 vsts      (1001) docker     (122)    22961 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/objToJSON.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     2365 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/py_defines.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4748 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/ujson.c
+-rw-r--r--   0 vsts      (1001) docker     (122)     1999 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/ujson/version.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1108 2023-02-28 12:33:43.000000 srsly-2.4.6/srsly/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-28 12:33:53.884413 srsly-2.4.6/srsly.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20009 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4750 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      172 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-28 12:33:53.000000 srsly-2.4.6/srsly.egg-info/zip-safe
```

### Comparing `srsly-2.4.5.dev1/LICENSE` & `srsly-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/PKG-INFO` & `srsly-2.4.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: srsly
-Version: 2.4.5.dev1
-Summary: Modern high-performance serialization utilities for Python
-Home-page: https://github.com/explosion/srsly
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # srsly: Modern high-performance serialization utilities for Python
 
 This package bundles some of the best Python serialization libraries into one
 standalone package, with a high-level API that makes it easy to write code
 that's correct across platforms and Pythons. This allows us to provide all the
@@ -43,15 +14,15 @@
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
 
 ## Motivation
 
 Serialization is hard, especially across Python versions and multiple platforms.
 After dealing with many subtle bugs over the years (encodings, locales, large
 files) our libraries like [spaCy](https://github.com/explosion/spaCy) and
-[Prodigy](https://prodi.gy) have steadily grown a number of utility functions to
+[Prodigy](https://prodi.gy) had steadily grown a number of utility functions to
 wrap the multiple serialization formats we need to support (especially `json`,
 `msgpack` and `pickle`). These wrapping functions ended up duplicated across our
 codebases, so we wanted to put them in one place.
 
 At the same time, we noticed that having a lot of small dependencies was making
 maintenance harder, and making installation slower. To solve this, we've made
 `srsly` standalone, by including the component packages directly within it. This
@@ -70,32 +41,57 @@
 
 > ⚠️ Note that `v2.x` is only compatible with **Python 3.6+**. For 2.7+ compatibility, use `v1.x`.
 
 `srsly` can be installed from pip. Before installing, make sure that your `pip`,
 `setuptools` and `wheel` are up to date.
 
 ```bash
-pip install -U pip setuptools wheel
-pip install srsly
+python -m pip install -U pip setuptools wheel
+python -m pip install srsly
 ```
 
 Or from conda via conda-forge:
 
 ```bash
 conda install -c conda-forge srsly
 ```
 
 Alternatively, you can also compile the library from source. You'll need to make
-sure that you have a development environment consisting of a Python distribution
+sure that you have a development environment with a Python distribution
 including header files, a compiler (XCode command-line tools on macOS / OS X or
-Visual C++ build tools on Windows), pip, virtualenv and git installed.
+Visual C++ build tools on Windows), pip and git installed.
+
+Install from source:
+
+```bash
+# clone the repo
+git clone https://github.com/explosion/srsly
+cd srsly
+
+# create a virtual environment
+python -m venv .env
+source .env/bin/activate
+
+# update pip
+python -m pip install -U pip setuptools wheel
+
+# compile and install from source
+python -m pip install .
+```
+
+For developers, install requirements separately and then install in editable
+mode without build isolation:
 
 ```bash
-pip install -r requirements.txt  # install development dependencies
-python setup.py build_ext --inplace  # compile the library
+# install in editable mode
+python -m pip install -r requirements.txt
+python -m pip install --no-build-isolation --editable .
+
+# run test suite
+python -m pytest --pyargs srsly
 ```
 
 ## API
 
 ### JSON
 
 > 📦 The underlying module is exposed via `srsly.ujson`. However, we normally
@@ -136,74 +132,103 @@
 Create a JSON file and dump contents or write to standard output.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_json("/path/to/file.json", data)
 ```
 
-| Argument   | Type         | Description                                            |
-| ---------- | ------------ | ------------------------------------------------------ |
-| `path` | str / `Path` | The file path or `"-"` to write to stdout.             |
-| `data`     | -            | The JSON-serializable data to output.                  |
-| `indent`   | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+| Argument | Type         | Description                                            |
+| -------- | ------------ | ------------------------------------------------------ |
+| `path`   | str / `Path` | The file path or `"-"` to write to stdout.             |
+| `data`   | -            | The JSON-serializable data to output.                  |
+| `indent` | int          | Number of spaces used to indent JSON. Defaults to `2`. |
 
 #### <kbd>function</kbd> `srsly.read_json`
 
 Load JSON from a file or standard input.
 
 ```python
 data = srsly.read_json("/path/to/file.json")
 ```
 
 | Argument    | Type         | Description                                |
 | ----------- | ------------ | ------------------------------------------ |
-| `path`  | str / `Path` | The file path or `"-"` to read from stdin. |
+| `path`      | str / `Path` | The file path or `"-"` to read from stdin. |
 | **RETURNS** | dict / list  | The loaded JSON content.                   |
 
 #### <kbd>function</kbd> `srsly.write_gzip_json`
 
 Create a gzipped JSON file and dump contents.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_gzip_json("/path/to/file.json.gz", data)
 ```
 
-| Argument   | Type         | Description                                            |
-| ---------- | ------------ | ------------------------------------------------------ |
-| `path` | str / `Path` | The file path.                                         |
-| `data`     | -            | The JSON-serializable data to output.                  |
-| `indent`   | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+| Argument | Type         | Description                                            |
+| -------- | ------------ | ------------------------------------------------------ |
+| `path`   | str / `Path` | The file path.                                         |
+| `data`   | -            | The JSON-serializable data to output.                  |
+| `indent` | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+
+#### <kbd>function</kbd> `srsly.write_gzip_jsonl`
+
+Create a gzipped JSONL file and dump contents.
+
+```python
+data = [{"foo": "bar"}, {"baz": 123}]
+srsly.write_gzip_json("/path/to/file.jsonl.gz", data)
+```
+
+| Argument          | Type         | Description                                                                                                                                                                                                             |
+| ----------------- | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `path`            | str / `Path` | The file path.                                                                                                                                                                                                          |
+| `lines`           | -            | The JSON-serializable contents of each line.                                                                                                                                                                            |
+| `append`          | bool         | Whether or not to append to the location. Appending to .gz files is generally not recommended, as it doesn't allow the algorithm to take advantage of all data when compressing - files may hence be poorly compressed. |
+| `append_new_line` | bool         | Whether or not to write a new line before appending to the file.                                                                                                                                                        |
 
 #### <kbd>function</kbd> `srsly.read_gzip_json`
 
 Load gzipped JSON from a file.
 
 ```python
 data = srsly.read_gzip_json("/path/to/file.json.gz")
 ```
 
 | Argument    | Type         | Description              |
 | ----------- | ------------ | ------------------------ |
-| `path`  | str / `Path` | The file path.           |
+| `path`      | str / `Path` | The file path.           |
 | **RETURNS** | dict / list  | The loaded JSON content. |
 
+#### <kbd>function</kbd> `srsly.read_gzip_jsonl`
+
+Load gzipped JSONL from a file.
+
+```python
+data = srsly.read_gzip_jsonl("/path/to/file.jsonl.gz")
+```
+
+| Argument    | Type         | Description               |
+| ----------- | ------------ | ------------------------- |
+| `path`      | str / `Path` | The file path.            |
+| **RETURNS** | dict / list  | The loaded JSONL content. |
+
 #### <kbd>function</kbd> `srsly.write_jsonl`
 
 Create a JSONL file (newline-delimited JSON) and dump contents line by line, or
 write to standard output.
 
 ```python
 data = [{"foo": "bar"}, {"baz": 123}]
 srsly.write_jsonl("/path/to/file.jsonl", data)
 ```
 
 | Argument          | Type         | Description                                                                                                            |
 | ----------------- | ------------ | ---------------------------------------------------------------------------------------------------------------------- |
-| `path`        | str / `Path` | The file path or `"-"` to write to stdout.                                                                             |
+| `path`            | str / `Path` | The file path or `"-"` to write to stdout.                                                                             |
 | `lines`           | iterable     | The JSON-serializable lines.                                                                                           |
 | `append`          | bool         | Append to an existing file. Will open it in `"a"` mode and insert a newline before writing lines. Defaults to `False`. |
 | `append_new_line` | bool         | Defines whether a new line should first be written when appending to an existing file. Defaults to `True`.             |
 
 #### <kbd>function</kbd> `srsly.read_jsonl`
 
 Read a JSONL file (newline-delimited JSON) or from JSONL data from standard
@@ -211,15 +236,15 @@
 
 ```python
 data = srsly.read_jsonl("/path/to/file.jsonl")
 ```
 
 | Argument   | Type       | Description                                                          |
 | ---------- | ---------- | -------------------------------------------------------------------- |
-| `path` | str / Path | The file path or `"-"` to read from stdin.                           |
+| `path`     | str / Path | The file path or `"-"` to read from stdin.                           |
 | `skip`     | bool       | Skip broken lines and don't raise `ValueError`. Defaults to `False`. |
 | **YIELDS** | -          | The loaded JSON contents of each line.                               |
 
 #### <kbd>function</kbd> `srsly.is_json_serializable`
 
 Check if a Python object is JSON-serializable.
 
@@ -272,30 +297,30 @@
 Create a msgpack file and dump contents.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_msgpack("/path/to/file.msg", data)
 ```
 
-| Argument   | Type         | Description            |
-| ---------- | ------------ | ---------------------- |
-| `path` | str / `Path` | The file path.         |
-| `data`     | -            | The data to serialize. |
+| Argument | Type         | Description            |
+| -------- | ------------ | ---------------------- |
+| `path`   | str / `Path` | The file path.         |
+| `data`   | -            | The data to serialize. |
 
 #### <kbd>function</kbd> `srsly.read_msgpack`
 
 Load a msgpack file.
 
 ```python
 data = srsly.read_msgpack("/path/to/file.msg")
 ```
 
 | Argument    | Type         | Description                                                                             |
 | ----------- | ------------ | --------------------------------------------------------------------------------------- |
-| `path`  | str / `Path` | The file path.                                                                          |
+| `path`      | str / `Path` | The file path.                                                                          |
 | `use_list`  | bool         | Don't use tuples instead of lists. Can make deserialization slower. Defaults to `True`. |
 | **RETURNS** | -            | The loaded and deserialized content.                                                    |
 
 ### pickle
 
 > 📦 The underlying module is exposed via `srsly.cloudpickle`. However, we
 > normally interact with it via the utility functions only.
@@ -343,15 +368,15 @@
 yaml_string = srsly.yaml_dumps(data)
 ```
 
 | Argument          | Type | Description                                |
 | ----------------- | ---- | ------------------------------------------ |
 | `data`            | -    | The JSON-serializable data to output.      |
 | `indent_mapping`  | int  | Mapping indentation. Defaults to `2`.      |
-| `indent_sequence` | int  | Sequence indentation. Defaults to `4`.      |
+| `indent_sequence` | int  | Sequence indentation. Defaults to `4`.     |
 | `indent_offset`   | int  | Indentation offset. Defaults to `2`.       |
 | `sort_keys`       | bool | Sort dictionary keys. Defaults to `False`. |
 | **RETURNS**       | str  | The serialized string.                     |
 
 #### <kbd>function</kbd> `srsly.yaml_loads`
 
 Deserialize unicode or a file object to a Python object.
@@ -373,32 +398,32 @@
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_yaml("/path/to/file.yml", data)
 ```
 
 | Argument          | Type         | Description                                |
 | ----------------- | ------------ | ------------------------------------------ |
-| `path`        | str / `Path` | The file path or `"-"` to write to stdout. |
+| `path`            | str / `Path` | The file path or `"-"` to write to stdout. |
 | `data`            | -            | The JSON-serializable data to output.      |
 | `indent_mapping`  | int          | Mapping indentation. Defaults to `2`.      |
-| `indent_sequence` | int          | Sequence indentation. Defaults to `4`.      |
+| `indent_sequence` | int          | Sequence indentation. Defaults to `4`.     |
 | `indent_offset`   | int          | Indentation offset. Defaults to `2`.       |
 | `sort_keys`       | bool         | Sort dictionary keys. Defaults to `False`. |
 
 #### <kbd>function</kbd> `srsly.read_yaml`
 
 Load YAML from a file or standard input.
 
 ```python
 data = srsly.read_yaml("/path/to/file.yml")
 ```
 
 | Argument    | Type         | Description                                |
 | ----------- | ------------ | ------------------------------------------ |
-| `path`  | str / `Path` | The file path or `"-"` to read from stdin. |
+| `path`      | str / `Path` | The file path or `"-"` to read from stdin. |
 | **RETURNS** | dict / list  | The loaded YAML content.                   |
 
 #### <kbd>function</kbd> `srsly.is_yaml_serializable`
 
 Check if a Python object is YAML-serializable.
 
 ```python
```

#### html2text {}

```diff
@@ -1,122 +1,130 @@
-Metadata-Version: 2.1 Name: srsly Version: 2.4.5.dev1 Summary: Modern high-
-performance serialization utilities for Python Home-page: https://github.com/
-explosion/srsly Author: Explosion Author-email: contact@explosion.ai License:
-MIT Classifier: Development Status :: 5 - Production/Stable Classifier:
-Environment :: Console Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Classifier: Programming Language :: Cython Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE [https://explosion.ai/assets/img/logo.svg] # srsly: Modern high-
-performance serialization utilities for Python This package bundles some of the
-best Python serialization libraries into one standalone package, with a high-
-level API that makes it easy to write code that's correct across platforms and
-Pythons. This allows us to provide all the serialization utilities we need in a
-single binary wheel. Currently supports **JSON**, **JSONL**, **MessagePack**,
-**Pickle** and **YAML**. [![Azure Pipelines](https://img.shields.io/azure-
-devops/build/explosion-ai/public/4/master.svg?logo=azure-pipelines&style=flat-
-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=4) [!
-[PyPi](https://img.shields.io/pypi/v/srsly.svg?style=flat-
+[https://explosion.ai/assets/img/logo.svg] # srsly: Modern high-performance
+serialization utilities for Python This package bundles some of the best Python
+serialization libraries into one standalone package, with a high-level API that
+makes it easy to write code that's correct across platforms and Pythons. This
+allows us to provide all the serialization utilities we need in a single binary
+wheel. Currently supports **JSON**, **JSONL**, **MessagePack**, **Pickle** and
+**YAML**. [![Azure Pipelines](https://img.shields.io/azure-devops/build/
+explosion-ai/public/4/master.svg?logo=azure-pipelines&style=flat-square)]
+(https://dev.azure.com/explosion-ai/public/_build?definitionId=4) [![PyPi]
+(https://img.shields.io/pypi/v/srsly.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/srsly) [!
 [conda](https://img.shields.io/conda/vn/conda-forge/srsly.svg?style=flat-
 square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/
 srsly) [![GitHub](https://img.shields.io/github/release/explosion/srsly/
 all.svg?style=flat-square&logo=github)](https://github.com/explosion/srsly) [!
 [Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
 4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://
 github.com/explosion/wheelwright/releases) ## Motivation Serialization is hard,
 especially across Python versions and multiple platforms. After dealing with
 many subtle bugs over the years (encodings, locales, large files) our libraries
 like [spaCy](https://github.com/explosion/spaCy) and [Prodigy](https://
-prodi.gy) have steadily grown a number of utility functions to wrap the
-multiple serialization formats we need to support (especially `json`, `msgpack`
-and `pickle`). These wrapping functions ended up duplicated across our
-codebases, so we wanted to put them in one place. At the same time, we noticed
-that having a lot of small dependencies was making maintenance harder, and
-making installation slower. To solve this, we've made `srsly` standalone, by
-including the component packages directly within it. This way we can provide
-all the serialization utilities we need in a single binary wheel. `srsly`
-currently includes forks of the following packages: - [`ujson`](https://
-github.com/esnme/ultrajson) - [`msgpack`](https://github.com/msgpack/msgpack-
-python) - [`msgpack-numpy`](https://github.com/lebedov/msgpack-numpy) -
-[`cloudpickle`](https://github.com/cloudpipe/cloudpickle) - [`ruamel.yaml`]
-(https://github.com/pycontribs/ruamel-yaml) (without unsafe implementations!)
-## Installation > â ï¸ Note that `v2.x` is only compatible with **Python
-3.6+**. For 2.7+ compatibility, use `v1.x`. `srsly` can be installed from pip.
-Before installing, make sure that your `pip`, `setuptools` and `wheel` are up
-to date. ```bash pip install -U pip setuptools wheel pip install srsly ``` Or
-from conda via conda-forge: ```bash conda install -c conda-forge srsly ```
-Alternatively, you can also compile the library from source. You'll need to
-make sure that you have a development environment consisting of a Python
+prodi.gy) had steadily grown a number of utility functions to wrap the multiple
+serialization formats we need to support (especially `json`, `msgpack` and
+`pickle`). These wrapping functions ended up duplicated across our codebases,
+so we wanted to put them in one place. At the same time, we noticed that having
+a lot of small dependencies was making maintenance harder, and making
+installation slower. To solve this, we've made `srsly` standalone, by including
+the component packages directly within it. This way we can provide all the
+serialization utilities we need in a single binary wheel. `srsly` currently
+includes forks of the following packages: - [`ujson`](https://github.com/esnme/
+ultrajson) - [`msgpack`](https://github.com/msgpack/msgpack-python) -
+[`msgpack-numpy`](https://github.com/lebedov/msgpack-numpy) - [`cloudpickle`]
+(https://github.com/cloudpipe/cloudpickle) - [`ruamel.yaml`](https://
+github.com/pycontribs/ruamel-yaml) (without unsafe implementations!) ##
+Installation > â ï¸ Note that `v2.x` is only compatible with **Python 3.6+**.
+For 2.7+ compatibility, use `v1.x`. `srsly` can be installed from pip. Before
+installing, make sure that your `pip`, `setuptools` and `wheel` are up to date.
+```bash python -m pip install -U pip setuptools wheel python -m pip install
+srsly ``` Or from conda via conda-forge: ```bash conda install -c conda-forge
+srsly ``` Alternatively, you can also compile the library from source. You'll
+need to make sure that you have a development environment with a Python
 distribution including header files, a compiler (XCode command-line tools on
-macOS / OS X or Visual C++ build tools on Windows), pip, virtualenv and git
-installed. ```bash pip install -r requirements.txt # install development
-dependencies python setup.py build_ext --inplace # compile the library ``` ##
-API ### JSON > ð¦ The underlying module is exposed via `srsly.ujson`.
-However, we normally > interact with it via the utility functions only. ####
-function `srsly.json_dumps` Serialize an object to a JSON string. Falls back to
-`json` if `sort_keys=True` is used (until it's fixed in `ujson`). ```python
-data = {"foo": "bar", "baz": 123} json_string = srsly.json_dumps(data) ``` |
-Argument | Type | Description | | ----------- | ---- | ------------------------
------------------------------- | | `data` | - | The JSON-serializable data to
-output. | | `indent` | int | Number of spaces used to indent JSON. Defaults to
-`0`. | | `sort_keys` | bool | Sort dictionary keys. Defaults to `False`. | |
-**RETURNS** | str | The serialized string. | #### function `srsly.json_loads`
-Deserialize unicode or bytes to a Python object. ```python data = '{"foo":
-"bar", "baz": 123}' obj = srsly.json_loads(data) ``` | Argument | Type |
-Description | | ----------- | ----------- | ------------------------------- | |
-`data` | str / bytes | The data to deserialize. | | **RETURNS** | - | The
-deserialized Python object. | #### function `srsly.write_json` Create a JSON
-file and dump contents or write to standard output. ```python data = {"foo":
-"bar", "baz": 123} srsly.write_json("/path/to/file.json", data) ``` | Argument
-| Type | Description | | ---------- | ------------ | --------------------------
----------------------------- | | `path` | str / `Path` | The file path or `"-"`
-to write to stdout. | | `data` | - | The JSON-serializable data to output. | |
-`indent` | int | Number of spaces used to indent JSON. Defaults to `2`. | ####
-function `srsly.read_json` Load JSON from a file or standard input. ```python
-data = srsly.read_json("/path/to/file.json") ``` | Argument | Type |
-Description | | ----------- | ------------ | ----------------------------------
--------- | | `path` | str / `Path` | The file path or `"-"` to read from stdin.
-| | **RETURNS** | dict / list | The loaded JSON content. | #### function
+macOS / OS X or Visual C++ build tools on Windows), pip and git installed.
+Install from source: ```bash # clone the repo git clone https://github.com/
+explosion/srsly cd srsly # create a virtual environment python -m venv .env
+source .env/bin/activate # update pip python -m pip install -U pip setuptools
+wheel # compile and install from source python -m pip install . ``` For
+developers, install requirements separately and then install in editable mode
+without build isolation: ```bash # install in editable mode python -m pip
+install -r requirements.txt python -m pip install --no-build-isolation --
+editable . # run test suite python -m pytest --pyargs srsly ``` ## API ### JSON
+> ð¦ The underlying module is exposed via `srsly.ujson`. However, we normally
+> interact with it via the utility functions only. #### function
+`srsly.json_dumps` Serialize an object to a JSON string. Falls back to `json`
+if `sort_keys=True` is used (until it's fixed in `ujson`). ```python data =
+{"foo": "bar", "baz": 123} json_string = srsly.json_dumps(data) ``` | Argument
+| Type | Description | | ----------- | ---- | ---------------------------------
+--------------------- | | `data` | - | The JSON-serializable data to output. |
+| `indent` | int | Number of spaces used to indent JSON. Defaults to `0`. | |
+`sort_keys` | bool | Sort dictionary keys. Defaults to `False`. | | **RETURNS**
+| str | The serialized string. | #### function `srsly.json_loads` Deserialize
+unicode or bytes to a Python object. ```python data = '{"foo": "bar", "baz":
+123}' obj = srsly.json_loads(data) ``` | Argument | Type | Description | | ----
+------- | ----------- | ------------------------------- | | `data` | str /
+bytes | The data to deserialize. | | **RETURNS** | - | The deserialized Python
+object. | #### function `srsly.write_json` Create a JSON file and dump contents
+or write to standard output. ```python data = {"foo": "bar", "baz": 123}
+srsly.write_json("/path/to/file.json", data) ``` | Argument | Type |
+Description | | -------- | ------------ | -------------------------------------
+----------------- | | `path` | str / `Path` | The file path or `"-"` to write
+to stdout. | | `data` | - | The JSON-serializable data to output. | | `indent`
+| int | Number of spaces used to indent JSON. Defaults to `2`. | #### function
+`srsly.read_json` Load JSON from a file or standard input. ```python data =
+srsly.read_json("/path/to/file.json") ``` | Argument | Type | Description | | -
+---------- | ------------ | ------------------------------------------ | |
+`path` | str / `Path` | The file path or `"-"` to read from stdin. | |
+**RETURNS** | dict / list | The loaded JSON content. | #### function
 `srsly.write_gzip_json` Create a gzipped JSON file and dump contents. ```python
 data = {"foo": "bar", "baz": 123} srsly.write_gzip_json("/path/to/
-file.json.gz", data) ``` | Argument | Type | Description | | ---------- | -----
-------- | ------------------------------------------------------ | | `path` |
-str / `Path` | The file path. | | `data` | - | The JSON-serializable data to
+file.json.gz", data) ``` | Argument | Type | Description | | -------- | -------
+----- | ------------------------------------------------------ | | `path` | str
+/ `Path` | The file path. | | `data` | - | The JSON-serializable data to
 output. | | `indent` | int | Number of spaces used to indent JSON. Defaults to
-`2`. | #### function `srsly.read_gzip_json` Load gzipped JSON from a file.
-```python data = srsly.read_gzip_json("/path/to/file.json.gz") ``` | Argument |
-Type | Description | | ----------- | ------------ | ------------------------ |
-| `path` | str / `Path` | The file path. | | **RETURNS** | dict / list | The
-loaded JSON content. | #### function `srsly.write_jsonl` Create a JSONL file
-(newline-delimited JSON) and dump contents line by line, or write to standard
-output. ```python data = [{"foo": "bar"}, {"baz": 123}] srsly.write_jsonl("/
-path/to/file.jsonl", data) ``` | Argument | Type | Description | | ------------
------ | ------------ | --------------------------------------------------------
--------------------------------------------------------------- | | `path` | str
-/ `Path` | The file path or `"-"` to write to stdout. | | `lines` | iterable |
-The JSON-serializable lines. | | `append` | bool | Append to an existing file.
-Will open it in `"a"` mode and insert a newline before writing lines. Defaults
-to `False`. | | `append_new_line` | bool | Defines whether a new line should
-first be written when appending to an existing file. Defaults to `True`. | ####
-function `srsly.read_jsonl` Read a JSONL file (newline-delimited JSON) or from
-JSONL data from standard input and yield contents line by line. Blank lines
-will always be skipped. ```python data = srsly.read_jsonl("/path/to/
-file.jsonl") ``` | Argument | Type | Description | | ---------- | ---------- |
--------------------------------------------------------------------- | | `path`
-| str / Path | The file path or `"-"` to read from stdin. | | `skip` | bool |
-Skip broken lines and don't raise `ValueError`. Defaults to `False`. | |
-**YIELDS** | - | The loaded JSON contents of each line. | #### function
+`2`. | #### function `srsly.write_gzip_jsonl` Create a gzipped JSONL file and
+dump contents. ```python data = [{"foo": "bar"}, {"baz": 123}]
+srsly.write_gzip_json("/path/to/file.jsonl.gz", data) ``` | Argument | Type |
+Description | | ----------------- | ------------ | ----------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+----------------------------- | | `path` | str / `Path` | The file path. | |
+`lines` | - | The JSON-serializable contents of each line. | | `append` | bool
+| Whether or not to append to the location. Appending to .gz files is generally
+not recommended, as it doesn't allow the algorithm to take advantage of all
+data when compressing - files may hence be poorly compressed. | |
+`append_new_line` | bool | Whether or not to write a new line before appending
+to the file. | #### function `srsly.read_gzip_json` Load gzipped JSON from a
+file. ```python data = srsly.read_gzip_json("/path/to/file.json.gz") ``` |
+Argument | Type | Description | | ----------- | ------------ | ----------------
+-------- | | `path` | str / `Path` | The file path. | | **RETURNS** | dict /
+list | The loaded JSON content. | #### function `srsly.read_gzip_jsonl` Load
+gzipped JSONL from a file. ```python data = srsly.read_gzip_jsonl("/path/to/
+file.jsonl.gz") ``` | Argument | Type | Description | | ----------- | ---------
+--- | ------------------------- | | `path` | str / `Path` | The file path. | |
+**RETURNS** | dict / list | The loaded JSONL content. | #### function
+`srsly.write_jsonl` Create a JSONL file (newline-delimited JSON) and dump
+contents line by line, or write to standard output. ```python data = [{"foo":
+"bar"}, {"baz": 123}] srsly.write_jsonl("/path/to/file.jsonl", data) ``` |
+Argument | Type | Description | | ----------------- | ------------ | ----------
+-------------------------------------------------------------------------------
+----------------------------- | | `path` | str / `Path` | The file path or `"-
+"` to write to stdout. | | `lines` | iterable | The JSON-serializable lines. |
+| `append` | bool | Append to an existing file. Will open it in `"a"` mode and
+insert a newline before writing lines. Defaults to `False`. | |
+`append_new_line` | bool | Defines whether a new line should first be written
+when appending to an existing file. Defaults to `True`. | #### function
+`srsly.read_jsonl` Read a JSONL file (newline-delimited JSON) or from JSONL
+data from standard input and yield contents line by line. Blank lines will
+always be skipped. ```python data = srsly.read_jsonl("/path/to/file.jsonl") ```
+| Argument | Type | Description | | ---------- | ---------- | -----------------
+--------------------------------------------------- | | `path` | str / Path |
+The file path or `"-"` to read from stdin. | | `skip` | bool | Skip broken
+lines and don't raise `ValueError`. Defaults to `False`. | | **YIELDS** | - |
+The loaded JSON contents of each line. | #### function
 `srsly.is_json_serializable` Check if a Python object is JSON-serializable.
 ```python assert srsly.is_json_serializable({"hello": "world"}) is True assert
 srsly.is_json_serializable(lambda x: x) is False ``` | Argument | Type |
 Description | | ----------- | ---- | ---------------------------------------- |
 | `obj` | - | The object to check. | | **RETURNS** | bool | Whether the object
 is JSON-serializable. | ### msgpack > ð¦ The underlying module is exposed via
 `srsly.msgpack`. However, we normally > interact with it via the utility
@@ -130,16 +138,16 @@
 Argument | Type | Description | | ----------- | ----- | -----------------------
 ---------------------------------------------------------------- | | `data` |
 bytes | The data to deserialize. | | `use_list` | bool | Don't use tuples
 instead of lists. Can make deserialization slower. Defaults to `True`. | |
 **RETURNS** | - | The deserialized Python object. | #### function
 `srsly.write_msgpack` Create a msgpack file and dump contents. ```python data =
 {"foo": "bar", "baz": 123} srsly.write_msgpack("/path/to/file.msg", data) ``` |
-Argument | Type | Description | | ---------- | ------------ | -----------------
------ | | `path` | str / `Path` | The file path. | | `data` | - | The data to
+Argument | Type | Description | | -------- | ------------ | -------------------
+--- | | `path` | str / `Path` | The file path. | | `data` | - | The data to
 serialize. | #### function `srsly.read_msgpack` Load a msgpack file. ```python
 data = srsly.read_msgpack("/path/to/file.msg") ``` | Argument | Type |
 Description | | ----------- | ------------ | ----------------------------------
 ----------------------------------------------------- | | `path` | str / `Path`
 | The file path. | | `use_list` | bool | Don't use tuples instead of lists. Can
 make deserialization slower. Defaults to `True`. | | **RETURNS** | - | The
 loaded and deserialized content. | ### pickle > ð¦ The underlying module is
```

### Comparing `srsly-2.4.5.dev1/README.md` & `srsly-2.4.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: srsly
+Version: 2.4.6
+Summary: Modern high-performance serialization utilities for Python
+Home-page: https://github.com/explosion/srsly
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # srsly: Modern high-performance serialization utilities for Python
 
 This package bundles some of the best Python serialization libraries into one
 standalone package, with a high-level API that makes it easy to write code
 that's correct across platforms and Pythons. This allows us to provide all the
@@ -14,15 +43,15 @@
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
 
 ## Motivation
 
 Serialization is hard, especially across Python versions and multiple platforms.
 After dealing with many subtle bugs over the years (encodings, locales, large
 files) our libraries like [spaCy](https://github.com/explosion/spaCy) and
-[Prodigy](https://prodi.gy) have steadily grown a number of utility functions to
+[Prodigy](https://prodi.gy) had steadily grown a number of utility functions to
 wrap the multiple serialization formats we need to support (especially `json`,
 `msgpack` and `pickle`). These wrapping functions ended up duplicated across our
 codebases, so we wanted to put them in one place.
 
 At the same time, we noticed that having a lot of small dependencies was making
 maintenance harder, and making installation slower. To solve this, we've made
 `srsly` standalone, by including the component packages directly within it. This
@@ -41,32 +70,57 @@
 
 > ⚠️ Note that `v2.x` is only compatible with **Python 3.6+**. For 2.7+ compatibility, use `v1.x`.
 
 `srsly` can be installed from pip. Before installing, make sure that your `pip`,
 `setuptools` and `wheel` are up to date.
 
 ```bash
-pip install -U pip setuptools wheel
-pip install srsly
+python -m pip install -U pip setuptools wheel
+python -m pip install srsly
 ```
 
 Or from conda via conda-forge:
 
 ```bash
 conda install -c conda-forge srsly
 ```
 
 Alternatively, you can also compile the library from source. You'll need to make
-sure that you have a development environment consisting of a Python distribution
+sure that you have a development environment with a Python distribution
 including header files, a compiler (XCode command-line tools on macOS / OS X or
-Visual C++ build tools on Windows), pip, virtualenv and git installed.
+Visual C++ build tools on Windows), pip and git installed.
+
+Install from source:
+
+```bash
+# clone the repo
+git clone https://github.com/explosion/srsly
+cd srsly
+
+# create a virtual environment
+python -m venv .env
+source .env/bin/activate
+
+# update pip
+python -m pip install -U pip setuptools wheel
+
+# compile and install from source
+python -m pip install .
+```
+
+For developers, install requirements separately and then install in editable
+mode without build isolation:
 
 ```bash
-pip install -r requirements.txt  # install development dependencies
-python setup.py build_ext --inplace  # compile the library
+# install in editable mode
+python -m pip install -r requirements.txt
+python -m pip install --no-build-isolation --editable .
+
+# run test suite
+python -m pytest --pyargs srsly
 ```
 
 ## API
 
 ### JSON
 
 > 📦 The underlying module is exposed via `srsly.ujson`. However, we normally
@@ -107,74 +161,103 @@
 Create a JSON file and dump contents or write to standard output.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_json("/path/to/file.json", data)
 ```
 
-| Argument   | Type         | Description                                            |
-| ---------- | ------------ | ------------------------------------------------------ |
-| `path` | str / `Path` | The file path or `"-"` to write to stdout.             |
-| `data`     | -            | The JSON-serializable data to output.                  |
-| `indent`   | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+| Argument | Type         | Description                                            |
+| -------- | ------------ | ------------------------------------------------------ |
+| `path`   | str / `Path` | The file path or `"-"` to write to stdout.             |
+| `data`   | -            | The JSON-serializable data to output.                  |
+| `indent` | int          | Number of spaces used to indent JSON. Defaults to `2`. |
 
 #### <kbd>function</kbd> `srsly.read_json`
 
 Load JSON from a file or standard input.
 
 ```python
 data = srsly.read_json("/path/to/file.json")
 ```
 
 | Argument    | Type         | Description                                |
 | ----------- | ------------ | ------------------------------------------ |
-| `path`  | str / `Path` | The file path or `"-"` to read from stdin. |
+| `path`      | str / `Path` | The file path or `"-"` to read from stdin. |
 | **RETURNS** | dict / list  | The loaded JSON content.                   |
 
 #### <kbd>function</kbd> `srsly.write_gzip_json`
 
 Create a gzipped JSON file and dump contents.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_gzip_json("/path/to/file.json.gz", data)
 ```
 
-| Argument   | Type         | Description                                            |
-| ---------- | ------------ | ------------------------------------------------------ |
-| `path` | str / `Path` | The file path.                                         |
-| `data`     | -            | The JSON-serializable data to output.                  |
-| `indent`   | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+| Argument | Type         | Description                                            |
+| -------- | ------------ | ------------------------------------------------------ |
+| `path`   | str / `Path` | The file path.                                         |
+| `data`   | -            | The JSON-serializable data to output.                  |
+| `indent` | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+
+#### <kbd>function</kbd> `srsly.write_gzip_jsonl`
+
+Create a gzipped JSONL file and dump contents.
+
+```python
+data = [{"foo": "bar"}, {"baz": 123}]
+srsly.write_gzip_json("/path/to/file.jsonl.gz", data)
+```
+
+| Argument          | Type         | Description                                                                                                                                                                                                             |
+| ----------------- | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `path`            | str / `Path` | The file path.                                                                                                                                                                                                          |
+| `lines`           | -            | The JSON-serializable contents of each line.                                                                                                                                                                            |
+| `append`          | bool         | Whether or not to append to the location. Appending to .gz files is generally not recommended, as it doesn't allow the algorithm to take advantage of all data when compressing - files may hence be poorly compressed. |
+| `append_new_line` | bool         | Whether or not to write a new line before appending to the file.                                                                                                                                                        |
 
 #### <kbd>function</kbd> `srsly.read_gzip_json`
 
 Load gzipped JSON from a file.
 
 ```python
 data = srsly.read_gzip_json("/path/to/file.json.gz")
 ```
 
 | Argument    | Type         | Description              |
 | ----------- | ------------ | ------------------------ |
-| `path`  | str / `Path` | The file path.           |
+| `path`      | str / `Path` | The file path.           |
 | **RETURNS** | dict / list  | The loaded JSON content. |
 
+#### <kbd>function</kbd> `srsly.read_gzip_jsonl`
+
+Load gzipped JSONL from a file.
+
+```python
+data = srsly.read_gzip_jsonl("/path/to/file.jsonl.gz")
+```
+
+| Argument    | Type         | Description               |
+| ----------- | ------------ | ------------------------- |
+| `path`      | str / `Path` | The file path.            |
+| **RETURNS** | dict / list  | The loaded JSONL content. |
+
 #### <kbd>function</kbd> `srsly.write_jsonl`
 
 Create a JSONL file (newline-delimited JSON) and dump contents line by line, or
 write to standard output.
 
 ```python
 data = [{"foo": "bar"}, {"baz": 123}]
 srsly.write_jsonl("/path/to/file.jsonl", data)
 ```
 
 | Argument          | Type         | Description                                                                                                            |
 | ----------------- | ------------ | ---------------------------------------------------------------------------------------------------------------------- |
-| `path`        | str / `Path` | The file path or `"-"` to write to stdout.                                                                             |
+| `path`            | str / `Path` | The file path or `"-"` to write to stdout.                                                                             |
 | `lines`           | iterable     | The JSON-serializable lines.                                                                                           |
 | `append`          | bool         | Append to an existing file. Will open it in `"a"` mode and insert a newline before writing lines. Defaults to `False`. |
 | `append_new_line` | bool         | Defines whether a new line should first be written when appending to an existing file. Defaults to `True`.             |
 
 #### <kbd>function</kbd> `srsly.read_jsonl`
 
 Read a JSONL file (newline-delimited JSON) or from JSONL data from standard
@@ -182,15 +265,15 @@
 
 ```python
 data = srsly.read_jsonl("/path/to/file.jsonl")
 ```
 
 | Argument   | Type       | Description                                                          |
 | ---------- | ---------- | -------------------------------------------------------------------- |
-| `path` | str / Path | The file path or `"-"` to read from stdin.                           |
+| `path`     | str / Path | The file path or `"-"` to read from stdin.                           |
 | `skip`     | bool       | Skip broken lines and don't raise `ValueError`. Defaults to `False`. |
 | **YIELDS** | -          | The loaded JSON contents of each line.                               |
 
 #### <kbd>function</kbd> `srsly.is_json_serializable`
 
 Check if a Python object is JSON-serializable.
 
@@ -243,30 +326,30 @@
 Create a msgpack file and dump contents.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_msgpack("/path/to/file.msg", data)
 ```
 
-| Argument   | Type         | Description            |
-| ---------- | ------------ | ---------------------- |
-| `path` | str / `Path` | The file path.         |
-| `data`     | -            | The data to serialize. |
+| Argument | Type         | Description            |
+| -------- | ------------ | ---------------------- |
+| `path`   | str / `Path` | The file path.         |
+| `data`   | -            | The data to serialize. |
 
 #### <kbd>function</kbd> `srsly.read_msgpack`
 
 Load a msgpack file.
 
 ```python
 data = srsly.read_msgpack("/path/to/file.msg")
 ```
 
 | Argument    | Type         | Description                                                                             |
 | ----------- | ------------ | --------------------------------------------------------------------------------------- |
-| `path`  | str / `Path` | The file path.                                                                          |
+| `path`      | str / `Path` | The file path.                                                                          |
 | `use_list`  | bool         | Don't use tuples instead of lists. Can make deserialization slower. Defaults to `True`. |
 | **RETURNS** | -            | The loaded and deserialized content.                                                    |
 
 ### pickle
 
 > 📦 The underlying module is exposed via `srsly.cloudpickle`. However, we
 > normally interact with it via the utility functions only.
@@ -314,15 +397,15 @@
 yaml_string = srsly.yaml_dumps(data)
 ```
 
 | Argument          | Type | Description                                |
 | ----------------- | ---- | ------------------------------------------ |
 | `data`            | -    | The JSON-serializable data to output.      |
 | `indent_mapping`  | int  | Mapping indentation. Defaults to `2`.      |
-| `indent_sequence` | int  | Sequence indentation. Defaults to `4`.      |
+| `indent_sequence` | int  | Sequence indentation. Defaults to `4`.     |
 | `indent_offset`   | int  | Indentation offset. Defaults to `2`.       |
 | `sort_keys`       | bool | Sort dictionary keys. Defaults to `False`. |
 | **RETURNS**       | str  | The serialized string.                     |
 
 #### <kbd>function</kbd> `srsly.yaml_loads`
 
 Deserialize unicode or a file object to a Python object.
@@ -344,32 +427,32 @@
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_yaml("/path/to/file.yml", data)
 ```
 
 | Argument          | Type         | Description                                |
 | ----------------- | ------------ | ------------------------------------------ |
-| `path`        | str / `Path` | The file path or `"-"` to write to stdout. |
+| `path`            | str / `Path` | The file path or `"-"` to write to stdout. |
 | `data`            | -            | The JSON-serializable data to output.      |
 | `indent_mapping`  | int          | Mapping indentation. Defaults to `2`.      |
-| `indent_sequence` | int          | Sequence indentation. Defaults to `4`.      |
+| `indent_sequence` | int          | Sequence indentation. Defaults to `4`.     |
 | `indent_offset`   | int          | Indentation offset. Defaults to `2`.       |
 | `sort_keys`       | bool         | Sort dictionary keys. Defaults to `False`. |
 
 #### <kbd>function</kbd> `srsly.read_yaml`
 
 Load YAML from a file or standard input.
 
 ```python
 data = srsly.read_yaml("/path/to/file.yml")
 ```
 
 | Argument    | Type         | Description                                |
 | ----------- | ------------ | ------------------------------------------ |
-| `path`  | str / `Path` | The file path or `"-"` to read from stdin. |
+| `path`      | str / `Path` | The file path or `"-"` to read from stdin. |
 | **RETURNS** | dict / list  | The loaded YAML content.                   |
 
 #### <kbd>function</kbd> `srsly.is_yaml_serializable`
 
 Check if a Python object is YAML-serializable.
 
 ```python
```

#### html2text {}

```diff
@@ -1,107 +1,145 @@
-[https://explosion.ai/assets/img/logo.svg] # srsly: Modern high-performance
-serialization utilities for Python This package bundles some of the best Python
-serialization libraries into one standalone package, with a high-level API that
-makes it easy to write code that's correct across platforms and Pythons. This
-allows us to provide all the serialization utilities we need in a single binary
-wheel. Currently supports **JSON**, **JSONL**, **MessagePack**, **Pickle** and
-**YAML**. [![Azure Pipelines](https://img.shields.io/azure-devops/build/
-explosion-ai/public/4/master.svg?logo=azure-pipelines&style=flat-square)]
-(https://dev.azure.com/explosion-ai/public/_build?definitionId=4) [![PyPi]
-(https://img.shields.io/pypi/v/srsly.svg?style=flat-
+Metadata-Version: 2.1 Name: srsly Version: 2.4.6 Summary: Modern high-
+performance serialization utilities for Python Home-page: https://github.com/
+explosion/srsly Author: Explosion Author-email: contact@explosion.ai License:
+MIT Classifier: Development Status :: 5 - Production/Stable Classifier:
+Environment :: Console Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
+:: Windows Classifier: Programming Language :: Cython Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE [https://explosion.ai/assets/img/logo.svg] # srsly: Modern high-
+performance serialization utilities for Python This package bundles some of the
+best Python serialization libraries into one standalone package, with a high-
+level API that makes it easy to write code that's correct across platforms and
+Pythons. This allows us to provide all the serialization utilities we need in a
+single binary wheel. Currently supports **JSON**, **JSONL**, **MessagePack**,
+**Pickle** and **YAML**. [![Azure Pipelines](https://img.shields.io/azure-
+devops/build/explosion-ai/public/4/master.svg?logo=azure-pipelines&style=flat-
+square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=4) [!
+[PyPi](https://img.shields.io/pypi/v/srsly.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/srsly) [!
 [conda](https://img.shields.io/conda/vn/conda-forge/srsly.svg?style=flat-
 square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/
 srsly) [![GitHub](https://img.shields.io/github/release/explosion/srsly/
 all.svg?style=flat-square&logo=github)](https://github.com/explosion/srsly) [!
 [Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
 4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://
 github.com/explosion/wheelwright/releases) ## Motivation Serialization is hard,
 especially across Python versions and multiple platforms. After dealing with
 many subtle bugs over the years (encodings, locales, large files) our libraries
 like [spaCy](https://github.com/explosion/spaCy) and [Prodigy](https://
-prodi.gy) have steadily grown a number of utility functions to wrap the
-multiple serialization formats we need to support (especially `json`, `msgpack`
-and `pickle`). These wrapping functions ended up duplicated across our
-codebases, so we wanted to put them in one place. At the same time, we noticed
-that having a lot of small dependencies was making maintenance harder, and
-making installation slower. To solve this, we've made `srsly` standalone, by
-including the component packages directly within it. This way we can provide
-all the serialization utilities we need in a single binary wheel. `srsly`
-currently includes forks of the following packages: - [`ujson`](https://
-github.com/esnme/ultrajson) - [`msgpack`](https://github.com/msgpack/msgpack-
-python) - [`msgpack-numpy`](https://github.com/lebedov/msgpack-numpy) -
-[`cloudpickle`](https://github.com/cloudpipe/cloudpickle) - [`ruamel.yaml`]
-(https://github.com/pycontribs/ruamel-yaml) (without unsafe implementations!)
-## Installation > â ï¸ Note that `v2.x` is only compatible with **Python
-3.6+**. For 2.7+ compatibility, use `v1.x`. `srsly` can be installed from pip.
-Before installing, make sure that your `pip`, `setuptools` and `wheel` are up
-to date. ```bash pip install -U pip setuptools wheel pip install srsly ``` Or
-from conda via conda-forge: ```bash conda install -c conda-forge srsly ```
-Alternatively, you can also compile the library from source. You'll need to
-make sure that you have a development environment consisting of a Python
+prodi.gy) had steadily grown a number of utility functions to wrap the multiple
+serialization formats we need to support (especially `json`, `msgpack` and
+`pickle`). These wrapping functions ended up duplicated across our codebases,
+so we wanted to put them in one place. At the same time, we noticed that having
+a lot of small dependencies was making maintenance harder, and making
+installation slower. To solve this, we've made `srsly` standalone, by including
+the component packages directly within it. This way we can provide all the
+serialization utilities we need in a single binary wheel. `srsly` currently
+includes forks of the following packages: - [`ujson`](https://github.com/esnme/
+ultrajson) - [`msgpack`](https://github.com/msgpack/msgpack-python) -
+[`msgpack-numpy`](https://github.com/lebedov/msgpack-numpy) - [`cloudpickle`]
+(https://github.com/cloudpipe/cloudpickle) - [`ruamel.yaml`](https://
+github.com/pycontribs/ruamel-yaml) (without unsafe implementations!) ##
+Installation > â ï¸ Note that `v2.x` is only compatible with **Python 3.6+**.
+For 2.7+ compatibility, use `v1.x`. `srsly` can be installed from pip. Before
+installing, make sure that your `pip`, `setuptools` and `wheel` are up to date.
+```bash python -m pip install -U pip setuptools wheel python -m pip install
+srsly ``` Or from conda via conda-forge: ```bash conda install -c conda-forge
+srsly ``` Alternatively, you can also compile the library from source. You'll
+need to make sure that you have a development environment with a Python
 distribution including header files, a compiler (XCode command-line tools on
-macOS / OS X or Visual C++ build tools on Windows), pip, virtualenv and git
-installed. ```bash pip install -r requirements.txt # install development
-dependencies python setup.py build_ext --inplace # compile the library ``` ##
-API ### JSON > ð¦ The underlying module is exposed via `srsly.ujson`.
-However, we normally > interact with it via the utility functions only. ####
-function `srsly.json_dumps` Serialize an object to a JSON string. Falls back to
-`json` if `sort_keys=True` is used (until it's fixed in `ujson`). ```python
-data = {"foo": "bar", "baz": 123} json_string = srsly.json_dumps(data) ``` |
-Argument | Type | Description | | ----------- | ---- | ------------------------
------------------------------- | | `data` | - | The JSON-serializable data to
-output. | | `indent` | int | Number of spaces used to indent JSON. Defaults to
-`0`. | | `sort_keys` | bool | Sort dictionary keys. Defaults to `False`. | |
-**RETURNS** | str | The serialized string. | #### function `srsly.json_loads`
-Deserialize unicode or bytes to a Python object. ```python data = '{"foo":
-"bar", "baz": 123}' obj = srsly.json_loads(data) ``` | Argument | Type |
-Description | | ----------- | ----------- | ------------------------------- | |
-`data` | str / bytes | The data to deserialize. | | **RETURNS** | - | The
-deserialized Python object. | #### function `srsly.write_json` Create a JSON
-file and dump contents or write to standard output. ```python data = {"foo":
-"bar", "baz": 123} srsly.write_json("/path/to/file.json", data) ``` | Argument
-| Type | Description | | ---------- | ------------ | --------------------------
----------------------------- | | `path` | str / `Path` | The file path or `"-"`
-to write to stdout. | | `data` | - | The JSON-serializable data to output. | |
-`indent` | int | Number of spaces used to indent JSON. Defaults to `2`. | ####
-function `srsly.read_json` Load JSON from a file or standard input. ```python
-data = srsly.read_json("/path/to/file.json") ``` | Argument | Type |
-Description | | ----------- | ------------ | ----------------------------------
--------- | | `path` | str / `Path` | The file path or `"-"` to read from stdin.
-| | **RETURNS** | dict / list | The loaded JSON content. | #### function
+macOS / OS X or Visual C++ build tools on Windows), pip and git installed.
+Install from source: ```bash # clone the repo git clone https://github.com/
+explosion/srsly cd srsly # create a virtual environment python -m venv .env
+source .env/bin/activate # update pip python -m pip install -U pip setuptools
+wheel # compile and install from source python -m pip install . ``` For
+developers, install requirements separately and then install in editable mode
+without build isolation: ```bash # install in editable mode python -m pip
+install -r requirements.txt python -m pip install --no-build-isolation --
+editable . # run test suite python -m pytest --pyargs srsly ``` ## API ### JSON
+> ð¦ The underlying module is exposed via `srsly.ujson`. However, we normally
+> interact with it via the utility functions only. #### function
+`srsly.json_dumps` Serialize an object to a JSON string. Falls back to `json`
+if `sort_keys=True` is used (until it's fixed in `ujson`). ```python data =
+{"foo": "bar", "baz": 123} json_string = srsly.json_dumps(data) ``` | Argument
+| Type | Description | | ----------- | ---- | ---------------------------------
+--------------------- | | `data` | - | The JSON-serializable data to output. |
+| `indent` | int | Number of spaces used to indent JSON. Defaults to `0`. | |
+`sort_keys` | bool | Sort dictionary keys. Defaults to `False`. | | **RETURNS**
+| str | The serialized string. | #### function `srsly.json_loads` Deserialize
+unicode or bytes to a Python object. ```python data = '{"foo": "bar", "baz":
+123}' obj = srsly.json_loads(data) ``` | Argument | Type | Description | | ----
+------- | ----------- | ------------------------------- | | `data` | str /
+bytes | The data to deserialize. | | **RETURNS** | - | The deserialized Python
+object. | #### function `srsly.write_json` Create a JSON file and dump contents
+or write to standard output. ```python data = {"foo": "bar", "baz": 123}
+srsly.write_json("/path/to/file.json", data) ``` | Argument | Type |
+Description | | -------- | ------------ | -------------------------------------
+----------------- | | `path` | str / `Path` | The file path or `"-"` to write
+to stdout. | | `data` | - | The JSON-serializable data to output. | | `indent`
+| int | Number of spaces used to indent JSON. Defaults to `2`. | #### function
+`srsly.read_json` Load JSON from a file or standard input. ```python data =
+srsly.read_json("/path/to/file.json") ``` | Argument | Type | Description | | -
+---------- | ------------ | ------------------------------------------ | |
+`path` | str / `Path` | The file path or `"-"` to read from stdin. | |
+**RETURNS** | dict / list | The loaded JSON content. | #### function
 `srsly.write_gzip_json` Create a gzipped JSON file and dump contents. ```python
 data = {"foo": "bar", "baz": 123} srsly.write_gzip_json("/path/to/
-file.json.gz", data) ``` | Argument | Type | Description | | ---------- | -----
-------- | ------------------------------------------------------ | | `path` |
-str / `Path` | The file path. | | `data` | - | The JSON-serializable data to
+file.json.gz", data) ``` | Argument | Type | Description | | -------- | -------
+----- | ------------------------------------------------------ | | `path` | str
+/ `Path` | The file path. | | `data` | - | The JSON-serializable data to
 output. | | `indent` | int | Number of spaces used to indent JSON. Defaults to
-`2`. | #### function `srsly.read_gzip_json` Load gzipped JSON from a file.
-```python data = srsly.read_gzip_json("/path/to/file.json.gz") ``` | Argument |
-Type | Description | | ----------- | ------------ | ------------------------ |
-| `path` | str / `Path` | The file path. | | **RETURNS** | dict / list | The
-loaded JSON content. | #### function `srsly.write_jsonl` Create a JSONL file
-(newline-delimited JSON) and dump contents line by line, or write to standard
-output. ```python data = [{"foo": "bar"}, {"baz": 123}] srsly.write_jsonl("/
-path/to/file.jsonl", data) ``` | Argument | Type | Description | | ------------
------ | ------------ | --------------------------------------------------------
--------------------------------------------------------------- | | `path` | str
-/ `Path` | The file path or `"-"` to write to stdout. | | `lines` | iterable |
-The JSON-serializable lines. | | `append` | bool | Append to an existing file.
-Will open it in `"a"` mode and insert a newline before writing lines. Defaults
-to `False`. | | `append_new_line` | bool | Defines whether a new line should
-first be written when appending to an existing file. Defaults to `True`. | ####
-function `srsly.read_jsonl` Read a JSONL file (newline-delimited JSON) or from
-JSONL data from standard input and yield contents line by line. Blank lines
-will always be skipped. ```python data = srsly.read_jsonl("/path/to/
-file.jsonl") ``` | Argument | Type | Description | | ---------- | ---------- |
--------------------------------------------------------------------- | | `path`
-| str / Path | The file path or `"-"` to read from stdin. | | `skip` | bool |
-Skip broken lines and don't raise `ValueError`. Defaults to `False`. | |
-**YIELDS** | - | The loaded JSON contents of each line. | #### function
+`2`. | #### function `srsly.write_gzip_jsonl` Create a gzipped JSONL file and
+dump contents. ```python data = [{"foo": "bar"}, {"baz": 123}]
+srsly.write_gzip_json("/path/to/file.jsonl.gz", data) ``` | Argument | Type |
+Description | | ----------------- | ------------ | ----------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+----------------------------- | | `path` | str / `Path` | The file path. | |
+`lines` | - | The JSON-serializable contents of each line. | | `append` | bool
+| Whether or not to append to the location. Appending to .gz files is generally
+not recommended, as it doesn't allow the algorithm to take advantage of all
+data when compressing - files may hence be poorly compressed. | |
+`append_new_line` | bool | Whether or not to write a new line before appending
+to the file. | #### function `srsly.read_gzip_json` Load gzipped JSON from a
+file. ```python data = srsly.read_gzip_json("/path/to/file.json.gz") ``` |
+Argument | Type | Description | | ----------- | ------------ | ----------------
+-------- | | `path` | str / `Path` | The file path. | | **RETURNS** | dict /
+list | The loaded JSON content. | #### function `srsly.read_gzip_jsonl` Load
+gzipped JSONL from a file. ```python data = srsly.read_gzip_jsonl("/path/to/
+file.jsonl.gz") ``` | Argument | Type | Description | | ----------- | ---------
+--- | ------------------------- | | `path` | str / `Path` | The file path. | |
+**RETURNS** | dict / list | The loaded JSONL content. | #### function
+`srsly.write_jsonl` Create a JSONL file (newline-delimited JSON) and dump
+contents line by line, or write to standard output. ```python data = [{"foo":
+"bar"}, {"baz": 123}] srsly.write_jsonl("/path/to/file.jsonl", data) ``` |
+Argument | Type | Description | | ----------------- | ------------ | ----------
+-------------------------------------------------------------------------------
+----------------------------- | | `path` | str / `Path` | The file path or `"-
+"` to write to stdout. | | `lines` | iterable | The JSON-serializable lines. |
+| `append` | bool | Append to an existing file. Will open it in `"a"` mode and
+insert a newline before writing lines. Defaults to `False`. | |
+`append_new_line` | bool | Defines whether a new line should first be written
+when appending to an existing file. Defaults to `True`. | #### function
+`srsly.read_jsonl` Read a JSONL file (newline-delimited JSON) or from JSONL
+data from standard input and yield contents line by line. Blank lines will
+always be skipped. ```python data = srsly.read_jsonl("/path/to/file.jsonl") ```
+| Argument | Type | Description | | ---------- | ---------- | -----------------
+--------------------------------------------------- | | `path` | str / Path |
+The file path or `"-"` to read from stdin. | | `skip` | bool | Skip broken
+lines and don't raise `ValueError`. Defaults to `False`. | | **YIELDS** | - |
+The loaded JSON contents of each line. | #### function
 `srsly.is_json_serializable` Check if a Python object is JSON-serializable.
 ```python assert srsly.is_json_serializable({"hello": "world"}) is True assert
 srsly.is_json_serializable(lambda x: x) is False ``` | Argument | Type |
 Description | | ----------- | ---- | ---------------------------------------- |
 | `obj` | - | The object to check. | | **RETURNS** | bool | Whether the object
 is JSON-serializable. | ### msgpack > ð¦ The underlying module is exposed via
 `srsly.msgpack`. However, we normally > interact with it via the utility
@@ -115,16 +153,16 @@
 Argument | Type | Description | | ----------- | ----- | -----------------------
 ---------------------------------------------------------------- | | `data` |
 bytes | The data to deserialize. | | `use_list` | bool | Don't use tuples
 instead of lists. Can make deserialization slower. Defaults to `True`. | |
 **RETURNS** | - | The deserialized Python object. | #### function
 `srsly.write_msgpack` Create a msgpack file and dump contents. ```python data =
 {"foo": "bar", "baz": 123} srsly.write_msgpack("/path/to/file.msg", data) ``` |
-Argument | Type | Description | | ---------- | ------------ | -----------------
------ | | `path` | str / `Path` | The file path. | | `data` | - | The data to
+Argument | Type | Description | | -------- | ------------ | -------------------
+--- | | `path` | str / `Path` | The file path. | | `data` | - | The data to
 serialize. | #### function `srsly.read_msgpack` Load a msgpack file. ```python
 data = srsly.read_msgpack("/path/to/file.msg") ``` | Argument | Type |
 Description | | ----------- | ------------ | ----------------------------------
 ----------------------------------------------------- | | `path` | str / `Path`
 | The file path. | | `use_list` | bool | Don't use tuples instead of lists. Can
 make deserialization slower. Defaults to `True`. | | **RETURNS** | - | The
 loaded and deserialized content. | ### pickle > ð¦ The underlying module is
```

### Comparing `srsly-2.4.5.dev1/setup.cfg` & `srsly-2.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/setup.py` & `srsly-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/__init__.py` & `srsly-2.4.6/srsly/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ._json_api import read_json, read_gzip_json, write_json, write_gzip_json
+from ._json_api import read_gzip_jsonl, write_gzip_jsonl
 from ._json_api import read_jsonl, write_jsonl
 from ._json_api import json_dumps, json_loads, is_json_serializable
 from ._msgpack_api import read_msgpack, write_msgpack, msgpack_dumps, msgpack_loads
 from ._msgpack_api import msgpack_encoders, msgpack_decoders
 from ._pickle_api import pickle_dumps, pickle_loads
 from ._yaml_api import read_yaml, write_yaml, yaml_dumps, yaml_loads
 from ._yaml_api import is_yaml_serializable
```

### Comparing `srsly-2.4.5.dev1/srsly/_json_api.py` & `srsly-2.4.6/srsly/_json_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Iterable, Sequence, Any, Optional
+from typing import Union, Iterable, Sequence, Any, Optional, Iterator
 import sys
 import json as _builtin_json
 import gzip
 
 from . import ujson
 from .util import force_path, force_string, FilePath, JSONInput, JSONOutput
 
@@ -52,22 +52,35 @@
     with file_path.open("r", encoding="utf8") as f:
         return ujson.load(f)
 
 
 def read_gzip_json(path: FilePath) -> JSONOutput:
     """Load JSON from a gzipped file.
 
-        location (FilePath): The file path.
-        RETURNS (JSONOutput): The loaded JSON content.
+    location (FilePath): The file path.
+    RETURNS (JSONOutput): The loaded JSON content.
     """
     file_path = force_string(path)
     with gzip.open(file_path, "r") as f:
         return ujson.load(f)
 
 
+def read_gzip_jsonl(path: FilePath, skip: bool = False) -> Iterator[JSONOutput]:
+    """Read a gzipped .jsonl file and yield contents line by line.
+    Blank lines will always be skipped.
+
+    path (FilePath): The file path.
+    skip (bool): Skip broken lines and don't raise ValueError.
+    YIELDS (JSONOutput): The unpacked, deserialized Python objects.
+    """
+    with gzip.open(force_path(path), "r") as f:
+        for line in _yield_json_lines(f, skip=skip):
+            yield line
+
+
 def write_json(path: FilePath, data: JSONInput, indent: int = 2) -> None:
     """Create a .json file and dump contents or write to standard
     output.
 
     location (FilePath): The file path. "-" for writing to stdout.
     data (JSONInput): The JSON-serializable data to output.
     indent (int): Number of spaces used to indent JSON.
@@ -90,14 +103,38 @@
     """
     json_data = json_dumps(data, indent=indent)
     file_path = force_string(path)
     with gzip.open(file_path, "w") as f:
         f.write(json_data.encode("utf-8"))
 
 
+def write_gzip_jsonl(
+    path: FilePath,
+    lines: Iterable[JSONInput],
+    append: bool = False,
+    append_new_line: bool = True,
+) -> None:
+    """Create a .jsonl.gz file and dump contents.
+
+    location (FilePath): The file path.
+    lines (Sequence[JSONInput]): The JSON-serializable contents of each line.
+    append (bool): Whether or not to append to the location. Appending to .gz files is generally not recommended, as it
+        doesn't allow the algorithm to take advantage of all data when compressing - files may hence be poorly
+        compressed.
+    append_new_line (bool): Whether or not to write a new line before appending
+        to the file.
+    """
+    mode = "a" if append else "w"
+    file_path = force_path(path, require_exists=False)
+    with gzip.open(file_path, mode=mode) as f:
+        if append and append_new_line:
+            f.write("\n".encode("utf-8"))
+        f.writelines([(json_dumps(line) + "\n").encode("utf-8") for line in lines])
+
+
 def read_jsonl(path: FilePath, skip: bool = False) -> Iterable[JSONOutput]:
     """Read a .jsonl file or standard input and yield contents line by line.
     Blank lines will always be skipped.
 
     path (FilePath): The file path. "-" for reading from stdin.
     skip (bool): Skip broken lines and don't raise ValueError.
     YIELDS (JSONOutput): The loaded JSON contents of each line.
```

### Comparing `srsly-2.4.5.dev1/srsly/_msgpack_api.py` & `srsly-2.4.6/srsly/_msgpack_api.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/_pickle_api.py` & `srsly-2.4.6/srsly/_pickle_api.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/_yaml_api.py` & `srsly-2.4.6/srsly/_yaml_api.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/cloudpickle/cloudpickle.py` & `srsly-2.4.6/srsly/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/cloudpickle/cloudpickle_fast.py` & `srsly-2.4.6/srsly/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/__init__.py` & `srsly-2.4.6/srsly/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/_msgpack_numpy.py` & `srsly-2.4.6/srsly/msgpack/_msgpack_numpy.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/_packer.cpp` & `srsly-2.4.6/srsly/msgpack/_packer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "__LITTLE_ENDIAN__",
                 "1"
             ]
         ],
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.14/x64/include/python3.8/Python.h",
-            "/opt/hostedtoolcache/Python/3.8.14/x64/include/python3.8/pythread.h",
+            "/opt/hostedtoolcache/Python/3.8.16/x64/include/python3.8/Python.h",
+            "/opt/hostedtoolcache/Python/3.8.16/x64/include/python3.8/pythread.h",
             "srsly/msgpack/buff_converter.h",
             "srsly/msgpack/pack.h"
         ],
         "include_dirs": [
             "srsly/msgpack",
-            "/opt/hostedtoolcache/Python/3.8.14/x64/include/python3.8",
+            "/opt/hostedtoolcache/Python/3.8.16/x64/include/python3.8",
             "."
         ],
         "language": "c++",
         "name": "srsly.msgpack._packer",
         "sources": [
             "srsly/msgpack/_packer.pyx"
         ]
@@ -35,16 +35,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_33"
+#define CYTHON_HEX_VERSION 0x001D21F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -113,15 +113,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -592,35 +592,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1210,26 +1210,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -6526,15 +6526,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_items.type = (PyObject*)&PyDict_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -6813,15 +6813,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_srsly__msgpack___packer) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -7943,29 +7943,27 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* PyObjectCallNoArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -8307,15 +8305,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/_packer.pyx` & `srsly-2.4.6/srsly/msgpack/_packer.pyx`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/_unpacker.cpp` & `srsly-2.4.6/srsly/msgpack/_unpacker.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "__LITTLE_ENDIAN__",
                 "1"
             ]
         ],
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.14/x64/include/python3.8/Python.h",
-            "/opt/hostedtoolcache/Python/3.8.14/x64/include/python3.8/pythread.h",
+            "/opt/hostedtoolcache/Python/3.8.16/x64/include/python3.8/Python.h",
+            "/opt/hostedtoolcache/Python/3.8.16/x64/include/python3.8/pythread.h",
             "srsly/msgpack/unpack.h"
         ],
         "include_dirs": [
             "srsly/msgpack",
-            "/opt/hostedtoolcache/Python/3.8.14/x64/include/python3.8",
+            "/opt/hostedtoolcache/Python/3.8.16/x64/include/python3.8",
             "."
         ],
         "language": "c++",
         "name": "srsly.msgpack._unpacker",
         "sources": [
             "srsly/msgpack/_unpacker.pyx"
         ]
@@ -34,16 +34,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_33"
+#define CYTHON_HEX_VERSION 0x001D21F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -112,15 +112,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -591,35 +591,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1278,26 +1278,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -7193,15 +7193,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -7480,15 +7480,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_srsly__msgpack___unpacker) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8656,15 +8656,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -9071,15 +9071,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/_unpacker.pyx` & `srsly-2.4.6/srsly/msgpack/_unpacker.pyx`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/buff_converter.h` & `srsly-2.4.6/srsly/msgpack/buff_converter.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/exceptions.py` & `srsly-2.4.6/srsly/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/pack.h` & `srsly-2.4.6/srsly/msgpack/pack.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/pack_template.h` & `srsly-2.4.6/srsly/msgpack/pack_template.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/sysdep.h` & `srsly-2.4.6/srsly/msgpack/sysdep.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/unpack.h` & `srsly-2.4.6/srsly/msgpack/unpack.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/unpack_define.h` & `srsly-2.4.6/srsly/msgpack/unpack_define.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/msgpack/unpack_template.h` & `srsly-2.4.6/srsly/msgpack/unpack_template.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/comments.py` & `srsly-2.4.6/srsly/ruamel_yaml/comments.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/compat.py` & `srsly-2.4.6/srsly/ruamel_yaml/compat.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/composer.py` & `srsly-2.4.6/srsly/ruamel_yaml/composer.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/constructor.py` & `srsly-2.4.6/srsly/ruamel_yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/cyaml.py` & `srsly-2.4.6/srsly/ruamel_yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/dumper.py` & `srsly-2.4.6/srsly/ruamel_yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/emitter.py` & `srsly-2.4.6/srsly/ruamel_yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/error.py` & `srsly-2.4.6/srsly/ruamel_yaml/error.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/events.py` & `srsly-2.4.6/srsly/ruamel_yaml/events.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/loader.py` & `srsly-2.4.6/srsly/ruamel_yaml/loader.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/main.py` & `srsly-2.4.6/srsly/ruamel_yaml/main.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/nodes.py` & `srsly-2.4.6/srsly/ruamel_yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/parser.py` & `srsly-2.4.6/srsly/ruamel_yaml/parser.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/reader.py` & `srsly-2.4.6/srsly/ruamel_yaml/reader.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/representer.py` & `srsly-2.4.6/srsly/ruamel_yaml/representer.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/resolver.py` & `srsly-2.4.6/srsly/ruamel_yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarbool.py` & `srsly-2.4.6/srsly/ruamel_yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarfloat.py` & `srsly-2.4.6/srsly/ruamel_yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarint.py` & `srsly-2.4.6/srsly/ruamel_yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/scalarstring.py` & `srsly-2.4.6/srsly/ruamel_yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/scanner.py` & `srsly-2.4.6/srsly/ruamel_yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/serializer.py` & `srsly-2.4.6/srsly/ruamel_yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/timestamp.py` & `srsly-2.4.6/srsly/ruamel_yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/tokens.py` & `srsly-2.4.6/srsly/ruamel_yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ruamel_yaml/util.py` & `srsly-2.4.6/srsly/ruamel_yaml/util.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/cloudpickle/cloudpickle_file_test.py` & `srsly-2.4.6/srsly/tests/cloudpickle/cloudpickle_file_test.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/cloudpickle/cloudpickle_test.py` & `srsly-2.4.6/srsly/tests/cloudpickle/cloudpickle_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -866,16 +866,20 @@
         # instances
         assert depickled_bound_meth() == bound_classicmethod()
         assert depickled_unbound_meth is unbound_classicmethod
         assert depickled_clsdict_meth is clsdict_classicmethod
 
 
     @pytest.mark.skipif(
-        platform.machine() == "aarch64" and sys.version_info[:2] >= (3, 10),
-        reason="Fails on aarch64 + python 3.10+ in cibuildwheel, currently unable to replicate failure elsewhere")
+        (platform.machine() == "aarch64" and sys.version_info[:2] >= (3, 10))
+            or platform.python_implementation() == "PyPy"
+            or (sys.version_info[:2] == (3, 10) and sys.version_info >= (3, 10, 8))
+            # Skipping tests on 3.11 due to https://github.com/cloudpipe/cloudpickle/pull/486.
+            or sys.version_info[:2] == (3, 11),
+        reason="Fails on aarch64 + python 3.10+ in cibuildwheel, currently unable to replicate failure elsewhere; fails sometimes for pypy on conda-forge; fails for python 3.10.8+ and 3.11")
     def test_builtin_classmethod(self):
         obj = 1.5  # float object
 
         bound_clsmethod = obj.fromhex  # builtin_function_or_method
         unbound_clsmethod = type(obj).fromhex  # builtin_function_or_method
         clsdict_clsmethod = type(
             obj).__dict__['fromhex']  # classmethod_descriptor
@@ -1466,14 +1470,15 @@
 
                     # Test whichmodule in save_function.
                     cloned = pickle_depickle(foo, protocol=self.protocol)
                     self.assertEqual(cloned(), "it works!")
                 finally:
                     sys.modules.pop("_faulty_module", None)
 
+    @pytest.mark.skip(reason="fails for pytest v7.2.0")
     def test_dynamic_pytest_module(self):
         # Test case for pull request https://github.com/cloudpipe/cloudpickle/pull/116
         import py
 
         def f():
             s = py.builtin.set([1])
             return s.pop()
@@ -1563,14 +1568,16 @@
 
         assert isinstance(depickled_t1, MyTuple)
         assert depickled_t1 == t1
         assert depickled_MyTuple is MyTuple
         assert isinstance(depickled_t2, MyTuple)
         assert depickled_t2 == t2
 
+    @pytest.mark.skipif(platform.python_implementation() == "PyPy",
+        reason="fails sometimes for pypy on conda-forge")
     def test_interactively_defined_function(self):
         # Check that callables defined in the __main__ module of a Python
         # script (or jupyter kernel) can be pickled / unpickled / executed.
         code = """\
         from srsly.tests.cloudpickle.testutils import subprocess_pickle_echo
 
         CONSTANT = 42
```

### Comparing `srsly-2.4.5.dev1/srsly/tests/cloudpickle/testutils.py` & `srsly-2.4.6/srsly/tests/cloudpickle/testutils.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_buffer.py` & `srsly-2.4.6/srsly/tests/msgpack/test_buffer.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_case.py` & `srsly-2.4.6/srsly/tests/msgpack/test_case.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_except.py` & `srsly-2.4.6/srsly/tests/msgpack/test_except.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_extension.py` & `srsly-2.4.6/srsly/tests/msgpack/test_extension.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_format.py` & `srsly-2.4.6/srsly/tests/msgpack/test_format.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_limits.py` & `srsly-2.4.6/srsly/tests/msgpack/test_limits.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_memoryview.py` & `srsly-2.4.6/srsly/tests/msgpack/test_memoryview.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_newspec.py` & `srsly-2.4.6/srsly/tests/msgpack/test_newspec.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_numpy.py` & `srsly-2.4.6/srsly/tests/msgpack/test_numpy.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_pack.py` & `srsly-2.4.6/srsly/tests/msgpack/test_pack.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_read_size.py` & `srsly-2.4.6/srsly/tests/msgpack/test_read_size.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_seq.py` & `srsly-2.4.6/srsly/tests/msgpack/test_seq.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_sequnpack.py` & `srsly-2.4.6/srsly/tests/msgpack/test_sequnpack.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_stricttype.py` & `srsly-2.4.6/srsly/tests/msgpack/test_stricttype.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/msgpack/test_unpack.py` & `srsly-2.4.6/srsly/tests/msgpack/test_unpack.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/roundtrip.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/roundtrip.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_a_dedent.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_a_dedent.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_add_xxx.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_add_xxx.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_anchor.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_anchor.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_api_change.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_api_change.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_appliance.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_appliance.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_class_register.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_class_register.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_comment_manipulation.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_comment_manipulation.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_comments.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_comments.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_contextmanager.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_contextmanager.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_copy.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_copy.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_datetime.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_datetime.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_documents.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_documents.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_fail.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_fail.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_float.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_float.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_indentation.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_indentation.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_int.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_int.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_issues.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_issues.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_json_numbers.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_json_numbers.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_line_col.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_line_col.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_literal.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_literal.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_none.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_none.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_program_config.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_program_config.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_spec_examples.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_spec_examples.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_string.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_string.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_tag.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_tag.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_version.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_version.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_yamlfile.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_yamlfile.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_yamlobject.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_yamlobject.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_z_check_debug_leftovers.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_z_check_debug_leftovers.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ruamel_yaml/test_z_data.py` & `srsly-2.4.6/srsly/tests/ruamel_yaml/test_z_data.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/test_json_api.py` & `srsly-2.4.6/srsly/tests/test_json_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import pytest
 from io import StringIO
 from pathlib import Path
 import gzip
 import numpy
 
-from .._json_api import read_json, write_json, read_jsonl, write_jsonl
+from .._json_api import (
+    read_json,
+    write_json,
+    read_jsonl,
+    write_jsonl,
+    read_gzip_jsonl,
+    write_gzip_jsonl,
+)
 from .._json_api import write_gzip_json, json_dumps, is_json_serializable
 from .._json_api import json_loads
 from ..util import force_string
 from .util import make_tempdir
 
 
 def test_json_dumps_sort_keys():
@@ -200,7 +207,58 @@
         json_loads(obj)
 
 
 def test_unsupported_type_error():
     f = numpy.float32()
     with pytest.raises(TypeError):
         s = json_dumps(f)
+
+
+def test_write_jsonl_gzip():
+    """Tests writing data to a gzipped .jsonl file."""
+    data = [{"hello": "world"}, {"test": 123}]
+    expected = ['{"hello":"world"}\n', '{"test":123}\n']
+
+    with make_tempdir() as temp_dir:
+        file_path = temp_dir / "tmp.json"
+        write_gzip_jsonl(file_path, data)
+        with gzip.open(file_path, "r") as f:
+            assert [line.decode("utf8") for line in f.readlines()] == expected
+
+
+def test_write_jsonl_gzip_append():
+    """Tests appending data to a gzipped .jsonl file."""
+    data = [{"hello": "world"}, {"test": 123}]
+    expected = [
+        '{"hello":"world"}\n',
+        '{"test":123}\n',
+        "\n",
+        '{"hello":"world"}\n',
+        '{"test":123}\n',
+    ]
+    with make_tempdir() as temp_dir:
+        file_path = temp_dir / "tmp.json"
+        write_gzip_jsonl(file_path, data)
+        write_gzip_jsonl(file_path, data, append=True)
+        with gzip.open(file_path, "r") as f:
+            assert [line.decode("utf8") for line in f.readlines()] == expected
+
+
+def test_read_jsonl_gzip():
+    """Tests reading data from a gzipped .jsonl file."""
+    file_contents = [{"hello": "world"}, {"test": 123}]
+    with make_tempdir() as temp_dir:
+        file_path = temp_dir / "tmp.json"
+        with gzip.open(file_path, "w") as f:
+            f.writelines(
+                [(json_dumps(line) + "\n").encode("utf-8") for line in file_contents]
+            )
+        assert file_path.exists()
+        data = read_gzip_jsonl(file_path)
+        # Make sure this returns a generator, not just a list
+        assert not hasattr(data, "__len__")
+        data = list(data)
+    assert len(data) == 2
+    assert len(data[0]) == 1
+    assert len(data[1]) == 1
+    assert data[0]["hello"] == "world"
+    assert data[1]["test"] == 123
```

### Comparing `srsly-2.4.5.dev1/srsly/tests/test_msgpack_api.py` & `srsly-2.4.6/srsly/tests/test_msgpack_api.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/test_pickle_api.py` & `srsly-2.4.6/srsly/tests/test_pickle_api.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/test_yaml_api.py` & `srsly-2.4.6/srsly/tests/test_yaml_api.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ujson/334-reproducer.json` & `srsly-2.4.6/srsly/tests/ujson/334-reproducer.json`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/tests/ujson/test_ujson.py` & `srsly-2.4.6/srsly/tests/ujson/test_ujson.py`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/JSONtoObj.c` & `srsly-2.4.6/srsly/ujson/JSONtoObj.c`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/lib/dconv_wrapper.cc` & `srsly-2.4.6/srsly/ujson/lib/dconv_wrapper.cc`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/lib/ultrajson.h` & `srsly-2.4.6/srsly/ujson/lib/ultrajson.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/lib/ultrajsondec.c` & `srsly-2.4.6/srsly/ujson/lib/ultrajsondec.c`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/lib/ultrajsonenc.c` & `srsly-2.4.6/srsly/ujson/lib/ultrajsonenc.c`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/objToJSON.c` & `srsly-2.4.6/srsly/ujson/objToJSON.c`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/py_defines.h` & `srsly-2.4.6/srsly/ujson/py_defines.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/ujson.c` & `srsly-2.4.6/srsly/ujson/ujson.c`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/ujson/version.h` & `srsly-2.4.6/srsly/ujson/version.h`

 * *Files identical despite different names*

### Comparing `srsly-2.4.5.dev1/srsly/util.py` & `srsly-2.4.6/srsly/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 # fmt: off
 FilePath = Union[str, Path]
 # Superficial JSON input/output types
 # https://github.com/python/typing/issues/182#issuecomment-186684288
 JSONOutput = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
 JSONOutputBin = Union[bytes, str, int, float, bool, None, Dict[str, Any], List[Any]]
 # For input, we also accept tuples, ordered dicts etc.
-JSONInput = Union[str, int, float, bool, None, Dict[str, Any], List[Any], Tuple[Any], OrderedDict]
-JSONInputBin = Union[bytes, str, int, float, bool, None, Dict[str, Any], List[Any], Tuple[Any], OrderedDict]
+JSONInput = Union[str, int, float, bool, None, Dict[str, Any], List[Any], Tuple[Any, ...], OrderedDict]
+JSONInputBin = Union[bytes, str, int, float, bool, None, Dict[str, Any], List[Any], Tuple[Any, ...], OrderedDict]
 YAMLInput = JSONInput
 YAMLOutput = JSONOutput
 # fmt: on
 
 
 def force_path(location, require_exists=True):
     if not isinstance(location, Path):
```

### Comparing `srsly-2.4.5.dev1/srsly.egg-info/PKG-INFO` & `srsly-2.4.6/srsly.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsly
-Version: 2.4.5.dev1
+Version: 2.4.6
 Summary: Modern high-performance serialization utilities for Python
 Home-page: https://github.com/explosion/srsly
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -43,15 +43,15 @@
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
 
 ## Motivation
 
 Serialization is hard, especially across Python versions and multiple platforms.
 After dealing with many subtle bugs over the years (encodings, locales, large
 files) our libraries like [spaCy](https://github.com/explosion/spaCy) and
-[Prodigy](https://prodi.gy) have steadily grown a number of utility functions to
+[Prodigy](https://prodi.gy) had steadily grown a number of utility functions to
 wrap the multiple serialization formats we need to support (especially `json`,
 `msgpack` and `pickle`). These wrapping functions ended up duplicated across our
 codebases, so we wanted to put them in one place.
 
 At the same time, we noticed that having a lot of small dependencies was making
 maintenance harder, and making installation slower. To solve this, we've made
 `srsly` standalone, by including the component packages directly within it. This
@@ -70,32 +70,57 @@
 
 > ⚠️ Note that `v2.x` is only compatible with **Python 3.6+**. For 2.7+ compatibility, use `v1.x`.
 
 `srsly` can be installed from pip. Before installing, make sure that your `pip`,
 `setuptools` and `wheel` are up to date.
 
 ```bash
-pip install -U pip setuptools wheel
-pip install srsly
+python -m pip install -U pip setuptools wheel
+python -m pip install srsly
 ```
 
 Or from conda via conda-forge:
 
 ```bash
 conda install -c conda-forge srsly
 ```
 
 Alternatively, you can also compile the library from source. You'll need to make
-sure that you have a development environment consisting of a Python distribution
+sure that you have a development environment with a Python distribution
 including header files, a compiler (XCode command-line tools on macOS / OS X or
-Visual C++ build tools on Windows), pip, virtualenv and git installed.
+Visual C++ build tools on Windows), pip and git installed.
+
+Install from source:
 
 ```bash
-pip install -r requirements.txt  # install development dependencies
-python setup.py build_ext --inplace  # compile the library
+# clone the repo
+git clone https://github.com/explosion/srsly
+cd srsly
+
+# create a virtual environment
+python -m venv .env
+source .env/bin/activate
+
+# update pip
+python -m pip install -U pip setuptools wheel
+
+# compile and install from source
+python -m pip install .
+```
+
+For developers, install requirements separately and then install in editable
+mode without build isolation:
+
+```bash
+# install in editable mode
+python -m pip install -r requirements.txt
+python -m pip install --no-build-isolation --editable .
+
+# run test suite
+python -m pytest --pyargs srsly
 ```
 
 ## API
 
 ### JSON
 
 > 📦 The underlying module is exposed via `srsly.ujson`. However, we normally
@@ -136,74 +161,103 @@
 Create a JSON file and dump contents or write to standard output.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_json("/path/to/file.json", data)
 ```
 
-| Argument   | Type         | Description                                            |
-| ---------- | ------------ | ------------------------------------------------------ |
-| `path` | str / `Path` | The file path or `"-"` to write to stdout.             |
-| `data`     | -            | The JSON-serializable data to output.                  |
-| `indent`   | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+| Argument | Type         | Description                                            |
+| -------- | ------------ | ------------------------------------------------------ |
+| `path`   | str / `Path` | The file path or `"-"` to write to stdout.             |
+| `data`   | -            | The JSON-serializable data to output.                  |
+| `indent` | int          | Number of spaces used to indent JSON. Defaults to `2`. |
 
 #### <kbd>function</kbd> `srsly.read_json`
 
 Load JSON from a file or standard input.
 
 ```python
 data = srsly.read_json("/path/to/file.json")
 ```
 
 | Argument    | Type         | Description                                |
 | ----------- | ------------ | ------------------------------------------ |
-| `path`  | str / `Path` | The file path or `"-"` to read from stdin. |
+| `path`      | str / `Path` | The file path or `"-"` to read from stdin. |
 | **RETURNS** | dict / list  | The loaded JSON content.                   |
 
 #### <kbd>function</kbd> `srsly.write_gzip_json`
 
 Create a gzipped JSON file and dump contents.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_gzip_json("/path/to/file.json.gz", data)
 ```
 
-| Argument   | Type         | Description                                            |
-| ---------- | ------------ | ------------------------------------------------------ |
-| `path` | str / `Path` | The file path.                                         |
-| `data`     | -            | The JSON-serializable data to output.                  |
-| `indent`   | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+| Argument | Type         | Description                                            |
+| -------- | ------------ | ------------------------------------------------------ |
+| `path`   | str / `Path` | The file path.                                         |
+| `data`   | -            | The JSON-serializable data to output.                  |
+| `indent` | int          | Number of spaces used to indent JSON. Defaults to `2`. |
+
+#### <kbd>function</kbd> `srsly.write_gzip_jsonl`
+
+Create a gzipped JSONL file and dump contents.
+
+```python
+data = [{"foo": "bar"}, {"baz": 123}]
+srsly.write_gzip_json("/path/to/file.jsonl.gz", data)
+```
+
+| Argument          | Type         | Description                                                                                                                                                                                                             |
+| ----------------- | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `path`            | str / `Path` | The file path.                                                                                                                                                                                                          |
+| `lines`           | -            | The JSON-serializable contents of each line.                                                                                                                                                                            |
+| `append`          | bool         | Whether or not to append to the location. Appending to .gz files is generally not recommended, as it doesn't allow the algorithm to take advantage of all data when compressing - files may hence be poorly compressed. |
+| `append_new_line` | bool         | Whether or not to write a new line before appending to the file.                                                                                                                                                        |
 
 #### <kbd>function</kbd> `srsly.read_gzip_json`
 
 Load gzipped JSON from a file.
 
 ```python
 data = srsly.read_gzip_json("/path/to/file.json.gz")
 ```
 
 | Argument    | Type         | Description              |
 | ----------- | ------------ | ------------------------ |
-| `path`  | str / `Path` | The file path.           |
+| `path`      | str / `Path` | The file path.           |
 | **RETURNS** | dict / list  | The loaded JSON content. |
 
+#### <kbd>function</kbd> `srsly.read_gzip_jsonl`
+
+Load gzipped JSONL from a file.
+
+```python
+data = srsly.read_gzip_jsonl("/path/to/file.jsonl.gz")
+```
+
+| Argument    | Type         | Description               |
+| ----------- | ------------ | ------------------------- |
+| `path`      | str / `Path` | The file path.            |
+| **RETURNS** | dict / list  | The loaded JSONL content. |
+
 #### <kbd>function</kbd> `srsly.write_jsonl`
 
 Create a JSONL file (newline-delimited JSON) and dump contents line by line, or
 write to standard output.
 
 ```python
 data = [{"foo": "bar"}, {"baz": 123}]
 srsly.write_jsonl("/path/to/file.jsonl", data)
 ```
 
 | Argument          | Type         | Description                                                                                                            |
 | ----------------- | ------------ | ---------------------------------------------------------------------------------------------------------------------- |
-| `path`        | str / `Path` | The file path or `"-"` to write to stdout.                                                                             |
+| `path`            | str / `Path` | The file path or `"-"` to write to stdout.                                                                             |
 | `lines`           | iterable     | The JSON-serializable lines.                                                                                           |
 | `append`          | bool         | Append to an existing file. Will open it in `"a"` mode and insert a newline before writing lines. Defaults to `False`. |
 | `append_new_line` | bool         | Defines whether a new line should first be written when appending to an existing file. Defaults to `True`.             |
 
 #### <kbd>function</kbd> `srsly.read_jsonl`
 
 Read a JSONL file (newline-delimited JSON) or from JSONL data from standard
@@ -211,15 +265,15 @@
 
 ```python
 data = srsly.read_jsonl("/path/to/file.jsonl")
 ```
 
 | Argument   | Type       | Description                                                          |
 | ---------- | ---------- | -------------------------------------------------------------------- |
-| `path` | str / Path | The file path or `"-"` to read from stdin.                           |
+| `path`     | str / Path | The file path or `"-"` to read from stdin.                           |
 | `skip`     | bool       | Skip broken lines and don't raise `ValueError`. Defaults to `False`. |
 | **YIELDS** | -          | The loaded JSON contents of each line.                               |
 
 #### <kbd>function</kbd> `srsly.is_json_serializable`
 
 Check if a Python object is JSON-serializable.
 
@@ -272,30 +326,30 @@
 Create a msgpack file and dump contents.
 
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_msgpack("/path/to/file.msg", data)
 ```
 
-| Argument   | Type         | Description            |
-| ---------- | ------------ | ---------------------- |
-| `path` | str / `Path` | The file path.         |
-| `data`     | -            | The data to serialize. |
+| Argument | Type         | Description            |
+| -------- | ------------ | ---------------------- |
+| `path`   | str / `Path` | The file path.         |
+| `data`   | -            | The data to serialize. |
 
 #### <kbd>function</kbd> `srsly.read_msgpack`
 
 Load a msgpack file.
 
 ```python
 data = srsly.read_msgpack("/path/to/file.msg")
 ```
 
 | Argument    | Type         | Description                                                                             |
 | ----------- | ------------ | --------------------------------------------------------------------------------------- |
-| `path`  | str / `Path` | The file path.                                                                          |
+| `path`      | str / `Path` | The file path.                                                                          |
 | `use_list`  | bool         | Don't use tuples instead of lists. Can make deserialization slower. Defaults to `True`. |
 | **RETURNS** | -            | The loaded and deserialized content.                                                    |
 
 ### pickle
 
 > 📦 The underlying module is exposed via `srsly.cloudpickle`. However, we
 > normally interact with it via the utility functions only.
@@ -343,15 +397,15 @@
 yaml_string = srsly.yaml_dumps(data)
 ```
 
 | Argument          | Type | Description                                |
 | ----------------- | ---- | ------------------------------------------ |
 | `data`            | -    | The JSON-serializable data to output.      |
 | `indent_mapping`  | int  | Mapping indentation. Defaults to `2`.      |
-| `indent_sequence` | int  | Sequence indentation. Defaults to `4`.      |
+| `indent_sequence` | int  | Sequence indentation. Defaults to `4`.     |
 | `indent_offset`   | int  | Indentation offset. Defaults to `2`.       |
 | `sort_keys`       | bool | Sort dictionary keys. Defaults to `False`. |
 | **RETURNS**       | str  | The serialized string.                     |
 
 #### <kbd>function</kbd> `srsly.yaml_loads`
 
 Deserialize unicode or a file object to a Python object.
@@ -373,32 +427,32 @@
 ```python
 data = {"foo": "bar", "baz": 123}
 srsly.write_yaml("/path/to/file.yml", data)
 ```
 
 | Argument          | Type         | Description                                |
 | ----------------- | ------------ | ------------------------------------------ |
-| `path`        | str / `Path` | The file path or `"-"` to write to stdout. |
+| `path`            | str / `Path` | The file path or `"-"` to write to stdout. |
 | `data`            | -            | The JSON-serializable data to output.      |
 | `indent_mapping`  | int          | Mapping indentation. Defaults to `2`.      |
-| `indent_sequence` | int          | Sequence indentation. Defaults to `4`.      |
+| `indent_sequence` | int          | Sequence indentation. Defaults to `4`.     |
 | `indent_offset`   | int          | Indentation offset. Defaults to `2`.       |
 | `sort_keys`       | bool         | Sort dictionary keys. Defaults to `False`. |
 
 #### <kbd>function</kbd> `srsly.read_yaml`
 
 Load YAML from a file or standard input.
 
 ```python
 data = srsly.read_yaml("/path/to/file.yml")
 ```
 
 | Argument    | Type         | Description                                |
 | ----------- | ------------ | ------------------------------------------ |
-| `path`  | str / `Path` | The file path or `"-"` to read from stdin. |
+| `path`      | str / `Path` | The file path or `"-"` to read from stdin. |
 | **RETURNS** | dict / list  | The loaded YAML content.                   |
 
 #### <kbd>function</kbd> `srsly.is_yaml_serializable`
 
 Check if a Python object is YAML-serializable.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: srsly Version: 2.4.5.dev1 Summary: Modern high-
+Metadata-Version: 2.1 Name: srsly Version: 2.4.6 Summary: Modern high-
 performance serialization utilities for Python Home-page: https://github.com/
 explosion/srsly Author: Explosion Author-email: contact@explosion.ai License:
 MIT Classifier: Development Status :: 5 - Production/Stable Classifier:
 Environment :: Console Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
@@ -30,93 +30,116 @@
 all.svg?style=flat-square&logo=github)](https://github.com/explosion/srsly) [!
 [Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
 4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://
 github.com/explosion/wheelwright/releases) ## Motivation Serialization is hard,
 especially across Python versions and multiple platforms. After dealing with
 many subtle bugs over the years (encodings, locales, large files) our libraries
 like [spaCy](https://github.com/explosion/spaCy) and [Prodigy](https://
-prodi.gy) have steadily grown a number of utility functions to wrap the
-multiple serialization formats we need to support (especially `json`, `msgpack`
-and `pickle`). These wrapping functions ended up duplicated across our
-codebases, so we wanted to put them in one place. At the same time, we noticed
-that having a lot of small dependencies was making maintenance harder, and
-making installation slower. To solve this, we've made `srsly` standalone, by
-including the component packages directly within it. This way we can provide
-all the serialization utilities we need in a single binary wheel. `srsly`
-currently includes forks of the following packages: - [`ujson`](https://
-github.com/esnme/ultrajson) - [`msgpack`](https://github.com/msgpack/msgpack-
-python) - [`msgpack-numpy`](https://github.com/lebedov/msgpack-numpy) -
-[`cloudpickle`](https://github.com/cloudpipe/cloudpickle) - [`ruamel.yaml`]
-(https://github.com/pycontribs/ruamel-yaml) (without unsafe implementations!)
-## Installation > â ï¸ Note that `v2.x` is only compatible with **Python
-3.6+**. For 2.7+ compatibility, use `v1.x`. `srsly` can be installed from pip.
-Before installing, make sure that your `pip`, `setuptools` and `wheel` are up
-to date. ```bash pip install -U pip setuptools wheel pip install srsly ``` Or
-from conda via conda-forge: ```bash conda install -c conda-forge srsly ```
-Alternatively, you can also compile the library from source. You'll need to
-make sure that you have a development environment consisting of a Python
+prodi.gy) had steadily grown a number of utility functions to wrap the multiple
+serialization formats we need to support (especially `json`, `msgpack` and
+`pickle`). These wrapping functions ended up duplicated across our codebases,
+so we wanted to put them in one place. At the same time, we noticed that having
+a lot of small dependencies was making maintenance harder, and making
+installation slower. To solve this, we've made `srsly` standalone, by including
+the component packages directly within it. This way we can provide all the
+serialization utilities we need in a single binary wheel. `srsly` currently
+includes forks of the following packages: - [`ujson`](https://github.com/esnme/
+ultrajson) - [`msgpack`](https://github.com/msgpack/msgpack-python) -
+[`msgpack-numpy`](https://github.com/lebedov/msgpack-numpy) - [`cloudpickle`]
+(https://github.com/cloudpipe/cloudpickle) - [`ruamel.yaml`](https://
+github.com/pycontribs/ruamel-yaml) (without unsafe implementations!) ##
+Installation > â ï¸ Note that `v2.x` is only compatible with **Python 3.6+**.
+For 2.7+ compatibility, use `v1.x`. `srsly` can be installed from pip. Before
+installing, make sure that your `pip`, `setuptools` and `wheel` are up to date.
+```bash python -m pip install -U pip setuptools wheel python -m pip install
+srsly ``` Or from conda via conda-forge: ```bash conda install -c conda-forge
+srsly ``` Alternatively, you can also compile the library from source. You'll
+need to make sure that you have a development environment with a Python
 distribution including header files, a compiler (XCode command-line tools on
-macOS / OS X or Visual C++ build tools on Windows), pip, virtualenv and git
-installed. ```bash pip install -r requirements.txt # install development
-dependencies python setup.py build_ext --inplace # compile the library ``` ##
-API ### JSON > ð¦ The underlying module is exposed via `srsly.ujson`.
-However, we normally > interact with it via the utility functions only. ####
-function `srsly.json_dumps` Serialize an object to a JSON string. Falls back to
-`json` if `sort_keys=True` is used (until it's fixed in `ujson`). ```python
-data = {"foo": "bar", "baz": 123} json_string = srsly.json_dumps(data) ``` |
-Argument | Type | Description | | ----------- | ---- | ------------------------
------------------------------- | | `data` | - | The JSON-serializable data to
-output. | | `indent` | int | Number of spaces used to indent JSON. Defaults to
-`0`. | | `sort_keys` | bool | Sort dictionary keys. Defaults to `False`. | |
-**RETURNS** | str | The serialized string. | #### function `srsly.json_loads`
-Deserialize unicode or bytes to a Python object. ```python data = '{"foo":
-"bar", "baz": 123}' obj = srsly.json_loads(data) ``` | Argument | Type |
-Description | | ----------- | ----------- | ------------------------------- | |
-`data` | str / bytes | The data to deserialize. | | **RETURNS** | - | The
-deserialized Python object. | #### function `srsly.write_json` Create a JSON
-file and dump contents or write to standard output. ```python data = {"foo":
-"bar", "baz": 123} srsly.write_json("/path/to/file.json", data) ``` | Argument
-| Type | Description | | ---------- | ------------ | --------------------------
----------------------------- | | `path` | str / `Path` | The file path or `"-"`
-to write to stdout. | | `data` | - | The JSON-serializable data to output. | |
-`indent` | int | Number of spaces used to indent JSON. Defaults to `2`. | ####
-function `srsly.read_json` Load JSON from a file or standard input. ```python
-data = srsly.read_json("/path/to/file.json") ``` | Argument | Type |
-Description | | ----------- | ------------ | ----------------------------------
--------- | | `path` | str / `Path` | The file path or `"-"` to read from stdin.
-| | **RETURNS** | dict / list | The loaded JSON content. | #### function
+macOS / OS X or Visual C++ build tools on Windows), pip and git installed.
+Install from source: ```bash # clone the repo git clone https://github.com/
+explosion/srsly cd srsly # create a virtual environment python -m venv .env
+source .env/bin/activate # update pip python -m pip install -U pip setuptools
+wheel # compile and install from source python -m pip install . ``` For
+developers, install requirements separately and then install in editable mode
+without build isolation: ```bash # install in editable mode python -m pip
+install -r requirements.txt python -m pip install --no-build-isolation --
+editable . # run test suite python -m pytest --pyargs srsly ``` ## API ### JSON
+> ð¦ The underlying module is exposed via `srsly.ujson`. However, we normally
+> interact with it via the utility functions only. #### function
+`srsly.json_dumps` Serialize an object to a JSON string. Falls back to `json`
+if `sort_keys=True` is used (until it's fixed in `ujson`). ```python data =
+{"foo": "bar", "baz": 123} json_string = srsly.json_dumps(data) ``` | Argument
+| Type | Description | | ----------- | ---- | ---------------------------------
+--------------------- | | `data` | - | The JSON-serializable data to output. |
+| `indent` | int | Number of spaces used to indent JSON. Defaults to `0`. | |
+`sort_keys` | bool | Sort dictionary keys. Defaults to `False`. | | **RETURNS**
+| str | The serialized string. | #### function `srsly.json_loads` Deserialize
+unicode or bytes to a Python object. ```python data = '{"foo": "bar", "baz":
+123}' obj = srsly.json_loads(data) ``` | Argument | Type | Description | | ----
+------- | ----------- | ------------------------------- | | `data` | str /
+bytes | The data to deserialize. | | **RETURNS** | - | The deserialized Python
+object. | #### function `srsly.write_json` Create a JSON file and dump contents
+or write to standard output. ```python data = {"foo": "bar", "baz": 123}
+srsly.write_json("/path/to/file.json", data) ``` | Argument | Type |
+Description | | -------- | ------------ | -------------------------------------
+----------------- | | `path` | str / `Path` | The file path or `"-"` to write
+to stdout. | | `data` | - | The JSON-serializable data to output. | | `indent`
+| int | Number of spaces used to indent JSON. Defaults to `2`. | #### function
+`srsly.read_json` Load JSON from a file or standard input. ```python data =
+srsly.read_json("/path/to/file.json") ``` | Argument | Type | Description | | -
+---------- | ------------ | ------------------------------------------ | |
+`path` | str / `Path` | The file path or `"-"` to read from stdin. | |
+**RETURNS** | dict / list | The loaded JSON content. | #### function
 `srsly.write_gzip_json` Create a gzipped JSON file and dump contents. ```python
 data = {"foo": "bar", "baz": 123} srsly.write_gzip_json("/path/to/
-file.json.gz", data) ``` | Argument | Type | Description | | ---------- | -----
-------- | ------------------------------------------------------ | | `path` |
-str / `Path` | The file path. | | `data` | - | The JSON-serializable data to
+file.json.gz", data) ``` | Argument | Type | Description | | -------- | -------
+----- | ------------------------------------------------------ | | `path` | str
+/ `Path` | The file path. | | `data` | - | The JSON-serializable data to
 output. | | `indent` | int | Number of spaces used to indent JSON. Defaults to
-`2`. | #### function `srsly.read_gzip_json` Load gzipped JSON from a file.
-```python data = srsly.read_gzip_json("/path/to/file.json.gz") ``` | Argument |
-Type | Description | | ----------- | ------------ | ------------------------ |
-| `path` | str / `Path` | The file path. | | **RETURNS** | dict / list | The
-loaded JSON content. | #### function `srsly.write_jsonl` Create a JSONL file
-(newline-delimited JSON) and dump contents line by line, or write to standard
-output. ```python data = [{"foo": "bar"}, {"baz": 123}] srsly.write_jsonl("/
-path/to/file.jsonl", data) ``` | Argument | Type | Description | | ------------
------ | ------------ | --------------------------------------------------------
--------------------------------------------------------------- | | `path` | str
-/ `Path` | The file path or `"-"` to write to stdout. | | `lines` | iterable |
-The JSON-serializable lines. | | `append` | bool | Append to an existing file.
-Will open it in `"a"` mode and insert a newline before writing lines. Defaults
-to `False`. | | `append_new_line` | bool | Defines whether a new line should
-first be written when appending to an existing file. Defaults to `True`. | ####
-function `srsly.read_jsonl` Read a JSONL file (newline-delimited JSON) or from
-JSONL data from standard input and yield contents line by line. Blank lines
-will always be skipped. ```python data = srsly.read_jsonl("/path/to/
-file.jsonl") ``` | Argument | Type | Description | | ---------- | ---------- |
--------------------------------------------------------------------- | | `path`
-| str / Path | The file path or `"-"` to read from stdin. | | `skip` | bool |
-Skip broken lines and don't raise `ValueError`. Defaults to `False`. | |
-**YIELDS** | - | The loaded JSON contents of each line. | #### function
+`2`. | #### function `srsly.write_gzip_jsonl` Create a gzipped JSONL file and
+dump contents. ```python data = [{"foo": "bar"}, {"baz": 123}]
+srsly.write_gzip_json("/path/to/file.jsonl.gz", data) ``` | Argument | Type |
+Description | | ----------------- | ------------ | ----------------------------
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+----------------------------- | | `path` | str / `Path` | The file path. | |
+`lines` | - | The JSON-serializable contents of each line. | | `append` | bool
+| Whether or not to append to the location. Appending to .gz files is generally
+not recommended, as it doesn't allow the algorithm to take advantage of all
+data when compressing - files may hence be poorly compressed. | |
+`append_new_line` | bool | Whether or not to write a new line before appending
+to the file. | #### function `srsly.read_gzip_json` Load gzipped JSON from a
+file. ```python data = srsly.read_gzip_json("/path/to/file.json.gz") ``` |
+Argument | Type | Description | | ----------- | ------------ | ----------------
+-------- | | `path` | str / `Path` | The file path. | | **RETURNS** | dict /
+list | The loaded JSON content. | #### function `srsly.read_gzip_jsonl` Load
+gzipped JSONL from a file. ```python data = srsly.read_gzip_jsonl("/path/to/
+file.jsonl.gz") ``` | Argument | Type | Description | | ----------- | ---------
+--- | ------------------------- | | `path` | str / `Path` | The file path. | |
+**RETURNS** | dict / list | The loaded JSONL content. | #### function
+`srsly.write_jsonl` Create a JSONL file (newline-delimited JSON) and dump
+contents line by line, or write to standard output. ```python data = [{"foo":
+"bar"}, {"baz": 123}] srsly.write_jsonl("/path/to/file.jsonl", data) ``` |
+Argument | Type | Description | | ----------------- | ------------ | ----------
+-------------------------------------------------------------------------------
+----------------------------- | | `path` | str / `Path` | The file path or `"-
+"` to write to stdout. | | `lines` | iterable | The JSON-serializable lines. |
+| `append` | bool | Append to an existing file. Will open it in `"a"` mode and
+insert a newline before writing lines. Defaults to `False`. | |
+`append_new_line` | bool | Defines whether a new line should first be written
+when appending to an existing file. Defaults to `True`. | #### function
+`srsly.read_jsonl` Read a JSONL file (newline-delimited JSON) or from JSONL
+data from standard input and yield contents line by line. Blank lines will
+always be skipped. ```python data = srsly.read_jsonl("/path/to/file.jsonl") ```
+| Argument | Type | Description | | ---------- | ---------- | -----------------
+--------------------------------------------------- | | `path` | str / Path |
+The file path or `"-"` to read from stdin. | | `skip` | bool | Skip broken
+lines and don't raise `ValueError`. Defaults to `False`. | | **YIELDS** | - |
+The loaded JSON contents of each line. | #### function
 `srsly.is_json_serializable` Check if a Python object is JSON-serializable.
 ```python assert srsly.is_json_serializable({"hello": "world"}) is True assert
 srsly.is_json_serializable(lambda x: x) is False ``` | Argument | Type |
 Description | | ----------- | ---- | ---------------------------------------- |
 | `obj` | - | The object to check. | | **RETURNS** | bool | Whether the object
 is JSON-serializable. | ### msgpack > ð¦ The underlying module is exposed via
 `srsly.msgpack`. However, we normally > interact with it via the utility
@@ -130,16 +153,16 @@
 Argument | Type | Description | | ----------- | ----- | -----------------------
 ---------------------------------------------------------------- | | `data` |
 bytes | The data to deserialize. | | `use_list` | bool | Don't use tuples
 instead of lists. Can make deserialization slower. Defaults to `True`. | |
 **RETURNS** | - | The deserialized Python object. | #### function
 `srsly.write_msgpack` Create a msgpack file and dump contents. ```python data =
 {"foo": "bar", "baz": 123} srsly.write_msgpack("/path/to/file.msg", data) ``` |
-Argument | Type | Description | | ---------- | ------------ | -----------------
------ | | `path` | str / `Path` | The file path. | | `data` | - | The data to
+Argument | Type | Description | | -------- | ------------ | -------------------
+--- | | `path` | str / `Path` | The file path. | | `data` | - | The data to
 serialize. | #### function `srsly.read_msgpack` Load a msgpack file. ```python
 data = srsly.read_msgpack("/path/to/file.msg") ``` | Argument | Type |
 Description | | ----------- | ------------ | ----------------------------------
 ----------------------------------------------------- | | `path` | str / `Path`
 | The file path. | | `use_list` | bool | Don't use tuples instead of lists. Can
 make deserialization slower. Defaults to `True`. | | **RETURNS** | - | The
 loaded and deserialized content. | ### pickle > ð¦ The underlying module is
```

### Comparing `srsly-2.4.5.dev1/srsly.egg-info/SOURCES.txt` & `srsly-2.4.6/srsly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

