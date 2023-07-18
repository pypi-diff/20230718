# Comparing `tmp/sts_libs-0.0.6.dev3.tar.gz` & `tmp/sts_libs-0.0.6.dev4.tar.gz`

## Comparing `sts_libs-0.0.6.dev3.tar` & `sts_libs-0.0.6.dev4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/__about__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    41654 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    48813 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    45059 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    66092 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    36056 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35919 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42566 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17994 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    28271 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22459 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/log.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/LICENSE
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/pyproject.toml
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/README.md
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    41654 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    48813 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    45059 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    66092 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    36056 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35919 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42566 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17994 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    28271 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22459 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/log.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/LICENSE
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/pyproject.toml
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/sts_libs/README.md
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev4/PKG-INFO
```

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/dm.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/dmpd.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/fc.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/fio.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/iscsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/linux.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/linux.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/lio.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/lio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/loopdev.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/lvm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/md.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/mp.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/mp.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/net.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/net.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/scsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/stratis.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/stratis.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/vdo.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/beaker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/cmdline.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """Runs cmd and returns rc int or rc int, output str tuple.
 
     For legacy compatibility only. TODO: remove it an it's usages
     """
     completed_command = host.run(cmd)
 
     if return_output:
-        output = completed_command.stdout if completed_command.stdout else completed_command.stderr
+        output = completed_command.stdout.rstrip if completed_command.stdout else completed_command.stderr.rstrip()
         return completed_command.rc, output  # type: ignore [return-value]
 
     return completed_command.rc
 
 
 def exists(cmd: str) -> bool:
     return host.exists(cmd)
```

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/logchecker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.6.dev4/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/cmdline_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/fio_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/linux_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/md_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/net_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.6.dev4/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/.gitignore` & `sts_libs-0.0.6.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/LICENSE` & `sts_libs-0.0.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/pyproject.toml` & `sts_libs-0.0.6.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/sts_libs/README.md` & `sts_libs-0.0.6.dev4/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev3/PKG-INFO` & `sts_libs-0.0.6.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.6.dev3
+Version: 0.0.6.dev4
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
```

