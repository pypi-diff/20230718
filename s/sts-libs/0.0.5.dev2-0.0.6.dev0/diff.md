# Comparing `tmp/sts_libs-0.0.5.dev2.tar.gz` & `tmp/sts_libs-0.0.6.dev0.tar.gz`

## Comparing `sts_libs-0.0.5.dev2.tar` & `sts_libs-0.0.6.dev0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    42305 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17423 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    50372 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    46948 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    66740 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    36092 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42709 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    28690 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    17167 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    23142 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/atomic_run.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0    12491 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/LICENSE
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/sts_libs/README.md
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev2/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    41654 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    45050 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    66092 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    36056 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35901 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42548 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17985 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    28199 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22450 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/log.py
+-rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/LICENSE
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/sts_libs/README.md
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev0/PKG-INFO
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/dm.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/dm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,174 @@
 """dm.py: Module to manipulate Device mapper devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
-import re  # regex
+import logging
+import re
 
 from sts.utils.cmdline import run, run_ret_out
 
 
 def dm_show_status(dm_device=None):  # noqa: ANN001, ANN201
     """Show dmsetup status.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     True
     or
     False.
     """
-    cmd = "dmsetup status"
+    cmd = 'dmsetup status'
     if dm_device:
-        cmd += f" {dm_device}"
+        cmd += f' {dm_device}'
 
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not show dmsetup status")
+    if run(cmd).rc != 0:
+        logging.error('Could not show dmsetup status')
         return False
     return True
 
 
 def dm_query_status(dm_device=None):  # noqa: ANN001, ANN201
     """Query dmsetup status and return a dictionary with table output for each device.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     dict: Return a dictionary with status info for each device.
     """
-    cmd = "dmsetup status"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = 'dmsetup status'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Could not list status")
+        logging.error('Could not list status')
         return None
-    devices = output.split("\n")
+    devices = output.split('\n')
 
-    status_basic_format_regex = r"(.*):\s+(\d+)\s+(\d+)\s+(\S+)"
+    status_basic_format_regex = r'(.*):\s+(\d+)\s+(\d+)\s+(\S+)'
     # Thin formats are available on: https://www.kernel.org/doc/Documentation/device-mapper/thin-provisioning.txt
-    status_thin_format_regex = status_basic_format_regex + r"\s+(\d+)\s+(\d+|-)"
-    status_thin_pool_format_regex = status_basic_format_regex + r"\s+(\d+)\s+(\d+)\/(\d+)\s+(\d+)\/(\d+)(.*)"
+    status_thin_format_regex = status_basic_format_regex + r'\s+(\d+)\s+(\d+|-)'
+    status_thin_pool_format_regex = status_basic_format_regex + r'\s+(\d+)\s+(\d+)\/(\d+)\s+(\d+)\/(\d+)(.*)'
     status_multipath_format_regex = (
-        status_basic_format_regex + r"\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(.*)"
+        status_basic_format_regex + r'\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(.*)'
     )
 
     dev_status_dict = {}
     for device in devices:
         m = re.match(status_basic_format_regex, device)
         if not m:
-            print(f"FAIL: dm_query_status() - ({device}) does not match dmsetup status output format")
+            logging.error(f'dm_query_status() - ({device}) does not match dmsetup status output format')
             continue
         dm_type = m.group(4)
         dm_status_format_dict = {}
-        if dm_type == "linear":
+        if dm_type == 'linear':
             dm_status_format_dict = {
-                "logical_start_sector": m.group(2),
-                "num_sec": m.group(3),
-                "target_type": dm_type,
+                'logical_start_sector': m.group(2),
+                'num_sec': m.group(3),
+                'target_type': dm_type,
             }
-        elif dm_type == "thin":
+        elif dm_type == 'thin':
             t = re.match(status_thin_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                logging.error(f'({device}) does not match dmsetup a valid {dm_type} table output format')
                 continue
             dm_status_format_dict = {
-                "logical_start_sector": t.group(2),
-                "num_sec": t.group(3),
-                "target_type": dm_type,
-                "nr_mapped_sec": t.group(5),
-                "highest_mapped_sec": t.group(6),
+                'logical_start_sector': t.group(2),
+                'num_sec': t.group(3),
+                'target_type': dm_type,
+                'nr_mapped_sec': t.group(5),
+                'highest_mapped_sec': t.group(6),
             }
-        elif dm_type == "thin-pool":
+        elif dm_type == 'thin-pool':
             t = re.match(status_thin_pool_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                logging.error(f'({device}) does not match dmsetup a valid {dm_type} table output format')
                 continue
             dm_status_format_dict = {
-                "logical_start_sector": t.group(2),
-                "num_sec": t.group(3),
-                "target_type": dm_type,
-                "trans_id": t.group(5),
-                "used_metadata": t.group(6),
-                "total_metadata": t.group(7),
-                "used_data_block": t.group(8),
-                "total_data_block": t.group(9),
-                "metadata": t.group(10),
+                'logical_start_sector': t.group(2),
+                'num_sec': t.group(3),
+                'target_type': dm_type,
+                'trans_id': t.group(5),
+                'used_metadata': t.group(6),
+                'total_metadata': t.group(7),
+                'used_data_block': t.group(8),
+                'total_data_block': t.group(9),
+                'metadata': t.group(10),
             }
-        elif dm_type == "multipath":
+        elif dm_type == 'multipath':
             t = re.match(status_multipath_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                logging.error(f'({device}) does not match dmsetup a valid {dm_type} table output format')
                 continue
             dm_status_format_dict = {
-                "logical_start_sector": m.group(2),
-                "num_sec": m.group(3),
-                "target_type": dm_type,
-                "nr_status_feature": t.group(5),
-                "all_io_queued": t.group(6),
-                "nr_att_init_grp": t.group(7),
-                "nr_hw_handlers": t.group(8),
-                "nr_path_grps": t.group(9),
-                "active_path_grp": t.group(10),
+                'logical_start_sector': m.group(2),
+                'num_sec': m.group(3),
+                'target_type': dm_type,
+                'nr_status_feature': t.group(5),
+                'all_io_queued': t.group(6),
+                'nr_att_init_grp': t.group(7),
+                'nr_hw_handlers': t.group(8),
+                'nr_path_grps': t.group(9),
+                'active_path_grp': t.group(10),
             }
             remaining_data = t.group(11)
 
-            status_multipath_path_args_format_regex = r"\s+(\S+)"
-            status_multipath_path_format_regex = r"\s+(\S+)\s+(\S+)\s+(\S+)"
-            status_multipath_grp_header_format_regex = r"\s?(\S)\s+(\d+)\s+(\d+)\s+(\d+)"
+            status_multipath_path_args_format_regex = r'\s+(\S+)'
+            status_multipath_path_format_regex = r'\s+(\S+)\s+(\S+)\s+(\S+)'
+            status_multipath_grp_header_format_regex = r'\s?(\S)\s+(\d+)\s+(\d+)\s+(\d+)'
 
-            nr_groups = int(dm_status_format_dict["nr_path_grps"])
+            nr_groups = int(dm_status_format_dict['nr_path_grps'])
             for group_nr in range(1, int(nr_groups) + 1):
                 grp_match = re.match(status_multipath_grp_header_format_regex, remaining_data)
                 if not grp_match:
-                    print("FAIL: dm_query_status() - Could not parse group multipath data")
+                    logging.error('dm_query_status() - Could not parse group multipath data')
                     return None
-                if "path_grp" not in list(dm_status_format_dict.keys()):
-                    dm_status_format_dict["path_grp"] = {}
-                dm_status_format_dict["path_grp"][group_nr] = {}
-                path_grp = dm_status_format_dict["path_grp"][group_nr]
-                path_grp["state"] = grp_match.group(1)
-                path_grp["nr_grp_status_arg"] = grp_match.group(2)
-                path_grp["nr_paths"] = grp_match.group(3)
-                path_grp["nr_path_status_arg"] = grp_match.group(4)
-                nr_paths = int(path_grp["nr_paths"])  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
-                remaining_data = re.sub(status_multipath_grp_header_format_regex, "", remaining_data, 1)
+                if 'path_grp' not in list(dm_status_format_dict.keys()):
+                    dm_status_format_dict['path_grp'] = {}
+                dm_status_format_dict['path_grp'][group_nr] = {}
+                path_grp = dm_status_format_dict['path_grp'][group_nr]
+                path_grp['state'] = grp_match.group(1)
+                path_grp['nr_grp_status_arg'] = grp_match.group(2)
+                path_grp['nr_paths'] = grp_match.group(3)
+                path_grp['nr_path_status_arg'] = grp_match.group(4)
+                nr_paths = int(path_grp['nr_paths'])  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
+                remaining_data = re.sub(status_multipath_grp_header_format_regex, '', remaining_data, count=1)
                 for p_nr in range(1, int(nr_paths) + 1):
                     path_match = re.match(status_multipath_path_format_regex, remaining_data)
                     if not path_match:
-                        print("FAIL: dm_query_status() - Could not parse path multipath data")
+                        logging.error('dm_query_status() - Could not parse path multipath data')
                         return None
-                    if "path" not in list(path_grp.keys()):
-                        path_grp["path"] = {}
-                    path_grp["path"][p_nr] = {}  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
-                    path = path_grp["path"][p_nr]  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
-                    path["device"] = path_match.group(1)
-                    path["state"] = path_match.group(2)
-                    path["failure_cnt"] = path_match.group(3)
-                    remaining_data = re.sub(status_multipath_path_format_regex, "", remaining_data, 1)
+                    if 'path' not in list(path_grp.keys()):
+                        path_grp['path'] = {}
+                    path_grp['path'][p_nr] = {}  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
+                    path = path_grp['path'][p_nr]  # FIXME: Expected type 'Union[int, slice]', got 'str' instead
+                    path['device'] = path_match.group(1)
+                    path['state'] = path_match.group(2)
+                    path['failure_cnt'] = path_match.group(3)
+                    remaining_data = re.sub(status_multipath_path_format_regex, '', remaining_data, count=1)
                     for _ in range(1, int(grp_match.group(4)) + 1):
                         path_arg_match = re.match(status_multipath_path_args_format_regex, remaining_data)
                         if not path_arg_match:
-                            print("FAIL: dm_query_status() - Could not parse path args multipath data")
+                            logging.error('dm_query_status() - Could not parse path args multipath data')
                             return None
-                        if "path_status_args" not in list(path.keys()):
-                            path["path_status_args"] = ""
-                        path["path_status_args"] += f"{path_arg_match.group(1)} "
+                        if 'path_status_args' not in list(path.keys()):
+                            path['path_status_args'] = ''
+                        path['path_status_args'] += f'{path_arg_match.group(1)} '
                         remaining_data = re.sub(
                             status_multipath_path_args_format_regex,
-                            "",
+                            '',
                             remaining_data,
-                            1,
+                            count=1,
                         )
                     # remove trailing space from the end of string
-                    if "path_status_args" in list(path.keys()):
-                        path["path_status_args"] = path["path_status_args"].strip()
+                    if 'path_status_args' in list(path.keys()):
+                        path['path_status_args'] = path['path_status_args'].strip()
 
         else:
-            print(f"FAIL: dm_query_status() - ({device}) can't parse status for device type {dm_type}")
+            logging.error(f"dm_query_status() - ({device}) can't parse status for device type {dm_type}")
 
         dev_status_dict[m.group(1)] = dm_status_format_dict
     if dm_device:
         if dm_device in list(dev_status_dict.keys()):
             return dev_status_dict[dm_device]
         return None
     return dev_status_dict
@@ -179,198 +180,198 @@
     dm_device:           Device name (optional).
 
     Returns:
     True
     or
     False.
     """
-    cmd = "dmsetup table"
+    cmd = 'dmsetup table'
     if dm_device:
-        cmd += f" {dm_device}"
+        cmd += f' {dm_device}'
 
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not show dmsetup table")
+    if run(cmd).rc != 0:
+        logging.error('Could not show dmsetup table')
         return False
     return True
 
 
 def dm_query_table(dm_device=None):  # noqa: ANN001, ANN201
     """Query dmsetup table and return a dictionary with table output for each device.
     The arguments are:
     dm_device:           Device name (optional).
 
     Returns:
     dict: Return a dictionary with table info for each device.
     """
-    cmd = "dmsetup table"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = 'dmsetup table'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Could not list table")
+        logging.error('Could not list table')
         return None
-    devices = output.split("\n")
+    devices = output.split('\n')
 
     # Basic format information is found on man dmsetup under "TABLE FORMAT" section
     # format of dmsetup table: logical_start_sector num_sectors target_type target_args
-    table_basic_format_regex = r"(.*):\s+(\S+)\s+(\S+)\s+(\S+)"
+    table_basic_format_regex = r'(.*):\s+(\S+)\s+(\S+)\s+(\S+)'
     # format for linear type
-    table_linear_format_regex = table_basic_format_regex + r"\s+(\S+)\s+(\S+)$"
+    table_linear_format_regex = table_basic_format_regex + r'\s+(\S+)\s+(\S+)$'
     # vgtest-thin1: 0 2097152 thin 253:5 1
-    table_thin_format_regex = table_basic_format_regex + r"\s+(\S+)\s+(\S+)$"
+    table_thin_format_regex = table_basic_format_regex + r'\s+(\S+)\s+(\S+)$'
     # vgtest-test_pool-tpool: 0 1638400 thin-pool 253:3 253:4 512 0 1 error_if_no_space
-    table_thin_pool_format_regex = table_basic_format_regex + r"\s+(\S+)\s+(\S+)\s+(\S+)\s+(\S+)\s+(.*)$"
+    table_thin_pool_format_regex = table_basic_format_regex + r'\s+(\S+)\s+(\S+)\s+(\S+)\s+(\S+)\s+(.*)$'
     # delayed: 0 20971520 delay 7:0 0 100
-    table_delay_format_regex = table_basic_format_regex + r"\s+(\S+)\s+(\S+)\s+(\S+)$"
+    table_delay_format_regex = table_basic_format_regex + r'\s+(\S+)\s+(\S+)\s+(\S+)$'
 
     dev_table_dict = {}
     for device in devices:
         m = re.match(table_basic_format_regex, device)
         if not m:
-            print(f"FAIL: ({device}) does not match dmsetup table output format")
+            logging.error(f'({device}) does not match dmsetup table output format')
             continue
         dm_type = m.group(4)
         dm_table_format_dict = {}
-        if dm_type == "linear":
+        if dm_type == 'linear':
             t = re.match(table_linear_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid linear table output format")
+                logging.error(f'({device}) does not match dmsetup a valid linear table output format')
                 continue
             dm_table_format_dict = {
-                "logical_start_sector": t.group(2),
-                "num_sec": t.group(3),
-                "target_type": dm_type,
-                "dev": t.group(5),
-                "start_sec": t.group(6),
+                'logical_start_sector': t.group(2),
+                'num_sec': t.group(3),
+                'target_type': dm_type,
+                'dev': t.group(5),
+                'start_sec': t.group(6),
             }
-        elif dm_type == "thin":
+        elif dm_type == 'thin':
             t = re.match(table_thin_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                logging.error(f'({device}) does not match dmsetup a valid {dm_type} table output format')
                 continue
             dm_table_format_dict = {
-                "logical_start_sector": t.group(2),
-                "num_sec": t.group(3),
-                "target_type": dm_type,
-                "pool_dev": t.group(5),
-                "dev_num": t.group(6),
+                'logical_start_sector': t.group(2),
+                'num_sec': t.group(3),
+                'target_type': dm_type,
+                'pool_dev': t.group(5),
+                'dev_num': t.group(6),
             }
-        elif dm_type == "thin-pool":
+        elif dm_type == 'thin-pool':
             t = re.match(table_thin_pool_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                logging.error(f'({device}) does not match dmsetup a valid {dm_type} table output format')
                 continue
             dm_table_format_dict = {
-                "logical_start_sector": t.group(2),
-                "num_sec": t.group(3),
-                "target_type": dm_type,
-                "metadata_dev": t.group(5),
-                "data_dev": t.group(6),
-                "data_block_size": t.group(7),
-                "low_water_mark": t.group(8),
-                "target_args": t.group(9),
+                'logical_start_sector': t.group(2),
+                'num_sec': t.group(3),
+                'target_type': dm_type,
+                'metadata_dev': t.group(5),
+                'data_dev': t.group(6),
+                'data_block_size': t.group(7),
+                'low_water_mark': t.group(8),
+                'target_args': t.group(9),
             }
-        elif dm_type == "delay":
+        elif dm_type == 'delay':
             t = re.match(table_delay_format_regex, device)
             if not t:
-                print(f"FAIL: ({device}) does not match dmsetup a valid {dm_type} table output format")
+                logging.error(f'({device}) does not match dmsetup a valid {dm_type} table output format')
                 continue
             dm_table_format_dict = {
-                "logical_start_sector": t.group(2),
-                "num_sec": t.group(3),
-                "target_type": dm_type,
-                "dev": t.group(5),
-                "start_sec": t.group(6),
-                "delay": t.group(7),
+                'logical_start_sector': t.group(2),
+                'num_sec': t.group(3),
+                'target_type': dm_type,
+                'dev': t.group(5),
+                'start_sec': t.group(6),
+                'delay': t.group(7),
             }
-        elif dm_type == "multipath":
+        elif dm_type == 'multipath':
             # multipath table format see: http://christophe.varoqui.free.fr/refbook.html
-            device_params = device.split(" ")
+            device_params = device.split(' ')
             dm_table_format_dict = {
-                "logical_start_sector": m.group(2),
-                "num_sec": m.group(3),
-                "target_type": dm_type,
-                "nr_status_feature": int(device_params[4]),
+                'logical_start_sector': m.group(2),
+                'num_sec': m.group(3),
+                'target_type': dm_type,
+                'nr_status_feature': int(device_params[4]),
             }
             # set index to next entry after nr_status_feature
             param_index = 4 + 1
-            if dm_table_format_dict["nr_status_feature"] > 0:
-                dm_table_format_dict["features"] = []
-                for _ in range(dm_table_format_dict["nr_status_feature"]):
-                    dm_table_format_dict["features"].append(device_params[param_index])
+            if dm_table_format_dict['nr_status_feature'] > 0:
+                dm_table_format_dict['features'] = []
+                for _ in range(dm_table_format_dict['nr_status_feature']):
+                    dm_table_format_dict['features'].append(device_params[param_index])
                     param_index += 1
 
-            dm_table_format_dict["nr_hw_handlers"] = int(device_params[param_index])
+            dm_table_format_dict['nr_hw_handlers'] = int(device_params[param_index])
             param_index += 1
-            if dm_table_format_dict["nr_hw_handlers"] > 0:
-                dm_table_format_dict["hw_handlers"] = []
-                for _ in range(dm_table_format_dict["nr_hw_handlers"]):
-                    dm_table_format_dict["hw_handlers"].append(device_params[param_index])
+            if dm_table_format_dict['nr_hw_handlers'] > 0:
+                dm_table_format_dict['hw_handlers'] = []
+                for _ in range(dm_table_format_dict['nr_hw_handlers']):
+                    dm_table_format_dict['hw_handlers'].append(device_params[param_index])
                     param_index += 1
 
-            dm_table_format_dict["nr_path_grps"] = int(device_params[param_index])
+            dm_table_format_dict['nr_path_grps'] = int(device_params[param_index])
             param_index += 1
-            dm_table_format_dict["try_next_path_grp"] = device_params[param_index]
+            dm_table_format_dict['try_next_path_grp'] = device_params[param_index]
             param_index += 1
 
-            remaining_data = ""
+            remaining_data = ''
             for _ in range(len(device_params) - param_index):
-                remaining_data += f"{device_params[param_index]} "
+                remaining_data += f'{device_params[param_index]} '
                 param_index += 1
             remaining_data = remaining_data.strip()
 
-            table_multipath_grp_header_format_regex = r"\s?(\S+)\s+(\d+)\s+(\d+)\s+(\d+)"
-            table_multipath_path_header_format_regex = r"\s?(\S+)"
-            table_multipath_path_args_format_regex = r"\s?(\S+)"
-            nr_groups = dm_table_format_dict["nr_path_grps"]
+            table_multipath_grp_header_format_regex = r'\s?(\S+)\s+(\d+)\s+(\d+)\s+(\d+)'
+            table_multipath_path_header_format_regex = r'\s?(\S+)'
+            table_multipath_path_args_format_regex = r'\s?(\S+)'
+            nr_groups = dm_table_format_dict['nr_path_grps']
             for group_nr in range(1, int(nr_groups) + 1):
                 grp_match = re.match(table_multipath_grp_header_format_regex, remaining_data)
                 if not grp_match:
-                    print("FAIL: dm_query_table() - Could not parse group multipath data")
+                    logging.error('dm_query_table() - Could not parse group multipath data')
                     return None
-                if "path_grp" not in list(dm_table_format_dict.keys()):
-                    dm_table_format_dict["path_grp"] = {}
-                dm_table_format_dict["path_grp"][group_nr] = {}
-                path_grp = dm_table_format_dict["path_grp"][group_nr]
-                path_grp["path_selector"] = grp_match.group(1)
-                path_grp["nr_selector_args"] = grp_match.group(2)
-                path_grp["nr_paths_grp"] = grp_match.group(3)
-                path_grp["nr_path_args"] = grp_match.group(4)
+                if 'path_grp' not in list(dm_table_format_dict.keys()):
+                    dm_table_format_dict['path_grp'] = {}
+                dm_table_format_dict['path_grp'][group_nr] = {}
+                path_grp = dm_table_format_dict['path_grp'][group_nr]
+                path_grp['path_selector'] = grp_match.group(1)
+                path_grp['nr_selector_args'] = grp_match.group(2)
+                path_grp['nr_paths_grp'] = grp_match.group(3)
+                path_grp['nr_path_args'] = grp_match.group(4)
                 # remove processed data
-                remaining_data = re.sub(table_multipath_grp_header_format_regex, "", remaining_data, 1)
-                for path_nr in range(1, int(path_grp["nr_paths_grp"]) + 1):
+                remaining_data = re.sub(table_multipath_grp_header_format_regex, '', remaining_data, count=1)
+                for path_nr in range(1, int(path_grp['nr_paths_grp']) + 1):
                     path_match = re.match(table_multipath_path_header_format_regex, remaining_data)
                     if not path_match:
-                        print("FAIL: dm_query_table() - Could not parse path multipath data")
+                        logging.error('dm_query_table() - Could not parse path multipath data')
                         return None
-                    if "path" not in list(dm_table_format_dict.keys()):
-                        dm_table_format_dict["path"] = {}
-                    dm_table_format_dict["path"][path_nr] = {}
-                    path = dm_table_format_dict["path"][path_nr]
-                    path["device"] = path_match.group(1)
+                    if 'path' not in list(dm_table_format_dict.keys()):
+                        dm_table_format_dict['path'] = {}
+                    dm_table_format_dict['path'][path_nr] = {}
+                    path = dm_table_format_dict['path'][path_nr]
+                    path['device'] = path_match.group(1)
 
-                    remaining_data = re.sub(table_multipath_path_header_format_regex, "", remaining_data, 1)
-                    for _ in range(1, int(path_grp["nr_path_args"]) + 1):
+                    remaining_data = re.sub(table_multipath_path_header_format_regex, '', remaining_data, count=1)
+                    for _ in range(1, int(path_grp['nr_path_args']) + 1):
                         arg_match = re.match(table_multipath_path_args_format_regex, remaining_data)
                         if not arg_match:
-                            print("FAIL: dm_query_table() - Could not parse path arg multipath data")
+                            logging.error('dm_query_table() - Could not parse path arg multipath data')
                             return None
-                        if "path_status_args" not in list(path.keys()):
-                            path["path_status_args"] = ""
-                        path["path_status_args"] += f"{arg_match.group(1)} "
+                        if 'path_status_args' not in list(path.keys()):
+                            path['path_status_args'] = ''
+                        path['path_status_args'] += f'{arg_match.group(1)} '
                         remaining_data = re.sub(
                             table_multipath_path_args_format_regex,
-                            "",
+                            '',
                             remaining_data,
-                            1,
+                            count=1,
                         )
-                    if "path_status_args" in list(path.keys()):
+                    if 'path_status_args' in list(path.keys()):
                         # remove trailing space
-                        path["path_status_args"] = path["path_status_args"].strip()
+                        path['path_status_args'] = path['path_status_args'].strip()
 
         else:
-            print(f"FAIL: dm_query_table() - ({device}) can't parse table for device type '{dm_type}'")
+            logging.error(f"dm_query_table() - ({device}) can't parse table for device type '{dm_type}'")
         dev_table_dict[m.group(1)] = dm_table_format_dict
 
     if dm_device:
         if dm_device in list(dev_table_dict.keys()):
             return dev_table_dict[dm_device]
         return None
     return dev_table_dict
@@ -378,18 +379,18 @@
 
 def dm_get_table_device(dm_name):  # noqa: ANN001, ANN201
     """Get table information for specific device.
     The table info is not parsed.
     """
     if not dm_name:
         return None
-    cmd = f"dmsetup table {dm_name}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'dmsetup table {dm_name}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Could not query table for {dm_name}")
+        logging.error(f'Could not query table for {dm_name}')
         return None
 
     return output
 
 
 def dm_set_target_type(dm_name, target_type):  # noqa: ANN001, ANN201
     """Change the target type of specific DM device
@@ -397,34 +398,34 @@
     The arguments are:
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
-    table_format_regex = r"(\S+)\s+(\S+)\s+(\S+)\s(.*)$"
+    table_format_regex = r'(\S+)\s+(\S+)\s+(\S+)\s(.*)$'
     table_info = dm_get_table_device(dm_name)
     if not table_info:
         # Could not get table for device name
         return False
 
     # We need to suspend the device first
     if not dm_suspend_dev(dm_name):
         return False
 
     m = re.match(table_format_regex, table_info)
     if not m:
-        print(f"FAIL: dm_set_target_type() - ({table_info}) does not match dmsetup table output format")
+        logging.error(f'dm_set_target_type() - ({table_info}) does not match dmsetup table output format')
         return False
     # load the table with new target type
     new_table = f'"{m.group(1)} {m.group(2)} {target_type} {m.group(4)}"'
 
-    cmd = f"dmsetup load {dm_name} --table {new_table}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: dm_set_target_type() - could not load table on {dm_name}")
+    cmd = f'dmsetup load {dm_name} --table {new_table}'
+    if run(cmd).rc != 0:
+        logging.error(f'dm_set_target_type() - could not load table on {dm_name}')
         dm_resume_dev(dm_name)
         return False
 
     if not dm_resume_dev(dm_name):
         return False
 
     return True
@@ -435,51 +436,51 @@
     The arguments are:
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
-    cmd = f"dmsetup suspend {dm_name}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: could not suspend {dm_name}")
+    cmd = f'dmsetup suspend {dm_name}'
+    if run(cmd).rc != 0:
+        logging.error(f'could not suspend {dm_name}')
         return False
 
     return True
 
 
 def dm_resume_dev(dm_name):  # noqa: ANN001, ANN201
     """Executes dmsetup resume to suspend a specific DM device
     The arguments are:
     Device name: eg. VG-lv_home
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
-    cmd = f"dmsetup resume {dm_name}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: could not resume {dm_name}")
+    cmd = f'dmsetup resume {dm_name}'
+    if run(cmd).rc != 0:
+        logging.error(f'could not resume {dm_name}')
         return False
 
     return True
 
 
 def dm_message_dev(dm_name, message):  # noqa: ANN001, ANN201
     """Executes dmsetup message to send a message to a specific DM device
     The arguments are:
     Device name: e.g. mpatha
     Returns:
     Boolean:
     True in case of success
     False in case of failure.
     """
-    cmd = f"dmsetup message {dm_name} {message}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: could not send message to {dm_name}")
+    cmd = f'dmsetup message {dm_name} {message}'
+    if run(cmd).rc != 0:
+        logging.error(f'could not send message to {dm_name}')
         return False
 
     return True
 
 
 def dm_remove(dm_name):  # noqa: ANN001, ANN201
     """Remove the specified device
@@ -491,12 +492,12 @@
     False in case of failure.
     """
     devs = dm_query_table()
     if dm_name not in list(devs.keys()):
         # device name does not exist
         return True
 
-    cmd = f"dmsetup remove {dm_name}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: could not remove {dm_name}")
+    cmd = f'dmsetup remove {dm_name}'
+    if run(cmd).rc != 0:
+        logging.error(f'could not remove {dm_name}')
         return False
     return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/dmpd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,198 +1,199 @@
 """dmpd.py: Module to manipulate LVM thinp and cache metadata devices and snapshot eras."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import sys
 from pathlib import Path
 from typing import Dict, List, Union
 
 from sts import linux, lvm
 from sts.utils.cli_tools import Wrapper
 from sts.utils.cmdline import run, run_ret_out
 
 
 def _get_devices():  # noqa: ANN202
     return lvm.lv_query()
 
 
 def _get_active_devices():  # noqa: ANN202
-    cmd = "ls /dev/mapper/"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = 'ls /dev/mapper/'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Could not find active dm devices")
+        logging.error('Could not find active dm devices')
         return False
     return output.split()
 
 
 def _get_device_path(vg_name, lv_name):  # noqa: ANN001, ANN202
-    device_path = vg_name + "-" + lv_name
-    if "/dev/mapper/" not in device_path:
-        device_path = "/dev/mapper/" + device_path
+    device_path = vg_name + '-' + lv_name
+    if '/dev/mapper/' not in device_path:
+        device_path = '/dev/mapper/' + device_path
     return device_path
 
 
 def _check_device(vg_name, lv_name):  # noqa: ANN001, ANN202
     devices = _get_devices()
-    device_list = [f["name"] for f in devices]
+    device_list = [f['name'] for f in devices]
     if lv_name not in device_list:
-        print(f"FAIL: {lv_name} is not a device")
+        logging.error(f'{lv_name} is not a device')
         return False
     for x in devices:
-        if x["name"] == lv_name and x["vg_name"] == vg_name:
-            print(f"INFO: Found device {lv_name} in group {vg_name}")
+        if x['name'] == lv_name and x['vg_name'] == vg_name:
+            logging.info(f'Found device {lv_name} in group {vg_name}')
             return True
     return False
 
 
 def _activate_device(vg_name, lv_name):  # noqa: ANN001, ANN202
     devices_active = _get_active_devices()
-    if vg_name + "-" + lv_name not in devices_active:
+    if vg_name + '-' + lv_name not in devices_active:
         ret = lvm.lv_activate(lv_name, vg_name)
         if not ret:
-            print(f"FAIL: Could not activate device {lv_name}")
+            logging.error(f'Could not activate device {lv_name}')
             return False
-        print(f"INFO: device {lv_name} was activated")
-    print(f"INFO: device {lv_name} is active")
+        logging.info(f'device {lv_name} was activated')
+    logging.info(f'device {lv_name} is active')
     return True
 
 
 def _fallocate(_file, size, command_message):  # noqa: ANN001, ANN202
-    cmd = f"fallocate -l {size}M {_file}"
+    cmd = f'fallocate -l {size}M {_file}'
     try:
-        retcode = run(cmd).returncode
+        retcode = run(cmd).rc
         if retcode != 0:
-            print(f"FAIL: Command failed with code {retcode}.")
-            print(f"FAIL: Could not create file to {command_message} metadata to.")
+            logging.error(f'Command failed with code {retcode}.')
+            logging.error(f'Could not create file to {command_message} metadata to.')
             return False
     except OSError as e:
-        print("command failed: ", e, file=sys.stderr)
+        print('command failed: ', e, file=sys.stderr)
         return False
     return True
 
 
 def get_help(cmd):  # noqa: ANN001, ANN201
     commands = [
-        "cache_check",
-        "cache_dump",
-        "cache_metadata_size",
-        "cache_repair",
-        "cache_restore",
-        "era_check",
-        "era_dump",
-        "era_invalidate",
-        "era_restore",
-        "thin_check",
-        "thin_delta",
-        "thin_dump",
-        "thin_ls",
-        "thin_metadata_size",
-        "thin_repair",
-        "thin_restore",
-        "thin_rmap",
-        "thin_show_duplicates",
-        "thin_trim",
+        'cache_check',
+        'cache_dump',
+        'cache_metadata_size',
+        'cache_repair',
+        'cache_restore',
+        'era_check',
+        'era_dump',
+        'era_invalidate',
+        'era_restore',
+        'thin_check',
+        'thin_delta',
+        'thin_dump',
+        'thin_ls',
+        'thin_metadata_size',
+        'thin_repair',
+        'thin_restore',
+        'thin_rmap',
+        'thin_show_duplicates',
+        'thin_trim',
     ]
     if cmd not in commands:
-        print(f"FAIL: Unknown command {cmd}")
+        logging.error(f'Unknown command {cmd}')
         return False
 
-    command = f"{cmd} -h"
-    retcode = run(command, verbose=True).returncode
+    command = f'{cmd} -h'
+    retcode = run(command).rc
     if retcode != 0:
-        print(f"FAIL: Could not get help for {cmd}.")
+        logging.error(f'Could not get help for {cmd}.')
         return False
 
     return True
 
 
 def get_version(cmd):  # noqa: ANN001, ANN201
     commands = [
-        "cache_check",
-        "cache_dump",
-        "cache_metadata_size",
-        "cache_repair",
-        "cache_restore",
-        "era_check",
-        "era_dump",
-        "era_invalidate",
-        "era_restore",
-        "thin_check",
-        "thin_delta",
-        "thin_dump",
-        "thin_ls",
-        "thin_metadata_size",
-        "thin_repair",
-        "thin_restore",
-        "thin_rmap",
-        "thin_show_duplicates",
-        "thin_trim",
+        'cache_check',
+        'cache_dump',
+        'cache_metadata_size',
+        'cache_repair',
+        'cache_restore',
+        'era_check',
+        'era_dump',
+        'era_invalidate',
+        'era_restore',
+        'thin_check',
+        'thin_delta',
+        'thin_dump',
+        'thin_ls',
+        'thin_metadata_size',
+        'thin_repair',
+        'thin_restore',
+        'thin_rmap',
+        'thin_show_duplicates',
+        'thin_trim',
     ]
     if cmd not in commands:
-        print(f"FAIL: Unknown command {cmd}")
+        logging.error(f'Unknown command {cmd}')
         return False
 
-    command = f"{cmd} -V"
-    retcode = run(command, verbose=True).returncode
+    command = f'{cmd} -V'
+    retcode = run(command).rc
     if retcode != 0:
-        print(f"FAIL: Could not get version of {cmd}.")
+        logging.error(f'Could not get version of {cmd}.')
         return False
 
     return True
 
 
 def _get_dev_id(dev_id, path=None, lv_name=None, vg_name=None):  # noqa: ANN001, ANN202
     dev_ids = []
 
     if path is None:
-        retcode, data = thin_dump(source_vg=vg_name, source_lv=lv_name, formatting="xml", return_output=True)
+        retcode, data = thin_dump(source_vg=vg_name, source_lv=lv_name, formatting='xml', return_output=True)
         if not retcode:
-            print(f"FAIL: Could not dump metadata from {vg_name}/{lv_name}")
+            logging.error(f'Could not dump metadata from {vg_name}/{lv_name}')
             return False
         data_lines = data.splitlines()
         for line in data_lines:
             blocks = line.split()
             for block in blocks:
-                if not block.startswith("dev_"):
+                if not block.startswith('dev_'):
                     continue
                 dev_ids.append(int(block[8:-1]))
 
     else:
-        with Path(path, encoding="UTF-8").open() as meta:
+        with Path(path, encoding='UTF-8').open() as meta:
             for line in meta:
                 blocks = line.split()
                 for block in blocks:
-                    if not block.startswith("dev_"):
+                    if not block.startswith('dev_'):
                         continue
                     dev_ids.append(int(block[8:-1]))
 
     if dev_id in dev_ids:
         return True
 
     return False
 
 
 def _metadata_size(source=None, lv_name=None, vg_name=None):  # noqa: ANN001, ANN202
     if source is None:
-        cmd = "lvs -a --units m"
+        cmd = 'lvs -a --units m'
         ret, data = run_ret_out(cmd, return_output=True)
         if ret != 0:
-            print("FAIL: Could not list LVs")
+            logging.error('Could not list LVs')
         data_line = data.splitlines()
         for line in data_line:
             cut = line.split()
             if not cut or lv_name != cut[0] and vg_name != cut[1]:
                 continue
             cut = cut[3]
-            cut = cut.split("m")
+            cut = cut.split('m')
             size = float(cut[0])
             run(cmd)
             return int(size)
-        print(f"FAIL: Could not find {lv_name} {vg_name} in lvs, setting size to 100m")
+        logging.error(f'Could not find {lv_name} {vg_name} in lvs, setting size to 100m')
         return 100
     return int(Path(source).stat().st_size) / 1000000
 
 
 ###########################################
 # cache section
 ###########################################
@@ -204,15 +205,14 @@
     source_lv=None,  # noqa: ANN001
     quiet=False,  # noqa: ANN001
     super_block_only=False,  # noqa: ANN001
     clear_needs_check_flag=False,  # noqa: ANN001
     skip_mappings=False,  # noqa: ANN001
     skip_hints=False,  # noqa: ANN001
     skip_discards=False,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Check cache pool metadata from either file or device.
     The arguments are:
     source_file
     source_vg VG name
     source_lv LV name
     quiet Mute STDOUT
@@ -222,68 +222,67 @@
     skip_hints
     skip_discards
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: cache_check requires either source_file OR source_vg and source_lv.")
+        logging.error('cache_check requires either source_file OR source_vg and source_lv.')
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return False
         device = source_file
 
     if quiet:
-        options += "--quiet "
+        options += '--quiet '
 
     if super_block_only:
-        options += "--super-block-only "
+        options += '--super-block-only '
 
     if clear_needs_check_flag:
-        options += "--clear-needs-check-flag "
+        options += '--clear-needs-check-flag '
 
     if skip_mappings:
-        options += "--skip-mappings "
+        options += '--skip-mappings '
 
     if skip_hints:
-        options += "--skip-hints "
+        options += '--skip-hints '
 
     if skip_discards:
-        options += "--skip-discards "
+        options += '--skip-discards '
 
-    cmd = f"cache_check {device} {options}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'cache_check {device} {options}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not check {device} metadata")
+        logging.error(f'Could not check {device} metadata')
         return False
 
     return True
 
 
 def cache_dump(  # noqa: ANN201
     source_file=None,  # noqa: ANN001
     source_vg=None,  # noqa: ANN001
     source_lv=None,  # noqa: ANN001
     output=None,  # noqa: ANN001
     repair=False,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
     return_output=False,  # noqa: ANN001
 ):
     """Dumps cache metadata from device of source file to standard output or file.
     The arguments are:
     source_file
     source_vg: VG name
     source_lv: LV name
@@ -292,202 +291,200 @@
     repair: Repair the metadata while dumping it
     Returns:
     Only Boolean if return_output False:
     True if success,
     False in case of failure,
     Boolean and data if return_output True.
     """
-    options = ""
+    options = ''
     data = None
 
     if return_output and output:
-        print("INFO: Cannot return to both STDOUT and file, returning only to file.")
+        logging.info('Cannot return to both STDOUT and file, returning only to file.')
         return_output = False
 
     ret_fail = (False, None) if return_output else False
 
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: cache_dump requires either source_file OR source_vg and source_lv.")
+        logging.error('cache_dump requires either source_file OR source_vg and source_lv.')
         return ret_fail
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return ret_fail
         device = source_file
 
     if output:
         if not Path(output).is_file():
             size = _metadata_size(source_file, source_lv, source_vg)
-            ret = _fallocate(output, size + 1, "dump")
+            ret = _fallocate(output, size + 1, 'dump')
             if not ret:
                 return ret_fail
-        options += f"-o {output} "
+        options += f'-o {output} '
 
     if repair:
-        options += "--repair"
+        options += '--repair'
 
-    cmd = f"cache_dump {device} {options}"
+    cmd = f'cache_dump {device} {options}'
     if return_output:
-        retcode, data = run_ret_out(cmd, return_output=True, verbose=verbose)
+        retcode, data = run_ret_out(cmd, return_output=True)
     else:
-        retcode = run(cmd, verbose=verbose).returncode
+        retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not dump {device} metadata.")
+        logging.error(f'Could not dump {device} metadata.')
         return ret_fail
 
     if return_output:
         return True, data
     return True
 
 
 def cache_repair(  # noqa: ANN201
     source_file=None,  # noqa: ANN001
     source_vg=None,  # noqa: ANN001
     source_lv=None,  # noqa: ANN001
     target_file=None,  # noqa: ANN001
     target_vg=None,  # noqa: ANN001
     target_lv=None,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Repairs cache metadata from source file/device to target file/device
     The arguments are:
     source as either source_file OR source_vg and source_lv
     target as either target_file OR target_vg and target_lv
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: cache_repair requires either source_file OR source_vg and source_lv as source.")
+        logging.error('cache_repair requires either source_file OR source_vg and source_lv as source.')
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        print("FAIL: cache_repair requires either target_file OR target_vg and target_lv as target.")
+        logging.error('cache_repair requires either target_file OR target_vg and target_lv as target.')
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         source = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return False
         source = source_file
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
         ret = _activate_device(target_vg, target_lv)
         if not ret:
             return False
         target = _get_device_path(target_vg, target_lv)
     else:
         if not Path(target_file).is_file():
             size = _metadata_size(source_file, source_lv, source_vg)
-            ret = _fallocate(target_file, size + 1, "repair")
+            ret = _fallocate(target_file, size + 1, 'repair')
             if not ret:
                 return False
         target = target_file
 
-    cmd = f"cache_repair -i {source} -o {target}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'cache_repair -i {source} -o {target}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not repair metadata from {source} to {target}")
+        logging.error(f'Could not repair metadata from {source} to {target}')
         return False
 
     return True
 
 
 def cache_restore(  # noqa: ANN201
     source_file,  # noqa: ANN001
     target_vg=None,  # noqa: ANN001
     target_lv=None,  # noqa: ANN001
     target_file=None,  # noqa: ANN001
     quiet=False,  # noqa: ANN001
     metadata_version=None,  # noqa: ANN001
     omit_clean_shutdown=False,  # noqa: ANN001
     override_metadata_version=None,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Restores cache metadata from source xml file to target device/file
     The arguments are:
     source_file Source xml file
     target as either target_file OR target_vg and target_lv
     quiet Mute STDOUT
     metadata_version Specify metadata version to restore
     omit_clean_shutdown Disable clean shutdown
     override_metadata_version DEBUG option to override metadata version without checking
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if source_file is None:
-        print("FAIL: cache_restore requires source file.")
+        logging.error('cache_restore requires source file.')
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        print("FAIL: cache_restore requires either target_file OR target_vg and target_lv as target.")
+        logging.error('cache_restore requires either target_file OR target_vg and target_lv as target.')
         return False
 
     if not Path(source_file).is_file():
-        print("FAIL: Source file is not a file.")
+        logging.error('Source file is not a file.')
         return False
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
         ret = _activate_device(target_vg, target_lv)
         if not ret:
             return False
         target = _get_device_path(target_vg, target_lv)
     else:
         if not Path(target_file).is_file():
             size = _metadata_size(source_file)
-            ret = _fallocate(target_file, size + 1, "restore")
+            ret = _fallocate(target_file, size + 1, 'restore')
             if not ret:
                 return False
         target = target_file
 
     if quiet:
-        options += "--quiet "
+        options += '--quiet '
 
     if metadata_version:
-        options += f"--metadata-version {metadata_version} "
+        options += f'--metadata-version {metadata_version} '
 
     if omit_clean_shutdown:
-        options += "--omit-clean-shutdown "
+        options += '--omit-clean-shutdown '
 
     if override_metadata_version:
-        options += f"--debug-override-metadata-version {override_metadata_version}"
+        options += f'--debug-override-metadata-version {override_metadata_version}'
 
-    cmd = f"cache_restore -i {source_file} -o {target} {options}"
+    cmd = f'cache_restore -i {source_file} -o {target} {options}'
 
-    retcode = run(cmd, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not restore metadata from {source_file} to {target}")
+        logging.error(f'Could not restore metadata from {source_file} to {target}')
         return False
 
     return True
 
 
 ###########################################
 # thinp section
@@ -499,15 +496,14 @@
     source_vg=None,  # noqa: ANN001
     source_lv=None,  # noqa: ANN001
     quiet=False,  # noqa: ANN001
     super_block_only=False,  # noqa: ANN001
     clear_needs_check_flag=False,  # noqa: ANN001
     skip_mappings=False,  # noqa: ANN001
     ignore_non_fatal_errors=False,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Check thin pool metadata from either file or device.
     The arguments are:
     source_file
     source_vg VG name
     source_lv LV name
     quiet Mute STDOUT
@@ -516,122 +512,122 @@
     skip_mappings
     ignore_non_fatal_errors
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: thin_check requires either source_file OR source_vg and source_lv.")
+        logging.error('thin_check requires either source_file OR source_vg and source_lv.')
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return False
         device = source_file
 
     if quiet:
-        options += "--quiet "
+        options += '--quiet '
 
     if super_block_only:
-        options += "--super-block-only "
+        options += '--super-block-only '
 
     if clear_needs_check_flag:
-        options += "--clear-needs-check-flag "
+        options += '--clear-needs-check-flag '
 
     if skip_mappings:
-        options += "--skip-mappings "
+        options += '--skip-mappings '
 
     if ignore_non_fatal_errors:
-        options += "--ignore-non-fatal-errors "
+        options += '--ignore-non-fatal-errors '
 
-    cmd = f"thin_check {device} {options}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'thin_check {device} {options}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not check {device} metadata")
+        logging.error(f'Could not check {device} metadata')
         return False
 
     return True
 
 
-def thin_ls(source_vg, source_lv, no_headers=False, fields=None, snapshot=False, verbose=True):  # noqa: ANN001, ANN201
+def thin_ls(source_vg, source_lv, no_headers=False, fields=None, snapshot=False):  # noqa: ANN001, ANN201
     """List information about thin LVs on thin pool.
     The arguments are:
     source_vg VG name
     source_lv LV name
     fields list of fields to output, default is all
     snapshot Use metadata snapshot, able to run on live snapshotted pool
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if not source_vg or not source_lv:
-        print("FAIL: thin_ls requires source_vg and source_lv.")
+        logging.error('thin_ls requires source_vg and source_lv.')
         return False
 
     ret = _check_device(source_vg, source_lv)
     if not ret:
         return False
     ret = _activate_device(source_vg, source_lv)
     if not ret:
         return False
     device = _get_device_path(source_vg, source_lv)
 
     if no_headers:
-        options += "--no-headers "
+        options += '--no-headers '
 
     fields_possible = [
-        "DEV",
-        "MAPPED_BLOCKS",
-        "EXCLUSIVE_BLOCKS",
-        "SHARED_BLOCKS",
-        "MAPPED_SECTORS",
-        "EXCLUSIVE_SECTORS",
-        "SHARED_SECTORS",
-        "MAPPED_BYTES",
-        "EXCLUSIVE_BYTES",
-        "SHARED_BYTES",
-        "MAPPED",
-        "EXCLUSIVE",
-        "TRANSACTION",
-        "CREATE_TIME",
-        "SHARED",
-        "SNAP_TIME",
+        'DEV',
+        'MAPPED_BLOCKS',
+        'EXCLUSIVE_BLOCKS',
+        'SHARED_BLOCKS',
+        'MAPPED_SECTORS',
+        'EXCLUSIVE_SECTORS',
+        'SHARED_SECTORS',
+        'MAPPED_BYTES',
+        'EXCLUSIVE_BYTES',
+        'SHARED_BYTES',
+        'MAPPED',
+        'EXCLUSIVE',
+        'TRANSACTION',
+        'CREATE_TIME',
+        'SHARED',
+        'SNAP_TIME',
     ]
     if fields is None:
         options += f" --format \"{','.join([str(i) for i in fields_possible])}\" "
     else:
         for field in fields:
             if field not in fields_possible:
-                print(f"FAIL: Unknown field {field} specified.")
-                print(f"INFO: Possible fields are: {', '.join([str(i) for i in fields_possible])}")
+                logging.error(f'Unknown field {field} specified.')
+                logging.info(f"Possible fields are: {', '.join([str(i) for i in fields_possible])}")
                 return False
         options += f" --format \"{','.join([str(i) for i in fields])}\" "
 
     if snapshot:
-        options += "--metadata-snap"
+        options += '--metadata-snap'
 
-    cmd = f"thin_ls {device} {options}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'thin_ls {device} {options}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not list {device} metadata")
+        logging.error(f'Could not list {device} metadata')
         return False
 
     return True
 
 
 def thin_dump(  # noqa: ANN201
     source_file=None,  # noqa: ANN001
@@ -639,15 +635,14 @@
     source_lv=None,  # noqa: ANN001
     output=None,  # noqa: ANN001
     repair=False,  # noqa: ANN001
     formatting=None,  # noqa: ANN001
     snapshot=None,  # noqa: ANN001
     dev_id=None,  # noqa: ANN001
     skip_mappings=False,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
     return_output=False,  # noqa: ANN001
 ):
     """Dumps thin metadata from device of source file to standard output or file.
     The arguments are:
     source_file
     source_vg: VG name
     source_lv: LV name
@@ -659,314 +654,311 @@
     dev_id: id of the device
     Returns:
     Only Boolean if return_output False:
     True if success
     False in case of failure
     Boolean and data if return_output True.
     """
-    options = ""
+    options = ''
     data = None
 
     if return_output and output:
-        print("INFO: Cannot return to both STDOUT and file, returning only to file.")
+        logging.info('Cannot return to both STDOUT and file, returning only to file.')
         return_output = False
 
     ret_fail = (False, None) if return_output else False
 
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: thin_dump requires either source_file OR source_vg and source_lv.")
+        logging.error('thin_dump requires either source_file OR source_vg and source_lv.')
         return ret_fail
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return ret_fail
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return ret_fail
         device = source_file
 
     if output:
         if not Path(output).is_file():
             size = _metadata_size(source_file, source_lv, source_vg)
-            ret = _fallocate(output, size + 1, "dump")
+            ret = _fallocate(output, size + 1, 'dump')
             if not ret:
                 return ret_fail
-        options += f"-o {output} "
+        options += f'-o {output} '
 
     if repair:
-        options += "--repair "
+        options += '--repair '
 
     if snapshot:
         if isinstance(snapshot, bool):
-            options += "--metadata-snap "
+            options += '--metadata-snap '
         elif isinstance(snapshot, int):
-            options += f"--metadata-snap {snapshot} "
+            options += f'--metadata-snap {snapshot} '
         else:
-            print("FAIL: Unknown snapshot value, use either Boolean or Int.")
+            logging.error('Unknown snapshot value, use either Boolean or Int.')
             return ret_fail
 
     if formatting:
-        if formatting in ["xml", "human_readable"]:
-            options += f"--format {formatting} "
-        elif formatting.startswith("custom="):
+        if formatting in ['xml', 'human_readable']:
+            options += f'--format {formatting} '
+        elif formatting.startswith('custom='):
             if not Path(formatting[8:-1]).is_file():
-                print("FAIL: Specified custom formatting file is not a file.")
+                logging.error('Specified custom formatting file is not a file.')
                 return ret_fail
-            options += f"--format {formatting} "
+            options += f'--format {formatting} '
         else:
-            print("FAIL: Unknown formatting specified, please use one of [xml, human_readable, custom='file'].")
+            logging.error("Unknown formatting specified, please use one of [xml, human_readable, custom='file'].")
             return ret_fail
 
     if dev_id:
         if isinstance(dev_id, int):
             if _get_dev_id(dev_id, source_file, source_lv, source_vg):
-                options += f"--dev-id {dev_id} "
+                options += f'--dev-id {dev_id} '
             else:
-                print(f"FAIL: Unknown dev_id value, device with id {dev_id} does not exist.")
+                logging.error(f'Unknown dev_id value, device with id {dev_id} does not exist.')
                 return ret_fail
         else:
-            print("FAIL: Unknown dev_id value, must be Int.")
+            logging.error('Unknown dev_id value, must be Int.')
             return ret_fail
 
     if skip_mappings:
-        options += "--skip-mappings "
+        options += '--skip-mappings '
 
-    cmd = f"thin_dump {device} {options}"
+    cmd = f'thin_dump {device} {options}'
     if return_output:
-        retcode, data = run_ret_out(cmd, return_output=True, verbose=verbose)
+        retcode, data = run_ret_out(cmd, return_output=True)
     else:
-        retcode = run(cmd, verbose=verbose).returncode
+        retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not dump {device} metadata.")
+        logging.error(f'Could not dump {device} metadata.')
         return ret_fail
 
     if return_output:
         return True, data
     return True
 
 
 def thin_restore(  # noqa: ANN201
     source_file,  # noqa: ANN001
     target_vg=None,  # noqa: ANN001
     target_lv=None,  # noqa: ANN001
     target_file=None,  # noqa: ANN001
     quiet=False,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Restores thin metadata from source xml file to target device/file
     The arguments are:
     source_file Source xml file
     target as either target_file OR target_vg and target_lv
     quiet Mute STDOUT
     metadata_version Specify metadata version to restore
     omit_clean_shutdown Disable clean shutdown
     override_metadata_version DEBUG option to override metadata version without checking
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if source_file is None:
-        print("FAIL: thin_restore requires source file.")
+        logging.error('thin_restore requires source file.')
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        print("FAIL: thin_restore requires either target_file OR target_vg and target_lv as target.")
+        logging.error('thin_restore requires either target_file OR target_vg and target_lv as target.')
         return False
 
     if not Path(source_file).is_file():
-        print("FAIL: Source file is not a file.")
+        logging.error('Source file is not a file.')
         return False
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
         ret = _activate_device(target_vg, target_lv)
         if not ret:
             return False
         target = _get_device_path(target_vg, target_lv)
     else:
         if not Path(target_file).is_file():
             size = _metadata_size(source_file)
-            ret = _fallocate(target_file, size + 1, "restore")
+            ret = _fallocate(target_file, size + 1, 'restore')
             if not ret:
                 return False
         target = target_file
 
     if quiet:
-        options += "--quiet"
+        options += '--quiet'
 
-    cmd = f"thin_restore -i {source_file} -o {target} {options}"
+    cmd = f'thin_restore -i {source_file} -o {target} {options}'
 
-    retcode = run(cmd, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not restore metadata from {source_file} to {target}")
+        logging.error(f'Could not restore metadata from {source_file} to {target}')
         return False
 
     return True
 
 
 def thin_repair(  # noqa: ANN201
     source_file=None,  # noqa: ANN001
     source_vg=None,  # noqa: ANN001
     source_lv=None,  # noqa: ANN001
     target_file=None,  # noqa: ANN001
     target_vg=None,  # noqa: ANN001
     target_lv=None,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Repairs thin metadata from source file/device to target file/device
     The arguments are:
     source as either source_file OR source_vg and source_lv
     target as either target_file OR target_vg and target_lv
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: thin_repair requires either source_file OR source_vg and source_lv as source.")
+        logging.error('thin_repair requires either source_file OR source_vg and source_lv as source.')
         return False
 
     if not target_file and (not target_vg or not target_lv):
-        print("FAIL: thin_repair requires either target_file OR target_vg and target_lv as target.")
+        logging.error('thin_repair requires either target_file OR target_vg and target_lv as target.')
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         source = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return False
         source = source_file
 
     if not target_file:
         ret = _check_device(target_vg, target_lv)
         if not ret:
             return False
         ret = _activate_device(target_vg, target_lv)
         if not ret:
             return False
         target = _get_device_path(target_vg, target_lv)
     else:
         if not Path(target_file).is_file():
             size = _metadata_size(source_file, source_lv, source_vg)
-            ret = _fallocate(target_file, size + 1, "repair")
+            ret = _fallocate(target_file, size + 1, 'repair')
             if not ret:
                 return False
         target = target_file
 
-    cmd = f"thin_repair -i {source} -o {target}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'thin_repair -i {source} -o {target}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not repair metadata from {source} to {target}")
+        logging.error(f'Could not repair metadata from {source} to {target}')
         return False
 
     return True
 
 
-def thin_rmap(region, source_file=None, source_vg=None, source_lv=None, verbose=True):  # noqa: ANN001, ANN201
+def thin_rmap(region, source_file=None, source_vg=None, source_lv=None):  # noqa: ANN001, ANN201
     """Output reverse map of a thin provisioned region of blocks from metadata device.
     The arguments are:
     source_vg VG name
     source_lv LV name
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: thin_rmap requires either source_file OR source_vg and source_lv as source.")
+        logging.error('thin_rmap requires either source_file OR source_vg and source_lv as source.')
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return False
         device = source_file
 
-    regions = region.split(".")
+    regions = region.split('.')
     try:
         int(regions[0])
         if regions[1]:
             raise ValueError  # noqa: TRY301
         int(regions[2])
         if regions[3] is not None:
             raise ValueError  # noqa: TRY301
     except ValueError:
-        print("FAIL: Region must be in format 'INT..INT'")
+        logging.exception("Region must be in format 'INT..INT'")
         return False
     except IndexError:
         pass
     # region 1..-1 must be valid, using unsigned 32bit ints
     if int(regions[0]) & 0xFFFFFFFF >= int(regions[2]) & 0xFFFFFFFF:
-        print("FAIL: Beginning of the region must be before its end.")
+        logging.error('Beginning of the region must be before its end.')
         return False
-    options = f"--region {region}"
+    options = f'--region {region}'
 
-    cmd = f"thin_rmap {device} {options}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'thin_rmap {device} {options}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not output reverse map from {device} metadata device")
+        logging.error(f'Could not output reverse map from {device} metadata device')
         return False
 
     return True
 
 
 def thin_trim(  # noqa: ANN201
     data_vg,  # noqa: ANN001
     data_lv,  # noqa: ANN001
     metadata_vg=None,  # noqa: ANN001
     metadata_lv=None,  # noqa: ANN001
     metadata_file=None,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Issue discard requests for free pool space.
     The arguments are:
     data_vg VG name of data device
     data_lv LV name of data device
     metadata_vg VG name of metadata device
     metadata_lv LV name of metadata device
     metadata_file file with metadata
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if not data_vg or not data_lv:
-        print("FAIL: thin_trim requires data_vg and data_lv.")
+        logging.error('thin_trim requires data_vg and data_lv.')
         return False
 
     if not metadata_file and (not metadata_vg or not metadata_lv):
-        print("FAIL: thin_trim requires either metadata_file OR metadata_vg and metadata_lv as target.")
+        logging.error('thin_trim requires either metadata_file OR metadata_vg and metadata_lv as target.')
         return False
 
     ret = _check_device(data_vg, data_lv)
     if not ret:
         return False
 
     ret = _activate_device(data_vg, data_lv)
@@ -979,291 +971,290 @@
             return False
         ret = _activate_device(metadata_vg, metadata_lv)
         if not ret:
             return False
         metadata_dev = _get_device_path(metadata_vg, metadata_lv)
     else:
         if not Path(metadata_file).is_file():
-            print(f"FAIL: metadata_file {metadata_file} is not a file.")
+            logging.error(f'metadata_file {metadata_file} is not a file.')
             return False
         metadata_dev = metadata_file
 
     data_dev = _get_device_path(data_vg, data_lv)
-    cmd = f"thin_trim --data-dev {data_dev} --metadata-dev {metadata_dev} {options}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'thin_trim --data-dev {data_dev} --metadata-dev {metadata_dev} {options}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not discard free pool space on device {data_dev} with metadata device {metadata_dev}.")
+        logging.error(f'Could not discard free pool space on device {data_dev} with metadata device {metadata_dev}.')
         return False
 
     return True
 
 
 def thin_delta(  # noqa: ANN201
     thin1,  # noqa: ANN001
     thin2,  # noqa: ANN001
     source_file=None,  # noqa: ANN001
     source_vg=None,  # noqa: ANN001
     source_lv=None,  # noqa: ANN001
     snapshot=False,  # noqa: ANN001
     verbosity=False,  # noqa: ANN001
-    verbose=True,  # noqa: ANN001
 ):
     """Print the differences in the mappings between two thin devices.
     The arguments are:
     source_vg VG name
     source_lv LV name
     thin1 numeric identificator of first thin volume
     thin2 numeric identificator of second thin volume
     snapshot (Boolean/Int) Use metadata snapshot. If Int provided, specifies block number
     verbosity Provide extra information on the mappings
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    options = ""
+    options = ''
 
     if not source_file and (not source_vg or not source_lv):
-        print("FAIL: thin_delta requires either source_file OR source_vg and source_lv.")
+        logging.error('thin_delta requires either source_file OR source_vg and source_lv.')
         return False
 
     if not source_file:
         ret = _check_device(source_vg, source_lv)
         if not ret:
             return False
         ret = _activate_device(source_vg, source_lv)
         if not ret:
             return False
         device = _get_device_path(source_vg, source_lv)
     else:
         if not Path(source_file).is_file():
-            print("FAIL: Source file is not a file.")
+            logging.error('Source file is not a file.')
             return False
         device = source_file
 
     if snapshot:
         if isinstance(snapshot, bool):
-            options += "--metadata-snap "
+            options += '--metadata-snap '
         elif isinstance(snapshot, int):
-            options += f"--metadata-snap {snapshot} "
+            options += f'--metadata-snap {snapshot} '
         else:
-            print("FAIL: Unknown snapshot value, use either Boolean or Int.")
+            logging.error('Unknown snapshot value, use either Boolean or Int.')
             return False
 
     if verbosity:
-        options += "--verbose"
+        options += '--verbose'
 
     if _get_dev_id(thin1, source_file, source_lv, source_vg) and _get_dev_id(thin2, source_file, source_lv, source_vg):
-        cmd = f"thin_delta {options} --thin1 {thin1} --thin2 {thin2} {device}"
-        retcode = run(cmd, verbose=verbose).returncode
+        cmd = f'thin_delta {options} --thin1 {thin1} --thin2 {thin2} {device}'
+        retcode = run(cmd).rc
         if retcode != 0:
-            print("FAIL: Could not get differences in mappings between two thin LVs.")
+            logging.error('Could not get differences in mappings between two thin LVs.')
             return False
     else:
-        print("FAIL: Specified id does not exist.")
+        logging.error('Specified id does not exist.')
         return False
     return True
 
 
 class DMPD(Wrapper):
     def __init__(self, disable_check=True) -> None:  # noqa: ANN001
         self.disable_check = disable_check
 
-        pkg = "device-mapper-persistent-data"
+        pkg = 'device-mapper-persistent-data'
         if not linux.is_installed(pkg) and not linux.install_package(pkg, check=False):
-            print(f"FATAL: Could not install {pkg} package")
+            logging.critical(f'Could not install {pkg} package')
 
         self.commands: Dict[str, Union[str, List[str]]] = {
-            "cache_check": "cache_check",
-            "cache_dump": "cache_dump",
-            "cache_metadata_size": "cache_metadata_size",
-            "cache_repair": "cache_repair",
-            "cache_restore": "cache_restore",
-            "cache_writeback": "cache_writeback",
-            "thin_check": "thin_check",
-            "thin_delta": "thin_delta",
-            "thin_dump": "thin_dump",
-            "thin_ls": "thin_ls",
-            "thin_metadata_size": "thin_metadata_size",
-            "thin_repair": "thin_repair",
-            "thin_restore": "thin_restore",
-            "thin_rmap": "thin_rmap",
-            "thin_trim": "thin_trim",
+            'cache_check': 'cache_check',
+            'cache_dump': 'cache_dump',
+            'cache_metadata_size': 'cache_metadata_size',
+            'cache_repair': 'cache_repair',
+            'cache_restore': 'cache_restore',
+            'cache_writeback': 'cache_writeback',
+            'thin_check': 'thin_check',
+            'thin_delta': 'thin_delta',
+            'thin_dump': 'thin_dump',
+            'thin_ls': 'thin_ls',
+            'thin_metadata_size': 'thin_metadata_size',
+            'thin_repair': 'thin_repair',
+            'thin_restore': 'thin_restore',
+            'thin_rmap': 'thin_rmap',
+            'thin_trim': 'thin_trim',
         }
-        self.commands["all"] = list(self.commands.keys())
+        self.commands['all'] = list(self.commands.keys())
         self.arguments = {
-            "help": [self.commands["all"], " --help"],
-            "version": [self.commands["all"], " --version"],
-            "verbose": [self.commands["all"], " --verbose"],
-            "block_size": [
-                ["cache_metadata_size", "thin_metadata_size"],
-                " --block-size&",
+            'help': [self.commands['all'], ' --help'],
+            'version': [self.commands['all'], ' --version'],
+            'verbose': [self.commands['all'], ' --verbose'],
+            'block_size': [
+                ['cache_metadata_size', 'thin_metadata_size'],
+                ' --block-size&',
             ],
-            "buffer_size": [["cache_writeback"], " --buffer-size-meg&"],
-            "clear_needs_check_flag": [
-                ["cache_check", "thin_check"],
-                " --clear-needs-check-flag",
+            'buffer_size': [['cache_writeback'], ' --buffer-size-meg&'],
+            'clear_needs_check_flag': [
+                ['cache_check', 'thin_check'],
+                ' --clear-needs-check-flag',
             ],
-            "data_dev": [["thin_trim"], " --data-dev&"],
-            "debug_override_metadata_version": [
-                ["cache_restore"],
-                " --debug-override-metadata-version&",
+            'data_dev': [['thin_trim'], ' --data-dev&'],
+            'debug_override_metadata_version': [
+                ['cache_restore'],
+                ' --debug-override-metadata-version&',
             ],
-            "dev_id": [["thin_dump"], " --dev-id&"],
-            "device_size": [["cache_metadata_size"], " --device-size&"],
-            "fast_device": [["cache_writeback"], " --fast-device&"],
-            "format": [["thin_ls", "thin_dump"], " --format&"],
-            "ignore_non_fatal_errors": [["thin_check"], " --ignore-non-fatal-errors"],
-            "input": [
-                ["cache_repair", "cache_restore", "thin_repair", "thin_restore"],
-                " -i&",
+            'dev_id': [['thin_dump'], ' --dev-id&'],
+            'device_size': [['cache_metadata_size'], ' --device-size&'],
+            'fast_device': [['cache_writeback'], ' --fast-device&'],
+            'format': [['thin_ls', 'thin_dump'], ' --format&'],
+            'ignore_non_fatal_errors': [['thin_check'], ' --ignore-non-fatal-errors'],
+            'input': [
+                ['cache_repair', 'cache_restore', 'thin_repair', 'thin_restore'],
+                ' -i&',
             ],
-            "list_failed_blocks": [["cache_writeback"], " --list-failed-blocks"],
-            "max_hint_width": [["cache_metadata_size"], " --max-hint-width&"],
-            "max_thins": [["thin_metadata_size"], " --max-thins&"],
-            "metadata_dev": [["thin_trim"], " --metadata-dev&"],
-            "metadata_device": [["cache_writeback"], " --metadata-device&"],
-            "metadata_snap": [["thin_dump", "thin_delta"], " --metadata-snap&"],
-            "metadata_version": [["cache_restore"], " --metadata-version&"],
-            "no_headers": [["thin_ls"], " --no-headers"],
-            "no_metadata_update": [["cache_writeback"], " --no-metadata-update"],
-            "nr_blocks": [["cache_metadata_size"], " --nr-blocks&"],
-            "numeric_only": [["thin_metadata_size"], " --numeric-only"],
-            "numeric_only_type": [["thin_metadata_size"], " --numeric-only="],
-            "omit_clean_shutdown": [["cache_restore"], " --omit-clean-shutdown"],
-            "origin_device": [["cache_writeback"], " --origin-device&"],
-            "output": [
+            'list_failed_blocks': [['cache_writeback'], ' --list-failed-blocks'],
+            'max_hint_width': [['cache_metadata_size'], ' --max-hint-width&'],
+            'max_thins': [['thin_metadata_size'], ' --max-thins&'],
+            'metadata_dev': [['thin_trim'], ' --metadata-dev&'],
+            'metadata_device': [['cache_writeback'], ' --metadata-device&'],
+            'metadata_snap': [['thin_dump', 'thin_delta'], ' --metadata-snap&'],
+            'metadata_version': [['cache_restore'], ' --metadata-version&'],
+            'no_headers': [['thin_ls'], ' --no-headers'],
+            'no_metadata_update': [['cache_writeback'], ' --no-metadata-update'],
+            'nr_blocks': [['cache_metadata_size'], ' --nr-blocks&'],
+            'numeric_only': [['thin_metadata_size'], ' --numeric-only'],
+            'numeric_only_type': [['thin_metadata_size'], ' --numeric-only='],
+            'omit_clean_shutdown': [['cache_restore'], ' --omit-clean-shutdown'],
+            'origin_device': [['cache_writeback'], ' --origin-device&'],
+            'output': [
                 [
-                    "cache_dump",
-                    "cache_repair",
-                    "cache_restore",
-                    "thin_dump",
-                    "thin_repair",
-                    "thin_restore",
+                    'cache_dump',
+                    'cache_repair',
+                    'cache_restore',
+                    'thin_dump',
+                    'thin_repair',
+                    'thin_restore',
                 ],
-                " -o&",
+                ' -o&',
             ],
-            "override_mapping_root": [["thin_check"], " --override-mapping-root&"],
-            "pool_size": [["thin_metadata_size"], " --pool-size&"],
-            "quiet": [
-                ["cache_check", "cache_restore", "thin_check", "thin_restore"],
-                " --quiet",
+            'override_mapping_root': [['thin_check'], ' --override-mapping-root&'],
+            'pool_size': [['thin_metadata_size'], ' --pool-size&'],
+            'quiet': [
+                ['cache_check', 'cache_restore', 'thin_check', 'thin_restore'],
+                ' --quiet',
             ],
-            "region": [["thin_rmap"], " --region&"],
-            "repair": [["cache_dump", "thin_dump"], " --repair"],
-            "skip_discards": [["cache_check"], " --skip-discards"],
-            "skip_hints": [["cache_check"], " --skip-hints"],
-            "skip_mappings": [["thin_check", "thin_dump"], " --skip-mappings"],
-            "snap1": [["thin_delta"], " --snap1&"],
-            "snap2": [["thin_delta"], " --snap2&"],
-            "snapshot": [["thin_ls", "thin_dump", "thin_delta"], " --metadata-snap"],
-            "super_block_only": [["cache_check", "thin_check"], " --super-block-only"],
-            "thin1": [["thin_delta"], " --thin1&"],
-            "thin2": [["thin_delta"], " --thin2&"],
-            "unit": [["thin_metadata_size"], " --unit&"],
+            'region': [['thin_rmap'], ' --region&'],
+            'repair': [['cache_dump', 'thin_dump'], ' --repair'],
+            'skip_discards': [['cache_check'], ' --skip-discards'],
+            'skip_hints': [['cache_check'], ' --skip-hints'],
+            'skip_mappings': [['thin_check', 'thin_dump'], ' --skip-mappings'],
+            'snap1': [['thin_delta'], ' --snap1&'],
+            'snap2': [['thin_delta'], ' --snap2&'],
+            'snapshot': [['thin_ls', 'thin_dump', 'thin_delta'], ' --metadata-snap'],
+            'super_block_only': [['cache_check', 'thin_check'], ' --super-block-only'],
+            'thin1': [['thin_delta'], ' --thin1&'],
+            'thin2': [['thin_delta'], ' --thin2&'],
+            'unit': [['thin_metadata_size'], ' --unit&'],
         }
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
     def _remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     def _get_possible_arguments(self, command=None):  # noqa: ANN001, ANN202
         return super()._get_possible_arguments(command.split()[0])
 
-    def _run(self, cmd, verbosity=True, **kwargs):  # noqa: ANN001, ANN003, ANN202
+    def _run(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
         cmd = self._add_arguments(cmd, **kwargs)
 
-        ret = run(cmd, verbose=verbosity).returncode
+        ret = run(cmd).rc
         if isinstance(ret, tuple) and ret[0] != 0:
-            print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+            logging.warning(f"Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+            logging.warning(f"Running command: '{cmd}' failed.")
         return ret
 
     def cache_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "cache_check "
+        cmd = 'cache_check '
         if source_file:
-            cmd += f"{source_file} "
+            cmd += f'{source_file} '
         if source_vg and source_lv:
-            cmd += f"{_get_device_path(source_vg, source_lv)} "
+            cmd += f'{_get_device_path(source_vg, source_lv)} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def cache_dump(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "cache_dump "
+        cmd = 'cache_dump '
         if source_file:
-            cmd += f"{source_file} "
+            cmd += f'{source_file} '
         if source_vg and source_lv:
-            cmd += f"{_get_device_path(source_vg, source_lv)} "
+            cmd += f'{_get_device_path(source_vg, source_lv)} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def cache_metadata_size(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "cache_metadata_size "
+        cmd = 'cache_metadata_size '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def cache_repair(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "cache_repair "
+        cmd = 'cache_repair '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def cache_restore(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "cache_restore "
+        cmd = 'cache_restore '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def cache_writeback(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "cache_writeback "
+        cmd = 'cache_writeback '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_check(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "thin_check "
+        cmd = 'thin_check '
         if source_file:
-            cmd += f"{source_file} "
+            cmd += f'{source_file} '
         if source_vg and source_lv:
-            cmd += f"{_get_device_path(source_vg, source_lv)} "
+            cmd += f'{_get_device_path(source_vg, source_lv)} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_delta(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "thin_delta "
+        cmd = 'thin_delta '
         if source_file:
-            cmd += f"{source_file} "
+            cmd += f'{source_file} '
         if source_vg and source_lv:
-            cmd += f"{_get_device_path(source_vg, source_lv)} "
+            cmd += f'{_get_device_path(source_vg, source_lv)} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_dump(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "thin_dump "
+        cmd = 'thin_dump '
         if source_file:
-            cmd += f"{source_file} "
+            cmd += f'{source_file} '
         if source_vg and source_lv:
-            cmd += f"{_get_device_path(source_vg, source_lv)} "
+            cmd += f'{_get_device_path(source_vg, source_lv)} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_ls(self, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "thin_ls "
+        cmd = 'thin_ls '
         if source_vg and source_lv:
             cmd += _get_device_path(source_vg, source_lv)
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_metadata_size(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "thin_metadata_size "
+        cmd = 'thin_metadata_size '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_repair(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "thin_repair "
+        cmd = 'thin_repair '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_restore(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "thin_restore "
+        cmd = 'thin_restore '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_rmap(self, source_file=None, source_vg=None, source_lv=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "thin_rmap "
+        cmd = 'thin_rmap '
         if source_file:
-            cmd += f"{source_file} "
+            cmd += f'{source_file} '
         if source_vg and source_lv:
-            cmd += f"{_get_device_path(source_vg, source_lv)} "
+            cmd += f'{_get_device_path(source_vg, source_lv)} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def thin_trim(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "thin_trim "
+        cmd = 'thin_trim '
         return self._run(cmd, **self._remove_nones(kwargs))
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/fc.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/fc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """fc.py: Module to manipulate FC devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
 import os.path
-import re  # regex
+import re
 from pathlib import Path
 
 from sts import linux, scsi
 from sts.utils.cmdline import run_ret_out
 
-host_path = "/sys/class/fc_host/"
+host_path = '/sys/class/fc_host/'
 
-remote_port_path = "/sys/class/fc_remote_ports/"
+remote_port_path = '/sys/class/fc_remote_ports/'
 
-regex_target_id = re.compile(r"target(\d+):(\d+):(\d+)")
-regex_target = re.compile(r"(\d+):(\d+):(\d+)")
-wwn_regex = re.compile(r"(?:[0-9a-f]{2}:){7}[0-9a-f]{2}")
+regex_target_id = re.compile(r'target(\d+):(\d+):(\d+)')
+regex_target = re.compile(r'(\d+):(\d+):(\d+)')
+wwn_regex = re.compile(r'(?:[0-9a-f]{2}:){7}[0-9a-f]{2}')
 
 
 def is_wwn(wwn):  # noqa: ANN001, ANN201
     """Checks if the entry is on valid WWN format.
     example: 10:00:5c:b9:01:c1:ec:71
     The arguments are:
     a WWN
@@ -48,19 +49,19 @@
         wwpn.
     """
     if not wwpn:
         return None
     wwpn = wwpn.lower()
     if is_wwn(wwpn):
         return wwpn
-    wwpn = re.sub("0x", "", wwpn)
+    wwpn = re.sub('0x', '', wwpn)
     # remove all : characters from the entry, later on they will be added in correct order
-    wwpn = wwpn.replace(":", "")
+    wwpn = wwpn.replace(':', '')
     # append ":" every 2nd character
-    wwpn = ":".join(wwpn[i : i + 2] for i in range(0, len(wwpn), 2))
+    wwpn = ':'.join(wwpn[i : i + 2] for i in range(0, len(wwpn), 2))
     if is_wwn(wwpn):
         return wwpn
     return None
 
 
 def query_all_fc_disks(host_id=None):  # noqa: ANN001, ANN201
     """Return SCSI disk info all all FC/FCoE devices."""
@@ -72,80 +73,80 @@
     if host_id:
         hosts = [host_id]
 
     scsi_disks = scsi.query_all_scsi_disks()
     fc_disks = {}
     for scsi_id in list(scsi_disks.keys()):
         scsi_disk = scsi_disks[scsi_id]
-        if scsi_disk["host_id"] in hosts:
+        if scsi_disk['host_id'] in hosts:
             fc_disks[scsi_id] = scsi_disk
     return fc_disks
 
 
 def scsi_wwid_of_fc_disks():  # noqa: ANN201
     """Return a list of all WWIDs of FC/FCoE disks."""
     disks_info = query_all_fc_disks()
     if not disks_info:
         return None
     wwids = []
     for info in list(disks_info.values()):
-        if "wwid" not in list(info.keys()):
+        if 'wwid' not in list(info.keys()):
             continue
-        if info["wwid"] and info["wwid"] not in wwids:
-            wwids.append(info["wwid"])
+        if info['wwid'] and info['wwid'] not in wwids:
+            wwids.append(info['wwid'])
     return wwids
 
 
 def is_fc_boot():  # noqa: ANN201
     """Check if it boots from FC/FCoE device."""
     fc_wwids = scsi_wwid_of_fc_disks()
     if not fc_wwids:
         return False
 
     boot_dev = linux.get_boot_device()
     if not boot_dev:
-        print("FAIL: is_fc_boot() - Could not determine boot device")
+        logging.error('is_fc_boot() - Could not determine boot device')
         return False
 
     boot_wwid = linux.get_device_wwid(boot_dev)
     if not boot_dev:
-        print(f"WARN: is_fc_boot() - Could not determine boot WWID for {boot_dev}")
+        logging.warning(f'is_fc_boot() - Could not determine boot WWID for {boot_dev}')
         return False
 
     if boot_wwid in fc_wwids:
         return True
 
     return False
 
 
 # Return an array with all fc_hosts numbers
 def get_fc_hosts():  # noqa: ANN201
-    cmd = "ls " + host_path
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = 'ls ' + host_path
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     # remove 'host' prefix
-    output = re.sub("host", "", output)
+    output = re.sub('host', '', output)
     return output.split()
 
 
 def get_fc_host_wwpn(host):  # noqa: ANN001, ANN201
     """Return the WWPN of specific sts."""
-    host_port_path = f"/sys/class/fc_host/host{host}/port_name"
-    cmd = "cat " + host_port_path
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    host_port_path = f'/sys/class/fc_host/host{host}/port_name'
+    cmd = 'cat ' + host_port_path
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return standardize_wwpn(output)
 
 
 def fc_host_id_of_wwpn(wwpn):  # noqa: ANN001, ANN201
     """Given a WWPN, return its host id."""
     if not wwpn:
-        print("FAIL: fc_host_id_of_wwpn() - requires wwpn parameter")
+        logging.error('fc_host_id_of_wwpn() - requires wwpn parameter')
         return None
     fc_hosts = get_fc_hosts()
     for fc_host in fc_hosts:
         if get_fc_host_wwpn(fc_host) == wwpn:
             return fc_host
 
     return None
@@ -184,24 +185,24 @@
     rports = os.listdir(remote_port_path)
     if not rports:
         return None
     return rports
 
 
 def get_fc_host_remote_ports(host):  # noqa: ANN001, ANN201
-    cmd = f"ls {remote_port_path} | grep rport-{host}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'ls {remote_port_path} | grep rport-{host}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return output.split()
 
 
 def wwpn_of_rport(r_port):  # noqa: ANN001, ANN201
-    cmd = f"cat {remote_port_path}/{r_port}/port_name"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'cat {remote_port_path}/{r_port}/port_name'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return standardize_wwpn(output)
 
 
 def rport_of_h_wwpn_t_wwpn(h_wwpn, t_wwpn):  # noqa: ANN001, ANN201
     """Return the remote port of given wwpn
@@ -225,24 +226,24 @@
     host_rports = get_fc_host_remote_ports(host_id)
     if not host_rports:
         return None
 
     for rport in host_rports:
         r_wwpn = wwpn_of_rport(rport)
         if not r_wwpn:
-            # print("FAIL: rport_of_h_wwpn_t_wwpn() - Could not get wwpn of rport %s" % rport)
+            # logging.error("rport_of_h_wwpn_t_wwpn() - Could not get wwpn of rport %s" % rport)
             continue
         if t_wwpn == r_wwpn:
             return rport
     return None
 
 
 def fc_target_id_of_wwpn(wwpn):  # noqa: ANN001, ANN201
     if not wwpn:
-        print("FAIL: fc_target_id_of_wwpn() - requires wwpn parameter")
+        logging.error('fc_target_id_of_wwpn() - requires wwpn parameter')
         return None
     t_ids = None
 
     # Get target id of all ports
     rport_id_2_target_id_dict = rport_id_2_target_id()
     if not rport_id_2_target_id_dict:
         return None
@@ -291,15 +292,15 @@
 
     for host in hosts:
         r_ports = get_fc_host_remote_ports(host)
         if r_ports:
             for r_port in r_ports:
                 wwpn = wwpn_of_rport(r_port)
                 if not wwpn:
-                    # print("FAIL: Could not find wwpn for r_port %s" % r_port)
+                    # logging.error("Could not find wwpn for r_port %s" % r_port)
                     continue
                 if wwpn in h_wwpns:
                     # We actually found our own WWPN, skip it
                     continue
                 if not wwpns:
                     wwpns = []
                 if wwpn not in wwpns:
@@ -318,75 +319,75 @@
         t_wwpn         # Storage Array front point WWPN
     Returns
         target_id      # like "0:1:0"
             or
         None           # error.
     """
     if not t_wwpn or not h_wwpn:
-        print("FAIL: fc_target_id_of_htwwpn() - requires t_wwpn and h_wwpn parameters")
+        logging.error('fc_target_id_of_htwwpn() - requires t_wwpn and h_wwpn parameters')
         return None
 
     scsi_host_id = fc_host_id_of_wwpn(h_wwpn)
     target_ids = fc_target_id_of_wwpn(t_wwpn)
     if not target_ids:
-        print("FAIL: fc_target_id_of_htwwpn(): No FC target assigned to target WWPN {t_wwpn}")
+        logging.error('fc_target_id_of_htwwpn(): No FC target assigned to target WWPN {t_wwpn}')
         return None
 
     for t_id in target_ids:
         m = regex_target.match(t_id)
         if m and scsi_host_id == m.group(1):
             return t_id
     return None
 
 
 def scsi_disk_of_htwwpn_wwid(h_wwpn, t_wwpn, wwid):  # noqa: ANN001, ANN201
     """Get the scsi disk name connected to specific host and target port and has
     given wwid.
     """
     if not h_wwpn or not t_wwpn or not wwid:
-        print("FAIL: scsi_disk_of_htwwpn_wwid() - requires h_wwpn, t_wwpn and wwid as parameters")
+        logging.error('scsi_disk_of_htwwpn_wwid() - requires h_wwpn, t_wwpn and wwid as parameters')
         return None
 
     target_id = fc_target_id_of_htwwpn(t_wwpn=t_wwpn, h_wwpn=h_wwpn)
     if not target_id:
         return None
 
     scsi_disk_ids = scsi.scsi_ids_of_wwid(wwid)
     if not scsi_disk_ids:
         return False
 
     for scsi_disk_id in scsi_disk_ids:
-        if re.match(r"%s:\d+$" % target_id, scsi_disk_id):
+        if re.match(r'%s:\d+$' % target_id, scsi_disk_id):
             disk_name = scsi.get_scsi_disk_name(scsi_disk_id)
             if not disk_name:
-                print(f"FAIL: Could not get SCSI disk name of: {scsi_disk_id}")
+                logging.error(f'Could not get SCSI disk name of: {scsi_disk_id}')
                 return False
             return disk_name
     return None
 
 
 def get_fc_host_rport_targets(host, r_port):  # noqa: ANN001, ANN201
-    cmd = f"ls /sys/bus/scsi/devices/host{host}/{r_port} | grep target"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'ls /sys/bus/scsi/devices/host{host}/{r_port} | grep target'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
-    output = re.sub("target", "", output)
+    output = re.sub('target', '', output)
     return output.split()
 
 
 def get_fc_host_rport_target_devices(host, r_port, target):  # noqa: ANN001, ANN201
     if not host or not r_port or not target:
-        print("FAIL: get_fc_host_rport_target_devices. Usage: host, r_port, target")
+        logging.error('get_fc_host_rport_target_devices. Usage: host, r_port, target')
         return None
 
     cmd = f'ls /sys/bus/scsi/devices/host{host}/{r_port}/target{target} | grep "{target}"'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
-    output = re.sub("target", "", output)
+    output = re.sub('target', '', output)
     return output.split()
 
 
 def rport_id_2_target_id():  # noqa: ANN201
     """Usage
         rport_id_2_target_id()
     Purpose
@@ -408,100 +409,100 @@
 
     rport_id_2_target_id_dict = None
     rports = get_rports()
     if not rports:
         return None
     for rport in rports:
         # search for targets connected to this rport
-        rport_target_sys_root_path = f"{remote_port_path}/{rport}/device"
+        rport_target_sys_root_path = f'{remote_port_path}/{rport}/device'
         entries = os.listdir(rport_target_sys_root_path)
 
         for entry in entries:
             m = regex_target_id.match(entry)
             if m:
                 if not rport_id_2_target_id_dict:
                     rport_id_2_target_id_dict = {}
-                rport_id_2_target_id_dict[rport] = f"{m.group(1)}:{m.group(2)}:{m.group(3)}"
+                rport_id_2_target_id_dict[rport] = f'{m.group(1)}:{m.group(2)}:{m.group(3)}'
 
     return rport_id_2_target_id_dict
 
 
 def fc_host_transport_type(scsi_host_id):  # noqa: ANN001, ANN201
     if not scsi_host_id:
-        print("FAIL: fc_host_transport_type - requires scsi_host_id")
+        logging.error('fc_host_transport_type - requires scsi_host_id')
         return None
 
     host_model2transport = {
-        "QLE2462": "FC",
-        "QLE2772": "FC",
-        "QLE8262": "FCoE",
-        "QLE8362": "FCoE",
-        "CN1000Q": "FCoE",
-        "QLogic-1020": "FCoE",
-        "554FLR-SFP+": "FCoE",
-        "Intel 82599": "FCoE",
+        'QLE2462': 'FC',
+        'QLE2772': 'FC',
+        'QLE8262': 'FCoE',
+        'QLE8362': 'FCoE',
+        'CN1000Q': 'FCoE',
+        'QLogic-1020': 'FCoE',
+        '554FLR-SFP+': 'FCoE',
+        'Intel 82599': 'FCoE',
     }
     host_info = scsi.query_scsi_host_info(scsi_host_id)
     # Check first if we can find what transport by HBA model
-    model_keys = ["model", "model_name"]
+    model_keys = ['model', 'model_name']
     for key in model_keys:
         if key in list(host_info.keys()) and host_info[key] in list(host_model2transport.keys()):
             return host_model2transport[host_info[key]]
 
     # Second option try to parse model description
-    if "model_description" in list(host_info.keys()):
-        fc_regex1 = re.compile("Fibre Channel")
-        fc_regex2 = re.compile(" FC ")
-        fcoe_regex = re.compile("FCoE")
-        if fc_regex1.search(host_info["model_description"]):
-            return "FC"
-        if fc_regex2.search(host_info["model_description"]):
-            return "FC"
-        if fcoe_regex.search(host_info["model_description"]):
-            return "FCoE"
-
-    if "model_desc" in list(host_info.keys()):
-        fc_regex1 = re.compile("Fibre Channel")
-        fc_regex2 = re.compile(" FC ")
-        fcoe_regex = re.compile("FCoE")
-        if fc_regex1.search(host_info["model_desc"]):
-            return "FC"
-        if fc_regex2.search(host_info["model_desc"]):
-            return "FC"
-        if fcoe_regex.search(host_info["model_desc"]):
-            return "FCoE"
-
-    if "modeldesc" in list(host_info.keys()):
-        fc_regex = re.compile("Fibre Channel")
-        fcoe_regex = re.compile("FCoE")
-        if fc_regex.search(host_info["modeldesc"]):
-            return "FC"
-        if fcoe_regex.search(host_info["modeldesc"]):
-            return "FCoE"
-
-    if "protocol" in list(host_info.keys()):
-        if host_info["protocol"] == "fc":
-            return "FC"
-        if host_info["protocol"] == "fcoe":
-            return "FCoE"
-
-    if "symbolic_name" in list(host_info.keys()):
-        fc_regex = re.compile("Fibre Channel")
-        fcoe_regex = re.compile("fcoe")
-        if fc_regex.search(host_info["symbolic_name"]):
-            return "FC"
-        if fcoe_regex.search(host_info["symbolic_name"]):
-            return "FCoE"
+    if 'model_description' in list(host_info.keys()):
+        fc_regex1 = re.compile('Fibre Channel')
+        fc_regex2 = re.compile(' FC ')
+        fcoe_regex = re.compile('FCoE')
+        if fc_regex1.search(host_info['model_description']):
+            return 'FC'
+        if fc_regex2.search(host_info['model_description']):
+            return 'FC'
+        if fcoe_regex.search(host_info['model_description']):
+            return 'FCoE'
+
+    if 'model_desc' in list(host_info.keys()):
+        fc_regex1 = re.compile('Fibre Channel')
+        fc_regex2 = re.compile(' FC ')
+        fcoe_regex = re.compile('FCoE')
+        if fc_regex1.search(host_info['model_desc']):
+            return 'FC'
+        if fc_regex2.search(host_info['model_desc']):
+            return 'FC'
+        if fcoe_regex.search(host_info['model_desc']):
+            return 'FCoE'
+
+    if 'modeldesc' in list(host_info.keys()):
+        fc_regex = re.compile('Fibre Channel')
+        fcoe_regex = re.compile('FCoE')
+        if fc_regex.search(host_info['modeldesc']):
+            return 'FC'
+        if fcoe_regex.search(host_info['modeldesc']):
+            return 'FCoE'
+
+    if 'protocol' in list(host_info.keys()):
+        if host_info['protocol'] == 'fc':
+            return 'FC'
+        if host_info['protocol'] == 'fcoe':
+            return 'FCoE'
+
+    if 'symbolic_name' in list(host_info.keys()):
+        fc_regex = re.compile('Fibre Channel')
+        fcoe_regex = re.compile('fcoe')
+        if fc_regex.search(host_info['symbolic_name']):
+            return 'FC'
+        if fcoe_regex.search(host_info['symbolic_name']):
+            return 'FCoE'
 
-    if "driver" in list(host_info.keys()) and host_info["driver"] in ["bnx2fc", "qedf"]:
-        return "FCoE"
+    if 'driver' in list(host_info.keys()) and host_info['driver'] in ['bnx2fc', 'qedf']:
+        return 'FCoE'
 
-    print(f"DEBUG: Could not figure out if controller {scsi_host_id} is FC or FCoE")
+    print(f'DEBUG: Could not figure out if controller {scsi_host_id} is FC or FCoE')
     print(host_info)
-    return "(TODO)FC/FCoE"
+    return '(TODO)FC/FCoE'
 
 
 def get_value_rport_parameter(r_port, r_port_param):  # noqa: ANN001, ANN201
     """Usage
         get_value_rport_parameter(r_port, r_port_param)
     Purpose
         Query out the r_port_param via sys:
@@ -511,25 +512,25 @@
         r_port_param    # like "dev_loss_tmo"
     Returns
         parameter value
             or
         None.
     """
     if not r_port or not r_port_param:
-        print("FAIL: get_value_rport_parameter() - requires r_port and r_port_param as parameter")
+        logging.error('get_value_rport_parameter() - requires r_port and r_port_param as parameter')
         return None
 
-    sys_r_port_param = f"{remote_port_path}/{r_port}/{r_port_param}"
+    sys_r_port_param = f'{remote_port_path}/{r_port}/{r_port_param}'
     if not Path(sys_r_port_param).is_file():
-        print(f"FAIL: get_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
+        logging.error(f"get_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
         return None
 
-    ret, value = run_ret_out(f"cat {sys_r_port_param}", return_output=True, verbose=False)
+    ret, value = run_ret_out(f'cat {sys_r_port_param}', return_output=True)
     if ret != 0:
-        print(f"FAIL: get_value_rport_parameter() - Could not read {sys_r_port_param}")
+        logging.error(f'get_value_rport_parameter() - Could not read {sys_r_port_param}')
         # print command output
         print(value)
         return None
 
     return value
 
 
@@ -545,22 +546,22 @@
         value           # like "60"
     Returns
         True
             or
         False.
     """
     if not r_port or not r_port_param or value is None:
-        print("FAIL: set_value_rport_parameter() - requires r_port, r_port_param and value as parameter")
+        logging.error('set_value_rport_parameter() - requires r_port, r_port_param and value as parameter')
         return False
 
-    sys_r_port_param = f"{remote_port_path}/{r_port}/{r_port_param}"
+    sys_r_port_param = f'{remote_port_path}/{r_port}/{r_port_param}'
     if not Path(sys_r_port_param).is_file():
-        print(f"FAIL: set_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
+        logging.error(f"set_value_rport_parameter() - File '{sys_r_port_param}' does not exist")
         return False
 
-    ret, output = run_ret_out(f"echo {value} > {sys_r_port_param}", return_output=True, verbose=False)
+    ret, output = run_ret_out(f'echo {value} > {sys_r_port_param}', return_output=True)
     if ret != 0:
-        print(f"FAIL: set_value_rport_parameter() - Could not set {sys_r_port_param} to {value}")
+        logging.error(f'set_value_rport_parameter() - Could not set {sys_r_port_param} to {value}')
         # print command output
         print(output)
         return False
     return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/fio.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/fio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,152 +1,152 @@
 """fio.py: Module to run FIO util."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
 import subprocess
 import sys
 
 from sts import linux
 from sts.utils.cmdline import exists, run, run_ret_out
 
 fio_default_options = {
-    "rw": "randrw",  # Type of I/O pattern. Supported(read, write, trim, randread, randwrite, rw, randrw, trimwrite)
-    "name": "fio_test",  # signalling the start of a new job.
-    "filename": None,  # device or filename
-    "direct": 1,  # If true, use non-buffered I/O (usually O_DIRECT)
-    "iodepth": 1,  # Number  of  I/O  units  to keep in flight against the file. Note that increasing
+    'rw': 'randrw',  # Type of I/O pattern. Supported(read, write, trim, randread, randwrite, rw, randrw, trimwrite)
+    'name': 'fio_test',  # signalling the start of a new job.
+    'filename': None,  # device or filename
+    'direct': 1,  # If true, use non-buffered I/O (usually O_DIRECT)
+    'iodepth': 1,  # Number  of  I/O  units  to keep in flight against the file. Note that increasing
     # iodepth beyond 1 will not affect synchronous ioengines
-    "runtime": None,  # Terminate processing after the specified number of seconds.
-    "size": None,  #
-    "time_based": None,  # If given, run for the specified runtime duration even if the files are
+    'runtime': None,  # Terminate processing after the specified number of seconds.
+    'size': None,  #
+    'time_based': None,  # If given, run for the specified runtime duration even if the files are
     # completely read or written.
-    "numjobs": 1,  # Number of clones (processes/threads performing the same workload) of this job
-    "bs": "4k",  # lock  size for I/O units.
-    "verify": None,  # Method  of verifying file contents after each iteration of the job
+    'numjobs': 1,  # Number of clones (processes/threads performing the same workload) of this job
+    'bs': '4k',  # lock  size for I/O units.
+    'verify': None,  # Method  of verifying file contents after each iteration of the job
 }  # (supports: md5 crc16 crc32 crc32c crc32c-intel crc64 crc7 sha256 sha512 sha1 xxhash)
 
 fio_default_verify_options = {
-    "verify_backlog": 1024,  # fio will write only N blocks before verifying these blocks.
+    'verify_backlog': 1024,  # fio will write only N blocks before verifying these blocks.
     # Set to None to verify after all IO is written
-    "verify_fatal": 1,  # If true, exit the job on the first observed verification failure
-    "do_verify": 1,
-    "verify": "crc32c",
+    'verify_fatal': 1,  # If true, exit the job on the first observed verification failure
+    'do_verify': 1,
+    'verify': 'crc32c',
 }
 
 
 def install_fio():  # noqa: ANN201
-    pkg = "fio"
+    pkg = 'fio'
     if linux.install_package(pkg):
         return True
-    if run("fio >/dev/null 2>&1").returncode == 1:
+    if run('fio >/dev/null 2>&1').rc == 1:
         return True
     # Try to install FIO from source
     return install_fio_from_src()
 
 
 def install_fio_from_src():  # noqa: ANN201
-    git_url = "git://git.kernel.org/pub/scm/linux/kernel/git/axboe/fio.git"
+    git_url = 'git://git.kernel.org/pub/scm/linux/kernel/git/axboe/fio.git'
 
-    if not linux.install_package("libaio-devel"):
-        print("FAIL: Could not install libaio-devel")
+    if not linux.install_package('libaio-devel'):
+        logging.error('Could not install libaio-devel')
         return False
 
-    if not linux.install_package("zlib-devel"):
-        print("FAIL: Could not install zlib-devel")
+    if not linux.install_package('zlib-devel'):
+        logging.error('Could not install zlib-devel')
         return False
 
-    if run(f"git clone {git_url}").returncode != 0:
-        print("FAIL: Could not clone fio repo")
+    if run(f'git clone {git_url}').rc != 0:
+        logging.error('Could not clone fio repo')
         return False
 
-    print("INFO: Installing FIO")
-    if run("cd fio && ./configure && make && make install").returncode != 0:
-        print("FAIL: Could not build fio")
+    logging.info('Installing FIO')
+    if run('cd fio && ./configure && make && make install').rc != 0:
+        logging.error('Could not build fio')
         return False
 
-    if not exists("fio"):
-        print("FAIL: FIO did not install properly")
+    if not exists('fio'):
+        logging.error('FIO did not install properly')
         return False
     return True
 
 
 # TODO: rewrite to cmdline.run()
-def fio_stress(of, verbose=False, return_output=False, **fio_opts):  # noqa: ANN001, ANN003, ANN201
+def fio_stress(of, return_output=False, **fio_opts):  # noqa: ANN001, ANN003, ANN201
     # For compatibility with tests using other named parameters
     convert_param = {
-        "io_type": "rw",
-        "time": "runtime",
-        "thread": "numjobs",
-        "log_file": "output",
+        'io_type': 'rw',
+        'time': 'runtime',
+        'thread': 'numjobs',
+        'log_file': 'output',
     }
 
     for key in convert_param:
         if key in list(fio_opts.keys()):
             fio_opts[convert_param[key]] = fio_opts.pop(key)
 
-    fio_opts["filename"] = of
+    fio_opts['filename'] = of
 
     for opt in fio_default_options:
         if opt not in list(fio_opts.keys()):
             fio_opts[opt] = fio_default_options[opt]
 
-    if int(fio_opts["numjobs"]) > 1:
-        fio_opts["group_reporting"] = 1
+    if int(fio_opts['numjobs']) > 1:
+        fio_opts['group_reporting'] = 1
 
-    if fio_opts["verify"] is not None:
+    if fio_opts['verify'] is not None:
         fio_opts.update(fio_default_verify_options)
 
-    if not exists("fio"):
-        print("FATAL: fio is not installed")
+    if not exists('fio'):
+        logging.critical('fio is not installed')
         return False
 
-    fio_param = ""
+    fio_param = ''
     for key in list(fio_opts.keys()):
         if fio_opts[key]:
             fio_param += f"--{key}='{fio_opts[key]}' "
 
-    if "fiojob" in list(fio_opts.keys()):
+    if 'fiojob' in list(fio_opts.keys()):
         fio_param = f"{fio_opts['fiojob']} --filename={fio_opts['filename']}"
 
-    cmd = f"fio {fio_param}"
+    cmd = f'fio {fio_param}'
     # Append time information to command
     date = 'date "+%Y-%m-%d %H:%M:%S"'
     p = subprocess.Popen(date, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     stdout, _ = p.communicate()
-    stdout = stdout.decode("ascii", "ignore")
-    stdout = stdout.rstrip("\n")
-    if not verbose:  # If verbose option is selected, the run() will print the fio command.
-        print(f"INFO: [{stdout}] FIO Running: '{cmd}'...")
+    stdout = stdout.decode('ascii', 'ignore')
+    stdout = stdout.rstrip('\n')
+    logging.info(f"[{stdout}] FIO Running: '{cmd}'...")
 
-    # print("INFO: Running %s" % cmd)
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    # logging.info("Running %s" % cmd)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: running FIO")
+        logging.error('running FIO')
         print(output)
         if return_output:
             return False, None
         return False
 
-    print("INFO: FIO executed successfully")
+    logging.info('FIO executed successfully')
     if return_output:
         return True, output
 
     return True
 
 
-def fio_stress_background(of, verbose=False, **fio_opts):  # noqa: ANN001, ANN003, ANN201
+def fio_stress_background(of, **fio_opts):  # noqa: ANN001, ANN003, ANN201
     """Run FIO on background."""
     newpid = os.fork()
     if newpid == 0:
         # Trying to flush stdout to avoid duplicated lines when running hba_test
         sys.stdout.flush()
-        rt = fio_stress(of, verbose=verbose, **fio_opts)
+        rt = fio_stress(of, **fio_opts)
         if not rt:
             os._exit(1)  # noqa: SLF001
         os._exit(0)  # noqa: SLF001
         return None
 
     sys.stdout.flush()
-    print("INFO: fio_stress_background(): Child thread %d is running FIO Stress" % newpid)
+    logging.info(f'fio_stress_background(): Child thread {newpid} is running FIO Stress')
     return newpid
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/iscsi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,107 @@
 """iscsi.py: Module with methods for iSCSI initiator."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import re
 from pathlib import Path
-from typing import ClassVar, Dict, List, Literal, Optional, Union, TypedDict
+from typing import ClassVar, Dict, List, Literal, Optional, TypedDict, Union
+
+from testinfra.backend.base import CommandResult
 
 from sts import linux, mp, net, scsi
-from sts.utils.cmdline import StsCompletedProcess, run, run_ret_out
+from sts.utils import remove_prefix
+from sts.utils.cmdline import run
 
-PACKAGE_NAME = "iscsi-initiator-utils"
-CLI_NAME = "iscsiadm"
-ISCSID_SERVICE_NAME = "iscsid"
-ISCSIUIO_SERVICE_NAME = "iscsiuio"
+PACKAGE_NAME = 'iscsi-initiator-utils'
+CLI_NAME = 'iscsiadm'
+ISCSID_SERVICE_NAME = 'iscsid'
+ISCSIUIO_SERVICE_NAME = 'iscsiuio'
 
 
 class IscsiAdm:
     """Class for `iscsiadm` cli tool (iscsi-initiator-utils)."""
 
     def __init__(
         self,
         debug_level: Literal[0, 1, 2, 3, 4, 5, 6, 7, 8] = 0,
         disable_check: bool = False,
-        verbose: bool = True,
     ) -> None:
         """Args:
         debug_level: print iscsiadm debug info (0-8)
         disable_check: disable argument validation.
         """
         self.disable_check = disable_check
         self.debug_level = debug_level
-        self.verbose = verbose
 
-        if not linux.install_package(PACKAGE_NAME, check=True, verbose=self.verbose):
-            print(f"FATAL: Could not install {PACKAGE_NAME}")
+        if not linux.install_package(PACKAGE_NAME, check=True):
+            logging.critical(f'Could not install {PACKAGE_NAME}')
 
     # available modes and respective short options available as per iscsiadm.c
     MODES: ClassVar[Dict[str, str]] = {
-        "discovery": "DSIPdntplov",
-        "discoverydb": "DSIPdntplov",
-        "node": "RsPIdlSonvupTULW",
-        "session": "PiRdrusonuSv",
-        "host": "CHdPotnvxA",
-        "iface": "HIdnvPoCabci",
-        "fw": "dlWnv",
+        'discovery': 'DSIPdntplov',
+        'discoverydb': 'DSIPdntplov',
+        'node': 'RsPIdlSonvupTULW',
+        'session': 'PiRdrusonuSv',
+        'host': 'CHdPotnvxA',
+        'iface': 'HIdnvPoCabci',
+        'fw': 'dlWnv',
     }
 
     OPTIONS: ClassVar[Dict[str, str]] = {
-        "p": "portal",
-        "T": "targetname",
-        "I": "interface",
-        "o": "op",
-        "t": "type",
-        "n": "name",
-        "v": "value",
-        "H": "host",
-        "r": "sid",
-        "R": "rescan",
-        "P": "print",
-        "D": "discover",
-        "l": "login",
-        "L": "loginall",
-        "u": "logout",
-        "U": "logoutall",
-        "s": "stats",
-        "k": "killiscsid",
-        "d": "debug",
-        "S": "show",
-        "V": "version",
-        "h": "help",
-        "C": "submode",
-        "a": "ip",
-        "b": "packetsize",
-        "c": "count",
-        "i": "interval",
-        "x": "index",
-        "A": "portal_type",
-        "W": "no_wait",
+        'p': 'portal',
+        'T': 'targetname',
+        'I': 'interface',
+        'o': 'op',
+        't': 'type',
+        'n': 'name',
+        'v': 'value',
+        'H': 'host',
+        'r': 'sid',
+        'R': 'rescan',
+        'P': 'print',
+        'D': 'discover',
+        'l': 'login',
+        'L': 'loginall',
+        'u': 'logout',
+        'U': 'logoutall',
+        's': 'stats',
+        'k': 'killiscsid',
+        'd': 'debug',
+        'S': 'show',
+        'V': 'version',
+        'h': 'help',
+        'C': 'submode',
+        'a': 'ip',
+        'b': 'packetsize',
+        'c': 'count',
+        'i': 'interval',
+        'x': 'index',
+        'A': 'portal_type',
+        'W': 'no_wait',
     }
 
     def validate_mode(self, mode: str) -> None:
         """Checks if mode is valid iscsiadm mode.
 
         Args:
           mode: Example: "discovery"
         """
         if mode not in self.MODES:
-            err_msg = f"Invalid {CLI_NAME} mode: {mode}"
+            err_msg = f'Invalid {CLI_NAME} mode: {mode}'
             raise ValueError(err_msg)
 
     def validate_arguments(self, mode: str, arguments: Union[Dict[str, str], Dict[str, Optional[str]]]) -> None:
         available_options: List[str] = self.get_short_options_list(mode) + self.get_long_options_list(mode)
         for key, _value in arguments.items():
-            key_to_check = key.strip("-")
+            key_to_check = key.strip('-')
             if key_to_check not in available_options:
-                err_msg = f"Invalid {CLI_NAME} argument: {key}"
+                err_msg = f'Invalid {CLI_NAME} argument: {key}'
                 raise ValueError(err_msg)
 
     def get_short_options_list(self, mode: str) -> List[str]:
         if mode not in self.MODES.keys():
             raise ValueError
         return [*self.MODES[mode]]
 
@@ -109,76 +111,75 @@
         return [self.OPTIONS[short_option] for short_option in [*self.MODES[mode]]]
 
     def available_options(self, mode: str) -> List[str]:
         return self.get_short_options_list(mode) + self.get_long_options_list(mode)
 
     def _run(
         self,
-        mode: str = "",
+        mode: str = '',
         arguments: Optional[Union[Dict[str, str], Dict[str, Optional[str]]]] = None,
-        timeout: Union[int, None] = None,
-    ) -> StsCompletedProcess:
+    ) -> CommandResult:
         if mode is not None:
             self.validate_mode(mode)
         if arguments is not None and self.disable_check is not True:
             self.validate_arguments(mode, arguments)
 
-        command_list: List[str] = [CLI_NAME, "--mode", mode]
+        command_list: List[str] = [CLI_NAME, '--mode', mode]
         if arguments is not None:
-            command_list = command_list + [f"{k}" if v is None else f"{k} {v}" for k, v in arguments.items()]
+            command_list = command_list + [f'{k}' if v is None else f'{k} {v}' for k, v in arguments.items()]
         if self.debug_level:
-            command_list = [*command_list, "--debug", str(self.debug_level)]
-        command: str = " ".join(command_list)
-        return run(command, capture_output=True, timeout=timeout, verbose=self.verbose)
+            command_list = [*command_list, '--debug', str(self.debug_level)]
+        command: str = ' '.join(command_list)
+        return run(command)
 
     def iface(
         self,
         op: str,
         iface: str,
         name: Optional[str] = None,
         value: Optional[str] = None,
-    ) -> StsCompletedProcess:
+    ) -> CommandResult:
         return self._run(
-            mode="iface",
-            arguments={"-o": op, "-n": name, "-v": value, "-I": iface},
+            mode='iface',
+            arguments={'-o': op, '-n': name, '-v': value, '-I': iface},
         )
 
-    def iface_update(self, iface: str, name: str, value: str) -> StsCompletedProcess:
-        return self.iface(op="update", iface=iface, name=f"iface.{name}", value=value)
+    def iface_update(self, iface: str, name: str, value: str) -> CommandResult:
+        return self.iface(op='update', iface=iface, name=f'iface.{name}', value=value)
 
-    def iface_update_iqn(self, iface: str, iqn: str) -> StsCompletedProcess:
-        return self.iface_update(iface=iface, name="initiatorname", value=iqn)
+    def iface_update_iqn(self, iface: str, iqn: str) -> CommandResult:
+        return self.iface_update(iface=iface, name='initiatorname', value=iqn)
 
-    def iface_update_ip(self, iface: str, ip: str) -> StsCompletedProcess:
-        return self.iface_update(iface=iface, name="iface.ipaddress", value=ip)
+    def iface_update_ip(self, iface: str, ip: str) -> CommandResult:
+        return self.iface_update(iface=iface, name='iface.ipaddress', value=ip)
 
     def iface_exists(self, iface: str) -> bool:
-        return self.iface(op="show", iface=iface).returncode == 0
+        return self.iface(op='show', iface=iface).succeeded
 
     def discovery(
         self,
         portal: str,
-        type: str = "st",  # noqa: A002
+        type: str = 'st',  # noqa: A002
         interface: Optional[str] = None,
         **kwargs: str,
-    ) -> StsCompletedProcess:
-        arguments = {"-t": type, "-p": portal, **kwargs}
+    ) -> CommandResult:
+        arguments = {'-t': type, '-p': portal, **kwargs}
         if interface:
-            arguments.update({"-I": interface})
-        return self._run(mode="discovery", arguments=arguments)
+            arguments.update({'-I': interface})
+        return self._run(mode='discovery', arguments=arguments)
 
-    def node(self, **kwargs: Union[str, Optional[str]]) -> StsCompletedProcess:
-        return self._run(mode="node", arguments={**kwargs})
+    def node(self, **kwargs: Union[str, Optional[str]]) -> CommandResult:
+        return self._run(mode='node', arguments={**kwargs})
 
-    def node_login(self, **kwargs: str) -> StsCompletedProcess:
-        arguments = {"--login": None, **kwargs}
+    def node_login(self, **kwargs: str) -> CommandResult:
+        arguments = {'--login': None, **kwargs}
         return self.node(**arguments)
 
-    def node_logout(self, **kwargs: str) -> StsCompletedProcess:
-        arguments = {"--logout": None, **kwargs}
+    def node_logout(self, **kwargs: str) -> CommandResult:
+        arguments = {'--logout': None, **kwargs}
         return self.node(**arguments)
 
 
 class IfaceVars(TypedDict):
     hwaddress: str
     iscsi_ifacename: str
     net_ifacename: str
@@ -250,244 +251,244 @@
     max_burst_len: str
     chap_auth: str
     bidi_chap: str
     strict_login_compliance: str
     discovery_auth: str
     discovery_logout: str
 
+
 class TargetVars(TypedDict):
     name: str  # iqn
     interface: str
     portal: str  # ip or hostname
     type: str  # discovery type
 
+
 class ConfVars(TypedDict):
     initiatorname: str  # iqn.1994-05.redhat:example
     targets: List[TargetVars]
     ifaces: List[IfaceVars]
 
+
 class AuthFields(TypedDict):
     tbl_idx: str
     authmethod: str
     username: str
     password: str
     password_length: str
     username_in: str
     password_in: str
 
 
 def setup(variables: ConfVars) -> bool:
     """Configure iSCSI initiator based on env variables."""
-    iscsiadm = IscsiAdm(verbose=True)
+    iscsiadm = IscsiAdm()
 
-    if "initiatorname" in variables:
-        if not set_initiatorname(variables["initiatorname"]):
+    if 'initiatorname' in variables:
+        if not set_initiatorname(variables['initiatorname']):
             return False
-        linux.service_restart(ISCSID_SERVICE_NAME, verbose=False)
+        linux.service_restart(ISCSID_SERVICE_NAME)
 
-    if "ifaces" in variables:
-        for iface in variables["ifaces"]:
-            ifacename = iface["iscsi_ifacename"]
-            if ("qedi" in ifacename or "bnx2i" in ifacename) and not linux.is_service_running(ISCSIUIO_SERVICE_NAME):
+    if 'ifaces' in variables:
+        for iface in variables['ifaces']:
+            ifacename = iface['iscsi_ifacename']
+            if ('qedi' in ifacename or 'bnx2i' in ifacename) and not linux.is_service_running(ISCSIUIO_SERVICE_NAME):
                 linux.service_enable(ISCSIUIO_SERVICE_NAME, now=True)
-            if not iscsiadm.iface_exists(iface = ifacename):
+            if not iscsiadm.iface_exists(iface=ifacename):
                 create_iscsi_iface(iface_name=ifacename)
             for n, v in iface.items():
-                if n == "iscsi_ifacename":
+                if n == 'iscsi_ifacename':
                     continue
-                completed_process = iscsiadm.iface_update(iface=ifacename, name=n, value=v)
-                ret = completed_process.returncode
-                out = completed_process.output
+                completed_process = iscsiadm.iface_update(iface=ifacename, name=n, value=str(v))
+                ret = completed_process.rc
+                out = completed_process.stdout
                 if ret != 0:
-                    print(f"FAIL: iscsi update command returned {ret}. Output: {out}")
+                    logging.error(f'iscsi update command returned {ret}. Output: {out}')
                     return False
 
-    if "targets" in variables:
-        for target in variables["targets"]:
+    if 'targets' in variables:
+        for target in variables['targets']:
             if iscsiadm.discovery(**target) != 0:
                 return False
 
     if not linux.is_service_enabled(ISCSID_SERVICE_NAME):
         linux.service_enable(ISCSID_SERVICE_NAME)
     return True
 
 
 def discovery_login(iface_name, portal, iqn, iface_ip=None, subnet_mask=None, gateway=None) -> bool:  # noqa: ANN001
     if not iface_name or not portal or not iqn:
-        print("FAIL: auto_conf() - Missing iface_name, portal or iqn")
+        logging.error('auto_conf() - Missing iface_name, portal or iqn')
         return False
 
     if iface_ip and not iface_set_ip(iface_name, iface_ip, subnet_mask, gateway):
-        print(f"FAIL: auto_conf() - Could not set IP for {iface_name}")
+        logging.error(f'auto_conf() - Could not set IP for {iface_name}')
         return False
 
-    print("INFO: IQN will be set to " + iqn)
+    logging.info(f'IQN will be set to {iqn}')
 
     if not iface_set_iqn(iqn, iface_name):
-        print(f"FAIL: auto_conf() - Could not set {iqn} to iface {iface_name}")
+        logging.error(f'auto_conf() - Could not set {iqn} to iface {iface_name}')
         return False
 
     if not discovery_st(portal, ifaces=iface_name, disc_db=True):
-        print(f"FAIL: auto_conf() - Could not discover any target on {portal} using iface {iface_name}")
+        logging.error(f'auto_conf() - Could not discover any target on {portal} using iface {iface_name}')
         return False
 
     if not node_login():
-        print("FAIL: auto_conf() - Could not login to new discovered portal")
+        logging.error('auto_conf() - Could not login to new discovered portal')
         return False
-    print(f"INFO: Iface {iface_name} logged in successfully to {portal}")
+    logging.info(f'Iface {iface_name} logged in successfully to {portal}')
 
     return True
 
 
 # used to match regex for each session information that we support
 supported_discovery_info = {
-    "address": r".*DiscoveryAddress: (\S+)",
-    "target": r".*Target: (\S+)",
-    "portal": r".*Portal: (\S+):(\S+),(\S+)",
-    "iface": r".*Iface Name: (\S+)",
+    'address': r'.*DiscoveryAddress: (\S+)',
+    'target': r'.*Target: (\S+)',
+    'portal': r'.*Portal: (\S+):(\S+),(\S+)',
+    'iface': r'.*Iface Name: (\S+)',
 }
 
 # used to match regex for each session information that we support
 supported_session_info = {
-    "t_iqn": r".*Target: (\S+)",
-    "h_iqn": r".*Iface Initiatorname: (\S+)",
-    "iface": r".*Iface Name: (\S+)",
-    "transport": r".*Iface Transport: (\S+)",
-    "iface_ip": r".*Iface IPaddress: (\S+)",
-    "mac": r".*Iface HWaddress: (\S+)",
-    "sid": r".*SID: (\S+)",
-    "host": r".*Host Number: (\S+).*State: (\S+)",  # e.g. Host Number: 6	State: running
-    "disks": r".*Attached scsi disk (\S+).*State: (\S+)",
+    't_iqn': r'.*Target: (\S+)',
+    'h_iqn': r'.*Iface Initiatorname: (\S+)',
+    'iface': r'.*Iface Name: (\S+)',
+    'transport': r'.*Iface Transport: (\S+)',
+    'iface_ip': r'.*Iface IPaddress: (\S+)',
+    'mac': r'.*Iface HWaddress: (\S+)',
+    'sid': r'.*SID: (\S+)',
+    'host': r'.*Host Number: (\S+).*State: (\S+)',  # e.g. Host Number: 6	State: running
+    'disks': r'.*Attached scsi disk (\S+).*State: (\S+)',
     # eg. Attached scsi disk sdb		State: running
-    "target_ip": r".*Current Portal: (\S+):[0-9]+,",
-    "persist_ip": r".*Persistent Portal: (\S+):[0-9]+,",
+    'target_ip': r'.*Current Portal: (\S+):[0-9]+,',
+    'persist_ip': r'.*Persistent Portal: (\S+):[0-9]+,',
     # negotiated parameters
-    "header_digest": r".*HeaderDigest: (\S+)",
-    "data_digest": r".*DataDigest: (\S+)",
-    "max_recv": r".*MaxRecvDataSegmentLength: (\S+)",
-    "max_xmit": r".*MaxXmitDataSegmentLength: (\S+)",
-    "first_burst": r".*FirstBurstLength: (\S+)",
-    "max_burst": r".*MaxBurstLength: (\S+)",
-    "immediate_data": r".*ImmediateData: (\S+)",
-    "initial_r2t": r".*InitialR2T: (\S+)",
-    "max_outst_r2t": r".*MaxOutstandingR2T: (\S+)",
+    'header_digest': r'.*HeaderDigest: (\S+)',
+    'data_digest': r'.*DataDigest: (\S+)',
+    'max_recv': r'.*MaxRecvDataSegmentLength: (\S+)',
+    'max_xmit': r'.*MaxXmitDataSegmentLength: (\S+)',
+    'first_burst': r'.*FirstBurstLength: (\S+)',
+    'max_burst': r'.*MaxBurstLength: (\S+)',
+    'immediate_data': r'.*ImmediateData: (\S+)',
+    'initial_r2t': r'.*InitialR2T: (\S+)',
+    'max_outst_r2t': r'.*MaxOutstandingR2T: (\S+)',
 }
 
-host_path = "/sys/class/iscsi_host/"
+host_path = '/sys/class/iscsi_host/'
 
 
 def is_iqn(iqn):  # noqa: ANN001, ANN201
-    if re.match(r"^iqn\.", iqn):
+    if re.match(r'^iqn\.', iqn):
         return True
     return False
 
 
 def install():  # noqa: ANN201
     """Install iscsiadm tool
     The arguments are:
     None
     Returns:
     True: If iscsiadm is installed correctly
     False: If some problem happened.
     """
     if not linux.install_package(PACKAGE_NAME):
-        print(f"FAIL: Could not install {PACKAGE_NAME}")
+        logging.error(f'Could not install {PACKAGE_NAME}')
         return False
 
     return True
 
 
-# Return an array with all iscsi_hosts numbers
-def get_iscsi_hosts():  # noqa: ANN201
-    cmd = "ls " + host_path
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        return None
-    # remove 'host' prefix
-    output = re.sub("host", "", output)
-    return output.split()
+def get_iscsi_hosts() -> List[str]:
+    return run(f'ls {host_path}').stdout.splitlines()
+
+
+def get_iscsi_host_numbers() -> List[str]:
+    hosts = get_iscsi_hosts()
+    return [h.lstrip('host') for h in hosts]
 
 
 # iSCSI discovery ###
 def query_discovery():  # noqa: ANN201
     """Query all iSCSI targets
     The arguments are:
     None
     Returns:
     Dict:    Dict with all discovered targets
     None:    If some problem happened.
     """
-    cmd = "iscsiadm -m discovery -P1"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
+    cp = run('iscsiadm -m discovery -P1')
+    if cp.failed:
         # If no target is found iscsiadm returns error code
         return None
-    lines = output.split("\n")
+    lines = cp.stdout.splitlines()
 
-    supported_discovery_modes = ["SENDTARGETS", "iSNS", "STATIC", "FIRMWARE"]
-    supported_mode_type = {"SENDTARGETS": "sendtargets", "iSNS": "isns"}
+    supported_discovery_modes = ['SENDTARGETS', 'iSNS', 'STATIC', 'FIRMWARE']
+    supported_mode_type = {'SENDTARGETS': 'sendtargets', 'iSNS': 'isns'}
 
     discovery_info_dict = {}
     discovery_address = None
     disc_mode = None
     target_name = None
 
     for line in lines:
         # print "(%s)" % line
         # Check if it is discovery mode information
-        m = re.match("(^.*):", line)
+        m = re.match('(^.*):', line)
         if m and m.group(1) in supported_discovery_modes:
             disc_mode = m.group(1)
             # We will use DiscoveryAddress as key
             discovery_info_dict[disc_mode] = {}
             discovery_address = None
             continue
 
         # We will use TargetAddress as key for the target dictionary
-        m = re.match(supported_discovery_info["address"], line)
+        m = re.match(supported_discovery_info['address'], line)
         if m:
             discovery_address = m.group(1)
             if discovery_address not in list(discovery_info_dict[disc_mode].keys()):
                 discovery_info_dict[disc_mode][discovery_address] = {}
-            disc_addr_regex = re.compile(r"(\S+),(\S+)")
+            disc_addr_regex = re.compile(r'(\S+),(\S+)')
             d = disc_addr_regex.match(discovery_address)
             if d:
-                discovery_info_dict[disc_mode][discovery_address]["disc_addr"] = d.group(1)
-                discovery_info_dict[disc_mode][discovery_address]["disc_port"] = d.group(2)
+                discovery_info_dict[disc_mode][discovery_address]['disc_addr'] = d.group(1)
+                discovery_info_dict[disc_mode][discovery_address]['disc_port'] = d.group(2)
 
             if disc_mode in list(supported_mode_type.keys()):
-                discovery_info_dict[disc_mode][discovery_address]["mode"] = supported_mode_type[disc_mode]
+                discovery_info_dict[disc_mode][discovery_address]['mode'] = supported_mode_type[disc_mode]
             continue
 
-        m = re.match(supported_discovery_info["target"], line)
+        m = re.match(supported_discovery_info['target'], line)
         if m:
             # FIRMWARE discovery might not use discovery address
             if not discovery_address:
-                discovery_address = "NotSet"
+                discovery_address = 'NotSet'
                 discovery_info_dict[disc_mode][discovery_address] = {}
 
             target_name = m.group(1)
-            if "targets" not in list(discovery_info_dict[disc_mode][discovery_address].keys()):
-                discovery_info_dict[disc_mode][discovery_address]["targets"] = {}
-            discovery_info_dict[disc_mode][discovery_address]["targets"][target_name] = {}
+            if 'targets' not in list(discovery_info_dict[disc_mode][discovery_address].keys()):
+                discovery_info_dict[disc_mode][discovery_address]['targets'] = {}
+            discovery_info_dict[disc_mode][discovery_address]['targets'][target_name] = {}
             continue
 
-        m = re.match(supported_discovery_info["portal"], line)
+        m = re.match(supported_discovery_info['portal'], line)
         if m:
-            discovery_info_dict[disc_mode][discovery_address]["targets"][target_name]["portal"] = {}
-            discovery_info_dict[disc_mode][discovery_address]["targets"][target_name]["portal"]["address"] = m.group(1)
-            discovery_info_dict[disc_mode][discovery_address]["targets"][target_name]["portal"]["port"] = m.group(2)
+            discovery_info_dict[disc_mode][discovery_address]['targets'][target_name]['portal'] = {}
+            discovery_info_dict[disc_mode][discovery_address]['targets'][target_name]['portal']['address'] = m.group(1)
+            discovery_info_dict[disc_mode][discovery_address]['targets'][target_name]['portal']['port'] = m.group(2)
             continue
 
-        m = re.match(supported_discovery_info["iface"], line)
+        m = re.match(supported_discovery_info['iface'], line)
         if m:
             iface = m.group(1)
-            if "iface" not in list(discovery_info_dict[disc_mode][discovery_address]["targets"][target_name].keys()):
-                discovery_info_dict[disc_mode][discovery_address]["targets"][target_name]["iface"] = []
-            discovery_info_dict[disc_mode][discovery_address]["targets"][target_name]["iface"].append(iface)
+            if 'iface' not in list(discovery_info_dict[disc_mode][discovery_address]['targets'][target_name].keys()):
+                discovery_info_dict[disc_mode][discovery_address]['targets'][target_name]['iface'] = []
+            discovery_info_dict[disc_mode][discovery_address]['targets'][target_name]['iface'].append(iface)
             continue
             # print "Found %s: %s" % (key, m.group(1))
 
     return discovery_info_dict
 
 
 def discovery_st(target, ifaces=None, disc_db=False):  # noqa: ANN001, ANN201
@@ -498,209 +499,209 @@
     disc_db:  To use discoverydb instead of discovery (optional).
 
     Returns:
     True:     If it discovered an iSCSI target
     False:    If some problem happened.
     """
     max_retries = 5
-    print("INFO: Executing Discovery_ST() with these arges:")
-    print(f"\tTarget: {target}")
+    logging.info('Executing Discovery_ST() with these arges:')
+    print(f'\tTarget: {target}')
     if ifaces:
-        print(f"\tIfaces: {ifaces}")
+        print(f'\tIfaces: {ifaces}')
 
-    disc_opt = "discovery"
+    disc_opt = 'discovery'
     operation = None
 
     if disc_db:
-        disc_opt = "discoverydb -D"
-        operation = "new"
+        disc_opt = 'discoverydb -D'
+        operation = 'new'
 
-    cmd = f"iscsiadm -m {disc_opt} -p {target}"
+    cmd = f'iscsiadm -m {disc_opt} -p {target}'
     if operation:
-        cmd += f" -o {operation}"
+        cmd += f' -o {operation}'
 
     if ifaces:
-        if ("bnx2i" in ifaces or "qedi" in ifaces) and linux.is_service_running(ISCSIUIO_SERVICE_NAME) != 0:
+        if ('bnx2i' in ifaces or 'qedi' in ifaces) and linux.is_service_running(ISCSIUIO_SERVICE_NAME) != 0:
             linux.service_enable(ISCSIUIO_SERVICE_NAME, now=True)
-        interfaces = ifaces.split(" ")
+        interfaces = ifaces.split(' ')
         for interface in interfaces:
-            cmd += f" -I {interface}"
-    cmd += " -t st"
+            cmd += f' -I {interface}'
+    cmd += ' -t st'
     retries = 0
-    retcode, data = run_ret_out(cmd, return_output=True, verbose=True)
-    while retcode == 0 and "(err 29)" in data and retries < max_retries:
-        retcode, data = run_ret_out(cmd, return_output=True, verbose=True)
+    result = run(cmd)
+    while result.failed and '(err 29)' in result.stderr and retries < max_retries:
+        result = run(cmd)
         retries += 1
-    if retcode != 0 or retries == max_retries:
-        print(f"FAIL: Could not discover iSCSI target. Return code: {retcode}")
+    if result.failed or retries == max_retries:
+        logging.error(f'Could not discover iSCSI target. Return code: {result.rc}')
         return False
     return True
 
 
 def is_target_discovered(t_iqn):  # noqa: ANN001, ANN201
     """Check if an iSCSI target is already discovered
     The arguments are:
     iSCSI Target:   iQN of iSCSI target
     Returns:
     True:     If target is discovered
     False:    If was not found.
     """
     if not t_iqn:
-        print("FAIL: is_target_discovered() - requires target iqn as parameter")
+        logging.error('is_target_discovered() - requires target iqn as parameter')
 
     disc_dict = query_discovery()
     if not disc_dict:
         return False
 
     for disc_type in list(disc_dict.keys()):
         for disc_addr in list(disc_dict[disc_type].keys()):
-            if "targets" not in list(disc_dict[disc_type][disc_addr].keys()):
+            if 'targets' not in list(disc_dict[disc_type][disc_addr].keys()):
                 continue
-            if t_iqn in list(disc_dict[disc_type][disc_addr]["targets"].keys()):
+            if t_iqn in list(disc_dict[disc_type][disc_addr]['targets'].keys()):
                 # Target is already discovered we do not need to do anything
                 return True
     return False
 
 
 def get_disc_ifaces_of_t_iqn(t_iqn):  # noqa: ANN001, ANN201
     """From given target IQN, return the interfaces that discovered it
     The arguments are:
     iSCSI Target:   iQN of iSCSI target
     Returns:
     List ifaces:     Discovered interfaces
     None:             If iface was not found.
     """
     if not t_iqn:
-        print("FAIL: get_t_iqn_disc_ifaces() - requires target iqn")
+        logging.error('get_t_iqn_disc_ifaces() - requires target iqn')
         return None
 
     if not is_target_discovered(t_iqn):
-        print(f"FAIL: get_t_iqn_disc_ifaces() - target iqn: {t_iqn} is not discovered")
+        logging.error(f'get_t_iqn_disc_ifaces() - target iqn: {t_iqn} is not discovered')
         return None
 
     disc_dict = query_discovery()
     for disc_type in list(disc_dict.keys()):
         for disc_addr in list(disc_dict[disc_type].keys()):
-            if "targets" not in list(disc_dict[disc_type][disc_addr].keys()):
+            if 'targets' not in list(disc_dict[disc_type][disc_addr].keys()):
                 continue
-            if t_iqn in list(disc_dict[disc_type][disc_addr]["targets"].keys()) and "iface" in list(
-                disc_dict[disc_type][disc_addr]["targets"][t_iqn].keys(),
+            if t_iqn in list(disc_dict[disc_type][disc_addr]['targets'].keys()) and 'iface' in list(
+                disc_dict[disc_type][disc_addr]['targets'][t_iqn].keys(),
             ):
-                return disc_dict[disc_type][disc_addr]["targets"][t_iqn]["iface"]
+                return disc_dict[disc_type][disc_addr]['targets'][t_iqn]['iface']
     return None
 
 
-def delete_discovery_target_portal(portal, port="3260", tp="st"):  # noqa: ANN001, ANN201
+def delete_discovery_target_portal(portal, port='3260', tp='st'):  # noqa: ANN001, ANN201
     """Delete discovered iSCSI target
     The arguments are:
     portal:   Address of target to be discovered
     port:     Port of iSCSI target to be deleted
     tp:       Discovery type, sendtargets, isns...
 
     Returns:
     True:     If deleted discovered iSCSI target
     False:    If some problem happened.
     """
-    print(f"INFO: Deleting target portal: {portal}")
+    logging.info(f'Deleting target portal: {portal}')
     if net.get_ip_version(portal) == 6:
         # IF IPv6 we need to append squared brackets to the address
-        portal = "[" + portal + "]"
+        portal = '[' + portal + ']'
 
     cmd = f'iscsiadm -m discoverydb --type {tp} --portal "{portal}:{port}" -o delete'
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not delete discover iSCSI target")
+    if run(cmd).failed:
+        logging.error('Could not delete discover iSCSI target')
         return False
     return True
 
 
-def clean_up(portal="all"):  # noqa: ANN001, ANN201
+def clean_up(portal='all'):  # noqa: ANN001, ANN201
     """Remove iSCSI session and discover information for specific target
     The arguments are:
     target:   Address of target to be removed
     Returns:
     True:     If iSCSI target is removed
     False:    If some problem happened.
     """
     error = 0
     # TODO: iSCSI boot clean up
     if is_iscsi_boot():
         boot_dev = linux.get_boot_device()
         if not boot_dev:
-            print("FAIL: clean_up() - Could not determine boot device")
+            logging.error('clean_up() - Could not determine boot device')
             return False
 
         boot_wwid = linux.get_device_wwid(boot_dev)
         if not boot_wwid:
-            print(f"FAIL: clean_up() - Could not determine boot WWID for {boot_dev}")
+            logging.error(f'clean_up() - Could not determine boot WWID for {boot_dev}')
             return False
 
         ses_ids = get_all_session_ids()
         if not ses_ids:
-            print("FAIL: is_iscsi_boot() - It is iSCSI boot, but did not find any session id")
+            logging.error('is_iscsi_boot() - It is iSCSI boot, but did not find any session id')
             return False
 
-        if portal == "all":
+        if portal == 'all':
             # Logout from all iSCSI session, that do not have boot device
             for ses_id in ses_ids:
                 iscsi_wwids = scsi_wwid_of_iscsi_session(sid=ses_id)
                 if boot_wwid in iscsi_wwids:
-                    print(f"INFO: Can't log out of session {ses_id}, because it is used for iSCSI boot")
+                    logging.info(f"Can't log out of session {ses_id}, because it is used for iSCSI boot")
                 else:
-                    print(f"INFO: Logging out of session {ses_id}")
+                    logging.info(f'Logging out of session {ses_id}')
                     session_logout(ses_id)
                     # TODO Clean up discovery info
         else:
             # TODO Logout single portal from iSCSI boot
-            print(f"FAIL: clean_up() - Does not know how to clean up portal {portal} for iSCSI boot")
+            logging.error(f'clean_up() - Does not know how to clean up portal {portal} for iSCSI boot')
             return False
 
         return True
 
     # Not iSCSI boot
-    if portal == "all":
+    if portal == 'all':
         # log out of all iSCSI sessions
         if get_all_session_ids():  # noqa: SIM102
             # There is at least one session
             if not node_logout():
-                print(f"FAIL: Could not logout from {portal} iSCSI target")
+                logging.error(f'Could not logout from {portal} iSCSI target')
                 error += 1
     elif not node_logout(portal=portal):
-        print(f"FAIL: Could not logout from {portal} iSCSI target")
+        logging.error(f'Could not logout from {portal} iSCSI target')
         error += 1
 
     disc_dict = query_discovery()
     # If there is discovery information
     if disc_dict:
         # We will search for this portal on sendtargets and iSNS
         for mode in list(disc_dict.keys()):
-            if mode != "SENDTARGETS" and mode != "iSNS":
+            if mode != 'SENDTARGETS' and mode != 'iSNS':
                 # We only delete discover info for st and isns
                 continue
             m_dict = disc_dict[mode]
             # Search for all discovered address if they match the one given
             for addr in list(m_dict.keys()):
                 d_dict = m_dict[addr]
 
-                disc_addr = d_dict["disc_addr"]
-                port = d_dict["disc_port"]
-                if disc_addr == portal or portal == "all":  # noqa: SIM102
-                    if not delete_discovery_target_portal(disc_addr, port=port, tp=d_dict["mode"]):
-                        print(f"FAIL: Deleting iSCSI target {d_dict['disc_addr']}")
+                disc_addr = d_dict['disc_addr']
+                port = d_dict['disc_port']
+                if disc_addr == portal or portal == 'all':  # noqa: SIM102
+                    if not delete_discovery_target_portal(disc_addr, port=port, tp=d_dict['mode']):
+                        logging.error(f"Deleting iSCSI target {d_dict['disc_addr']}")
                         error += 1
 
     if error:
         return False
     return True
 
 
 # iSCSI session ###
 # def query_sessions():
 #    #cmd output: tcp: [21] 127.0.0.1:3260,1 iqn.2009-10.com.redhat:storage-1 (non-flash)
 #    cmd = "iscsiadm -m session"
-#    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+#    retcode, output = run_ret_out(cmd, return_output=True)
 #    if (retcode != 0):
 #        return None
 #    lines = output.split("\n")
 #    session_regex = re.compile("(\S+):\s[(\d+)]\s(\S+):(\S+),(\d+),(\S+)")
 #    sessions_dict = {}
 #    for line in lines:
 #        m = session_regex.search(line)
@@ -711,51 +712,35 @@
 #            ses_dict["portal"] = m.group(3)
 #            ses_dict["portal_port"] = m.group(4)
 #            ses_dict["target_iqn"] = m.group(6)
 #            sessions[sid] = ses_dict
 #    return sessions_dict
 
 
-def get_all_session_ids():  # noqa: ANN201
-    cmd = "iscsiadm -m session -P1"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        # print ("INFO: there is no iSCSI session")
-        return None
-    lines = output.split("\n")
-
-    session_ids = []
-
-    for line in lines:
-        m = re.match(supported_session_info["sid"], line)
-        if not m:
-            continue
-        # print "Found session id: %s" %m.group(1)
-        session_ids.append(m.group(1))
-    return session_ids
+def get_all_session_ids() -> List[Optional[str]]:
+    """Returns list of session ids."""
+    session_info = run('iscsiadm -m session -P1').stdout.splitlines()
+    return [remove_prefix(id, '\t\tSID: ') for id in session_info if 'SID' in id]
 
 
 def query_iscsi_session(sid):  # noqa: ANN001, ANN201
     """Query information from a specific iSCSI session
     The arguments are:
     sid:      Session id
     Returns:
     Dict:     A dictionary with session info
     None:     If some problem happened.
     """
     if not sid:
-        print("FAIL: query_iscsi_session() - requires sid as argument")
+        logging.error('query_iscsi_session() - requires sid as argument')
         return None
 
-    regex_session_scsi_id = "^[ \t]+scsi([0-9]+) Channel ([0-9]+) Id ([0-9])+ Lun: ([0-9]+)$"
-    cmd = f"iscsiadm -m session -P3 -S -r {sid}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        return None
-    lines = output.split("\n")
+    regex_session_scsi_id = '^[ \t]+scsi([0-9]+) Channel ([0-9]+) Id ([0-9])+ Lun: ([0-9]+)$'
+
+    lines = run(f'iscsiadm -m session -P3 -S -r {sid}').stdout.splitlines()
 
     session_info_dict = {}
     # dict with disk name and its status
     session_disks_dict = {}
     # store host number and status
     session_host_dict = {}
     for line in lines:
@@ -763,53 +748,53 @@
 
         m = re.match(regex_session_scsi_id, line)
         if m:
             host_id = m.group(1)
             target_id_only = m.group(2)
             bus_id_only = m.group(3)
             lun_id = m.group(4)
-            target_id_only = re.sub("^0+(?=.)", "", target_id_only)
-            scsi_id = f"{host_id}:{target_id_only}:{bus_id_only}:{lun_id}"
+            target_id_only = re.sub('^0+(?=.)', '', target_id_only)
+            scsi_id = f'{host_id}:{target_id_only}:{bus_id_only}:{lun_id}'
 
-            if "scsi_id_info" not in list(session_info_dict.keys()):
-                session_info_dict["scsi_id_info"] = {}
-            session_info_dict["scsi_id_info"][scsi_id] = {}
-            session_info_dict["scsi_id_info"][scsi_id]["scsi_id"] = scsi_id
+            if 'scsi_id_info' not in list(session_info_dict.keys()):
+                session_info_dict['scsi_id_info'] = {}
+            session_info_dict['scsi_id_info'][scsi_id] = {}
+            session_info_dict['scsi_id_info'][scsi_id]['scsi_id'] = scsi_id
 
         # Could be more than one scsi disk, will add as dict
-        m = re.match(supported_session_info["disks"], line)
+        m = re.match(supported_session_info['disks'], line)
         if m:
-            disk_dict = {"status": m.group(2), "wwid": scsi.wwid_of_disk(m.group(1))}
+            disk_dict = {'status': m.group(2), 'wwid': scsi.wwid_of_disk(m.group(1))}
             # disk_dict["scsi_name"] = m.group(1)
             session_disks_dict[m.group(1)] = disk_dict
             continue
 
         # Could be more than one scsi disk, will add as dict
-        m = re.match(supported_session_info["host"], line)
+        m = re.match(supported_session_info['host'], line)
         if m:
             session_host_dict[m.group(1)] = m.group(2)
             continue
         # Generic search for keys and values
         for key in list(supported_session_info.keys()):
             m = re.match(supported_session_info[key], line)
             if not m:
                 continue
             # print "Found %s: %s" % (key, m.group(1))
             session_info_dict[key] = m.group(1)
-            if session_info_dict[key] == "<empty>":
+            if session_info_dict[key] == '<empty>':
                 session_info_dict[key] = None
-                if key == "mac":  # noqa: SIM102
+                if key == 'mac':  # noqa: SIM102
                     # Try to get based on iface IP address
-                    if "iface_ip" in list(session_info_dict.keys()):
-                        nic = net.get_nic_of_ip(session_info_dict["iface_ip"])
+                    if 'iface_ip' in list(session_info_dict.keys()):
+                        nic = net.get_nic_of_ip(session_info_dict['iface_ip'])
                         if nic:
                             session_info_dict[key] = net.get_mac_of_nic(nic)
     # added info for the specific session
-    session_info_dict["disks"] = session_disks_dict
-    session_info_dict["host"] = session_host_dict
+    session_info_dict['disks'] = session_disks_dict
+    session_info_dict['host'] = session_host_dict
     return session_info_dict
 
 
 def query_all_iscsi_sessions() -> Union[dict, None]:
     """First we get all iSCSI ids, later on we get the information of each session individually."""
     session_ids = get_all_session_ids()
     if not session_ids:
@@ -822,35 +807,31 @@
         iscsi_sessions[sid] = session_info_dict
 
     # print iscsi_sessions
     return iscsi_sessions
 
 
 def session_logout(sid=None):  # noqa: ANN001, ANN201
-    cmd = "iscsiadm -m session -u"
+    run('iscsiadm -m session -u')
+    cmd = 'iscsiadm -m session -u'
     if sid:
-        cmd += f" -r {sid}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        print(output)
-        print("FAIL: session_logout() - Could not logout from session")
-        return None
-    return True
+        cmd += f' -r {sid}'
+    run('iscsiadm -m session -u')
 
 
 def get_iscsi_session_by_scsi_id(scsi_id):  # noqa: ANN001, ANN201
     """Return the Session Dict that has the scsi_id."""
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     for ses in sessions:
-        if "scsi_id_info" not in list(sessions[ses].keys()):
+        if 'scsi_id_info' not in list(sessions[ses].keys()):
             continue
-        if scsi_id in list(sessions[ses]["scsi_id_info"].keys()):
+        if scsi_id in list(sessions[ses]['scsi_id_info'].keys()):
             return sessions[ses]
     return None
 
 
 def h_iqn_of_sessions():  # noqa: ANN201
     """Usage
         h_iqn_of_sessions()
@@ -866,19 +847,19 @@
     h_iqns = None
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     for key in list(sessions.keys()):
         info = sessions[key]
-        if "h_iqn" in list(info.keys()):
+        if 'h_iqn' in list(info.keys()):
             if not h_iqns:
                 h_iqns = []
-            if info["h_iqn"] not in h_iqns:
-                h_iqns.append(info["h_iqn"])
+            if info['h_iqn'] not in h_iqns:
+                h_iqns.append(info['h_iqn'])
     return h_iqns
 
 
 def t_iqn_of_sessions():  # noqa: ANN201
     """Usage
         t_iqn_of_sessions()
     Purpose
@@ -893,19 +874,19 @@
     t_iqns = None
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     for key in list(sessions.keys()):
         info = sessions[key]
-        if "t_iqn" in list(info.keys()):
+        if 't_iqn' in list(info.keys()):
             if not t_iqns:
                 t_iqns = []
-            if info["t_iqn"] not in t_iqns:
-                t_iqns.append(info["t_iqn"])
+            if info['t_iqn'] not in t_iqns:
+                t_iqns.append(info['t_iqn'])
     return t_iqns
 
 
 def mac_of_iscsi_session():  # noqa: ANN201
     """Usage
         mac_of_iscsi_session()
     Purpose
@@ -920,19 +901,19 @@
     macs = None
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     for key in list(sessions.keys()):
         info = sessions[key]
-        if "mac" in list(info.keys()):
+        if 'mac' in list(info.keys()):
             if not macs:
                 macs = []
-            if info["mac"] != "<empty>" and info["mac"] and info["mac"] not in macs:
-                macs.append(info["mac"])
+            if info['mac'] != '<empty>' and info['mac'] and info['mac'] not in macs:
+                macs.append(info['mac'])
     return macs
 
 
 def scsi_names_of_iscsi_session(h_iqn=None, t_iqn=None, sid=None):  # noqa: ANN001, ANN201
     """Usage
         scsi_names_of_iscsi_session();
         scsi_names_of_iscsi_session(sid=1);
@@ -954,38 +935,38 @@
         None.
     """
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     if sid:
-        if sid in list(sessions.keys()) and "disks" in list(sessions[sid].keys()):
-            return list(sessions[sid]["disks"].keys())
+        if sid in list(sessions.keys()) and 'disks' in list(sessions[sid].keys()):
+            return list(sessions[sid]['disks'].keys())
         return None
 
     scsi_names = None
     if not h_iqn and not t_iqn:
         for sid in list(sessions.keys()):
-            if "disks" in list(sessions[sid].keys()):
+            if 'disks' in list(sessions[sid].keys()):
                 if not scsi_names:
                     scsi_names = []
-                scsi_names.extend(list(sessions[sid]["disks"].keys()))
+                scsi_names.extend(list(sessions[sid]['disks'].keys()))
         return scsi_names
 
     if h_iqn and t_iqn:
         for sid in list(sessions.keys()):
-            if (sessions[sid]["h_iqn"] == h_iqn and sessions[sid]["t_iqn"] == t_iqn) and "disks" in list(
+            if (sessions[sid]['h_iqn'] == h_iqn and sessions[sid]['t_iqn'] == t_iqn) and 'disks' in list(
                 sessions[sid].keys(),
             ):
                 if not scsi_names:
                     scsi_names = []
-                scsi_names.extend(list(sessions[sid]["disks"].keys()))
+                scsi_names.extend(list(sessions[sid]['disks'].keys()))
         return scsi_names
 
-    print("FAIL: scsi_names_of_iscsi_session() - Unsupported parameters given")
+    logging.error('scsi_names_of_iscsi_session() - Unsupported parameters given')
     return None
 
 
 def scsi_wwid_of_iscsi_session(h_iqn=None, t_iqn=None, sid=None):  # noqa: ANN001, ANN201
     """Usage
         scsi_wwid_of_iscsi_session();
         scsi_wwid_of_iscsi_session(sid=1);
@@ -1008,68 +989,68 @@
     """
     wwids = None
     if sid:
         sid = str(sid)
         session_info = query_iscsi_session(sid)
         if not session_info:
             return None
-        if "disks" in list(session_info.keys()):
+        if 'disks' in list(session_info.keys()):
             if not wwids:
                 wwids = []
-            for scsi_name in list(session_info["disks"].keys()):
-                wwid = session_info["disks"][scsi_name]["wwid"]
+            for scsi_name in list(session_info['disks'].keys()):
+                wwid = session_info['disks'][scsi_name]['wwid']
                 if wwid and wwid not in wwids:
                     wwids.append(wwid)
             return wwids
         return None
 
     sessions = query_all_iscsi_sessions()
     if not sessions:
         return None
 
     if not h_iqn and not t_iqn:
         for sid in list(sessions.keys()):
-            if "disks" in list(sessions[sid].keys()):
+            if 'disks' in list(sessions[sid].keys()):
                 if not wwids:
                     wwids = []
-                for scsi_name in list(sessions[sid]["disks"].keys()):
+                for scsi_name in list(sessions[sid]['disks'].keys()):
                     wwid = scsi.wwid_of_disk(scsi_name)
                     if wwid and wwid not in wwids:
                         wwids.append(wwid)
         return wwids
 
     if h_iqn and t_iqn:
         for sid in list(sessions.keys()):
-            if (sessions[sid]["h_iqn"] == h_iqn and sessions[sid]["t_iqn"] == t_iqn) and "disks" in list(
+            if (sessions[sid]['h_iqn'] == h_iqn and sessions[sid]['t_iqn'] == t_iqn) and 'disks' in list(
                 sessions[sid].keys(),
             ):
                 if not wwids:
                     wwids = []
-                for scsi_name in list(sessions[sid]["disks"].keys()):
+                for scsi_name in list(sessions[sid]['disks'].keys()):
                     wwid = scsi.wwid_of_disk(scsi_name)
                     if wwid and wwid not in wwids:
                         wwids.append(wwid)
         return wwids
 
-    print("FAIL: scsi_wwid_of_iscsi_session() - Unsupported parameters given")
+    logging.error('scsi_wwid_of_iscsi_session() - Unsupported parameters given')
     return None
 
 
 def is_iscsi_boot():  # noqa: ANN201
     iscsi_wwids = scsi_wwid_of_iscsi_session()
     if not iscsi_wwids:
         return False
     boot_dev = linux.get_boot_device()
     if not boot_dev:
-        print("FAIL: is_iscsi_boot() - Could not determine boot device")
+        logging.error('is_iscsi_boot() - Could not determine boot device')
         return False
 
     boot_wwid = linux.get_device_wwid(boot_dev)
     if not boot_wwid:
-        print(f"WARN: is_iscsi_boot() - Could not determine boot WWID for {boot_dev}")
+        logging.warning(f'is_iscsi_boot() - Could not determine boot WWID for {boot_dev}')
         return False
 
     if boot_wwid in iscsi_wwids:
         return True
 
     return False
 
@@ -1081,30 +1062,29 @@
     arget:    iSCSI targets to be used, separated by space (optional)
     options:   extra parameters. eg: "-T <target> -p <portal>"
     Returns:
     True:     If iSCSI node is logged in
     False:    If some problem happened.
     """
     # Going to delete discovered target information
-    print("INFO: Performing iSCSI login")
-    cmd = "iscsiadm -m node -l"
+    logging.info('Performing iSCSI login')
+    cmd = 'iscsiadm -m node -l'
     if options:
-        cmd += f" {options}"
+        cmd += f' {options}'
 
     if target:
         for target_iqn in target.split():
-            cmd += f" -T {target_iqn}"
+            cmd += f' -T {target_iqn}'
 
     if portal:
-        cmd += f" -p {portal}"
+        cmd += f' -p {portal}'
 
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
-    if retcode != 0:
-        print("FAIL: Could not login to iSCSI target")
-        print(output)
+    result = run(cmd)
+    if result.failed:
+        logging.error('Could not login to iSCSI target')
         return False
 
     linux.wait_udev(udev_wait_time)
     return True
 
 
 def node_logout(options=None, target=None, portal=None):  # noqa: ANN001, ANN201
@@ -1115,45 +1095,44 @@
     True:     If iSCSI node is removed
     False:    If some problem happened.
     """
     ses_dict = query_all_iscsi_sessions()
     if not ses_dict:
         # There is no session to logout just skip
         return True
-    print("INFO: Performing iSCSI logout")
-    cmd = "iscsiadm -m node -u"
+    logging.info('Performing iSCSI logout')
+    cmd = 'iscsiadm -m node -u'
     if options:
-        cmd += f" {options}"
+        cmd += f' {options}'
 
     if target:
-        cmd += f" -T {target}"
+        cmd += f' -T {target}'
 
     if portal:
-        cmd += f" -p {portal}"
+        cmd += f' -p {portal}'
 
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
-    if retcode != 0:
-        print("FAIL: Could not logout from iSCSI target")
-        print(output)
+    result = run(cmd)
+    if result.failed:
+        logging.error('Could not logout to iSCSI target')
         return False
     return True
 
 
 def node_delete(options=None):  # noqa: ANN001, ANN201
     """Delete node information."""
     if not options:
-        print("FAIL: node_delete() - requires portal and/or target parameters")
+        logging.error('node_delete() - requires portal and/or target parameters')
         return False
 
-    cmd = "iscsiadm -m node -o delete"
+    cmd = 'iscsiadm -m node -o delete'
     if options:
-        cmd += f" {options}"
+        cmd += f' {options}'
 
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not delete node iSCSI target")
+    if run(cmd).failed:
+        logging.error('Could not login to iSCSI target')
         return False
     return True
 
 
 # iSCSI iface ###
 def iface_query_all_info(iface_name=None):  # noqa: ANN001, ANN201
     """Return a dict with interface names as key with detailed information of
@@ -1161,31 +1140,31 @@
     """
     ifaces = [iface_name] if iface_name else get_iscsi_iface_names()
 
     if not ifaces:
         return None
 
     all_iface_dict = {}
-    iface_info_regex = re.compile(r"iface\.(\S+) = (\S+)")
+    iface_info_regex = re.compile(r'iface\.(\S+) = (\S+)')
 
     for iface in ifaces:
-        cmd = f"iscsiadm -m iface -I {iface}"
-        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-        if retcode != 0:
-            print("FAIL: Could not delete node iSCSI target")
+        cmd = f'iscsiadm -m iface -I {iface}'
+        result = run(cmd)
+        if result.failed:
+            logging.warning('Could not login to iSCSI target')
             continue
-        details = output.split("\n")
+        details = result.stdout.splitlines()
         for info in details:
             m = iface_info_regex.match(info)
             if not m:
                 continue
             if iface not in list(all_iface_dict.keys()):
                 all_iface_dict[iface] = {}
             value = m.group(2)
-            if value == "<empty>":
+            if value == '<empty>':
                 value = None
             all_iface_dict[iface][m.group(1)] = value
 
     if iface_name:
         if iface_name not in list(all_iface_dict.keys()):
             return None
         return all_iface_dict[iface_name]
@@ -1201,174 +1180,166 @@
     value  # Value to set (-v $).
 
     Returns:
     True:     If value is set successfully
     False:    If some problem happened.
     """
     if not iface or not name or not value:
-        print("FAIL: iface_update() - required parameters: iface, name, value")
+        logging.error('iface_update() - required parameters: iface, name, value')
         return False
 
-    cmd = f"iscsiadm -m iface -I {iface} -o update -n iface.{name} -v {value}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        print(f"FAIL: Could not set {name} to {value} on iface {iface}")
-        print(output)
+    cmd = f'iscsiadm -m iface -I {iface} -o update -n iface.{name} -v {value}'
+    result = run(cmd)
+    if result.failed:
+        logging.error('Could not login to iSCSI target')
         return False
 
     return True
 
 
 def set_initiatorname(iqn: str) -> bool:
-    initiatorname_file = "/etc/iscsi/initiatorname.iscsi"
-    str_to_write = f"InitiatorName={iqn}"
+    initiatorname_file = '/etc/iscsi/initiatorname.iscsi'
+    str_to_write = f'InitiatorName={iqn}'
     try:
         path = Path(initiatorname_file)
         if not path.is_file():
             linux.service_start(ISCSID_SERVICE_NAME)
         existing_name = path.read_text()
         if str_to_write != existing_name:
-            with path.open(mode="w") as i:
-                print(f"INFO: Writing {iqn} to {initiatorname_file}")
+            with path.open(mode='w') as i:
+                logging.info(f'Writing {iqn} to {initiatorname_file}')
                 i.write(str_to_write)
-                linux.service_restart(ISCSID_SERVICE_NAME, verbose=True)
-    except Exception as e:
-        print(f"FAIL: Could not set iqn in {initiatorname_file}. Exception: {e}")
+                linux.service_restart(ISCSID_SERVICE_NAME)
+    except Exception:
+        logging.exception(f'Could not set iqn in {initiatorname_file}')
         return False
     return True
 
 
-def iface_set_iqn(iqn, iface="default"):  # noqa: ANN001, ANN201
+def iface_set_iqn(iqn, iface='default'):  # noqa: ANN001, ANN201
     """Set IQN in /etc/iscsi/initiatorname or for specific iface
     Return:
         True
         of
         False.
     """
     if not iqn:
-        print("FAIL: iface_set_iqn() - requires iqn to be set")
+        logging.error('iface_set_iqn() - requires iqn to be set')
         return False
 
-    if iface == "default":
+    if iface == 'default':
         set_initiatorname(iqn=iqn)
         return True
 
     iscsiadm = IscsiAdm()
-    if not iscsiadm.iface_update(iface, name="initiatorname", value=iqn):
+    if not iscsiadm.iface_update(iface, name='initiatorname', value=iqn):
         return False
 
     return True
 
 
 def iface_set_ip(iface, ip, mask=None, gw=None):  # noqa: ANN001, ANN201
     """Set IP information for specific iface
     Return:
         True
         of
         False.
     """
     if not iface or not ip:
-        print("FAIL: iface_set_ip() - requires iface and ip parameters")
+        logging.error('iface_set_ip() - requires iface and ip parameters')
         return False
 
-    if not iface_update(iface, "ipaddress", ip):
+    if not iface_update(iface, 'ipaddress', ip):
         return False
 
-    if mask and not iface_update(iface, "subnet_mask", mask):
+    if mask and not iface_update(iface, 'subnet_mask', mask):
         return False
 
-    if gw and not iface_update(iface, "gateway", gw):
+    if gw and not iface_update(iface, 'gateway', gw):
         return False
 
     return True
 
 
-def get_iscsi_iface_names():  # noqa: ANN201
+def get_iscsi_iface_names() -> List[str]:
     """Return a list with the name of all iSCSI interfaces on the host."""
-    cmd = 'iscsiadm -m iface | cut -d " " -f 1'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        print("FAIL: Could not read iSCSI interfaces")
-        print(output)
-        return None
-    ifaces = output.split("\n")
-    ifaces[:] = (value for value in ifaces if "iSCSI ERROR" not in value)  # bz1997710
-    return ifaces
+    ifaces = run('iscsiadm -m iface').stdout.splitlines()
+    return [i.split(' ')[0] for i in ifaces if 'iSCSI ERROR' not in i]  # bz1997710
 
 
 def set_iscsid_parameter(parameters: dict) -> bool:
     """Change parameter in iscsid.conf file and restarts iscsid service
     Use dictionary with parameter:value as argument.
     """
-    filename = "/etc/iscsi/iscsid.conf"
+    filename = '/etc/iscsi/iscsid.conf'
     if not linux.edit_config(filename, parameters, list_values=False):
-        print(f"FAIL: Unable to set iscsi parameters: {parameters}")
+        logging.error(f'Unable to set iscsi parameters: {parameters}')
         return False
 
     if not linux.service_restart(ISCSID_SERVICE_NAME):
-        print("FAIL: Unable to restart iscsid service")
+        logging.error('Unable to restart iscsid service')
         return False
 
     return True
 
 
 def set_chap(target_user, target_pass, initiator_user=None, initiator_pass=None):  # noqa: ANN001, ANN201
     """Set CHAP authentication."""
     if not target_user or not target_pass:
-        print("FAIL: set_chap() - requires username and password")
+        logging.error('set_chap() - requires username and password')
         return False
 
     parameters = {
-        "node.session.auth.authmethod": "CHAP",
-        "node.session.auth.username": target_user,
-        "node.session.auth.password": target_pass,
-        "discovery.sendtargets.auth.authmethod": "CHAP",  # NetApp array requires discovery authentication
-        "discovery.sendtargets.auth.username": target_user,
-        "discovery.sendtargets.auth.password": target_pass,
+        'node.session.auth.authmethod': 'CHAP',
+        'node.session.auth.username': target_user,
+        'node.session.auth.password': target_pass,
+        'discovery.sendtargets.auth.authmethod': 'CHAP',  # NetApp array requires discovery authentication
+        'discovery.sendtargets.auth.username': target_user,
+        'discovery.sendtargets.auth.password': target_pass,
     }
 
     if initiator_user and initiator_pass:
-        print("INFO: Setting mutual two-way CHAP authentication")
-        parameters["node.session.auth.username_in"] = initiator_user
-        parameters["node.session.auth.password_in"] = initiator_pass
-        parameters["discovery.sendtargets.auth.username_in"] = initiator_user
-        parameters["discovery.sendtargets.auth.password_in"] = initiator_pass
+        logging.info('Setting mutual two-way CHAP authentication')
+        parameters['node.session.auth.username_in'] = initiator_user
+        parameters['node.session.auth.password_in'] = initiator_pass
+        parameters['discovery.sendtargets.auth.username_in'] = initiator_user
+        parameters['discovery.sendtargets.auth.password_in'] = initiator_pass
 
     if not set_iscsid_parameter(parameters):
-        print("FAIL: Unable to set CHAP authentication")
+        logging.error('Unable to set CHAP authentication')
         return False
 
-    if not linux.service_restart("iscsid"):
-        print("FAIL: Unable to restart iscsid service")
+    if not linux.service_restart('iscsid'):
+        logging.error('Unable to restart iscsid service')
         return False
 
-    print("INFO: CHAP authentication enabled")
+    logging.info('CHAP authentication enabled')
     return True
 
 
 def disable_chap():  # noqa: ANN201
     """Disable CHAP authentication in iscsid.conf and restarts the service."""
     # Removing all previously set auth parameters.
     parameters = [
-        "node.session.auth.authmethod",
-        "node.session.auth.username",
-        "node.session.auth.password",
-        "discovery.sendtargets.auth.authmethod",
-        "discovery.sendtargets.auth.username",
-        "discovery.sendtargets.auth.password",
-        "node.session.auth.username_in",
-        "node.session.auth.password_in",
-        "discovery.sendtargets.auth.username_in",
-        "discovery.sendtargets.auth.password_in",
+        'node.session.auth.authmethod',
+        'node.session.auth.username',
+        'node.session.auth.password',
+        'discovery.sendtargets.auth.authmethod',
+        'discovery.sendtargets.auth.username',
+        'discovery.sendtargets.auth.password',
+        'node.session.auth.username_in',
+        'node.session.auth.password_in',
+        'discovery.sendtargets.auth.username_in',
+        'discovery.sendtargets.auth.password_in',
     ]
 
-    linux.remove_from_config("/etc/iscsi/iscsid.conf", parameters, warn=False)
+    linux.remove_from_config('/etc/iscsi/iscsid.conf', parameters, warn=False)
 
-    if not linux.service_restart("iscsid"):
-        print("FAIL: Unable to restart iscsid service")
+    if not linux.service_restart('iscsid'):
+        logging.error('Unable to restart iscsid service')
         return False
 
     return True
 
 
 def multipath_timeo(seconds=None):  # noqa: ANN001, ANN201
     """If multipath is used for iSCSI session, session replacement
@@ -1377,103 +1348,101 @@
     multipathd service should be running when calling this
     The arguments are:
     Seconds - default 10 or number of seconds
     Returns:
     True: Successfully modified iscsid config file.
     False: There was some problem.
     """
-    param = "node.session.timeo.replacement_timeout"
+    param = 'node.session.timeo.replacement_timeout'
 
     if not seconds:
         seconds = 10
     seconds = str(seconds)
 
     if mp.is_multipathd_running():
-        print("INFO: multipathd is running")
+        logging.info('multipathd is running')
     else:
-        print("FAIL: multipathd is not running")
+        logging.error('multipathd is not running')
         return False
 
     if not set_iscsid_parameter({param: seconds}):
         return False
 
     return True
 
 
 def create_iscsi_iface(iface_name: str, mac: Optional[str] = None) -> bool:
     """Create a new iSCSI interface, assign mac if specified."""
     if not iface_name:
-        print("FAIL: create_iscsi_iface() - requires iface name as parameter")
+        logging.error('create_iscsi_iface() - requires iface name as parameter')
         return False
 
     if iface_name in get_iscsi_iface_names():
-        print(f"INFO: iSCSI interface {iface_name} already exists")
+        logging.info(f'iSCSI interface {iface_name} already exists')
         return True
-    iscsiadm = IscsiAdm(verbose=True)
-    retcode, output = iscsiadm.iface(op="new", iface=iface_name)
+    iscsiadm = IscsiAdm()
+    retcode, output = iscsiadm.iface(op='new', iface=iface_name)
     if retcode != 0:
-        print("FAIL: Could not create iSCSI interface")
+        logging.error('Could not create iSCSI interface')
         print(output)
         return False
 
-    if mac is not None and not iscsiadm.iface_update(iface=iface_name, name="iface.hwaddress", value=mac):
+    if mac is not None and not iscsiadm.iface_update(iface=iface_name, name='iface.hwaddress', value=mac):
         return False
 
     return True
 
 
 def clone_iscsi_iface(new_iface_name, base_iface):  # noqa: ANN001, ANN201
-    print(f"Cloning iface: {base_iface} to {new_iface_name}")
+    print(f'Cloning iface: {base_iface} to {new_iface_name}')
     if not create_iscsi_iface(new_iface_name):
         return False
 
     iface_info = iface_query_all_info(base_iface)
     if iface_info is None:
-        print(f"FAIL: Could not query all info about iface: {base_iface}")
+        logging.error(f'Could not query all info about iface: {base_iface}')
         return False
 
-    if iface_info["hwaddress"] is not None and not iface_update(new_iface_name, "hwaddress", iface_info["hwaddress"]):
+    if iface_info['hwaddress'] is not None and not iface_update(new_iface_name, 'hwaddress', iface_info['hwaddress']):
         return False
 
-    if iface_info["transport_name"] is not None:  # noqa: SIM102
-        if not iface_update(new_iface_name, "transport_name", iface_info["transport_name"]):
+    if iface_info['transport_name'] is not None:  # noqa: SIM102
+        if not iface_update(new_iface_name, 'transport_name', iface_info['transport_name']):
             return False
 
-    if iface_info["initiatorname"] is not None:  # noqa: SIM102
-        if not iface_update(new_iface_name, "initiatorname", iface_info["initiatorname"]):
+    if iface_info['initiatorname'] is not None:  # noqa: SIM102
+        if not iface_update(new_iface_name, 'initiatorname', iface_info['initiatorname']):
             return False
 
-    if iface_info["ipaddress"] is not None and not iface_update(new_iface_name, "ipaddress", iface_info["ipaddress"]):
+    if iface_info['ipaddress'] is not None and not iface_update(new_iface_name, 'ipaddress', iface_info['ipaddress']):
         return False
 
-    print(f"successfully cloned {base_iface}. new iface: {new_iface_name}")
+    print(f'successfully cloned {base_iface}. new iface: {new_iface_name}')
     return True
 
 
 def remove_iscsi_iface(iface_name):  # noqa: ANN001, ANN201
     if iface_name not in get_iscsi_iface_names():
-        print(f"INFO: iSCSI interface '{iface_name}' does not exist")
+        logging.info(f"iSCSI interface '{iface_name}' does not exist")
         return False
 
-    cmd = f"iscsiadm -m iface -o delete -I {iface_name}"
-    if run(cmd, verbose=False).returncode != 0:
-        print("FAIL: Could not remove iSCSI interface")
+    cmd = f'iscsiadm -m iface -o delete -I {iface_name}'
+    if run(cmd).failed:
+        logging.error('Could not remove iSCSI interface')
         return False
 
     return True
 
 
 def node_iface_info(iface_name):  # noqa: ANN001, ANN201
-    cmd = f"iscsiadm -m node -I {iface_name}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-    if retcode != 0:
-        print("FAIL: Could not get iface info!")
-        print(output)
+    cmd = f'iscsiadm -m node -I {iface_name}'
+    result = run(cmd)
+    if result.failed:
+        logging.error('Could not get iface info!')
         return False
-
     return True
 
 
 # iSCSI disks ###
 
 
 def get_all_iscsi_disks():  # noqa: ANN201
@@ -1482,29 +1451,29 @@
     if not sessions:
         # there is no iSCSI session
         return None
 
     # search for disks in each session
     for sid in list(sessions.keys()):
         ses = sessions[sid]
-        if ses["disks"]:
+        if ses['disks']:
             # disk names are key values
-            disks.extend(list(ses["disks"].keys()))
+            disks.extend(list(ses['disks'].keys()))
 
     return disks
 
 
 def get_session_id_from_disk(disk_name: str):  # noqa: ANN201
     sids = query_all_iscsi_sessions()
     fail_msg = f"FAIL: Could not find disk '{disk_name}' in iscsi sessions."
     if not sids:
         print(fail_msg)
         return None
     for sid in sids:
         session = query_iscsi_session(sid)
         if not session:
-            print(f"FAIL: Could not query iscsi session sid: '{sid}'.")
+            logging.error(f"Could not query iscsi session sid: '{sid}'.")
             continue
-        if disk_name in session["disks"]:
-            return session["sid"]
+        if disk_name in session['disks']:
+            return session['sid']
     print(fail_msg)
     return None
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/linux.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/linux.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,448 +1,422 @@
 """py: Module to get information from servers."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import errno
+import logging
 import os.path
-import re  # regex
+import re
 import signal
 import subprocess
 import sys
 import time
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, List, Literal, Optional, Tuple, Union
 
 from configobj import ConfigObj
-from pkg_resources import parse_version
 
 from sts import mp, scsi
 from sts.utils.cmdline import exists, run, run_ret_out
 
 
 def hostname():  # noqa: ANN201
-    ret, host = run_ret_out("hostname", verbose=False, return_output=True)
+    ret, host = run_ret_out('hostname', return_output=True)
     if ret != 0:
-        print("FAIL: hostname() - could not run command")
+        logging.error('hostname() - could not run command')
         print(host)
         return None
     return host
 
 
 def linux_distribution():  # noqa: ANN201
     # Not using platform module, as it doesn't provide needed information
     # on recent python3 versions
     # see: https://bugzilla.redhat.com/show_bug.cgi?id=1920385
     # see: https://bugs.python.org/issue28167
     data = {}
-    with Path("/etc/os-release").open(encoding="UTF-8") as f:
+    with Path('/etc/os-release').open(encoding='UTF-8') as f:
         for line in f:
             line = line.strip()  # noqa: PLW2901
-            if line == "":
+            if line == '':
                 continue
-            k, v = line.split("=")
+            k, v = line.split('=')
             data[k] = v.strip('"')
-    return [data["ID"], data["VERSION_ID"]]
+    return [data['ID'], data['VERSION_ID']]
 
 
 def dist_release():  # noqa: ANN201
     """Find out the release number of distribution."""
     # We are base on output of lsb_release -r -s, which is shipped by redhat-lsb rpm.
-    # ret, release = run_ret_out("lsb_release --release --short", verbose=False, return_output=True)
+    # ret, release = run_ret_out("lsb_release --release --short", return_output=True)
     # if ret == 0:
     #    return release
     dist = linux_distribution()
     if not dist:
-        print("FAIL: Could not determine dist release!")
+        logging.error('Could not determine dist release!')
         return None
     return dist[1]
 
 
 def dist_ver():  # noqa: ANN201
     """Check the distribution version."""
     release = dist_release()
     if not release:
         return None
-    m = re.match(r"(\d+).\d+", release)
+    m = re.match(r'(\d+).\d+', release)
     if m:
         return int(m.group(1))
 
     # See if it is only digits, in that case return it
-    m = re.match(r"(\d+)", release)
+    m = re.match(r'(\d+)', release)
     if m:
         return int(m.group(1))
 
-    print(f"FAIL: dist_ver() - Invalid release output {release}")
+    logging.error(f'dist_ver() - Invalid release output {release}')
     return None
 
 
 def dist_ver_minor():  # noqa: ANN201
     """Check the distribution minor version.
     For example: RHEL-7.4 returns 4.
     """
     release = dist_release()
     if not release:
         return None
-    m = re.match(r"\d+.(\d+)", release)
+    m = re.match(r'\d+.(\d+)', release)
     if m:
         return int(m.group(1))
 
-    print(f"FAIL: dist_ver_minor() - Release does not seem to have minor version: {release}")
+    logging.error(f'dist_ver_minor() - Release does not seem to have minor version: {release}')
     return None
 
 
 def dist_name():  # noqa: ANN201
     """Find out the name of distribution."""
     # We are base on output of lsb_release -r -s, which is shipped by redhat-lsb rpm.
-    # ret, release = run_ret_out("lsb_release --release --short", verbose=False, return_output=True)
+    # ret, release = run_ret_out("lsb_release --release --short", return_output=True)
     # if ret == 0:
     #    return release
     dist = linux_distribution()
     if not dist:
-        print("FAIL: dist_name() - Could not determine dist name")
+        logging.error('dist_name() - Could not determine dist name')
         return None
 
-    if dist[0] == "rhel":
-        return "RHEL"
+    if dist[0] == 'rhel':
+        return 'RHEL'
 
     return dist[0]
 
 
 def service_start(service_name):  # noqa: ANN001, ANN201
     """Start service
     The arguments are:
     None
     Returns:
     True: Service started
     False: There was some problem.
     """
-    cmd = f"systemctl start {service_name}"
+    cmd = f'systemctl start {service_name}'
     has_systemctl = True
 
-    if not exists("systemctl"):
+    if not exists('systemctl'):
         has_systemctl = False
     if not has_systemctl:
-        cmd = f"service {service_name} start"
+        cmd = f'service {service_name} start'
 
-    if run(cmd).returncode != 0:
-        print(f"FAIL: Could not start {service_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not start {service_name}')
         if has_systemctl:
-            run(f"systemctl status {service_name}")
-            run("journalctl -xn")
+            run(f'systemctl status {service_name}')
+            run('journalctl -xn')
         return False
     return True
 
 
 def service_stop(service_name):  # noqa: ANN001, ANN201
     """Stop service
     The arguments are:
     Name of the service
     Returns:
     True: Service stopped
     False: There was some problem.
     """
-    cmd = f"systemctl stop {service_name}"
+    cmd = f'systemctl stop {service_name}'
     has_systemctl = True
 
-    if not exists("systemctl"):
+    if not exists('systemctl'):
         has_systemctl = False
     if not has_systemctl:
-        cmd = f"service {service_name} stop"
+        cmd = f'service {service_name} stop'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not stop {service_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not stop {service_name}')
         if has_systemctl:
-            run(f"systemctl status {service_name}")
-            run("journalctl -xn")
+            run(f'systemctl status {service_name}')
+            run('journalctl -xn')
         return False
     return True
 
 
-def service_restart(service_name, verbose=True):  # noqa: ANN001, ANN201
+def service_restart(service_name):  # noqa: ANN001, ANN201
     """Restart service
     The arguments are:
     Name of the service
     Returns:
     True: Service restarted
     False: There was some problem.
     """
-    cmd = f"systemctl restart {service_name}"
+    cmd = f'systemctl restart {service_name}'
     has_systemctl = True
 
-    if not exists("systemctl"):
+    if not exists('systemctl'):
         has_systemctl = False
     if not has_systemctl:
-        cmd = f"service {service_name} restart"
+        cmd = f'service {service_name} restart'
     service_timestamp = get_service_timestamp(service_name)
     if service_timestamp is not None:
-        timestamp_struct = time.strptime(service_timestamp, "%a %Y-%m-%d %H:%M:%S %Z")
+        timestamp_struct = time.strptime(service_timestamp, '%a %Y-%m-%d %H:%M:%S %Z')
         actual_time = time.localtime()
         if time.mktime(actual_time) - time.mktime(timestamp_struct) < 5:
-            print("Waiting 5 seconds before restart.")
+            print('Waiting 5 seconds before restart.')
             time.sleep(5)
-    if run(cmd, capture_output=False, verbose=verbose).returncode != 0:
-        print(f"FAIL: Could not restart {service_name}")
+    if run(cmd).failed:
+        logging.error(f'Could not restart {service_name}')
         if has_systemctl:
-            run(f"systemctl status {service_name}")
-            run("journalctl -xn")
+            run(f'systemctl status {service_name}')
+            run('journalctl -xn')
         return False
     return True
 
 
 def systemctl_is_enabled(unit: str) -> bool:
-    if run(f"systemctl is-enabled {unit}", verbose=False).returncode != 0:
+    if run(f'systemctl is-enabled {unit}').rc != 0:
         return False
     return True
 
 
 def is_service_enabled(service_name: str) -> bool:
-    return systemctl_is_enabled(f"{service_name}.service")
+    return systemctl_is_enabled(f'{service_name}.service')
 
 
 def service_enable(service_name, now=False):  # noqa: ANN001, ANN201
     """Enable service
     The arguments are:
     Name of the service
     Returns:
     True: Service got enabled
     False: There was some problem.
     """
-    cmd = f"systemctl enable {service_name}"
+    cmd = f'systemctl enable {service_name}'
     if now:
-        cmd = cmd + " --now"
+        cmd = cmd + ' --now'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not enable {service_name}")
-        run(f"systemctl status {service_name}")
-        run("journalctl -xn")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not enable {service_name}')
+        run(f'systemctl status {service_name}')
+        run('journalctl -xn')
         return False
     return True
 
 
-def service_status(service_name, verbose=True):  # noqa: ANN001, ANN201
+def service_status(service_name):  # noqa: ANN001, ANN201
     """Check service status
     The arguments are:
     Name of service
     Returns:
     0 - service is running and OK
     1 - service is dead and /run pid file exists
     2 - service is dead and /lock lock file exists
     3 - service is not running
     4 - service could not be found.
     False - something went wrong.
     """
-    cmd = f"systemctl status {service_name}"
+    cmd = f'systemctl status {service_name}'
     has_systemctl = True
 
-    if not exists("systemctl"):
+    if not exists('systemctl'):
         has_systemctl = False
     if not has_systemctl:
-        cmd = f"service {service_name} status"
+        cmd = f'service {service_name} status'
 
-    retcode = run(cmd, capture_output=False, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode == 0:
-        print(f"INFO: Service {service_name} is running.")
+        logging.info(f'Service {service_name} is running.')
     elif retcode == 1:
-        print(f"INFO: Service {service_name} is dead and /run pid file exists.")
+        logging.info(f'Service {service_name} is dead and /run pid file exists.')
     elif retcode == 2:
-        print(f"INFO: Service {service_name} is dead and /lock lock file exists.")
+        logging.info(f'Service {service_name} is dead and /lock lock file exists.')
     elif retcode == 3:
-        print(f"INFO: Service {service_name} is not running.")
+        logging.info(f'Service {service_name} is not running.')
     elif retcode == 4:
-        print(f"INFO: Service {service_name} could not be found.")
+        logging.info(f'Service {service_name} could not be found.')
     else:
-        print(f"INFO: Service {service_name} returned unknown code {retcode}.")
+        logging.info(f'Service {service_name} returned unknown code {retcode}.')
     return retcode
 
 
 def is_service_running(service_name):  # noqa: ANN001, ANN201
     """Check if service is running
     The arguments are:
     Name of service
     Returns:
      True: service is running
      False: service is not running.
     """
-    return service_status(service_name, verbose=False) == 0
+    return service_status(service_name) == 0
 
 
 def os_arch():  # noqa: ANN201
-    ret, arch = run_ret_out("uname -m", verbose=False, return_output=True)
+    ret, arch = run_ret_out('uname -m', return_output=True)
     if ret != 0:
-        print("FAIL: could not get OS arch")
+        logging.error('could not get OS arch')
         return None
 
     return arch
 
 
-def is_installed(pack, verbose=False):  # noqa: ANN001, ANN201
+def is_installed(pack):  # noqa: ANN001, ANN201
     """Checks if package is installed."""
-    ret, ver = run_ret_out(f"rpm -q {pack}", verbose=False, return_output=True)
+    ret, ver = run_ret_out(f'rpm -q {pack}', return_output=True)
     if ret == 0:
-        if verbose:
-            print(f"INFO: {pack} is installed ({ver})")
+        logging.info(f'{pack} is installed ({ver})')
         return True
 
-    if verbose:
-        print(f"INFO: {pack} is not installed ")
+    logging.info(f'{pack} is not installed ')
     return False
 
 
-def install_package(pack, check=True, verbose=True):  # noqa: ANN001, ANN201
+def install_package(pack, check=True):  # noqa: ANN001, ANN201
     """Install a package "pack" via `yum|dnf install -y`."""
     # Check if package is already installed
-    if check and is_installed(pack, verbose):
+    if check and is_installed(pack):
         return True
 
-    packmngr = "yum"
-    if is_installed("dnf"):
-        packmngr = "dnf"
+    packmngr = 'yum'
+    if is_installed('dnf'):
+        packmngr = 'dnf'
 
-    if run(f"{packmngr} install -y {pack}").returncode != 0:
-        msg = f"FAIL: Could not install {pack}"
+    if run(f'{packmngr} install -y {pack}').rc != 0:
+        msg = f'FAIL: Could not install {pack}'
         print(msg)
         return False
 
-    if verbose:
-        print(f"INFO: {pack} was successfully installed")
+    logging.info(f'{pack} was successfully installed')
     return True
 
 
 def package_version(pkg):  # noqa: ANN001, ANN201
     """Get the version of specific package."""
     if not pkg:
-        print("FAIL: package_version requires package name as parameter")
+        logging.error('package_version requires package name as parameter')
         return None
 
     release = dist_name().lower()
     if not release:
-        print("FAIL: package_version() - Couldn't get release")
+        logging.error("package_version() - Couldn't get release")
         return None
-    if exists("rpm"):
+    if exists('rpm'):
         ret, output = run_ret_out(
             "rpm -qa --qf='%%{version}.%%{release}' %s" % pkg,
             return_output=True,
-            verbose=False,
         )
         if ret != 0:
-            print(f"FAIL: Could not get version for package: {pkg}")
+            logging.error(f'Could not get version for package: {pkg}')
             print(output)
             return None
         return output
 
-    print(f"FAIL: package_version() - Unsupported release: {release}")
+    logging.error(f'package_version() - Unsupported release: {release}')
     return None
 
 
-def compare_version(package: str, version: str, release: str, equal: bool = True) -> Union[bool, None]:
-    """Returns 'True' if installed version is newer or equal than asked,
-    'False' if older Return 'None' if the package is not installed (not found).
-
-    Args:
-      package: package name
-      version: package version
-      release: package release
-      equal: return value if packaged are equal version (default 'True').
-    """
-    pkg = package_version(package)
-    if pkg is None:
-        return None
-    if any(True for x in pkg if not isinstance(x, int)):
-        # cut ending of package name containing string, parse_version() does not work with ints and strings at once
-        pack = [int(p) for p in pkg.split(".") if p.isdigit()]
-        pkg = ".".join(map(str, pack))
-    if equal:
-        return parse_version(version + "." + release) <= parse_version(pkg)
-    return parse_version(version + "." + release) < parse_version(pkg)
-
-
 def wait_udev(sleeptime=15):  # noqa: ANN001, ANN201
     """Wait udev to finish. Often used after scsi rescan."""
-    print("INFO: Waiting udev to finish storage scan")
+    logging.info('Waiting udev to finish storage scan')
     # For example, on RHEL 7 scsi_wait_scan module is deprecated
-    if run("modinfo scsi_wait_scan", verbose=False).returncode == 0:
-        run("modprobe -q scsi_wait_scan")
-        run("modprobe -r -q scsi_wait_scan")
+    if run('modinfo scsi_wait_scan').rc == 0:
+        run('modprobe -q scsi_wait_scan')
+        run('modprobe -r -q scsi_wait_scan')
 
-    run("udevadm settle")
+    run('udevadm settle')
     sleep(sleeptime)
 
     return True
 
 
 def get_all_loaded_modules():  # noqa: ANN201
     """Check /proc/modules and return a list of all modules that are loaded."""
     cmd = 'cat /proc/modules | cut -d " " -f 1'
-    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print(f"FAIL: load_module() - Could not execute: {cmd}")
+        logging.error(f'load_module() - Could not execute: {cmd}')
         print(output)
         return None
 
-    return output.split("\n")
+    return output.split('\n')
 
 
 def load_module(module):  # noqa: ANN001, ANN201
     """Run modprobe using module with parameters given as input
     Parameters:
     module:       module name and it's parameters.
     """
     if not module:
-        print("FAIL: load_module() - requires module parameter")
+        logging.error('load_module() - requires module parameter')
         return False
-    cmd = f"modprobe {module}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: load_module() - Could not execute: {module}")
+    cmd = f'modprobe {module}'
+    if run(cmd).rc != 0:
+        logging.error(f'load_module() - Could not execute: {module}')
         return False
     return True
 
 
 def unload_module(module_name, remove_dependent=False):  # noqa: ANN001, ANN201
     """Run rmmod to unload module
     Parameters:
     module_name:       module name.
     """
     if not module_name:
-        print("FAIL: unload_module() - requires module_name parameter")
+        logging.error('unload_module() - requires module_name parameter')
         return False
-    cmd = f"modprobe -r {module_name}"
+    cmd = f'modprobe -r {module_name}'
 
     if remove_dependent:
         dep_modules = get_dependent_modules(module_name)
         if dep_modules:  # print info only if there are any modules to remove
-            print(f"INFO: Removing modules dependent on {module_name}")
+            logging.info(f'Removing modules dependent on {module_name}')
             for module in dep_modules:
                 if not unload_module(module, remove_dependent=remove_dependent):
-                    print("FAIL: unload_module() - Could not unload dependent modules")
+                    logging.error('unload_module() - Could not unload dependent modules')
                     return False
 
-    if run(cmd).returncode != 0:
-        print(f"FAIL: unload_module() - Could not unload: {module_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'unload_module() - Could not unload: {module_name}')
         return False
 
     return True
 
 
 def get_dependent_modules(module_name):  # noqa: ANN001, ANN201
     """Returns list of modules that loaded this module as a dependency
     Useful when removing parent modules (error "Module is in use by: ")
     Parameters:
     module_name:      module_name.
     """
     if not module_name:
-        print("FAIL: get_dependent_modules() - requires module_name parameter")
+        logging.error('get_dependent_modules() - requires module_name parameter')
         return None
     cmd = f'cat /proc/modules | grep -Ew "^{module_name}" | cut -d \' \' -f 4 | tr "," " "'
-    ret, dependent_modules = run_ret_out(cmd, return_output=True, verbose=False)
-    if dependent_modules == "-":
+    ret, dependent_modules = run_ret_out(cmd, return_output=True)
+    if dependent_modules == '-':
         return []  # No dependent modules found
     if ret != 0:
-        print("FAIL: get_dependent_modules() - failed to get a list of modules")
+        logging.error('get_dependent_modules() - failed to get a list of modules')
         return None
     return dependent_modules.split()
 
 
 def is_module_loaded(module_name):  # noqa: ANN001, ANN201
     """Check if given module is loaded
     Parameters:
@@ -460,84 +434,84 @@
     sys.stdout.flush()
     sys.stderr.flush()
     time.sleep(duration)
 
 
 def is_mounted(device=None, mountpoint=None):  # noqa: ANN001, ANN201
     """Check if mountpoint is already mounted."""
-    if device and run(f"mount | grep {device}", verbose=False) != 0:
+    if device and run(f'mount | grep {device}') != 0:
         return False
-    if mountpoint and run(f"mount | grep {mountpoint}", verbose=False) != 0:
+    if mountpoint and run(f'mount | grep {mountpoint}') != 0:
         return False
     return True
 
 
 def mount(device=None, mountpoint=None, fs=None, options=None):  # noqa: ANN001, ANN201
-    cmd = "mount"
+    cmd = 'mount'
     if fs:
-        cmd += f" -t {fs}"
+        cmd += f' -t {fs}'
     if options:
-        cmd += f" -o {options}"
+        cmd += f' -o {options}'
     if device:
-        cmd += f" {device}"
+        cmd += f' {device}'
     if mountpoint:
-        cmd += f" {mountpoint}"
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not mount partition")
+        cmd += f' {mountpoint}'
+    if run(cmd).rc != 0:
+        logging.error('Could not mount partition')
         return False
 
     return True
 
 
 def umount(device=None, mountpoint=None):  # noqa: ANN001, ANN201
-    cmd = "umount"
+    cmd = 'umount'
     if device:
-        cmd += f" {device}"
+        cmd += f' {device}'
         if not is_mounted(device):
             # Device is not mounted
             return True
 
     if mountpoint:
-        cmd += f" {mountpoint}"
+        cmd += f' {mountpoint}'
         if not is_mounted(mountpoint=mountpoint):
             # Device is not mounted
             return True
 
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not umount partition")
+    if run(cmd).rc != 0:
+        logging.error('Could not umount partition')
         return False
 
     return True
 
 
 def get_default_fs():  # noqa: ANN201
     """Return the default FileSystem for this release."""
-    if dist_name() == "RHEL" and dist_ver() > 6:
-        return "xfs"
+    if dist_name() == 'RHEL' and dist_ver() > 6:
+        return 'xfs'
 
-    return "ext4"
+    return 'ext4'
 
 
 def run_cmd_background(cmd):  # noqa: ANN001, ANN201
     """Run Command on background
     Returns:
     subprocess.
     PID is on process.pid
-    Exit code is on process.returncode (after run process.communicate())
+    Exit code is on process.rc (after run process.communicate())
     Wait for process to finish
     while process.poll() is None:
     sleep(1)
     Get stdout and stderr
     (stdout, stderr) = process.communicate().
     """
     process = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     if not process:
-        print(f"FAIL: Could not run '{cmd}' on background")
+        logging.error(f"Could not run '{cmd}' on background")
         return None
-    print("INFO: running %s on background. PID is %d" % (cmd, process.pid))
+    logging.info(f'running {cmd} on background. PID is {process.pid}')
     return process
 
 
 def kill_pid(pid):  # noqa: ANN001, ANN201
     os.kill(pid, signal.SIGTERM)
     sleep(1)
     if check_pid(pid):
@@ -545,15 +519,15 @@
         sleep(1)
         if check_pid(pid):
             return False
     return True
 
 
 def kill_all(process_name):  # noqa: ANN001, ANN201
-    ret = run(f"killall {process_name}", verbose=False).returncode
+    ret = run(f'killall {process_name}').rc
     # Wait few seconds for process to finish
     sleep(3)
     return ret
 
 
 def check_pid(pid):  # noqa: ANN001, ANN201
     """Check there is a process running with this PID."""
@@ -571,25 +545,25 @@
             raise
 
 
 def time_stamp(utc: bool = False, in_seconds: bool = False):  # noqa: ANN201
     now = datetime.now(tz=timezone.utc if utc else None)
 
     # ts = "%s%s%s%s%s%s" % (now.year, now.month, now.day, now.hour, now.minute, now.second)
-    ts = now.strftime("%Y%m%d%H%M%S")
+    ts = now.strftime('%Y%m%d%H%M%S')
     if in_seconds:
-        ts = now.strftime("%s")
+        ts = now.strftime('%s')
     return ts
 
 
 def kernel_command_line():  # noqa: ANN201
     """Return the kernel command line used to boot."""
-    retcode, output = run_ret_out("cat /proc/cmdline", return_output=True, verbose=False)
+    retcode, output = run_ret_out('cat /proc/cmdline', return_output=True)
     if retcode != 0:
-        print("FAIL: could not get kernel command line")
+        logging.error('could not get kernel command line')
         print(output)
         return None
     return output
 
 
 def kernel_version():  # noqa: ANN201
     """Usage
@@ -597,21 +571,21 @@
     Purpose
         Check out running kernel version. The same as output of `uname -r`
     Parameter
         N/A
     Returns
         kernel_version.
     """
-    retcode, output = run_ret_out("uname -r", return_output=True, verbose=False)
+    retcode, output = run_ret_out('uname -r', return_output=True)
     if retcode != 0:
-        print("FAIL: could not get kernel version")
+        logging.error('could not get kernel version')
         print(output)
         return None
     # remove arch detail and kernel type
-    return re.sub(r"\.%s.*" % os_arch(), "", output)
+    return re.sub(r'\.%s.*' % os_arch(), '', output)
 
 
 def kernel_type():  # noqa: ANN201
     """Usage
         kernel_type()
     Purpose
         Check the kernel type. Current we support detection of these types:
@@ -619,27 +593,27 @@
             2. debug kernel.
             3. rt kernel.
     Parameter
         N/A
     Returns
         kernel_type        # 'debug|rt|default'.
     """
-    retcode, version = run_ret_out("uname -r", return_output=True, verbose=False)
+    retcode, version = run_ret_out('uname -r', return_output=True)
     if retcode != 0:
-        print("FAIL: kernel_type() - could not get kernel version")
+        logging.error('kernel_type() - could not get kernel version')
         print(version)
         return None
 
-    if re.match(r".*\.debug$", version):
-        return "debug"
+    if re.match(r'.*\.debug$', version):
+        return 'debug'
 
-    if re.match(r".*\.rt$", version):
-        return "rt"
+    if re.match(r'.*\.rt$', version):
+        return 'rt'
 
-    return "default"
+    return 'default'
 
 
 def kmem_leak_start():  # noqa: ANN201
     """Usage
         kmem_leak_start()
     Purpose
         Start and clear kernel memory leak detection.
@@ -648,47 +622,47 @@
     Returns
         True
           or
         False       # not debug kernel or failure found.
     """
     k_type = kernel_type()
 
-    if not k_type or k_type != "debug":
-        print("WARN: Not debug kernel, will not enable kernel memory leak check")
+    if not k_type or k_type != 'debug':
+        logging.warning('Not debug kernel, will not enable kernel memory leak check')
         return False
 
     arch = os_arch()
-    if arch == "i386" or arch == "i686":
-        print("INFO: Not enabling kmemleak on 32 bits server.")
+    if arch == 'i386' or arch == 'i686':
+        logging.info('Not enabling kmemleak on 32 bits server.')
         return False
 
     k_commandline = kernel_command_line()
-    if not re.search("kmemleak=on", k_commandline):
-        print("WARN: kmem_leak_start(): need 'kmemleak=on' kernel_option to enable kernel memory leak detection")
+    if not re.search('kmemleak=on', k_commandline):
+        logging.warning("kmem_leak_start(): need 'kmemleak=on' kernel_option to enable kernel memory leak detection")
 
     check_debugfs_mount_cmd = 'mount | grep "/sys/kernel/debug type debugfs"'
-    retcode = run(check_debugfs_mount_cmd, verbose=False).returncode
+    retcode = run(check_debugfs_mount_cmd).rc
     if retcode != 0:
         # debugfs is not mounted
-        mount_debugfs_cli_cmd = "mount -t debugfs nodev /sys/kernel/debug"
-        run(mount_debugfs_cli_cmd, verbose=True)
+        mount_debugfs_cli_cmd = 'mount -t debugfs nodev /sys/kernel/debug'
+        run(mount_debugfs_cli_cmd)
         check_debugfs_mount_cmd = 'mount | grep "/sys/kernel/debug type debugfs"'
-        retcode, output = run_ret_out(check_debugfs_mount_cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(check_debugfs_mount_cmd, return_output=True)
         if retcode != 0:
-            print("WARN: Failed to mount debugfs to /sys/kernel/debug")
+            logging.warning('Failed to mount debugfs to /sys/kernel/debug')
             print(output)
             return False
 
     # enable kmemleak and clear
-    print("INFO: Begin kernel memory leak check")
-    if run("echo scan=on > /sys/kernel/debug/kmemleak") != 0:
+    logging.info('Begin kernel memory leak check')
+    if run('echo scan=on > /sys/kernel/debug/kmemleak') != 0:
         return False
-    if run("echo stack=on > /sys/kernel/debug/kmemleak") != 0:
+    if run('echo stack=on > /sys/kernel/debug/kmemleak') != 0:
         return False
-    if run("echo clear > /sys/kernel/debug/kmemleak") != 0:
+    if run('echo clear > /sys/kernel/debug/kmemleak') != 0:
         return False
     return True
 
 
 def kmem_leak_check():  # noqa: ANN201
     """Usage
         kmem_leak_check()
@@ -698,31 +672,31 @@
         N/A
     Returns
         kmemleak_log
           or
         None       # when file '/sys/kernel/debug/kmemleak' not exists
                   # or no leak found.
     """
-    sysfs_kmemleak = "/sys/kernel/debug/kmemleak"
+    sysfs_kmemleak = '/sys/kernel/debug/kmemleak'
     if not Path(sysfs_kmemleak).is_file():
         return None
 
     with Path(sysfs_kmemleak).open() as f:
         if not f:
-            print(f"FAIL: Could not read {sysfs_kmemleak}")
+            logging.error(f'Could not read {sysfs_kmemleak}')
             return None
         kmemleak_log = f.read()
 
     if kmemleak_log:
-        print(f"WARN: Found kernel memory leak:\n{kmemleak_log}")
-        print("INFO: Clearing memory leak for next check")
+        logging.warning(f'Found kernel memory leak:\n{kmemleak_log}')
+        logging.info('Clearing memory leak for next check')
         run(f"echo 'clear' > {sysfs_kmemleak}")
         return kmemleak_log
 
-    print("INFO: No kernel memory leak found")
+    logging.info('No kernel memory leak found')
     return None
 
 
 def kmem_leak_disable():  # noqa: ANN201
     """Usage
         kmem_leak_disable()
     Purpose
@@ -731,28 +705,28 @@
     Parameter
         N/A
     Returns
         True           # disabled or not enabled yet
           or
         False       # failed to run 'echo' command.
     """
-    sysfs_kmemleak = "/sys/kernel/debug/kmemleak"
+    sysfs_kmemleak = '/sys/kernel/debug/kmemleak'
     if not Path(sysfs_kmemleak).is_file():
         return True
 
-    print("INFO: kmem_leak_disable(): Disabling kernel memory leak detection")
-    ok1, ok1_output = run_ret_out(f"echo scan=off > {sysfs_kmemleak}", return_output=True)
-    ok2, ok2_output = run_ret_out(f"echo stack=off > {sysfs_kmemleak}", return_output=True)
+    logging.info('kmem_leak_disable(): Disabling kernel memory leak detection')
+    ok1, ok1_output = run_ret_out(f'echo scan=off > {sysfs_kmemleak}', return_output=True)
+    ok2, ok2_output = run_ret_out(f'echo stack=off > {sysfs_kmemleak}', return_output=True)
     if ok1 != 0 or ok2 != 0:
-        print("FAIL: kmem_leak_disable(): Failed to disable kernel memory leak detection")
+        logging.error('kmem_leak_disable(): Failed to disable kernel memory leak detection')
         print(ok1_output)
         print(ok2_output)
         return False
 
-    print("INFO: kmem_leak_disable(): Kernel memory leak detection disabled")
+    logging.info('kmem_leak_disable(): Kernel memory leak detection disabled')
     return True
 
 
 def query_os_info():  # noqa: ANN201
     """Query OS information and set a reference below:
         os_info = {
             dist_name       = dist_name,
@@ -767,118 +741,118 @@
         N/A
     Returns
         os_info_dict
             or
         None       # got error
     """
     return {
-        "dist_name": dist_name(),
-        "dist_version": dist_ver(),
-        "dist_release": dist_release(),
-        "os_arch": os_arch(),
-        "arch": os_arch(),
-        "pkg_arch": os_arch(),
-        "kernel_version": kernel_version(),
-        "kernel_type": kernel_type(),
+        'dist_name': dist_name(),
+        'dist_version': dist_ver(),
+        'dist_release': dist_release(),
+        'os_arch': os_arch(),
+        'arch': os_arch(),
+        'pkg_arch': os_arch(),
+        'kernel_version': kernel_version(),
+        'kernel_type': kernel_type(),
     }
 
 
 def get_driver_info(driver: str):  # noqa: ANN201
     if not driver:
-        print("FAIL: get_driver_info() - requires driver parameter")
+        logging.error('get_driver_info() - requires driver parameter')
         return None
 
-    sys_fs_dir = "/sys/module"
+    sys_fs_dir = '/sys/module'
     sys_fs_path = Path(sys_fs_dir)
     if not sys_fs_path.is_dir():
-        print(f"FAIL: get_driver_info() - {sys_fs_path} is not a valid directory")
+        logging.error(f'get_driver_info() - {sys_fs_path} is not a valid directory')
         return None
 
     sysfs_driver_folder = sys_fs_path / driver
     if not sysfs_driver_folder.is_dir():
-        print(f"FAIL: get_driver_info() - module {driver} is not loaded")
+        logging.error(f'get_driver_info() - module {driver} is not loaded')
         return None
 
     driver_info = {}
-    infos = ["srcversion", "version", "taint"]
+    infos = ['srcversion', 'version', 'taint']
     for info in infos:
         info_path = sysfs_driver_folder / info
         if not Path(info_path).is_file():
             continue
-        output = run(f"cat {info_path}", capture_output=True, verbose=False).output
+        output = run(f'cat {info_path}').stdout
         driver_info[info] = output
 
-    sys_driver_parameter = sysfs_driver_folder / "parameters"
+    sys_driver_parameter = sysfs_driver_folder / 'parameters'
     if sys_driver_parameter.is_dir():
         # Need to add driver parameters
         param_files = list(sys_driver_parameter.iterdir())
         for param in param_files:
-            output = run(f"cat {sys_driver_parameter}/{param}", capture_output=True, verbose=False).output
-            if "parameters" not in driver_info:
-                driver_info["parameters"] = {}
-            driver_info["parameters"][param] = output
+            output = run(f'cat {sys_driver_parameter}/{param}').stdout
+            if 'parameters' not in driver_info:
+                driver_info['parameters'] = {}
+            driver_info['parameters'][param] = output
     return driver_info
 
 
 def mkdir(new_dir):  # noqa: ANN001, ANN201
     if Path(new_dir).is_dir():
-        print(f"INFO: {new_dir} already exist")
+        logging.info(f'{new_dir} already exist')
         return True
-    cmd = f"mkdir -p {new_dir}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'mkdir -p {new_dir}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: could create directory {new_dir}")
+        logging.error(f'could create directory {new_dir}')
         print(output)
         return False
     return True
 
 
 def rmdir(dir_name):  # noqa: ANN001, ANN201
     """Remove directory and all content from it."""
     if not Path(dir_name).is_dir():
-        print(f"INFO: {dir_name} does not exist")
+        logging.info(f'{dir_name} does not exist')
         return True
-    cmd = f"rm -rf {dir_name}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'rm -rf {dir_name}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: could remove directory {dir_name}")
+        logging.error(f'could remove directory {dir_name}')
         print(output)
         return False
     return True
 
 
 def mkfs(device_name, fs_type, force=False):  # noqa: ANN001, ANN201
     """Create a Filesystem on device."""
     if not device_name or not fs_type:
-        print("INFO: mkfs() requires device_name and fs_type")
+        logging.info('mkfs() requires device_name and fs_type')
         return False
 
-    force_option = "-F"
-    if fs_type == "xfs":
-        force_option = "-f"
+    force_option = '-F'
+    if fs_type == 'xfs':
+        force_option = '-f'
 
-    cmd = f"mkfs.{fs_type} "
+    cmd = f'mkfs.{fs_type} '
     if force:
-        cmd += f"{force_option} "
+        cmd += f'{force_option} '
     cmd += device_name
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=True)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: could create filesystem {fs_type} on {device_name}")
+        logging.error(f'could create filesystem {fs_type} on {device_name}')
         print(output)
         return False
     return True
 
 
 def sync(directory=None):  # noqa: ANN001, ANN201
-    cmd = "sync"
+    cmd = 'sync'
     if directory:
-        cmd += f" {directory}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+        cmd += f' {directory}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: could not sync")
+        logging.error('could not sync')
         print(output)
         return False
     return True
 
 
 def get_free_space(path):  # noqa: ANN001, ANN201
     """Get free space of a path.
@@ -886,164 +860,163 @@
     /dev/sda
     /root
     ./.
     """
     if not path:
         return None
 
-    cmd = f"df -B 1 {path}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'df -B 1 {path}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: get_free_space() - could not run {cmd}")
+        logging.error(f'get_free_space() - could not run {cmd}')
         print(output)
         return None
-    fs_list = output.split("\n")
+    fs_list = output.split('\n')
     # delete the header info
     del fs_list[0]
 
     if len(fs_list) > 1:
         # Could be the information was too long and splited in lines
-        tmp_info = "".join(fs_list)
+        tmp_info = ''.join(fs_list)
         fs_list[0] = tmp_info
 
     # expected order
     # Filesystem    1B-blocks       Used   Available Use% Mounted on
-    free_space_regex = re.compile(r"\S+\s+\d+\s+\d+\s+(\d+)")
+    free_space_regex = re.compile(r'\S+\s+\d+\s+\d+\s+(\d+)')
     m = free_space_regex.search(fs_list[0])
     if m:
         return int(m.group(1))
     return None
 
 
 def get_block_device_name(device):  # noqa: ANN001, ANN201
     """Returns kernel name from block device
     eg. lvm1 from /dev/mapper/lvm1.
     """
-    if not device.startswith("/dev/"):
+    if not device.startswith('/dev/'):
         device = get_full_path(device)
     if not device:
-        print("FAIL: get_block_device_name - unknown device")
-    cmd = f"lsblk -ndlo NAME {device}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+        logging.error('get_block_device_name - unknown device')
+    cmd = f'lsblk -ndlo NAME {device}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: run {cmd}")
+        logging.error(f'run {cmd}')
         print(output)
         return None
     return output
 
 
 def get_full_path(device_name):  # noqa: ANN001, ANN201
     """Returns full block device path, eg. from device: /dev/mapper/device."""
     cmds = [
-        f"lsblk -pnalo NAME  | grep {device_name} -m1",  # should be more robust
-        f"find /dev/ -name {device_name}",
+        f'lsblk -pnalo NAME  | grep {device_name} -m1',  # should be more robust
+        f'find /dev/ -name {device_name}',
     ]  # older OS(rhel-6), will fail with partitions
 
     for cmd in cmds:
-        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
-        if retcode == 0 and output != "":
+        retcode, output = run_ret_out(cmd, return_output=True)
+        if retcode == 0 and output != '':
             return output
 
-    print(f"FAIL: get_full_path() - {device_name}")
+    logging.error(f'get_full_path() - {device_name}')
     return None
 
 
 def get_parent_device(child_device, only_direct=False):  # noqa: ANN001, ANN201
     """Returns block device's parent device: eg. sda, nvme0n1
     child_device: eg. /dev/sda2, nvme0n1p1, /dev/mapper/device
     only_direct: returns only the direct parent. eg. lvm -> sda3, not sda.
     """
-    if not child_device.startswith("/dev/"):
+    if not child_device.startswith('/dev/'):
         child_device = get_full_path(child_device)
     if not child_device:  # get_full_path would return None if device does not exist
-        print(f"FAIL: get_parent_device - unknown child_device '{child_device}'")
-    cmd = f"lsblk -nsl {child_device} -o KNAME | tail -n 1"
+        logging.error(f"get_parent_device - unknown child_device '{child_device}'")
+    cmd = f'lsblk -nsl {child_device} -o KNAME | tail -n 1'
     if only_direct:
-        cmd = f"lsblk -nsl {child_device} -o KNAME | sed -n 2p"  # if no parent, returns nothing
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+        cmd = f'lsblk -nsl {child_device} -o KNAME | sed -n 2p'  # if no parent, returns nothing
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: run {cmd}")
+        logging.error(f'run {cmd}')
         print(output)
         return None
     if not output or output == child_device:
-        print("WARN: get_parent_device - device has no parent")
+        logging.warning('get_parent_device - device has no parent')
         return None
     return output
 
 
 def get_udev_property(device_name: str, property_key: str) -> Union[str, None]:
     """Given an /dev device name, returns specified property using udevadm.
 
     Args:
       device_name: e.g. 'sda', 'mpatha', 'dm-0', 'nvme0n1', 'sr0', ...
       property_key: eg. 'ID_SERIAL', 'DM_WWN', 'ID_PATH', ...
     :return property_value: eg. for ID_SERIAL: '360fff19abdd9f5fb943525d45126ca27'
     """
     if not device_name:
-        print("WARN: get_udev_property() - requires device_name parameter")
+        logging.warning('get_udev_property() - requires device_name parameter')
         return None
 
     # Converts for example mpatha to /dev/mapper/mpatha or sda to /dev/sda
     device = get_full_path(device_name)
     if not device:
-        print(f"FAIL: get_udev_property - unknown device_name '{device_name}'")
+        logging.error(f"get_udev_property - unknown device_name '{device_name}'")
 
     # Trying to catch wrong key name when dm-multipath is used.
     if mp.is_mpath_device(device_name, print_fail=False):  # noqa: SIM102
-        if property_key.startswith("ID_") and not property_key.startswith("ID_FS_"):
-            property_key = property_key.replace("ID_", "DM_")
+        if property_key.startswith('ID_') and not property_key.startswith('ID_FS_'):
+            property_key = property_key.replace('ID_', 'DM_')
 
     ret, property_value = run_ret_out(
-        f"udevadm info -q property --name={device} | grep {property_key}= | cut -d = -f 2",
+        f'udevadm info -q property --name={device} | grep {property_key}= | cut -d = -f 2',
         return_output=True,
-        verbose=False,
     )
     if ret:
-        print(f"WARN: Could not get udevadm info of device '{device}'")
+        logging.warning(f"Could not get udevadm info of device '{device}'")
         return None
     if not property_value:
-        print(f"WARN: Could not find property '{property_key}' in udevadm info of device '{device}'")
+        logging.warning(f"Could not find property '{property_key}' in udevadm info of device '{device}'")
         return None
 
     return property_value
 
 
 def get_boot_device(parent_device=False, full_path=False):  # noqa: ANN001, ANN201
     """Returns boot device, eg. 'sda1'
     parent_device, eg. 'sda'
     full_path, eg. '/dev/sda1'.
     """
-    boot_mount = "/boot"
-    root_mount = "/"
+    boot_mount = '/boot'
+    root_mount = '/'
     # get boot device
     cmd = f"mount | grep ' {boot_mount} ' | cut -d ' ' -f 1"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: run {cmd}")
+        logging.error(f'run {cmd}')
         print(output)
         return None
     boot_device = output
     # get root device
     cmd = f"mount | grep ' {root_mount} ' | cut -d ' ' -f 1"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: run {cmd}")
+        logging.error(f'run {cmd}')
         print(output)
         return None
     root_device = output
 
     if not boot_device and not root_device:
-        print("FAIL: Could not find '/boot' and '/' mounted!")
+        logging.error("Could not find '/boot' and '/' mounted!")
         return None
     if not boot_device:
         # /boot is not mounted on openstack virtual machines
-        print("INFO: Could not find /boot mounted... Assuming this is a virtual machine")
+        logging.info('Could not find /boot mounted... Assuming this is a virtual machine')
         boot_device = root_device
-    if boot_device == "overlay":
-        print("INFO: / mounted on overlay device. Assuming running in a container")
+    if boot_device == 'overlay':
+        logging.info('/ mounted on overlay device. Assuming running in a container')
         return None
 
     if parent_device:
         boot_device = get_parent_device(boot_device)
     if full_path:
         return get_full_path(boot_device)
     return get_block_device_name(boot_device)
@@ -1054,114 +1027,114 @@
 
     Args:
       device_name: e.g. 'sda', 'mpatha', ...
     """
     # Converts for example mpatha to /dev/mapper/mpatha or sda to /dev/sda
     device = get_full_path(device_name)
     if not device:
-        print(f"FAIL: is_dm_device - unknown device_name '{device_name}'")
+        logging.error(f"is_dm_device - unknown device_name '{device_name}'")
         return False
-    ret, name = run_ret_out(f"udevadm info -q name --name={device}", return_output=True, verbose=False)
+    ret, name = run_ret_out(f'udevadm info -q name --name={device}', return_output=True)
     if ret:
-        print(f"FAIL: Could not get udevadm info for device '{device}'")
+        logging.error(f"Could not get udevadm info for device '{device}'")
         return False
     if not name:
-        print(f"FAIL: Could not find udev name for '{device}'")
+        logging.error(f"Could not find udev name for '{device}'")
         return False
 
-    if name.startswith("dm"):
+    if name.startswith('dm'):
         return True
 
     return False
 
 
 def is_nvme_device(device):  # noqa: ANN001, ANN201
     """Checks if device is nvme device."""
-    return bool(re.match("^nvme[0-9]n[0-9]$", device))
+    return bool(re.match('^nvme[0-9]n[0-9]$', device))
 
 
 def get_wwid_of_nvme(device):  # noqa: ANN001, ANN201
     """Reads WWID from udev ID_WWN."""
-    return get_udev_property(device, property_key="ID_WWN")
+    return get_udev_property(device, property_key='ID_WWN')
 
 
 def get_device_wwid(device):  # noqa: ANN001, ANN201
     """Given an SCSI, NVMe or multipath device, returns its WWID."""
-    if device.startswith("vd"):
-        print(f"INFO: {device}: Presuming virtual disk does not have wwid.")
+    if device.startswith('vd'):
+        logging.info(f'{device}: Presuming virtual disk does not have wwid.')
         return None
 
-    serial = get_udev_property(device_name=device, property_key="ID_SERIAL")
+    serial = get_udev_property(device_name=device, property_key='ID_SERIAL')
     if not serial and is_dm_device(device):  # RHEL-6 workaround
-        dm_uuid = get_udev_property(device_name=device, property_key="DM_UUID")
-        serial = dm_uuid.replace("mpath-", "")
+        dm_uuid = get_udev_property(device_name=device, property_key='DM_UUID')
+        serial = dm_uuid.replace('mpath-', '')
     if not serial:
-        print(f"INFO: get_device_wwid() - Could not find WWID for {device}")
+        logging.info(f'get_device_wwid() - Could not find WWID for {device}')
         return None
 
     return serial
 
 
 def remove_device_wwid(wwid):  # noqa: ANN001, ANN201
     if not wwid:
-        print("FAIL: remove_device_wwid() - requires wwid as parameter")
+        logging.error('remove_device_wwid() - requires wwid as parameter')
         return False
 
     mpath_wwid = mp.mpath_name_of_wwid(wwid)
     if mpath_wwid:
         mp.remove_mpath(mpath_wwid)
 
     scsi_ids_wwid = scsi.scsi_ids_of_wwid(wwid)
     if scsi_ids_wwid:
         for scsi_id in scsi_ids_wwid:
             scsi_name = scsi.get_scsi_disk_name(scsi_id)
             if not scsi_name:
                 continue
-            print(f"INFO: detaching SCSI disk {scsi_name}")
+            logging.info(f'detaching SCSI disk {scsi_name}')
             scsi.delete_disk(scsi_name)
     return True
 
 
 def clear_dmesg():  # noqa: ANN201
-    cmd = "dmesg --clear"
+    cmd = 'dmesg --clear'
     if dist_ver() < 7:
-        cmd = "dmesg -c"
-    run(cmd, verbose=False)
+        cmd = 'dmesg -c'
+    run(cmd)
     return True
 
 
 def get_regex_pci_id():  # noqa: ANN201
-    regex_pci_id = r"(?:([0-0a-f]{4}):){0,1}"  # domain id (optional)
-    regex_pci_id += r"([0-9a-f]{2})"  # bus id
-    regex_pci_id += r":"
-    regex_pci_id += r"([0-9a-f]{2})"  # slot id
-    regex_pci_id += r"\."
-    regex_pci_id += r"(\d+)"  # function id
+    regex_pci_id = r'(?:([0-0a-f]{4}):){0,1}'  # domain id (optional)
+    regex_pci_id += r'([0-9a-f]{2})'  # bus id
+    regex_pci_id += r':'
+    regex_pci_id += r'([0-9a-f]{2})'  # slot id
+    regex_pci_id += r'\.'
+    regex_pci_id += r'(\d+)'  # function id
     return regex_pci_id
 
 
 def get_partitions(device):  # noqa: ANN001, ANN201
     """Return a list of all parition numbers from the device."""
     if not device:
-        print("WARN: get_partitions() - requires device as parameter")
+        logging.warning('get_partitions() - requires device as parameter')
         return None
 
-    cmd = f"parted -s {device} print"
-    ret, output = run_ret_out(cmd, verbose=False, return_output=True)
+    cmd = f'parted -s {device} print'
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        # print("FAIL: get_partitions() - Could not read partition information from %s" % device)
+        # logging.error("get_partitions() - Could not read partition information from %s" % device)
         # print output
         return None
 
-    lines = output.split("\n")
+    lines = output.split('\n')
     if not lines:
         return None
 
-    header_regex = re.compile(r"Number  Start   End     Size    Type")
-    partition_regex = re.compile(r"\s(\d+)\s+\S+")
+    header_regex = re.compile(r'Number  Start   End     Size    Type')
+    partition_regex = re.compile(r'\s(\d+)\s+\S+')
     partitions = []
     found_header = False
     for line in lines:
         if header_regex.match(line):
             found_header = True
             continue
         if found_header:
@@ -1171,132 +1144,132 @@
 
     return partitions
 
 
 def delete_partition(device, partition):  # noqa: ANN001, ANN201
     """Delete specific partition from the device."""
     if not device or not partition:
-        print("FAIL: delete_partition() - requires device and partition as argument")
+        logging.error('delete_partition() - requires device and partition as argument')
         return False
 
-    cmd = f"parted -s {device} rm {partition}"
-    ret, output = run_ret_out(cmd, verbose=False, return_output=True)
+    cmd = f'parted -s {device} rm {partition}'
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print("FAIL: delete_partition() - Could not delete partition %d from %s" % (partition, device))
+        logging.error(f'delete_partition() - Could not delete partition {partition} from {device}')
         print(output)
         return False
 
     return True
 
 
 def add_repo(name, address, metalink=False):  # noqa: ANN001, ANN201
     """Adds yum repository to /etc/yum.repos.d/NAME.repo."""
-    repo = Path(f"/etc/yum.repos.d/{name.lower()}.repo")
+    repo = Path(f'/etc/yum.repos.d/{name.lower()}.repo')
     if repo.is_file():
-        print(f"INFO: Repo {repo} already exists.")
+        logging.info(f'Repo {repo} already exists.')
         return True
 
-    url = "metalink" if metalink else "baseurl"
+    url = 'metalink' if metalink else 'baseurl'
 
     repo_conf_table = {
-        "name": name,
+        'name': name,
         url: address,
-        "enabled": "1",
-        "gpgcheck": "0",
-        "skip_if_unavailable": "1",
+        'enabled': '1',
+        'gpgcheck': '0',
+        'skip_if_unavailable': '1',
     }
 
-    repo_conf = f"[{name}]\n"
+    repo_conf = f'[{name}]\n'
     for setting, value in repo_conf_table.items():
-        repo_conf += f"{setting}={value}\n"
+        repo_conf += f'{setting}={value}\n'
 
-    with repo.open(mode="w") as f:
+    with repo.open(mode='w') as f:
         f.write(repo_conf)
 
     return True
 
 
 def download_repo_file(url, name=None, overwrite=True):  # noqa: ANN001, ANN201
     """Downloads .repo file to /etc.repos.d/."""
     if not url:
-        print("FAIL: repo file url argument required")
+        logging.error('repo file url argument required')
         return False
     if not name:
-        name = url.split("/")[-1]
-    if name[-5:] != ".repo":
-        name = f"{name}.repo"
-    path = f"/etc/yum.repos.d/{name}"
+        name = url.split('/')[-1]
+    if name[-5:] != '.repo':
+        name = f'{name}.repo'
+    path = f'/etc/yum.repos.d/{name}'
 
     if Path(path).is_file():
         if overwrite is False:
-            print(f"WARN: {name} exits, skipping repo file download")
+            logging.warning(f'{name} exits, skipping repo file download')
             return True
-        print(f"WARN: {name} exits, overwriting .repo file")
-    install_package("curl", check=True, verbose=False)
-    if not run(f"curl {url} --output {path}", verbose=True):
+        logging.warning(f'{name} exits, overwriting .repo file')
+    install_package('curl', check=True)
+    if not run(f'curl {url} --output {path}'):
         return False
 
     return True
 
 
 def del_repo(name):  # noqa: ANN001, ANN201
     """Removes .repo file."""
     try:
-        Path(f"/etc/yum.repos.d/{name}.repo").unlink()
+        Path(f'/etc/yum.repos.d/{name}.repo').unlink()
     except FileNotFoundError:
-        print(f"WARN: Removing repository {name} failed.")
+        logging.warning(f'Removing repository {name} failed.')
         return False
     return True
 
 
 def check_repo(name, check_if_enabled=True):  # noqa: ANN001, ANN201
     """Checks if repository works and is enabled."""
     if not name:
-        print("FAIL: repo name argument required")
+        logging.error('repo name argument required')
         return False
 
-    cmd = f"yum repoinfo {name} | grep Repo-status"  # yum=dnf alias works here
+    cmd = f'yum repoinfo {name} | grep Repo-status'  # yum=dnf alias works here
     ret, out = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print(f"{name} repo is not present")
+        print(f'{name} repo is not present')
         return False
-    if check_if_enabled and "enabled" not in out:
-        print(f"{name} repo is not enabled")
+    if check_if_enabled and 'enabled' not in out:
+        print(f'{name} repo is not enabled')
         return False
 
     return True
 
 
-def is_docker():  # noqa: ANN201
-    """Check if we are running inside docker container."""
-    cmd = "cat /proc/self/cgroup | grep docker"
-    if run(cmd, verbose=False).returncode == 0:
-        # It is docker
+def in_container() -> bool:
+    """Check if we are running inside container."""
+    if run('cat /proc/1/attr/current | grep container_t').rc == 0:
+        return True
+    if run('cat /proc/self/cgroup | grep docker').rc == 0:
         return True
     return False
 
 
-def get_memory(units="m", total=False):  # noqa: ANN001, ANN201
+def get_memory(units='m', total=False):  # noqa: ANN001, ANN201
     """Returns data from 'free' as a dict."""
-    possible_units = "b bytes k kilo m mega  g giga tera peta".split()
+    possible_units = 'b bytes k kilo m mega  g giga tera peta'.split()
     if units not in possible_units:
-        print("FAIL: 'units' must be one of %s" % [str(x) for x in possible_units])
+        logging.error(f"'units' must be one of {[str(x) for x in possible_units]}")
         return None
 
     memory = {}
     columns = []
 
     if len(units) > 1:
-        units = "-" + units
-    cmd = f"free -{units}"
+        units = '-' + units
+    cmd = f'free -{units}'
     if total:
-        cmd += " -t"
+        cmd += ' -t'
     ret, mem = run_ret_out(cmd=cmd, return_output=True)
     if ret != 0:
-        print(f"FAIL: Running '{cmd}' failed.")
+        logging.error(f"Running '{cmd}' failed.")
         return None
 
     for row, m in enumerate(mem.splitlines()):
         if row == 0:
             columns = [c.strip() for c in m.split()]
             continue
         m = [x.strip() for x in m.split()]  # noqa: PLW2901
@@ -1314,82 +1287,80 @@
     Args:
       service_name: Name of the service
 
     Returns:
     Time in format: a YYYY-MM-DD hh:mm:ss Z
     None: systemctl is not installed or timestamp does not exist
     """
-    if not exists("systemctl"):
-        cmd = f"systemctl show {service_name} --property=ActiveEnterTimestamp"
+    if not exists('systemctl'):
+        cmd = f'systemctl show {service_name} --property=ActiveEnterTimestamp'
         ret, data = run_ret_out(cmd, return_output=True)
         if ret == 0:
-            timestamp = data.split("=")
+            timestamp = data.split('=')
             if timestamp[1]:
                 return timestamp[1]
             return None
-        print(f"WARN: Could not get active enter timestamp of service: {service_name}")
+        logging.warning(f'Could not get active enter timestamp of service: {service_name}')
     return None
 
 
 def get_system_logs(
     length: Optional[int] = None,
     reverse: bool = False,
     kernel_only: bool = False,
     since: Optional[str] = None,
     grep: Optional[str] = None,
     options: Optional[List[str]] = None,
-    verbose: bool = False,
     return_output: bool = True,
 ) -> Union[Literal[0, 1], Tuple[Literal[0, 1]], Any]:
     """Gets system logs using journalctl.
 
     Args:
       length: Get last $length messages.
       reverse: Get logs in reverse.
       kernel_only: Get only kernel messages.
       since: Get messages since some time, can you '+' and '-' prefix.
       grep: String to test_filter messages using 'grep'.
       options: Any other possible options with its value as a string.
-      verbose: Print the journal when getting it.
       return_output: Should the function return only retcode or also the output.
 
     Returns:
       retcode / (retcode, data)
     """
-    cmd = "journalctl"
+    cmd = 'journalctl'
     if kernel_only:
-        cmd += " -k"
+        cmd += ' -k'
     if length:
-        cmd += f" -n {length}"
+        cmd += f' -n {length}'
     if reverse:
-        cmd += " -r"
+        cmd += ' -r'
     if since:
         # since can be used with '+' and '-', see man journalctl
-        cmd += f" -S {since}"
+        cmd += f' -S {since}'
     if options:
-        cmd += " " + " ".join(options)
+        cmd += ' ' + ' '.join(options)
 
     if grep:
         cmd += f" | grep '{grep}'"
 
-    ret, journal = run_ret_out(cmd, return_output=return_output, verbose=verbose)
+    ret, journal = run_ret_out(cmd, return_output=return_output)
     if ret:
-        print(f"FAIL: cmd '{cmd}' failed with retcode {ret}.")
+        logging.error(f"cmd '{cmd}' failed with retcode {ret}.")
         return None
     if not return_output:
         return ret
 
     # shorten the hostname to match /var/log/messages format
-    data = ""
+    data = ''
     for line in journal.splitlines():
         line = line.split()  # noqa: PLW2901
         if len(line) < 4:
             continue
-        line[3] = line[3].split(".")[0]
-        data += " ".join(line) + "\n"
+        line[3] = line[3].split('.')[0]
+        data += ' '.join(line) + '\n'
     return ret, data
 
 
 def edit_config(
     file: str,
     parameters: dict,
     update: bool = False,
@@ -1410,15 +1381,15 @@
         config = ConfigObj(file, file_error=file_error, list_values=list_values)
     except OSError as e:
         print(e)
         return False
 
     config.filename = file
 
-    print(f"INFO: Updating {file}")
+    logging.info(f'Updating {file}')
     if update:
         config.update(parameters)
     else:
         config.merge(parameters)
 
     config.write()
     return True
@@ -1432,74 +1403,74 @@
       parameters_to_remove: (list) Parameters to remove.
       section: (str) Specify section of config file parameters are nested in.
       warn: (bool) Set False to supress warning when deleting nonexistent parameter.
     """
     try:
         config = ConfigObj(file, file_error=True)
     except OSError as e:
-        print("FAIL: Unable to open {}. It might not exist")
+        logging.exception('Unable to open {}. It might not exist')
         print(e)
         return False
 
     config.filename = file
     fail = False
     try:
         for param in parameters_to_remove:
             print(f'INFO: Removing "{param}" from {file}')
             if section:
                 config[section].pop(param)
             else:
                 config.pop(param)
     except KeyError:
         if warn:
-            print("WARN: Parameter to remove is not in config")
+            logging.warning('Parameter to remove is not in config')
         fail = True
 
     config.write()
     if fail:
         return False
     return True
 
 
-def generate_sosreport(skip_plugins=None, plugin_timeout=300, timeout=900):  # noqa: ANN001, ANN201
+def generate_sosreport(skip_plugins=None, plugin_timeout=300):  # noqa: ANN001, ANN201
     """Generates a sos report.
 
     Args:
       skip_plugins: (string) comma separated list of plugins to skip (no space after comma)
       plugin_timeout: (int) timeout in seconds to allow each plugin to run for (only applicable to rhel-8+)
       timeout: (int) timeout for the sosreport proces in seconds. Use `None` for no timeout.
     """
-    cmd = f"sos report --batch --plugin-timeout {plugin_timeout}"
+    cmd = f'sos report --batch --plugin-timeout {plugin_timeout}'
     dist = dist_ver()
     if dist < 8:
-        cmd = "sosreport --batch"
+        cmd = 'sosreport --batch'
 
-    if not install_package("sos", check=True):
-        print("FAIL: unable to install sos package")
+    if not install_package('sos', check=True):
+        logging.error('unable to install sos package')
         return False
 
     mount_flag = False
-    if is_mounted("/var/crash"):
-        print("INFO: Unmounting /var/crash to avoid sosreport being hang there")
-        umount("/var/crash")
+    if is_mounted('/var/crash'):
+        logging.info('Unmounting /var/crash to avoid sosreport being hang there')
+        umount('/var/crash')
         mount_flag = True
 
     if skip_plugins:
-        cmd = cmd + f" --skip-plugins {skip_plugins}"
+        cmd = cmd + f' --skip-plugins {skip_plugins}'
 
-    ret_code, sosreport_ret = run_ret_out(cmd, return_output=True, timeout=timeout)
+    ret_code, sosreport_ret = run_ret_out(cmd, return_output=True)
     if ret_code != 0:
-        print("FAIL: sosreport command failed")
+        logging.error('sosreport command failed')
         if mount_flag:
-            mount("/var/crash")
+            mount('/var/crash')
         return False
 
     sos_report = None
-    for line in sosreport_ret.split("\n"):
-        if "/tmp/sosreport" in line:
+    for line in sosreport_ret.split('\n'):
+        if '/tmp/sosreport' in line:
             sos_report = line.strip()
             break
 
     if mount_flag:
-        mount("/var/crash")
+        mount('/var/crash')
 
     return sos_report
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/lio.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/lio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 """lio.py: Module to manipulate LIO target (using targetcli)."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
-import re  # regex
+import logging
+import re
 
 from sts import fc, linux
 from sts.utils.cmdline import run, run_ret_out
 
-regex_tgtcli_wwpn = "naa.\\S+"
+regex_tgtcli_wwpn = 'naa.\\S+'
 
 
 def _tgt_wwn_2_wwn(wwn):  # noqa: ANN001, ANN202
     """On RHEL-6 targetcli stores WWN on WWN format,
     but on RHEL-7 it is something like: naa.200090e2baa397ca
     The arguments are:
     None
     Returns:
     String: WWN as: 20:00:90:e2:ba:a3:97:ca.
     """
     # Converting Targetcli wwpn format to common format
-    if linux.dist_name() == "RHEL" and linux.dist_ver() < 7:
+    if linux.dist_name() == 'RHEL' and linux.dist_ver() < 7:
         return wwn
 
-    wwn_regex = r"naa\."
-    wwn = re.sub(wwn_regex, "", wwn)
+    wwn_regex = r'naa\.'
+    wwn = re.sub(wwn_regex, '', wwn)
     # append ":" after every 2nd character
-    wwn = re.sub(r"(\S{2})", r"\1:", wwn)
+    wwn = re.sub(r'(\S{2})', r'\1:', wwn)
     # remove trail :
-    return re.sub(":$", "", wwn)
+    return re.sub(':$', '', wwn)
 
 
 def _wwn_2_tgt_wwn(wwn) -> str:  # noqa: ANN001
     """On RHEL-6 targetcli stores WWN on WWN format,
     but on RHEL-7 it is something like: naa.200090e2baa397ca
     The arguments are:
     WWN:      20:00:90:e2:ba:a3:97:ca
     Returns:
     String: target WWN format as: naa.200090e2baa397ca.
     """
     # Converting Targetcli wwpn format to common format
-    if linux.dist_name() == "RHEL" and linux.dist_ver() < 7:
+    if linux.dist_name() == 'RHEL' and linux.dist_ver() < 7:
         return wwn
 
     # remove all ':'
-    wwn = re.sub(":", "", wwn)
+    wwn = re.sub(':', '', wwn)
     # append "naa." after every 2nd character
-    return "naa." + wwn
+    return 'naa.' + wwn
 
 
 def lio_query(show_output=False):  # noqa: ANN001, ANN201
     """Query all information from targetcli using targetcli ls
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with targetcli information.
     """
-    cmd = "targetcli ls"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = 'targetcli ls'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Could not run targetcli")
+        logging.error('Could not run targetcli')
         return None
-    lio_data = output.split("\n")
+    lio_data = output.split('\n')
 
-    lio_field_regex = re.compile(r"o-\s(.*?)\s.*\[(.*)\]")
+    lio_field_regex = re.compile(r'o-\s(.*?)\s.*\[(.*)\]')
     # supported types for LIO
-    lio_supported_types = ("backstores", "iscsi", "loopback", "tcm_fc")
+    lio_supported_types = ('backstores', 'iscsi', 'loopback', 'tcm_fc')
     lio_supported_backstores = (
-        "block",
-        "fileio",
-        "pscsi",
-        "ramdisk",
-        "user:qcow",
-        "user:rbd",
-        "user:zbc",
+        'block',
+        'fileio',
+        'pscsi',
+        'ramdisk',
+        'user:qcow',
+        'user:rbd',
+        'user:zbc',
     )
 
     lio_dict = {}
     data_type = None
 
     bs_type_dict = {}
 
@@ -100,211 +101,211 @@
     tcm_fc_processing_acls = False
     tcm_fc_processing_luns = False
 
     for data in lio_data:
         m = lio_field_regex.search(data)
         if not m:
             # Just ignore entry we can't parse
-            # print("FAIL: (%s) does not match LIO field format" % data)
+            # logging.error("(%s) does not match LIO field format" % data)
             continue
         entry = m.group(1)
         entry_details = m.group(2)
 
-        if entry == "/":
+        if entry == '/':
             # Skip root
             continue
 
         # print "INFO: LIO field %s" % entry
         if entry in lio_supported_types:
             data_type = entry
             # bs_type_dict = {}
             lio_dict[data_type] = {}
             continue
         if not data_type:
-            print(f"FATAL: {entry} is does not belong to any supported data type")
+            logging.critical(f'{entry} is does not belong to any supported data type')
             continue
         # print "INFO: %s is subitem of %s" % (entry, data_type)
         # ################# PROCESSING BACKSTORES data type ####################
-        if data_type == "backstores":
+        if data_type == 'backstores':
             if entry in lio_supported_backstores:
                 # print "INFO: Processing backstores %s subtiems" % entry
                 bs_type = entry
                 bs_type_dict[bs_type] = {}
                 lio_dict[data_type] = bs_type_dict
                 continue
-            if entry == "alua" or entry == "default_tg_pt_gp":
+            if entry == 'alua' or entry == 'default_tg_pt_gp':
                 continue
-            details_regex = re.compile(r"(.*)\s+\((\S+)\)\s+(\S+)\s+(\S+)")
+            details_regex = re.compile(r'(.*)\s+\((\S+)\)\s+(\S+)\s+(\S+)')
             details_dict = {}
             m = details_regex.search(entry_details)
             if m:
-                details_dict["file_path"] = m.group(1)
-                details_dict["lun_size"] = m.group(2)
+                details_dict['file_path'] = m.group(1)
+                details_dict['lun_size'] = m.group(2)
             details_dict.update(lio_get_backstore_lun_details(bs_type, entry))
-            if "wwn" in list(details_dict.keys()):
-                details_dict["wwid"] = _lun_wwn2wwid(details_dict["wwn"])
+            if 'wwn' in list(details_dict.keys()):
+                details_dict['wwid'] = _lun_wwn2wwid(details_dict['wwn'])
             # print "BRUNO DEBUG backstore %s (%s)" % (entry, entry_details)
             bs_type_dict[bs_type][entry] = details_dict
             lio_dict[data_type] = bs_type_dict
 
         # ################# PROCESSING iSCSI data type ####################
-        if data_type == "iscsi":
-            iqn_regex = re.compile(r"iqn\..*")
+        if data_type == 'iscsi':
+            iqn_regex = re.compile(r'iqn\..*')
             if iqn_regex.match(entry) and not iscsi_processing_acls:
                 # print "INFO: Processing tcm_fc %s subtiems" % entry
                 iscsi_tgt_iqn = entry
                 # The target wwn is a dict key
                 iscsi_dict[iscsi_tgt_iqn] = {}
                 lio_dict[data_type] = iscsi_dict
                 continue
-            tpg_regex = re.compile(r"(tpg\d+)")
+            tpg_regex = re.compile(r'(tpg\d+)')
             m = tpg_regex.match(entry)
             if m:
                 # print "INFO: Processing tcm_fc %s subtiems" % entry
                 current_tpg = m.group(1)
                 # The target wwn is a dict key
                 iscsi_dict[iscsi_tgt_iqn][current_tpg] = {}
                 iscsi_acls_dict = {}
                 iscsi_luns = []
                 iscsi_portals = []
                 lio_dict[data_type] = iscsi_dict
                 continue
 
-            if entry == "acls":
-                iscsi_dict[iscsi_tgt_iqn][current_tpg]["acls"] = {}
+            if entry == 'acls':
+                iscsi_dict[iscsi_tgt_iqn][current_tpg]['acls'] = {}
                 iscsi_processing_acls = True
                 iscsi_processing_luns = False
                 iscsi_processing_portals = False
-            if entry == "luns":
-                iscsi_dict[iscsi_tgt_iqn][current_tpg]["luns"] = {}
+            if entry == 'luns':
+                iscsi_dict[iscsi_tgt_iqn][current_tpg]['luns'] = {}
                 iscsi_processing_acls = False
                 iscsi_processing_luns = True
                 iscsi_processing_portals = False
                 continue
-            if entry == "portals":
-                iscsi_dict[iscsi_tgt_iqn][current_tpg]["portals"] = {}
+            if entry == 'portals':
+                iscsi_dict[iscsi_tgt_iqn][current_tpg]['portals'] = {}
                 iscsi_processing_acls = False
                 iscsi_processing_luns = False
                 iscsi_processing_portals = True
                 continue
             # ################# PROCESSING ACLS ####################
             # If we are processing ACLs entry
             if iscsi_processing_acls:
                 # print "BRUNO ISCSI ACL init (%s)" % entry
                 if iqn_regex.match(entry):
                     iscsi_init_iqn = entry
                     iscsi_acls_dict[iscsi_init_iqn] = []
-                    iscsi_dict[iscsi_tgt_iqn][current_tpg]["acls"] = iscsi_acls_dict
+                    iscsi_dict[iscsi_tgt_iqn][current_tpg]['acls'] = iscsi_acls_dict
                     lio_dict[data_type] = iscsi_dict
                     continue
-                map_regex = re.compile(r"mapped_(lun.*)$")
+                map_regex = re.compile(r'mapped_(lun.*)$')
                 # Check if it is lun mapping information
                 m = map_regex.match(entry)
                 if m:
                     # print "INFO: found mapped lun: %s" % m.group(1)
                     iscsi_acls_dict[iscsi_init_iqn].append(m.group(1))
-                    iscsi_dict[iscsi_tgt_iqn][current_tpg]["acls"] = iscsi_acls_dict
+                    iscsi_dict[iscsi_tgt_iqn][current_tpg]['acls'] = iscsi_acls_dict
                 lio_dict[data_type] = iscsi_dict
 
             # ################# PROCESSING LUNs ####################
             # If we are processing LUNs entry
             if iscsi_processing_luns:
                 iscsi_luns.append(entry)
-                iscsi_dict[iscsi_tgt_iqn][current_tpg]["luns"] = iscsi_luns
+                iscsi_dict[iscsi_tgt_iqn][current_tpg]['luns'] = iscsi_luns
                 lio_dict[data_type] = iscsi_dict
                 continue
             # ################# PROCESSING Portlas ####################
             # If we are processing Portals entry
             if iscsi_processing_portals:
                 iscsi_portals.append(entry)
-                iscsi_dict[iscsi_tgt_iqn][current_tpg]["portals"] = iscsi_portals
+                iscsi_dict[iscsi_tgt_iqn][current_tpg]['portals'] = iscsi_portals
                 lio_dict[data_type] = iscsi_dict
                 continue
 
         # ################# PROCESSING TCM_FC data type ####################
 
-        if data_type == "tcm_fc":
+        if data_type == 'tcm_fc':
             # if tcm_fc_processing_luns is true, it is because we reached the end
             # of host wwn, and now we are probably processing next host wwn
             # so do not test it on the if below
             tmp_entry = _tgt_wwn_2_wwn(entry)
             if fc.is_wwn(tmp_entry) and not tcm_fc_processing_acls:
                 # print "INFO: Processing tcm_fc %s subtiems" % tmp_entry
                 tcm_fc_wwn = tmp_entry
                 # The target wwn is a dict key
                 tcm_fc_dict[tcm_fc_wwn] = {}
                 tcm_fc_processing_acls = False
                 tcm_fc_processing_luns = False
                 lio_dict[data_type] = tcm_fc_dict
                 continue
 
-            if entry == "acls":
+            if entry == 'acls':
                 tcm_fc_acls_dict = {}
-                tcm_fc_dict[tcm_fc_wwn]["acls"] = {}
+                tcm_fc_dict[tcm_fc_wwn]['acls'] = {}
                 tcm_fc_processing_acls = True
                 tcm_fc_processing_luns = False
                 continue
-            if entry == "luns":
+            if entry == 'luns':
                 tcm_fc_luns = {}
-                tcm_fc_dict[tcm_fc_wwn]["luns"] = {}
+                tcm_fc_dict[tcm_fc_wwn]['luns'] = {}
                 tcm_fc_processing_luns = True
                 tcm_fc_processing_acls = False
                 continue
             # ################# PROCESSING ACLS ####################
             # If we are processing ACLs entry
             if tcm_fc_processing_acls:
                 # It can be initiator, but be using tag instead of wwn
                 # TODO: lio_is_fc_tag causes the whole query command to be slow
                 # need to find a better way to do it
                 tmp_entry = _tgt_wwn_2_wwn(entry)
                 if fc.is_wwn(tmp_entry) or lio_is_fc_tag(tcm_fc_wwn, entry):
                     tcm_fc_init_wwn = tmp_entry
                     tcm_fc_acls_dict[tcm_fc_init_wwn] = {}
-                    tcm_fc_dict[tcm_fc_wwn]["acls"] = tcm_fc_acls_dict
+                    tcm_fc_dict[tcm_fc_wwn]['acls'] = tcm_fc_acls_dict
                     continue
-                map_regex = re.compile(r"mapped_(lun.*)$")
+                map_regex = re.compile(r'mapped_(lun.*)$')
                 # Check if it is lun mapping information
                 m = map_regex.match(entry)
                 if m:
-                    t_lun_id_regex = re.compile(r"(lun\d+)\s(\S+)/(\S+)")
+                    t_lun_id_regex = re.compile(r'(lun\d+)\s(\S+)/(\S+)')
                     t = t_lun_id_regex.match(entry_details)
                     if t:
                         # print "INFO: found mapped lun: %s" % m.group(1)
                         # print "INFO: entry_details %s" % entry_details
                         tcm_fc_acls_dict[tcm_fc_init_wwn][t.group(1)] = m.group(1)
-                        tcm_fc_dict[tcm_fc_wwn]["acls"] = tcm_fc_acls_dict
+                        tcm_fc_dict[tcm_fc_wwn]['acls'] = tcm_fc_acls_dict
                         # Update mapping info on backstore session
                         bs_type = t.group(2)
                         lun_name = t.group(3)
                         # print "INFO: tcm_fc acls: bs_type %s lun_name %s is mapped to %s/%s" %
                         # (bs_type, lun_name, tcm_fc_wwn, tcm_fc_init_wwn)
-                        details_dict = lio_dict["backstores"][bs_type][lun_name]
+                        details_dict = lio_dict['backstores'][bs_type][lun_name]
                         mapping_dict = {
-                            "t_wwpn": tcm_fc_wwn,
-                            "h_wwpn": tcm_fc_init_wwn,
-                            "t_lun_id": t.group(1),
-                            "h_lun_id": m.group(1),
+                            't_wwpn': tcm_fc_wwn,
+                            'h_wwpn': tcm_fc_init_wwn,
+                            't_lun_id': t.group(1),
+                            'h_lun_id': m.group(1),
                         }
-                        if "mapping" not in list(details_dict.keys()):
-                            details_dict["mapping"] = []
-                        details_dict["mapping"].append(mapping_dict)
+                        if 'mapping' not in list(details_dict.keys()):
+                            details_dict['mapping'] = []
+                        details_dict['mapping'].append(mapping_dict)
 
             # ################# PROCESSING LUNS that are added to target wwn ####################
             # If we are processing LUNs entry
             if tcm_fc_processing_luns:
-                t_lun_info_regex = re.compile(r"(\S+)/(\S+)\s.*")
+                t_lun_info_regex = re.compile(r'(\S+)/(\S+)\s.*')
                 t = t_lun_info_regex.match(entry_details)
                 # print "INFO: entry_details tcm_fc luns %s" % entry_details
                 if t:
                     # print "INFO: found mapped lun: %s" % m.group(1)
                     # print "INFO: entry_details %s" % entry_details
                     tcm_fc_luns[entry] = {}
-                    tcm_fc_luns[entry]["bs_type"] = t.group(1)
-                    tcm_fc_luns[entry]["lun_name"] = t.group(2)
-                tcm_fc_dict[tcm_fc_wwn]["luns"] = tcm_fc_luns
+                    tcm_fc_luns[entry]['bs_type'] = t.group(1)
+                    tcm_fc_luns[entry]['lun_name'] = t.group(2)
+                tcm_fc_dict[tcm_fc_wwn]['luns'] = tcm_fc_luns
 
             lio_dict[data_type] = tcm_fc_dict
 
     if show_output:
         print(lio_dict)
     return lio_dict
 
@@ -317,29 +318,29 @@
     The arguments are:
     None
     Returns:
     True: Device was created
     False: There was some problem.
     """
     created = False
-    if bs_type == "block":
+    if bs_type == 'block':
         created = _lio_create_backstore_block(lun_name, device_name)
 
-    if bs_type == "fileio":
+    if bs_type == 'fileio':
         created = _lio_create_backstore_fileio(lun_name, lun_size=lun_size)
 
-    if bs_type == "pscsi":
+    if bs_type == 'pscsi':
         created = _lio_create_backstore_pscsi(lun_name, device_name)
 
     if not created:
-        print(f"FAIL: Could not create lun using ({bs_type}) on lio_create_backstore")
+        logging.error(f'Could not create lun using ({bs_type}) on lio_create_backstore')
         return False
 
     if lun_name not in list(lio_get_backstores(bs_type).keys()):
-        print(f"FAIL: It seems {lun_name} was created, but it was not")
+        logging.error(f'It seems {lun_name} was created, but it was not')
         return False
 
     return True
 
 
 def lio_get_backstores(bs_type=None, lio_dict=None):  # noqa: ANN001, ANN201
     """Return a dict with all backstores. If a backstore type
@@ -352,66 +353,66 @@
     Dict: if there are devices and backstore type was provided
     Dict
     Dict: All backstore devices.
     """
     if not lio_dict:
         lio_dict = lio_query()
 
-    if "backstores" not in list(lio_dict.keys()):
-        print("FAIL: there is not backstore defined on targetcli")
+    if 'backstores' not in list(lio_dict.keys()):
+        logging.error('there is not backstore defined on targetcli')
         print(lio_dict)
         return None
 
     if not bs_type:
-        return lio_dict["backstores"]
+        return lio_dict['backstores']
 
-    if bs_type not in list(lio_dict["backstores"].keys()):
+    if bs_type not in list(lio_dict['backstores'].keys()):
         return None
 
-    return lio_dict["backstores"][bs_type]
+    return lio_dict['backstores'][bs_type]
 
 
 def lio_get_backstore_details(bs_type, lun_name, lio_dict=None):  # noqa: ANN001, ANN201
     """Get the size of specific Backstore device
     Returns:
     Dic:      Detailed information about this device
     None:     If something went wrong.
     """
     bs_dict = lio_get_backstores(bs_type, lio_dict=lio_dict)
     if not bs_dict:
         return None
 
     if lun_name not in list(bs_dict.keys()):
-        print(f"FAIL: {lun_name} is not defined on {bs_type}")
+        logging.error(f'{lun_name} is not defined on {bs_type}')
         lio_dict = lio_query()
         print(lio_dict)
         return None
 
     return bs_dict[lun_name]
 
 
 def lio_get_backstore_lun_details(bs_type, lun_name):  # noqa: ANN001, ANN201
     """Get the detailed information about the lun."""
     if not bs_type or not lun_name:
-        print("FAIL: lio_get_backstore_lun_details() - requires bs_type and lun_name")
+        logging.error('lio_get_backstore_lun_details() - requires bs_type and lun_name')
         return None
 
-    cmd = f"targetcli /backstores/{bs_type}/{lun_name} info"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'targetcli /backstores/{bs_type}/{lun_name} info'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Could not get {bs_type} details for {lun_name}")
+        logging.error(f'Could not get {bs_type} details for {lun_name}')
         return None
 
-    details = output.split("\n")
+    details = output.split('\n')
     supported_details = {
-        "dev": r"^dev: (\S+)",
-        "name": r"^name: (\S+)",
-        "size_bytes": r"^size: (\S+)",
-        "write_back": r"^write_back: (\S+)",
-        "wwn": r"^wwn: (\S+)",
+        'dev': r'^dev: (\S+)',
+        'name': r'^name: (\S+)',
+        'size_bytes': r'^size: (\S+)',
+        'write_back': r'^write_back: (\S+)',
+        'wwn': r'^wwn: (\S+)',
     }
 
     lun_details = {}
     for info in details:
         for sup_detail in supported_details:
             m = re.match(supported_details[sup_detail], info)
             if m:
@@ -419,142 +420,142 @@
 
     return lun_details
 
 
 def _lun_wwn2wwid(wwn):  # noqa: ANN001, ANN202
     """From the LUN WWN is possible to get WWID."""
     wwid = wwn
-    wwid = wwid.replace("-", "")
+    wwid = wwid.replace('-', '')
     # Just the first 26 bytes are the wwid
     wwid = wwid[:25]
-    return "36001405" + wwid
+    return '36001405' + wwid
 
 
 def lio_delete_backstore(bs_type=None, lun_name=None):  # noqa: ANN001, ANN201
     """Delete backstore device
     The arguments are:
     Backstore type
     LUN name
     Returns:
     True: Device was deleted
     False: There was some problem.
     """
     deleted = False
-    if bs_type == "block":
+    if bs_type == 'block':
         deleted = _lio_delete_backstore_block(lun_name)
 
-    if bs_type == "fileio":
+    if bs_type == 'fileio':
         deleted = _lio_delete_backstore_fileio(lun_name)
 
-    if bs_type == "pscsi":
+    if bs_type == 'pscsi':
         deleted = _lio_delete_backstore_pscsi(lun_name)
 
     if not deleted:
-        print(f"FAIL: Could not delete lun using ({bs_type}) on lio_create_backstore")
+        logging.error(f'Could not delete lun using ({bs_type}) on lio_create_backstore')
         return False
 
     if lun_name in list(lio_get_backstores(bs_type).keys()):
-        print(f"FAIL: It seems {lun_name} was deleted, but it was not")
+        logging.error(f'It seems {lun_name} was deleted, but it was not')
         return False
 
     return True
 
 
 # ## BLOCK ###
 def _lio_create_backstore_block(lun_name, device):  # noqa: ANN001, ANN202
     if not lun_name:
-        print("FAIL: _lio_create_backstore_block needs lun_name parameter")
+        logging.error('_lio_create_backstore_block needs lun_name parameter')
         return False
     if not device:
-        print("FAIL: _lio_create_backstore_block needs device parameter")
+        logging.error('_lio_create_backstore_block needs device parameter')
         return False
 
-    cmd = f"targetcli /backstores/block create {lun_name} {device}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: Could not create block {lun_name}")
+    cmd = f'targetcli /backstores/block create {lun_name} {device}'
+    if run(cmd).rc != 0:
+        logging.error(f'Could not create block {lun_name}')
         return False
     return True
 
 
 def _lio_delete_backstore_block(lun_name):  # noqa: ANN001, ANN202
-    cmd = f"targetcli /backstores/block delete {lun_name}"
-    if run(cmd).returncode != 0:
-        print(f"FAIL: Could not delete block {lun_name}")
+    cmd = f'targetcli /backstores/block delete {lun_name}'
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete block {lun_name}')
         return False
 
     return True
 
 
 # ## FILEIO ###
 def _lio_create_backstore_fileio(lun_name, file_name=None, lun_size=None):  # noqa: ANN001, ANN202
     if not lun_name:
-        print("_lio_create_backstore_fileio() - requires lun_name parameter")
+        print('_lio_create_backstore_fileio() - requires lun_name parameter')
         return False
 
     if not file_name:
         # Set default backend file name
-        file_name = f"{lun_name}.img"
+        file_name = f'{lun_name}.img'
 
     # disable spare, to force targetcli to allocate the whole file to avoid problem
     # of running out of disk space and not have enough space to store data
-    cmd = f"targetcli /backstores/fileio create {lun_name} {file_name} sparse=false"
+    cmd = f'targetcli /backstores/fileio create {lun_name} {file_name} sparse=false'
     if lun_size:
-        cmd = cmd + f" {lun_size}"
+        cmd = cmd + f' {lun_size}'
 
-    if run(cmd).returncode != 0:
-        print(f"FAIL: Could not create fileio {lun_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not create fileio {lun_name}')
         return False
     return True
 
 
 def _lio_delete_backstore_fileio(lun_name):  # noqa: ANN001, ANN202
     file_name = _lio_get_backstore_fileio_file(lun_name)
 
-    if run(f"targetcli /backstores/fileio delete {lun_name}").returncode != 0:
-        print(f"FAIL: Could not delete fileio {lun_name}")
+    if run(f'targetcli /backstores/fileio delete {lun_name}').rc != 0:
+        logging.error(f'Could not delete fileio {lun_name}')
         return False
 
-    if file_name and run(f"rm -f {file_name}").returncode != 0:
-        print(f"WARN: could not delete file {file_name}")
+    if file_name and run(f'rm -f {file_name}').rc != 0:
+        logging.warning(f'could not delete file {file_name}')
 
     return True
 
 
 def _lio_get_backstore_fileio_file(lun_name):  # noqa: ANN001, ANN202
     """Get the file used by a specific LUN."""
-    cmd = f"targetcli /backstores/fileio/{lun_name} ls"
-    completed_process = run(cmd, capture_output=True, verbose=False)
-    if completed_process.returncode != 0:
-        print(f"FAIL: Could not get fileio file {lun_name}")
+    cmd = f'targetcli /backstores/fileio/{lun_name} ls'
+    completed_process = run(cmd)
+    if completed_process.rc != 0:
+        logging.error(f'Could not get fileio file {lun_name}')
         return None
 
-    path_regex = re.compile(r"\[(.*)\s\(")
-    m = path_regex.search(completed_process.output)
+    path_regex = re.compile(r'\[(.*)\s\(')
+    m = path_regex.search(completed_process.stdout)
     if m:
         return m.group(1)
     return None
 
 
 # ## PSCSI ###
 def _lio_create_backstore_pscsi(lun_name, device, lun_size=None):  # noqa: ANN001, ANN202
-    cmd = f"targetcli /backstores/pscsi create {lun_name} {device}"
+    cmd = f'targetcli /backstores/pscsi create {lun_name} {device}'
     if lun_size:
-        cmd = cmd + f" {lun_size}M"
+        cmd = cmd + f' {lun_size}M'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not create pscsi {lun_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not create pscsi {lun_name}')
         return False
     return True
 
 
 def _lio_delete_backstore_pscsi(lun_name):  # noqa: ANN001, ANN202
-    cmd = f"targetcli /backstores/pscsi delete {lun_name}"
+    cmd = f'targetcli /backstores/pscsi delete {lun_name}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete pscsi {lun_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete pscsi {lun_name}')
         return False
 
     return True
 
 
 ##################################################
 # ################# iSCSI ########################
@@ -565,15 +566,15 @@
     None
     Returns:
     True: Host supports iscsi
     False: Host does not support iscsi.
     """
     lio_dict = lio_query()
 
-    if "iscsi" not in list(lio_dict.keys()):
+    if 'iscsi' not in list(lio_dict.keys()):
         # Host does not support iSCSI target
         return False
     return True
 
 
 # ## iSCSI target ###
 def lio_iscsi_create_target(iqn):  # noqa: ANN001, ANN201
@@ -581,39 +582,39 @@
     The arguments are:
     iqn:     Target IQN
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     if not lio_support_iscsi_target():
-        print("FAIL: server does not support iSCSI target")
+        logging.error('server does not support iSCSI target')
         return False
 
-    cmd = f"targetcli /iscsi/ create {iqn}"
+    cmd = f'targetcli /iscsi/ create {iqn}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not create iSCSI target {iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not create iSCSI target {iqn}')
         return False
 
     if iqn not in lio_iscsi_get_target():
-        print("FAIL: It seems to have added iSCSI target, but it did not")
+        logging.error('It seems to have added iSCSI target, but it did not')
         lio_dict = lio_query()
-        print(lio_dict["iscsi"])
+        print(lio_dict['iscsi'])
         return False
     # targetcli by default enable only IPv$ connection
     # we want also IPv6
-    if not lio_iscsi_delete_target_portal(iqn, "tpg1", "0.0.0.0"):
-        print("FAIL: could not remove default iSCSI target portal")
+    if not lio_iscsi_delete_target_portal(iqn, 'tpg1', '0.0.0.0'):
+        logging.error('could not remove default iSCSI target portal')
         lio_dict = lio_query()
-        print(lio_dict["iscsi"])
+        print(lio_dict['iscsi'])
 
-    if not lio_iscsi_create_target_portal(iqn, "tpg1", "::0"):
-        print("FAIL: could not create IPv6 iSCSI target portal")
+    if not lio_iscsi_create_target_portal(iqn, 'tpg1', '::0'):
+        logging.error('could not create IPv6 iSCSI target portal')
         lio_dict = lio_query()
-        print(lio_dict["iscsi"])
+        print(lio_dict['iscsi'])
     return True
 
 
 def lio_iscsi_get_target():  # noqa: ANN201
     """Return a list of all iSCSI targets configured
     The arguments are:
     None
@@ -622,15 +623,15 @@
     """
     lio_dict = lio_query()
 
     if not lio_support_iscsi_target():
         # Host does not support iSCSI target
         return None
 
-    return list(lio_dict["iscsi"].keys())
+    return list(lio_dict['iscsi'].keys())
 
 
 def lio_iscsi_target_set_parameter(tgt_iqn, tpg, group, attr_name, attr_value):  # noqa: ANN001, ANN201
     """Set a parameter to an iSCSI target
     if tgt_iqn is not set, set it globally
     The arguments are:
     tgt_iqn       HOST IQN
@@ -638,20 +639,20 @@
     group         eg: attribute, parameter, discovery_auth...
     attr_name     Attribute name
     attr_value    Attribute value
     Returns:
     True: If target is attribute is set
     False: If some problem happened.
     """
-    cmd = f"targetcli /iscsi set {group} {attr_name}={attr_value}"
+    cmd = f'targetcli /iscsi set {group} {attr_name}={attr_value}'
     if tgt_iqn:
-        cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/ set {group} {attr_name}={attr_value}"
+        cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/ set {group} {attr_name}={attr_value}'
 
-    if run(cmd).returncode != 0:
-        print(f"FAIL: Could not set iSCSI target attribute {attr_name}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not set iSCSI target attribute {attr_name}')
         return False
     return True
 
 
 # ## iSCSI ACLS ###
 def lio_iscsi_create_acl(tgt_iqn, tpg, init_iqn):  # noqa: ANN001, ANN201
     """Add an initiator IQN to target IQN
@@ -659,36 +660,36 @@
     tgt_iqn:     Host IQN
     tpg:         Target Portal Group
     init_iqn:    Initiator IQN
     Returns:
     True: If init IQN is created
     False: If some problem happened.
     """
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls create {init_iqn} add_mapped_luns=false"
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/acls create {init_iqn} add_mapped_luns=false'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not add iSCSI initiator {init_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not add iSCSI initiator {init_iqn}')
         return False
     return True
 
 
 def lio_iscsi_delete_acl(tgt_iqn, tpg, init_iqn):  # noqa: ANN001, ANN201
     """Remove an initiator IQN from target IQN
     The arguments are:
     tgt_iqn:     Host IQN
     tpg:         Target Portal Group
     init_iqn:    Initiator IQN
     Returns:
     True: If init iqn is removed
     False: If some problem happened.
     """
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls delete {init_iqn}"
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/acls delete {init_iqn}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete iSCSI initiator {init_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete iSCSI initiator {init_iqn}')
         return False
 
     return True
 
 
 # ## iSCSI LUNs ###
 def lio_iscsi_add_lun(tgt_iqn, tpg, bs_type, lun_name):  # noqa: ANN001, ANN201
@@ -698,23 +699,18 @@
     tpg:          Target Portal Group
     bs_type:      Backstore type
     lun_name:     Lun Name
     Returns:
     True: If LUN is added
     False: If some problem happened.
     """
-    cmd = "targetcli /iscsi/{}/{}/luns create /backstores/{}/{} add_mapped_luns=false".format(
-        tgt_iqn,
-        tpg,
-        bs_type,
-        lun_name,
-    )
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/luns create /backstores/{bs_type}/{lun_name} add_mapped_luns=false'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not add lun to iSCSI target {tgt_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not add lun to iSCSI target {tgt_iqn}')
         return False
 
     return True
 
 
 def lio_iscsi_remove_lun(tgt_iqn, tpg, lun_id):  # noqa: ANN001, ANN201
     """Remove a LUN target IQN
@@ -722,99 +718,99 @@
     tgt_iqn:     Target IQN
     tpg:         Target Portal Group
     lun_id:      Lun id
     Returns:
     True: If LUN is removed
     False: If some problem happened.
     """
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/luns delete {lun_id}"
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/luns delete {lun_id}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete LUN from iSCSI target {tgt_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete LUN from iSCSI target {tgt_iqn}')
         return False
 
     return True
 
 
 def lio_iscsi_get_luns(tgt_iqn, tpg):  # noqa: ANN001, ANN201
     """Return a list with all LUNs added to an iSCSI target.
     The arguments are:
     None
     Returns:
     List: list of luns
     None if something went wrong.
     """
     if tgt_iqn not in lio_iscsi_get_target():
-        print(f"FAIL: {tgt_iqn} is not defined on targetcli")
+        logging.error(f'{tgt_iqn} is not defined on targetcli')
         return None
 
     lio_dict = lio_query()
-    if "luns" not in list(lio_dict["iscsi"][tgt_iqn].keys()):
-        print("INFO: target %s does not have any LUN\n")
+    if 'luns' not in list(lio_dict['iscsi'][tgt_iqn].keys()):
+        logging.info('target %s does not have any LUN\n')
         return None
 
-    return lio_dict["tcm_fc"][tgt_iqn][tpg]["luns"]
+    return lio_dict['tcm_fc'][tgt_iqn][tpg]['luns']
 
 
 # ## iSCSI Portals ###
-def lio_iscsi_create_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):  # noqa: ANN001, ANN201
+def lio_iscsi_create_target_portal(tgt_iqn, tpg, portal_ip, portal_port='3260'):  # noqa: ANN001, ANN201
     """Remove a Portal target IQN
     The arguments are:
     tgt_iqn:     Target IQN
     tpg:         Target Portal Group
     portal_ip:   IP of host allowed to connect. (0.0.0.0) any IPv4 address
     portal_port  Port to listen for connection, default 3260
     Returns:
     True: If Portal is created
     False: If some problem happened.
     """
     lio_dict = lio_query()
-    if "portals" not in list(lio_dict["iscsi"][tgt_iqn][tpg].keys()):
-        print(f"INFO: target {tgt_iqn} does not have support Portal")
+    if 'portals' not in list(lio_dict['iscsi'][tgt_iqn][tpg].keys()):
+        logging.info(f'target {tgt_iqn} does not have support Portal')
         return False
 
-    portal = portal_ip + ":" + portal_port
-    if portal in lio_dict["iscsi"][tgt_iqn][tpg]["portals"]:
-        print(f"INFO: portal {portal} does already exist on target {tgt_iqn}")
+    portal = portal_ip + ':' + portal_port
+    if portal in lio_dict['iscsi'][tgt_iqn][tpg]['portals']:
+        logging.info(f'portal {portal} does already exist on target {tgt_iqn}')
         return True
 
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/portals create {portal_ip} {portal_port}"
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/portals create {portal_ip} {portal_port}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete Portal from iSCSI target {tgt_iqn}')
         return False
 
     return True
 
 
-def lio_iscsi_delete_target_portal(tgt_iqn, tpg, portal_ip, portal_port="3260"):  # noqa: ANN001, ANN201
+def lio_iscsi_delete_target_portal(tgt_iqn, tpg, portal_ip, portal_port='3260'):  # noqa: ANN001, ANN201
     """Remove a Portal target IQN
     The arguments are:
     tgt_iqn:     Target IQN
     tpg:         Target Portal Group
     portal_ip:   IP of host allowed to connect. (0.0.0.0) any IPv4 address
     portal_port  Port to listen for connection, default 3260
     Returns:
     True: If Portal is removed
     False: If some problem happened.
     """
     lio_dict = lio_query()
-    if "portals" not in list(lio_dict["iscsi"][tgt_iqn][tpg].keys()):
-        print(f"INFO: target {tgt_iqn} does not have support Portal")
+    if 'portals' not in list(lio_dict['iscsi'][tgt_iqn][tpg].keys()):
+        logging.info(f'target {tgt_iqn} does not have support Portal')
         return False
 
-    portal = portal_ip + ":" + portal_port
-    if portal not in lio_dict["iscsi"][tgt_iqn][tpg]["portals"]:
-        print(f"INFO: portal {portal} does not exist on target {tgt_iqn}")
+    portal = portal_ip + ':' + portal_port
+    if portal not in lio_dict['iscsi'][tgt_iqn][tpg]['portals']:
+        logging.info(f'portal {portal} does not exist on target {tgt_iqn}')
         return True
 
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/portals delete {portal_ip} {portal_port}"
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/portals delete {portal_ip} {portal_port}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete Portal from iSCSI target {tgt_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete Portal from iSCSI target {tgt_iqn}')
         return False
     return True
 
 
 # ## iSCSI LUNs mapping ###
 def lio_iscsi_map_lun(tgt_iqn, tpg, init_iqn, init_lun_id, bs_type, lun_name):  # noqa: ANN001, ANN201
     """Map a LUN to target IQN / Initiator IQN
@@ -822,23 +818,23 @@
     tgt_iqn:      Target IQN
     tpg:          Target Portal group
     init_iqn:     Host IQN
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
-    lun_path = f"/backstores/{bs_type}/{lun_name}"
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{tpg}/acls/{init_iqn} create {init_lun_id} {lun_path}"
+    lun_path = f'/backstores/{bs_type}/{lun_name}'
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{tpg}/acls/{init_iqn} create {init_lun_id} {lun_path}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not map lun to iSCSI target {tgt_iqn}/{init_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not map lun to iSCSI target {tgt_iqn}/{init_iqn}')
         return False
 
     if not lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, init_lun_id):
-        print(f"FAIL: It seems to have mapped lun {init_lun_id}, but it did not")
+        logging.error(f'It seems to have mapped lun {init_lun_id}, but it did not')
         return False
 
     return True
 
 
 def lio_iscsi_unmap_lun(tgt_iqn, init_iqn, tpg, init_lun_id):  # noqa: ANN001, ANN201
     """Un map LUN from tgt_wwn/init_wwn
@@ -847,22 +843,22 @@
     init_iqn:     Host IQN
     tpg:          Target Portal group
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is unmapped
     False: If some problem happened.
     """
-    cmd = f"targetcli /iscsi/{tgt_iqn}/{init_iqn}/acls/{tpg} delete {init_lun_id}"
+    cmd = f'targetcli /iscsi/{tgt_iqn}/{init_iqn}/acls/{tpg} delete {init_lun_id}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not unmap LUN from target {tgt_iqn}/{init_iqn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not unmap LUN from target {tgt_iqn}/{init_iqn}')
         return False
 
     if not lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, init_lun_id):
-        print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
+        logging.error(f'It seems to have unmapped lun {init_lun_id}, but it did not')
         return False
     return True
 
 
 def lio_iscsi_get_lun_map(tgt_iqn, init_iqn, tpg, tgt_lun_id):  # noqa: ANN001, ANN201
     """Check if a LUN is mapped to target WWN / Initiator port
     The arguments are:
@@ -870,31 +866,31 @@
     init_iqn:     Host IQN
     tpg:          Target Portal group no.
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
-    cmd = f"targetcli /iscsi/{tgt_iqn}/tpg{tpg}/acls/{init_iqn} ls | grep {tgt_lun_id}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'targetcli /iscsi/{tgt_iqn}/tpg{tpg}/acls/{init_iqn} ls | grep {tgt_lun_id}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Could not get mapping for lun {tgt_lun_id} on iSCSI target {tgt_iqn}/{init_iqn}")
+        logging.error(f'Could not get mapping for lun {tgt_lun_id} on iSCSI target {tgt_iqn}/{init_iqn}')
         return False
 
     if not output:
         return False
     return True
 
 
 def lio_add_iscsi_target(  # noqa: ANN201
     tgt_iqn=None,  # noqa: ANN001
     init_iqn=None,  # noqa: ANN001
-    bs_type="fileio",  # noqa: ANN001
+    bs_type='fileio',  # noqa: ANN001
     lun_name=None,  # noqa: ANN001
-    lun_size="1G",  # noqa: ANN001
+    lun_size='1G',  # noqa: ANN001
     device_name=None,  # noqa: ANN001
     tgt_cnt=1,  # noqa: ANN001
     lun_cnt=1,  # noqa: ANN001
 ):
     """Create new iSCSI target, create LUNs and do LUN mapping
     The arguments are:
     tgt_iqn:          Target IQN, if not specified LIO will create a target IQN
@@ -906,92 +902,92 @@
     tgt_cnt:          Number of targets to create, default: 1
     lun_cnt:          Number of LUNs to create, default: 1
     Returns:
     True: if iSCSI target is created
     False: If some problem happened.
     """
     new_tgt_iqns = []
-    iqn_preffix = "iqn.2009-10.com.redhat:storage-"
+    iqn_preffix = 'iqn.2009-10.com.redhat:storage-'
     # need to create new iSCSI targets, first get the existing targets
     if not tgt_iqn:
         existing_targets = lio_iscsi_get_target()
         iqn_suffix = 0
         # Create new target_iqn names
         while len(new_tgt_iqns) < tgt_cnt:
-            tmp_iqn = "%s%d" % (iqn_preffix, iqn_suffix)
+            tmp_iqn = '%s%d' % (iqn_preffix, iqn_suffix)
             if tmp_iqn not in existing_targets:
                 new_tgt_iqns.append(tmp_iqn)
             iqn_suffix += 1
     else:
         new_tgt_iqns = [tgt_iqn]
 
     for target_iqn in new_tgt_iqns:
         if not lio_iscsi_create_target(target_iqn):
-            print(f"FAIL: Could not create iSCSI target '{target_iqn}'")
+            logging.error(f"Could not create iSCSI target '{target_iqn}'")
             return False
 
-        m = re.match(r"%s(\d+)" % iqn_preffix, target_iqn)
-        tgt_name = "tgt%d" % int(m.group(1)) if m else target_iqn.split(":")[1]
+        m = re.match(r'%s(\d+)' % iqn_preffix, target_iqn)
+        tgt_name = 'tgt%d' % int(m.group(1)) if m else target_iqn.split(':')[1]
 
         for lun_num in range(1, lun_cnt + 1):
-            tgt_lun_name = "%s_lun%d" % (tgt_name, lun_num)
+            tgt_lun_name = '%s_lun%d' % (tgt_name, lun_num)
             # If lun name was passed as argument, try to use it
             if lun_name:
                 tgt_lun_name = lun_name
 
             if not lio_create_backstore(
                 bs_type=bs_type,
                 lun_name=tgt_lun_name,
                 lun_size=lun_size,
                 device_name=device_name,
             ):
-                print("FAIL: Could not create backstore for iSCSI target")
+                logging.error('Could not create backstore for iSCSI target')
                 return False
 
-            tpg = "tpg1"
+            tpg = 'tpg1'
 
             if not lio_iscsi_add_lun(target_iqn, tpg, bs_type, tgt_lun_name):
-                print("FAIL: Could not add LUN to iSCSI target")
+                logging.error('Could not add LUN to iSCSI target')
                 return False
 
             # This is a global setting
-            if not lio_iscsi_target_set_parameter(None, None, "discovery_auth", "enable", "0"):
-                print("FAIL: Could not set Attr to iSCSI target")
+            if not lio_iscsi_target_set_parameter(None, None, 'discovery_auth', 'enable', '0'):
+                logging.error('Could not set Attr to iSCSI target')
                 return False
 
-            if not lio_iscsi_target_set_parameter(target_iqn, tpg, "attribute", "authentication", "0"):
-                print("FAIL: Could not set Attr to iSCSI target")
+            if not lio_iscsi_target_set_parameter(target_iqn, tpg, 'attribute', 'authentication', '0'):
+                logging.error('Could not set Attr to iSCSI target')
                 return False
 
-            if not lio_iscsi_target_set_parameter(target_iqn, tpg, "attribute", "generate_node_acls", "1"):
-                print("FAIL: Could not set Attr to iSCSI target")
+            if not lio_iscsi_target_set_parameter(target_iqn, tpg, 'attribute', 'generate_node_acls', '1'):
+                logging.error('Could not set Attr to iSCSI target')
                 return False
 
-            if not lio_iscsi_target_set_parameter(target_iqn, tpg, "attribute", "demo_mode_write_protect", "0"):
-                print("FAIL: Could not set Attr to iSCSI target")
+            if not lio_iscsi_target_set_parameter(target_iqn, tpg, 'attribute', 'demo_mode_write_protect', '0'):
+                logging.error('Could not set Attr to iSCSI target')
                 return False
 
-            lun_id = "0"
+            lun_id = '0'
             if init_iqn:
                 if not lio_iscsi_create_acl(target_iqn, tpg, init_iqn):
-                    print("FAIL: Could not create iSCSI initiator ACL")
+                    logging.error('Could not create iSCSI initiator ACL')
                     return False
                 if not lio_iscsi_map_lun(target_iqn, tpg, init_iqn, lun_id, bs_type, tgt_lun_name):
-                    print("FAIL: Could not map LUN to iSCSI initiator")
+                    logging.error('Could not map LUN to iSCSI initiator')
                     return False
 
     return True
 
 
 def lio_setup_iscsi_target(  # noqa: ANN201
     tgt_iqn=None,  # noqa: ANN001
     init_iqn=None,  # noqa: ANN001
-    bs_type="fileio",  # noqa: ANN001
+    bs_type='fileio',  # noqa: ANN001
     lun_name=None,  # noqa: ANN001
-    lun_size="1G",  # noqa: ANN001
+    lun_size='1G',  # noqa: ANN001
     device_name=None,  # noqa: ANN001
     tgt_cnt=1,  # noqa: ANN001
     lun_cnt=1,  # noqa: ANN001
 ):
     """Create a basic iSCSI target
     The arguments are:
     tgt_iqn:          Target IQN, if not specified LIO will create a target IQN
@@ -1002,24 +998,24 @@
     device_name:      Device name when using block device, for example LV name
     tgt_cnt:          Number of targets to create, default: 1
     lun_cnt:          Number of LUNs to create, default: 1
     Returns:
     True: if iSCSI target is created
     False: If some problem happened.
     """
-    print("INFO: Creating basic iSCSI target...")
+    logging.info('Creating basic iSCSI target...')
     lio_install()
     lio_restart()
     lio_clearconfig()
 
     ver = lio_version()
-    print(f"INFO: Running targetcli version {ver}")
+    logging.info(f'Running targetcli version {ver}')
 
     if not lio_support_iscsi_target():
-        print("FAIL: Server does not support iSCSI target")
+        logging.error('Server does not support iSCSI target')
         return False
 
     lio_add_iscsi_target(tgt_iqn, init_iqn, bs_type, lun_name, lun_size, device_name, tgt_cnt, lun_cnt)
 
     return True
 
 
@@ -1032,15 +1028,15 @@
     None
     Returns:
     True: Host supports tcm_fc
     False: Host does not support tcm_fc.
     """
     lio_dict = lio_query()
 
-    if "tcm_fc" not in list(lio_dict.keys()):
+    if 'tcm_fc' not in list(lio_dict.keys()):
         # Host does not support FC target
         return False
 
     return True
 
 
 # ## FC target ###
@@ -1049,28 +1045,28 @@
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     if not wwn:
-        print("FAIL: lio_create_fc_target() - requires wwn parameter")
+        logging.error('lio_create_fc_target() - requires wwn parameter')
         return False
 
-    cmd = f"targetcli /tcm_fc/ create {wwn}"
+    cmd = f'targetcli /tcm_fc/ create {wwn}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: lio_create_fc_target() - Could not create FC target {wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'lio_create_fc_target() - Could not create FC target {wwn}')
         return False
 
     if wwn not in lio_get_fc_target():
         lio_dict = lio_query()
-        run("targetcli ls", verbose=True)
-        print("FAIL: lio_create_fc_target() - It seems to have added FC target, but it did not")
-        print(lio_dict["tcm_fc"])
+        run('targetcli ls')
+        logging.error('lio_create_fc_target() - It seems to have added FC target, but it did not')
+        print(lio_dict['tcm_fc'])
         print(lio_dict)
 
         return False
 
     return True
 
 
@@ -1079,28 +1075,28 @@
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
     if not wwn:
-        print("FAIL: lio_delete_fc_target() - requires wwn parameter")
+        logging.error('lio_delete_fc_target() - requires wwn parameter')
         return False
 
-    cmd = f"targetcli /tcm_fc/ delete {wwn}"
+    cmd = f'targetcli /tcm_fc/ delete {wwn}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: lio_delete_fc_target() - Could not delete FC target {wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'lio_delete_fc_target() - Could not delete FC target {wwn}')
         return False
 
     if wwn in lio_get_fc_target():
         lio_dict = lio_query()
-        run("targetcli ls", return_output=False, verbose=True)
-        print("FAIL: lio_delete_fc_target() - It seems to have deleted FC target, but it did not")
-        print(lio_dict["tcm_fc"])
+        run('targetcli ls', return_output=False)
+        logging.error('lio_delete_fc_target() - It seems to have deleted FC target, but it did not')
+        print(lio_dict['tcm_fc'])
         print(lio_dict)
 
         return False
 
     return True
 
 
@@ -1114,122 +1110,122 @@
     if not lio_dict:
         lio_dict = lio_query()
 
     if not lio_support_fc_target():
         # Host does not support FC target
         return None
 
-    return list(lio_dict["tcm_fc"].keys())
+    return list(lio_dict['tcm_fc'].keys())
 
 
 # ## FC ACLS ###
 def lio_create_fc_target_acl(tgt_wwn, init_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Add an initiator WWN to target WWN port
     The arguments are:
     tgt_wwn:     Host WWN
     init_wwn:    Initiator WWN
     Returns:
     True: If init wwn is created
     False: If some problem happened.
     """
     tgt_acls = lio_get_fc_target_acl(tgt_wwn, lio_dict=lio_dict)
     if tgt_acls and (init_wwn in tgt_acls):
-        print(f"INFO: {init_wwn} is already added to target {tgt_wwn}")
+        logging.info(f'{init_wwn} is already added to target {tgt_wwn}')
         return True
 
-    cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls create {init_wwn} add_mapped_luns=false"
+    cmd = f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls create {init_wwn} add_mapped_luns=false'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not add FC initiator {init_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not add FC initiator {init_wwn}')
         return False
 
     return True
 
 
 def lio_delete_fc_target_acl(tgt_wwn, init_wwn):  # noqa: ANN001, ANN201
     """Remove an initiator WWN from target WWN port
     The arguments are:
     tgt_wwn:     Host WWN
     init_wwn:    Initiator WWN
     Returns:
     True: If init wwn is removed
     False: If some problem happened.
     """
-    cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls delete {init_wwn}"
+    cmd = f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls delete {init_wwn}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete FC initiator {init_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete FC initiator {init_wwn}')
         return False
 
     return True
 
 
 def lio_get_fc_target_acl(tgt_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Get all acls from a specifc target
     The arguments are:
     tgt_wwn:     Host WWN
     Returns:
     List: List of initiators
     None: If some problem happened.
     """
     if not tgt_wwn:
-        print("FAIL: lio_get_fc_target_acl() - requires tgt_wwpn as argument")
+        logging.error('lio_get_fc_target_acl() - requires tgt_wwpn as argument')
         return None
     if not lio_dict:
         lio_dict = lio_query()
-    if not lio_dict["tcm_fc"][tgt_wwn]:
-        print(f"FAIL: {tgt_wwn} does not exist")
+    if not lio_dict['tcm_fc'][tgt_wwn]:
+        logging.error(f'{tgt_wwn} does not exist')
         print(lio_dict)
         return None
 
-    if "acls" not in list(lio_dict["tcm_fc"][tgt_wwn].keys()):
-        # print("FAIL: %s does not have acls" % tgt_wwn)
+    if 'acls' not in list(lio_dict['tcm_fc'][tgt_wwn].keys()):
+        # logging.error("%s does not have acls" % tgt_wwn)
         # print lio_dict
         return None
 
-    return list(lio_dict["tcm_fc"][tgt_wwn]["acls"].keys())
+    return list(lio_dict['tcm_fc'][tgt_wwn]['acls'].keys())
 
 
 # ## FC LUNs ###
 def lio_create_fc_target_lun(tgt_wwn, bs_type, lun_name):  # noqa: ANN001, ANN201
     """Add a LUN to target WWN port
     The arguments are:
     tgt_wwn:      Host WWN
     bs_type:      Backstore type
     lun_name:     Lun Name
     Returns:
     True: If LUN is created
     False: If some problem happened.
     """
-    cmd = "targetcli /tcm_fc/{}/luns create /backstores/{}/{} add_mapped_luns=false".format(
+    cmd = 'targetcli /tcm_fc/{}/luns create /backstores/{}/{} add_mapped_luns=false'.format(
         _wwn_2_tgt_wwn(tgt_wwn),
         bs_type,
         lun_name,
     )
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not add lun to FC target {tgt_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not add lun to FC target {tgt_wwn}')
         return False
 
     return True
 
 
 def lio_delete_fc_target_lun(tgt_wwn, lun_id):  # noqa: ANN001, ANN201
     """Remove an initiator WWN from target WWN port
     The arguments are:
     tgt_wwn:     Target WWN
     lun_id:      Lun id
     Returns:
     True: If LUN is removed
     False: If some problem happened.
     """
-    cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/luns delete {lun_id}"
+    cmd = f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/luns delete {lun_id}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not delete LUN from target {tgt_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not delete LUN from target {tgt_wwn}')
         return False
 
     return True
 
 
 def lio_get_fc_target_luns(tgt_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Return a dict with all backstores. If a backstore type
@@ -1240,22 +1236,22 @@
     List: list of luns
     None if something went wrong.
     """
     if not lio_dict:
         lio_dict = lio_query()
 
     if tgt_wwn not in lio_get_fc_target(lio_dict=lio_dict):
-        print(f"FAIL: {tgt_wwn} is not defined on targetcli")
+        logging.error(f'{tgt_wwn} is not defined on targetcli')
         return None
 
-    if "luns" not in list(lio_dict["tcm_fc"][tgt_wwn].keys()):
-        print(f"INFO: target {tgt_wwn} does not have any LUN\n")
+    if 'luns' not in list(lio_dict['tcm_fc'][tgt_wwn].keys()):
+        logging.info(f'target {tgt_wwn} does not have any LUN\n')
         return None
 
-    return lio_dict["tcm_fc"][tgt_wwn]["luns"]
+    return lio_dict['tcm_fc'][tgt_wwn]['luns']
 
 
 def lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=None):  # noqa: ANN001, ANN201
     """Return the target LUN id.
     The arguments are:
     tgt_wwn:      Target WWN
     bs_type:      Backstore Type
@@ -1268,100 +1264,100 @@
         lio_dict = lio_query()
 
     t_luns_dict = lio_get_fc_target_luns(tgt_wwn, lio_dict)
     if not t_luns_dict:
         return None
 
     for lun_id in list(t_luns_dict.keys()):
-        if t_luns_dict[lun_id]["bs_type"] == bs_type and t_luns_dict[lun_id]["lun_name"] == lun_name:
+        if t_luns_dict[lun_id]['bs_type'] == bs_type and t_luns_dict[lun_id]['lun_name'] == lun_name:
             return lun_id
     return None
 
 
 #    cmd = "targetcli /tcm_fc/%s/luns ls | grep %s/%s | awk '{print$2}'" % (_wwn_2_tgt_wwn(tgt_wwn), bs_type, lun_name)
-#    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+#    retcode, output = run_ret_out(cmd, return_output=True)
 #    if (retcode != 0):
 #        print ("FAIL: Could not get lun %s for FC target %s" % (lun_name, tgt_wwn))
 #        return None
 #
 #    if output == "":
 #        return None
 #    return output
 
 
 # ## FC LUNs mapping ###
 def lio_fc_lun_map(lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id):  # noqa: ANN001, ANN201
     """Map a LUN to a t_wwpn and h_wwpn."""
     if not lun_name or not bs_type or not tgt_wwn or not init_wwn or not init_lun_id:
-        print("FAIL: lio_fc_lun_map() - requires lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id parameters")
+        logging.error('lio_fc_lun_map() - requires lun_name, bs_type, tgt_wwn, init_wwn, init_lun_id parameters')
         return False
 
-    print(f"INFO: Mapping LUN {bs_type}/{lun_name} to {tgt_wwn}/{init_wwn}...")
+    logging.info(f'Mapping LUN {bs_type}/{lun_name} to {tgt_wwn}/{init_wwn}...')
     lio_dict = lio_query()
     if tgt_wwn not in lio_get_fc_target(lio_dict=lio_dict):
         lio_create_fc_target(tgt_wwn)
         # update lio_dict with new fc target
         lio_dict = lio_query()
 
     if not lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=lio_dict):
         lio_create_fc_target_lun(tgt_wwn, bs_type, lun_name)
         # update lio_dict with new fc target
         lio_dict = lio_query()
 
     # Do not pass lio_dict as parameter as we need to query it again to get updated info
     lun_id = lio_get_fc_target_lun_id(tgt_wwn, bs_type, lun_name, lio_dict=lio_dict)
     if not lun_id:
-        print(f"FAIL: lio_fc_lun_map() - Could not find lun {bs_type}/{lun_name} on target {tgt_wwn}")
+        logging.error(f'lio_fc_lun_map() - Could not find lun {bs_type}/{lun_name} on target {tgt_wwn}')
         lio_show()
         return False
 
     if not lio_create_fc_target_acl(tgt_wwn, init_wwn, lio_dict=lio_dict):
-        print(f"FAIL: Could not create ACL to host {init_wwn}")
+        logging.error(f'Could not create ACL to host {init_wwn}')
         lio_show()
         return False
 
     if not lio_create_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id, lun_id, lio_dict=lio_dict):
-        print(f"FAIL: Could not map LUN {lun_name} to host {init_wwn}")
+        logging.error(f'Could not map LUN {lun_name} to host {init_wwn}')
         return False
 
-    print(f"INFO: LUN {lun_name} mapped successfully")
+    logging.info(f'LUN {lun_name} mapped successfully')
     return True
 
 
 def lio_create_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id, tgt_lun_id, lio_dict=None):  # noqa: ANN001, ANN201
     """Map a LUN to target WWN / Initiator port
     The arguments are:
     tgt_wwn:      Target WWN
     init_wwn:     Host WWN
     init_lun_id   LUN id for the initiator
     tgt_lun_id:   LUN id on target
     Returns:
     True: If LUN is mapped
     False: If some problem happened.
     """
-    print("BRUNO lio_create_fc_target_map_lun")
+    print('BRUNO lio_create_fc_target_map_lun')
     # print lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id)
 
     if lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id, lio_dict=lio_dict):
-        print(f"INFO: lun {tgt_lun_id} is already mapped to FC target {tgt_wwn}/{init_wwn}")
+        logging.info(f'lun {tgt_lun_id} is already mapped to FC target {tgt_wwn}/{init_wwn}')
         return True
 
-    cmd = "targetcli /tcm_fc/{}/acls/{} create {} {}".format(
+    cmd = 'targetcli /tcm_fc/{}/acls/{} create {} {}'.format(
         _wwn_2_tgt_wwn(tgt_wwn),
         _wwn_2_tgt_wwn(init_wwn),
         init_lun_id,
         tgt_lun_id,
     )
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not map lun to FC target {tgt_wwn}/{init_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not map lun to FC target {tgt_wwn}/{init_wwn}')
         return False
 
     if not lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id):
-        print(f"FAIL: It seems to have mapped lun {tgt_lun_id}, but it did not")
+        logging.error(f'It seems to have mapped lun {tgt_lun_id}, but it did not')
         return False
 
     return True
 
 
 def lio_fc_target_get_mapped_luns(tgt_wwn, init_wwn, lio_dict=None):  # noqa: ANN001, ANN201
     """Get LUN mapping from tgt_wwn/init_wwn
@@ -1374,15 +1370,15 @@
     """
     if not lio_dict:
         lio_dict = lio_query()
 
     if init_wwn not in lio_get_fc_target_acl(tgt_wwn, lio_dict=lio_dict):
         return None
 
-    mapped_luns_dict = lio_dict["tcm_fc"][tgt_wwn]["acls"][init_wwn]
+    mapped_luns_dict = lio_dict['tcm_fc'][tgt_wwn]['acls'][init_wwn]
     if not mapped_luns_dict:
         return None
     return mapped_luns_dict
 
 
 def lio_fc_target_unmap_lun(tgt_wwn, init_wwn, init_lun_id):  # noqa: ANN001, ANN201
     """Un map LUN from tgt_wwn/init_wwn
@@ -1390,22 +1386,22 @@
     tgt_wwn:      Target WWN
     init_wwn:     Host WWN
     init_lun_id   LUN id for the initiator
     Returns:
     True: If LUN is unmapped
     False: If some problem happened.
     """
-    cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls/{_wwn_2_tgt_wwn(init_wwn)} delete {init_lun_id}"
+    cmd = f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls/{_wwn_2_tgt_wwn(init_wwn)} delete {init_lun_id}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not unmap LUN from target {tgt_wwn}/{init_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not unmap LUN from target {tgt_wwn}/{init_wwn}')
         return False
 
     if lio_get_fc_target_map_lun(tgt_wwn, init_wwn, init_lun_id):
-        print(f"FAIL: It seems to have unmapped lun {init_lun_id}, but it did not")
+        logging.error(f'It seems to have unmapped lun {init_lun_id}, but it did not')
         return False
     return True
 
 
 def lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id, lio_dict=None):  # noqa: ANN001, ANN201
     """Get initator LUN ID if a LUN is mapped to target WWN / Initiator port
     The arguments are:
@@ -1422,15 +1418,15 @@
 
     if init_wwn not in lio_get_fc_target_acl(tgt_wwn, lio_dict=lio_dict):
         return None
 
     # print "DEBUG lio_get_fc_target_map_lunt t: %s" % tgt_wwn
     # print "DEBUG lio_get_fc_target_map_lunt i: %s" % init_wwn
     # print "DEBUG lio_get_fc_target_map_lunt tgt_id: %s" % tgt_lun_id
-    init_acls_dict = lio_dict["tcm_fc"][tgt_wwn]["acls"][init_wwn]
+    init_acls_dict = lio_dict['tcm_fc'][tgt_wwn]['acls'][init_wwn]
     if tgt_lun_id not in list(init_acls_dict.keys()):
         # print ("FAIL: Could not get mapping for lun %s on FC target %s/%s" % (tgt_lun_id, tgt_wwn, init_wwn))
         return None
 
     return init_acls_dict[tgt_lun_id]
 
 
@@ -1447,68 +1443,68 @@
         lio_dict = lio_query()
 
     bs_details_dict = lio_get_backstore_details(bs_type, lun_name, lio_dict=lio_dict)
     if not bs_details_dict:
         # It does not exist
         return None
 
-    if "mapping" not in list(bs_details_dict.keys()):
+    if 'mapping' not in list(bs_details_dict.keys()):
         return None
 
-    return bs_details_dict["mapping"]
+    return bs_details_dict['mapping']
 
 
 # ## FC tag ###
 def lio_tag_fc_initiator(tgt_wwn, init_wwn, tag):  # noqa: ANN001, ANN201
     """Create a tag for initiator wwn
     The arguments are:
     tgt_wwn:     Host wwn
     init_wwn:    Initiator wwn
     tag:          tag for the initiator wwn
     Returns:
     True: If tag is created
     False: If some problem happened.
     """
-    cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls tag {_wwn_2_tgt_wwn(init_wwn)} {tag}"
+    cmd = f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls tag {_wwn_2_tgt_wwn(init_wwn)} {tag}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not tag FC initiator {init_wwn}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not tag FC initiator {init_wwn}')
         return False
 
     return True
 
 
 def lio_untag_fc_initiator(tgt_wwn, tag):  # noqa: ANN001, ANN201
     """Remove tag from initiator wwn
     The arguments are:
     tgt_wwn:     Host wwn
     tag:          tag for the initiator wwn
     Returns:
     True: If tag is created
     False: If some problem happened.
     """
-    cmd = f"targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls untag {tag}"
+    cmd = f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls untag {tag}'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print(f"FAIL: Could not untag FC tag {tag}")
+    if run(cmd).rc != 0:
+        logging.error(f'Could not untag FC tag {tag}')
         return False
 
     return True
 
 
 def lio_is_fc_tag(tgt_wwn, tag):  # noqa: ANN001, ANN201
     """Check if a tag is an FC initiator tag
     The arguments are:
     wwn:     Host wwn
     Returns:
     True: If target is added
     False: If some problem happened.
     """
-    cmd = f"targetcli /tcm_fc/{tgt_wwn}/acls/{tag}"
-    if run(cmd, verbose=False).returncode != 0:
+    cmd = f'targetcli /tcm_fc/{tgt_wwn}/acls/{tag}'
+    if run(cmd).rc != 0:
         return False
     return True
 
 
 ##################################################
 # ################ LIO General ####################
 ##################################################
@@ -1520,59 +1516,59 @@
     True: If targetcli is installed correctly
     False: If some problem happened.
     """
     ver = linux.dist_ver()
     if not ver:
         return False
 
-    targetcli_pack = "targetcli"
-    if linux.dist_name() == "RHEL" and ver < 7:
-        targetcli_pack = "fcoe-target-utils"
+    targetcli_pack = 'targetcli'
+    if linux.dist_name() == 'RHEL' and ver < 7:
+        targetcli_pack = 'fcoe-target-utils'
 
     if not linux.install_package(targetcli_pack):
-        print(f"FAIL: Could not install {targetcli_pack}")
+        logging.error(f'Could not install {targetcli_pack}')
         return False
 
     return True
 
 
 def lio_get_service_name():  # noqa: ANN201
     """Get service name that targetcli uses
     The arguments are:
     None
     Returns:
     String: Name of the service
     None: If some problem happened.
     """
-    targetcli_service = "target"
+    targetcli_service = 'target'
     ver = linux.dist_ver()
     if not ver:
         return None
 
-    if linux.dist_name() == "RHEL" and ver < 7:
-        targetcli_service = "fcoe-target"
+    if linux.dist_name() == 'RHEL' and ver < 7:
+        targetcli_service = 'fcoe-target'
 
     return targetcli_service
 
 
 def lio_restart():  # noqa: ANN201
     """Restart LIO service
     The arguments are:
     None
     Returns:
     True: Service started
     False: If some problem happened.
     """
     targetcli_service = lio_get_service_name()
     if not targetcli_service:
-        print("FAIL: lio_restart() - Could not get LIO service name")
+        logging.error('lio_restart() - Could not get LIO service name')
         return False
 
     if not linux.service_restart(targetcli_service):
-        print("FAIL: Could not restart LIO service")
+        logging.error('Could not restart LIO service')
         return False
     # sleep 5s to avoid service to not be restarted
     # target.service start request repeated too quickly, refusing to start.
     linux.sleep(5)
     return True
 
 
@@ -1580,85 +1576,85 @@
     """List LIO configuration
     The arguments are:
     None
     Returns:
     True: If listed config
     False: If some problem happened.
     """
-    cmd = "targetcli ls"
+    cmd = 'targetcli ls'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print("FAIL: Could not show LIO config")
+    if run(cmd).rc != 0:
+        logging.error('Could not show LIO config')
         return False
     return True
 
 
 def lio_saveconfig():  # noqa: ANN201
     """Save LIO configuration
     The arguments are:
     None
     Returns:
     True: If config is saved
     False: If some problem happened.
     """
-    cmd = "targetcli saveconfig"
+    cmd = 'targetcli saveconfig'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print("FAIL: Could not save LIO config")
+    if run(cmd).rc != 0:
+        logging.error('Could not save LIO config')
         return False
     return True
 
 
 def lio_clearconfig():  # noqa: ANN201
     """Clear LIO configuration
     The arguments are:
     None
     Returns:
     True: If config is deleted
     False: If some problem happened.
     """
-    print("INFO: Cleaning up LIO configuration")
+    logging.info('Cleaning up LIO configuration')
 
-    if not linux.is_installed("targetcli"):
+    if not linux.is_installed('targetcli'):
         return True
 
-    fileio_dict = lio_get_backstores("fileio")
+    fileio_dict = lio_get_backstores('fileio')
     if fileio_dict:
         # Delete all files before cleaning configuration
         for lun in list(fileio_dict.keys()):
-            lio_delete_backstore(bs_type="fileio", lun_name=lun)
+            lio_delete_backstore(bs_type='fileio', lun_name=lun)
 
-    cmd = "targetcli clearconfig true"
+    cmd = 'targetcli clearconfig true'
 
-    if run(cmd, verbose=True).returncode != 0:
-        print("FAIL: Could not delete LIO config")
+    if run(cmd).rc != 0:
+        logging.error('Could not delete LIO config')
         return False
 
     return True
 
 
 def lio_version():  # noqa: ANN201
     """Get targetcli version
     The arguments are:
     None
     Returns:
     String: TargetCli version
     None: If some problem happened.
     """
-    cmd = "targetcli version"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = 'targetcli version'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Could not get targetcli version")
+        logging.error('Could not get targetcli version')
         return None
 
-    version_regex = re.compile(".* version (.*)$")
+    version_regex = re.compile('.* version (.*)$')
     m = version_regex.search(output)
     if m:
         return m.group(1)
-    print(f"FAIL: Could not parse targetcli version output ({output})")
+    logging.error(f'Could not parse targetcli version output ({output})')
     return None
 
 
 def lio_clean_up_targets(lio_dict=None):  # noqa: ANN001, ANN201
     """Removing backstore might leave targets with empty mapping
     They should be removed.
     """
@@ -1671,284 +1667,284 @@
     need_to_query_lio = False
     success = True
     for tgt in fc_targets:
         initiators = lio_get_fc_target_acl(tgt, lio_dict=lio_dict)
         if initiators:
             for init in initiators:
                 if not lio_fc_target_get_mapped_luns(tgt, init, lio_dict=lio_dict):
-                    print(f"DEBUG: Should remove initiator {init} from tgt {tgt}")
+                    print(f'DEBUG: Should remove initiator {init} from tgt {tgt}')
                     if not lio_delete_fc_target_acl(tgt, init):
                         success = False
                     need_to_query_lio = True
 
     # Check again for targets without any initiator
     if need_to_query_lio:
         lio_dict = lio_query()
     fc_targets = lio_get_fc_target(lio_dict=lio_dict)
     for tgt in fc_targets:
         initiators = lio_get_fc_target_acl(tgt, lio_dict=lio_dict)
         if not initiators:
-            print(f"DEBUG: Should remove target {tgt}")
+            print(f'DEBUG: Should remove target {tgt}')
             if not lio_delete_fc_target(tgt):
                 success = False
 
     return success
 
 
 class TargetCLI:
-    def __init__(self, path="", disable_check=False) -> None:  # noqa: ANN001
+    def __init__(self, path='', disable_check=False) -> None:  # noqa: ANN001
         self.disable_check = disable_check
         self.path = path
         if linux.dist_ver() < 7:
-            print("FATAL: TargetCLI is not supported on RHEL < 7.")
+            logging.critical('TargetCLI is not supported on RHEL < 7.')
 
-        if not linux.install_package("targetcli", check=False):
-            print("FATAL: Could not install targetcli package")
+        if not linux.install_package('targetcli', check=False):
+            logging.critical('Could not install targetcli package')
 
     @staticmethod
     def remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     @staticmethod
     def _extract_args(kwargs, keys=None):  # noqa: ANN001, ANN205
-        keys = keys or ["return_output", "verbosity", "path"]
+        keys = keys or ['return_output', 'verbosity', 'path']
         arguments = {}
         for key in keys:
             if key not in kwargs:
                 continue
             arguments[key] = kwargs.pop(key)
         return arguments, kwargs
 
-    def _run(self, cmd, verbosity=True, return_output=False, path=None):  # noqa: ANN001, ANN202
+    def _run(self, cmd, return_output=False, path=None):  # noqa: ANN001, ANN202
         # Constructs the command to run and runs it
 
         if path is not None:
             self.path = path
 
-        cmd = "targetcli cd" if cmd == "cd" and self.path is None else "targetcli " + self.path + " " + cmd
+        cmd = 'targetcli cd' if cmd == 'cd' and self.path is None else 'targetcli ' + self.path + ' ' + cmd
 
         if return_output:
-            ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
+            ret, data = run_ret_out(cmd, return_output=True)
             if ret != 0:
-                print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+                logging.warning(f"Running command: '{cmd}' failed. Return with output.")
             return ret, data
 
-        ret = run(cmd, verbose=verbosity).returncode
+        ret = run(cmd).rc
         if ret != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+            logging.warning(f"Running command: '{cmd}' failed.")
         return ret
 
-    def ls(self, depth="", **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"ls {depth}", **kwargs)
+    def ls(self, depth='', **kwargs):  # noqa: ANN001, ANN003, ANN201
+        return self._run(f'ls {depth}', **kwargs)
 
     def cd(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("cd", **kwargs)
+        return self._run('cd', **kwargs)
 
     def pwd(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("pwd", **kwargs)
+        return self._run('pwd', **kwargs)
 
     def create(self, **kwargs):  # noqa: ANN003, ANN201
         keys = None
-        cmd = "create "
+        cmd = 'create '
         arguments, kwargs = self._extract_args(kwargs)
         # the following ensures the ordering is correct in correct paths
         # True means it is required, False it is optional
-        if "backstores/block" in self.path:
-            keys = {"name": True, "dev": True, "readonly": False, "wwn": False}
-        elif "backstores/fileio" in self.path:
+        if 'backstores/block' in self.path:
+            keys = {'name': True, 'dev': True, 'readonly': False, 'wwn': False}
+        elif 'backstores/fileio' in self.path:
             keys = {
-                "name": True,
-                "file_or_dev": True,
-                "size": True,
-                "write_back": False,
-                "sparse": False,
-                "wwn": False,
+                'name': True,
+                'file_or_dev': True,
+                'size': True,
+                'write_back': False,
+                'sparse': False,
+                'wwn': False,
             }
-        elif "backstores/pscsi" in self.path:
-            keys = {"name": True, "dev": True}
-        elif "backstores/ramdisk" in self.path:
-            keys = {"name": True, "size": True, "nullio": False, "wwn": False}
-        elif "backstores/user:qcow" in self.path:  # noqa: SIM114
+        elif 'backstores/pscsi' in self.path:
+            keys = {'name': True, 'dev': True}
+        elif 'backstores/ramdisk' in self.path:
+            keys = {'name': True, 'size': True, 'nullio': False, 'wwn': False}
+        elif 'backstores/user:qcow' in self.path:  # noqa: SIM114
             keys = {
-                "name": True,
-                "size": True,
-                "cfgstring": True,
-                "wwn": False,
-                "hw_max_sectors": False,
-                "control": False,
+                'name': True,
+                'size': True,
+                'cfgstring': True,
+                'wwn': False,
+                'hw_max_sectors': False,
+                'control': False,
             }
-        elif "backstores/user:rbd" in self.path:  # noqa: SIM114
+        elif 'backstores/user:rbd' in self.path:  # noqa: SIM114
             keys = {
-                "name": True,
-                "size": True,
-                "cfgstring": True,
-                "wwn": False,
-                "hw_max_sectors": False,
-                "control": False,
+                'name': True,
+                'size': True,
+                'cfgstring': True,
+                'wwn': False,
+                'hw_max_sectors': False,
+                'control': False,
             }
-        elif "backstores/user:zbc" in self.path:
+        elif 'backstores/user:zbc' in self.path:
             keys = {
-                "name": True,
-                "size": True,
-                "cfgstring": True,
-                "wwn": False,
-                "hw_max_sectors": False,
-                "control": False,
+                'name': True,
+                'size': True,
+                'cfgstring': True,
+                'wwn': False,
+                'hw_max_sectors': False,
+                'control': False,
             }
-        elif self.path.startswith("/iscsi/"):
-            if "iqn" in self.path:
-                if "acls" in self.path:
-                    keys = {"wwn": True, "add_mapped_luns": False}
-                elif "luns" in self.path:
+        elif self.path.startswith('/iscsi/'):
+            if 'iqn' in self.path:
+                if 'acls' in self.path:
+                    keys = {'wwn': True, 'add_mapped_luns': False}
+                elif 'luns' in self.path:
                     keys = {
-                        "storage_object": True,
-                        "lun": False,
-                        "add_mapped_luns": False,
+                        'storage_object': True,
+                        'lun': False,
+                        'add_mapped_luns': False,
                     }
-                elif "portals" in self.path:
-                    keys = {"ip_address": False, "ip_port": False}
+                elif 'portals' in self.path:
+                    keys = {'ip_address': False, 'ip_port': False}
                 else:
-                    keys = {"tag": False}
+                    keys = {'tag': False}
             else:
-                keys = {"wwn": False}
-        elif self.path.startswith("/loopback"):
-            if "naa" in self.path:
-                if "luns" in self.path:
+                keys = {'wwn': False}
+        elif self.path.startswith('/loopback'):
+            if 'naa' in self.path:
+                if 'luns' in self.path:
                     keys = {
-                        "storage_object": True,
-                        "lun": False,
-                        "add_mapped_luns": False,
+                        'storage_object': True,
+                        'lun': False,
+                        'add_mapped_luns': False,
                     }
             else:
-                keys = {"wwn": False}
+                keys = {'wwn': False}
         else:
-            keys = {"wwn": False}
+            keys = {'wwn': False}
         try:
             for key in keys:
-                cmd += f"{key}={kwargs[key]} "
+                cmd += f'{key}={kwargs[key]} '
         except KeyError:
             if not self.disable_check and keys[key]:
-                print(f"FAIL: Create on path '{self.path}' requires argument {key}.")
+                logging.exception(f"Create on path '{self.path}' requires argument {key}.")
                 return 1
         return self._run(cmd, **arguments)
 
     def delete(self, **kwargs):  # noqa: ANN003, ANN201
         keys = None
-        cmd = "delete "
+        cmd = 'delete '
         arguments, kwargs = self._extract_args(kwargs)
         # the following ensures the ordering is correct in correct paths
         # True means it is required, False it is optional
-        if "backstores/block" in self.path:  # noqa: SIM114
-            keys = {"name": True}
-        elif "backstores/fileio" in self.path:  # noqa: SIM114
-            keys = {"name": True}
-        elif "backstores/pscsi" in self.path:  # noqa: SIM114
-            keys = {"name": True}
-        elif "backstores/ramdisk" in self.path:  # noqa: SIM114
-            keys = {"name": True}
-        elif "backstores/user:qcow" in self.path:  # noqa: SIM114
-            keys = {"name": True}
-        elif "backstores/user:rbd" in self.path:  # noqa: SIM114
-            keys = {"name": True}
-        elif "backstores/user:zbc" in self.path:
-            keys = {"name": True}
-        elif self.path.startswith("/iscsi/"):
-            if "iqn" in self.path:
-                if "acls" in self.path:
-                    keys = {"wwn": True}
-                elif "luns" in self.path:
-                    keys = {"lun": True}
-                elif "portals" in self.path:
-                    keys = {"ip_address": True, "ip_port": True}
+        if 'backstores/block' in self.path:  # noqa: SIM114
+            keys = {'name': True}
+        elif 'backstores/fileio' in self.path:  # noqa: SIM114
+            keys = {'name': True}
+        elif 'backstores/pscsi' in self.path:  # noqa: SIM114
+            keys = {'name': True}
+        elif 'backstores/ramdisk' in self.path:  # noqa: SIM114
+            keys = {'name': True}
+        elif 'backstores/user:qcow' in self.path:  # noqa: SIM114
+            keys = {'name': True}
+        elif 'backstores/user:rbd' in self.path:  # noqa: SIM114
+            keys = {'name': True}
+        elif 'backstores/user:zbc' in self.path:
+            keys = {'name': True}
+        elif self.path.startswith('/iscsi/'):
+            if 'iqn' in self.path:
+                if 'acls' in self.path:
+                    keys = {'wwn': True}
+                elif 'luns' in self.path:
+                    keys = {'lun': True}
+                elif 'portals' in self.path:
+                    keys = {'ip_address': True, 'ip_port': True}
                 else:
-                    keys = {"tag": True}
+                    keys = {'tag': True}
             else:
-                keys = {"wwn": True}
-        elif self.path.startswith("/loopback"):
-            if "naa" in self.path:
-                if "luns" in self.path:
-                    keys = {"lun": True}
+                keys = {'wwn': True}
+        elif self.path.startswith('/loopback'):
+            if 'naa' in self.path:
+                if 'luns' in self.path:
+                    keys = {'lun': True}
             else:
-                keys = {"wwn": False}
+                keys = {'wwn': False}
         else:
-            keys = {"wwn": True}
+            keys = {'wwn': True}
 
         try:
             for key in keys:
-                cmd += f"{key}={kwargs[key]} "
+                cmd += f'{key}={kwargs[key]} '
         except KeyError:
             if not self.disable_check and keys[key]:
-                print(f"FAIL: Delete on path '{self.path}' requires argument {key}.")
+                logging.exception(f"Delete on path '{self.path}' requires argument {key}.")
                 return 1
 
         return self._run(cmd, **arguments)
 
-    def help(self, topic="", **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
-        return self._run(f"help {topic}", **kwargs)
+    def help(self, topic='', **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
+        return self._run(f'help {topic}', **kwargs)
 
     def saveconfig(self, savefile=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "saveconfig"
+        cmd = 'saveconfig'
         if savefile:
-            cmd += f" {savefile}"
+            cmd += f' {savefile}'
         return self._run(cmd, **kwargs)
 
     def restoreconfig(  # noqa: ANN201
         self,
-        savefile="/etc/target/saveconfig.json",  # noqa: ANN001
+        savefile='/etc/target/saveconfig.json',  # noqa: ANN001
         clearexisting=False,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        return self._run(f"restoreconfig {savefile} {clearexisting}", **kwargs)
+        return self._run(f'restoreconfig {savefile} {clearexisting}', **kwargs)
 
     def clearconfig(self, confirm=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"clearconfig {confirm}", **kwargs)
+        return self._run(f'clearconfig {confirm}', **kwargs)
 
-    def sessions(self, action="", sid="", **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"sessions {action} {sid}", **kwargs)
+    def sessions(self, action='', sid='', **kwargs):  # noqa: ANN001, ANN003, ANN201
+        return self._run(f'sessions {action} {sid}', **kwargs)
 
     def exit(self, **kwargs):  # noqa: A003, ANN003, ANN201
-        return self._run("exit", **kwargs)
+        return self._run('exit', **kwargs)
 
-    def get(self, group="", **kwargs):  # noqa: ANN001, ANN003, ANN201
+    def get(self, group='', **kwargs):  # noqa: ANN001, ANN003, ANN201
         arguments, kwargs = self._extract_args(kwargs)
         cmd = f"get {group} {' '.join(kwargs.keys())}"
         return self._run(cmd, **arguments)
 
-    def set(self, group="", **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
+    def set(self, group='', **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
         arguments, kwargs = self._extract_args(kwargs)
         params = [f"{kwarg}='{kwargs[kwarg]}'" if kwargs[kwarg] else f"{kwarg}='{kwargs[kwarg]}'" for kwarg in kwargs]
         cmd = f"set {group} {' '.join(params)}"
         return self._run(cmd, **arguments)
 
     def info(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("info", **kwargs)
+        return self._run('info', **kwargs)
 
     def version(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("version", **kwargs)
+        return self._run('version', **kwargs)
 
     def status(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("status", **kwargs)
+        return self._run('status', **kwargs)
 
     def refresh(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("refresh", **kwargs)
+        return self._run('refresh', **kwargs)
 
     def disable(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("disable", **kwargs)
+        return self._run('disable', **kwargs)
 
     def enable(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("enable", **kwargs)
+        return self._run('enable', **kwargs)
 
     def bookmarks(self, **kwargs):  # noqa: ANN003, ANN201
         # How to use this?
-        return self._run("bookmarks", **kwargs)
+        return self._run('bookmarks', **kwargs)
 
-    def enable_iser(self, boolean="", **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"enable_iser {boolean}", **kwargs)
+    def enable_iser(self, boolean='', **kwargs):  # noqa: ANN001, ANN003, ANN201
+        return self._run(f'enable_iser {boolean}', **kwargs)
 
-    def enable_offload(self, boolean="", **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"enable_offload {boolean}", **kwargs)
+    def enable_offload(self, boolean='', **kwargs):  # noqa: ANN001, ANN003, ANN201
+        return self._run(f'enable_offload {boolean}', **kwargs)
 
-    def tag(self, wwn_or_tag="", new_tag="", **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"tag {wwn_or_tag} {new_tag}", **kwargs)
+    def tag(self, wwn_or_tag='', new_tag='', **kwargs):  # noqa: ANN001, ANN003, ANN201
+        return self._run(f'tag {wwn_or_tag} {new_tag}', **kwargs)
 
-    def untag(self, wwn_or_tag="", **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run(f"untag {wwn_or_tag}", **kwargs)
+    def untag(self, wwn_or_tag='', **kwargs):  # noqa: ANN001, ANN003, ANN201
+        return self._run(f'untag {wwn_or_tag}', **kwargs)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/lsm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """lsm.py: Module with test specific method for libstoragemgmt."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
 import re
 import sys
 from contextlib import suppress
 from time import sleep
 from typing import Dict, List, Union
 
@@ -20,89 +21,89 @@
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.persistent_vars import read_env, read_var
 
 
 def check_ssl(protocol) -> bool:  # noqa: ANN001
     """Checks if fmf_protocol is ssl/no_ssl and limits the protocol by this."""
     try:
-        ssl = read_env("fmf_protocol")
+        ssl = read_env('fmf_protocol')
     except KeyError:
         # Protocol not limited
         return True
-    if ssl == "ssl" and "ssl" in protocol or ssl == "no_ssl" and "ssl" not in protocol:
+    if ssl == 'ssl' and 'ssl' in protocol or ssl == 'no_ssl' and 'ssl' not in protocol:
         return True
     return False
 
 
 def yield_lsm_config():  # noqa: ANN201
-    config = {"protocols": [], "username": None, "password": None, "target": None}
+    config = {'protocols': [], 'username': None, 'password': None, 'target': None}
 
     for conf in config:
         with suppress(OSError):
-            config[conf] = read_var("LSM_" + conf.upper())
+            config[conf] = read_var('LSM_' + conf.upper())
 
     try:
-        if not isinstance(config["protocols"], list):
+        if not isinstance(config['protocols'], list):
             raise TypeError  # noqa: TRY301
     except TypeError:
         print(
             f"ERROR: Protocols must be list, got {config['protocols']}, type '{type(config['protocols'])}'.",
         )
         sys.exit(1)
 
-    protocols = config.pop("protocols")
+    protocols = config.pop('protocols')
     for protocol in protocols:
         if not check_ssl(protocol):
             continue
-        config["protocol"] = protocol
+        config['protocol'] = protocol
         yield config
 
 
-def get_data_from_script_output(data, id="id"):  # noqa: ANN001, ANN201
-    split_string = re.match("(-*)", data).group()
+def get_data_from_script_output(data, id='id'):  # noqa: ANN001, ANN201
+    split_string = re.match('(-*)', data).group()
     try:
         items = [x for x in data.split(split_string) if id in x]
     except ValueError as e:
         print(repr(e))
         return None
     data = {}
     for item in items:
         for line in item.splitlines():
             if len(line) < 2:
                 continue
             if line.startswith(id):
                 # luckily id is always first
-                item_id = line.split("|").pop().strip()
+                item_id = line.split('|').pop().strip()
                 data[item_id] = {}
             else:
-                line_data = line.split("|")
+                line_data = line.split('|')
                 data[item_id][line_data[0].strip()] = line_data[1].strip()
     return data
 
 
 def get_local_disk_data(data):  # noqa: ANN001, ANN201
-    return get_data_from_script_output(data, id="Path")
+    return get_data_from_script_output(data, id='Path')
 
 
-def get_id_from_name(data, name, field="Name", item_id="id"):  # noqa: ANN001, ANN201
+def get_id_from_name(data, name, field='Name', item_id='id'):  # noqa: ANN001, ANN201
     data = get_data_from_script_output(data, id=item_id)
     for line in data:
         if data[line][field] == name:
             return line
-    print(f"FAIL: Could not find item named '{name}'.")
+    logging.error(f"Could not find item named '{name}'.")
     return None
 
 
-def get_data_from_id(data, name, field="Name", item_id="id"):  # noqa: ANN001, ANN201
+def get_data_from_id(data, name, field='Name', item_id='id'):  # noqa: ANN001, ANN201
     data = get_data_from_script_output(data, id=item_id)
     for line in data:
         if line != name:
             continue
         return data[line][field]
-    print(f"FAIL: Could not find item named '{name}'.")
+    logging.error(f"Could not find item named '{name}'.")
     return None
 
 
 def get_ag_id_from_name(data, name):  # noqa: ANN001, ANN201
     return get_id_from_name(data, name)
 
 
@@ -112,51 +113,51 @@
 
 def get_vol_id_from_name(data, name):  # noqa: ANN001, ANN201
     return get_id_from_name(data, name)
 
 
 def get_export_id_from_export_path(data, export_path):  # noqa: ANN001, ANN201
     # policy is 'disabled' but cli takes 'disable'
-    return get_id_from_name(data, export_path, field="Export Path")
+    return get_id_from_name(data, export_path, field='Export Path')
 
 
 def get_system_read_pct_of_sys(data, sys):  # noqa: ANN001, ANN201
-    return get_data_from_script_output(data)[sys]["Read Cache Percentage"]
+    return get_data_from_script_output(data)[sys]['Read Cache Percentage']
 
 
 def get_cache_policy_from_id(data, vol_id, field):  # noqa: ANN001, ANN201
-    return translate_cache_policy(get_data_from_id(data, vol_id, field=field, item_id="Volume id"))
+    return translate_cache_policy(get_data_from_id(data, vol_id, field=field, item_id='Volume id'))
 
 
 def translate_cache_policy(policy):  # noqa: ANN001, ANN201
     dictionary = {
-        "Write Back": "WB",
-        "Write Through": "WT",
-        "Auto": "AUTO",
-        "Enabled": "enable",
-        "Disabled": "disable",
+        'Write Back': 'WB',
+        'Write Through': 'WT',
+        'Auto': 'AUTO',
+        'Enabled': 'enable',
+        'Disabled': 'disable',
     }
     try:
         return dictionary[policy]
     except KeyError:
         return policy
 
 
 def get_replace_dict():  # noqa: ANN201
     """Returns dict of keys to replace from fmf to sts.lsm.LibStorageMgmt.
 
     Returns:
       dict.
     """
     return {
-        "ag_name": "name",
-        "vol_name": "name",
-        "fs_name": "name",
-        "snap_name": "name",
-        "rep_name": "name",
+        'ag_name': 'name',
+        'vol_name': 'name',
+        'fs_name': 'name',
+        'snap_name': 'name',
+        'rep_name': 'name',
     }
 
 
 def _cli(func):  # noqa: ANN001, ANN202
     # This is a decorator to mark functions callable by 'lsmcli'
     func.cli = True
     return func
@@ -169,15 +170,15 @@
         password=None,  # noqa: ANN001
         target=None,  # noqa: ANN001
         protocol=None,  # noqa: ANN001
         disable_check=False,  # noqa: ANN001
     ) -> None:
         self.disable_check = disable_check
         if linux.dist_ver() < 7:
-            print("FATAL: libstoragemgmt is not supported on RHEL < 7.")
+            logging.critical('libstoragemgmt is not supported on RHEL < 7.')
 
         self.username = None
         self.password = None
         self.target = None
         self.protocol = None
         self.port = None
         self.query_params = None
@@ -193,366 +194,366 @@
 
         # local target does not require anything of this and megaraid/sim needs only protocol
         if username and password and target and protocol:
             self.username = username
             self.password = password
             self.target = target
             self.protocol = protocol
-        elif protocol and "megaraid" in protocol or "sim" in protocol:
+        elif protocol and 'megaraid' in protocol or 'sim' in protocol:
             self.protocol = protocol
 
         if self.password:
-            os.environ["LSMCLI_PASSWORD"] = self.password
-            print("INFO: Password set")
-        elif os.environ.get("LSMCLI_PASSWORD"):
-            del os.environ["LSMCLI_PASSWORD"]
-            print("INFO: Password cleaned")
+            os.environ['LSMCLI_PASSWORD'] = self.password
+            logging.info('Password set')
+        elif os.environ.get('LSMCLI_PASSWORD'):
+            del os.environ['LSMCLI_PASSWORD']
+            logging.info('Password cleaned')
 
         requires_restart = False
         # stop if lsm package cannot be installed
-        if not linux.is_installed("libstoragemgmt"):
-            if not linux.install_package("libstoragemgmt", check=False):
-                print("FATAL: Could not install libstoragemgmt package")
+        if not linux.is_installed('libstoragemgmt'):
+            if not linux.install_package('libstoragemgmt', check=False):
+                logging.critical('Could not install libstoragemgmt package')
             else:
                 requires_restart = True
 
-        if self.protocol == "smispy":
-            self.port = "5988"
-            self.query_params = "?namespace=root/emc"
-        if self.protocol == "smispy+ssl":
+        if self.protocol == 'smispy':
+            self.port = '5988'
+            self.query_params = '?namespace=root/emc'
+        if self.protocol == 'smispy+ssl':
             # ssl uses different port
-            self.port = "5989"
+            self.port = '5989'
             # ignore missing ssl certificate
-            self.query_params = "?namespace=root/emc&no_ssl_verify=yes"
+            self.query_params = '?namespace=root/emc&no_ssl_verify=yes'
 
         # install protocol specific packages
         if self.protocol:
-            if "ontap" in self.protocol:
-                if not linux.is_installed("libstoragemgmt-netapp-plugin"):
-                    if not linux.install_package("libstoragemgmt-netapp-plugin", check=False):
-                        print("FATAL: Could not install LSM NetApp plugin")
+            if 'ontap' in self.protocol:
+                if not linux.is_installed('libstoragemgmt-netapp-plugin'):
+                    if not linux.install_package('libstoragemgmt-netapp-plugin', check=False):
+                        logging.critical('Could not install LSM NetApp plugin')
                     else:
                         requires_restart = True
-            elif "smispy" in self.protocol:
-                if not linux.is_installed("libstoragemgmt-smis-plugin"):
-                    if not linux.install_package("libstoragemgmt-smis-plugin", check=False):
-                        print("FATAL: Could not install LSM SMIS plugin")
+            elif 'smispy' in self.protocol:
+                if not linux.is_installed('libstoragemgmt-smis-plugin'):
+                    if not linux.install_package('libstoragemgmt-smis-plugin', check=False):
+                        logging.critical('Could not install LSM SMIS plugin')
                     else:
                         requires_restart = True
-            elif "targetd" in self.protocol:
-                if not linux.is_installed("libstoragemgmt-targetd-plugin"):
-                    if not linux.install_package("libstoragemgmt-targetd-plugin", check=False):
-                        print("FATAL: Could not install LSM targetd plugin")
+            elif 'targetd' in self.protocol:
+                if not linux.is_installed('libstoragemgmt-targetd-plugin'):
+                    if not linux.install_package('libstoragemgmt-targetd-plugin', check=False):
+                        logging.critical('Could not install LSM targetd plugin')
                     else:
                         requires_restart = True
-            elif "megaraid" in self.protocol:
-                if not linux.is_installed("libstoragemgmt-megaraid-plugin"):
-                    if not linux.install_package("libstoragemgmt-megaraid-plugin", check=False):
-                        print("FATAL: Could not install LSM megaraid plugin")
+            elif 'megaraid' in self.protocol:
+                if not linux.is_installed('libstoragemgmt-megaraid-plugin'):
+                    if not linux.install_package('libstoragemgmt-megaraid-plugin', check=False):
+                        logging.critical('Could not install LSM megaraid plugin')
                     else:
                         requires_restart = True
                 # needs to install 3rd party tool
-                if not linux.install_package("storcli"):
-                    print("FATAL: Could not install storcli")
+                if not linux.install_package('storcli'):
+                    logging.critical('Could not install storcli')
 
         if requires_restart:
-            if run("service libstoragemgmt restart", verbose=True).returncode != 0:
-                print("FATAL: Could not restart libstoragemgmt service")
+            if run('service libstoragemgmt restart').rc != 0:
+                logging.critical('Could not restart libstoragemgmt service')
             else:
-                print("INFO: Waiting for service to restart.")
+                logging.info('Waiting for service to restart.')
                 sleep(5)
-        elif linux.service_status("libstoragemgmt") != 0:  # noqa: SIM102
-            if linux.service_start("libstoragemgmt"):
-                print("INFO: Waiting for service to start.")
+        elif linux.service_status('libstoragemgmt') != 0:  # noqa: SIM102
+            if linux.service_start('libstoragemgmt'):
+                logging.info('Waiting for service to start.')
                 sleep(5)
 
         self.commands: Dict[str, Union[str, List[str]]] = {
-            "list": "list",
-            "job_status": "job-status",
-            "capabilities": "capabilities",
-            "plugin_info": "plugin-info",
-            "volume_create": "volume-create",
-            "volume_raid_create": "volume-raid-create",
-            "volume_raid_create_cap": "volume-raid-create-cap",
-            "volume_delete": "volume-delete",
-            "volume_resize": "volume-resize",
-            "volume_replicate": "volume-replicate",
-            "volume_replicate_range": "volume-replicate-range",
-            "volume_replicate_range_block_size": "volume-replicate-range-block-size",
-            "volume_dependants": "volume-dependants",
-            "volume_dependants_rm": "volume-dependants-rm",
-            "volume_access_group": "volume-access-group",
-            "volume_mask": "volume-mask",
-            "volume_unmask": "volume-unmask",
-            "volume_enable": "volume-enable",
-            "volume_disable": "volume-disable",
-            "volume_raid_info": "volume-raid-info",
-            "volume_ident_led_on": "volume-ident-led-on",
-            "volume_ident_led_off": "volume-ident-led-off",
-            "system_read_cache_pct_update": "system-read-cache-pct-update",
-            "pool_member_info": "pool-member-info",
-            "access_group_create": "access-group-create",
-            "access_group_add": "access-group-add",
-            "access_group_remove": "access-group-remove",
-            "access_group_delete": "access-group-delete",
-            "access_group_volumes": "access-group-volumes",
-            "iscsi_chap": "iscsi-chap",
-            "fs_create": "fs-create",
-            "fs_delete": "fs-delete",
-            "fs_resize": "fs-resize",
-            "fs_export": "fs-export",
-            "fs_unexport": "fs-unexport",
-            "fs_clone": "fs-clone",
-            "fs_snap_create": "fs-snap-create",
-            "fs_snap_delete": "fs-snap-delete",
-            "fs_snap_restore": "fs-snap-restore",
-            "fs_dependants": "fs-dependants",
-            "fs_dependants_rm": "fs-dependants-rm",
-            "file_clone": "file-clone",
-            "local_disk_list": "local-disk-list",
-            "volume_cache_info": "volume-cache-info",
-            "volume_phy_disk_cache_update": "volume-phy-disk-cache-update",
-            "volume_read_cache_policy_update": "volume-read-cache-policy-update",
-            "volume_write_cache_policy_update": "volume-write-cache-policy-update",
-            "local_disk_ident_led_on": "local-disk-ident-led-on",
-            "local_disk_ident_led_off": "local-disk-ident-led-off",
-            "local_disk_fault_led_on": "local-disk-fault-led-on",
-            "local_disk_fault_led_off": "local-disk-fault-led-off",
+            'list': 'list',
+            'job_status': 'job-status',
+            'capabilities': 'capabilities',
+            'plugin_info': 'plugin-info',
+            'volume_create': 'volume-create',
+            'volume_raid_create': 'volume-raid-create',
+            'volume_raid_create_cap': 'volume-raid-create-cap',
+            'volume_delete': 'volume-delete',
+            'volume_resize': 'volume-resize',
+            'volume_replicate': 'volume-replicate',
+            'volume_replicate_range': 'volume-replicate-range',
+            'volume_replicate_range_block_size': 'volume-replicate-range-block-size',
+            'volume_dependants': 'volume-dependants',
+            'volume_dependants_rm': 'volume-dependants-rm',
+            'volume_access_group': 'volume-access-group',
+            'volume_mask': 'volume-mask',
+            'volume_unmask': 'volume-unmask',
+            'volume_enable': 'volume-enable',
+            'volume_disable': 'volume-disable',
+            'volume_raid_info': 'volume-raid-info',
+            'volume_ident_led_on': 'volume-ident-led-on',
+            'volume_ident_led_off': 'volume-ident-led-off',
+            'system_read_cache_pct_update': 'system-read-cache-pct-update',
+            'pool_member_info': 'pool-member-info',
+            'access_group_create': 'access-group-create',
+            'access_group_add': 'access-group-add',
+            'access_group_remove': 'access-group-remove',
+            'access_group_delete': 'access-group-delete',
+            'access_group_volumes': 'access-group-volumes',
+            'iscsi_chap': 'iscsi-chap',
+            'fs_create': 'fs-create',
+            'fs_delete': 'fs-delete',
+            'fs_resize': 'fs-resize',
+            'fs_export': 'fs-export',
+            'fs_unexport': 'fs-unexport',
+            'fs_clone': 'fs-clone',
+            'fs_snap_create': 'fs-snap-create',
+            'fs_snap_delete': 'fs-snap-delete',
+            'fs_snap_restore': 'fs-snap-restore',
+            'fs_dependants': 'fs-dependants',
+            'fs_dependants_rm': 'fs-dependants-rm',
+            'file_clone': 'file-clone',
+            'local_disk_list': 'local-disk-list',
+            'volume_cache_info': 'volume-cache-info',
+            'volume_phy_disk_cache_update': 'volume-phy-disk-cache-update',
+            'volume_read_cache_policy_update': 'volume-read-cache-policy-update',
+            'volume_write_cache_policy_update': 'volume-write-cache-policy-update',
+            'local_disk_ident_led_on': 'local-disk-ident-led-on',
+            'local_disk_ident_led_off': 'local-disk-ident-led-off',
+            'local_disk_fault_led_on': 'local-disk-fault-led-on',
+            'local_disk_fault_led_off': 'local-disk-fault-led-off',
         }
-        self.commands["all"] = list(self.commands.keys())
+        self.commands['all'] = list(self.commands.keys())
 
         self.arguments = {
-            "human": [self.commands["all"], " --human"],
-            "terse": [self.commands["all"], " --terse="],
-            "enum": [self.commands["all"], " --enum"],
-            "force": [self.commands["all"], " --force"],
-            "wait": [self.commands["all"], " --wait="],
-            "header": [self.commands["all"], " --header"],
-            "async": [self.commands["all"], " --b"],
-            "script": [self.commands["all"], " --script"],
-            "lsm_type": [["list"], " --type="],
-            "sys": [
+            'human': [self.commands['all'], ' --human'],
+            'terse': [self.commands['all'], ' --terse='],
+            'enum': [self.commands['all'], ' --enum'],
+            'force': [self.commands['all'], ' --force'],
+            'wait': [self.commands['all'], ' --wait='],
+            'header': [self.commands['all'], ' --header'],
+            'async': [self.commands['all'], ' --b'],
+            'script': [self.commands['all'], ' --script'],
+            'lsm_type': [['list'], ' --type='],
+            'sys': [
                 [
-                    "list",
-                    "capabilities",
-                    "volume_raid_create_cap",
-                    "volume_replicate_range_block_size",
-                    "system_read_cache_pct_update",
-                    "access_group_create",
+                    'list',
+                    'capabilities',
+                    'volume_raid_create_cap',
+                    'volume_replicate_range_block_size',
+                    'system_read_cache_pct_update',
+                    'access_group_create',
                 ],
-                " --sys=",
+                ' --sys=',
             ],
-            "pool": [
+            'pool': [
                 [
-                    "list",
-                    "volume_create",
-                    "volume_replicate",
-                    "pool_member_info",
-                    "fs_create",
+                    'list',
+                    'volume_create',
+                    'volume_replicate',
+                    'pool_member_info',
+                    'fs_create',
                 ],
-                " --pool=",
+                ' --pool=',
             ],
-            "vol": [
+            'vol': [
                 [
-                    "list",
-                    "volume_delete",
-                    "volume_resize",
-                    "volume_replicate",
-                    "volume_dependants",
-                    "volume_dependants_rm",
-                    "volume_access_group",
-                    "volume_mask",
-                    "volume_unmask",
-                    "volume_enable",
-                    "volume_disable",
-                    "volume_raid_info",
-                    "volume_ident_led_on",
-                    "volume_ident_led_off",
-                    "volume_cache_info",
-                    "volume_phy_disk_cache_update",
-                    "volume_read_cache_policy_update",
-                    "volume_read_cache_policy_update",
+                    'list',
+                    'volume_delete',
+                    'volume_resize',
+                    'volume_replicate',
+                    'volume_dependants',
+                    'volume_dependants_rm',
+                    'volume_access_group',
+                    'volume_mask',
+                    'volume_unmask',
+                    'volume_enable',
+                    'volume_disable',
+                    'volume_raid_info',
+                    'volume_ident_led_on',
+                    'volume_ident_led_off',
+                    'volume_cache_info',
+                    'volume_phy_disk_cache_update',
+                    'volume_read_cache_policy_update',
+                    'volume_read_cache_policy_update',
                 ],
-                " --vol=",
+                ' --vol=',
             ],
-            "disk": [["list", "volume_raid_create"], " --disk="],
-            "ag": [
+            'disk': [['list', 'volume_raid_create'], ' --disk='],
+            'ag': [
                 [
-                    "list",
-                    "volume_mask",
-                    "volume_unmask",
-                    "access_group_add",
-                    "access_group_remove",
-                    "access_group_delete",
-                    "access_group_volumes",
+                    'list',
+                    'volume_mask',
+                    'volume_unmask',
+                    'access_group_add',
+                    'access_group_remove',
+                    'access_group_delete',
+                    'access_group_volumes',
                 ],
-                " --ag=",
+                ' --ag=',
             ],
-            "fs": [
+            'fs': [
                 [
-                    "list",
-                    "fs_delete",
-                    "fs_resize",
-                    "fs_export",
-                    "fs_snap_create",
-                    "fs_snap_delete",
-                    "fs_snap_restore",
-                    "fs_dependants",
-                    "fs_dependants_rm",
-                    "file_clone",
+                    'list',
+                    'fs_delete',
+                    'fs_resize',
+                    'fs_export',
+                    'fs_snap_create',
+                    'fs_snap_delete',
+                    'fs_snap_restore',
+                    'fs_dependants',
+                    'fs_dependants_rm',
+                    'file_clone',
                 ],
-                " --fs=",
+                ' --fs=',
             ],
-            "nfs_export": [["list"], " --nfs-export="],
-            "tgt": [["list"], " --tgt="],
-            "job": [["job_status"], " --job="],
-            "name": [
+            'nfs_export': [['list'], ' --nfs-export='],
+            'tgt': [['list'], ' --tgt='],
+            'job': [['job_status'], ' --job='],
+            'name': [
                 [
-                    "volume_create",
-                    "volume_raid_create",
-                    "volume_replicate",
-                    "access_group_create",
-                    "fs_create",
-                    "fs_snap_create",
+                    'volume_create',
+                    'volume_raid_create',
+                    'volume_replicate',
+                    'access_group_create',
+                    'fs_create',
+                    'fs_snap_create',
                 ],
-                " --name=",
+                ' --name=',
             ],
-            "size": [
-                ["volume_create", "volume_resize", "fs_create", "fs_resize"],
-                " --size=",
-            ],
-            "provisioning": [["volume_create"], " --provisioning="],
-            "raid_type": [["volume_raid_create"], " --raid-type="],
-            "strip_size": [["volume_raid_create"], " --strip-size="],
-            "rep_type": [
-                ["volume_replicate", "volume_replicate_range"],
-                " --rep-type=",
-            ],
-            "src_vol": [["volume_replicate_range"], " --src-vol="],
-            "dst_vol": [["volume_replicate_range"], " --dst-vol="],
-            "src_start": [["volume_replicate_range"], " --src-start="],
-            "dst_start": [["volume_replicate_range"], " --dst-start="],
-            "count": [["volume_replicate_range"], " --count="],
-            "read_pct": [["system_read_cache_pct_update"], " --read-pct="],
-            "init": [
+            'size': [
+                ['volume_create', 'volume_resize', 'fs_create', 'fs_resize'],
+                ' --size=',
+            ],
+            'provisioning': [['volume_create'], ' --provisioning='],
+            'raid_type': [['volume_raid_create'], ' --raid-type='],
+            'strip_size': [['volume_raid_create'], ' --strip-size='],
+            'rep_type': [
+                ['volume_replicate', 'volume_replicate_range'],
+                ' --rep-type=',
+            ],
+            'src_vol': [['volume_replicate_range'], ' --src-vol='],
+            'dst_vol': [['volume_replicate_range'], ' --dst-vol='],
+            'src_start': [['volume_replicate_range'], ' --src-start='],
+            'dst_start': [['volume_replicate_range'], ' --dst-start='],
+            'count': [['volume_replicate_range'], ' --count='],
+            'read_pct': [['system_read_cache_pct_update'], ' --read-pct='],
+            'init': [
                 [
-                    "access_group_create",
-                    "access_group_add",
-                    "access_group_remove",
-                    "iscsi_chap",
+                    'access_group_create',
+                    'access_group_add',
+                    'access_group_remove',
+                    'iscsi_chap',
                 ],
-                " --init=",
+                ' --init=',
             ],
-            "in_user": [["iscsi_chap"], " --in-user="],
-            "in_pass": [["iscsi_chap"], " --in-pass="],
-            "out_user": [["iscsi_chap"], " --out-user="],
-            "out_pass": [["iscsi_chap"], " --out-pass="],
-            "export_path": [["iscsi_chap"], " --exportpath="],
-            "anonuid": [["fs_export"], " --anonuid="],
-            "anongid": [["fs_export"], " --anongid="],
-            "auth_type": [["fs_export"], " --auth-type="],
-            "root_host": [["fs_export"], " --root-host="],
-            "ro_host": [["fs_export"], " --ro-host="],
-            "rw_host": [["fs_export"], " --rw-host="],
-            "export": [["fs_unexport"], " --export="],
-            "src_fs": [["fs_clone"], " --src-fs="],
-            "dst_name": [["fs_clone"], " --dst-name="],
-            "backing_snapshot": [["fs_clone", "file_clone"], " --backing-snapshot="],
-            "snap": [["fs_snap_delete", "fs_snap_restore"], " --snap="],
-            "lsm_file": [
-                ["fs_snap_restore", "fs_dependants", "fs_dependants_rm"],
-                " --file=",
-            ],
-            "fileas": [["fs_snap_restore"], " --fileas="],
-            "src": [["file_clone"], " --src"],
-            "dst": [["file_clone"], " --dst"],
-            "policy": [
+            'in_user': [['iscsi_chap'], ' --in-user='],
+            'in_pass': [['iscsi_chap'], ' --in-pass='],
+            'out_user': [['iscsi_chap'], ' --out-user='],
+            'out_pass': [['iscsi_chap'], ' --out-pass='],
+            'export_path': [['iscsi_chap'], ' --exportpath='],
+            'anonuid': [['fs_export'], ' --anonuid='],
+            'anongid': [['fs_export'], ' --anongid='],
+            'auth_type': [['fs_export'], ' --auth-type='],
+            'root_host': [['fs_export'], ' --root-host='],
+            'ro_host': [['fs_export'], ' --ro-host='],
+            'rw_host': [['fs_export'], ' --rw-host='],
+            'export': [['fs_unexport'], ' --export='],
+            'src_fs': [['fs_clone'], ' --src-fs='],
+            'dst_name': [['fs_clone'], ' --dst-name='],
+            'backing_snapshot': [['fs_clone', 'file_clone'], ' --backing-snapshot='],
+            'snap': [['fs_snap_delete', 'fs_snap_restore'], ' --snap='],
+            'lsm_file': [
+                ['fs_snap_restore', 'fs_dependants', 'fs_dependants_rm'],
+                ' --file=',
+            ],
+            'fileas': [['fs_snap_restore'], ' --fileas='],
+            'src': [['file_clone'], ' --src'],
+            'dst': [['file_clone'], ' --dst'],
+            'policy': [
                 [
-                    "volume_phy_disk_cache_update",
-                    "volume_read_cache_policy_update",
-                    "volume_read_cache_policy_update",
+                    'volume_phy_disk_cache_update',
+                    'volume_read_cache_policy_update',
+                    'volume_read_cache_policy_update',
                 ],
-                " --policy=",
+                ' --policy=',
             ],
-            "path": [
+            'path': [
                 [
-                    "local_disk_ident_led_on",
-                    "local_disk_ident_led_off",
-                    "local_disk_fault_led_on",
-                    "local_disk_fault_led_on",
+                    'local_disk_ident_led_on',
+                    'local_disk_ident_led_off',
+                    'local_disk_fault_led_on',
+                    'local_disk_fault_led_on',
                 ],
-                " --path=",
+                ' --path=',
             ],
         }
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
-        print("INFO: LSM configured")
+        logging.info('LSM configured')
 
     def _check(self, cmd):  # noqa: ANN001, ANN202
         if self.disable_check or cmd:
             # Do not check if checking is disabled
             return True
 
         return True
 
-    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):  # noqa: ANN001, ANN003, ANN202
+    def _run(self, cmd, return_output=False, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
 
         ret_fail = False
         if return_output:
             ret_fail = (False, None)
 
         try:
             command = self._add_command(cmd)
             command = self._add_arguments(command, **kwargs)
 
         except WrongCommandExceptionError as e:
-            print(f"WARN: Given command '{e.command}' is not allowed in this version.")
+            logging.warning(f"Given command '{e.command}' is not allowed in this version.")
             return ret_fail
         except WrongArgumentExceptionError as e:
             message = f"WARN: Given argument '{e.argument}' is not allowed for given command."
             if e.command:
                 message = message[:-1] + " '" + e.command + "'."
             if e.arguments:
                 message += f"\nPlease use only these: {', '.join(e.arguments)}."
             print(message)
             return ret_fail
 
-        cmd = "lsmcli "
+        cmd = 'lsmcli '
         if self.timeout:
-            cmd += f"-w {self.timeout} "
+            cmd += f'-w {self.timeout} '
         if self.protocol:
             cmd += f'-u "{self.protocol}://'
             if self.username and self.target:
-                cmd += f"{self.username}@{self.target}"
+                cmd += f'{self.username}@{self.target}'
             if self.port:
-                cmd += f":{self.port}"
+                cmd += f':{self.port}'
             if self.query_params:
-                cmd += f"{self.query_params}"
+                cmd += f'{self.query_params}'
             cmd += '" '
         cmd += command
 
         try:
             self._check(cmd)
         except WrongArgumentExceptionError:
             pass
         except FailedCheckExceptionError as e:
-            print(f"WARN: Failed checking on argument {e.argument}")
+            logging.warning(f'Failed checking on argument {e.argument}')
             return ret_fail
 
         if return_output:
-            ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
+            ret, data = run_ret_out(cmd, return_output=True)
             if ret != 0:
-                print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+                logging.warning(f"Running command: '{cmd}' failed. Return with output.")
             return ret, data
 
-        ret = run(cmd, verbose=verbosity).returncode
+        ret = run(cmd).rc
         if ret != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+            logging.warning(f"Running command: '{cmd}' failed.")
         return ret
 
     @staticmethod
     def _remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     @_cli
@@ -567,235 +568,235 @@
         ag=None,  # noqa: ANN001
         nfs_export=None,  # noqa: ANN001
         tgt=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
-                "lsm_type": lsm_type,
-                "fs": fs,
-                "sys": sys,
-                "pool": pool,
-                "vol": vol,
-                "disk": disk,
-                "ag": ag,
-                "nfs_export": nfs_export,
-                "tgt": tgt,
+                'lsm_type': lsm_type,
+                'fs': fs,
+                'sys': sys,
+                'pool': pool,
+                'vol': vol,
+                'disk': disk,
+                'ag': ag,
+                'nfs_export': nfs_export,
+                'tgt': tgt,
             },
         )
-        return self._run("list", **self._remove_nones(kwargs))
+        return self._run('list', **self._remove_nones(kwargs))
 
     @_cli
     def job_status(self, job=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"job": job})
-        return self._run("job_status", **self._remove_nones(kwargs))
+        kwargs.update({'job': job})
+        return self._run('job_status', **self._remove_nones(kwargs))
 
     @_cli
     def capabilities(self, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"sys": sys})
-        return self._run("capabilities", **self._remove_nones(kwargs))
+        kwargs.update({'sys': sys})
+        return self._run('capabilities', **self._remove_nones(kwargs))
 
     @_cli
     def plugin_info(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("plugin_info", **self._remove_nones(kwargs))
+        return self._run('plugin_info', **self._remove_nones(kwargs))
 
     @_cli
     def volume_create(  # noqa: ANN201
         self,
         name=None,  # noqa: ANN001
         size=None,  # noqa: ANN001
         pool=None,  # noqa: ANN001
         provisioning=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        kwargs.update({"name": name, "size": size, "pool": pool, "provisioning": provisioning})
-        return self._run("volume_create", **self._remove_nones(kwargs))
+        kwargs.update({'name': name, 'size': size, 'pool': pool, 'provisioning': provisioning})
+        return self._run('volume_create', **self._remove_nones(kwargs))
 
     @_cli
     def volume_raid_create(  # noqa: ANN201
         self,
         name=None,  # noqa: ANN001
         raid_type=None,  # noqa: ANN001
         disk=None,  # noqa: ANN001
         strip_size=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
-                "name": name,
-                "raid_type": raid_type,
-                "disk": disk,
-                "strip_size": strip_size,
+                'name': name,
+                'raid_type': raid_type,
+                'disk': disk,
+                'strip_size': strip_size,
             },
         )
-        return self._run("volume_raid_create", **self._remove_nones(kwargs))
+        return self._run('volume_raid_create', **self._remove_nones(kwargs))
 
     @_cli
     def volume_raid_create_cap(self, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"sys": sys})
-        return self._run("volume_raid_create_cap", **self._remove_nones(kwargs))
+        kwargs.update({'sys': sys})
+        return self._run('volume_raid_create_cap', **self._remove_nones(kwargs))
 
     @_cli
     def volume_ident_led_on(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_ident_led_on", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_ident_led_on', **self._remove_nones(kwargs))
 
     @_cli
     def volume_ident_led_off(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_ident_led_off", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_ident_led_off', **self._remove_nones(kwargs))
 
     @_cli
     def volume_delete(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_delete", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_delete', **self._remove_nones(kwargs))
 
     @_cli
     def volume_resize(self, vol=None, size=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "size": size})
-        return self._run("volume_resize", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'size': size})
+        return self._run('volume_resize', **self._remove_nones(kwargs))
 
     @_cli
     def volume_replicate(self, vol=None, name=None, rep_type=None, pool=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "name": name, "rep_type": rep_type, "pool": pool})
-        return self._run("volume_replicate", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'name': name, 'rep_type': rep_type, 'pool': pool})
+        return self._run('volume_replicate', **self._remove_nones(kwargs))
 
     @_cli
     def volume_replicate_range(  # noqa: ANN201
         self,
         src_vol=None,  # noqa: ANN001
         dst_vol=None,  # noqa: ANN001
         rep_type=None,  # noqa: ANN001
         src_start=None,  # noqa: ANN001
         dst_start=None,  # noqa: ANN001
         count=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
-                "src_vol": src_vol,
-                "dst_vol": dst_vol,
-                "rep_type": rep_type,
-                "src_start": src_start,
-                "dst_start": dst_start,
-                "count": count,
+                'src_vol': src_vol,
+                'dst_vol': dst_vol,
+                'rep_type': rep_type,
+                'src_start': src_start,
+                'dst_start': dst_start,
+                'count': count,
             },
         )
-        return self._run("volume_replicate_range", **self._remove_nones(kwargs))
+        return self._run('volume_replicate_range', **self._remove_nones(kwargs))
 
     @_cli
     def volume_replicate_range_block_size(self, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"sys": sys})
-        return self._run("volume_replicate_range_block_size", **self._remove_nones(kwargs))
+        kwargs.update({'sys': sys})
+        return self._run('volume_replicate_range_block_size', **self._remove_nones(kwargs))
 
     @_cli
     def volume_dependants(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_dependants", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_dependants', **self._remove_nones(kwargs))
 
     @_cli
     def volume_dependants_rm(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_dependants_rm", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_dependants_rm', **self._remove_nones(kwargs))
 
     @_cli
     def volume_access_group(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_access_group", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_access_group', **self._remove_nones(kwargs))
 
     @_cli
     def volume_mask(self, vol=None, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "ag": ag})
-        return self._run("volume_mask", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'ag': ag})
+        return self._run('volume_mask', **self._remove_nones(kwargs))
 
     @_cli
     def volume_unmask(self, vol=None, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "ag": ag})
-        return self._run("volume_unmask", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'ag': ag})
+        return self._run('volume_unmask', **self._remove_nones(kwargs))
 
     @_cli
     def volume_enable(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_enable", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_enable', **self._remove_nones(kwargs))
 
     @_cli
     def volume_disable(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_disable", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_disable', **self._remove_nones(kwargs))
 
     @_cli
     def volume_raid_info(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_raid_info", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_raid_info', **self._remove_nones(kwargs))
 
     @_cli
     def pool_member_info(self, pool=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"pool": pool})
-        return self._run("pool_member_info", **self._remove_nones(kwargs))
+        kwargs.update({'pool': pool})
+        return self._run('pool_member_info', **self._remove_nones(kwargs))
 
     @_cli
     def access_group_create(self, name=None, init=None, sys=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"name": name, "init": init, "sys": sys})
-        return self._run("access_group_create", **self._remove_nones(kwargs))
+        kwargs.update({'name': name, 'init': init, 'sys': sys})
+        return self._run('access_group_create', **self._remove_nones(kwargs))
 
     @_cli
     def access_group_add(self, ag=None, init=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"ag": ag, "init": init})
-        return self._run("access_group_add", **self._remove_nones(kwargs))
+        kwargs.update({'ag': ag, 'init': init})
+        return self._run('access_group_add', **self._remove_nones(kwargs))
 
     @_cli
     def access_group_remove(self, ag=None, init=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"ag": ag, "init": init})
-        return self._run("access_group_remove", **self._remove_nones(kwargs))
+        kwargs.update({'ag': ag, 'init': init})
+        return self._run('access_group_remove', **self._remove_nones(kwargs))
 
     @_cli
     def access_group_delete(self, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"ag": ag})
-        return self._run("access_group_delete", **self._remove_nones(kwargs))
+        kwargs.update({'ag': ag})
+        return self._run('access_group_delete', **self._remove_nones(kwargs))
 
     @_cli
     def access_group_volumes(self, ag=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"ag": ag})
-        return self._run("access_group_volumes", **self._remove_nones(kwargs))
+        kwargs.update({'ag': ag})
+        return self._run('access_group_volumes', **self._remove_nones(kwargs))
 
     @_cli
     def iscsi_chap(  # noqa: ANN201
         self,
         init=None,  # noqa: ANN001
         in_user=None,  # noqa: ANN001
         in_pass=None,  # noqa: ANN001
         out_user=None,  # noqa: ANN001
         out_pass=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
-                "init": init,
-                "in_user": in_user,
-                "in_pass": in_pass,
-                "out_user": out_user,
-                "out_pass": out_pass,
+                'init': init,
+                'in_user': in_user,
+                'in_pass': in_pass,
+                'out_user': out_user,
+                'out_pass': out_pass,
             },
         )
-        return self._run("iscsi_chap", **self._remove_nones(kwargs))
+        return self._run('iscsi_chap', **self._remove_nones(kwargs))
 
     @_cli
     def fs_create(self, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs})
-        return self._run("fs_create", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs})
+        return self._run('fs_create', **self._remove_nones(kwargs))
 
     @_cli
     def fs_delete(self, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs})
-        return self._run("fs_delete", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs})
+        return self._run('fs_delete', **self._remove_nones(kwargs))
 
     @_cli
     def fs_resize(self, fs=None, size=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs, "size": size})
-        return self._run("fs_resize", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs, 'size': size})
+        return self._run('fs_resize', **self._remove_nones(kwargs))
 
     @_cli
     def fs_export(  # noqa: ANN201
         self,
         fs=None,  # noqa: ANN001
         exportpath=None,  # noqa: ANN001
         anonguid=None,  # noqa: ANN001
@@ -804,145 +805,145 @@
         root_host=None,  # noqa: ANN001
         ro_host=None,  # noqa: ANN001
         rw_host=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
         kwargs.update(
             {
-                "fs": fs,
-                "exportpath": exportpath,
-                "anonguid": anonguid,
-                "anongid": anongid,
-                "auth_type": auth_type,
-                "root_host": root_host,
-                "ro_host": ro_host,
-                "rw_host": rw_host,
+                'fs': fs,
+                'exportpath': exportpath,
+                'anonguid': anonguid,
+                'anongid': anongid,
+                'auth_type': auth_type,
+                'root_host': root_host,
+                'ro_host': ro_host,
+                'rw_host': rw_host,
             },
         )
-        return self._run("fs_export", **self._remove_nones(kwargs))
+        return self._run('fs_export', **self._remove_nones(kwargs))
 
     @_cli
     def fs_unexport(self, export=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"export": export})
-        return self._run("fs_unexport", **self._remove_nones(kwargs))
+        kwargs.update({'export': export})
+        return self._run('fs_unexport', **self._remove_nones(kwargs))
 
     @_cli
     def fs_clone(self, src_fs=None, dst_name=None, backing_snapshot=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
         kwargs.update(
             {
-                "src_fs": src_fs,
-                "dst_name": dst_name,
-                "backing_snapshot": backing_snapshot,
+                'src_fs': src_fs,
+                'dst_name': dst_name,
+                'backing_snapshot': backing_snapshot,
             },
         )
-        return self._run("fs_clone", **self._remove_nones(kwargs))
+        return self._run('fs_clone', **self._remove_nones(kwargs))
 
     @_cli
     def fs_snap_create(self, name=None, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"name": name, "fs": fs})
-        return self._run("fs_snap_create", **self._remove_nones(kwargs))
+        kwargs.update({'name': name, 'fs': fs})
+        return self._run('fs_snap_create', **self._remove_nones(kwargs))
 
     @_cli
     def fs_snap_delete(self, snap=None, fs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"snap": snap, "fs": fs})
-        return self._run("fs_snap_delete", **self._remove_nones(kwargs))
+        kwargs.update({'snap': snap, 'fs': fs})
+        return self._run('fs_snap_delete', **self._remove_nones(kwargs))
 
     @_cli
     def fs_snap_restore(self, fs=None, snap=None, lsm_file=None, fileas=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs, "snap": snap, "lsm_file": lsm_file, "fileas": fileas})
-        return self._run("fs_snap_restore", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs, 'snap': snap, 'lsm_file': lsm_file, 'fileas': fileas})
+        return self._run('fs_snap_restore', **self._remove_nones(kwargs))
 
     @_cli
     def fs_dependants(self, fs=None, lsm_file=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs, "lsm_file": lsm_file})
-        return self._run("fs_dependants", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs, 'lsm_file': lsm_file})
+        return self._run('fs_dependants', **self._remove_nones(kwargs))
 
     @_cli
     def fs_dependants_rm(self, fs=None, lsm_file=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs, "lsm_file": lsm_file})
-        return self._run("fs_dependants_rm", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs, 'lsm_file': lsm_file})
+        return self._run('fs_dependants_rm', **self._remove_nones(kwargs))
 
     @_cli
     def file_clone(self, fs=None, src=None, dst=None, backing_snapshot=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"fs": fs, "src": src, "dst": dst, "backing_snapshot": backing_snapshot})
-        return self._run("file_clone", **self._remove_nones(kwargs))
+        kwargs.update({'fs': fs, 'src': src, 'dst': dst, 'backing_snapshot': backing_snapshot})
+        return self._run('file_clone', **self._remove_nones(kwargs))
 
     @_cli
     def system_read_cache_pct_update(self, sys=None, read_pct=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"sys": sys, "read_pct": read_pct})
-        return self._run("system_read_cache_pct_update", **self._remove_nones(kwargs))
+        kwargs.update({'sys': sys, 'read_pct': read_pct})
+        return self._run('system_read_cache_pct_update', **self._remove_nones(kwargs))
 
     @_cli
     def local_disk_list(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("local_disk_list", **self._remove_nones(kwargs))
+        return self._run('local_disk_list', **self._remove_nones(kwargs))
 
     @_cli
     def volume_cache_info(self, vol=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol})
-        return self._run("volume_cache_info", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol})
+        return self._run('volume_cache_info', **self._remove_nones(kwargs))
 
     @_cli
     def volume_phy_disk_cache_update(self, vol=None, policy=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "policy": policy})
-        return self._run("volume_phy_disk_cache_update", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'policy': policy})
+        return self._run('volume_phy_disk_cache_update', **self._remove_nones(kwargs))
 
     @_cli
     def volume_read_cache_policy_update(self, vol=None, policy=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "policy": policy})
-        return self._run("volume_read_cache_policy_update", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'policy': policy})
+        return self._run('volume_read_cache_policy_update', **self._remove_nones(kwargs))
 
     @_cli
     def volume_write_cache_policy_update(self, vol=None, policy=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"vol": vol, "policy": policy})
-        return self._run("volume_write_cache_policy_update", **self._remove_nones(kwargs))
+        kwargs.update({'vol': vol, 'policy': policy})
+        return self._run('volume_write_cache_policy_update', **self._remove_nones(kwargs))
 
     @_cli
     def local_disk_ident_led_on(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"path": path})
-        return self._run("local_disk_ident_led_on", **self._remove_nones(kwargs))
+        kwargs.update({'path': path})
+        return self._run('local_disk_ident_led_on', **self._remove_nones(kwargs))
 
     @_cli
     def local_disk_ident_led_off(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"path": path})
-        return self._run("local_disk_ident_led_off", **self._remove_nones(kwargs))
+        kwargs.update({'path': path})
+        return self._run('local_disk_ident_led_off', **self._remove_nones(kwargs))
 
     @_cli
     def local_disk_fault_led_on(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"path": path})
-        return self._run("local_disk_fault_led_on", **self._remove_nones(kwargs))
+        kwargs.update({'path': path})
+        return self._run('local_disk_fault_led_on', **self._remove_nones(kwargs))
 
     @_cli
     def local_disk_fault_led_off(self, path=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        kwargs.update({"path": path})
-        return self._run("local_disk_fault_led_off", **self._remove_nones(kwargs))
+        kwargs.update({'path': path})
+        return self._run('local_disk_fault_led_off', **self._remove_nones(kwargs))
 
-    def help(self, cmd=""):  # noqa: A003, ANN001, ANN201
+    def help(self, cmd=''):  # noqa: A003, ANN001, ANN201
         """Retrieve help.
         The arguments are:
         cmd - optional | get help on this command
         Returns:
         Boolean:
         True if success
         False in case of failure.
         """
         if cmd and cmd not in list(self.commands.keys()):
-            print(f"FAIL: Unknown command {cmd}.")
+            logging.error(f'Unknown command {cmd}.')
             return False
 
         command = f"{cmd.replace('_', '-')} -h"
-        return run(command, verbose=True)
+        return run(command)
 
-    def version(self, cmd=""):  # noqa: ANN001, ANN201
+    def version(self, cmd=''):  # noqa: ANN001, ANN201
         """Retrieve plugin version.
         The arguments are:
         cmd - optional | get version of this command
         Returns:
         Boolean:
         True if success
         False in case of failure.
         """
         if cmd and cmd not in list(self.commands.keys()):
-            print(f"FAIL: Unknown command {cmd}.")
+            logging.error(f'Unknown command {cmd}.')
             return False
 
         command = f"{cmd.replace('_', '-')} -v"
-        return run(command, verbose=True)
+        return run(command)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/lvm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,133 @@
 """lvm.py: Module with test specific method for LVM."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import fileinput
+import logging
 import re
 from functools import wraps
 from pathlib import Path
 from typing import Dict, List, Union
 
 from sts import vdo
 from sts.utils.cli_tools import Wrapper
 from sts.utils.cmdline import run, run_ret_out
 
 
 def check_lv_expected_value(test_obj, lv_name, vg_name, opt_val_dict):  # noqa: ANN001, ANN201
     if not test_obj or not opt_val_dict or not lv_name or not vg_name:
         return
 
-    opt_str = ",".join(opt_val_dict)
+    opt_str = ','.join(opt_val_dict)
     lv = lv_info(lv_name, vg_name, options=opt_str)
     if not lv:
-        test_obj.tfail(f"{vg_name}/{lv_name} does not exist")
-        run(f"lvs -a -o +{opt_str}")
+        test_obj.tfail(f'{vg_name}/{lv_name} does not exist')
+        run(f'lvs -a -o +{opt_str}')
         return
     for opt in opt_val_dict:
         if lv[opt] == opt_val_dict[opt]:
-            test_obj.tpass(f"{vg_name}/{lv_name} {opt} == {opt_val_dict[opt]}")
+            test_obj.tpass(f'{vg_name}/{lv_name} {opt} == {opt_val_dict[opt]}')
             continue
 
-        if test_obj.tfail(f"{vg_name}/{lv_name} {opt} == {lv[opt]}, but expected {opt_val_dict[opt]}"):
+        if test_obj.tfail(f'{vg_name}/{lv_name} {opt} == {lv[opt]}, but expected {opt_val_dict[opt]}'):
             print(lv)
-            run(f"lvs -a -o +{opt_str}")
+            run(f'lvs -a -o +{opt_str}')
             continue
 
 
 ###########################################
 # PV section
 ###########################################
-def pv_query(verbose=False):  # noqa: ANN001, ANN201
+def pv_query():  # noqa: ANN201
     """Query Physical Volumes and return a dictionary with PV information for each PV.
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with PV info for each PV.
     """
     cmd = 'pvs --noheadings --separator ","'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("INFO: there is no VGs")
+        logging.info('there is no VGs')
         return None
-    pvs = output.split("\n")
+    pvs = output.split('\n')
 
     # format of PV info: PV,VG,Fmt,Attr,PSize,PFree
-    pv_info_regex = r"\s+(\S+),(\S+)?,(\S+),(.*),(.*),(.*)$"
+    pv_info_regex = r'\s+(\S+),(\S+)?,(\S+),(.*),(.*),(.*)$'
 
     pv_dict = {}
     for pv in pvs:
         m = re.match(pv_info_regex, pv)
         if not m:
-            # print("WARN: (%s) does not match vgdisplay output format" % vg)
+            # logging.warning("(%s) does not match vgdisplay output format" % vg)
             continue
         pv_info_dict = {
-            "vg": m.group(2),
-            "fmt": m.group(3),  # not sure what it is
-            "attr": m.group(4),
-            "psize": m.group(5),
-            "pfree": m.group(6),
+            'vg': m.group(2),
+            'fmt': m.group(3),  # not sure what it is
+            'attr': m.group(4),
+            'psize': m.group(5),
+            'pfree': m.group(6),
         }
         pv_dict[m.group(1)] = pv_info_dict
 
     return pv_dict
 
 
-def pv_create(pv_name: str, options="", verbose=True):  # noqa: ANN001, ANN201
+def pv_create(pv_name: str, options=''):  # noqa: ANN001, ANN201
     """Create a Volume Group.
     The arguments are:
     PV name
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not pv_name:
-        print("FAIL: pv_create requires pv_name")
+        logging.error('pv_create requires pv_name')
         return False
-    cmd = f"pvcreate {options} {pv_name}"
-    if run(cmd, verbose=verbose).returncode != 0:
+    cmd = f'pvcreate {options} {pv_name}'
+    if run(cmd).rc != 0:
         # print ("FAIL: Could not create %s" % pv_name)
         return False
     return True
 
 
-def pv_remove(pv_name: str, force=None, verbose=True) -> bool:  # noqa: ANN001
+def pv_remove(pv_name: str, force=None) -> bool:  # noqa: ANN001
     """Delete a Volume Group.
     The arguments are:
     VG name
     force (boolean)
     verbose (boolean).
 
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not pv_name:
-        print("FAIL: pv_remove requires pv_name")
+        logging.error('pv_remove requires pv_name')
         return False
 
     pv_dict = pv_query()
 
     pv_names = pv_name.split()
     for pv_name in pv_names:
         if pv_name not in list(pv_dict.keys()):
-            print(f"INFO: pv_remove - {pv_name} does not exist. Skipping...")
+            logging.info(f'pv_remove - {pv_name} does not exist. Skipping...')
             return True
 
-        options = ""
+        options = ''
         if force:
-            options += "--force --force"
-        cmd = f"pvremove {options} {pv_name}"
-        retcode = run(cmd, verbose=verbose).returncode
+            options += '--force --force'
+        cmd = f'pvremove {options} {pv_name}'
+        retcode = run(cmd).rc
         if retcode != 0:
-            print(f"FAIL: Could not delete {pv_name}")
+            logging.error(f'Could not delete {pv_name}')
             return False
     return True
 
 
 ###########################################
 # VG section
 ###########################################
@@ -137,106 +138,106 @@
     The arguments are:
     None
     Returns:
     True
     or
     False.
     """
-    cmd = "vgs -a"
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not show VGs")
+    cmd = 'vgs -a'
+    if run(cmd).rc != 0:
+        logging.error('Could not show VGs')
         return False
     return True
 
 
-def vg_query(verbose=False):  # noqa: ANN001, ANN201
+def vg_query():  # noqa: ANN201
     """Query Volume Groups and return a dictonary with VG information for each VG.
     The arguments are:
     None
     Returns:
     dict: Return a dictionary with VG info for each VG.
     """
     cmd = 'vgs --noheadings --separator ","'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("INFO: there is no VGs")
+        logging.info('there is no VGs')
         return None
-    vgs = output.split("\n")
+    vgs = output.split('\n')
 
     # format of VG info: name #PV #LV #SN Attr VSize VFree
-    vg_info_regex = r"\s+(\S+),(\S+),(\S+),(.*),(.*),(.*),(.*)$"
+    vg_info_regex = r'\s+(\S+),(\S+),(\S+),(.*),(.*),(.*),(.*)$'
 
     vg_dict = {}
     for vg in vgs:
         m = re.match(vg_info_regex, vg)
         if not m:
-            # print("WARN: (%s) does not match vgdisplay output format" % vg)
+            # logging.warning("(%s) does not match vgdisplay output format" % vg)
             continue
         vg_info_dict = {
-            "num_pvs": m.group(2),
-            "num_lvs": m.group(3),
-            "num_sn": m.group(4),  # not sure what it is
-            "attr": m.group(5),
-            "vsize": m.group(6),
-            "vfree": m.group(7),
+            'num_pvs': m.group(2),
+            'num_lvs': m.group(3),
+            'num_sn': m.group(4),  # not sure what it is
+            'attr': m.group(5),
+            'vsize': m.group(6),
+            'vfree': m.group(7),
         }
         vg_dict[m.group(1)] = vg_info_dict
 
     return vg_dict
 
 
-def vg_create(vg_name: str, pv_name: str, force=False, verbose=True):  # noqa: ANN001, ANN201
+def vg_create(vg_name: str, pv_name: str, force=False):  # noqa: ANN001, ANN201
     """Create a Volume Group.
     The arguments are:
     PV name
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not vg_name or not pv_name:
-        print("FAIL: vg_create requires vg_name and pv_name")
+        logging.error('vg_create requires vg_name and pv_name')
         return False
 
-    options = ""
+    options = ''
     if force:
-        options += "--force"
-    cmd = f"vgcreate {options} {vg_name} {pv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+        options += '--force'
+    cmd = f'vgcreate {options} {vg_name} {pv_name}'
+    retcode = run(cmd).rc
     if retcode != 0:
         # print ("FAIL: Could not create %s" % vg_name)
         return False
     return True
 
 
-def vg_remove(vg_name: str, force=False, verbose=True):  # noqa: ANN001, ANN201
+def vg_remove(vg_name: str, force=False):  # noqa: ANN001, ANN201
     """Delete a Volume Group.
     The arguments are:
     VG name
     force (boolean).
 
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not vg_name:
-        print("FAIL: vg_remove requires vg_name")
+        logging.error('vg_remove requires vg_name')
         return False
 
     vg_dict = vg_query()
     if vg_name not in list(vg_dict.keys()):
-        print(f"INFO: vg_remove - {vg_name} does not exist. Skipping...")
+        logging.info(f'vg_remove - {vg_name} does not exist. Skipping...')
         return True
 
-    options = ""
+    options = ''
     if force:
-        options += "--force"
-    cmd = f"vgremove {options} {vg_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+        options += '--force'
+    cmd = f'vgremove {options} {vg_name}'
+    retcode = run(cmd).rc
     if retcode != 0:
         # print ("FAIL: Could not delete %s" % vg_name)
         return False
     return True
 
 
 ###########################################
@@ -249,357 +250,357 @@
     The arguments are:
     None
     Returns:
     True
     or
     False.
     """
-    cmd = "lvs -a"
-    if run(cmd).returncode != 0:
-        print("FAIL: Could not show LVs")
+    cmd = 'lvs -a'
+    if run(cmd).rc != 0:
+        logging.error('Could not show LVs')
         return False
     return True
 
 
-def lv_query(options="", verbose=False):  # noqa: ANN001, ANN201
+def lv_query(options=''):  # noqa: ANN001, ANN201
     """Query Logical Volumes and return a dictonary with LV information for each LV.
     The arguments are:
     options:  If not want to use default lvs output. Use -o for no default fields
     Returns:
     dict: Return a list with LV info for each LV.
     """
     # Use \",\" as separator, as some output might contain ','
     # For example, lvs -o modules on thin device returns "thin,thin-pool"
     cmd = 'lvs -a --noheadings --separator \\",\\"'
 
     # format of LV info: Name VG Attr LSize Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
     lv_info_regex = (
-        r"\s+(\S+)\",\"(\S+)\",\"(\S+)\""
-        r",\"(\S+)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)$"
+        r'\s+(\S+)\",\"(\S+)\",\"(\S+)\"'
+        r',\"(\S+)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)\",\"(.*)$'
     )
 
     # default parameters returned by lvs -a
     param_names = [
-        "name",
-        "vg_name",
-        "attr",
-        "size",
-        "pool",
-        "origin",
-        "data_per",
-        "meta_per",
-        "move",
-        "log",
-        "copy_per",
-        "convert",
+        'name',
+        'vg_name',
+        'attr',
+        'size',
+        'pool',
+        'origin',
+        'data_per',
+        'meta_per',
+        'move',
+        'log',
+        'copy_per',
+        'convert',
     ]
 
     if options:
-        param_names = ["name", "vg_name"]
+        param_names = ['name', 'vg_name']
         # need to change default regex
-        lv_info_regex = r"\s+(\S+)\",\"(\S+)"
-        parameters = options.split(",")
+        lv_info_regex = r'\s+(\S+)\",\"(\S+)'
+        parameters = options.split(',')
         for param in parameters:
             lv_info_regex += '","(.*)'
             param_names.append(param)
-        lv_info_regex += "$"
-        cmd += f" -o lv_name,vg_name,{options}"
+        lv_info_regex += '$'
+        cmd += f' -o lv_name,vg_name,{options}'
 
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("INFO: there is no LVs")
+        logging.info('there is no LVs')
         return None
-    lvs = output.split("\n")
+    lvs = output.split('\n')
 
     lv_list = []
     for lv in lvs:
         m = re.match(lv_info_regex, lv)
         if not m:
-            print(f"FAIL: ({lv}) does not match lvs output format")
+            logging.error(f'({lv}) does not match lvs output format')
             continue
         lv_info_dict = {}
         for index in range(len(param_names)):
             lv_info_dict[param_names[index]] = m.group(index + 1)
         lv_list.append(lv_info_dict)
 
     return lv_list
 
 
-def lv_create(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
+def lv_create(vg_name: str, lv_name: str, options: list):  # noqa: ANN201
     """Create a Logical Volume.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not vg_name or not lv_name:
-        print("FAIL: lv_create requires vg_name and lv_name")
+        logging.error('lv_create requires vg_name and lv_name')
         return False
 
     cmd = f"lvcreate {' '.join(str(i) for i in options)} {vg_name} -n {lv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode != 0:
         # print ("FAIL: Could not create %s" % lv_name)
         return False
     return True
 
 
-def lv_info(lv_name: str, vg_name: str, options="", verbose=False):  # noqa: ANN001, ANN201
+def lv_info(lv_name: str, vg_name: str, options=''):  # noqa: ANN001, ANN201
     """Show information of specific LV."""
     if not lv_name or not vg_name:
-        print("FAIL: lv_info() - requires lv_name and vg_name as parameters")
+        logging.error('lv_info() - requires lv_name and vg_name as parameters')
         return None
 
-    lvs = lv_query(options=options, verbose=verbose)
+    lvs = lv_query(options=options)
 
     if not lvs:
         return None
 
     for lv in lvs:
-        if lv["name"] == lv_name and lv["vg_name"] == vg_name:
+        if lv['name'] == lv_name and lv['vg_name'] == vg_name:
             return lv
     return None
 
 
-def lv_activate(lv_name: str, vg_name: str, verbose=True):  # noqa: ANN001, ANN201
+def lv_activate(lv_name: str, vg_name: str):  # noqa: ANN201
     """Activate a Logical Volume
     The arguments are:
     LV name
     VG name
     Returns:
     Boolean:
     True in case of success
     False if something went wrong.
     """
     if not lv_name or not vg_name:
-        print("FAIL: lv_activate requires lv_name and vg_name")
+        logging.error('lv_activate requires lv_name and vg_name')
         return False
 
-    cmd = f"lvchange -ay {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'lvchange -ay {vg_name}/{lv_name}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not activate LV {lv_name}")
+        logging.error(f'Could not activate LV {lv_name}')
         return False
 
     # Maybe we should query the LVs and make sure it is really activated
     return True
 
 
-def lv_deactivate(lv_name: str, vg_name: str, verbose=True):  # noqa: ANN001, ANN201
+def lv_deactivate(lv_name: str, vg_name: str):  # noqa: ANN201
     """Deactivate a Logical Volume
     The arguments are:
     LV name
     VG name
     Returns:
     Boolean:
     True in case of success
     False if something went wrong.
     """
     if not lv_name or not vg_name:
-        print("FAIL: lv_deactivate requires lv_name and vg_name")
+        logging.error('lv_deactivate requires lv_name and vg_name')
         return False
 
-    cmd = f"lvchange -an {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+    cmd = f'lvchange -an {vg_name}/{lv_name}'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not deactivate LV {lv_name}")
+        logging.error(f'Could not deactivate LV {lv_name}')
         return False
 
     # Maybe we should query the LVs and make sure it is really deactivated
     return True
 
 
-def lv_remove(lv_name: str, vg_name: str, verbose=True):  # noqa: ANN001, ANN201
+def lv_remove(lv_name: str, vg_name: str):  # noqa: ANN201
     """Remove an LV from a VG
     The arguments are:
     LV name
     VG name
     Returns:
     Boolean:
     True in case of success
     False if something went wrong.
     """
     if not lv_name or not vg_name:
-        print("FAIL: lv_remove requires lv_name and vg_name")
+        logging.error('lv_remove requires lv_name and vg_name')
         return False
 
     lv_names = lv_name.split()
 
     for lv_name in lv_names:
         if not lv_info(lv_name, vg_name):
-            print(f"INFO: lv_remove - LV {lv_name} does not exist. Skipping")
+            logging.info(f'lv_remove - LV {lv_name} does not exist. Skipping')
             continue
 
-        cmd = f"lvremove --force {vg_name}/{lv_name}"
-        retcode = run(cmd, verbose=verbose).returncode
+        cmd = f'lvremove --force {vg_name}/{lv_name}'
+        retcode = run(cmd).rc
         if retcode != 0:
-            print(f"FAIL: Could not remove LV {lv_name}")
+            logging.error(f'Could not remove LV {lv_name}')
             return False
 
         if lv_info(lv_name, vg_name):
-            print(f"INFO: lv_remove - LV {lv_name} still exists.")
+            logging.info(f'lv_remove - LV {lv_name} still exists.')
             return False
 
     return True
 
 
-def lv_convert(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
+def lv_convert(vg_name: str, lv_name: str, options: list):  # noqa: ANN201
     """Change Logical Volume layout.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not options:
-        print("FAIL: lv_convert requires at least some options specified.")
+        logging.error('lv_convert requires at least some options specified.')
         return False
 
     if not lv_name or not vg_name:
-        print("FAIL: lv_convert requires vg_name and lv_name")
+        logging.error('lv_convert requires vg_name and lv_name')
         return False
 
     cmd = f"lvconvert {' '.join(options)} {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not convert {lv_name}")
+        logging.error(f'Could not convert {lv_name}')
         return False
 
     return True
 
 
-def lv_extend(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
+def lv_extend(vg_name: str, lv_name: str, options: list):  # noqa: ANN201
     """Increase size of logical volume.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not options:
-        print("FAIL: lv_extend requires at least some options specified.")
+        logging.error('lv_extend requires at least some options specified.')
         return False
 
     if not lv_name or not vg_name:
-        print("FAIL: lv_extend requires vg_name and lv_name")
+        logging.error('lv_extend requires vg_name and lv_name')
         return False
 
     cmd = f"lvextend {' '.join(options)} {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not extend {lv_name}")
+        logging.error(f'Could not extend {lv_name}')
         return False
 
     return True
 
 
-def lv_reduce(vg_name: str, lv_name: str, options: list, verbose=True):  # noqa: ANN001, ANN201
+def lv_reduce(vg_name: str, lv_name: str, options: list):  # noqa: ANN201
     """Decrease size of logical volume.
     The arguments are:
     VG name
     LV name
     options
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     if not options:
-        print("FAIL: lv_reduce requires at least some options specified.")
+        logging.error('lv_reduce requires at least some options specified.')
         return False
 
     if not lv_name or not vg_name:
-        print("FAIL: lv_reduce requires vg_name and lv_name")
+        logging.error('lv_reduce requires vg_name and lv_name')
         return False
 
     cmd = f"lvreduce {' '.join(options)} {vg_name}/{lv_name}"
-    retcode = run(cmd, verbose=verbose).returncode
+    retcode = run(cmd).rc
     if retcode != 0:
-        print(f"FAIL: Could not reduce {lv_name}")
+        logging.error(f'Could not reduce {lv_name}')
         return False
 
     return True
 
 
 ###########################################
 # Config file
 ###########################################
 
 
 def get_config_file_path():  # noqa: ANN201
-    return "/etc/lvm/lvm.conf"
+    return '/etc/lvm/lvm.conf'
 
 
 def update_config(key: str, value: str):  # noqa: ANN201
     config_file = get_config_file_path()
-    search_regex = re.compile(r"(\s*)%s(\s*)=(\s*)\S*" % key)
-    search_regex_with_comment = re.compile(r"(\s*#\s*)%s(\s*)=(\s*)\S*" % key)
+    search_regex = re.compile(r'(\s*)%s(\s*)=(\s*)\S*' % key)
+    search_regex_with_comment = re.compile(r'(\s*#\s*)%s(\s*)=(\s*)\S*' % key)
     for line in fileinput.input(config_file, inplace=True):
         m = search_regex.match(line)
         m_with_comment = search_regex_with_comment.match(line)
         if m:
-            line = f"{m.group(1)}{key} = {value}"  # noqa: PLW2901
+            line = f'{m.group(1)}{key} = {value}'  # noqa: PLW2901
         if m_with_comment:
             line = f"{m_with_comment.group(1).replace('#', '')}{key} = {value}"  # noqa: PLW2901
         # print saves the line to the file
         # need to remove new line character as print will add it
-        line = line.rstrip("\n")  # noqa: PLW2901
+        line = line.rstrip('\n')  # noqa: PLW2901
         print(line)
 
 
 def get_lvm_config_options(all_params=False):  # noqa: ANN001, ANN201
     """Get all the configuration types from lvm.conf file."""
-    out = run("lvmconfig --type full", capture_output=True, verbose=False).output
+    out = run('lvmconfig --type full').stdout
 
     options = {}
-    category = ""
-    for line in out.split("\n"):
+    category = ''
+    for line in out.split('\n'):
         line = line.strip()  # noqa: PLW2901
-        if not line or "}" in line:
+        if not line or '}' in line:
             # skip empty or end of list line
             continue
-        if "{" in line:
+        if '{' in line:
             # category part
             category = line[:-2]  # removing "allocation {"[:-2] == "allocation"
             options[category] = []
-        elif "=" in line:
+        elif '=' in line:
             # content of a category
-            options[category].append(line.split("=")[0])
+            options[category].append(line.split('=')[0])
 
     if not all_params:
         return options
 
     options_all = []
     for value in options.values():
         options_all.extend(value)
     return options_all
 
 
 def check_lvm_config(option):  # noqa: ANN001, ANN201
-    return run(f"lvs -o {option}", capture_output=True).output
+    return run(f'lvs -o {option}').stdout
 
 
 def get_all_lvm_config_options():  # noqa: ANN201
-    all_opts = check_lvm_config("asdf")  # needs just something that it doesn't know
+    all_opts = check_lvm_config('asdf')  # needs just something that it doesn't know
     # we need to test_filter on lines that look like this
     # lvm_blahblah - explanation
     # and remove separators
 
     # at the end is '?' which should not be there therefore [:-1]
-    return [i.split()[0] for i in all_opts if re.match(r".+-.+", i) and "--" not in i][:-1]
+    return [i.split()[0] for i in all_opts if re.match(r'.+-.+', i) and '--' not in i][:-1]
 
 
 def run_cmd(func):  # noqa: ANN001, ANN201
     # TODO: Duplicate of run_command
     """Decorator for running commands
     kwargs need to be edited every time, so decorator is probably the best solution.
     """
@@ -609,35 +610,31 @@
         return run_ret_out(func(), *args, **kwargs, return_output=True)  # cmd == func()
 
     return wrapped
 
 
 @run_cmd
 def get_all_lvmvdoconfig_options():  # noqa: ANN201
-    return "lvmconfig --type list"
+    return 'lvmconfig --type list'
 
 
 @run_cmd
 def lvdisplay():  # noqa: ANN201
-    return "lvdisplay"
+    return 'lvdisplay'
 
 
 def print_profile_file(profile_name, path=None):  # noqa: ANN001, ANN201
     if not path:
-        path = "/etc/lvm/profile"  # default profile location
-    run(f"cat {path}/{profile_name}.profile")
+        path = '/etc/lvm/profile'  # default profile location
+    run(f'cat {path}/{profile_name}.profile')
 
 
 def get_lvdisplay_data():  # noqa: ANN201
     _, out = lvdisplay()
-    try:
-        lines = [line for line in out if "LV Name" in line and "pool" not in line][0].split()
-    except Exception as exc:
-        lines = [""]
-        print("Exception", exc)
+    lines = [line for line in out if 'LV Name' in line and 'pool' not in line][0].split()
     print(lines)
     return lines[-1]
 
 
 def run_command(func):  # noqa: ANN001, ANN201
     """Decorator for running commands
     kwargs need to be edited every time, so decorator is probably the best solution.
@@ -657,15 +654,15 @@
         cmd, kwargs = func(inst, **kwargs)
 
         # remove everything not necessary
         kwargs = inst.remove_nones(inst.remove_vdo_arguments(**kwargs))
 
         # Check
         if inst.check(**kwargs) is not True:  # check() with "the manual"
-            print("Check failed.")
+            print('Check failed.')
             return False
 
         # Run
         return inst.run(cmd, **kwargs)
 
     return wrapped
 
@@ -674,102 +671,102 @@
     """Class for creating LVMVDO commands."""
 
     def __init__(self, disable_check=True, vdo_arguments_flag=True) -> None:  # noqa: ANN001
         self.disable_check = disable_check
         self.tmp_kwargs: dict = {}
 
         self.commands: Dict[str, Union[str, List[str]]] = {
-            "lvcreate": "lvcreate",
-            "lvremove": "lvremove",
-            "lvconvert": "lvconvert",
-            "lvchange": "lvchange",
-            "lvextend": "lvextend",
-            "lvreduce": "lvreduce",
-            "lvresize": "lvresize",
+            'lvcreate': 'lvcreate',
+            'lvremove': 'lvremove',
+            'lvconvert': 'lvconvert',
+            'lvchange': 'lvchange',
+            'lvextend': 'lvextend',
+            'lvreduce': 'lvreduce',
+            'lvresize': 'lvresize',
         }
 
-        self.commands["all"] = list(self.commands.keys())
+        self.commands['all'] = list(self.commands.keys())
 
         self.arguments = {  # "": [[""], "--"],
-            "help": [self.commands["all"], " --help"],
-            "version": [self.commands["all"], " --version"],
-            "verbose": [self.commands["all"], " --verbose"],
-            "type": [["lvcreate", "lvconvert"], "--type&"],
-            "vdo": [["lvcreate"], "--vdo"],
-            "vdopool": [["lvcreate"], "--vdopool&"],
-            "vdo_name": [["lvcreate", "lvconvert"], "--name&"],
-            "size": [["lvcreate", "lvextend"], "--size&"],
-            "logical_size": [["lvcreate", "lvconvert"], "--virtualsize&"],
-            "config": [["lvcreate", "lvextend"], "--config&"],
-            "extents": [["lvcreate"], "--extents&"],
-            "stripes": [["lvcreate", "lvextend"], "--stripes&"],
-            "stripesize": [["lvcreate", "lvextend"], "--stripesize&"],
-            "compression": [["lvcreate", "lvconvert", "lvchange"], "--compression&"],
-            "deduplication": [
-                ["lvcreate", "lvconvert", "lvchange"],
-                "--deduplication&",
+            'help': [self.commands['all'], ' --help'],
+            'version': [self.commands['all'], ' --version'],
+            'verbose': [self.commands['all'], ' --verbose'],
+            'type': [['lvcreate', 'lvconvert'], '--type&'],
+            'vdo': [['lvcreate'], '--vdo'],
+            'vdopool': [['lvcreate'], '--vdopool&'],
+            'vdo_name': [['lvcreate', 'lvconvert'], '--name&'],
+            'size': [['lvcreate', 'lvextend'], '--size&'],
+            'logical_size': [['lvcreate', 'lvconvert'], '--virtualsize&'],
+            'config': [['lvcreate', 'lvextend'], '--config&'],
+            'extents': [['lvcreate'], '--extents&'],
+            'stripes': [['lvcreate', 'lvextend'], '--stripes&'],
+            'stripesize': [['lvcreate', 'lvextend'], '--stripesize&'],
+            'compression': [['lvcreate', 'lvconvert', 'lvchange'], '--compression&'],
+            'deduplication': [
+                ['lvcreate', 'lvconvert', 'lvchange'],
+                '--deduplication&',
             ],
-            "activate": [["lvchange"], "--activate&"],
-            "metadataprofile": [
-                ["lvcreate", "lvconvert", "lvchange"],
-                "--metadataprofile&",
+            'activate': [['lvchange'], '--activate&'],
+            'metadataprofile': [
+                ['lvcreate', 'lvconvert', 'lvchange'],
+                '--metadataprofile&',
             ],
-            "force": [["lvremove"], "--force"],
-            "yes": [["lvremove"], "-y"],
-            "refresh": [["lvchange"], ""],
-            "vg_name": [["lvcreate", "lvextend"], ""],
-            "lv_name": [["lvchange"], ""],
+            'force': [['lvremove'], '--force'],
+            'yes': [['lvremove'], '-y'],
+            'refresh': [['lvchange'], ''],
+            'vg_name': [['lvcreate', 'lvextend'], ''],
+            'lv_name': [['lvchange'], ''],
         }
 
         self.no_check_size_unit = [
-            "logical_size",
-            "cachesize",
-            "chunksize",
-            "poolmetadatasize",
-            "regionsize",
-            "size",
-            "stripesize",
-            "virtualsize",
+            'logical_size',
+            'cachesize',
+            'chunksize',
+            'poolmetadatasize',
+            'regionsize',
+            'size',
+            'stripesize',
+            'virtualsize',
         ]
 
         self.argument_options = {
             # argument: [(.fmf option name values), (command option values)]
             # order in tuples matters
             # enable == 'y', disable == 'n'
-            "activate": [("enabled", "disabled", "auto"), ("y", "n", "ay")],
-            "deduplication": [("enabled", "disabled"), ("y", "n")],
-            "compression": [("enabled", "disabled"), ("y", "n")],
+            'activate': [('enabled', 'disabled', 'auto'), ('y', 'n', 'ay')],
+            'deduplication': [('enabled', 'disabled'), ('y', 'n')],
+            'compression': [('enabled', 'disabled'), ('y', 'n')],
             # '': [(,),(,)],
         }
 
         self.multiple_option_arguments = self.argument_options.keys()
 
         self.lvm_arguments = self.arguments.copy()
 
         self.option_translator_dictionary = {
-            "1": "vdo_use_compression",
-            "2": "vdo_use_deduplication",
-            "3": "vdo_use_metadata_hints",
-            "4": "vdo_minimum_io_size",
-            "block_map_cache_size": "vdo_block_map_cache_size_mb",
-            "block_map_period": "vdo_block_map_period",
-            "5": "vdo_check_point_frequency",
-            "sparse_index": "vdo_use_sparse_index",
-            "index_mem": "vdo_index_memory_size_mb",
-            "slab_size": "vdo_slab_size_mb",
-            "ack_threads": "vdo_ack_threads",
-            "bio_threads": "vdo_bio_threads",
-            "bio_rotation_interval": "vdo_bio_rotation",
-            "cpu_threads": "vdo_cpu_threads",
-            "hash_zone_threads": "vdo_hash_zone_threads",
-            "logical_threads": "vdo_logical_threads",
-            "physical_threads": "vdo_physical_threads",
-            "write_policy": "vdo_write_policy",
-            "max_discard_size": "vdo_max_discard",
-            "6": "vdo_pool_header_size",
+            '1': 'vdo_use_compression',
+            '2': 'vdo_use_deduplication',
+            '3': 'vdo_use_metadata_hints',
+            '4': 'vdo_minimum_io_size',
+            'block_map_cache_size': 'vdo_block_map_cache_size_mb',
+            'block_map_period': 'vdo_block_map_period',
+            '5': 'vdo_check_point_frequency',
+            'sparse_index': 'vdo_use_sparse_index',
+            'index_mem': 'vdo_index_memory_size_mb',
+            'slab_size': 'vdo_slab_size_mb',
+            'ack_threads': 'vdo_ack_threads',
+            'bio_threads': 'vdo_bio_threads',
+            'bio_rotation_interval': 'vdo_bio_rotation',
+            'cpu_threads': 'vdo_cpu_threads',
+            'hash_zone_threads': 'vdo_hash_zone_threads',
+            'logical_threads': 'vdo_logical_threads',
+            'physical_threads': 'vdo_physical_threads',
+            'write_policy': 'vdo_write_policy',
+            'max_discard_size': 'vdo_max_discard',
+            '6': 'vdo_pool_header_size',
         }
         self.config_arguments = self.option_translator_dictionary.keys()
 
         self.vdo_arguments = {}
         if vdo_arguments_flag:
             # obtain arguments from VDO for backwards compatibility
             self.vdo_arguments = vdo.VDO().arguments.copy()
@@ -791,28 +788,28 @@
     @staticmethod
     def remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
     @staticmethod
     def _add_value(value, command, argument):  # noqa: ANN001, ANN205
         """Copied from Wrapper."""
-        if argument[-1:] in ["=", "&"]:
-            if argument[-1:] == "&":
-                argument = argument[:-1] + " "
+        if argument[-1:] in ['=', '&']:
+            if argument[-1:] == '&':
+                argument = argument[:-1] + ' '
             if isinstance(value, list):
                 # allows to use repeatable arguments as a list of values
                 for val in value:
                     command += argument + "'" + str(val) + "'"
             else:
                 command += argument + "'" + str(value) + "'"
-        elif argument[-1:] in "*":
+        elif argument[-1:] in '*':
             command += str(value)
         else:
             command += argument
-        return command + " "  # added space at the end to fix formatting
+        return command + ' '  # added space at the end to fix formatting
 
     def _add_argument(self, arg, value, command):  # noqa: ANN001, ANN202
         """Copied from Wrapper."""
         # Checks if given argument is allowed for given command and adds it to cmd string
         self._check_allowed_argument(arg, command)
         return self._add_value(value, command, self._get_arg(arg))
 
@@ -822,37 +819,37 @@
         for kwarg in kwargs:
             # skip adding this argument if the value is False
             if kwargs[kwarg] is False:
                 continue
             # skip:
             # vg_name, it should be last
             # vdo_name should be just "name" but not used is OK :D
-            if kwarg in "vg_name":  # ,"vdo_name"):  # maybe more names will be here
+            if kwarg in 'vg_name':  # ,"vdo_name"):  # maybe more names will be here
                 continue
             command = self._add_argument(kwarg, kwargs[kwarg], command)
 
         # vg_name must be the last in command
-        if "vg_name" in kwargs:
-            command += kwargs["vg_name"]
+        if 'vg_name' in kwargs:
+            command += kwargs['vg_name']
         return command
 
     def _get_possible_arguments(self, command=None):  # noqa: ANN001, ANN202
         return super()._get_possible_arguments(command.split()[0])
 
-    def run(self, cmd, verbosity=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
+    def run(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN201
         """Constructs the command to run and runs it."""
         cmd = self._add_arguments(cmd, **kwargs)
 
         print(cmd)
-        ret = run(cmd, verbose=verbosity).returncode
+        ret = run(cmd).rc
 
         if isinstance(ret, tuple) and ret[0] != 0:
-            print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+            logging.warning(f"Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+            logging.warning(f"Running command: '{cmd}' failed.")
         return ret
 
     def number_of_conf_args(self, **kwargs):  # noqa: ANN003, ANN201
         """Counts the number of configuration arguments in kwargs and returns it."""
         return sum(conf_arg in kwargs for conf_arg in self.config_arguments)
 
     def _set_kwargs_value(self, arg, **kwargs):  # noqa: ANN001, ANN003, ANN202
@@ -885,95 +882,95 @@
         ret, device_size = run_ret_out(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
         print(device_name, ret, device_size)
         if ret != 0:
             raise VDODeviceNotFoundError
 
         # ['└─myvg-vdotest', '252:2', '0', '4G', '0', 'lvm'][3] == '4G'
         size = device_size.split()[3]
-        multipliers = ["M", "G", "T", "P", "E"]
+        multipliers = ['M', 'G', 'T', 'P', 'E']
 
         device_size = (float(size[:-1]) * (1024 ** multipliers.index(size[-1:]))).__int__()
         max_number_of_slabs = 8192
         minimum_size = max(2 ** int(device_size / max_number_of_slabs).bit_length(), 128)  # reused from vdo.py
         if default_to_2g and minimum_size < 2048:
-            return "2G"
-        return f"{minimum_size!s}M"
+            return '2G'
+        return f'{minimum_size!s}M'
 
     def check_conf_value(self, val):  # noqa: ANN001, ANN201
         """Remove units K, G, T and convert accordingly."""
-        if "fail" in self.tmp_kwargs["name"]:
+        if 'fail' in self.tmp_kwargs['name']:
             return val  # don't check
 
         units = {
-            "K": 0.001,  # 1/1024 = 0.00097656,
-            "k": 0.001,
-            "M": 1,
-            "m": 1,
-            "G": 1024,  # 1000
-            "g": 1024,
-            "T": 1048576,  # 1000000
-            "t": 1048576,
+            'K': 0.001,  # 1/1024 = 0.00097656,
+            'k': 0.001,
+            'M': 1,
+            'm': 1,
+            'G': 1024,  # 1000
+            'g': 1024,
+            'T': 1048576,  # 1000000
+            't': 1048576,
             # "B": 1  # should do nothing
         }
 
-        if re.match(r"[0-9]+\.[0-9]+", str(val)):  # float
+        if re.match(r'[0-9]+\.[0-9]+', str(val)):  # float
             return val
 
-        match = re.match(r"([0-9]+)(.+|)", str(val))
+        match = re.match(r'([0-9]+)(.+|)', str(val))
         if not match:
             return val
 
         multiplier = 1
         if len(match.groups()) == 2 and match.group(2):  # should not be empty
             try:
                 multiplier = units[match.group(2)]
             except KeyError:  # because of "512B"
-                print("Argument value: ", match.group(2), ".")
-                print(f"Original {val}; will return {val[:-1]}")
+                print('Argument value: ', match.group(2), '.')
+                print(f'Original {val}; will return {val[:-1]}')
                 return val[:-1]
         return str(int(match.group(1)) * multiplier)
 
     def check_config_arguments(self, **kwargs):  # noqa: ANN003, ANN201
         """Check arguments in config."""
-        if "slab_size" in kwargs:
-            device_name = kwargs["device"].split("/")[-1]
+        if 'slab_size' in kwargs:
+            device_name = kwargs['device'].split('/')[-1]
             # Slab_size value should be in MB
-            kwargs["slab_size"] = self.check_conf_value(self.minimum_slab_size(device_name))
+            kwargs['slab_size'] = self.check_conf_value(self.minimum_slab_size(device_name))
 
         return kwargs
 
     def create_profile_file(self, profile_name, args_to_remove, **kwargs):  # noqa: ANN001, ANN003, ANN201
         """Example: category {
             arg1 = value,
             arg2 = value
         }.
         """
-        run(f"rm /etc/lvm/profile/{profile_name}.profile")
+        run(f'rm /etc/lvm/profile/{profile_name}.profile')
 
         # creates metadataprofile ONLY ONE CATEGORY NOW!!!!
         # update 28022022 don't know if it is true, after code review this should do multiple categories...
         to_write = {}  # category: [list of values]
-        with Path(f"/etc/lvm/profile/{profile_name}.profile").open("w", encoding="utf-8") as fp:
+        with Path(f'/etc/lvm/profile/{profile_name}.profile').open('w', encoding='utf-8') as fp:
             # create the structure of the document and save it in a string
             for arg, value in kwargs.items():
                 if arg in self.config_arguments:  # do just what is necessary
                     category = self.get_category(arg)
                     if category not in to_write:
                         to_write[category] = []
 
-                    to_write[category].append(f"{self.get_option(arg)}={self.check_conf_value(value)}")
+                    to_write[category].append(f'{self.get_option(arg)}={self.check_conf_value(value)}')
                     args_to_remove.append(arg)
 
-            str_to_write = ""
+            str_to_write = ''
             for category in to_write:
                 for value in to_write.values():
-                    str_to_write += f"{category} {{\n"
+                    str_to_write += f'{category} {{\n'
                     for opt in value:
-                        str_to_write += f"\t{opt}\n"
-                str_to_write += "}\n"
+                        str_to_write += f'\t{opt}\n'
+                str_to_write += '}\n'
             fp.write(str_to_write)  # in 'with' section there is no need for fp.close()
 
         return args_to_remove
 
     def replace_multiple_option_values(self, **kwargs):  # noqa: ANN003, ANN201
         """Check and replace what is defined in .fmf test file with corresponding value from man page
         e.g. 'enabled' -> 'y'.
@@ -1005,92 +1002,92 @@
 
         # using the list containing the argument as item of the list
         index = list(self.config_options.values()).index(arguments_of_category)
         return list(self.config_options.keys())[index]
 
     def check(self, **kwargs):  # noqa: ANN003, ANN201
         """Check arguments compatibility with command."""
-        if "name" in kwargs:
-            kwargs.pop("name")  # remove name, because it is not used in lvmvdo
+        if 'name' in kwargs:
+            kwargs.pop('name')  # remove name, because it is not used in lvmvdo
 
-        if "size" in kwargs:
+        if 'size' in kwargs:
             # value format for size parameter
-            return bool(re.match(r"^([\+|\-]|)[0-9]+[T|G|M|K]$", kwargs["size"]))
+            return bool(re.match(r'^([\+|\-]|)[0-9]+[T|G|M|K]$', kwargs['size']))
         return True
 
     @staticmethod
     def remove_args(to_remove, **kwargs):  # noqa: ANN001, ANN003, ANN205
         """Return only what is intended."""
         return {k: v for k, v in kwargs.items() if k not in to_remove}
 
     @run_command
     def lvcreate(self, **kwargs):  # noqa: ANN003, ANN201
-        print("LVCREATE", kwargs)
-        cmd = "lvcreate --vdo "
+        print('LVCREATE', kwargs)
+        cmd = 'lvcreate --vdo '
 
         # config part START
         args_to_remove = []
         use_conf_file = False
 
         if use_conf_file:
-            profile_name = "vdo_create"
+            profile_name = 'vdo_create'
             args_to_remove = self.create_profile_file(profile_name, args_to_remove, **kwargs)
-            cmd += f"--metadataprofile {profile_name} "
+            cmd += f'--metadataprofile {profile_name} '
             print_profile_file(profile_name)
-        elif self.number_of_conf_args(**kwargs).returncode != 0:
-            cmd += "--config"
+        elif self.number_of_conf_args(**kwargs).rc != 0:
+            cmd += '--config'
             # --config="    for condition == 1
             # --config '   else
             cmd += '="' if self.number_of_conf_args(**kwargs) == 1 else " '"
 
             for arg, value in kwargs.items():
                 if arg in self.config_arguments:  # do just what is necessary
                     if self.number_of_conf_args(**kwargs) == 1:
                         # --config="cat/opt=val
-                        cmd += f"{self.get_category(arg)}/{self.get_option(arg)}={self.check_conf_value(value)}"
+                        cmd += f'{self.get_category(arg)}/{self.get_option(arg)}={self.check_conf_value(value)}'
                     else:
                         # --config 'cat/opt=val cat/opt=val cat/opt=val
-                        cmd += f"{self.get_category(arg)}/{self.get_option(arg)}={self.check_conf_value(value)} "
+                        cmd += f'{self.get_category(arg)}/{self.get_option(arg)}={self.check_conf_value(value)} '
                     args_to_remove.append(arg)
 
             # --config="cat/opt=val"                          == 1
             # --config 'cat/opt=val cat/opt=val cat/opt=val'  else
             cmd += '" ' if self.number_of_conf_args(**kwargs) == 1 else "' "
 
         # some arguments are used as config and are no longer needed
         kwargs = self.remove_args(args_to_remove, **kwargs)
         # config part END
 
-        kwargs["yes"] = "-y"  # see lvremove
+        kwargs['yes'] = '-y'  # see lvremove
 
         return cmd, kwargs
 
     @run_command
     def lvremove(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "lvremove "
+        cmd = 'lvremove '
 
         # lvmvdo uses human interface for some activities like removing vdo pools
         # in automation we don't want this, so we add '-y' to force it
-        kwargs["yes"] = "-y"
+        kwargs['yes'] = '-y'
         return cmd, kwargs
 
     @run_command
     def lvconvert(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "lvconvert --vdo "
+        cmd = 'lvconvert --vdo '
         return cmd, kwargs
 
     @run_command
     def lvchange(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "lvchange "
-        if "vdo_name" in kwargs:
-            kwargs.pop("vdo_name")
+        cmd = 'lvchange '
+        if 'vdo_name' in kwargs:
+            kwargs.pop('vdo_name')
         return cmd, kwargs
 
     @run_command
     def lvextend(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "lvextend "
+        cmd = 'lvextend '
         return cmd, kwargs
 
     @run_command
     def lvmconfig(self, **kwargs):  # noqa: ANN003, ANN201
-        cmd = "lvmconfig "
+        cmd = 'lvmconfig '
         return cmd, kwargs
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/md.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/md.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,189 @@
 """md.py: Module to manipulate MD devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import re
 from pathlib import Path
 
 from sts.utils.cmdline import exists, run_ret_out
 
 
-def _mdadm_query(md_device, verbose=False):  # noqa: ANN001, ANN202
-    if not exists("mdadm"):
-        if verbose:
-            print("INFO: mdadm is not installed")
+def _mdadm_query(md_device):  # noqa: ANN001, ANN202
+    if not exists('mdadm'):
+        logging.info('mdadm is not installed')
         return None
 
-    cmd = f"mdadm -D /dev/{md_device}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    cmd = f'mdadm -D /dev/{md_device}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: couldn't query {md_device}")
-        if verbose:
-            print(output)
+        logging.error(f"couldn't query {md_device}")
         return None
     return output
 
 
-def md_query(verbose=False):  # noqa: ANN001, ANN201
+def md_query():  # noqa: ANN201
     """Query Soft RAID devices.
     The arguments are:
-    verbose: Print additional information. Default: False
     Returns:
     dict: Return a list of md devices.
     """
-    mdstat_file = "/proc/mdstat"
+    mdstat_file = '/proc/mdstat'
 
     if not Path(mdstat_file).exists():
-        if verbose:
-            print("INFO: there is no MD device")
+        logging.info('there is no MD device')
         return False
 
-    cmd = f"cat {mdstat_file}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    cmd = f'cat {mdstat_file}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        if verbose:
-            print("INFO: there is no MD device")
+        logging.info('there is no MD device')
         return None
 
-    md_name_regex = r"^(md\d+) :"
+    md_name_regex = r'^(md\d+) :'
     md_devices = []
-    for line in output.split("\n"):
+    for line in output.split('\n'):
         m = re.match(md_name_regex, line)
         if not m:
             continue
         md_devices.append(m.group(1))
 
     return md_devices
 
 
-def md_get_info(md_device, verbose=False):  # noqa: ANN001, ANN201
+def md_get_info(md_device):  # noqa: ANN001, ANN201
     """Query information of an MD device.
     The arguments are:
     md_device: md device name to get information about
-    verbose: Print additional information. Default: False
     Returns:
     dict: Return a dictionary with details about the md device.
     """
     if not md_device:
         return None
 
     if md_device not in md_query():
-        if verbose:
-            print(f"INFO: {md_device} is not a MD device")
+        logging.info(f'{md_device} is not a MD device')
         return None
 
-    output = _mdadm_query(md_device, verbose)
+    output = _mdadm_query(md_device)
     if not output:
         return None
 
     md_info = {}
     # Try to get general information about the device
-    md_info_regex = r"\s+(.*) : (.*)"
-    for line in output.split("\n"):
+    md_info_regex = r'\s+(.*) : (.*)'
+    for line in output.split('\n'):
         info_match = re.match(md_info_regex, line)
         if not info_match:
             continue
         info_name = info_match.group(1).lower()
-        info_name = info_name.replace(" ", "_")
+        info_name = info_name.replace(' ', '_')
         md_info[info_name] = info_match.group(2)
 
     # Try to get the storage devices linked to the MD
     storage_section = False
-    storage_regex = r"\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(.*)\s+(\S+)$"
-    for line in output.split("\n"):
-        if re.search(r"Number\s+Major\s+Minor\s+RaidDevice\s+State", line):
+    storage_regex = r'\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(.*)\s+(\S+)$'
+    for line in output.split('\n'):
+        if re.search(r'Number\s+Major\s+Minor\s+RaidDevice\s+State', line):
             storage_section = True
-            md_info["storage_devices"] = {}
+            md_info['storage_devices'] = {}
         if not storage_section:
             continue
         storage_match = re.match(storage_regex, line)
         if not storage_match:
             continue
         storage_info = {
-            "number": storage_match.group(1),
-            "major": storage_match.group(2),
-            "minor": storage_match.group(3),
-            "raid_device": storage_match.group(4),
-            "state": storage_match.group(5).strip(),
+            'number': storage_match.group(1),
+            'major': storage_match.group(2),
+            'minor': storage_match.group(3),
+            'raid_device': storage_match.group(4),
+            'state': storage_match.group(5).strip(),
         }
-        md_info["storage_devices"][storage_match.group(6)] = storage_info
+        md_info['storage_devices'][storage_match.group(6)] = storage_info
 
     return md_info
 
 
-def md_get_storage_dev(md_device, verbose=False):  # noqa: ANN001, ANN201
+def md_get_storage_dev(md_device):  # noqa: ANN001, ANN201
     """Get the storage devices of an MD device.
     The arguments are:
     md_device: md device name to get information about
-    verbose: Print additional information. Default: False
     Returns:
     list: Return a list of storage devices.
     """
     if not md_device:
         return None
 
-    md_info = md_get_info(md_device, verbose)
+    md_info = md_get_info(md_device)
     if not md_info:
         return None
 
-    if "storage_devices" not in md_info:
+    if 'storage_devices' not in md_info:
         return None
-    return md_info["storage_devices"].keys()
+    return md_info['storage_devices'].keys()
 
 
-def md_stop(md_device, verbose=False):  # noqa: ANN001, ANN201
+def md_stop(md_device):  # noqa: ANN001, ANN201
     """Stop a specific md device.
     The arguments are:
     md_device: md device name to get information about
-    verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    cmd = f"mdadm --stop /dev/{md_device}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    cmd = f'mdadm --stop /dev/{md_device}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: couldn't stop {md_device}")
-        if verbose:
-            print(output)
+        logging.error(f"couldn't stop {md_device}")
         return False
     return True
 
 
-def md_clean(device, verbose=False):  # noqa: ANN001, ANN201
+def md_clean(device):  # noqa: ANN001, ANN201
     """Clean a specific storage device.
     The arguments are:
     device: storage device like /dev/sda
-    verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
-    cmd = f"mdadm --zero-superblock {device}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    cmd = f'mdadm --zero-superblock {device}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: couldn't clean {device}")
-        if verbose:
-            print(output)
+        logging.error(f"couldn't clean {device}")
         return False
     return True
 
 
-def md_remove(md_device, clean=False, verbose=False):  # noqa: ANN001, ANN201
+def md_remove(md_device, clean=False):  # noqa: ANN001, ANN201
     """Remove a specific md device.
     The arguments are:
     md_device: md device name to get information about
-    verbose: Print additional information. Default: False
     Returns:
     Boolean:
     True if success
     False in case of failure.
     """
     sto_devices = md_get_storage_dev(md_device)
 
     if not md_stop(md_device):
         return False
 
-    cmd = f"mdadm --remove /dev/{md_device}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=verbose)
+    cmd = f'mdadm --remove /dev/{md_device}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if (
         retcode != 0
         and
         # error opening the device can be ignored
-        f"mdadm: error opening /dev/{md_device}: No such file or directory" not in output
+        f'mdadm: error opening /dev/{md_device}: No such file or directory' not in output
     ):
-        print(f"FAIL: couldn't remove {md_device}")
-        if verbose:
-            print(output)
+        logging.error(f"couldn't remove {md_device}")
         return False
     if clean and sto_devices:
         for device in sto_devices:
-            if not md_clean(device, verbose):
+            if not md_clean(device):
                 return False
     return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/mp.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/mp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """mp.py: Module to manage multipath devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import re
 from pathlib import Path
 from typing import Literal
 
 from sts import fc, iscsi, linux, lvm, net, scsi
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.size import size_human_2_size_bytes
 
-MULTIPATH_CONF_PATH = "/etc/multipath.conf"
-aug_conf_path = "/files/etc/multipath.conf"
-package_name = "device-mapper-multipath"
+MULTIPATH_CONF_PATH = '/etc/multipath.conf'
+aug_conf_path = '/files/etc/multipath.conf'
+package_name = 'device-mapper-multipath'
 
 
 def mp_service_name():  # noqa: ANN201
     """Return the name of multipath service."""
-    return "multipathd"
+    return 'multipathd'
 
 
 def mp_start_service():  # noqa: ANN201
     """Start multipath service."""
     if linux.is_installed(package_name) and not Path(MULTIPATH_CONF_PATH).is_file():
         mpathconf_enable()
     return linux.service_start(mp_service_name())
@@ -34,29 +35,29 @@
 
 
 def is_multipathd_running():  # noqa: ANN201
     """Check if multipathd is running."""
     return linux.is_service_running(mp_service_name())
 
 
-def mpathconf_enable(find_mpaths: Literal["yes", "no", "strict", "greedy", "smart", None] = None) -> bool:
+def mpathconf_enable(find_mpaths: Literal['yes', 'no', 'strict', 'greedy', 'smart', None] = None) -> bool:
     """Runs 'mpathconf --enable' command."""
-    cmd = "mpathconf --enable"
+    cmd = 'mpathconf --enable'
     if find_mpaths:
-        cmd = cmd + f" --find_multipaths {find_mpaths}"
-    if run(cmd).returncode != 0:
+        cmd = cmd + f' --find_multipaths {find_mpaths}'
+    if run(cmd).rc != 0:
         return False
 
     return True
 
 
 def mp_enable() -> bool:
     """Installs and enable multipath."""
     if not is_multipathd_running():
-        linux.install_package("device-mapper-multipath")
+        linux.install_package('device-mapper-multipath')
         mpathconf_enable()
         if not linux.service_start(mp_service_name()):
             return False
 
     return True
 
 
@@ -66,87 +67,87 @@
     Args:
       mpath_name: name of device to check
       print_fail: Should we print "FAIL: ..." in case of fail?
 
     Returns:
       True / False.
     """
-    cmd = f"multipath -l {mpath_name}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'multipath -l {mpath_name}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         if print_fail:
             print(f'FAIL: Could not execute "{cmd}"')
         return None
 
     # There could be error in the output, so we need to check if we really found the mpath device.
     # 'multipath -l device_name' always should return device_name at the beginning if found
-    if output and len(output) > 0 and output.startswith(f"{mpath_name} "):
+    if output and len(output) > 0 and output.startswith(f'{mpath_name} '):
         return True
     return False
 
 
 def get_mpath_of_disk(disk):  # noqa: ANN001, ANN201
     """Get the multipath device of a disk
     The arguments are:
     Disk:   Disk
     Returns:
     String: Return the name of multipath device.
     """
-    if linux.dist_name() == "RHEL" and linux.dist_ver() < 7:
-        device = f"/dev/{disk}"
+    if linux.dist_name() == 'RHEL' and linux.dist_ver() < 7:
+        device = f'/dev/{disk}'
         mmnum_cmd = 'ls -l %s | awk \'{print "("$5,$6")"}\'' % device
-        retcode, output = run_ret_out(mmnum_cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(mmnum_cmd, return_output=True)
         if retcode != 0:
-            print(f"FAIL: Could not get device information for {device}")
+            logging.error(f'Could not get device information for {device}')
             print(output)
             return None
         deps_cmd = rf"dmsetup deps | grep \"{output}\" | awk -v device={device} '{{print $1}}' | tr -d \"\:\""
-        retcode, output = run_ret_out(deps_cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(deps_cmd, return_output=True)
         if retcode != 0:
-            print(f"FAIL: Could not get dmsetup information for {device}")
+            logging.error(f'Could not get dmsetup information for {device}')
             print(output)
             return None
         mpath = output
     else:
         # BZ891921 - Multipath provides the mpath device of given scsi block device
-        cmd = "pidof multipathd"
-        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+        cmd = 'pidof multipathd'
+        retcode, output = run_ret_out(cmd, return_output=True)
         if retcode != 0:
-            print("FAIL: For some reason multipathd is not running")
+            logging.error('For some reason multipathd is not running')
             print(output)
             return None
         fmt = '"%d %m"'
         cmd = f"multipathd show paths format {fmt} | egrep \"^{disk}\" | awk '{{print$2}}'"
-        retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+        retcode, output = run_ret_out(cmd, return_output=True)
         if retcode != 0:
-            print(f"FAIL: to find multipath of disk {disk}")
+            logging.error(f'to find multipath of disk {disk}')
             print(output)
             return None
         mpath = output
 
     if not mpath:
-        print(f"WARN: Could not find multipath for {disk}")
+        logging.warning(f'Could not find multipath for {disk}')
         return None
     return mpath
 
 
 def get_disks_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return all SCSI devices that belong to this mpath."""
     if not mpath_name:
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
         return None
 
-    if "disk" not in list(mpath_dict.keys()):
-        print(f"WARN: mpath {mpath_name} has no disk")
+    if 'disk' not in list(mpath_dict.keys()):
+        logging.warning(f'mpath {mpath_name} has no disk')
         return None
 
-    return list(mpath_dict["disk"].keys())
+    return list(mpath_dict['disk'].keys())
 
 
 def get_disks_of_mpath_by_wwpn(mpath_name, wwpn):  # noqa: ANN001, ANN201
     """From a specific mpath device, return the devices
     connected to this WWPN.
     """
     if not mpath_name or not wwpn:
@@ -154,20 +155,20 @@
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
         return None
 
     scsi_devices = []
     wwpn = fc.standardize_wwpn(wwpn)
-    if wwpn and "disk" in list(mpath_dict.keys()):
-        port_entries = ["h_wwpn", "t_wwpn"]
-        for disk in list(mpath_dict["disk"].keys()):
+    if wwpn and 'disk' in list(mpath_dict.keys()):
+        port_entries = ['h_wwpn', 't_wwpn']
+        for disk in list(mpath_dict['disk'].keys()):
             for port_entry in port_entries:
-                if port_entry in list(mpath_dict["disk"][disk].keys()):  # noqa: SIM102
-                    if mpath_dict["disk"][disk][port_entry] and wwpn in mpath_dict["disk"][disk][port_entry]:
+                if port_entry in list(mpath_dict['disk'][disk].keys()):  # noqa: SIM102
+                    if mpath_dict['disk'][disk][port_entry] and wwpn in mpath_dict['disk'][disk][port_entry]:
                         scsi_devices.append(disk)
     return scsi_devices
 
 
 def get_disks_of_mpath_by_iqn(mpath_name, iqn):  # noqa: ANN001, ANN201
     """From a specific mpath device, return the devices
     connected to this IQN.
@@ -179,20 +180,20 @@
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
         return None
 
     scsi_devices = []
-    if "disk" in list(mpath_dict.keys()):
-        port_entries = ["h_iqn", "t_iqn"]
-        for disk in list(mpath_dict["disk"].keys()):
+    if 'disk' in list(mpath_dict.keys()):
+        port_entries = ['h_iqn', 't_iqn']
+        for disk in list(mpath_dict['disk'].keys()):
             for port_entry in port_entries:
-                if port_entry in list(mpath_dict["disk"][disk].keys()):  # noqa: SIM102
-                    if mpath_dict["disk"][disk][port_entry] and iqn in mpath_dict["disk"][disk][port_entry]:
+                if port_entry in list(mpath_dict['disk'][disk].keys()):  # noqa: SIM102
+                    if mpath_dict['disk'][disk][port_entry] and iqn in mpath_dict['disk'][disk][port_entry]:
                         scsi_devices.append(disk)
     return scsi_devices
 
 
 def get_disks_of_mpath_by_mac(mpath_name, mac):  # noqa: ANN001, ANN201
     """From a specific mpath device, return the devices
     connected to this MAC.
@@ -204,20 +205,20 @@
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
         return None
 
     scsi_devices = []
-    if "disk" in list(mpath_dict.keys()):
-        port_entries = ["iface_mac"]
-        for disk in list(mpath_dict["disk"].keys()):
+    if 'disk' in list(mpath_dict.keys()):
+        port_entries = ['iface_mac']
+        for disk in list(mpath_dict['disk'].keys()):
             for port_entry in port_entries:
-                if port_entry in list(mpath_dict["disk"][disk].keys()):  # noqa: SIM102
-                    if mpath_dict["disk"][disk][port_entry] and mac in mpath_dict["disk"][disk][port_entry]:
+                if port_entry in list(mpath_dict['disk'][disk].keys()):  # noqa: SIM102
+                    if mpath_dict['disk'][disk][port_entry] and mac in mpath_dict['disk'][disk][port_entry]:
                         scsi_devices.append(disk)
     return scsi_devices
 
 
 def multipath_query_all(mpath_name=None):  # noqa: ANN001, ANN201
     # Not sure with of these 2 commands I should use
     # multipath -ll
@@ -226,64 +227,64 @@
     # multipathd show top
     # multipath will not run a checker on the paths. It will simply report the
     # current state. This means that you get the results from the last time
     # that multipathd ran the path checker.  If there is no IO going to the
     # device, the kernel won't return an error on the path, and so you will
     # not see any errors until the next checker is run after you bring the
     # port down.
-    cmd = "multipath -ll"
+    cmd = 'multipath -ll'
     if mpath_name:
-        cmd += f" {mpath_name}"
+        cmd += f' {mpath_name}'
     # cmd = "multipathd -k\"show top\""
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         print(f'FAIL: Could not execute "{cmd}"')
         return None
 
     if not output:
-        # print("FAIL: Got no output from \"%s\"" % cmd)
+        # logging.error("Got no output from \"%s\"" % cmd)
         return None
 
-    regex_mpath = r"^(?:create\:\ ){0,1}"  # might have when creating mpath
-    regex_mpath += r"(?:reload\:\ ){0,1}"  # might have when creating mpath
-    regex_mpath += r"([^ ]+?)\ +"  # 1. mpath_name
-    regex_mpath += r"(?:\((\S+)\)\ +){0,1}"  # 2. wwid if different from #1
-    regex_mpath += r"(?:(dm\-[0-9]+)\ +){0,1}"  # 3. dm_name if known
-    regex_mpath += r"(?:([^,]+),){0,1}"  # 4. vendor, might not have
-    regex_mpath += r"(?:([^,]+)){0,1}$"  # 5. product,  might not have
+    regex_mpath = r'^(?:create\:\ ){0,1}'  # might have when creating mpath
+    regex_mpath += r'(?:reload\:\ ){0,1}'  # might have when creating mpath
+    regex_mpath += r'([^ ]+?)\ +'  # 1. mpath_name
+    regex_mpath += r'(?:\((\S+)\)\ +){0,1}'  # 2. wwid if different from #1
+    regex_mpath += r'(?:(dm\-[0-9]+)\ +){0,1}'  # 3. dm_name if known
+    regex_mpath += r'(?:([^,]+),){0,1}'  # 4. vendor, might not have
+    regex_mpath += r'(?:([^,]+)){0,1}$'  # 5. product,  might not have
 
-    regex_feature = r"size=([0-9\.]+[A-Z])\ +"  # 1. size
+    regex_feature = r'size=([0-9\.]+[A-Z])\ +'  # 1. size
     regex_feature += r"features=\'([^\']+)\'\ +"  # 2. features
     regex_feature += r"hwhandler=\'([^\']+)\'\ +"  # 3. hardware handler
-    regex_feature += r"(?:wp=([rw]+)){0,1}"  # 4. write permission if known
+    regex_feature += r'(?:wp=([rw]+)){0,1}'  # 4. write permission if known
 
     regex_pg = r"[^a-z]+policy=\'([^\`]+)\'\ +"  # 1. policy of this PG path_selector
-    regex_pg += r"(?:prio=([0-9\-]+)\ +){0,1}"  # 2. priority of this PG if known
-    regex_pg += r"(?:status=([a-z]+)){0,1}"  # 3. status of this PG if known (active or enable, etc)
+    regex_pg += r'(?:prio=([0-9\-]+)\ +){0,1}'  # 2. priority of this PG if known
+    regex_pg += r'(?:status=([a-z]+)){0,1}'  # 3. status of this PG if known (active or enable, etc)
 
-    regex_disk = r"[^0-9]+"
-    regex_disk += r"([0-9]+:[0-9]+:[0-9]+:[0-9]+)\ +"  # 1. scsi_id
-    regex_disk += r"([a-z]+)\ +"  # 2. dev_name
-    regex_disk += r"([0-9]+:[0-9]+)\ +"  # 3. major:minor
-    regex_disk += r"(?:([a-z]+)\ +){0,1}"  # 4. dm_status if known, kernel level
+    regex_disk = r'[^0-9]+'
+    regex_disk += r'([0-9]+:[0-9]+:[0-9]+:[0-9]+)\ +'  # 1. scsi_id
+    regex_disk += r'([a-z]+)\ +'  # 2. dev_name
+    regex_disk += r'([0-9]+:[0-9]+)\ +'  # 3. major:minor
+    regex_disk += r'(?:([a-z]+)\ +){0,1}'  # 4. dm_status if known, kernel level
     #   failed or active
-    regex_disk += r"(?:([a-z]+)\ +){0,1}"  # 5. path_status if known, maintained
+    regex_disk += r'(?:([a-z]+)\ +){0,1}'  # 5. path_status if known, maintained
     #   by multipathd path_checker
     #   ready  or ghost or
     #   faulty or shaky
-    regex_disk += r"(?:([a-z]+)){0,1}"  # 6. online_status: running or offline
+    regex_disk += r'(?:([a-z]+)){0,1}'  # 6. online_status: running or offline
 
     _mpath_name = None
     pg_id = None
     size = None
     size_human = None
     size_bytes = None
     wwid = None
 
-    all_mpath_dict = {"by_wwid": {}, "by_mpath_name": {}, "by_scsi_id": {}}
+    all_mpath_dict = {'by_wwid': {}, 'by_mpath_name': {}, 'by_scsi_id': {}}
     mpath_dict = {}
 
     scsi_host_id_2_driver = {}
     scsi_host_id_2_h_wwpn = {}
     fc_target_id_2_t_wwpn = {}
 
     all_scsi_host_ids = scsi.get_hosts()
@@ -297,62 +298,62 @@
         if t_wwpns_of_host:
             for t_wwpn in t_wwpns_of_host:
                 t_ids = fc.fc_target_id_of_wwpn(t_wwpn)
                 if t_ids:
                     for t_id in t_ids:
                         fc_target_id_2_t_wwpn[t_id] = t_wwpn
 
-    lines = output.split("\n")
+    lines = output.split('\n')
 
     for line in lines:
         m = re.match(regex_feature, line)
         if m:
             if not wwid or not mpath_dict:
                 continue
             size = m.group(1)
-            size_human = size + "iB"
+            size_human = size + 'iB'
             size_bytes = size_human_2_size_bytes(size_human)
-            mpath_dict["size_mp"] = size
-            mpath_dict["size_human"] = size_human
-            mpath_dict["size_bytes"] = size_bytes
-            mpath_dict["feature"] = m.group(2)
-            mpath_dict["hw_handleer"] = m.group(3)
-            mpath_dict["permission"] = m.group(4)
-            mpath_dict["disk"] = {}
-            mpath_dict["t_wwpns"] = []
-            mpath_dict["h_wwpns"] = []
-            mpath_dict["t_iqns"] = []
-            mpath_dict["h_iqns"] = []
-            mpath_dict["map_info"] = []
-            mpath_dict["iface_macs"] = []
-            mpath_dict["iface_names"] = []
-            mpath_dict["target_ips"] = []
-            mpath_dict["persist_ips"] = []
-            mpath_dict["transport_types"] = []
-            mpath_dict["scsi_drivers"] = []
-            mpath_dict["host_ids"] = []
+            mpath_dict['size_mp'] = size
+            mpath_dict['size_human'] = size_human
+            mpath_dict['size_bytes'] = size_bytes
+            mpath_dict['feature'] = m.group(2)
+            mpath_dict['hw_handleer'] = m.group(3)
+            mpath_dict['permission'] = m.group(4)
+            mpath_dict['disk'] = {}
+            mpath_dict['t_wwpns'] = []
+            mpath_dict['h_wwpns'] = []
+            mpath_dict['t_iqns'] = []
+            mpath_dict['h_iqns'] = []
+            mpath_dict['map_info'] = []
+            mpath_dict['iface_macs'] = []
+            mpath_dict['iface_names'] = []
+            mpath_dict['target_ips'] = []
+            mpath_dict['persist_ips'] = []
+            mpath_dict['transport_types'] = []
+            mpath_dict['scsi_drivers'] = []
+            mpath_dict['host_ids'] = []
             # print("\n\nDEBUG - Feature - query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
 
             continue
 
         m = re.match(regex_pg, line)
         if m:
             if not wwid or not mpath_dict:
                 continue
             pg_id += 1
-            mpath_dict["path_group"][pg_id] = {}
-            mpath_dict["path_group"][pg_id]["wwid"] = wwid
-            mpath_dict["path_group"][pg_id]["mpath_name"] = _mpath_name
-            mpath_dict["path_group"][pg_id]["wwid"] = wwid
-            mpath_dict["path_group"][pg_id]["pg_id"] = pg_id
-            mpath_dict["path_group"][pg_id]["policy"] = m.group(1)
-            mpath_dict["path_group"][pg_id]["prio"] = m.group(2)
-            mpath_dict["path_group"][pg_id]["status"] = m.group(3)
-            mpath_dict["path_group"][pg_id]["disk"] = {}
+            mpath_dict['path_group'][pg_id] = {}
+            mpath_dict['path_group'][pg_id]['wwid'] = wwid
+            mpath_dict['path_group'][pg_id]['mpath_name'] = _mpath_name
+            mpath_dict['path_group'][pg_id]['wwid'] = wwid
+            mpath_dict['path_group'][pg_id]['pg_id'] = pg_id
+            mpath_dict['path_group'][pg_id]['policy'] = m.group(1)
+            mpath_dict['path_group'][pg_id]['prio'] = m.group(2)
+            mpath_dict['path_group'][pg_id]['status'] = m.group(3)
+            mpath_dict['path_group'][pg_id]['disk'] = {}
             # print("\n\nDEBUG - PG : query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
 
             continue
 
         m = re.match(regex_disk, line)
         if m:
@@ -362,141 +363,141 @@
             scsi_disk = m.group(2)
             major_minor = m.group(3)
             dm_status = m.group(4)
             path_status = m.group(5)
             online_status = m.group(6)
             # host id is the first numbers of scsi_id
             host_id = None
-            m = re.match(r"(\d+):.*", scsi_id)
+            m = re.match(r'(\d+):.*', scsi_id)
             if m:
                 host_id = m.group(1)
 
             t_wwpn = None
             h_wwpn = None
             h_iqn = None
             t_iqn = None
             iface_name = None
             iface_mac = None
             target_ip = None
             persist_ip = None
-            scsi_driver = "N/A"
+            scsi_driver = 'N/A'
 
             match_scsi_id = re.search(scsi.get_regex_scsi_id(), line)
             if match_scsi_id:
                 scsi_host_id = match_scsi_id.group(1)
-                fc_target_id = f"{match_scsi_id.group(1)}:{match_scsi_id.group(2)}:{match_scsi_id.group(3)}"
+                fc_target_id = f'{match_scsi_id.group(1)}:{match_scsi_id.group(2)}:{match_scsi_id.group(3)}'
                 if scsi_host_id in list(scsi_host_id_2_driver.keys()):
                     scsi_driver = scsi_host_id_2_driver[scsi_host_id]
 
                 if scsi_host_id in list(scsi_host_id_2_h_wwpn.keys()):
                     h_wwpn = scsi_host_id_2_h_wwpn[scsi_host_id]
 
                 if h_wwpn:
                     if fc_target_id in list(fc_target_id_2_t_wwpn.keys()):
                         t_wwpn = fc_target_id_2_t_wwpn[fc_target_id]
                 else:
                     iscsi_session = iscsi.get_iscsi_session_by_scsi_id(scsi_id)
                     if iscsi_session:
-                        h_iqn = iscsi_session["h_iqn"]
-                        t_iqn = iscsi_session["t_iqn"]
-                        iface_name = iscsi_session["iface"]
-                        iface_mac = iscsi_session["mac"]
-                        target_ip = iscsi_session["target_ip"]
-                        persist_ip = iscsi_session["persist_ip"]
+                        h_iqn = iscsi_session['h_iqn']
+                        t_iqn = iscsi_session['t_iqn']
+                        iface_name = iscsi_session['iface']
+                        iface_mac = iscsi_session['mac']
+                        target_ip = iscsi_session['target_ip']
+                        persist_ip = iscsi_session['persist_ip']
 
             disk_info_dict = {
-                "scsi_id": scsi_id,
-                "host_id": host_id,
-                "scsi_disk": scsi_disk,
-                "scsi_driver": scsi_driver,
-                "pg_id": pg_id,
-                "mpath_name": _mpath_name,
-                "wwid": wwid,
-                "dm_status": dm_status,
-                "path_status": path_status,
-                "online_status": online_status,
-                "major_minor": major_minor,
-                "size": size,
-                "size_human": size_human,
-                "size_bytes": size_bytes,
-                "t_wwpn": t_wwpn,
-                "h_wwpn": h_wwpn,
-                "t_iqn": t_iqn,
-                "h_iqn": h_iqn,
-                "iface_name": iface_name,
-                "iface_mac": iface_mac,
-                "target_ip": target_ip,
-                "persist_ip": persist_ip,
-                "transport_type": "UNKNOWN",
+                'scsi_id': scsi_id,
+                'host_id': host_id,
+                'scsi_disk': scsi_disk,
+                'scsi_driver': scsi_driver,
+                'pg_id': pg_id,
+                'mpath_name': _mpath_name,
+                'wwid': wwid,
+                'dm_status': dm_status,
+                'path_status': path_status,
+                'online_status': online_status,
+                'major_minor': major_minor,
+                'size': size,
+                'size_human': size_human,
+                'size_bytes': size_bytes,
+                't_wwpn': t_wwpn,
+                'h_wwpn': h_wwpn,
+                't_iqn': t_iqn,
+                'h_iqn': h_iqn,
+                'iface_name': iface_name,
+                'iface_mac': iface_mac,
+                'target_ip': target_ip,
+                'persist_ip': persist_ip,
+                'transport_type': 'UNKNOWN',
             }
 
             if h_iqn:
-                disk_info_dict["transport_type"] = "iSCSI"
+                disk_info_dict['transport_type'] = 'iSCSI'
 
             if h_wwpn:
-                disk_info_dict["transport_type"] = fc.fc_host_transport_type(fc.fc_host_id_of_wwpn(h_wwpn))
+                disk_info_dict['transport_type'] = fc.fc_host_transport_type(fc.fc_host_id_of_wwpn(h_wwpn))
 
-            if scsi_driver == "scsi_debug":
-                disk_info_dict["transport_type"] = "scsi_debug"
+            if scsi_driver == 'scsi_debug':
+                disk_info_dict['transport_type'] = 'scsi_debug'
 
             # Each disk has its own information, we should add each disk from mpath info to mpath info
-            if disk_info_dict["transport_type"] not in mpath_dict["transport_types"]:
-                mpath_dict["transport_types"].append(disk_info_dict["transport_type"])
+            if disk_info_dict['transport_type'] not in mpath_dict['transport_types']:
+                mpath_dict['transport_types'].append(disk_info_dict['transport_type'])
 
-            if scsi_driver and scsi_driver not in mpath_dict["scsi_drivers"]:
-                mpath_dict["scsi_drivers"].append(scsi_driver)
+            if scsi_driver and scsi_driver not in mpath_dict['scsi_drivers']:
+                mpath_dict['scsi_drivers'].append(scsi_driver)
 
-            if host_id and host_id not in mpath_dict["host_ids"]:
-                mpath_dict["host_ids"].append(host_id)
+            if host_id and host_id not in mpath_dict['host_ids']:
+                mpath_dict['host_ids'].append(host_id)
 
-            if t_wwpn and t_wwpn not in mpath_dict["t_wwpns"]:
-                mpath_dict["t_wwpns"].append(t_wwpn)
+            if t_wwpn and t_wwpn not in mpath_dict['t_wwpns']:
+                mpath_dict['t_wwpns'].append(t_wwpn)
 
-            if h_wwpn and h_wwpn not in mpath_dict["h_wwpns"]:
-                mpath_dict["h_wwpns"].append(h_wwpn)
+            if h_wwpn and h_wwpn not in mpath_dict['h_wwpns']:
+                mpath_dict['h_wwpns'].append(h_wwpn)
 
             if h_wwpn and t_wwpn:
-                map_info = {"t_wwpn": t_wwpn, "h_wwpn": h_wwpn}
-                mpath_dict["map_info"].append(map_info)
+                map_info = {'t_wwpn': t_wwpn, 'h_wwpn': h_wwpn}
+                mpath_dict['map_info'].append(map_info)
 
-            if t_iqn and t_iqn not in mpath_dict["t_iqns"]:
-                mpath_dict["t_iqns"].append(t_iqn)
+            if t_iqn and t_iqn not in mpath_dict['t_iqns']:
+                mpath_dict['t_iqns'].append(t_iqn)
 
-            if h_iqn and h_iqn not in mpath_dict["h_iqns"]:
-                mpath_dict["h_iqns"].append(h_iqn)
+            if h_iqn and h_iqn not in mpath_dict['h_iqns']:
+                mpath_dict['h_iqns'].append(h_iqn)
 
             if h_iqn and t_iqn:
-                map_info = {"t_iqn": t_iqn, "h_iqn": h_iqn}
-                mpath_dict["map_info"].append(map_info)
+                map_info = {'t_iqn': t_iqn, 'h_iqn': h_iqn}
+                mpath_dict['map_info'].append(map_info)
 
-            if iface_mac and iface_mac not in mpath_dict["iface_macs"]:
-                mpath_dict["iface_macs"].append(iface_mac)
+            if iface_mac and iface_mac not in mpath_dict['iface_macs']:
+                mpath_dict['iface_macs'].append(iface_mac)
 
-            if iface_name and h_iqn not in mpath_dict["iface_names"]:
-                mpath_dict["iface_names"].append(iface_name)
+            if iface_name and h_iqn not in mpath_dict['iface_names']:
+                mpath_dict['iface_names'].append(iface_name)
 
-            if target_ip and target_ip not in mpath_dict["target_ips"]:
-                mpath_dict["target_ips"].append(target_ip)
+            if target_ip and target_ip not in mpath_dict['target_ips']:
+                mpath_dict['target_ips'].append(target_ip)
 
-            if persist_ip and persist_ip not in mpath_dict["persist_ips"]:
-                mpath_dict["persist_ips"].append(persist_ip)
+            if persist_ip and persist_ip not in mpath_dict['persist_ips']:
+                mpath_dict['persist_ips'].append(persist_ip)
 
-            mpath_dict["disk"][disk_info_dict["scsi_disk"]] = disk_info_dict
-            mpath_dict["path_group"][pg_id]["disk"][scsi_id] = disk_info_dict
-            all_mpath_dict["by_scsi_id"][scsi_id] = disk_info_dict
+            mpath_dict['disk'][disk_info_dict['scsi_disk']] = disk_info_dict
+            mpath_dict['path_group'][pg_id]['disk'][scsi_id] = disk_info_dict
+            all_mpath_dict['by_scsi_id'][scsi_id] = disk_info_dict
             # print("\n\nDEBUG - Disk: query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
 
             continue
 
         # as regex_mpath is an aggressive regex, we leave it at the last
         # one to check.
         m = re.match(regex_mpath, line)
         if m:
-            if re.match(r"^\|", line):
+            if re.match(r'^\|', line):
                 continue
 
             _mpath_name = m.group(1)
             pg_id = 0
             wwid = _mpath_name
             if m.group(2):
                 wwid = m.group(2)
@@ -505,292 +506,292 @@
             if m.group(3):
                 dm_name = m.group(3)
 
             vendor_raw = None
             vendor = vendor_raw
             if m.group(4):
                 vendor_raw = m.group(4)
-                vendor = re.sub("[ ]+$", "", vendor_raw)
+                vendor = re.sub('[ ]+$', '', vendor_raw)
 
             product_raw = None
             product = product_raw
             if m.group(5):
                 product_raw = m.group(5)
-                product = re.sub("[ ]+$", "", product_raw)
+                product = re.sub('[ ]+$', '', product_raw)
 
             mpath_dict = {
-                "mpath_name": _mpath_name,
-                "wwid": wwid,
-                "dm_name": dm_name,
-                "vendor": vendor,
-                "vendor_raw": vendor_raw,
-                "product": product,
-                "product_raw": product_raw,
-                "h_wwpns": [],
-                "t_wwpns": [],
-                "disk": {},
-                "path_group": {},
-                "transport_types": [],
+                'mpath_name': _mpath_name,
+                'wwid': wwid,
+                'dm_name': dm_name,
+                'vendor': vendor,
+                'vendor_raw': vendor_raw,
+                'product': product,
+                'product_raw': product_raw,
+                'h_wwpns': [],
+                't_wwpns': [],
+                'disk': {},
+                'path_group': {},
+                'transport_types': [],
             }
 
-            all_mpath_dict["by_wwid"][wwid] = mpath_dict
-            all_mpath_dict["by_mpath_name"][_mpath_name] = mpath_dict
+            all_mpath_dict['by_wwid'][wwid] = mpath_dict
+            all_mpath_dict['by_mpath_name'][_mpath_name] = mpath_dict
             # print("\n\nDEBUG: query all mpath [%s]" % line)
             # print all_mpath_dict["by_mpath_name"]
             continue
     if mpath_name:
-        if mpath_name in list(all_mpath_dict["by_mpath_name"].keys()):
-            return all_mpath_dict["by_mpath_name"][mpath_name]
+        if mpath_name in list(all_mpath_dict['by_mpath_name'].keys()):
+            return all_mpath_dict['by_mpath_name'][mpath_name]
         return None
 
     return all_mpath_dict
 
 
 def mpath_name_of_wwid(wwid):  # noqa: ANN001, ANN201
     if not wwid:
-        print("FAIL: mpath_name_of_wwid() - requires wwid parameter")
+        logging.error('mpath_name_of_wwid() - requires wwid parameter')
         return None
 
     mp_devs = multipath_query_all()
     if not mp_devs:
         return None
 
-    if wwid in list(mp_devs["by_wwid"].keys()):
-        return mp_devs["by_wwid"][wwid]["mpath_name"]
+    if wwid in list(mp_devs['by_wwid'].keys()):
+        return mp_devs['by_wwid'][wwid]['mpath_name']
 
     return None
 
 
 def mpath_names_of_vendor(vendor):  # noqa: ANN001, ANN201
     """Given a Vendor return a list with all multipath device names with this vendor."""
     if not vendor:
-        print("FAIL: mpath_names_of_vendor() - requires vendor parameter")
+        logging.error('mpath_names_of_vendor() - requires vendor parameter')
         return None
 
     mp_devs = multipath_query_all()
     if not mp_devs:
         return None
 
     return [
-        mpath_info["mpath_name"]
-        for mpath_info in mp_devs["by_mpath_name"].values()
-        if "vendor" in mpath_info and mpath_info["vendor"] == vendor
+        mpath_info['mpath_name']
+        for mpath_info in mp_devs['by_mpath_name'].values()
+        if 'vendor' in mpath_info and mpath_info['vendor'] == vendor
     ]
 
 
 def mpath_check_disk_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the online status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
-        print("FAIL: mpath_check_disk_status() - requires mpath_name and scsi_disk parameters")
+        logging.error('mpath_check_disk_status() - requires mpath_name and scsi_disk parameters')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: mpath_check_disk_status() - Could not get mpath info for {mpath_name}")
+        logging.error(f'mpath_check_disk_status() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "disk" not in list(mpath_dict.keys()):
-        print(f"FAIL: mpath_check_disk_status() - Could not find any SCSI disk for {mpath_name}")
+    if 'disk' not in list(mpath_dict.keys()):
+        logging.error(f'mpath_check_disk_status() - Could not find any SCSI disk for {mpath_name}')
         return None
 
-    for disk in list(mpath_dict["disk"].keys()):
-        if scsi_disk == mpath_dict["disk"][disk]["scsi_disk"]:
-            return mpath_dict["disk"][disk]["online_status"]
+    for disk in list(mpath_dict['disk'].keys()):
+        if scsi_disk == mpath_dict['disk'][disk]['scsi_disk']:
+            return mpath_dict['disk'][disk]['online_status']
 
     return None
 
 
 def mpath_check_disk_dm_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the dm status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
-        print("FAIL: mpath_check_disk_dm_status() - requires mpath_name and scsi_disk parameters")
+        logging.error('mpath_check_disk_dm_status() - requires mpath_name and scsi_disk parameters')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: mpath_check_disk_dm_status() - Could not get mpath info for {mpath_name}")
+        logging.error(f'mpath_check_disk_dm_status() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "disk" not in list(mpath_dict.keys()):
-        print(f"FAIL: mpath_check_disk_dm_status() - Could not find any SCSI disk for {mpath_name}")
+    if 'disk' not in list(mpath_dict.keys()):
+        logging.error(f'mpath_check_disk_dm_status() - Could not find any SCSI disk for {mpath_name}')
         return None
 
-    for disk in list(mpath_dict["disk"].keys()):
-        if scsi_disk == mpath_dict["disk"][disk]["scsi_disk"]:
-            return mpath_dict["disk"][disk]["dm_status"]
+    for disk in list(mpath_dict['disk'].keys()):
+        if scsi_disk == mpath_dict['disk'][disk]['scsi_disk']:
+            return mpath_dict['disk'][disk]['dm_status']
 
     return None
 
 
 def mpath_check_disk_path_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the path status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
-        print("FAIL: mpath_check_disk_path_status() - requires mpath_name and scsi_disk parameters")
+        logging.error('mpath_check_disk_path_status() - requires mpath_name and scsi_disk parameters')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: mpath_check_disk_path_status() - Could not get mpath info for {mpath_name}")
+        logging.error(f'mpath_check_disk_path_status() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "disk" not in list(mpath_dict.keys()):
-        print(f"FAIL: mpath_check_disk_path_status() - Could not find any SCSI disk for {mpath_name}")
+    if 'disk' not in list(mpath_dict.keys()):
+        logging.error(f'mpath_check_disk_path_status() - Could not find any SCSI disk for {mpath_name}')
         return None
 
-    for disk in list(mpath_dict["disk"].keys()):
-        if scsi_disk == mpath_dict["disk"][disk]["scsi_disk"]:
-            return mpath_dict["disk"][disk]["path_status"]
+    for disk in list(mpath_dict['disk'].keys()):
+        if scsi_disk == mpath_dict['disk'][disk]['scsi_disk']:
+            return mpath_dict['disk'][disk]['path_status']
 
     return None
 
 
 def mpath_get_active_disk(mpath_name):  # noqa: ANN001, ANN201
     """From specific mpath device get which disk is the active one
     Return
     List of active SCSI disks.
     """
     if not mpath_name:
-        print("FAIL: mpath_get_active_disk() - requires mpath_name parameter")
+        logging.error('mpath_get_active_disk() - requires mpath_name parameter')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: mpath_get_active_disk() - Could not get mpath info for {mpath_name}")
+        logging.error(f'mpath_get_active_disk() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "disk" not in list(mpath_dict.keys()):
-        print(f"FAIL: mpath_get_active_disk() - Could not find any SCSI disk for {mpath_name}")
+    if 'disk' not in list(mpath_dict.keys()):
+        logging.error(f'mpath_get_active_disk() - Could not find any SCSI disk for {mpath_name}')
         return None
 
     active_disks = []
-    for disk in list(mpath_dict["disk"].keys()):
-        pg = mpath_dict["disk"][disk]["pg_id"]
-        if mpath_dict["path_group"][pg]["status"] == "active":
+    for disk in list(mpath_dict['disk'].keys()):
+        pg = mpath_dict['disk'][disk]['pg_id']
+        if mpath_dict['path_group'][pg]['status'] == 'active':
             active_disks.append(disk)
 
     if active_disks:
         return active_disks
 
-    print(f"FAIL: mpath_get_active_disk() - Could not find any active disk for {mpath_name}")
+    logging.error(f'mpath_get_active_disk() - Could not find any active disk for {mpath_name}')
     return None
 
 
 def get_free_mpaths(exclude_boot_device=True, exclude_lvm_device=True):  # noqa: ANN001, ANN201
     """Return a dict of free mpath devices."""
     all_mp_info = multipath_query_all()
     if not all_mp_info:
         # could not query multipath devices
         return None
 
-    if "by_wwid" not in list(all_mp_info.keys()):
+    if 'by_wwid' not in list(all_mp_info.keys()):
         # mpath device was not found
         print(list(all_mp_info.keys()))
         return None
 
     pvs = lvm.pv_query()
     boot_dev = linux.get_boot_device()
     boot_wwid = None
     # if for some reason we boot from a single disk, but this disk is part of multipath device
     # the mpath device should be skipped as well
     if boot_dev:
         boot_wwid = linux.get_device_wwid(boot_dev)
 
     chosen_mpaths = {}
 
-    for mp_wwid in list(all_mp_info["by_wwid"].keys()):
-        mp_info = all_mp_info["by_wwid"][mp_wwid]
+    for mp_wwid in list(all_mp_info['by_wwid'].keys()):
+        mp_info = all_mp_info['by_wwid'][mp_wwid]
         # Skip if mpath device is used for boot
-        if boot_wwid == mp_info["wwid"] and exclude_boot_device:
+        if boot_wwid == mp_info['wwid'] and exclude_boot_device:
             print(f"DEBUG: get_free_mpaths() - skip {mp_info['mpath_name']} as it is used for boot")
             continue
 
         # Skip if it is used by LVM
         if pvs and exclude_lvm_device:
             mp_used_by_lvm = False
             for pv in list(pvs.keys()):
-                if mpath_device_2_mpath_name(pv) == mp_info["mpath_name"]:
+                if mpath_device_2_mpath_name(pv) == mp_info['mpath_name']:
                     mp_used_by_lvm = True
                     print(f"DEBUG: get_free_mpaths() - skip {mp_info['mpath_name']} as it is used for LVM")
                     continue
             if mp_used_by_lvm:
                 continue
 
-        chosen_mpaths[mp_info["mpath_name"]] = mp_info
+        chosen_mpaths[mp_info['mpath_name']] = mp_info
 
     return chosen_mpaths
 
 
 def h_wwpns_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the h_wwpns of specific mpath device."""
     if not mpath_name:
-        print("FAIL: h_wwpns_of_mpath() - requires mpath_name parameter")
+        logging.error('h_wwpns_of_mpath() - requires mpath_name parameter')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: h_wwpns_of_mpath() - Could not get mpath info for {mpath_name}")
+        logging.error(f'h_wwpns_of_mpath() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "h_wwpns" in mpath_dict:
-        return mpath_dict["h_wwpns"]
+    if 'h_wwpns' in mpath_dict:
+        return mpath_dict['h_wwpns']
     return None
 
 
 def t_wwpns_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the h_wwpns of specific mpath device."""
     if not mpath_name:
-        print("FAIL: t_wwpns_of_mpath() - requires mpath_name parameter")
+        logging.error('t_wwpns_of_mpath() - requires mpath_name parameter')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: t_wwpns_of_mpath() - Could not get mpath info for {mpath_name}")
+        logging.error(f't_wwpns_of_mpath() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "t_wwpns" in mpath_dict:
-        return mpath_dict["t_wwpns"]
+    if 't_wwpns' in mpath_dict:
+        return mpath_dict['t_wwpns']
     return None
 
 
 def iface_macs_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the iface_macs_of_mpath of specific mpath device."""
     if not mpath_name:
-        print("FAIL: iface_macs_of_mpath() - requires mpath_name parameter")
+        logging.error('iface_macs_of_mpath() - requires mpath_name parameter')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: iface_macs_of_mpath() - Could not get mpath info for {mpath_name}")
+        logging.error(f'iface_macs_of_mpath() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "iface_macs" in mpath_dict:
-        return mpath_dict["iface_macs"]
+    if 'iface_macs' in mpath_dict:
+        return mpath_dict['iface_macs']
     return None
 
 
 def transport_types_of_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Return the transport_types of specific mpath device."""
     if not mpath_name:
-        print("FAIL: transport_types_of_mpath() - requires mpath_name parameter")
+        logging.error('transport_types_of_mpath() - requires mpath_name parameter')
         return None
 
     mpath_dict = multipath_query_all(mpath_name)
     if not mpath_dict:
-        print(f"FAIL: transport_types_of_mpath() - Could not get mpath info for {mpath_name}")
+        logging.error(f'transport_types_of_mpath() - Could not get mpath info for {mpath_name}')
         return None
 
-    if "transport_types" in mpath_dict:
-        return mpath_dict["transport_types"]
+    if 'transport_types' in mpath_dict:
+        return mpath_dict['transport_types']
     return None
 
 
 def multipath_show(mpath_name=None):  # noqa: ANN001, ANN201
-    cmd = "multipath -ll"
+    cmd = 'multipath -ll'
     if mpath_name:
-        cmd += f" {mpath_name}"
+        cmd += f' {mpath_name}'
     run(cmd)
 
 
 def multipath_reload(mpath_name=None):  # noqa: ANN001, ANN201
     """Usage
     multipath_reload()
     Purpose
@@ -800,38 +801,38 @@
     Returns
         1
             or
         undef
     Exceptions
         N/A.
     """
-    cmd = "multipath -r"
+    cmd = 'multipath -r'
     if mpath_name:
-        cmd += f" {mpath_name}"
-    if run(cmd).returncode != 0:
+        cmd += f' {mpath_name}'
+    if run(cmd).rc != 0:
         return False
 
     return True
 
 
 def remove_mpath(mpath_name):  # noqa: ANN001, ANN201
     """Remove specific mpath."""
     if not mpath_name:
-        print("FAIL: remove_mpath() - requires mpath_name parameter")
+        logging.error('remove_mpath() - requires mpath_name parameter')
         return False
-    if run(f"multipath -f {mpath_name}").returncode != 0:
-        print(f"FAIL: Could not remove mpath {mpath_name}")
+    if run(f'multipath -f {mpath_name}').rc != 0:
+        logging.error(f'Could not remove mpath {mpath_name}')
         return False
     return True
 
 
 def flush_all():  # noqa: ANN201
     """Flush all unused multipath device maps."""
-    cmd = "multipath -F"
-    if run(cmd).returncode != 0:
+    cmd = 'multipath -F'
+    if run(cmd).rc != 0:
         return False
 
     return True
 
 
 def multipath_backup_conf(bak_file):  # noqa: ANN001, ANN201
     """backup_mp_conf ()
@@ -845,26 +846,26 @@
     true
         or
     False           # file exists or source file not exists;
     Exceptions
     N/A.
     """
     if not Path(MULTIPATH_CONF_PATH).is_file():
-        print(f"FAIL: {MULTIPATH_CONF_PATH} does not exist")
+        logging.error(f'{MULTIPATH_CONF_PATH} does not exist')
         return False
 
     if Path(bak_file).is_file():
-        print(f"FAIL: mpath backup file {bak_file} already exists")
+        logging.error(f'mpath backup file {bak_file} already exists')
         return False
 
-    print(f"INFO: Backing up {MULTIPATH_CONF_PATH} to {bak_file}")
-    cmd = f"cp -f {MULTIPATH_CONF_PATH} {bak_file}"
+    logging.info(f'Backing up {MULTIPATH_CONF_PATH} to {bak_file}')
+    cmd = f'cp -f {MULTIPATH_CONF_PATH} {bak_file}'
     ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print(f"FAIL: Could not backup {MULTIPATH_CONF_PATH}")
+        logging.error(f'Could not backup {MULTIPATH_CONF_PATH}')
         print(output)
         return False
 
     return True
 
 
 def multipath_restore_conf(bak_file):  # noqa: ANN001, ANN201
@@ -880,22 +881,22 @@
     True
         or
     False           # file exists or source file not exists;
     Exceptions
     N/A.
     """
     if not Path(bak_file).is_file():
-        print(f"FAIL: {bak_file} does not exist")
+        logging.error(f'{bak_file} does not exist')
         return False
 
-    print(f"INFO: Restoring multipath configuration from {bak_file}")
-    cmd = f"cp -f {bak_file} {MULTIPATH_CONF_PATH}"
+    logging.info(f'Restoring multipath configuration from {bak_file}')
+    cmd = f'cp -f {bak_file} {MULTIPATH_CONF_PATH}'
     ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print(f"FAIL: Could not restore backup from {bak_file}")
+        logging.error(f'Could not restore backup from {bak_file}')
         print(output)
         return False
 
     multipath_reload_conf()
     return True
 
 
@@ -911,15 +912,15 @@
         1
             or
         undef
     Exceptions
         N/A.
     """
     cmd = "multipathd -k'reconfig'"
-    ret = run(cmd, verbose=True).returncode
+    ret = run(cmd).rc
 
     multipath_reload()
     if ret != 0:
         return False
 
     return True
 
@@ -941,26 +942,26 @@
     undef
     Exceptions
     N/A.
     """
     all_mp_info_dict = multipath_query_all()
     if not all_mp_info_dict:
         return False
-    current_wwids = list(all_mp_info_dict["by_wwid"].keys())
+    current_wwids = list(all_mp_info_dict['by_wwid'].keys())
     if not current_wwids:
         return False
 
-    if not mpath_conf_set("/blacklist/wwid", ".*"):
+    if not mpath_conf_set('/blacklist/wwid', '.*'):
         return False
 
     for wwid in current_wwids:
-        if not mpath_conf_set("/blacklist_exceptions/wwid[last()+1]", wwid):
+        if not mpath_conf_set('/blacklist_exceptions/wwid[last()+1]', wwid):
             return False
 
-    print("INFO: Reloading updated multipath configuration")
+    logging.info('Reloading updated multipath configuration')
     multipath_reload_conf()
     return True
 
 
 def mpath_conf_remove(path, value):  # noqa: ANN001, ANN201
     """Remove parameter from multipath config using augeas.
     For non-unique paths, use return of mpath_conf_match as path
@@ -975,17 +976,17 @@
 
     Raises:
       IOError: Augeas save fails. Check if multipath.conf changes are valid.
     """
     matched_path = mpath_conf_match(path, value)
 
     if matched_path:
-        out = run(f'augtool -s rm "{matched_path}"', capture_output=True, verbose=False).output
-        if "Saved 1 file(s)" not in out:
-            print(f"FAIL: unable to set {path} to {value}")
+        out = run(f'augtool -s rm "{matched_path}"').stdout
+        if 'Saved 1 file(s)' not in out:
+            logging.error(f'unable to set {path} to {value}')
             return False
 
     return True
 
 
 def mpath_conf_match(path, value):  # noqa: ANN001, ANN201
     """Checks if parameter is set in multipath.conf using augeas
@@ -996,22 +997,22 @@
     Args:
       path: eg. "/blacklist/wwid"
       value: eg. "<device wwid>"
 
     Returns:
       matched path or None
     """
-    if not linux.install_package("augeas", verbose=False):
-        print("FAIL: Could not install augeas")
+    if not linux.install_package('augeas'):
+        logging.error('Could not install augeas')
         return None
 
     full_path = path if path.startswith(aug_conf_path) else aug_conf_path + path
 
     # successfully matches also when end of path is not unique - path[*] value, but not path[*]/path value
-    out = run(f'augtool match "{full_path}" "{value}"', capture_output=True, verbose=False).output
+    out = run(f'augtool match "{full_path}" "{value}"').stdout
 
     # augtool prints path when matched, return codes seems useless
     if aug_conf_path in out:
         # returning path, as it can be useful when modifying non-unique paths
         return out
     return None
 
@@ -1031,97 +1032,97 @@
 
     Raises:
       IOError: Augeas save fails. Check if multipath.conf changes are valid.
     """
     full_path = path if path.startswith(aug_conf_path) else aug_conf_path + path
 
     # Need to check if not already exists to avoid duplicates
-    path_to_match = re.sub(r"\[[^]]*]", "[.]", path)  # in case path expressions are being used
+    path_to_match = re.sub(r'\[[^]]*]', '[.]', path)  # in case path expressions are being used
     matched_path = mpath_conf_match(path_to_match, value)
 
     if not matched_path:
-        if not linux.is_installed("augeas"):
-            print("FAIL: Could not install augeas")
+        if not linux.is_installed('augeas'):
+            logging.error('Could not install augeas')
             return False
-        out = run(f'augtool -s set "{full_path}" "{value}"', capture_output=True, verbose=False).output
-        if "Saved 1 file(s)" not in out:
-            print(f"FAIL: unable to set {path} to {value}. Try")
+        out = run(f'augtool -s set "{full_path}" "{value}"').stdout
+        if 'Saved 1 file(s)' not in out:
+            logging.error(f'unable to set {path} to {value}. Try')
             return False
 
     return True
 
 
 def mp_query_conf(config_str):  # noqa: ANN001, ANN201
     """Parse string containing multipath config to a dict."""
-    regex_option = r"^[ \t]*"
-    regex_option += r"([^\ #=\t]+)"
-    regex_option += r"[\ \t]+"
+    regex_option = r'^[ \t]*'
+    regex_option += r'([^\ #=\t]+)'
+    regex_option += r'[\ \t]+'
     regex_option += r"(?:'|\"){0,1}"
     regex_option += r"([^'\"]+)"
     regex_option += r"(?:'|\"){0,1}"
-    regex_option += r"(?:\#.*){0,1}"  # we remove '|"
+    regex_option += r'(?:\#.*){0,1}'  # we remove '|"
 
-    regex_section = r"[ \t]*([a-z_]+)[ \t]*\{"
+    regex_section = r'[ \t]*([a-z_]+)[ \t]*\{'
     if not config_str:
         return None
 
     config_dict = {}
 
     current_section = None
     section_name = None
-    for line in config_str.split("\n"):
+    for line in config_str.split('\n'):
         m = re.match(regex_section, line)
         if m:
             key = m.group(1)
-            if key == "device":
+            if key == 'device':
                 if not section_name:
                     continue
-                if "devs" not in list(config_dict[section_name].keys()):
-                    config_dict[section_name]["devs"] = []
+                if 'devs' not in list(config_dict[section_name].keys()):
+                    config_dict[section_name]['devs'] = []
                 # We are in a subsection, need to update current_section
                 tmp_dict = {}
-                config_dict[section_name]["devs"].append(tmp_dict)
+                config_dict[section_name]['devs'].append(tmp_dict)
                 # poiting current_section to last item in the list
-                current_section = config_dict[section_name]["devs"][-1]
+                current_section = config_dict[section_name]['devs'][-1]
                 continue
 
-            if key == "multipath":
+            if key == 'multipath':
                 if not section_name:
                     continue
-                if "mpaths" not in list(config_dict[section_name].keys()):
-                    config_dict[section_name]["mpaths"] = []
+                if 'mpaths' not in list(config_dict[section_name].keys()):
+                    config_dict[section_name]['mpaths'] = []
                 # We are in a subsection, need to update current_section
                 tmp_dict = {}
-                config_dict[section_name]["mpaths"].append(tmp_dict)
+                config_dict[section_name]['mpaths'].append(tmp_dict)
                 # pointing current_section to last item in the list
-                current_section = config_dict[section_name]["mpaths"][-1]
+                current_section = config_dict[section_name]['mpaths'][-1]
                 continue
 
             if key not in config_dict:
                 config_dict[key] = {}
             current_section = config_dict[key]
             section_name = key
             continue
         m = re.match(regex_option, line)
         if m:
             key = m.group(1)
             value = m.group(2)
             if current_section is None:
                 continue
-            if key == "devnode":
-                if "devnodes" not in list(current_section.keys()):
-                    current_section["devnodes"] = []
-                current_section["devnodes"].append(value)
+            if key == 'devnode':
+                if 'devnodes' not in list(current_section.keys()):
+                    current_section['devnodes'] = []
+                current_section['devnodes'].append(value)
                 continue
 
-            match_section = re.match("^blacklist", section_name)
-            if key == "wwid" and match_section:
-                if "wwids" not in list(current_section.keys()):
-                    current_section["wwids"] = []
-                current_section["wwids"].append(value)
+            match_section = re.match('^blacklist', section_name)
+            if key == 'wwid' and match_section:
+                if 'wwids' not in list(current_section.keys()):
+                    current_section['wwids'] = []
+                current_section['wwids'].append(value)
                 continue
 
             current_section[key] = value
             continue
 
     return config_dict
 
@@ -1133,15 +1134,15 @@
         Load multipath config file and return it as a dict
     Parameter
         N/A
     Returns
         mp_conf_dict.
     """
     if not Path(MULTIPATH_CONF_PATH).is_file():
-        print(f"FAIL: {MULTIPATH_CONF_PATH} does not exist")
+        logging.error(f'{MULTIPATH_CONF_PATH} does not exist')
         return None
 
     cfg_text = _load_config(MULTIPATH_CONF_PATH)
     if not cfg_text:
         return None
 
     return mp_query_conf(cfg_text)
@@ -1151,84 +1152,84 @@
     """Parse multipath config file to dict."""
     with Path(config_file).open() as f:
         return f.read()
 
 
 def _save_config(config_dict, config_file=MULTIPATH_CONF_PATH):  # noqa: ANN001, ANN202
     """Convert multipath config dict to string and save to file."""
-    config_str = ""
-    if "defaults" in list(config_dict.keys()):
-        config_str += "defaults {\n"
-        for key in list(config_dict["defaults"].keys()):
+    config_str = ''
+    if 'defaults' in list(config_dict.keys()):
+        config_str += 'defaults {\n'
+        for key in list(config_dict['defaults'].keys()):
             config_str += f"\t{key} {config_dict['defaults'][key]}\n"
-        config_str += "}\n"
+        config_str += '}\n'
 
-    blacklist_sections = ["blacklist", "blacklist_exceptions"]
+    blacklist_sections = ['blacklist', 'blacklist_exceptions']
     for b_section in blacklist_sections:
         if b_section in list(config_dict.keys()):
-            config_str += "%s {\n" % b_section
+            config_str += '%s {\n' % b_section
 
-            if "devnodes" in list(config_dict[b_section].keys()):
-                for node in config_dict[b_section]["devnodes"]:
+            if 'devnodes' in list(config_dict[b_section].keys()):
+                for node in config_dict[b_section]['devnodes']:
                     config_str += f'\tdevnode "{node}"\n'
 
-            if "wwids" in list(config_dict[b_section].keys()):
-                for wwid in config_dict[b_section]["wwids"]:
+            if 'wwids' in list(config_dict[b_section].keys()):
+                for wwid in config_dict[b_section]['wwids']:
                     config_str += f'\twwid "{wwid}"\n'
 
-            if "devs" in list(config_dict[b_section].keys()):
-                for device in config_dict[b_section]["devs"]:
-                    config_str += "\tdevice {\n"
+            if 'devs' in list(config_dict[b_section].keys()):
+                for device in config_dict[b_section]['devs']:
+                    config_str += '\tdevice {\n'
                     for key in list(device.keys()):
-                        config_str += f"\t\t{key} {device[key]}\n"
-                    config_str += "\t}\n"
+                        config_str += f'\t\t{key} {device[key]}\n'
+                    config_str += '\t}\n'
 
-            config_str += "}\n"
+            config_str += '}\n'
 
-    if "devices" in list(config_dict.keys()):
-        config_str += "devices {\n"
-        for vendor in list(config_dict["devices"].keys()):
-            for product in config_dict["devices"][vendor]:
-                config_str += "\tdevice {\n"
+    if 'devices' in list(config_dict.keys()):
+        config_str += 'devices {\n'
+        for vendor in list(config_dict['devices'].keys()):
+            for product in config_dict['devices'][vendor]:
+                config_str += '\tdevice {\n'
                 for name in list(product.keys()):
-                    config_str += f"\t\t{name} {product[name]}\n"
-                config_str += "\t}\n"
-        config_str += "}\n"
-
-    if "multipaths" in list(config_dict.keys()):
-        config_str += "multipaths {\n"
-        for key in list(config_dict["multipaths"].keys()):
-            config_str += "\tmultipath {\n"
-            for wwid in config_dict["multipaths"][key]:
-                config_str += f"\t\t{key} {wwid}\n"
-            config_str += "}\n"
-        config_str += "}\n"
+                    config_str += f'\t\t{name} {product[name]}\n'
+                config_str += '\t}\n'
+        config_str += '}\n'
+
+    if 'multipaths' in list(config_dict.keys()):
+        config_str += 'multipaths {\n'
+        for key in list(config_dict['multipaths'].keys()):
+            config_str += '\tmultipath {\n'
+            for wwid in config_dict['multipaths'][key]:
+                config_str += f'\t\t{key} {wwid}\n'
+            config_str += '}\n'
+        config_str += '}\n'
 
-    with Path(config_file).open("w") as f:
+    with Path(config_file).open('w') as f:
         f.write(config_str)
 
     return True
 
 
 def mpath_device_2_mpath_name(mpath_device):  # noqa: ANN001, ANN201
     """Convert a specific multipath device to mpath_name
     E.g. /dev/mapper/mpathap1 => mpatha.
     """
-    multipath_dev_regex = r"/dev/mapper\/(.*)"
+    multipath_dev_regex = r'/dev/mapper\/(.*)'
     m = re.match(multipath_dev_regex, mpath_device)
     if m:
         # need to remove partition information
         # Multipath names has changed on RHEL7 and if a device name ends in letter the
         # partition number is just append to the device number, if it ends in digit
         # it appends 'p' before the partition number
         # So we can have device partitions as below...
         # device_name = "mapper/360a98000572d5765636f69746f6a4f6a1"
         # device_name = "mapper/360a98000572d5765636f69746f6a4f61p1"
         device_name = m.group(1)
-        m = re.match(r"(.*)p?\d", device_name)
+        m = re.match(r'(.*)p?\d', device_name)
         if not m:
             # does not seem to be a valid mpath device
             return None
         device_name = m.group(1)
         # remove trailing p if it exists
-        return re.sub(r"(\S+)p$", r"\1", device_name)
+        return re.sub(r'(\S+)p$', r'\1', device_name)
     return None
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/net.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/net.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,104 @@
 """net.py: Module to manipulate network devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import ipaddress
+import logging
 import os.path
-import re  # regex
+import re
 from os import listdir, readlink
 from os.path import lexists
 from pathlib import Path
+from typing import List, Union
 
-import netifaces
-
-from sts import linux
+from sts import host_init, linux
 from sts.utils.cmdline import exists, run, run_ret_out
 
-__author__ = "Bruno Goncalves"
-__copyright__ = "Copyright (c) 2016 Red Hat, Inc. All rights reserved."
+__author__ = 'Bruno Goncalves'
+__copyright__ = 'Copyright (c) 2016 Red Hat, Inc. All rights reserved.'
 
-sysfs_class_net_path = "/sys/class/net"
+sysfs_class_net_path = '/sys/class/net'
 
 
 def is_mac(mac):  # noqa: ANN001, ANN201
     """Check if given MAC is  on valid format."""
     if standardize_mac(mac):
         return True
     return False
 
 
-def get_nics():  # noqa: ANN201
-    """Return list of all NICs on the server."""
-    ifaces = netifaces.interfaces()
-    if ifaces is None:  # No NIC on this server
-        return None
+def get_nics() -> List[str]:
+    """Return list of all NICs on the host."""
+    host = host_init()
+    return host.interface.names()
 
-    return ifaces
 
+def get_eth_nics() -> List[str]:
+    """Return list of interfaces with link/ether."""
+    nics = get_nics()
+    return [i for i in nics if get_mac_of_nic(i)]
 
-def get_mac_of_nic(nic):  # noqa: ANN001, ANN201
+
+def get_mac_of_nic(nic: str) -> Union[str, None]:
     """Given a NIC name return its MAC address."""
+    cp = run(f'ip -o link show {nic}').stdout
+    if not cp:
+        return None
+    ip_link = cp.split()
     try:
-        mac = netifaces.ifaddresses(nic)[netifaces.AF_PACKET][0]["addr"]
-    except Exception as e:
-        print(repr(e))
+        mac = ip_link[ip_link.index('link/ether') + 1]
+    except ValueError:
         return None
-    else:
-        return mac
+
+    return mac
 
 
 def get_nic_of_mac(mac_address):  # noqa: ANN001, ANN201
     """Give an MAC address return the server interface name."""
     if not mac_address:
-        print("FAIL: get_nic_of_mac() - requires mac as argument")
+        logging.error('get_nic_of_mac() - requires mac as argument')
         return None
 
     mac = mac_address.lower()
 
     if not is_mac(mac):
-        print(f"FAIL: get_nic_of_mac() - {mac} does not seem to be a valid MAC")
+        logging.error(f'get_nic_of_mac() - {mac} does not seem to be a valid MAC')
         return None
 
-    nics = get_nics()
+    nics = get_eth_nics()
     if not nics:
         return None
 
     for nic in nics:
         if mac == get_mac_of_nic(nic):
             return nic
 
     return None
 
 
-def get_ip_address_of_nic(nic):  # noqa: ANN001, ANN201
+def get_ip_addresses_of_nic(nic: str) -> Union[List[str], None]:
     """Get IPv4 of specific network interface."""
-    try:
-        ip = netifaces.ifaddresses(nic)[netifaces.AF_INET][0]["addr"]
-    except KeyError as e:
-        print(f"KeyError - Iface probably does not have a IP address - {e!s}")
-    except Exception as e:
-        print(repr(e))
-    else:
-        return ip
-    return None
-
+    host = host_init()
+    if not host.interface(nic).exists:
+        return None
 
-def get_ipv6_address_of_nic(nic):  # noqa: ANN001, ANN201
-    """Get IPv6 of specific network interface."""
-    try:
-        ip = netifaces.ifaddresses(nic)[netifaces.AF_INET6][0]["addr"]
-    except KeyError as e:
-        print(f"KeyError - Iface probably does not have a IPv6 address - {e!s}")
-    except Exception as e:
-        print(repr(e))
-    else:
-        return ip
-    return None
+    return host.interface(nic).addresses
 
 
-def get_nic_of_ip(ip):  # noqa: ANN001, ANN201
+def get_nic_of_ip(ip: str) -> Union[str, None]:
     """Given an IP address return the NIC name using it."""
-    if not ip:
-        return None
-
     nics = get_nics()
-    if not nics:
-        return None
 
     for nic in nics:
-        if ip == get_ip_address_of_nic(nic):
+        addresses = get_ip_addresses_of_nic(nic)
+        if addresses and ip in addresses:
             return nic
+
     return None
 
 
 def nic_2_driver():  # noqa: ANN201
     """Return a dictionary where nic name is the key and driver name is the value.
     Will skip sub interfaces, loop device, tun, vboxnet0.
     The arguments are:
@@ -120,20 +106,20 @@
     return_output (Dict): Return a dictionary
     Returns:
     dict: Return dict containing all NICs.
     """
     nic_dict = {}
     for nic in listdir(sysfs_class_net_path):
         if (
-            nic == "."
-            or nic == ".."
-            or nic == "lo"
-            or re.match("^tun[0-9]+", nic)  # loop
-            or re.match("^vboxnet[0-9]+", nic)  # TUN NIC
-            or re.search(r"\.", nic)  # virtualbox NIC.
+            nic == '.'
+            or nic == '..'
+            or nic == 'lo'
+            or re.match('^tun[0-9]+', nic)  # loop
+            or re.match('^vboxnet[0-9]+', nic)  # TUN NIC
+            or re.search(r'\.', nic)  # virtualbox NIC.
         ):  # sub-interface
             continue
         nic_dict[nic] = driver_of_nic(nic)
     # print nic_dict
     return nic_dict
 
 
@@ -148,26 +134,26 @@
     nic: NIC name, e.g. eth0
     Returns:
     str: Driver name.
     """
     nic = phy_nic_of(nic)
     nic_file = Path(sysfs_class_net_path)
     if not (nic_file / nic).exists():
-        print(f"FAIL: No such NIC exists: {nic}")
+        logging.error(f'No such NIC exists: {nic}')
         print(nic_file)
         return None
-    driver_file = f"/sys/class/net/{nic}/device/driver"
+    driver_file = f'/sys/class/net/{nic}/device/driver'
     if not lexists(driver_file):
-        print(f"FAIL: path {driver_file} does not exist")
+        logging.error(f'path {driver_file} does not exist')
         return None
     # from a symlink get real path
     real_path = os.readlink(driver_file)
-    m = re.match(".*drivers/(.*)$", real_path)
+    m = re.match('.*drivers/(.*)$', real_path)
     if not m:
-        print(f"FAIL: Could not find driver name for {nic}")
+        logging.error(f'Could not find driver name for {nic}')
         return None
     return m.group(1)
 
 
 # End of driver_of_nic()
 
 
@@ -176,24 +162,24 @@
     The arguments are:
     nic: NIC name, e.g. eth0.802-fcoe
     Returns:
     str: phy NIC, e.g. eth0.
     """
     if not nic:
         return None
-    return re.sub(r"\..+$", "", nic)
+    return re.sub(r'\..+$', '', nic)
 
 
 def get_pci_id_of_nic(nic):  # noqa: ANN001, ANN201
     """From a specific network interface return its PCI id."""
     regex_pci_id = linux.get_regex_pci_id()
-    sys_path = f"{sysfs_class_net_path}/{nic}"
+    sys_path = f'{sysfs_class_net_path}/{nic}'
     link_path = readlink(sys_path)
     # print("DEBUG: get_pci_id_of_nic - %s" % link_path)
-    m = re.search(f"({regex_pci_id})/net/{nic}", link_path)
+    m = re.search(f'({regex_pci_id})/net/{nic}', link_path)
     if m:
         return m.group(1)
     return None
 
 
 def get_ip_version(addr):  # noqa: ANN001, ANN201
     """Given an address, tries to check if it is IPv6 or not
@@ -225,32 +211,32 @@
     Returns
         mac
             or
         None.
     """
     if not mac:
         return None
-    regex_standard_mac = "^(?:[0-9A-F]{2}:){5}[0-9A-F]{2}$"
+    regex_standard_mac = '^(?:[0-9A-F]{2}:){5}[0-9A-F]{2}$'
 
     mac = mac.lower()
-    mac = re.sub("^0x", "", mac)
-    mac = re.sub("[^0-9A-Fa-f]", "", mac)
+    mac = re.sub('^0x', '', mac)
+    mac = re.sub('[^0-9A-Fa-f]', '', mac)
     # If mac given has no ':' we will add it
-    if re.match("[0-9a-f]{12}", mac):
-        mac_regex = re.compile("(.{2})")
-        mac = mac_regex.sub(r"\g<1>:", mac)
-        mac = re.sub(":$", "", mac)
+    if re.match('[0-9a-f]{12}', mac):
+        mac_regex = re.compile('(.{2})')
+        mac = mac_regex.sub(r'\g<1>:', mac)
+        mac = re.sub(':$', '', mac)
 
     if re.match(regex_standard_mac, mac, re.IGNORECASE):
         return mac
 
     return None
 
 
-def convert_netmask(netmask="255.255.255.0"):  # noqa: ANN001, ANN201
+def convert_netmask(netmask='255.255.255.0'):  # noqa: ANN001, ANN201
     """Converts subnet mask to CIDR prefix.
     netmask: common subnet mask.
     """
     try:
         cidr = ipaddress.IPv4Network((0, netmask)).prefixlen
     except ValueError as e:
         print(e)
@@ -261,88 +247,87 @@
 
 def if_down(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface down using ifdown tool
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        print("FAIL: if_down() - requires nic or mac as argument")
+        logging.error('if_down() - requires nic or mac as argument')
         return None
 
     # ifup/ifdown scripts are not shipped by default on RHEL-8+
     if (
-        not exists("ifdown")
-        and linux.is_installed("NetworkManager")
-        and not linux.install_package("NetworkManager-initscripts-updown")
+        not exists('ifdown')
+        and linux.is_installed('NetworkManager')
+        and not linux.install_package('NetworkManager-initscripts-updown')
     ):
         print('FAIL: unable to run "ifdown" command')
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
-    if run(f"ifdown {nic}"):
+    if run(f'ifdown {nic}'):
         return True
     return False
 
 
 def if_up(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface up using ifup tool
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        print("FAIL: if_up() - requires nic or mac as argument")
+        logging.error('if_up() - requires nic or mac as argument')
         return None
 
     # ifup/ifdown scripts are not shipped by default on RHEL-8+
     if (
-        not exists("ifup")
-        and linux.is_installed("NetworkManager")
-        and not linux.install_package("NetworkManager-initscripts-updown")
+        not exists('ifup')
+        and linux.is_installed('NetworkManager')
+        and not linux.install_package('NetworkManager-initscripts-updown')
     ):
         print('FAIL: unable to run "ifup" command')
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
-    if run(f"ifup {nic}"):
+    if run(f'ifup {nic}'):
         return True
     return False
 
 
 def iface_up(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface up
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        print("FAIL: iface_up() - requires nic or mac as argument")
+        logging.error('iface_up() - requires nic or mac as argument')
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
 
-    retcode, output = run_ret_out(f"ip link set {nic} up", return_output=True)
+    retcode, output = run_ret_out(f'ip link set {nic} up', return_output=True)
     if retcode != 0:
         print(output)
         return False
     return True
 
 
 def iface_down(nic_or_mac):  # noqa: ANN001, ANN201
     """Bring the interface down
     Parameters:
      Interface name, or it's MAC address.
     """
     if not nic_or_mac:
-        print("FAIL: iface_down() - requires nic or mac as argument")
+        logging.error('iface_down() - requires nic or mac as argument')
         return False
 
     nic = get_nic_of_mac(nic_or_mac) if is_mac(nic_or_mac) else nic_or_mac
-
-    retcode, output = run_ret_out(f"ip link set {nic} down", return_output=True)
+    retcode, output = run_ret_out(f'ip link set {nic} down', return_output=True)
     if retcode != 0:
         print(output)
         return False
     return True
 
 
 def set_ifcfg(nic_or_mac, parameters):  # noqa: ANN001, ANN201
@@ -350,216 +335,205 @@
     Parameters:
      nic_or_mac: interface name or mac address
      parameters: dict of params e.g. {'IPADDR': '10.37.151.7'}.
     """
     if is_mac(nic_or_mac):
         nic = get_nic_of_mac(nic_or_mac)
         if not nic:
-            print("FAIL: Couldn't find NIC from MAC.")
+            logging.error("Couldn't find NIC from MAC.")
             return False
     else:
         nic = nic_or_mac
 
-    file_to_edit = f"/etc/sysconfig/network-scripts/ifcfg-{nic}"
+    file_to_edit = f'/etc/sysconfig/network-scripts/ifcfg-{nic}'
     if not linux.edit_config(file_to_edit, parameters):
         return False
 
     if_down(nic)
     if_up(nic)
     return True
 
 
-def get_default_iface():  # noqa: ANN201
-    """Returns tuple with ip and interface.
-    example: ('10.1.1.1', 'eno1').
-    """
-    try:
-        return netifaces.default_gateway()[netifaces.AF_INET]
-    except Exception as e:
-        print(repr(e))
-        return None
-
-
 def nm_get_conn(nic_or_mac):  # noqa: ANN001, ANN201
     """Returns NetworkManager connection UUID
     nic_or_mac: interface name or mac address.
     """
     if is_mac(nic_or_mac):
         nic = get_nic_of_mac(nic_or_mac)
         if not nic:
-            print("FAIL: Couldn't find NIC from MAC.")
+            logging.error("Couldn't find NIC from MAC.")
             return None
     else:
         nic = nic_or_mac
 
     conn = nm_get_conn_from_dev(nic)
     if not conn:
-        print(f"WARN: {nic} not used in any active connection. Trying connections with same name")
+        logging.warning(f'{nic} not used in any active connection. Trying connections with same name')
         # Check connection with same name as device
         if nm_get_conn_iface(nic) == nic:
             return nm_get_conn_uuid(nic)
         return None
     conn = str(conn)
     return nm_get_conn_uuid(conn)
 
 
 def nm_get_conn_iface(conn):  # noqa: ANN001, ANN201
     """Returns interface name used by NM connection
     conn: connection id or uuid.
     """
     cmd = f"nmcli -g connection.interface-name con show '{conn}'"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Couldn't get connection.interface-name for connection " + conn)
+        logging.error(f"Couldn't get connection.interface-name for connection {conn}")
         print(output)
         return None
     return output
 
 
 def nm_get_conn_uuid(conn):  # noqa: ANN001, ANN201
     """Returns NetworkManager connection UUID
     conn: connection id.
     """
     cmd = f"nmcli -g connection.uuid conn show '{conn}'"
     print(cmd)
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Couldn't get NM connection uuid using " + conn)
+        logging.error(f"Couldn't get NM connection uuid using {conn}")
         print(output)
         return None
     return output
 
 
 def nm_get_conn_from_dev(nic):  # noqa: ANN001, ANN201
     """Returns connection id(name) using specified device.
     nic: network interface - device.
     """
     nic = str(nic)
-    cmd = "nmcli -g GENERAL.CONNECTION device show " + nic
+    cmd = 'nmcli -g GENERAL.CONNECTION device show ' + nic
 
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Couldn't get NM connection using device " + nic)
+        logging.error(f"Couldn't get NM connection using device {nic}")
         print(output)
         return None
     return output
 
 
 def nm_get_dev_from_conn(conn):  # noqa: ANN001, ANN201
     """Returns a device used by specified connection
     conn: networkmanager connection id(name) or uuid.
     """
     conn = str(conn)
     cmd = f"nmcli -g connection.interface-name con show '{conn}'"
 
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Couldn't get device used by NM connection " + conn)
+        logging.error(f"Couldn't get device used by NM connection {conn}")
         print(output)
         return None
     return output
 
 
 def nm_conn_up(conn):  # noqa: ANN001, ANN201
     """Uses nmcli to activate connection
     conn: connection id(name) or uuid.
     """
     cmd = f'nmcli conn up "{conn}"'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to activate the connection: {conn}")
+        logging.error(f'Unable to activate the connection: {conn}')
         return False
     print(output)
     return True
 
 
 def nm_conn_down(conn):  # noqa: ANN001, ANN201
     """Uses nmcli to deactivate connection
     conn: connection id(name) or uuid.
     """
     cmd = f'nmcli conn down "{conn}"'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to deactivate the connection: {conn}")
+        logging.error(f'Unable to deactivate the connection: {conn}')
         return False
     print(output)
     return True
 
 
 def nm_conn_reload():  # noqa: ANN201
     """Runs `nmcli conn reload`. Does not support RHEL6."""
-    cmd = "nmcli conn reload"
-    retcode = run(cmd, verbose=False).returncode
+    cmd = 'nmcli conn reload'
+    retcode = run(cmd).rc
     if retcode != 0:
-        print("FAIL: Unable to reload NetworkManager")
+        logging.error('Unable to reload NetworkManager')
         return False
     return True
 
 
 def nm_conn_show(conn):  # noqa: ANN001, ANN201
     """Use nmcli conn to show all connection parameters. Does not support RHEL6
     conn: networkmanager connection id(name) or uuid.
     """
     if not conn:
-        print("FAIL: No conn specified")
+        logging.error('No conn specified')
         return False
 
     cmd = f'nmcli conn show "{conn}"'
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print("FAIL: Unable to show conn")
+        logging.error('Unable to show conn')
         return False
     print(output)
     return True
 
 
 def nm_conn_del(conn):  # noqa: ANN001, ANN201
     """Deletes NetworkManager connection using nmcli
     conn: connection id(name) or uuid.
     """
-    cmd = f"nmcli conn delete {conn}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'nmcli conn delete {conn}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to delete the conn {conn}")
+        logging.error(f'Unable to delete the conn {conn}')
         return False
     print(output)
     return True
 
 
-def nm_add_conn(name=None, nic_or_mac=None, nic_type="ethernet"):  # noqa: ANN001, ANN201
+def nm_add_conn(name=None, nic_or_mac=None, nic_type='ethernet'):  # noqa: ANN001, ANN201
     """Use it to add new connection for devices without one
     cmd="nmcli con add type ethernet ifname enp5s0f1 con-name enp5s0f1 ".
     """
     if is_mac(nic_or_mac):
         nic = get_nic_of_mac(nic_or_mac)
         if not nic:
-            print("FAIL: Couldn't find NIC from MAC.")
+            logging.error("Couldn't find NIC from MAC.")
             return False
     else:
         nic = nic_or_mac
 
     if not name:
         name = nic
 
     conn = None
     if nic:
         conn = nm_get_conn_from_dev(nic)
     # Exit if there is a connection already
     if conn:
-        print(f"Connection already exists. Linked to: {conn} ")
+        print(f'Connection already exists. Linked to: {conn} ')
         return True
 
-    cmd = f"nmcli conn add type {nic_type} con-name {name}"
+    cmd = f'nmcli conn add type {nic_type} con-name {name}'
     if nic:
-        cmd += f" ifname {nic}"
-    if "_" in cmd:
-        cmd = cmd.replace("_", "-")
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+        cmd += f' ifname {nic}'
+    if '_' in cmd:
+        cmd = cmd.replace('_', '-')
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to add con with cmd {cmd} ")
+        logging.error(f'Unable to add con with cmd {cmd} ')
         print(output)
         return False
     nm_conn_reload()
     return True
 
 
 def nm_conn_mod(conn, key, value):  # noqa: ANN001, ANN201
@@ -575,69 +549,69 @@
     connection.autoconnect yes   >> ONBOOT=yes
     connection.id eth0   >> NAME=eth0
     connection.interface-name eth0   >> DEVICE=eth0
     802-3-ethernet.mac-address 08:00:27:4b:7a:80 >> HWADDR=08:00:27:4b:7a:80
     ipv4.never-default no   >> DEFROUTE=yes.
     """
     if not conn:
-        print("FAIL: No connection specified")
+        logging.error('No connection specified')
         return False
     conn_uuid = nm_get_conn_uuid(conn)
     if not conn_uuid:
         return False
-    cmd = f"nmcli conn modify {conn_uuid}"
+    cmd = f'nmcli conn modify {conn_uuid}'
 
-    cmd += f" {key} {value}"
+    cmd += f' {key} {value}'
 
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to modify conn {conn} with cmd {cmd} ")
+        logging.error(f'Unable to modify conn {conn} with cmd {cmd} ')
         print(output)
         return False
     return True
 
 
 def nm_dev_mod(dev, key, value):  # noqa: ANN001, ANN201
     """Modify one or more properties that are currently active on the device without modifying
     the connection profile. The changes have immediate effect.
     nmcli dev modify em1 ipv4.method shared
     nmcli dev modify em1 ipv4.address xx.
     """
-    cmd = f"nmcli device modify {dev}"
-    cmd += f" {key} {value}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'nmcli device modify {dev}'
+    cmd += f' {key} {value}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to modify dev {dev} with cmd {cmd} ")
+        logging.error(f'Unable to modify dev {dev} with cmd {cmd} ')
         print(output)
         return False
     return True
 
 
-def nm_set_ip(conn, ip, netmask="24", activate=True):  # noqa: ANN001, ANN201
+def nm_set_ip(conn, ip, netmask='24', activate=True):  # noqa: ANN001, ANN201
     """Uses nmcli to set static IP, netmask and activates connection.
     conn: networkmanager connection id(name) or uuid
     ip: IPv4 or IPv6.
     """
     ip = str(ip)
     ipver = get_ip_version(ip)
 
     if ipver == 4:
-        cmd_ip = "ipv4"
+        cmd_ip = 'ipv4'
     elif ipver == 6:
-        cmd_ip = "ipv6"
+        cmd_ip = 'ipv6'
     else:
-        print("FAIL: Invalid IP format")
+        logging.error('Invalid IP format')
         return False
 
-    if "." in netmask:
+    if '.' in netmask:
         netmask = convert_netmask(netmask)
 
-    cmd = f"nmcli conn modify {conn} {cmd_ip}.method manual {cmd_ip}.addr {ip}/{netmask}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'nmcli conn modify {conn} {cmd_ip}.method manual {cmd_ip}.addr {ip}/{netmask}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: Unable to set IP using nmcli: {conn} {ip}")
+        logging.error(f'Unable to set IP using nmcli: {conn} {ip}')
         print(output)
         return False
 
     if activate and not nm_conn_up(conn):
         return False
     return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/scsi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 """scsi.py: Module to manipulate SCSI devices."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os.path
 import re
 from os import readlink
 from pathlib import Path
 
 from sts import linux, lvm, md, mp, net
 from sts.utils import size
 from sts.utils.cmdline import exists, run, run_ret_out
 
 # I'm still note sure whether to use /sys/class/scsi_disk or /sys/class/scsi_device
 
-sys_disk_path = "/sys/class/scsi_disk"
-host_path = "/sys/class/scsi_host"
+sys_disk_path = '/sys/class/scsi_disk'
+host_path = '/sys/class/scsi_host'
 
 # add /lib/udev to PATH because scsi_id is located there on RHEL7
-os.environ["PATH"] += ":/lib/udev"
+os.environ['PATH'] += ':/lib/udev'
 
 
 def get_regex_scsi_id():  # noqa: ANN201
-    return "([0-9]+):([0-9]+):([0-9]+):([0-9]+)"
+    return '([0-9]+):([0-9]+):([0-9]+):([0-9]+)'
 
 
 def is_scsi_device(scsi_device):  # noqa: ANN001, ANN201
-    return bool(re.match("^sd[a-z]+$", scsi_device))
+    return bool(re.match('^sd[a-z]+$', scsi_device))
 
 
 def get_scsi_disk_ids():  # noqa: ANN201
     """Return an array of scsi_ids. If an scsi_device name is given as
     parameter, then just the id of the device is returned (TODO)
     The arguments are:
     None
     Device name: eg. sda
     Returns:
     array: Return an array of SCSI IDs.
     """
-    cmd = f"ls {sys_disk_path}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'ls {sys_disk_path}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return output.split()
 
 
 def get_scsi_disk_name(device_id):  # noqa: ANN001, ANN201
     if not device_id:
-        print("FAIL: get_scsi_disk_name() requires scsi_device_id as parameter")
+        logging.error('get_scsi_disk_name() requires scsi_device_id as parameter')
         return None
 
-    cmd = f"ls {sys_disk_path}/{device_id}/device/block"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'ls {sys_disk_path}/{device_id}/device/block'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return output
 
 
 def get_scsi_disk_vendor(device_id):  # noqa: ANN001, ANN201
     if not device_id:
-        print("FAIL: get_scsi_disk_vendor() requires scsi_device_id as parameter")
+        logging.error('get_scsi_disk_vendor() requires scsi_device_id as parameter')
         return None
 
-    cmd = f"cat {sys_disk_path}/{device_id}/device/vendor"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'cat {sys_disk_path}/{device_id}/device/vendor'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return output
 
 
 def get_scsi_disk_model(device_id):  # noqa: ANN001, ANN201
     if not device_id:
-        print("FAIL: get_scsi_disk_model() requires scsi_device_id as parameter")
+        logging.error('get_scsi_disk_model() requires scsi_device_id as parameter')
         return None
 
-    cmd = f"cat {sys_disk_path}/{device_id}/device/model"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'cat {sys_disk_path}/{device_id}/device/model'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     return output
 
 
 def query_all_scsi_disks(scsi_disk=None):  # noqa: ANN001, ANN201
     """Query information of all SCSI disks and return them as a dict
@@ -96,15 +97,15 @@
     scsi_disks = {}
     for disk_id in disk_ids:
         scsi_name = get_scsi_disk_name(disk_id)
         if scsi_disk and scsi_name and scsi_disk != scsi_name:
             # optimization in case we requested specific disk, do not query all
             continue
         if not scsi_name:
-            print(f"WARN: Could not get scsi_name for disk_id '{disk_id}'.")
+            logging.warning(f"Could not get scsi_name for disk_id '{disk_id}'.")
             scsi_wwid = scsi_wwn = udev_wwn = size_bytes = state = timeout = None
         else:
             scsi_wwid = wwid_of_disk(scsi_name)
             scsi_wwn = wwn_of_disk(scsi_name)
             udev_wwn = udev_wwn_of_disk(scsi_name)
             size_bytes = size_of_disk(scsi_name)
             state = disk_sys_check(scsi_name)
@@ -114,33 +115,33 @@
         m = re.match(get_regex_scsi_id(), disk_id)
         host_id = None
         driver = None
         if m:
             host_id = m.group(1)
             driver = scsi_driver_of_host_id(host_id)
         scsi_info = {
-            "name": scsi_name,
-            "wwid": scsi_wwid,
-            "wwn": scsi_wwn,  # Uses scsi_id to query WWN
-            "udev_wwn": udev_wwn,  # Used udevadm to query WWN
-            "size": size_bytes,
-            "size_human": size.size_bytes_2_size_human(size_bytes),
-            "state": state,
-            "timeout": timeout,
-            "vendor": scsi_vendor,
-            "model": scsi_model,
-            "host_id": host_id,
-            "driver": driver,
-            "scsi_id": disk_id,
+            'name': scsi_name,
+            'wwid': scsi_wwid,
+            'wwn': scsi_wwn,  # Uses scsi_id to query WWN
+            'udev_wwn': udev_wwn,  # Used udevadm to query WWN
+            'size': size_bytes,
+            'size_human': size.size_bytes_2_size_human(size_bytes),
+            'state': state,
+            'timeout': timeout,
+            'vendor': scsi_vendor,
+            'model': scsi_model,
+            'host_id': host_id,
+            'driver': driver,
+            'scsi_id': disk_id,
         }
         scsi_disks[disk_id] = scsi_info
 
     if scsi_disk:
         for disk_id in list(scsi_disks.keys()):
-            if scsi_disk == scsi_disks[disk_id]["name"]:
+            if scsi_disk == scsi_disks[disk_id]['name']:
                 return scsi_disks[disk_id]
         return None
 
     return scsi_disks
 
 
 def get_scsi_name_by_vendor(vendor):  # noqa: ANN001, ANN201
@@ -148,65 +149,65 @@
     are from the requested vendor
     Parameter:
     vendor:        SCSI disk Vendor. eg: 'LIO'
     Return:
     List:          List of SCSI names.
     """
     if not vendor:
-        print("FAIL: get_scsi_name_by_vendor() - requires vendor parameter")
+        logging.error('get_scsi_name_by_vendor() - requires vendor parameter')
         return None
 
     all_scsi_disks_info = query_all_scsi_disks()
     if not all_scsi_disks_info:
         return None
 
     return [
-        scsi_info["name"]
+        scsi_info['name']
         for scsi_info in all_scsi_disks_info.values()
-        if "vendor" in scsi_info and scsi_info["vendor"] == vendor
+        if 'vendor' in scsi_info and scsi_info['vendor'] == vendor
     ]
 
 
 def scsi_host_of_scsi_name(scsi_name):  # noqa: ANN001, ANN201
     if not scsi_name:
-        print("FAIL: scsi_host_of_scsi_name() - requires scsi_name parameter")
+        logging.error('scsi_host_of_scsi_name() - requires scsi_name parameter')
         return None
 
     scsi_disk_info = query_all_scsi_disks(scsi_name)
     if not scsi_disk_info:
-        print(f"WARN: scsi_host_of_scsi_name() did not query info for {scsi_name}")
+        logging.warning(f'scsi_host_of_scsi_name() did not query info for {scsi_name}')
         return None
-    return scsi_disk_info["host_id"]
+    return scsi_disk_info['host_id']
 
 
 def scsi_name_2_scsi_id(scsi_name):  # noqa: ANN001, ANN201
     if not scsi_name:
-        print("FAIL: scsi_name_2_scsi_id() - requires scsi_name parameter")
+        logging.error('scsi_name_2_scsi_id() - requires scsi_name parameter')
         return None
 
     scsi_disk_info = query_all_scsi_disks(scsi_name)
     if not scsi_disk_info:
-        print(f"WARN: scsi_name_2_scsi_id() did not query info for {scsi_name}")
+        logging.warning(f'scsi_name_2_scsi_id() did not query info for {scsi_name}')
         return None
-    return scsi_disk_info["scsi_id"]
+    return scsi_disk_info['scsi_id']
 
 
 def delete_disk(device_name):  # noqa: ANN001, ANN201
     """device_name:    eg. sda."""
     if not device_name:
-        print("FAIL: delete_disk() requires scsi_device_name as parameter")
+        logging.error('delete_disk() requires scsi_device_name as parameter')
         return None
 
     device_id = scsi_name_2_scsi_id(device_name)
     if not device_id:
-        print(f"FAIL: delete_disk() could not find disk {device_name}")
+        logging.error(f'delete_disk() could not find disk {device_name}')
         return None
 
     cmd = f'echo "1" >  {sys_disk_path}/{device_id}/device/delete'
-    if run(cmd, verbose=False).returncode != 0:
+    if run(cmd).rc != 0:
         return None
     return True
 
 
 def get_hosts(somethings=None):  # noqa: ANN001, ANN201
     """Return a list with all SCSI hosts.
     The arguments are:
@@ -215,29 +216,29 @@
     scsi_disk     e.g. sda
     or
     scsi_id       e.g. 3:0:0:1
     Returns:
     Host list     if no problem executing command
     None          if something went wrong.
     """
-    cmd = f"ls {host_path}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'ls {host_path}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         return None
     # remove 'host' prefix
-    output = re.sub("host", "", output)
+    output = re.sub('host', '', output)
     all_host_ids = output.split()
     if not somethings:
         return all_host_ids
 
     scsi_host_ids = None
     # If something is a single string, convert it to list
     for something in somethings if not isinstance(somethings, str) else [somethings]:
         if something is None:
-            print("FAIL: get_hosts() - Invalid input")
+            logging.error('get_hosts() - Invalid input')
             print(somethings)
             return None
         m = re.match(get_regex_scsi_id(), something)
         if m and m.group(1) in all_host_ids:
             if not scsi_host_ids:
                 scsi_host_ids = []
             if m.group(1) not in scsi_host_ids:
@@ -270,111 +271,109 @@
         scsi_host_id           # like '0' for host0
     Returns
         scsi_host_info
             or
         None.
     """
     if not host_id:
-        print("FAIL: query_scsi_host_info() - requires host_id")
+        logging.error('query_scsi_host_info() - requires host_id')
         return None
 
-    sysfs_folder = Path(f"/sys/class/scsi_host/host{host_id}")
+    sysfs_folder = Path(f'/sys/class/scsi_host/host{host_id}')
     if not sysfs_folder.is_dir():
-        print(f"FAIL: {host_id} is not a valid directory")
+        logging.error(f'{host_id} is not a valid directory')
         return None
 
     scsi_host_info = {
-        "scsi_host_id": host_id,
-        "pci_id": pci_id_of_host_id(host_id),
-        "driver": scsi_driver_of_host_id(host_id),
+        'scsi_host_id': host_id,
+        'pci_id': pci_id_of_host_id(host_id),
+        'driver': scsi_driver_of_host_id(host_id),
     }
 
     param_files = list(sysfs_folder.iterdir())
     for param in param_files:
-        ret, output = run_ret_out(f"cat {sysfs_folder}/{param}", return_output=True, verbose=False)
+        ret, output = run_ret_out(f'cat {sysfs_folder}/{param}', return_output=True)
         if ret != 0:
             # For some reason could not read the file
             continue
-        scsi_host_info[param] = ", ".join(output.split("\n"))
+        scsi_host_info[param] = ', '.join(output.split('\n'))
 
     sysfs_hosts = [
-        f"/sys/class/iscsi_host/host{host_id}",
-        f"/sys/class/fc_host/host{host_id}",
+        f'/sys/class/iscsi_host/host{host_id}',
+        f'/sys/class/fc_host/host{host_id}',
     ]
     for sysfs_host in sysfs_hosts:
         path = Path(sysfs_host)
         if not path.is_dir():
             continue
         host_files = list(path.iterdir())
         for param in host_files:
-            ret, output = run_ret_out(f"cat {sysfs_host}/{param}", return_output=True, verbose=False)
+            ret, output = run_ret_out(f'cat {sysfs_host}/{param}', return_output=True)
             if ret != 0:
                 # For some reason could not read the file
                 continue
-            scsi_host_info[param] = ", ".join(output.split("\n"))
+            scsi_host_info[param] = ', '.join(output.split('\n'))
 
     return scsi_host_info
 
 
 def scsi_driver_of_host_id(host_id):  # noqa: ANN001, ANN201
     if not host_id:
-        print("FAIL: scsi_driver_of_host_id() - requires host_id parameter")
+        logging.error('scsi_driver_of_host_id() - requires host_id parameter')
         return None
-    scsi_drv_sysfs = f"/sys/class/scsi_host/host{host_id}/proc_name"
+    scsi_drv_sysfs = f'/sys/class/scsi_host/host{host_id}/proc_name'
     if not Path(scsi_drv_sysfs).is_file():
-        print(f"FAIL: {scsi_drv_sysfs} is not a valid path")
+        logging.error(f'{scsi_drv_sysfs} is not a valid path')
         return None
 
-    output = run(f"cat {scsi_drv_sysfs}", capture_output=True, verbose=False).output
+    output = run(f'cat {scsi_drv_sysfs}').stdout
     scsi_driver = output
-    if not scsi_driver or scsi_driver == "(null)":
+    if not scsi_driver or scsi_driver == '(null)':
         # Driver information was not exported, let try to find it out some other way
-        lpfc_sysfs_file = f"/sys/class/scsi_host/host{host_id}/lpfc_drvr_version"
+        lpfc_sysfs_file = f'/sys/class/scsi_host/host{host_id}/lpfc_drvr_version'
         if Path(lpfc_sysfs_file).is_file():
-            return "lpfc"
+            return 'lpfc'
 
-        driver_sysfs_file = f"/sys/class/scsi_host/host{host_id}/driver_name"
+        driver_sysfs_file = f'/sys/class/scsi_host/host{host_id}/driver_name'
         if Path(driver_sysfs_file).is_file():
-            return run(f"cat {driver_sysfs_file}", capture_output=True, verbose=False).output
+            return run(f'cat {driver_sysfs_file}').stdout
 
-        model_sysfs_file = f"/sys/class/scsi_host/host{host_id}/model_name"
+        model_sysfs_file = f'/sys/class/scsi_host/host{host_id}/model_name'
         if Path(model_sysfs_file).is_file():
-            output = run(f"cat {model_sysfs_file}", capture_output=True, verbose=False).output
-            if re.match("^QLE", output):
-                return "qla2xxx"
+            output = run(f'cat {model_sysfs_file}').stdout
+            if re.match('^QLE', output):
+                return 'qla2xxx'
 
-        symbolic_sysfs_file = f"/sys/class/fc_host/host{host_id}/symbolic_name"
+        symbolic_sysfs_file = f'/sys/class/fc_host/host{host_id}/symbolic_name'
         if Path(symbolic_sysfs_file).is_file():
-            output = run(f"cat {symbolic_sysfs_file}", capture_output=True, verbose=False).output
-            if re.search("bnx2fc", output):
-                return "bnx2fc"
+            output = run(f'cat {symbolic_sysfs_file}').stdout
+            if re.search('bnx2fc', output):
+                return 'bnx2fc'
 
         pci_id = pci_id_of_host_id(host_id)
         if pci_id:
-            lspci_regex = r"Kernel modules:\s+(\S+)"
-            if not exists("lspci"):
-                print("FAIL: pciutils is not installed. Can't query driver name using pci_id.")
+            lspci_regex = r'Kernel modules:\s+(\S+)'
+            if not exists('lspci'):
+                logging.error("pciutils is not installed. Can't query driver name using pci_id.")
                 return None
             output = run(
                 f'lspci -s "{pci_id}" -v | grep "Kernel modules:"',
-                capture_output=True,
-                verbose=False,
-            ).output
+            ).stdout
             if output:
                 m = re.search(lspci_regex, output)
                 if m:
                     return m.group(1)
 
-        print(f"FAIL: Could not get driver name for SCSI host{host_id}")
+        logging.error(f'Could not get driver name for SCSI host{host_id}')
         return None
-    if scsi_driver == "fcoe":
-        drv_version_path = f"/sys/class/fc_host/host{host_id}/driver_version"
-        output = run(f"cat {drv_version_path}", capture_output=True, verbose=False).output
-        if re.search("ixgbe", output):
-            return "ixgbe"
+    if scsi_driver == 'fcoe':
+        drv_version_path = f'/sys/class/fc_host/host{host_id}/driver_version'
+        output = run(f'cat {drv_version_path}').stdout
+        if re.search('ixgbe', output):
+            return 'ixgbe'
     return scsi_driver
 
 
 def pci_id_of_host_id(host_id):  # noqa: ANN001, ANN201
     """Usage
         pci_id_of(scsi_host_id);
     Purpose
@@ -382,63 +381,62 @@
             readlink("/sys/class/scsi_host/host'scsi_host_id'");
     Parameter
         $scsi_host_id           # like '0' for host0
     Returns
         pci_id                 # like '0000:00:1c.0'.
     """
     if not host_id:
-        print("FAIL: pci_id_of_host_id() - requires host_id parameter")
+        logging.error('pci_id_of_host_id() - requires host_id parameter')
         return None
-    sys_path = f"/sys/class/scsi_host/host{host_id}"
+    sys_path = f'/sys/class/scsi_host/host{host_id}'
     if not Path(sys_path).exists():
-        print(f"FAIL: {sys_path} is not a valid path")
+        logging.error(f'{sys_path} is not a valid path')
         return None
 
     link_path = readlink(sys_path)
 
     regex_pci_id = linux.get_regex_pci_id()
-    m = re.search(f"({regex_pci_id})/host{host_id}/scsi_host", link_path)
+    m = re.search(f'({regex_pci_id})/host{host_id}/scsi_host', link_path)
     # print("DEBUG: pci_id_of_host_id - %s" % link_path)
     if m:
         return m.group(1)
 
     # for example ixgbe need to check the PCI id from the network device
     # check for network interface name
-    net_regex = re.compile(r"devices/virtual/net/(.*)\.")
+    net_regex = re.compile(r'devices/virtual/net/(.*)\.')
     m = net_regex.search(link_path)
     if m:
         return net.get_pci_id_of_nic(m.group(1))
 
     return None
 
 
-def rescan_host(host=None, verbose=True):  # noqa: ANN001, ANN201
+def rescan_host(host=None):  # noqa: ANN001, ANN201
     """Rescan for devices for specific host
     If no host is given it will scan all SCSI hosts
     The arguments are:
     Host:      e.g. 1 for host1
     Returns:
     True if no problem executing command
     False if something went wrong.
     """
     host_list = [host] if host else list(get_hosts())
 
     error = 0
 
     if not host_list:
-        print("WARN: No host found on server to rescan")
+        logging.warning('No host found on server to rescan')
         return True
 
     for host in host_list:
-        if verbose:
-            print(f"INFO: Rescanning host{host}")
+        logging.info(f'Rescanning host{host}')
         cmd = f'echo "- - -" > {host_path}/host{host}/scan'
-        if run(cmd, verbose=verbose).returncode != 0:
+        if run(cmd).rc != 0:
             error += 1
-            print(f"FAIL: there was some problem scanning host{host}")
+            logging.error(f'there was some problem scanning host{host}')
 
     if error:
         return False
 
     return True
 
 
@@ -451,17 +449,17 @@
     True if no problem executing command
     False if something went wrong.
     """
     scsi_disks = [scsi_disk] if scsi_disk else [get_scsi_disk_name(_id) for _id in get_scsi_disk_ids()]
 
     error = 0
     for scsi_disk in scsi_disks:
-        cmd = f"echo 1 > /sys/block/{scsi_disk}/device/rescan"
-        if run(cmd).returncode != 0:
-            print(f"FAIL: Could not rescan {scsi_disk}")
+        cmd = f'echo 1 > /sys/block/{scsi_disk}/device/rescan'
+        if run(cmd).rc != 0:
+            logging.error(f'Could not rescan {scsi_disk}')
             error += 1
 
     if error:
         return False
 
     return True
 
@@ -476,28 +474,28 @@
     Returns
         size in bytes.
 
     """
     if not scsi_disk:
         return None
 
-    cmd = f"cat /sys/block/{scsi_disk}/queue/logical_block_size"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'cat /sys/block/{scsi_disk}/queue/logical_block_size'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: size_of_disk() - Could not get size for disk {scsi_disk}")
+        logging.error(f'size_of_disk() - Could not get size for disk {scsi_disk}')
         print(output)
         return None
     if not output:
         return None
     logical_block_size = output
 
-    cmd = f"cat /sys/block/{scsi_disk}/size"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'cat /sys/block/{scsi_disk}/size'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: size_of_disk() - Could not get sectore size for disk {scsi_disk}")
+        logging.error(f'size_of_disk() - Could not get sectore size for disk {scsi_disk}')
         print(output)
         return None
     if not output:
         return None
 
     sector_size = output
 
@@ -511,44 +509,44 @@
         Given a scsi_disk name. E.g. sda, mpatha
     Parameter
         scsi_disk   device to get wwid for
     Returns
         wwid:       e.g. 360fff19abdd9f5fb943525d45126ca27.
     """
     if not scsi_disk:
-        print("FAIL: wwid_of_disk() - requires scsi_disk parameter")
+        logging.error('wwid_of_disk() - requires scsi_disk parameter')
         return None
 
     if linux.is_dm_device(scsi_disk):
-        return linux.get_udev_property(scsi_disk, "DM_SERIAL")
+        return linux.get_udev_property(scsi_disk, 'DM_SERIAL')
 
-    return linux.get_udev_property(scsi_disk, "ID_SERIAL")
+    return linux.get_udev_property(scsi_disk, 'ID_SERIAL')
 
 
 def scsi_ids_of_wwid(wwid):  # noqa: ANN001, ANN201
     """Usage
         scsi_ids_of_wwid(wwid)
     Purpose
         Find out all SCSI id for WWID.
     Parameter
         wwid
     Returns
         scsi_ids.
     """
     if not wwid:
-        print("FAIL: scsi_ids_of_wwid(): Got NULL input for WWID")
+        logging.error('scsi_ids_of_wwid(): Got NULL input for WWID')
         return None
 
     scsi_ids = []
     all_scsi_info = query_all_scsi_disks()
     if not all_scsi_info:
         # Could not find any SCSI device
         return None
 
-    scsi_ids = [_id for _id in all_scsi_info if all_scsi_info[_id]["wwid"] == wwid]
+    scsi_ids = [_id for _id in all_scsi_info if all_scsi_info[_id]['wwid'] == wwid]
 
     if scsi_ids:
         scsi_ids = list(set(scsi_ids))  # dedup
     return scsi_ids
 
 
 def wwn_of_disk(scsi_disk):  # noqa: ANN001, ANN201
@@ -558,53 +556,53 @@
         Given an scsi_disk name. Eg. sda
     Parameter
         scsi_disk
     Returns
         wwid:       eg. 0x60a980003246694a412b45673342616e.
     """
     if not scsi_disk:
-        print("FAIL: wwn_of_disk() - requires scsi_disk parameter")
+        logging.error('wwn_of_disk() - requires scsi_disk parameter')
         return None
 
-    key_regex = "ID_WWN_WITH_EXTENSION=(.*)"
+    key_regex = 'ID_WWN_WITH_EXTENSION=(.*)'
 
     # cmd = "udevadm info --name=%s --query=all" % scsi_disk
-    # retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    # retcode, output = run_ret_out(cmd, return_output=True)
     # if (retcode != 0):
-    # #print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
+    # #logging.error("wwn_of_disk() - Could not query %s" % scsi_disk)
     # #print output
 
     # return None
 
     # udev_wwn = None
     # lines = output.split("\n")
     # for line in lines:
     # m = re.search(key_regex, line)
     # if m:
     # udev_wwn = m.group(1)
 
-    cmd = f"scsi_id --whitelisted --export /dev/{scsi_disk}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'scsi_id --whitelisted --export /dev/{scsi_disk}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        # print("FAIL: wwn_of_disk() - Could not query %s" % scsi_disk)
+        # logging.error("wwn_of_disk() - Could not query %s" % scsi_disk)
         # print output
         return None
 
-    lines = output.split("\n")
+    lines = output.split('\n')
     for line in lines:
         m = re.search(key_regex, line)
         if m:
             return m.group(1)
 
     # if udev_wwn and scsi_wwn:
     # if udev_wwn == scsi_wwn:
     # return udev_wwn
     # print("udevadm WWN is %s" % udev_wwn)
     # print("scsi_id WWN is %s" % scsi_wwn)
-    # print("FAIL: wwn_of_disk() - udevadm WWN and scsi_id WWN for %s do not match" % scsi_disk)
+    # logging.error("wwn_of_disk() - udevadm WWN and scsi_id WWN for %s do not match" % scsi_disk)
     # return None
 
     return None
 
 
 def udev_wwn_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
@@ -613,56 +611,56 @@
         Given an scsi_disk name. Eg. sda
     Parameter
         scsi_disk
     Returns
         wwid:       eg. 0x60a980003246694a412b45673342616e.
     """
     if not scsi_disk:
-        print("FAIL: udev_wwn_of_disk() - requires scsi_disk parameter")
+        logging.error('udev_wwn_of_disk() - requires scsi_disk parameter')
         return None
 
-    key_regex = "ID_WWN_WITH_EXTENSION=(.*)"
+    key_regex = 'ID_WWN_WITH_EXTENSION=(.*)'
 
-    cmd = f"udevadm info --name={scsi_disk} --query=all"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'udevadm info --name={scsi_disk} --query=all'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        # print("FAIL: udev_wwn_of_disk() - Could not query %s" % scsi_disk)
+        # logging.error("udev_wwn_of_disk() - Could not query %s" % scsi_disk)
         # print output
         return None
 
-    lines = output.split("\n")
+    lines = output.split('\n')
     for line in lines:
         m = re.search(key_regex, line)
         if m:
             return m.group(1)
     return None
 
 
 def query_scsi_driver_info(driver):  # noqa: ANN001, ANN201
     if not driver:
-        print("FAIL: query_scsi_driver_info() - requires driver parameter")
+        logging.error('query_scsi_driver_info() - requires driver parameter')
         return None
 
     all_scsi_host_ids = get_hosts()
     if not all_scsi_host_ids:
-        print("FAIL: query_scsi_driver_info() - Host does not have any SCSI host")
+        logging.error('query_scsi_driver_info() - Host does not have any SCSI host')
         return None
 
     # Check which SCSI hosts are using the driver we want
     driver_host_ids = [host_id for host_id in all_scsi_host_ids if scsi_driver_of_host_id(host_id) == driver]
 
     if not driver_host_ids:
-        print(f"FAIL:  No SCSI disk found from driver {driver}")
+        logging.error(f' No SCSI disk found from driver {driver}')
         return None
 
-    scsi_driver_info = {"scsi_host": {}}
+    scsi_driver_info = {'scsi_host': {}}
     for host_id in driver_host_ids:
-        scsi_driver_info["scsi_host"][host_id] = query_scsi_host_info(host_id)
+        scsi_driver_info['scsi_host'][host_id] = query_scsi_host_info(host_id)
 
-    scsi_driver_info["driver_name"] = driver
+    scsi_driver_info['driver_name'] = driver
     # Add general driver info to this dict
     scsi_driver_info.update(linux.get_driver_info(driver))
 
     return scsi_driver_info
 
 
 def get_free_disks(  # noqa: ANN201
@@ -689,88 +687,88 @@
     # the mpath device should be skipped as well
     if boot_dev:
         boot_wwid = linux.get_device_wwid(boot_dev)
 
     all_mp_info = None
     if (mp.is_multipathd_running()) and exclude_mpath_device:
         all_mp_info = mp.multipath_query_all()
-        if all_mp_info and "by_wwid" not in list(all_mp_info.keys()):
+        if all_mp_info and 'by_wwid' not in list(all_mp_info.keys()):
             # Fail querying mpath, setting it back to None
             all_mp_info = None
 
     chosen_disks = {}
     for scsi_disk in list(all_scsi_disks.keys()):
         scsi_info = all_scsi_disks[scsi_disk]
         # Skip if mpath device is used for boot
-        if boot_wwid == scsi_info["wwid"] and exclude_boot_device:
+        if boot_wwid == scsi_info['wwid'] and exclude_boot_device:
             print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for boot")
             continue
 
         # Skip if disk is used by multipath
-        if all_mp_info and scsi_info["wwid"] in list(all_mp_info["by_wwid"].keys()) and exclude_mpath_device:
+        if all_mp_info and scsi_info['wwid'] in list(all_mp_info['by_wwid'].keys()) and exclude_mpath_device:
             print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for mpath")
             continue
 
         # Skip if it is used by Soft RAID
         if md_devices and exclude_md_device:
             used_by_md = False
             for md_dev in md_devices:
                 storage_devs = md.md_get_storage_dev(md_dev)
                 if not storage_devs:
                     continue
                 for dev in storage_devs:
                     dev_wwid = wwid_of_disk(dev)
                     if not dev_wwid:
                         continue
-                    if dev_wwid == scsi_info["wwid"]:
+                    if dev_wwid == scsi_info['wwid']:
                         print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for md")
                         used_by_md = True
                         continue
             if used_by_md:
                 continue
 
         # Skip if filter_only is specified
         filtered = False
         if filter_only is not None:
             for key in filter_only:
                 if scsi_info[key] != filter_only[key]:
                     print(
-                        "DEBUG: get_free_disks() - filtered {} as {} is not {}".format(
-                            scsi_info["name"],
+                        'DEBUG: get_free_disks() - filtered {} as {} is not {}'.format(
+                            scsi_info['name'],
                             key,
                             filter_only[key],
                         ),
                     )
                     filtered = True
                     continue
         if filtered:
             continue
 
-        chosen_disks[scsi_info["name"]] = scsi_info
+        chosen_disks[scsi_info['name']] = scsi_info
 
         # Skip if it is used by LVM
         if pvs and exclude_lvm_device:
             for pv in list(pvs.keys()):
-                if "/" + get_scsi_disk_name(scsi_disk) in pv:
+                if '/' + get_scsi_disk_name(scsi_disk) in pv:
                     print(f"DEBUG: get_free_disks() - skip {scsi_info['name']} as it is used for LVM")
-                    chosen_disks.pop(scsi_info["name"])
+                    chosen_disks.pop(scsi_info['name'])
 
     return chosen_disks
 
 
 def scsi_device_2_scsi_name(scsi_device):  # noqa: ANN001, ANN201
     """Convert an specific SCSI device to scsi_name
     Eg. /dev/sdap1 => sda.
     """
-    scsi_dev_regex = r"/dev\/(sd.*)"
+    scsi_dev_regex = r'/dev\/(sd.*)'
     m = re.match(scsi_dev_regex, scsi_device)
     if m:
         # remove partition if it has
         device_name = m.group(1)
-        m = re.match(r"(.*)\d+", device_name)
+        m = re.match(r'(.*)\d+', device_name)
         if m:
             device_name = m.group(1)
         return device_name
     # does not seem to be a valid SCSI device
     return None
 
 
@@ -787,42 +785,42 @@
         action         # 'UP|DOWN|other'
     Returns
         True               # got expected /sys/block/sdX/device/state
             or
         False.
     """
     if not scsi_disk or not action:
-        print("FAIL: disk_sys_trigger() - requires scsi_disk and action parameters")
+        logging.error('disk_sys_trigger() - requires scsi_disk and action parameters')
         return False
 
-    sys_path = f"/sys/block/{scsi_disk}/device/state"
+    sys_path = f'/sys/block/{scsi_disk}/device/state'
     if not Path(sys_path).is_file():
-        print(f"FAIL: No such file: {sys_path}")
+        logging.error(f'No such file: {sys_path}')
         return False
 
-    if action == "UP":
-        action = "running"
-    if action == "DOWN":
-        action = "offline"
+    if action == 'UP':
+        action = 'running'
+    if action == 'DOWN':
+        action = 'offline'
 
-    cmd = f"echo {action} > {sys_path}"
-    retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'echo {action} > {sys_path}'
+    retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
-        print(f"FAIL: disk_sys_trigger() - Could not execute {cmd}")
+        logging.error(f'disk_sys_trigger() - Could not execute {cmd}')
         print(output)
         return None
 
     # cmd = "cat %s 2>/dev/null" % sys_path
     new_state = disk_sys_check(scsi_disk)
     if not new_state:
-        print(f"FAIL: disk_sys_trigger() - Could not get state of {scsi_disk}")
+        logging.error(f'disk_sys_trigger() - Could not get state of {scsi_disk}')
         return False
 
     if action != new_state:
-        print(f"FAIL: disk_sys_trigger() - Current state is '{new_state}' expected '{action}'")
+        logging.error(f"disk_sys_trigger() - Current state is '{new_state}' expected '{action}'")
         return False
 
     return True
 
 
 def disk_sys_check(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
@@ -834,26 +832,26 @@
         scsi_disk      # like 'sda'
     Returns
         running/offline       # got expected /sys/block/sdX/device/state
             or
         None.
     """
     if not scsi_disk:
-        print("FAIL: disk_sys_check() - requires scsi_disk parameter")
+        logging.error('disk_sys_check() - requires scsi_disk parameter')
         return None
 
-    sys_path = f"/sys/block/{scsi_disk}/device/state"
+    sys_path = f'/sys/block/{scsi_disk}/device/state'
     if not Path(sys_path).is_file():
-        print(f"FAIL: disk_sys_check() - No such file: {sys_path}")
+        logging.error(f'disk_sys_check() - No such file: {sys_path}')
         return None
 
-    cmd = f"cat {sys_path} 2>/dev/null"
-    state = run(cmd, capture_output=True, verbose=False).output
+    cmd = f'cat {sys_path} 2>/dev/null'
+    state = run(cmd).stdout
     if not state:
-        print(f"FAIL: disk_sys_check() - Could not read from {sys_path}")
+        logging.error(f'disk_sys_check() - Could not read from {sys_path}')
         return None
 
     return state
 
 
 def timeout_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
@@ -865,22 +863,22 @@
         scsi_disk      # like 'sda'
     Returns
         timeout in seconds       # got expected /sys/block/sdX/device/timeout
             or
         None.
     """
     if not scsi_disk:
-        print("FAIL: timeout_of_disk() - requires scsi_disk parameter")
+        logging.error('timeout_of_disk() - requires scsi_disk parameter')
         return None
 
-    sys_path = f"/sys/block/{scsi_disk}/device/timeout"
+    sys_path = f'/sys/block/{scsi_disk}/device/timeout'
     if not Path(sys_path).is_file():
-        print(f"FAIL: timeout_of_disk() - No such file: {sys_path}")
+        logging.error(f'timeout_of_disk() - No such file: {sys_path}')
         return None
 
-    cmd = f"cat {sys_path} 2>/dev/null"
-    timeout = run(cmd, capture_output=True, verbose=False).output
+    cmd = f'cat {sys_path} 2>/dev/null'
+    timeout = run(cmd).stdout
     if not timeout:
-        print(f"FAIL: timeout_of_disk() - Could not read from {sys_path}")
+        logging.error(f'timeout_of_disk() - Could not read from {sys_path}')
         return None
 
     return timeout
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/scsi_debug.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 """scsi_debug.py: Module to manipulate devices created by scsi_debug module."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
+
 from sts import linux, mp
 from sts.scsi import get_scsi_name_by_vendor
 from sts.utils.cmdline import run
 
 
 def scsi_debug_load_module(options=None):  # noqa: ANN001, ANN201
-    module_cmd = "scsi_debug"
+    module_cmd = 'scsi_debug'
     if linux.is_module_loaded(module_cmd):
-        print("WARN: scsi_debug_load_module() - Module is already loaded")
+        logging.warning('scsi_debug_load_module() - Module is already loaded')
         return True
 
     if options:
-        module_cmd += f" {options}"
+        module_cmd += f' {options}'
 
     if not linux.load_module(module_cmd):
-        print(f"FAIL: scsi_debug_load_module() - Could not load {module_cmd}")
+        logging.error(f'scsi_debug_load_module() - Could not load {module_cmd}')
         return False
     # Wait a bit, for example for multipath to create the device
     linux.sleep(2)
     return True
 
 
 def scsi_debug_unload_module():  # noqa: ANN201
-    module_name = "scsi_debug"
+    module_name = 'scsi_debug'
     if not linux.is_module_loaded(module_name):
         # Module is not loaded, return success
         return True
 
     if mp.is_multipathd_running():
-        mpaths = mp.mpath_names_of_vendor("Linux")
+        mpaths = mp.mpath_names_of_vendor('Linux')
         for mpath in mpaths:
             mp.remove_mpath(mpath)
             # Wait a bit, for example for multipath to remove the device
             linux.sleep(2)
 
     if not linux.unload_module(module_name):
-        print(f"FAIL: scsi_debug_load_module() - Could not unload {module_name}")
+        logging.error(f'scsi_debug_load_module() - Could not unload {module_name}')
         return False
     return True
 
 
 def get_scsi_debug_devices():  # noqa: ANN201
     """Return a list of scsi_debug devices."""
-    module_name = "scsi_debug"
-    vendor = "Linux"
+    module_name = 'scsi_debug'
+    vendor = 'Linux'
     if not linux.is_module_loaded(module_name):
         return None
 
     mpaths = mp.mpath_names_of_vendor(vendor)
     if mpaths:
         return mpaths
 
@@ -61,25 +63,24 @@
 
     return None
 
 
 def scsi_debug_set_param(param, value):  # noqa: ANN001, ANN201
     """Set specific value to scsi debug parameter."""
     if param is None or value is None:
-        print("FAIL: scsi_debug_set_param() - requires param_name and value")
+        logging.error('scsi_debug_set_param() - requires param_name and value')
         return False
 
     if (
         run(
             f"echo '{value}' > /sys/bus/pseudo/drivers/scsi_debug/{param}",
-            verbose=False,
         )
         != 0
     ):
-        print(f"FAIL: scsi_debug_set_param() - Could not set {param} with value {value}")
+        logging.error(f'scsi_debug_set_param() - Could not set {param} with value {value}')
         return False
     return True
 
 
 def scsi_debug_insert_failure(every_nth, opts):  # noqa: ANN001, ANN201
     """Purpose:
     Enable/Disable failure on scsi_debug device
@@ -97,36 +98,36 @@
     False: if some problem occurred.
     """
     if not every_nth:
         every_nth = 0
     if not opts:
         opts = 0
 
-    if not scsi_debug_set_param("every_nth", every_nth):
-        print(f"FAIL: scsi_debug_insert_failure() - Could not set every_nth with value: {every_nth}")
+    if not scsi_debug_set_param('every_nth', every_nth):
+        logging.error(f'scsi_debug_insert_failure() - Could not set every_nth with value: {every_nth}')
         return False
-    if not scsi_debug_set_param("opts", opts):
-        print(f"FAIL: scsi_debug_insert_failure() - Could not set opts with value: {opts}")
+    if not scsi_debug_set_param('opts', opts):
+        logging.error(f'scsi_debug_insert_failure() - Could not set opts with value: {opts}')
         return False
     return True
 
 
 def self_test():  # noqa: ANN201
     if not scsi_debug_load_module():
-        print("FAIL: self_test() - Could not load the module")
+        logging.error('self_test() - Could not load the module')
         return False
 
     if not get_scsi_debug_devices():
-        print("FAIL: self_test() - Could not find any scsi debug device")
+        logging.error('self_test() - Could not find any scsi debug device')
         scsi_debug_unload_module()
         return False
 
     if not scsi_debug_insert_failure(0, 0):
-        print("FAIL: self_test() - Could not set parameters")
+        logging.error('self_test() - Could not set parameters')
         scsi_debug_unload_module()
         return False
 
     if not scsi_debug_unload_module():
-        print("FAIL: self_test() - Could not unload the module")
+        logging.error('self_test() - Could not unload the module')
         return False
 
     return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/stratis.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/stratis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,113 @@
 """stratis.py: Module with test specific method for Stratis."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import json
+import logging
 from typing import Dict, List
 
 from sts import linux
 from sts.utils.cli_tools import Wrapper
 from sts.utils.cmdline import run
 
 
 def get_stratis_service() -> str:
     """Return name of the stratis service.
 
     Returns:
       str: Name of the stratis service.
     """
-    return "stratisd"
+    return 'stratisd'
 
 
 class Stratis(Wrapper):
     """Wrapper class for stratis command line interface."""
 
     def __init__(self, disable_check=True) -> None:  # noqa: ANN001
-        self.stratis_version = ""
+        self.stratis_version = ''
         self.disable_check = disable_check
         if linux.dist_ver() < 8:
-            print("FATAL: Stratis is not supported on RHEL < 8.")
+            logging.critical('Stratis is not supported on RHEL < 8.')
 
-        for pkg in ["stratisd", "stratis-cli"]:
+        for pkg in ['stratisd', 'stratis-cli']:
             if not linux.is_installed(pkg) and not linux.install_package(pkg, check=False):
-                print(f"FATAL: Could not install {pkg} package")
+                logging.critical(f'Could not install {pkg} package')
 
         self.commands: Dict[str, List[str]] = {}
-        self.commands["all"] = list(self.commands.keys())
+        self.commands['all'] = list(self.commands.keys())
         self.arguments = {
-            "force": [self.commands["all"], " --force"],
-            "redundancy": [self.commands["all"], " --redundancy"],
-            "propagate": [self.commands["all"], "--propagate "],
+            'force': [self.commands['all'], ' --force'],
+            'redundancy': [self.commands['all'], ' --redundancy'],
+            'propagate': [self.commands['all'], '--propagate '],
         }
 
-        if linux.service_status(get_stratis_service(), verbose=False) != 0:
+        if linux.service_status(get_stratis_service()) != 0:
             if not linux.service_restart(get_stratis_service()):
-                print(f"FAIL: Could not start {get_stratis_service()} service")
+                logging.error(f'Could not start {get_stratis_service()} service')
             else:
-                print(f"INFO: Service {get_stratis_service()} restarted.")
+                logging.info(f'Service {get_stratis_service()} restarted.')
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
     def _remove_nones(kwargs):  # noqa: ANN001, ANN205
         return {k: v for k, v in kwargs.items() if v is not None}
 
-    def _run(self, cmd, verbosity=True, **kwargs):  # noqa: ANN001, ANN003, ANN202
+    def _run(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
 
         # add '--propagate' flag by default to show whole trace when getting errors
         # This is a suggestion from devs
-        if not ("propagate" in kwargs and not kwargs["propagate"]):
-            cmd = self.arguments["propagate"][1] + cmd
+        if not ('propagate' in kwargs and not kwargs['propagate']):
+            cmd = self.arguments['propagate'][1] + cmd
 
-        cmd = "stratis " + cmd
+        cmd = 'stratis ' + cmd
         cmd = self._add_arguments(cmd, **kwargs)
 
-        ret = run(cmd, verbose=verbosity).returncode
+        ret = run(cmd).rc
         if isinstance(ret, tuple) and ret[0] != 0:
-            print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+            logging.warning(f"Running command: '{cmd}' failed. Return with output.")
         elif isinstance(ret, int) and ret != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+            logging.warning(f"Running command: '{cmd}' failed.")
         return ret
 
     def set_stratis_version(self, version):  # noqa: ANN001, ANN201
         self.stratis_version = version
 
     def get_stratis_version(self):  # noqa: ANN201
         if not self.stratis_version:
-            ret, data = self._run(cmd="--version", return_output=True)
+            ret, data = self._run(cmd='--version', return_output=True)
             if ret == 0:
                 self.set_stratis_version(data)
                 return data
-            print("FAIL: Could not get stratis version!")
-            return "0.0.0"
+            logging.error('Could not get stratis version!')
+            return '0.0.0'
         return self.stratis_version
 
     def get_stratis_major_version(self):  # noqa: ANN201
-        return int(self.get_stratis_version().split(".")[0])
+        return int(self.get_stratis_version().split('.')[0])
 
     def get_stratis_minor_version(self):  # noqa: ANN201
-        return int(self.get_stratis_version().split(".")[1])
+        return int(self.get_stratis_version().split('.')[1])
 
     def get_pool_uuid(self, pool_name):  # noqa: ANN001, ANN201
-        ret, data = self._run(cmd="report", return_output=True)
+        ret, data = self._run(cmd='report', return_output=True)
         if ret == 0 and data:
             try:
                 report = json.loads(data)
             except json.JSONDecodeError:
-                print("FAIL: Could not deserialize data returned from 'stratis report' command!")
+                logging.exception("Could not deserialize data returned from 'stratis report' command!")
                 return None
-            for pool in report["pools"]:
-                if pool_name == pool["name"]:
-                    print(f"INFO: Found UUID: {pool['uuid']} for pool_name: {pool_name}.")
-                    return pool["uuid"]
-            print(f"FAIL: Could not find pool UUID for provided pool_name: {pool_name}!")
+            for pool in report['pools']:
+                if pool_name == pool['name']:
+                    logging.info(f"Found UUID: {pool['uuid']} for pool_name: {pool_name}.")
+                    return pool['uuid']
+            logging.error(f'Could not find pool UUID for provided pool_name: {pool_name}!')
             return None
         return None
 
     def pool_create(  # noqa: ANN201
         self,
         pool_name=None,  # noqa: ANN001
         blockdevs=None,  # noqa: ANN001
@@ -116,361 +117,361 @@
         tang_url=None,  # noqa: ANN001
         thumbprint=None,  # noqa: ANN001
         clevis=None,  # noqa: ANN001
         trust_url=None,  # noqa: ANN001
         no_overprovision=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "pool create "
+        cmd = 'pool create '
         if key_desc:
-            cmd += f"--key-desc {key_desc} "
+            cmd += f'--key-desc {key_desc} '
         if clevis:
-            cmd += f"--clevis {clevis} "
+            cmd += f'--clevis {clevis} '
         if tang_url:
-            cmd += f"--tang-url {tang_url} "
+            cmd += f'--tang-url {tang_url} '
         if thumbprint:
-            cmd += f"--thumbprint {thumbprint} "
+            cmd += f'--thumbprint {thumbprint} '
         if trust_url:
-            cmd += "--trust-url "
+            cmd += '--trust-url '
         if no_overprovision:
-            cmd += "--no-overprovision "
+            cmd += '--no-overprovision '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if blockdevs:
             if not isinstance(blockdevs, list):
                 blockdevs = [blockdevs]
-            cmd += " ".join(blockdevs)
+            cmd += ' '.join(blockdevs)
         kwargs.update(
             {
-                "force": force,
-                "redundancy": redundancy,
+                'force': force,
+                'redundancy': redundancy,
             },
         )
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_list(self, pool_uuid=None, stopped_pools=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool list "
+        cmd = 'pool list '
         if pool_uuid:
-            cmd += f"--uuid {pool_uuid} "
+            cmd += f'--uuid {pool_uuid} '
         if stopped_pools:
-            cmd += "--stopped "
+            cmd += '--stopped '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_destroy(self, pool_name=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool destroy "
+        cmd = 'pool destroy '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_rename(self, current=None, new=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool rename "
+        cmd = 'pool rename '
         if current:
-            cmd += f"{current} "
+            cmd += f'{current} '
         if new:
-            cmd += f"{new} "
+            cmd += f'{new} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_add_data(self, pool_name=None, blockdevs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool add-data "
+        cmd = 'pool add-data '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if blockdevs:
             if not isinstance(blockdevs, list):
                 blockdevs = [blockdevs]
-            cmd += " ".join(blockdevs)
+            cmd += ' '.join(blockdevs)
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_add_cache(self, pool_name=None, blockdevs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool add-cache "
+        cmd = 'pool add-cache '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if blockdevs:
             if not isinstance(blockdevs, list):
                 blockdevs = [blockdevs]
-            cmd += " ".join(blockdevs)
+            cmd += ' '.join(blockdevs)
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_init_cache(self, pool_name=None, blockdevs=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool init-cache "
+        cmd = 'pool init-cache '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if blockdevs:
             if not isinstance(blockdevs, list):
                 blockdevs = [blockdevs]
-            cmd += " ".join(blockdevs)
+            cmd += ' '.join(blockdevs)
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_bind(  # noqa: ANN201
         self,
         binding_method=None,  # noqa: ANN001
         pool_name=None,  # noqa: ANN001
         key_desc=None,  # noqa: ANN001
         trust_url=None,  # noqa: ANN001
         thumbprint=None,  # noqa: ANN001
         tang_url=None,  # noqa: ANN001
         force=None,  # noqa: ANN001
         redundancy=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "pool bind "
+        cmd = 'pool bind '
         if binding_method:
-            cmd += f"{binding_method} "
+            cmd += f'{binding_method} '
         if trust_url:
-            cmd += "--trust-url "
+            cmd += '--trust-url '
         if thumbprint:
-            cmd += f"--thumbprint {thumbprint} "
+            cmd += f'--thumbprint {thumbprint} '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if key_desc:
-            cmd += f"{key_desc} "
+            cmd += f'{key_desc} '
         if tang_url:
-            cmd += f"{tang_url} "
+            cmd += f'{tang_url} '
         kwargs.update(
             {
-                "force": force,
-                "redundancy": redundancy,
+                'force': force,
+                'redundancy': redundancy,
             },
         )
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_rebind(  # noqa: ANN201
         self,
         binding_method=None,  # noqa: ANN001
         pool_name=None,  # noqa: ANN001
         key_desc=None,  # noqa: ANN001
         force=None,  # noqa: ANN001
         redundancy=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "pool rebind "
+        cmd = 'pool rebind '
         if binding_method:
-            cmd += f"{binding_method} "
+            cmd += f'{binding_method} '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if key_desc:
-            cmd += f"{key_desc} "
+            cmd += f'{key_desc} '
         kwargs.update(
             {
-                "force": force,
-                "redundancy": redundancy,
+                'force': force,
+                'redundancy': redundancy,
             },
         )
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_unbind(  # noqa: ANN201
         self,
         binding_method=None,  # noqa: ANN001
         pool_name=None,  # noqa: ANN001
         force=None,  # noqa: ANN001
         redundancy=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "pool unbind "
+        cmd = 'pool unbind '
         if binding_method:
-            cmd += f"{binding_method} "
+            cmd += f'{binding_method} '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         kwargs.update(
             {
-                "force": force,
-                "redundancy": redundancy,
+                'force': force,
+                'redundancy': redundancy,
             },
         )
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_set_fs_limit(  # noqa: ANN201
         self,
         pool_name=None,  # noqa: ANN001
         fs_amount=None,  # noqa: ANN001
         force=None,  # noqa: ANN001
         redundancy=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "pool set-fs-limit "
+        cmd = 'pool set-fs-limit '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if fs_amount:
-            cmd += f"{fs_amount} "
+            cmd += f'{fs_amount} '
         kwargs.update(
             {
-                "force": force,
-                "redundancy": redundancy,
+                'force': force,
+                'redundancy': redundancy,
             },
         )
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_overprovision(self, pool_name=None, pool_overprovision=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool overprovision "
+        cmd = 'pool overprovision '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if pool_overprovision:
-            cmd += f"{pool_overprovision}"
+            cmd += f'{pool_overprovision}'
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_explain(self, pool_error_code=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool explain "
+        cmd = 'pool explain '
         if pool_error_code:
-            cmd += f"{pool_error_code} "
+            cmd += f'{pool_error_code} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_debug(  # noqa: ANN201
         self,
         debug_subcommand=None,  # noqa: ANN001
         pool_name=None,  # noqa: ANN001
         pool_uuid=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "pool debug "
+        cmd = 'pool debug '
         if debug_subcommand:
-            cmd += f"{debug_subcommand} "
+            cmd += f'{debug_subcommand} '
         if pool_name:
-            cmd += f"--name {pool_name} "
+            cmd += f'--name {pool_name} '
         if pool_uuid:
-            cmd += f"--uuid {pool_uuid} "
+            cmd += f'--uuid {pool_uuid} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_start(self, pool_name=None, pool_uuid=None, unlock_method=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool start "
+        cmd = 'pool start '
         if unlock_method:
-            cmd += f"--unlock-method {unlock_method} "
+            cmd += f'--unlock-method {unlock_method} '
         if self.get_stratis_major_version() <= 3 and self.get_stratis_minor_version() < 4:
             if pool_uuid:
-                cmd += f"{pool_uuid} "
+                cmd += f'{pool_uuid} '
             return self._run(cmd, **self._remove_nones(kwargs))
         if pool_name:
-            cmd += f"--name {pool_name} "
+            cmd += f'--name {pool_name} '
         if pool_uuid:
-            cmd += f"--uuid {pool_uuid} "
+            cmd += f'--uuid {pool_uuid} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_stop(self, pool_name=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool stop "
+        cmd = 'pool stop '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def pool_extend_data(self, pool_name=None, device_uuid=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "pool extend-data "
+        cmd = 'pool extend-data '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if device_uuid:
-            cmd += f"--device-uuid {device_uuid}"
+            cmd += f'--device-uuid {device_uuid}'
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def blockdev_list(self, pool_name=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "blockdev list "
+        cmd = 'blockdev list '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def blockdev_debug(self, debug_subcommand=None, dev_uuid=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "blockdev debug "
+        cmd = 'blockdev debug '
         if debug_subcommand:
-            cmd += f"{debug_subcommand} "
+            cmd += f'{debug_subcommand} '
         if dev_uuid:
-            cmd += f"--uuid {dev_uuid} "
+            cmd += f'--uuid {dev_uuid} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def fs_create(self, pool_name=None, fs_name=None, fs_size=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "fs create "
+        cmd = 'fs create '
         if fs_size:
-            cmd += f"--size {fs_size} "
+            cmd += f'--size {fs_size} '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if fs_name:
-            cmd += f"{fs_name} "
+            cmd += f'{fs_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def fs_debug(self, debug_subcommand=None, fs_name=None, fs_uuid=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "fs debug "
+        cmd = 'fs debug '
         if debug_subcommand:
-            cmd += f"{debug_subcommand} "
+            cmd += f'{debug_subcommand} '
         if fs_name:
-            cmd += f"--name {fs_name} "
+            cmd += f'--name {fs_name} '
         if fs_uuid:
-            cmd += f"--uuid {fs_uuid} "
+            cmd += f'--uuid {fs_uuid} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def fs_snapshot(  # noqa: ANN201
         self,
         pool_name=None,  # noqa: ANN001
         origin_name=None,  # noqa: ANN001
         snapshot_name=None,  # noqa: ANN001
         **kwargs,  # noqa: ANN003
     ):
-        cmd = "fs snapshot "
+        cmd = 'fs snapshot '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if origin_name:
-            cmd += f"{origin_name} "
+            cmd += f'{origin_name} '
         if snapshot_name:
-            cmd += f"{snapshot_name} "
+            cmd += f'{snapshot_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def fs_list(self, pool_name=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "fs list "
+        cmd = 'fs list '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def fs_destroy(self, pool_name=None, fs_name=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "fs destroy "
+        cmd = 'fs destroy '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if fs_name:
-            cmd += f"{fs_name} "
+            cmd += f'{fs_name} '
         return self._run(cmd, **self._remove_nones(kwargs))
 
     def fs_rename(self, pool_name=None, fs_name=None, new_name=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "fs rename "
+        cmd = 'fs rename '
         if pool_name:
-            cmd += f"{pool_name} "
+            cmd += f'{pool_name} '
         if fs_name:
-            cmd += f"{fs_name} "
+            cmd += f'{fs_name} '
         if new_name:
-            cmd += f"{new_name} "
+            cmd += f'{new_name} '
         return self._run(cmd, **kwargs)
 
     def key_set(self, keyfile_path=None, key_desc=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "key set "
+        cmd = 'key set '
         if keyfile_path:
-            cmd += f"--keyfile-path {keyfile_path} "
+            cmd += f'--keyfile-path {keyfile_path} '
         if key_desc:
-            cmd += f"{key_desc} "
-        ret = self._run("key list", return_output=True)
+            cmd += f'{key_desc} '
+        ret = self._run('key list', return_output=True)
         # ret is a tuple in format -> (return_code, return_output)
         if key_desc in ret[1]:
-            return self._run("key list")
+            return self._run('key list')
         return self._run(cmd, **kwargs)
 
     def key_reset(self, keyfile_path=None, key_desc=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "key reset "
+        cmd = 'key reset '
         if keyfile_path:
-            cmd += f"--keyfile-path {keyfile_path} "
+            cmd += f'--keyfile-path {keyfile_path} '
         if key_desc:
-            cmd += f"{key_desc} "
+            cmd += f'{key_desc} '
         return self._run(cmd, **kwargs)
 
     def key_list(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("key list", **kwargs)
+        return self._run('key list', **kwargs)
 
     def key_unset(self, key_desc=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        cmd = "key unset "
+        cmd = 'key unset '
         if key_desc:
-            cmd += f"{key_desc} "
+            cmd += f'{key_desc} '
         return self._run(cmd, **kwargs)
 
     # Pool unlock has been removed in favor of pool_start in Stratisd 3.2.0
     def pool_unlock(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("pool unlock", **kwargs)
+        return self._run('pool unlock', **kwargs)
 
     def daemon_redundancy(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("daemon redundancy", **kwargs)
+        return self._run('daemon redundancy', **kwargs)
 
     def daemon_version(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("daemon version", **kwargs)
+        return self._run('daemon version', **kwargs)
 
     def debug_refresh(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("debug refresh", **kwargs)
+        return self._run('debug refresh', **kwargs)
 
     def version(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("--version", **kwargs)
+        return self._run('--version', **kwargs)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/vdo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,263 +1,244 @@
 """vdo.py: Module with test specific method for VDO."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import stat
 from difflib import context_diff
 from pathlib import Path
 from typing import Dict, List, Union
 
 from sts import linux
-from sts.utils.atomic_run import atomic_run
 from sts.utils.cli_tools import (
     FailedCheckExceptionError,
     Wrapper,
     WrongArgumentExceptionError,
     WrongCommandExceptionError,
 )
 from sts.utils.cmdline import run, run_ret_out
 
 
-def restart_modify(vdo_object, vdo_name, errors):  # noqa: ANN001, ANN201
-    # sometimes VDO needs to be restarted for changes to take effect
-    print("Restarting VDO for changes to take effect.")
-    commands = [
-        {
-            "message": "Stopping VDO to apply modification.",
-            "command": vdo_object.stop,
-            "expected_out": ["Stopping VDO"],
-        },
-        {
-            "message": "Starting VDO to apply modification.",
-            "command": vdo_object.start,
-            "expected_out": ["Starting VDO", "VDO instance", "is ready"],
-        },
-    ]
-    for command in commands:
-        atomic_run(name=vdo_name, errors=errors, expected_ret=0, **command)
-
-
 def report_modify_difference(errors, status_old, status_new, changed_var, changed_argument):  # noqa: ANN001, ANN201
     status_old = [x for x in status_old.splitlines() if changed_var in x]
     status_new = [x for x in status_new.splitlines() if changed_var in x]
     print(f"Before: {', '.join(status_old)}")
     print(f"After:  {', '.join(status_new)}")
     diff = list(context_diff(status_old, status_new))
-    difference = "\n".join([x for x in diff if x.startswith("!")])
+    difference = '\n'.join([x for x in diff if x.startswith('!')])
 
     if not difference:
-        error = f"WARN: Modifying VDO to {changed_argument} did nothing."
+        error = f'WARN: Modifying VDO to {changed_argument} did nothing.'
         print(error)
         errors.append(error)
 
 
 def minimum_slab_size(device, default_to_2g=True):  # noqa: ANN001, ANN201
     def _get_raid_device(device):  # noqa: ANN001, ANN202
-        device_name = device.split("/").pop()
-        ret, device_link = run_ret_out(cmd=f"ls -al /dev/md | grep {device_name}", return_output=True)
+        device_name = device.split('/').pop()
+        ret, device_link = run_ret_out(cmd=f'ls -al /dev/md | grep {device_name}', return_output=True)
         if ret or device_link is None:
-            print(f"WARN: Device {device_name} not found in /dev/md.")
+            logging.warning(f'Device {device_name} not found in /dev/md.')
             return None
-        return device_link.split("../").pop()  # raid device
+        return device_link.split('../').pop()  # raid device
 
-    device_name = _get_raid_device(device) if device.startswith("/dev/md") else device.split("/").pop()
+    device_name = _get_raid_device(device) if device.startswith('/dev/md') else device.split('/').pop()
     ret, device_size = run_ret_out(cmd=f"lsblk | grep '{device_name} ' ", return_output=True)
     if ret or device_size is None:
-        print(f"WARN: Device {device_name} not found using lsblk. Using default 2G size.")
-        return "2G"
+        logging.warning(f'Device {device_name} not found using lsblk. Using default 2G size.')
+        return '2G'
     size = device_size.split()[3]
-    multipliers = ["M", "G", "T", "P", "E"]
+    multipliers = ['M', 'G', 'T', 'P', 'E']
     device_size = (float(size[:-1]) * (1024 ** multipliers.index(size[-1:]))).__int__()
     max_number_of_slabs = 8192
     minimum_size = 2 ** int(device_size / max_number_of_slabs).bit_length()
     if minimum_size < 128:
         minimum_size = 128
     if default_to_2g and minimum_size < 2048:
-        return "2G"
-    return str(minimum_size) + "M"
+        return '2G'
+    return str(minimum_size) + 'M'
 
 
 def maximum_logical_size():  # noqa: ANN201
     """Returns maximum logical size based on memory.
 
     Returns:
       string max_size.
     """
     good_size = 4096
-    memory = linux.get_memory()["mem"]["free"]
-    size = f"{good_size}T"
+    memory = linux.get_memory()['mem']['free']
+    size = f'{good_size}T'
     if memory < 10000:
         size = 2 ** (((4096.0 / 10000) * float(memory)).__int__().bit_length() - 1)
         if size > good_size:
             size = good_size
     return size
 
 
 def is_block_device(device):  # noqa: ANN001, ANN201
     try:
         mode = Path(device).stat().st_mode
     except OSError:
-        return f"Device {device} does not exist."
+        return f'Device {device} does not exist.'
 
     if not stat.S_ISBLK(mode):
-        msg = f"Device {device} is not block device, aborting."
+        msg = f'Device {device} is not block device, aborting.'
         print(msg)
         return msg
     return True
 
 
-def get_underlying_device(name, conf_file="/etc/vdoconf.yml"):  # noqa: ANN001, ANN201
+def get_underlying_device(name, conf_file='/etc/vdoconf.yml'):  # noqa: ANN001, ANN201
     vdo = VDO(disable_check=True)
     ret, data = vdo.status(name=name, return_output=True, verbosity=False, conf_file=conf_file)
     if ret != 0:
         msg = f"FAIL: Could not get status of VDO device '{name}'."
         print(msg)
         return None
     device = None
     for line in data.splitlines():
-        if "Storage device" in line:
+        if 'Storage device' in line:
             device = f"/dev/{line.split('/dev/').pop().split().pop(0).strip()}"
     if device is None:
         # The device is probably crashed and needs to be force removed
-        print("WARN: Could not find 'Device mapper status' in vdo status output.")
+        logging.warning("Could not find 'Device mapper status' in vdo status output.")
         # Let's try alternative way of getting the device by checking vdo config file
         # First get the config file
         conf_file = None
         for line in data.splitlines():
-            if "File:" in line:
-                conf_file = line.split("File:").pop().strip()
+            if 'File:' in line:
+                conf_file = line.split('File:').pop().strip()
         if not conf_file:
-            print("FAIL: Could not find vdo conf file in vdo status, something is really wrong!")
+            logging.error('Could not find vdo conf file in vdo status, something is really wrong!')
             return None
         # Read the file contents
         with Path(conf_file).open() as f:
             lines = f.readlines()
         correct_vdo_device = False
         for line in lines:
-            if f"{name}:" in line:
+            if f'{name}:' in line:
                 # Get the correct VDO device in the config, there might be more
                 correct_vdo_device = True
-            if correct_vdo_device and "device:" in line:
+            if correct_vdo_device and 'device:' in line:
                 # Now we have the device, just need to follow the link
-                device = line.split("device:").pop().strip()
+                device = line.split('device:').pop().strip()
                 break
 
     # now we might have /dev/disk/by-id/UUID, need to get something reasonable
-    data = run(f"ls -la {device}", capture_output=True, verbose=False).output
-    device = data.split("/").pop().strip()
+    data = run(f'ls -la {device}').stdout
+    device = data.split('/').pop().strip()
 
     # format dm-X causes issues later on, where the device cannot be found using lsblk to check for size
-    if device.startswith("dm-"):
-        with Path(f"/sys/block/{device}/dm/name").open() as f:
-            dev_name = f.readline().rstrip("\n")
-        device = f"/dev/mapper/{dev_name}"
+    if device.startswith('dm-'):
+        with Path(f'/sys/block/{device}/dm/name').open() as f:
+            dev_name = f.readline().rstrip('\n')
+        device = f'/dev/mapper/{dev_name}'
     else:
-        device = f"/dev/{device}"
+        device = f'/dev/{device}'
 
     return device
 
 
 def get_replace_dict():  # noqa: ANN201
     """Returns dict of keys to replace from fmf to sts.vdo.VDO.
 
     Returns:
       dict.
     """
-    return {"vdo_name": "name"}
+    return {'vdo_name': 'name'}
 
 
 class VDO(Wrapper):
     def __init__(self, disable_check=False) -> None:  # noqa: ANN001
         self.disable_check = disable_check
 
         self.commands: Dict[str, Union[str, List[str]]] = {
-            "create": "create",
-            "remove": "remove",
-            "start": "start",
-            "stop": "stop",
-            "activate": "activate",
-            "deactivate": "deactivate",
-            "status": "status",
-            "list": "list",
-            "modify": "modify",
-            "change_write_policy": "changeWritePolicy",
-            "enable_deduplication": "enableDeduplication",
-            "disable_deduplication": "disableDeduplication",
-            "enable_compression": "enableCompression",
-            "disable_compression": "disableCompression",
-            "grow_logical": "growLogical",
-            "grow_physical": "growPhysical",
-            "print_config_file": "printConfigFile",
+            'create': 'create',
+            'remove': 'remove',
+            'start': 'start',
+            'stop': 'stop',
+            'activate': 'activate',
+            'deactivate': 'deactivate',
+            'status': 'status',
+            'list': 'list',
+            'modify': 'modify',
+            'change_write_policy': 'changeWritePolicy',
+            'enable_deduplication': 'enableDeduplication',
+            'disable_deduplication': 'disableDeduplication',
+            'enable_compression': 'enableCompression',
+            'disable_compression': 'disableCompression',
+            'grow_logical': 'growLogical',
+            'grow_physical': 'growPhysical',
+            'print_config_file': 'printConfigFile',
         }
-        self.commands["all"] = list(self.commands.keys())
+        self.commands['all'] = list(self.commands.keys())
 
         self.arguments = {
-            "all": [self.commands["all"], " --all"],
-            "conf_file": [self.commands["all"], " --confFile="],
-            "log_file": [self.commands["all"], " --logfile="],
-            "name": [self.commands["all"], " --name="],
-            "no_run": [self.commands["all"], " --noRun"],
-            "verbose": [self.commands["all"], " --verbose"],
-            "activate": [["create"], " --activate="],
-            "compression": [["create"], " --compression="],
-            "deduplication": [["create"], " --deduplication="],
-            "device": [["create"], " --device="],
-            "emulate512": [["create"], " --emulate512="],
-            "index_mem": [["create"], " --indexMem="],
-            "sparse_index": [["create"], " --sparseIndex="],
-            "logical_size": [["create", "grow_logical"], " --vdoLogicalSize="],
-            "log_level": [["create"], " --vdoLogLevel="],
-            "slab_size": [["create"], " --vdoSlabSize="],
-            "block_map_cache_size": [["create", "modify"], " --blockMapCacheSize="],
-            "block_map_period": [["create", "modify"], " --blockMapPeriod="],
-            "max_discard_size": [["create", "modify"], " --maxDiscardSize="],
-            "ack_threads": [["create", "modify"], " --vdoAckThreads="],
-            "bio_rotation_interval": [
-                ["create", "modify"],
-                " --vdoBioRotationInterval=",
+            'all': [self.commands['all'], ' --all'],
+            'conf_file': [self.commands['all'], ' --confFile='],
+            'log_file': [self.commands['all'], ' --logfile='],
+            'name': [self.commands['all'], ' --name='],
+            'no_run': [self.commands['all'], ' --noRun'],
+            'verbose': [self.commands['all'], ' --verbose'],
+            'activate': [['create'], ' --activate='],
+            'compression': [['create'], ' --compression='],
+            'deduplication': [['create'], ' --deduplication='],
+            'device': [['create'], ' --device='],
+            'emulate512': [['create'], ' --emulate512='],
+            'index_mem': [['create'], ' --indexMem='],
+            'sparse_index': [['create'], ' --sparseIndex='],
+            'logical_size': [['create', 'grow_logical'], ' --vdoLogicalSize='],
+            'log_level': [['create'], ' --vdoLogLevel='],
+            'slab_size': [['create'], ' --vdoSlabSize='],
+            'block_map_cache_size': [['create', 'modify'], ' --blockMapCacheSize='],
+            'block_map_period': [['create', 'modify'], ' --blockMapPeriod='],
+            'max_discard_size': [['create', 'modify'], ' --maxDiscardSize='],
+            'ack_threads': [['create', 'modify'], ' --vdoAckThreads='],
+            'bio_rotation_interval': [
+                ['create', 'modify'],
+                ' --vdoBioRotationInterval=',
             ],
-            "bio_threads": [["create", "modify"], " --vdoBioThreads="],
-            "cpu_threads": [["create", "modify"], " --vdoCpuThreads="],
-            "hash_zone_threads": [["create", "modify"], " --vdoHashZoneThreads="],
-            "logical_threads": [["create", "modify"], " --vdoLogicalThreads="],
-            "physical_threads": [["create", "modify"], " --vdoPhysicalThreads="],
-            "write_policy": [
-                ["create", "modify", "change_write_policy"],
-                " --writePolicy=",
+            'bio_threads': [['create', 'modify'], ' --vdoBioThreads='],
+            'cpu_threads': [['create', 'modify'], ' --vdoCpuThreads='],
+            'hash_zone_threads': [['create', 'modify'], ' --vdoHashZoneThreads='],
+            'logical_threads': [['create', 'modify'], ' --vdoLogicalThreads='],
+            'physical_threads': [['create', 'modify'], ' --vdoPhysicalThreads='],
+            'write_policy': [
+                ['create', 'modify', 'change_write_policy'],
+                ' --writePolicy=',
             ],
-            "force_rebuild": [["start"], " --forceRebuild"],
-            "force": [["stop", "remove", "create"], " --force"],
+            'force_rebuild': [['start'], ' --forceRebuild'],
+            'force': [['stop', 'remove', 'create'], ' --force'],
         }
 
         Wrapper.__init__(self, self.commands, self.arguments, self.disable_check)
 
     @staticmethod
     def _check_size_format(size, return_size=False):  # noqa: ANN001, ANN205
         # check if requested size format is in supported formats and the rest is numbers
         # FIXME: Is KiB and KB valid too?
         size = size.strip("'")
         try:
-            if size[-3:] in ["KiB", "MiB", "GiB", "TiB"] and isinstance(int(size[:-3]), int):
+            if size[-3:] in ['KiB', 'MiB', 'GiB', 'TiB'] and isinstance(int(size[:-3]), int):
                 if return_size:
                     return True, [size[:-3], size[-3:-2]]
                 return True
-            if size[-2:] in ["KB", "MB", "GB", "TB"] and isinstance(int(size[:-2]), int):
+            if size[-2:] in ['KB', 'MB', 'GB', 'TB'] and isinstance(int(size[:-2]), int):
                 if return_size:
                     return True, [size[:-2], size[-2:-1]]
                 return True
-            if size[-1:].upper() in ["K", "M", "G", "T"] and isinstance(int(size[:-1]), int):
+            if size[-1:].upper() in ['K', 'M', 'G', 'T'] and isinstance(int(size[:-1]), int):
                 if return_size:
                     return True, [size[:-1], size[-1:]]
                 return True
             if int(size):
                 if return_size:
                     # default size is megabytes
-                    return True, [size, "M"]
+                    return True, [size, 'M']
                 return True
         except ValueError:
             pass
         return False, []
 
     @staticmethod
     def _is_positive_int(value):  # noqa: ANN001, ANN205
@@ -270,240 +251,244 @@
         return True
 
     def _check(self, cmd):  # noqa: ANN001, ANN202
         if self.disable_check:
             # Do not check if checking is disabled
             return True
 
-        if self._get_arg("all") in cmd and self._get_arg("name") in cmd:
-            print("WARN: Use either 'name' or 'all', not both.")
+        if self._get_arg('all') in cmd and self._get_arg('name') in cmd:
+            logging.warning("Use either 'name' or 'all', not both.")
             raise FailedCheckExceptionError
 
-        if self._get_arg("conf_file") in cmd:
-            _file = self._get_value(cmd, self._get_arg("conf_file"))
+        if self._get_arg('conf_file') in cmd:
+            _file = self._get_value(cmd, self._get_arg('conf_file'))
             if not Path(_file).is_file():
-                print(f"WARN: Config file {_file} is not a regular file.")
-                raise FailedCheckExceptionError(self._get_arg("conf_file"))
+                logging.warning(f'Config file {_file} is not a regular file.')
+                raise FailedCheckExceptionError(self._get_arg('conf_file'))
 
-        if self._get_arg("log_file") in cmd:
-            _file = self._get_value(cmd, self._get_arg("log_file"))
+        if self._get_arg('log_file') in cmd:
+            _file = self._get_value(cmd, self._get_arg('log_file'))
             f = Path(_file)
             if not f.is_file() and stat.S_ISBLK(f.stat().st_mode):
-                print(f"WARN: Path {_file} exists and is not a regular file.")
-                raise FailedCheckExceptionError(self._get_arg("log_file"))
+                logging.warning(f'Path {_file} exists and is not a regular file.')
+                raise FailedCheckExceptionError(self._get_arg('log_file'))
 
-        if self._get_arg("name") in cmd:
+        if self._get_arg('name') in cmd:
             # FIXME: Check if VDO already exists
             pass
 
         for arg in [
-            "activate",
-            "compression",
-            "deduplication",
-            "emulate512",
-            "sparse_index",
+            'activate',
+            'compression',
+            'deduplication',
+            'emulate512',
+            'sparse_index',
         ]:
             if self._get_arg(arg) in cmd:
                 _value = self._get_value(cmd, self._get_arg(arg))
-                if _value not in ["enabled", "disabled"]:
-                    print(f"WARN: {arg} value must be either 'enabled' or 'disabled'.")
+                if _value not in ['enabled', 'disabled']:
+                    logging.warning(f"{arg} value must be either 'enabled' or 'disabled'.")
                     raise FailedCheckExceptionError(self._get_arg(arg))
 
         for arg in [
-            "logical_size",
-            "slab_size",
-            "block_map_cache_size",
-            "max_discard_size",
+            'logical_size',
+            'slab_size',
+            'block_map_cache_size',
+            'max_discard_size',
         ]:
             if self._get_arg(arg) in cmd:
                 _value = self._get_value(cmd, self._get_arg(arg))
                 ret, _ = self._check_size_format(_value, return_size=True)
                 if not ret:
-                    print(f"WARN: VDO {' '.join(arg.split('_'))} value {_value} is in unknown format.")
+                    logging.warning(f"VDO {' '.join(arg.split('_'))} value {_value} is in unknown format.")
                     raise FailedCheckExceptionError(self._get_arg(arg))
                 if arg == "slab_size":  # noqaSIM114
                     pass
                     # FIXME: Check if size is power of 2 between 128M and 32G
-                elif arg == "block_map_cache_size":
+                elif arg == 'block_map_cache_size':
                     pass
                     # FIXME: Check if size is multiple of 4096
 
-        if self._get_arg("index_mem") in cmd:
-            _value = self._get_value(cmd, self._get_arg("index_mem"), return_type=float)
+        if self._get_arg('index_mem') in cmd:
+            _value = self._get_value(cmd, self._get_arg('index_mem'), return_type=float)
             if not (_value in [0, 0.25, 0.5, 0.75] or self._is_positive_int(_value)):
-                print(f"WARN: Albireo mem value {_value} is not a 0, 0.25, 0.5, 0.75 or positive int.")
-                raise FailedCheckExceptionError(self._get_arg("index_mem"))
+                logging.warning(f'Albireo mem value {_value} is not a 0, 0.25, 0.5, 0.75 or positive int.')
+                raise FailedCheckExceptionError(self._get_arg('index_mem'))
 
-        if self._get_arg("log_level") in cmd:
-            _value = self._get_value(cmd, self._get_arg("log_level"))
+        if self._get_arg('log_level') in cmd:
+            _value = self._get_value(cmd, self._get_arg('log_level'))
             possible_values = [
-                "critical",
-                "error",
-                "warning",
-                "notice",
-                "info",
-                "debug",
+                'critical',
+                'error',
+                'warning',
+                'notice',
+                'info',
+                'debug',
             ]
             if _value not in possible_values:
-                print(f"WARN: Unknown vdo log level value, must be one of {possible_values}.")
-                raise FailedCheckExceptionError(self._get_arg("log_level"))
+                logging.warning(f'Unknown vdo log level value, must be one of {possible_values}.')
+                raise FailedCheckExceptionError(self._get_arg('log_level'))
 
-        if self._get_arg("device") in cmd:
-            _value = self._get_value(cmd, self._get_arg("device"))
+        if self._get_arg('device') in cmd:
+            _value = self._get_value(cmd, self._get_arg('device'))
             # FIXME: Check if device exists
 
-        if self._get_arg("block_map_period") in cmd:
-            _value = self._get_value(cmd, self._get_arg("block_map_period"))
+        if self._get_arg('block_map_period') in cmd:
+            _value = self._get_value(cmd, self._get_arg('block_map_period'))
             if not self._is_positive_int(_value):
-                print("WARN: Block map period value must be a positive integer.")
-                raise FailedCheckExceptionError(self._get_arg("block_map_period"))
+                logging.warning('Block map period value must be a positive integer.')
+                raise FailedCheckExceptionError(self._get_arg('block_map_period'))
             # FIXME: Can this be higher than 16380?
 
         for arg in [
-            "ack_threads",
-            "bio_rotation_interval",
-            "bio_threads",
-            "cpu_threads",
-            "hash_zone_threads",
-            "logical_threads",
-            "physical_threads",
+            'ack_threads',
+            'bio_rotation_interval',
+            'bio_threads',
+            'cpu_threads',
+            'hash_zone_threads',
+            'logical_threads',
+            'physical_threads',
         ]:
             if self._get_arg(arg) in cmd:
                 _value = self._get_value(cmd, self._get_arg(arg))
                 if not self._is_positive_int(_value):
-                    print(f"WARN: VDO {' '.join(arg.split('_'))} value must be a positive integer.")
+                    logging.warning(f"VDO {' '.join(arg.split('_'))} value must be a positive integer.")
                     raise FailedCheckExceptionError(self._get_arg(arg))
                     # FIXME: Is 0 valid?
 
-        if self._get_arg("write_policy") in cmd:
-            _value = self._get_value(cmd, self._get_arg("write_policy"))
-            if _value not in ["sync", "async"]:
-                print("WARN: VDO read cache value must be either 'sync' or 'async'.")
-                raise FailedCheckExceptionError(self._get_arg("write_policy"))
+        if self._get_arg('write_policy') in cmd:
+            _value = self._get_value(cmd, self._get_arg('write_policy'))
+            if _value not in ['sync', 'async']:
+                logging.warning("VDO read cache value must be either 'sync' or 'async'.")
+                raise FailedCheckExceptionError(self._get_arg('write_policy'))
 
-        if self._get_arg("force_rebuild") in cmd and self._get_arg("upgrade") in cmd:
-            print("WARN: Cannot use both force_rebuild and upgrade when starting VDO volume.")
+        if self._get_arg('force_rebuild') in cmd and self._get_arg('upgrade') in cmd:
+            logging.warning('Cannot use both force_rebuild and upgrade when starting VDO volume.')
             raise FailedCheckExceptionError
 
         return True
 
-    def _run(self, cmd, verbosity=True, return_output=False, **kwargs):  # noqa: ANN001, ANN003, ANN202
+    def _run(self, cmd, return_output=False, **kwargs):  # noqa: ANN001, ANN003, ANN202
         # Constructs the command to run and runs it
 
         ret_fail = False
         if return_output:
             ret_fail = (False, None)
 
         try:
             command = self._add_command(cmd)
             command = self._add_arguments(command, **kwargs)
 
         except WrongCommandExceptionError as e:
-            print(f"WARN: Given command '{e.command}' is not allowed in this VDO version.")
+            logging.warning(f"Given command '{e.command}' is not allowed in this VDO version.")
             return ret_fail
         except WrongArgumentExceptionError as e:
             message = f"WARN: Given argument '{e.argument}' is not allowed for given command."
             if e.command:
                 message = message[:-1] + " '" + e.command + "'."
             if e.arguments:
                 message += f"\nPlease use only these: {', '.join(e.arguments)}."
             print(message)
             return ret_fail
 
-        cmd = "vdo " + command
+        cmd = 'vdo ' + command
 
         try:
             self._check(cmd)
         except WrongArgumentExceptionError:
             pass
         except FailedCheckExceptionError as e:
-            print(f"WARN: Failed checking on argument {e.argument}")
+            logging.warning(f'Failed checking on argument {e.argument}')
             return ret_fail
 
         if return_output:
-            ret, data = run_ret_out(cmd, verbose=verbosity, return_output=True)
+            ret, data = run_ret_out(cmd, return_output=True)
             if ret != 0:
-                print(f"WARN: Running command: '{cmd}' failed. Return with output.")
+                logging.warning(f"Running command: '{cmd}' failed. Return with output.")
             return ret, data
-        ret = run(cmd, verbose=verbosity).returncode
+        ret = run(cmd).rc
         if ret != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+            logging.warning(f"Running command: '{cmd}' failed.")
         return ret
 
     @staticmethod
     def help():  # noqa: A003, ANN205
-        if run("vdo --help", verbose=True) != 0:
-            print("WARN: Running command: 'vdo --help' failed.")
+        if run('vdo --help') != 0:
+            logging.warning("Running command: 'vdo --help' failed.")
             return False
         return True
 
     def create(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("create", **kwargs)
+        return self._run('create', **kwargs)
 
     def remove(self, force=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run("remove", force=force, **kwargs)
+        return self._run('remove', force=force, **kwargs)
 
     def start(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("start", **kwargs)
+        return self._run('start', **kwargs)
 
     def stop(self, force=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run("stop", force=force, **kwargs)
+        return self._run('stop', force=force, **kwargs)
+
+    def restart(self) -> None:
+        self.stop()
+        self.start()
 
     def activate(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("activate", **kwargs)
+        return self._run('activate', **kwargs)
 
     def deactivate(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("deactivate", **kwargs)
+        return self._run('deactivate', **kwargs)
 
     def status(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("status", **kwargs)
+        return self._run('status', **kwargs)
 
     def list(self, **kwargs):  # noqa: A003, ANN003, ANN201
-        return self._run("list", **kwargs)
+        return self._run('list', **kwargs)
 
     def modify(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("modify", **kwargs)
+        return self._run('modify', **kwargs)
 
     def change_write_policy(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("change_write_policy", **kwargs)
+        return self._run('change_write_policy', **kwargs)
 
     def deduplication(self, enable=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run("enable_deduplication", **kwargs) if enable else self._run("disable_deduplication", **kwargs)
+        return self._run('enable_deduplication', **kwargs) if enable else self._run('disable_deduplication', **kwargs)
 
     def compression(self, enable=True, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        return self._run("enable_compression", **kwargs) if enable else self._run("disable_compression", **kwargs)
+        return self._run('enable_compression', **kwargs) if enable else self._run('disable_compression', **kwargs)
 
     def grow(self, grow_type=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
-        if grow_type.upper() not in ["LOGICAL", "PHYSICAL"]:
-            print("WARN: Please specify either 'logical' or 'physical' type for growing VDO.")
-            if kwargs["return_output"]:
+        if grow_type.upper() not in ['LOGICAL', 'PHYSICAL']:
+            logging.warning("Please specify either 'logical' or 'physical' type for growing VDO.")
+            if kwargs['return_output']:
                 return False, None
             return False
 
-        if grow_type.upper() == "LOGICAL":
-            ret = self._run("grow_logical", **kwargs)
+        if grow_type.upper() == 'LOGICAL':
+            ret = self._run('grow_logical', **kwargs)
         else:
-            ret = self._run("grow_physical", **kwargs)
+            ret = self._run('grow_physical', **kwargs)
         return ret
 
     def print_config_file(self, **kwargs):  # noqa: ANN003, ANN201
-        return self._run("print_config_file", **kwargs)
+        return self._run('print_config_file', **kwargs)
 
 
 class VDOStats:
     def __init__(self, disable_check=False) -> None:  # noqa: ANN001
         self.disable_check = disable_check
-        self.command = "vdostats"
+        self.command = 'vdostats'
         self.arguments = {
-            "help": " --help",
-            "all": " --all",
-            "human_readable": " --human-readable",
-            "si": " --si",
-            "verbose": " --verbose",
-            "version": " --version",
+            'help': ' --help',
+            'all': ' --all',
+            'human_readable': ' --human-readable',
+            'si': ' --si',
+            'verbose': ' --verbose',
+            'version': ' --version',
         }
 
     def _get_arg(self, name):  # noqa: ANN001, ANN202
         return self.arguments[name]
 
     def _get_possible_arguments(self):  # noqa: ANN202
         # Returns possible arguments
@@ -519,15 +504,15 @@
 
     def _add_arguments(self, cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
         command = cmd
         for kwarg in kwargs:
             command = self._add_argument(kwarg, command)
             if command is None:
                 args = self._get_possible_arguments()
-                print(f"WARN: Unknown argument '{kwarg}', please use only these: {args}.")
+                logging.warning(f"Unknown argument '{kwarg}', please use only these: {args}.")
                 return None
         return command
 
     def _check(self, cmd):  # noqa: ANN001, ANN202
         if self.disable_check:
             # Do not check if checking is disabled
             return True
@@ -536,41 +521,41 @@
         for block in cmd.split():
             file = Path(block)
             if (
                 (block not in list(self.arguments.values()) and block != self.command)
                 and file.exists()
                 and not stat.S_ISBLK(file.stat().st_mode)
             ):
-                print(f"WARN: Device {block} is not a block device.")
+                logging.warning(f'Device {block} is not a block device.')
                 return False
 
         return True
 
     def _run(self, **kwargs):  # noqa: ANN003, ANN202
         # Constructs the command to run and runs it
         cmd = self.command
 
-        if "devices" in kwargs:
-            devices = kwargs.pop("devices")
+        if 'devices' in kwargs:
+            devices = kwargs.pop('devices')
             if isinstance(devices, list):
                 for device in devices:
-                    cmd += " " + str(device)
+                    cmd += ' ' + str(device)
             else:
-                cmd += " " + str(devices)
+                cmd += ' ' + str(devices)
 
         cmd = self._add_arguments(cmd, **kwargs)
         if cmd is None:
             return False
 
         if not self._check(cmd):
             # Requested command did not pass checking, reason was already written by _check()
             return False
 
-        if run(cmd, verbose=True).returncode != 0:
-            print(f"WARN: Running command: '{cmd}' failed.")
+        if run(cmd).rc != 0:
+            logging.warning(f"Running command: '{cmd}' failed.")
             return False
         return True
 
     def help(self):  # noqa: A003, ANN201
         if not self._run(help=True):
             return False
         return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/beaker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """beaker.py: Module to manage beaker."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
-import re  # regex
+import re
 
 from sts.utils.cmdline import run, run_ret_out
 from sts.utils.restraint import is_restraint_job, log_submit
 
 
 def get_task_timeout(task_id):  # noqa: ANN001, ANN201
     """Get how much time the task still has
@@ -19,102 +20,102 @@
     or
     int(value):       The remaining time in seconds.
     """
     if not is_restraint_job():
         return None
 
     if task_id is None:
-        print("FAIL: beaker get_task_timeout() - requires task_id as parameter")
+        logging.error('beaker get_task_timeout() - requires task_id as parameter')
         return None
 
-    cmd = f"bkr watchdog-show {task_id}"
-    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'bkr watchdog-show {task_id}'
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print("FAIL: beaker get_task_timeout() - Could not get beaker kill time")
+        logging.error('beaker get_task_timeout() - Could not get beaker kill time')
         print(output)
         return None
 
-    output_regex = re.compile(r"%s: (\d+)" % task_id)
+    output_regex = re.compile(r'%s: (\d+)' % task_id)
     m = output_regex.match(output)
     if m:
         return int(m.group(1))
-    print("FAIL: beaker get_task_timeout() - Could not parse output:")
+    logging.error('beaker get_task_timeout() - Could not parse output:')
     print(output)
     return None
 
 
 def get_task_status(task_id):  # noqa: ANN001, ANN201
     """Requires beaker-client package installed and configured."""
     if not is_restraint_job():
         return None
 
     if not task_id:
-        print("FAIL: get_task_status() - requires task id")
+        logging.error('get_task_status() - requires task id')
         return None
 
-    cmd = f"bkr job-results --prettyxml T:{task_id}"
-    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'bkr job-results --prettyxml T:{task_id}'
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print(f"FAIL: get_task_status() - Could not get beaker task result for T:{task_id}")
+        logging.error(f'get_task_status() - Could not get beaker task result for T:{task_id}')
         print(output)
         return None
 
-    lines = output.split("\n")
-    status_regex = re.compile(r"<task.*status=\"(\S+)\"")
+    lines = output.split('\n')
+    status_regex = re.compile(r'<task.*status=\"(\S+)\"')
     for line in lines:
         m = status_regex.match(line)
         if m:
             return m.group(1)
     return None
 
 
 def console_log_check(error_mgs):  # noqa: ANN001, ANN201
     """Checks for error messages on console log ("Call Trace and segfault")."""
     error = 0
-    console_log_file = "/root/console.log"
-    prev_console_log_file = "/root/console.log.prev"
-    new_console_log_file = "/root/console.log.new"
+    console_log_file = '/root/console.log'
+    prev_console_log_file = '/root/console.log.prev'
+    new_console_log_file = '/root/console.log.new'
 
     if not is_beaker_job():
-        print("WARN: skip console_log_check as it doesn't seem to be a beaker job")
+        logging.warning("skip console_log_check as it doesn't seem to be a beaker job")
         return True
 
-    lab_controller = os.environ["LAB_CONTROLLER"]
-    recipe_id = os.environ["BEAKER_RECIPE_ID"]
+    lab_controller = os.environ['LAB_CONTROLLER']
+    recipe_id = os.environ['BEAKER_RECIPE_ID']
 
     # get current console log
-    url = f"http://{lab_controller}:8000/recipes/{recipe_id}/logs/console.log"
+    url = f'http://{lab_controller}:8000/recipes/{recipe_id}/logs/console.log'
 
-    if run(f"curl -s {url} -O {new_console_log_file}") != 0:
-        print("INFO: Could not get console log")
+    if run(f'curl -s {url} -O {new_console_log_file}') != 0:
+        logging.info('Could not get console log')
         # return success when could not get console.log
         return True
 
     # if there was previous console log, we just check the new part
     run(
-        f"diff -N -n --unidirectional-new-file {prev_console_log_file} {new_console_log_file} > {console_log_file}",
+        f'diff -N -n --unidirectional-new-file {prev_console_log_file} {new_console_log_file} > {console_log_file}',
     )
 
     # backup the current full console.log
     # next time we run the test we will compare just
     # what has been appended to console.log
-    run(f"mv -f {new_console_log_file} {prev_console_log_file}")
+    run(f'mv -f {new_console_log_file} {prev_console_log_file}')
 
-    print(f"INFO: Checking for errors on {console_log_file}")
+    logging.info(f'Checking for errors on {console_log_file}')
     for msg in error_mgs:
-        output = run(f"cat {console_log_file} | grep -i '{msg}'", capture_output=True).output
+        output = run(f"cat {console_log_file} | grep -i '{msg}'").stdout
         if output:
-            print(f"INFO found {msg} on {console_log_file}")
+            print(f'INFO found {msg} on {console_log_file}')
             log_submit(console_log_file)
             error = +1
 
     if error:
         return False
 
-    print(f"PASS: No errors on {console_log_file} have been found.")
+    print(f'PASS: No errors on {console_log_file} have been found.')
     return True
 
 
 def is_beaker_job():  # noqa: ANN201
     """Checks if it is beaker job."""
-    need_env = ["BEAKER", "BEAKER_RECIPE_ID", "LAB_CONTROLLER"]
+    need_env = ['BEAKER', 'BEAKER_RECIPE_ID', 'LAB_CONTROLLER']
     return all(not var not in os.environ for var in need_env)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/cli_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """cli_tools.py: Module to provide tools of wrapping command line tools for further usage."""
-from typing import List, Optional
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
+from typing import List, Optional
+
 
 class WrongCommandExceptionError(Exception):
     def __init__(self, cmd) -> None:  # noqa: ANN001
         self.command = cmd
         super().__init__()
 
     def __str__(self) -> str:
-        return repr(WrongCommandExceptionError.__name__ + ", caused by " + repr(self.command))
+        return repr(WrongCommandExceptionError.__name__ + ', caused by ' + repr(self.command))
 
 
 class WrongArgumentExceptionError(Exception):
     def __init__(self, arg, cmd=None, args=None) -> None:  # noqa: ANN001
         self.argument = arg
         self.command = cmd
         self.arguments = args
         super().__init__()
 
     def __str__(self) -> str:
-        return repr(WrongArgumentExceptionError.__name__ + ", caused by " + repr(self.argument))
+        return repr(WrongArgumentExceptionError.__name__ + ', caused by ' + repr(self.argument))
 
 
 class FailedCheckExceptionError(Exception):
     def __init__(self, arg=None) -> None:  # noqa: ANN001
         self.argument = arg
         super().__init__()
 
     def __str__(self) -> str:
         message = repr(FailedCheckExceptionError.__name__)
         if self.argument:
-            message += ", caused by " + repr(self.argument)
+            message += ', caused by ' + repr(self.argument)
         return message
 
 
 class Wrapper:
     def __init__(self, commands, arguments, disable_check) -> None:  # noqa: ANN001
         self.commands = commands
         self.arguments = arguments
@@ -54,42 +56,42 @@
             if name in self.arguments:
                 return self.arguments[name][1]
             raise WrongArgumentExceptionError(name)
         return self.arguments[name][1]
 
     def _get_cmd(self, name):  # noqa: ANN001, ANN202
         if self.disable_check:
-            return self.commands["all"]
+            return self.commands['all']
         if name in self.arguments:
             return self.arguments[name][0]
         raise WrongCommandExceptionError(name)
 
     @staticmethod
     def _get_value(string, command, return_type=str):  # noqa: ANN001, ANN205
         _value = string.split(command)[1].split()[0]
         try:
             value = return_type(_value)
         except ValueError as e:
-            print(f"WARN: Got ValueError: {e}.")
+            logging.warning(f'Got ValueError: {e}.')
             return None
         return value
 
     def _get_possible_arguments(self, command: Optional[str] = None) -> List[str]:
         # Returns possible arguments for the specified command if provided
         if command:
             args = [key for key in self.arguments if self._get_cmd(key) == command]
         else:
             args = list(self.arguments.keys())
         return args
 
     @staticmethod
     def _add_value(value, command, argument):  # noqa: ANN001, ANN205
-        if argument[-1:] in ["=", "&"]:
-            if argument[-1:] == "&":
-                argument = argument[:-1] + " "
+        if argument[-1:] in ['=', '&']:
+            if argument[-1:] == '&':
+                argument = argument[:-1] + ' '
             if isinstance(value, list):
                 # allows to use repeatable arguments as a list of values
                 for val in value:
                     command += argument + "'" + str(val) + "'"
             else:
                 command += argument + "'" + str(value) + "'"
         else:
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/logchecker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """logchecker.py: Module to Check for errors on the system."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import re
 from datetime import datetime
 from os import getenv
 from pathlib import Path
 
 import sts.linux
 from sts.utils import beaker, restraint
 from sts.utils.cmdline import run, run_ret_out
 
-segfault_msg = " segfault "
-calltrace_msg = "Call Trace:"
+segfault_msg = ' segfault '
+calltrace_msg = 'Call Trace:'
 
 error_mgs = [segfault_msg, calltrace_msg]
 
-tmt_test_data = getenv("TMT_TEST_DATA")
-LOG_PATH = tmt_test_data if tmt_test_data else "./"
+tmt_test_data = getenv('TMT_TEST_DATA')
+LOG_PATH = tmt_test_data if tmt_test_data else './'
 
 
 def journalctl_timestamp() -> str:
     """Returns current time in journalctl-compatible format.
 
     Usage example:
         logging_start = journalctl_timestamp()
-        failure_logs = run(f"journalctl -S {logging_start}, capture_output=True).output"
+        failure_logs = run(f"journalctl -S {logging_start}).stdout"
     """
-    return datetime.now().isoformat(sep=" ", timespec="minutes")  # noqa: DTZ005 <- We want local timezone.
+    return datetime.now().isoformat(sep=' ', timespec='minutes')  # noqa: DTZ005 <- We want local timezone.
 
 
 def check_all():  # noqa: ANN201
     """Check for error on the system
     Returns:
     Boolean:
     True is no error was found
     False if some error was found.
     """
-    print("INFO: Checking for error on the system")
+    logging.info('Checking for error on the system')
     error = 0
 
     if not kernel_check():
         error += 1
     if not abrt_check():
         error += 1
     if not messages_dump_check():
@@ -51,22 +52,22 @@
         error += 1
     if not console_log_check():
         error += 1
     if not kdump_check():
         error += 1
 
     if error:
-        log_messages = "/var/log/messages"
+        log_messages = '/var/log/messages'
         log_messages_path = Path(log_messages)
         if log_messages_path.is_file():
-            print(f"submit {log_messages}, named messages.log")
-            run(f"cp {log_messages} {LOG_PATH}messages.log")
-            restraint.log_submit("messages.log")
+            print(f'submit {log_messages}, named messages.log')
+            run(f'cp {log_messages} {LOG_PATH}messages.log')
+            restraint.log_submit('messages.log')
 
-        if sts.linux.is_installed("sos"):
+        if sts.linux.is_installed('sos'):
             sos_file = sts.linux.generate_sosreport()
             if not sos_file:
                 return False
             restraint.log_submit(sos_file)
         return False
 
     return True
@@ -75,55 +76,55 @@
 def abrt_check():  # noqa: ANN201
     """Check if abrtd found any issue
     Returns:
     Boolean:
     True no error was found
     False some error was found.
     """
-    print("INFO: Checking abrt for error")
+    logging.info('Checking abrt for error')
 
-    if run("rpm -q abrt", verbose=False) != 0:
-        print("WARN: abrt tool does not seem to be installed")
-        print("WARN: skipping abrt check")
+    if run('rpm -q abrt') != 0:
+        logging.warning('abrt tool does not seem to be installed')
+        logging.warning('skipping abrt check')
         return True
 
-    if run("pidof abrtd", verbose=False) != 0:
-        print("FAIL: abrtd is not running")
+    if run('pidof abrtd') != 0:
+        logging.error('abrtd is not running')
         return False
 
-    ret, log = run_ret_out("abrt-cli list", return_output=True)
+    ret, log = run_ret_out('abrt-cli list', return_output=True)
     if ret != 0:
-        print("FAIL: abrt-cli command failed")
+        logging.error('abrt-cli command failed')
         return False
 
     # We try to match for "Directory" to check if
     # abrt-cli list is actually listing any issue
     error = False
     if log:
-        lines = log.split("\n")
+        lines = log.split('\n')
         for line in lines:
-            m = re.match(r"Directory:\s+(\S+)", line)
+            m = re.match(r'Directory:\s+(\S+)', line)
             if m:
                 directory = m.group(1)
                 filename = directory
-                filename = filename.replace(":", "-")
-                filename += ".tar.gz"
-                run(f"tar cfzP {filename} {directory}")
+                filename = filename.replace(':', '-')
+                filename += '.tar.gz'
+                run(f'tar cfzP {filename} {directory}')
                 restraint.log_submit(filename)
-                run(f"mv {filename} {LOG_PATH}")
+                run(f'mv {filename} {LOG_PATH}')
                 # if log is saved on restraint, it can be deleted from server
                 # it avoids next test from detecting this failure
-                run(f"abrt-cli rm {directory}")
+                run(f'abrt-cli rm {directory}')
                 error = True
 
     if error:
-        print("FAIL: Found abrt error")
+        logging.error('Found abrt error')
         return False
 
-    print("PASS: no Abrt entry has been found.")
+    print('PASS: no Abrt entry has been found.')
     return True
 
 
 def kernel_check():  # noqa: ANN201
     """Check if kernel got tainted.
     It checks /proc/sys/kernel/tainted which returns a bitmask.
     The values are defined in the kernel source file include/linux/kernel.h,
@@ -131,172 +132,171 @@
     cd /usr/src/kernels/`uname -r`/
     Sources are provided by kernel-devel
     Returns:
     Boolean:
     True if did not find any issue
     False if found some issue.
     """
-    print("INFO: Checking for tainted kernel")
+    logging.info('Checking for tainted kernel')
 
-    previous_tainted_file = "/tmp/previous-tainted"
+    previous_tainted_file = '/tmp/previous-tainted'
 
-    tainted = run("cat /proc/sys/kernel/tainted", capture_output=True).output
+    tainted = run('cat /proc/sys/kernel/tainted').stdout
 
     tainted_val = int(tainted)
     if tainted_val == 0:
-        run("echo %d > %s" % (tainted_val, previous_tainted_file), verbose=False)
+        run('echo %d > %s' % (tainted_val, previous_tainted_file))
         return True
 
-    print("WARN: Kernel is tainted!")
+    logging.warning('Kernel is tainted!')
 
     if not Path(previous_tainted_file).is_file():
-        run(f"echo {tainted_val} > {previous_tainted_file}", verbose=False)
-    prev_taint = run(f"cat {previous_tainted_file}", capture_output=True).output
+        run(f'echo {tainted_val} > {previous_tainted_file}')
+    prev_taint = run(f'cat {previous_tainted_file}').stdout
     prev_taint_val = int(prev_taint)
     if prev_taint_val == tainted_val:
-        print("INFO: Kernel tainted has already been handled")
+        logging.info('Kernel tainted has already been handled')
         return True
 
-    run("echo %d > %s" % (tainted_val, previous_tainted_file), verbose=False)
+    run('echo %d > %s' % (tainted_val, previous_tainted_file))
 
     # check all bits that are set
     bit = 0
     while tainted_val != 0:
         # need to change back to int because it got changed to float at shifting
         tainted_val = int(tainted_val)
         if tainted_val & 1:
-            print("\tTAINT bit %d is set\n" % bit)
+            print('\tTAINT bit %d is set\n' % bit)
         bit += 1
         # shift tainted value
         tainted_val /= 2
     # List all tainted bits that are defined
-    print("List bit definition for tainted kernel")
-    run("cat /usr/src/kernels/`uname -r`/include/linux/kernel.h | grep TAINT_")
+    print('List bit definition for tainted kernel')
+    run('cat /usr/src/kernels/`uname -r`/include/linux/kernel.h | grep TAINT_')
 
     found_issue = False
     # try to find the module which tainted the kernel, tainted module have a mark between '('')'
-    output = run("cat /proc/modules | grep -e '(.*)' |  cut -d' ' -f1", capture_output=True).output
-    tainted_mods = output.split("\n")
+    output = run("cat /proc/modules | grep -e '(.*)' |  cut -d' ' -f1").stdout
+    tainted_mods = output.split('\n')
     # For example during iscsi async_events scst tool loads an unsigned module
     # just ignores it, so we will ignore this tainted if there is no tainted
     # modules loaded
     if not tainted_mods:
-        print("INFO: ignoring tainted as the module is not loaded anymore")
+        logging.info('ignoring tainted as the module is not loaded anymore')
     else:
         # ignore ocrdma due BZ#1334675
         # ignore nvme_fc and nvmet_fc due Tech Preview - BZ#1384922
-        ignore_modules = ["ocrdma", "nvme_fc", "nvmet_fc"]
+        ignore_modules = ['ocrdma', 'nvme_fc', 'nvmet_fc']
         for tainted_mod in tainted_mods:
             if tainted_mod:
-                print(f"INFO: The following module got tainted: {tainted_mod}")
-                run(f"modinfo {tainted_mod}")
+                logging.info(f'The following module got tainted: {tainted_mod}')
+                run(f'modinfo {tainted_mod}')
                 # due BZ#1334675  we are ignoring ocrdma module
                 if tainted_mod in ignore_modules:
-                    print(f"INFO: ignoring tainted on {tainted_mod}")
+                    logging.info(f'ignoring tainted on {tainted_mod}')
                     run(
-                        "echo %d > %s" % (tainted_val, previous_tainted_file),
-                        verbose=False,
+                        'echo %d > %s' % (tainted_val, previous_tainted_file),
                     )
                     continue
                 found_issue = True
 
-    run(f"echo {tainted} > {previous_tainted_file}", verbose=False)
+    run(f'echo {tainted} > {previous_tainted_file}')
     if found_issue:
         return False
 
     return True
 
 
 def _date2num(date):  # noqa: ANN001, ANN202
     date_map = {
-        "Jan": "1",
-        "Feb": "2",
-        "Mar": "3",
-        "Apr": "4",
-        "May": "5",
-        "Jun": "6",
-        "Jul": "7",
-        "Aug": "8",
-        "Sep": "9",
-        "Oct": "10",
-        "Nov": "11",
-        "Dec": "12",
+        'Jan': '1',
+        'Feb': '2',
+        'Mar': '3',
+        'Apr': '4',
+        'May': '5',
+        'Jun': '6',
+        'Jul': '7',
+        'Aug': '8',
+        'Sep': '9',
+        'Oct': '10',
+        'Nov': '11',
+        'Dec': '12',
     }
 
-    date_regex = r"(\S\S\S)\s(\d+)\s(\d\d:\d\d:\d\d)"
+    date_regex = r'(\S\S\S)\s(\d+)\s(\d\d:\d\d:\d\d)'
     m = re.match(date_regex, date)
     month = date_map[m.group(1)]
     day = str(m.group(2))
     # if day is a single digit, add '0' to begin
     if len(day) == 1:
-        day = "0" + day
+        day = '0' + day
 
     hour = m.group(3)
-    hour = hour.replace(":", "")
+    hour = hour.replace(':', '')
 
     return month + day + hour
 
 
 def messages_dump_check():  # noqa: ANN201
-    previous_time_file = "/tmp/previous-dump-check"
+    previous_time_file = '/tmp/previous-dump-check'
 
-    log_msg_file = "/var/log/messages"
+    log_msg_file = '/var/log/messages'
     if not Path(log_msg_file).is_file():
-        print(f"WARN: Could not open {log_msg_file}")
+        logging.warning(f'Could not open {log_msg_file}')
         return True
 
-    with Path(log_msg_file).open("rb") as log_file:
-        log = ""
+    with Path(log_msg_file).open('rb') as log_file:
+        log = ''
         try:
             for line in log_file.readlines():
-                log += line.decode("UTF-8")
+                log += line.decode('UTF-8')
         except UnicodeDecodeError:
-            log += line.decode("latin-1")
+            log += line.decode('latin-1')
 
-    begin_tag = "\\[ cut here \\]"
-    end_tag = "\\[ end trace "
+    begin_tag = '\\[ cut here \\]'
+    end_tag = '\\[ end trace '
 
     if not Path(previous_time_file).is_file():
-        first_time = "Jan 01 00:00:00"
+        first_time = 'Jan 01 00:00:00'
         time = _date2num(first_time)
-        run(f"echo {time} > {previous_time_file}")
+        run(f'echo {time} > {previous_time_file}')
 
     # Read the last time test ran
-    last_run = run(f"cat {previous_time_file}", capture_output=True).output
-    print(f"INFO: Checking for stack dump messages after: {last_run}")
+    last_run = run(f'cat {previous_time_file}').stdout
+    logging.info(f'Checking for stack dump messages after: {last_run}')
 
     # Going to search the file for text that matches begin_tag until end_tag
-    dump_regex = begin_tag + "(.*?)" + end_tag
+    dump_regex = begin_tag + '(.*?)' + end_tag
     m = re.findall(dump_regex, log, re.MULTILINE)
     if m:
-        print(f"INFO: Checking if it is newer than: {last_run}")
+        logging.info(f'Checking if it is newer than: {last_run}')
         print(m.group(1))
         # TODO
 
-    print("PASS: No recent dump messages has been found.")
+    print('PASS: No recent dump messages has been found.')
     return True
 
 
 def dmesg_check():  # noqa: ANN201
     """Check for error messages on dmesg ("Call Trace and segfault")."""
-    print("INFO: Checking for errors on dmesg.")
+    logging.info('Checking for errors on dmesg.')
     error = 0
     for msg in error_mgs:
-        output = run(f"dmesg | grep -i '{msg}'", capture_output=True).output
+        output = run(f"dmesg | grep -i '{msg}'").stdout
         if output:
-            print(f"FAIL: found {msg} on dmesg")
+            logging.error(f'found {msg} on dmesg')
             run(f"echo '\nINFO found {msg}  Saving it\n'>> dmesg.log")
-            run(f"dmesg >> {LOG_PATH}dmesg.log")
-            restraint.log_submit("dmesg.log")
+            run(f'dmesg >> {LOG_PATH}dmesg.log')
+            restraint.log_submit('dmesg.log')
             error = 1
     sts.linux.clear_dmesg()
     if error:
         return False
 
-    print("PASS: No errors on dmesg have been found.")
+    print('PASS: No errors on dmesg have been found.')
     return True
 
 
 def console_log_check():  # noqa: ANN201
     """Checks for error messages on console log ("Call Trace and segfault")."""
     if not beaker.is_beaker_job():
         # skip check
@@ -306,72 +306,72 @@
 
 def kdump_check():  # noqa: ANN201
     """Check for kdump error messages.
     It assumes kdump is configured on /var/crash.
     """
     error = 0
 
-    previous_kdump_check_file = "/tmp/previous-kdump-check"
-    kdump_dir = "/var/crash"
-    ret, hostname = run_ret_out("hostname", verbose=False, return_output=True)
+    previous_kdump_check_file = '/tmp/previous-kdump-check'
+    kdump_dir = '/var/crash'
+    ret, hostname = run_ret_out('hostname', return_output=True)
 
-    if not Path(f"{kdump_dir}/{hostname}").exists():
-        print("INFO: No kdump log found for this server")
+    if not Path(f'{kdump_dir}/{hostname}').exists():
+        logging.info('No kdump log found for this server')
         return True
 
     ret, output = run_ret_out(f"ls -l {kdump_dir}/{hostname} |  awk '{{print$9}}'", return_output=True)
-    kdumps = output.split("\n")
+    kdumps = output.split('\n')
     kdump_dates = []
     for kdump in kdumps:
         if not kdump:
             continue
         # parse on the date, remove the ip of the uploader
-        m = re.match(".*?-(.*)", kdump)
+        m = re.match('.*?-(.*)', kdump)
         if not m:
-            print(f"WARN: unexpected format for kdump ({kdump})")
+            logging.warning(f'unexpected format for kdump ({kdump})')
             continue
         date = m.group(1)
         # Old dump were using "."
-        date = date.replace(r"\.", "-")
+        date = date.replace(r'\.', '-')
         # replace last "-" with space to format date properly
-        index = date.rfind("-")
-        date = date[:index] + " " + date[index + 1 :]
-        print(f"INFO: Found kdump from {date}")
+        index = date.rfind('-')
+        date = date[:index] + ' ' + date[index + 1 :]
+        logging.info(f'Found kdump from {date}')
         kdump_dates.append(date)
 
     # checks if a file to store last run exists, if not create it
-    if not Path(f"{previous_kdump_check_file}").is_file():
+    if not Path(f'{previous_kdump_check_file}').is_file():
         # time in seconds
-        ret, time = run_ret_out(r"date +\"\%s\"", verbose=False, return_output=True)
-        run(f"echo -n {time} > {previous_kdump_check_file}", verbose=False)
-        print("INFO: kdump check is executing for the first time.")
-        print("INFO: doesn't know from which date should check files.")
-        print("PASS: Returning success.")
+        ret, time = run_ret_out(r'date +\"\%s\"', return_output=True)
+        run(f'echo -n {time} > {previous_kdump_check_file}')
+        logging.info('kdump check is executing for the first time.')
+        logging.info("doesn't know from which date should check files.")
+        print('PASS: Returning success.')
         return True
 
     # Read the last time test ran
-    ret, previous_check_time = run_ret_out(f"cat {previous_kdump_check_file}", return_output=True)
+    ret, previous_check_time = run_ret_out(f'cat {previous_kdump_check_file}', return_output=True)
     # just add new line to terminal because the file should not have already new line character
-    print("")
+    print('')
 
     for date in kdump_dates:
         # Note %% is escape form to use % in a string
         ret, kdump_time = run_ret_out('date --date="%s" +%%s' % date, return_output=True)
         if ret != 0:
-            print(f"WARN: Could not convert date {date}")
+            logging.warning(f'Could not convert date {date}')
             continue
 
         if not kdump_time:
             continue
         if int(kdump_time) > int(previous_check_time):
-            print(f"FAIL: Found a kdump log from {date} (more recent than {previous_check_time})")
-            print(f"FAIL: Check {kdump_dir}/{hostname}")
+            logging.error(f'Found a kdump log from {date} (more recent than {previous_check_time})')
+            logging.error(f'Check {kdump_dir}/{hostname}')
             error += 1
 
-    ret, time = run_ret_out(r"date +\"\%s\"", verbose=False, return_output=True)
-    run(f"echo -n {time} > {previous_kdump_check_file}", verbose=False)
+    ret, time = run_ret_out(r'date +\"\%s\"', return_output=True)
+    run(f'echo -n {time} > {previous_kdump_check_file}')
 
     if error:
         return False
 
-    print("PASS: No errors on kdump have been found.")
+    print('PASS: No errors on kdump have been found.')
     return True
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 """persistent_vars.py: Module to share variables between scripts using writing to file."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
 from pathlib import Path
 from typing import Any, Literal, Tuple, Union
 
 from sts.utils.cmdline import run
 
 
 def get_persistent_files_dir() -> str:
     """Returns directory of persistent vars."""
-    return "/var/tmp/"
+    return '/var/tmp/'
 
 
 def get_persistent_vars_file_name() -> str:
     """Returns file name of persistent vars file."""
-    return "FILE_NAMES"
+    return 'FILE_NAMES'
 
 
 def exists_persistent_vars_file() -> bool:
     """Returns True if persistent vars filer exists, default /tmp/FILE_NAMES."""
     return Path(get_persistent_files_dir() + get_persistent_vars_file_name()).exists()
 
 
 def _check_0_start(value) -> bool:  # noqa: ANN001
     """Checks if value starts with 0 but is not 0. This prevents from changing '02314' but allows changing '0'.
 
     Args:
       value (string): value to check
     """
-    return all([value.startswith("0"), value != "0"])
+    return all([value.startswith('0'), value != '0'])
 
 
 def _read_to_float(value: Union[str, Any]) -> Tuple[bool, Any]:
     """Args:
       value (Any, preferable string): Value to try to change to float.
 
     Returns:
       tuple: (False, original value) or (True, float(value))
     """
     try:
-        return (True, float(value)) if not all([_check_0_start(value), not value.startswith("0.")]) else (False, value)
+        return (True, float(value)) if not all([_check_0_start(value), not value.startswith('0.')]) else (False, value)
     except ValueError:
         return False, value
 
 
 def _read_to_int(value: Union[str, Any]) -> Tuple[bool, Any]:
     """Args:
       value (Any, preferable string): Value to try to change to integer.
@@ -66,16 +67,16 @@
     Args:
       value (Any, preferable string): Value to try to change to list
 
     Returns:
       tuple.: (False, original value) or (True, list(value))
     """
     try:
-        if value.startswith("["):
-            return True, value[1:-1].split(", ")
+        if value.startswith('['):
+            return True, value[1:-1].split(', ')
         else:  # noqa: RET505
             return False, value
     except AttributeError:
         return False, value
 
 
 def _read_to_none(value: Union[str, Any]) -> Tuple[bool, Any]:
@@ -95,31 +96,31 @@
 
     Args:
       value (Any, preferable string): Value to try to change to bool
 
     Returns:
       tuple.: (False, original value) or (True, True/False)
     """
-    if value.lower() == "true":
+    if value.lower() == 'true':
         return True, True
-    if value.lower() == "false":
+    if value.lower() == 'false':
         return True, False
     return False, value
 
 
 def _remove_quotes(value: str) -> str:
     """Removes any characters ' or " from any string.
 
     Args:
       value (string): Value to remove quotes from
 
     Returns:
       original string without quotes
     """
-    return "".join([char for char in value if char not in ["'", '"']])
+    return ''.join([char for char in value if char not in ["'", '"']])
 
 
 def recursive_read_value(value: str) -> Any:  # noqa: ANN401
     """Given string tries to change type of the string to different types. Returns value of new type of possible.
     Supported new types: list, int, float, None, bool
     Example: str("21654") changes to int(21654).
 
@@ -150,15 +151,15 @@
       var (string): variable name saved in file of the same name in get_persistent_files_dir() location.
 
     Returns:
       Any(_recursive_read_value): Value saved in the file with proper type
     """
     if not Path(get_persistent_files_dir() + var).is_file():
         if var != get_persistent_vars_file_name():
-            print(f"WARN: File {get_persistent_files_dir() + var} does not exist.")
+            logging.warning(f'File {get_persistent_files_dir() + var} does not exist.')
         return None
     with Path(get_persistent_files_dir() + var).open() as f:
         value = f.read()
     return recursive_read_value(value)
 
 
 def read_env(var: str) -> Any:  # noqa: ANN401
@@ -202,15 +203,15 @@
     """Args:
       var (dict): variable to write to file in format {var_name: var_value}.
 
     Returns:
       int: 0 pass, 1 fail
     """
     if not isinstance(var, dict):
-        print("FAIL: var manipulation requires var as a dict. {name: value}")
+        logging.error('var manipulation requires var as a dict. {name: value}')
         return 1
     file_name = list(var.keys()).pop()
     write_file(file_name, list(var.values()).pop())
     add_file_to_list(file_name)
     return 0
 
 
@@ -218,15 +219,15 @@
     """Args:
       file_name (string): File name to write to location get_persistent_files_dir() + file_name
       value: value to write to the file.
 
     Returns:
       None: None
     """
-    with Path(get_persistent_files_dir() + file_name).open("w") as f:
+    with Path(get_persistent_files_dir() + file_name).open('w') as f:
         for func in (_write_from_list, _write_to_string):
             ret, value_to_write = func(value)
             if ret:
                 break
         f.write(value_to_write)
 
 
@@ -254,43 +255,43 @@
     Returns:
       int.: 0
     """
     Path(get_persistent_files_dir() + var).unlink()
     return 0
 
 
-def clean_all_vars(prefix: str = "") -> Literal[0]:
+def clean_all_vars(prefix: str = '') -> Literal[0]:
     """This uses list of persistent vars files from get_persistent_files_dir() and get_persistent_vars_file_name() and
     cleans them from filesystem.
 
     Args:
       prefix (string): prefix to clean only some, for example "LSM_"
 
     Returns:
       int.: 0
     """
-    prefix = prefix or ""
+    prefix = prefix or ''
     variables = get_persistent_var_names(prefix)
     if exists_persistent_vars_file() and get_persistent_vars_file_name() not in variables:
         variables.append(get_persistent_vars_file_name())
-    print("INFO: Will clean these variables: \n\t%s" % "\n\t".join(variables))
+    logging.info(f'Will clean these variables: {variables}')
     for var in variables:
         clean_var(var)
     return 0
 
 
-def get_persistent_var_names(prefix: str = "") -> list:
+def get_persistent_var_names(prefix: str = '') -> list:
     """Gets persistent vars from get_persistent_vars_file_name() file
        or filesystem in get_persistent_files_dir() location.
 
     Args:
       prefix (string): prefix to clean only some, for example "LSM_"
 
     Returns:
       list.: List of persistent vars file names having the specified prefix
     """
     if exists_persistent_vars_file():
         variables = read_var(get_persistent_vars_file_name())
     else:
-        variables = run(f"ls -la {get_persistent_files_dir()}", capture_output=True, verbose=False).output
+        variables = run(f'ls -la {get_persistent_files_dir()}').stdout
         variables = [line.split().pop() for line in variables.splitlines()[3:]]
     return [value for value in variables if value.startswith(prefix)]
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/restraint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """restraint.py: Module to manage restraint."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
 from pathlib import Path
 
 from sts import linux
 from sts.utils.cmdline import run_ret_out
 
 
@@ -21,85 +22,78 @@
     """
     if not is_restraint_job():
         return False
 
     if not kill_time:
         kill_time = 1
 
-    result_server = os.environ["RESULT_SERVER"]
-    jobid = os.environ["RSTRNT_JOBID"]
-    test = os.environ["RSTRNT_TASKNAME"]
-    testid = os.environ["RSTRNT_TASKID"]
+    result_server = os.environ['RESULT_SERVER']
+    jobid = os.environ['RSTRNT_JOBID']
+    test = os.environ['RSTRNT_TASKNAME']
+    testid = os.environ['RSTRNT_TASKID']
 
     host = linux.hostname()
-    cmd = "rhts-test-checkin {} {} {} {} {} {}".format(
-        result_server,
-        host,
-        jobid,
-        test,
-        kill_time,
-        testid,
-    )
-    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
+    cmd = f'rhts-test-checkin {result_server} {host} {jobid} {test} {kill_time} {testid}'
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print("FAIL: Could not update beaker kill time")
+        logging.error('Could not update beaker kill time')
         print(output)
         return False
-    print("INFO: beaker_update_killtime() - Watchdog timer successfully updated to %d hours" % kill_time)
+    logging.info(f'beaker_update_killtime() - Watchdog timer successfully updated to {kill_time} hours')
     return True
 
 
 def log_submit(log_file):  # noqa: ANN001, ANN201
     """Upload log file."""
     if not is_restraint_job():
         return True
 
     if not log_file:
-        print("FAIL: log_submit() - requires log_file parameter")
+        logging.error('log_submit() - requires log_file parameter')
         return False
 
     if not Path(log_file).exists():
-        print(f"FAIL: log_submit() - file ({log_file}) does not exist")
+        logging.error(f'log_submit() - file ({log_file}) does not exist')
         return False
 
     cmd = f'rhts-submit-log -l "{log_file}"'
-    ret, output = run_ret_out(cmd, return_output=True, verbose=False)
+    ret, output = run_ret_out(cmd, return_output=True)
     if ret != 0:
-        print(f"FAIL: Could not upload log {log_file}")
+        logging.error(f'Could not upload log {log_file}')
         print(output)
         return False
-    print(f"INFO: log_submit() - {log_file} uploaded successfully")
+    logging.info(f'log_submit() - {log_file} uploaded successfully')
     return True
 
 
 def get_recipe_id():  # noqa: ANN201
     """Get current recipe id
     Parameter:
     None
     Return:
     recipe_id:          Restraint recipe id
     or
     None:               When not running using restraint.
     """
     if not is_restraint_job():
         return None
-    return os.environ["RSTRNT_RECIPEID"]
+    return os.environ['RSTRNT_RECIPEID']
 
 
 def get_task_id():  # noqa: ANN201
     """Get current task id
     Parameter:
     None
     Return:
     task_id:          Beaker task id
     or
     None:             Some error occurred.
     """
     if not is_restraint_job():
         return None
-    return os.environ["RSTRNT_TASKID"]
+    return os.environ['RSTRNT_TASKID']
 
 
 def is_restraint_job():  # noqa: ANN201
     """Checks if it is restraint job."""
-    need_env = ["RSTRNT_TASKNAME", "RSTRNT_TASKID"]
+    need_env = ['RSTRNT_TASKNAME', 'RSTRNT_TASKID']
     return all(not var not in os.environ for var in need_env)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/size.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """size.py: Module to convert human size <=> bytes."""
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import re
 
-size_human_regex = re.compile(r"([\-0-9\.]+)(Ki|Mi|Gi|Ti|Ei|Zi){0,1}B$")
+size_human_regex = re.compile(r'([\-0-9\.]+)(Ki|Mi|Gi|Ti|Ei|Zi){0,1}B$')
 
 
 def size_human_check(size_human):  # noqa: ANN001, ANN201
     size_human = str(size_human)
     m = size_human_regex.match(size_human)
     if not m:
-        print(f"FAIL: size_human_check() - incorrect number format {size_human}")
+        logging.error(f'size_human_check() - incorrect number format {size_human}')
         return False
     return True
 
 
 def size_human_2_size_bytes(size_human):  # noqa: ANN001, ANN201
     """Usage
         size_human_2_size_bytes(size_human)
@@ -28,42 +29,42 @@
         size_bytes     # like 1024.
     """
     if not size_human:
         return None
 
     # make sure size_human is a string, could be only numbers, for example
     size_human = str(size_human)
-    if not re.search(r"\d", size_human):
+    if not re.search(r'\d', size_human):
         # Need at least 1 digit
         return None
 
     m = size_human_regex.match(size_human)
     if not m:
-        if re.match(r"^\d+$", size_human):
+        if re.match(r'^\d+$', size_human):
             # Assume size is already in bytes
             return size_human
-        print(f"FAIL: '{size_human}' is an invalid human size format")
+        logging.error(f"'{size_human}' is an invalid human size format")
         return None
 
     fraction = 0
     # check if number is fractional
-    f = re.match(r"(\d+)\.(\d+)", m.group(1))
+    f = re.match(r'(\d+)\.(\d+)', m.group(1))
     if f:
         number = int(f.group(1))
         fraction = int(f.group(2))
     else:
         number = int(m.group(1))
 
     unit = m.group(2)
     if not unit:
-        unit = "B"
+        unit = 'B'
 
-    for valid_unit in ["B", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
+    for valid_unit in ['B', 'Ki', 'Mi', 'Gi', 'Ti', 'Pi', 'Ei', 'Zi']:
         if unit == valid_unit:
-            if unit == "B":
+            if unit == 'B':
                 # cut any fraction if was given, as it is not valid
                 return str(number)
             return int(number + fraction)
         number *= 1024
         fraction *= 1024
         fraction /= 10
     return int(number + fraction)
@@ -71,17 +72,17 @@
 
 def size_bytes_2_size_human(num):  # noqa: ANN001, ANN201
     if not num:
         return None
 
     # Even if we receive string we , so we can process it
     num = int(num)
-    for unit in ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB"]:
+    for unit in ['B', 'KiB', 'MiB', 'GiB', 'TiB', 'PiB', 'EiB', 'ZiB']:
         if abs(num) < 1024.0:
-            size_human = f"{num:3.1f}{unit}"
+            size_human = f'{num:3.1f}{unit}'
             # round it down removing decimal numbers
-            return re.sub(r"\.\d+", "", size_human)
+            return re.sub(r'\.\d+', '', size_human)
         num /= 1024.0
     # Very big number!!
-    size_human = f"{num:.1f}Yi"
+    size_human = f'{num:.1f}Yi'
     # round it down removing decimal numbers
-    return re.sub(r"\.\d+", "", size_human)
+    return re.sub(r'\.\d+', '', size_human)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.6.dev0/sts_libs/src/sts/utils/tmt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 """Test Management Tool related things."""
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import json
+import logging
 import tarfile
 import time
 from os import getenv
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
-from typing_extensions import TypedDict
-
-test_data_path = getenv("TMT_TEST_DATA")
+test_data_path = getenv('TMT_TEST_DATA')
 if not test_data_path:
     from uuid import uuid4
 
     dir_name = str(uuid4())
-    print(f"WARN: TMT_TEST_DATA env var not detected. Using '/var/tmp/{dir_name}'")
+    logging.warning(f"TMT_TEST_DATA env var not detected. Using '/var/tmp/{dir_name}'")
     test_data_path = dir_name
 
 TMT_TEST_DATA = Path(test_data_path)
 
 
 def gather_logs_from_dir(logs_path: str, name: Optional[str]) -> Union[Path, None]:
     path = Path(logs_path)
     if not path.is_dir():
         return None
     if not name:
-        name = str(path).replace("/", "_")
-    if ".tar" not in name:
-        name = f"{name}.tar"
+        name = str(path).replace('/', '_')
+    if '.tar' not in name:
+        name = f'{name}.tar'
 
-    tarfile_path = f"{TMT_TEST_DATA}/{name}"
-    with tarfile.open(tarfile_path, "w") as tar:
+    tarfile_path = f'{TMT_TEST_DATA}/{name}'
+    with tarfile.open(tarfile_path, 'w') as tar:
         tar.add(path, recursive=True)
     return Path(tarfile_path)
 
 
 def timestamp() -> float:
     return time.time()
 
 
 def calculate_duration(start: float, end: float) -> str:
     """Returns hh:mm:ss duration."""
     secs = int(end - start)
-    return f"{secs // 3600:02d}:{secs % 3600 // 60:02d}:{secs % 60:02d}"
+    return f'{secs // 3600:02d}:{secs % 3600 // 60:02d}:{secs % 60:02d}'
 
 
 class GuestType(TypedDict):
     name: Optional[str]
     role: Optional[str]
 
 
-TmtResult = Literal["pass", "fail", "info", "warn", "error"]
+TmtResult = Literal['pass', 'fail', 'info', 'warn', 'error']
 
 
 class CustomResults(TypedDict):
     name: str  # e.g. "/step-1" or "/setup/iscsi/target"
     result: TmtResult
     note: Optional[str]
     log: Optional[List[str]]  # path(s) to log file
@@ -80,16 +79,16 @@
 
     def __init__(self) -> None:
         self.results: List[Dict[str, Any]] = []
         self.timestamp = timestamp()
 
     def add(
         self,
-        name: str = "/",
-        result: Literal["pass", "fail", "info", "warn", "error"] = "pass",
+        name: str = '/',
+        result: Literal['pass', 'fail', 'info', 'warn', 'error'] = 'pass',
         note: Optional[str] = None,
         log: Optional[List[str]] = None,
         errors: Optional[List[str]] = None,
     ) -> None:
         """Add result to custom results list.
 
         When tmt plan is set to 'result: custom', use this followed by submit() to create the necessary result.json.
@@ -102,18 +101,18 @@
             results.submit()
 
         Args:
             name: Optional path-like string. e.g. '/setup/something' or 'setup'.
             log: Paths in the custom results file are treated as relative to ${TMT_TEST_DATA} path.
             errors: Can be used with atomic_run. If errors are not None, result is overwritten to "false".
         """
-        if not name.startswith("/"):
-            name = f"/{name}"
+        if not name.startswith('/'):
+            name = f'/{name}'
         if errors:
-            result = "fail"
+            result = 'fail'
         new_timestamp = timestamp()
         duration = calculate_duration(self.timestamp, new_timestamp)
         self.timestamp = new_timestamp
 
         result_to_add = CustomResults(
             name=name,
             result=result,
@@ -124,10 +123,10 @@
             serialnumber=None,
             guest=None,
         )
 
         self.results.append(remove_nones(result_to_add))
 
     def submit(self) -> None:
-        file = Path(TMT_TEST_DATA / "results.json")
-        with file.open("w") as f:
+        file = Path(TMT_TEST_DATA / 'results.json')
+        with file.open('w') as f:
             json.dump(self.results, f)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/cmdline_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/cmdline_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
-import io
-import sys
+import logging
 import unittest
 
 from sts.utils.cmdline import run, run_ret_out
 
 
 class TestCmdline(unittest.TestCase):
     def test_run_verbose(self) -> None:
-        test_msg = "run test message"
+        test_msg = 'run test message'
         # write to stderr, the message should be shown in the test
-        test_cmd = f"echo {test_msg} >&2"
-        running_string = f"Running command: '{test_cmd}'"
+        test_cmd = f'echo {test_msg} >&2'
+        verbose_log = f"INFO:root:Running command: '{test_cmd}'"
 
-        new_callable = io.StringIO()
-        sys.stdout = new_callable
-        # Default is verbose=True
-        assert run(test_cmd).returncode == 0
-        sys.stdout = sys.__stdout__
-        assert running_string in new_callable.getvalue().split("\n")[0]
-        assert test_msg in new_callable.getvalue().split("\n")[1]
-        sys.stdout = sys.__stdout__
-
-        # not verbose
-        new_callable = io.StringIO()
-        sys.stdout = new_callable
-        assert run(test_cmd, verbose=False).returncode == 0
-        sys.stdout = sys.__stdout__
-        assert new_callable.getvalue() == ""
-        sys.stdout = sys.__stdout__
+        logger = logging.getLogger()
+        with self.assertLogs(logger, level='INFO') as cm:
+            result = run(test_cmd)
+
+        assert result.rc == 0
+        assert verbose_log == cm.output[0]
 
     def test_run_return_output(self) -> None:
-        test_msg = "run test message"
-        test_cmd = f"echo {test_msg}"
-        ret_out = run(test_cmd, capture_output=True)
-        assert ret_out.returncode == 0
-        assert ret_out.output == test_msg
+        test_msg = 'run test message'
+        test_cmd = f'echo {test_msg}'
+        ret_out = run(test_cmd)
+        assert ret_out.rc == 0
+        assert ret_out.stdout == f'{test_msg}\n'
 
     def test_run_return_output_legacy(self) -> None:
-        test_msg = "run test message"
-        test_cmd = f"echo {test_msg}"
-        assert run_ret_out(test_cmd, return_output=True) == (0, test_msg)
+        test_msg = 'run test message'
+        test_cmd = f'echo {test_msg}'
+        assert run_ret_out(test_cmd, return_output=True) == (0, f'{test_msg}\n')
 
     def test_run_fail_return_output(self) -> None:
         failure_msg = "ls: cannot access 'invalid_file': No such file or directory"
-        test_cmd = "ls invalid_file"
-        ret_out = run(test_cmd, capture_output=True)
-        assert ret_out.returncode == 2
-        assert ret_out.output == failure_msg
+        test_cmd = 'ls invalid_file'
+        ret_out = run(test_cmd)
+        assert ret_out.rc == 2
+        assert ret_out.stderr == f'{failure_msg}\n'
 
     def test_run_fail_return_output_legacy(self) -> None:
         failure_msg = "ls: cannot access 'invalid_file': No such file or directory"
-        test_cmd = "ls invalid_file"
-        assert run_ret_out(test_cmd, return_output=True) == (2, failure_msg)
-
-    def test_run_timeout(self) -> None:
-        test_cmd = "sleep 9"
-        expected_retcode = 124
-        assert run(test_cmd, timeout=1).returncode == expected_retcode
-
-    def test_run_timeout_legacy(self) -> None:
-        test_cmd = "sleep 9"
-        expected_retcode = 124
-        assert run_ret_out(test_cmd, return_output=True, timeout=1) == (expected_retcode, None)
+        test_cmd = 'ls invalid_file'
+        assert run_ret_out(test_cmd, return_output=True) == (2, f'{failure_msg}\n')
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/fio_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/fio_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
 import os
 from pathlib import Path
 
 import pytest
 
 from sts import fio
 from sts.utils.cmdline import run
 
 
 def test_fio() -> None:
     if not fio.install_fio():
-        pytest.fail("Unable to install fio")
+        pytest.fail('Unable to install fio')
 
-    output_file = "fio.test"
+    output_file = 'fio.test'
 
     # Create a file big enough to use by FIO
-    run(f"dd if=/dev/zero of={output_file} count=20 bs=1024k")
+    run(f'dd if=/dev/zero of={output_file} count=20 bs=1024k')
 
     try:
-        fio_pid = fio.fio_stress_background(output_file, size="1m")
+        fio_pid = fio.fio_stress_background(output_file, size='1m')
     except Exception as e:
-        pytest.fail(f"FAIL: Exception: {e}")
+        pytest.fail(f'FAIL: Exception: {e}')
 
     # Make sure background process does not generate exception
-    print("INFO: Waiting FIO process to finish")
+    logging.info('Waiting FIO process to finish')
     try:
         _, exit_status = os.waitpid(fio_pid, 0)
     except Exception as e:
-        pytest.fail(f"FAIL: Exception: {e}")
+        pytest.fail(f'FAIL: Exception: {e}')
 
     if exit_status != 0:
-        pytest.fail("FAIL: there was some error running FIO")
+        pytest.fail('FAIL: there was some error running FIO')
     try:
         Path(output_file).unlink()
     except Exception:
-        pytest.fail(f"FAIL: Could not delete {output_file}")
+        pytest.fail(f'FAIL: Could not delete {output_file}')
 
     assert 1
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/iscsi_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 from unittest.mock import patch
 
 import pytest
+from testinfra.backend.base import CommandResult
 
 from sts import iscsi
 
-target = "localhost"
+target = 'localhost'
 
 
 def test_install_initiator() -> None:
     if not iscsi.install():
-        pytest.fail("FAIL: Could not install iSCSI initiator package")
+        pytest.fail('FAIL: Could not install iSCSI initiator package')
     assert 1
 
 
-@patch("sts.iscsi.run_ret_out")
-def test_query_discovery(iscsi_run_func) -> None:  # noqa: ANN001
-    discovery_output = """
-SENDTARGETS:
-DiscoveryAddress: localhost,3260
-Target: iqn.2009-10.com.redhat:storage-0
-    Portal: [::1]:3260,1
-        Iface Name: default
-iSNS:
-No targets found.
-STATIC:
-No targets found.
-FIRMWARE:
-No targets found.
-"""
-    iscsi_run_func.return_value = (0, discovery_output)
+def test_query_discovery(monkeypatch) -> None:  # noqa: ANN001
+    discovery_output = (
+        'SENDTARGETS:\nDiscoveryAddress: 172.16.0.10,3260\nTarget: '
+        'iqn.2002-03.com.compellent:test-0\n\tPortal: 172.16.0.10:3260,0\n\t\tIface Name: '
+        'qedi.00:0e:1e:f1:9c:f0\nTarget: iqn.2002-03.com.compellent:test-1\n\tPortal: '
+        '172.16.0.10:3260,0\n\t\tIface Name: qedi.00:0e:1e:f1:9c:f0\niSNS:\nNo targets '
+        'found.\nSTATIC:\nNo targets found.\nFIRMWARE:\nNo targets found.\n'
+    )
+    monkeypatch.setattr(CommandResult, 'failed', False)
+    monkeypatch.setattr(CommandResult, 'stdout', discovery_output)
 
     expected_ret = {
-        "SENDTARGETS": {
-            "localhost,3260": {
-                "disc_addr": "localhost",
-                "disc_port": "3260",
-                "mode": "sendtargets",
-                "targets": {
-                    "iqn.2009-10.com.redhat:storage-0": {
-                        "portal": {"address": "[::1]", "port": "3260"},
-                        "iface": ["default"],
+        'SENDTARGETS': {
+            '172.16.0.10,3260': {
+                'disc_addr': '172.16.0.10',
+                'disc_port': '3260',
+                'mode': 'sendtargets',
+                'targets': {
+                    'iqn.2002-03.com.compellent:test-0': {
+                        'portal': {
+                            'address': '172.16.0.10',
+                            'port': '3260',
+                        },
+                        'iface': ['qedi.00:0e:1e:f1:9c:f0'],
+                    },
+                    'iqn.2002-03.com.compellent:test-1': {
+                        'portal': {'address': '172.16.0.10', 'port': '3260'},
+                        'iface': ['qedi.00:0e:1e:f1:9c:f0'],
                     },
                 },
             },
         },
-        "iSNS": {},
-        "STATIC": {},
-        "FIRMWARE": {},
+        'iSNS': {},
+        'STATIC': {},
+        'FIRMWARE': {},
     }
+
     assert iscsi.query_discovery() == expected_ret
 
 
-@patch("sts.iscsi.run_ret_out")
-def test_discovery(iscsi_run_func) -> None:  # noqa: ANN001
-    discovery_output = "[::1]:3260,1 iqn.2009-10.com.redhat:storage-0"
-    iscsi_run_func.return_value = (0, discovery_output)
+def test_discovery(monkeypatch) -> None:  # noqa: ANN001
+    discovery_output = '[::1]:3260,1 iqn.2009-10.com.redhat:storage-0'
+    monkeypatch.setattr(CommandResult, 'failed', False)
+    monkeypatch.setattr(CommandResult, 'stdout', discovery_output)
 
     if not iscsi.discovery_st(target):
-        pytest.fail("FAIL: Could not discovery iSCSI target")
+        pytest.fail('FAIL: Could not discover iSCSI target')
     assert 1
 
 
-@patch("sts.linux.service_restart")
+@patch('sts.linux.service_restart')
 def test_set_iscsid_parameter(service_restart_func) -> None:  # noqa: ANN001
     service_restart_func.return_value = True
-    if not iscsi.set_iscsid_parameter({"node.session.cmds_max": "4096", "node.session.queue_depth": "128"}):
-        pytest.fail("FAIL: Unable to set iscsid parameter")
+    if not iscsi.set_iscsid_parameter({'node.session.cmds_max': '4096', 'node.session.queue_depth': '128'}):
+        pytest.fail('FAIL: Unable to set iscsid parameter')
     assert 1
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/linux_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/linux_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,119 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
+import logging
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
 
 from sts import linux, scsi_debug
 
 
 def test_os_info():  # noqa: ANN201
     os_info = linux.query_os_info()
     if not os_info:
-        pytest.fail("FAIL: Could not query OS info")
+        pytest.fail('FAIL: Could not query OS info')
 
     for info in os_info:
-        print(f"{info}: {os_info[info]}")
+        print(f'{info}: {os_info[info]}')
     assert 1
 
 
 def test_using_scsi_debug():  # noqa: ANN201
-    if linux.is_docker():
-        print("SKIP: Cannot create scsi_debug in container")
+    if linux.in_container():
+        logging.info('SKIP: Cannot create scsi_debug in container')
         return
     if not scsi_debug.scsi_debug_load_module():
-        pytest.fail("FAIL: loading scsi_debug module")
+        pytest.fail('FAIL: loading scsi_debug module')
 
     device = scsi_debug.get_scsi_debug_devices()[-1]
 
     if linux.get_parent_device(device) != device:  # scsi_debug does not have parent
-        pytest.fail("FAIL: get_parent_device using scsi_debug")
-    if linux.get_full_path(device) != f"/dev/{device}":
-        pytest.fail("FAIL: get_full_path using scsi_debug")
+        pytest.fail('FAIL: get_parent_device using scsi_debug')
+    if linux.get_full_path(device) != f'/dev/{device}':
+        pytest.fail('FAIL: get_full_path using scsi_debug')
     wwid = linux.get_device_wwid(device)
     if not wwid:
-        pytest.fail("FAIL: get_device_wwid using scsi_debug")
-    if linux.get_udev_property(device, "ID_MODEL") != "scsi_debug":
-        pytest.fail("FAIL: device ID_MODEL should be 'scsi_debug'")
+        pytest.fail('FAIL: get_device_wwid using scsi_debug')
+    if linux.get_udev_property(device, 'ID_MODEL') != 'scsi_debug':
+        pytest.fail("FAIL: device ID_MODEL should be 'scsi_debug")
     if linux.is_dm_device(device):
-        pytest.fail("FAIL: scsi_debug device should not be mapped by DM")
+        pytest.fail('FAIL: scsi_debug device should not be mapped by DM')
 
     if not scsi_debug.scsi_debug_unload_module():
-        pytest.fail("FAIL: loading scsi_debug module")
+        pytest.fail('FAIL: loading scsi_debug module')
     assert 1
 
 
 def test_get_boot_device():  # noqa: ANN201
     get_boot = linux.get_boot_device()
-    if get_boot is None and linux.is_docker() is False:
+    if get_boot is None and linux.in_container() is False:
         pytest.fail("FAIL: Could not find '/boot' and '/'! ")
-    print(f"INFO: Boot device is: {get_boot}")
+    logging.info(f'Boot device is: {get_boot}')
     assert 1
 
 
 def test_get_dist_release():  # noqa: ANN201
     release = linux.dist_release()
     if not release:
-        pytest.fail("FAIL: Could not find distribution release")
+        pytest.fail('FAIL: Could not find distribution release')
 
 
 def test_get_dist_ver():  # noqa: ANN201
     version = linux.dist_ver()
     if not version:
-        pytest.fail("FAIL: Could not find distribution version")
+        pytest.fail('FAIL: Could not find distribution version')
 
 
 def test_get_dist_name():  # noqa: ANN201
     name = linux.dist_name()
     if not name:
-        pytest.fail("FAIL: Could not find distribution name")
+        pytest.fail('FAIL: Could not find distribution name')
 
 
-@patch("sts.linux.download_repo_file")
+@patch('sts.linux.download_repo_file')
 def test_rpm_repo(get_mock):  # noqa: ANN001, ANN201
     content = """[test-fedora-debuginfo]
 name=testrepo
 #baseurl=http://download.example/pub/fedora/linux/releases/$releasever/Everything/$basearch/debug/tree/
 metalink=https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch
 enabled=1
 repo_gpgcheck=0
 type=rpm
 skip_if_unavailable=False
 """
 
     def create_repo_file(_):  # noqa: ANN001, ANN202
-        with Path("/etc/yum.repos.d/test2.repo").open("w") as f:
+        with Path('/etc/yum.repos.d/test2.repo').open('w') as f:
             f.write(content)
 
     get_mock.side_effect = create_repo_file
-    repo_metalink = "https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch"
-    repo_url = "https://testurl.com/test.repo"
-    repo_name = "testrepo"
-    linux.add_repo("test1", repo_metalink, metalink=True)
-    if not linux.check_repo("test1"):
-        pytest.fail("FAIL: Created repo is not working")
-    if not linux.del_repo("test1"):
-        pytest.fail("FAIL: Unable to delete repo")
+    repo_metalink = 'https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch'
+    repo_url = 'https://testurl.com/test.repo'
+    repo_name = 'testrepo'
+    linux.add_repo('test1', repo_metalink, metalink=True)
+    if not linux.check_repo('test1'):
+        pytest.fail('FAIL: Created repo is not working')
+    if not linux.del_repo('test1'):
+        pytest.fail('FAIL: Unable to delete repo')
     linux.download_repo_file(repo_url)
     if not linux.check_repo(repo_name):
-        pytest.fail("FAIL: Test repo is not working")
-    if not linux.del_repo("test2"):
-        pytest.fail("FAIL: Unable to delete repo")
-    if Path("/etc/yum.repos.d/test2.repo").exists():
-        pytest.fail("FAIL: repo file should have been deleted")
+        pytest.fail('FAIL: Test repo is not working')
+    if not linux.del_repo('test2'):
+        pytest.fail('FAIL: Unable to delete repo')
+    if Path('/etc/yum.repos.d/test2.repo').exists():
+        pytest.fail('FAIL: repo file should have been deleted')
 
 
-@patch("sts.linux.run")
+@patch('sts.linux.run')
 def test_is_mounted(run_func):  # noqa: ANN001, ANN201
     run_func.return_value = 0
-    if not linux.is_mounted("testdev"):
-        pytest.fail("FAIL: device should have been mounted")
-    if not linux.is_mounted(mountpoint="testdir"):
-        pytest.fail("FAIL: mountpoint should have been mounted")
+    if not linux.is_mounted('testdev'):
+        pytest.fail('FAIL: device should have been mounted')
+    if not linux.is_mounted(mountpoint='testdir'):
+        pytest.fail('FAIL: mountpoint should have been mounted')
     run_func.return_value = 1
-    if linux.is_mounted("testdev"):
-        pytest.fail("FAIL: device should NOT have been mounted")
-    if linux.is_mounted(mountpoint="testdir"):
-        pytest.fail("FAIL: mountpoint should NOT have been mounted")
+    if linux.is_mounted('testdev'):
+        pytest.fail('FAIL: device should NOT have been mounted')
+    if linux.is_mounted(mountpoint='testdir'):
+        pytest.fail('FAIL: mountpoint should NOT have been mounted')
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/logchecker_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,74 +5,74 @@
 from unittest.mock import call, patch
 
 import sts.utils.logchecker as log_checker
 from sts.utils.cmdline import run
 
 # found segfault
 segfault_msg = (
-    " segfault at 10 ip 00007f9bebcca90d sp 00007fffb62705f0 error 4 in libQtWebKit.so.4.5.2[7f9beb83a000+f6f000]"
+    ' segfault at 10 ip 00007f9bebcca90d sp 00007fffb62705f0 error 4 in libQtWebKit.so.4.5.2[7f9beb83a000+f6f000]'
 )
-calltrace_msg = " Call Trace: "
+calltrace_msg = ' Call Trace: '
 
 
 def _run_dmesg_segfault(cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
-    if cmd.startswith("dmesg | grep"):
-        cmd = cmd.replace("dmesg", f"echo '{segfault_msg}'")
-        return run(cmd, verbose=False, **kwargs)
+    if cmd.startswith('dmesg | grep'):
+        cmd = cmd.replace('dmesg', f"echo '{segfault_msg}'")
+        return run(cmd, **kwargs)
 
-    return 0, ""
+    return 0, ''
 
 
 def _run_dmesg_calltrace(cmd, **kwargs):  # noqa: ANN001, ANN003, ANN202
-    if cmd.startswith("dmesg | grep"):
-        cmd = cmd.replace("dmesg", f"echo '{calltrace_msg}'")
-        return run(cmd, verbose=False, **kwargs)
+    if cmd.startswith('dmesg | grep'):
+        cmd = cmd.replace('dmesg', f"echo '{calltrace_msg}'")
+        return run(cmd, **kwargs)
 
-    return 0, ""
+    return 0, ''
 
 
 class Testlogchecker(unittest.TestCase):
-    @patch("sts.utils.logchecker.run")
+    @patch('sts.utils.logchecker.run')
     def test_kernel_check(self, run_func):  # noqa: ANN001, ANN201
-        run_func.return_value.returncode = 0
-        run_func.return_value.output = "0"
+        run_func.return_value.rc = 0
+        run_func.return_value.stdout = '0'
         assert log_checker.kernel_check() is True
         # already handled taint
-        run_func.return_value.returncode = 0
-        run_func.return_value.output = "1"
+        run_func.return_value.rc = 0
+        run_func.return_value.stdout = '1'
         assert log_checker.kernel_check() is True
 
-    @patch("sts.utils.logchecker.run")
+    @patch('sts.utils.logchecker.run')
     def test_dmesg_check(self, run_func):  # noqa: ANN001, ANN201
-        run_func.return_value.returncode = 0
-        run_func.return_value.output = ""
+        run_func.return_value.rc = 0
+        run_func.return_value.stdout = ''
         assert log_checker.dmesg_check() is True
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_segfault
         assert log_checker.dmesg_check() is False
         run_calls = [
-            call("dmesg | grep -i ' segfault '", capture_output=True),
+            call("dmesg | grep -i ' segfault '"),
             call("echo '\nINFO found  segfault   Saving it\n'>> dmesg.log"),
-            call("dmesg >> ./dmesg.log"),
-            call("dmesg | grep -i 'Call Trace:'", capture_output=True),
+            call('dmesg >> ./dmesg.log'),
+            call("dmesg | grep -i 'Call Trace:'"),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
 
         run_func.side_effect = _run_dmesg_calltrace
         assert log_checker.dmesg_check() is False
         run_calls = [
-            call("dmesg | grep -i ' segfault '", capture_output=True),
-            call("dmesg | grep -i 'Call Trace:'", capture_output=True),
+            call("dmesg | grep -i ' segfault '"),
+            call("dmesg | grep -i 'Call Trace:'"),
             call("echo '\nINFO found Call Trace:  Saving it\n'>> dmesg.log"),
-            call("dmesg >> ./dmesg.log"),
+            call('dmesg >> ./dmesg.log'),
         ]
         # print(run_func.call_args_list)
         run_func.assert_has_calls(run_calls)
         run_func.reset_mock()
 
-    @patch("sts.utils.logchecker.kernel_check")
+    @patch('sts.utils.logchecker.kernel_check')
     def test_check_all(self, check_func):  # noqa: ANN001, ANN201
         check_func.return_value = False
         assert log_checker.check_all() is False
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/lvm_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,77 +4,77 @@
 import unittest
 from unittest.mock import patch
 
 from sts import lvm
 
 
 class TestPV(unittest.TestCase):
-    pvs_output = "  /dev/vda1,lvm_test,lvm2,a--,98.41g,0"
+    pvs_output = '  /dev/vda1,lvm_test,lvm2,a--,98.41g,0'
     pv_query_output = {  # noqa: RUF012
-        "/dev/vda1": {
-            "vg": "lvm_test",
-            "fmt": "lvm2",
-            "attr": "a--",
-            "psize": "98.41g",
-            "pfree": "0",
+        '/dev/vda1': {
+            'vg': 'lvm_test',
+            'fmt': 'lvm2',
+            'attr': 'a--',
+            'psize': '98.41g',
+            'pfree': '0',
         },
     }
 
     def test_pv_query(self) -> None:
-        with patch("sts.lvm.run_ret_out") as run_func:
+        with patch('sts.lvm.run_ret_out') as run_func:
             run_func.return_value = [0, self.pvs_output]
             assert self.pv_query_output == lvm.pv_query()
 
     def test_pv_create(self) -> None:
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 0
-            assert lvm.pv_create("/dev/vda1")
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 1
-            assert not lvm.pv_create("/dev/vda1")
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 0
+            assert lvm.pv_create('/dev/vda1')
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 1
+            assert not lvm.pv_create('/dev/vda1')
 
-    @patch("sts.lvm.pv_query")
+    @patch('sts.lvm.pv_query')
     def test_pv_remove(self, mock):  # noqa: ANN001, ANN201
         mock.return_value = self.pv_query_output
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 0
-            assert lvm.pv_remove("/dev/vda1")
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 1
-            assert not lvm.pv_remove("/dev/vda1")
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 0
+            assert lvm.pv_remove('/dev/vda1')
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 1
+            assert not lvm.pv_remove('/dev/vda1')
 
 
 class TestVG(unittest.TestCase):
-    vgs_output = "  lvm_test,1,3,0,wz--n-,98.41g,0"
+    vgs_output = '  lvm_test,1,3,0,wz--n-,98.41g,0'
     vg_query_output = {  # noqa: RUF012
-        "lvm_test": {
-            "num_pvs": "1",
-            "num_lvs": "3",
-            "num_sn": "0",
-            "attr": "wz--n-",
-            "vsize": "98.41g",
-            "vfree": "0",
+        'lvm_test': {
+            'num_pvs': '1',
+            'num_lvs': '3',
+            'num_sn': '0',
+            'attr': 'wz--n-',
+            'vsize': '98.41g',
+            'vfree': '0',
         },
     }
 
     def test_vg_query(self) -> None:
-        with patch("sts.lvm.run_ret_out") as run_func:
+        with patch('sts.lvm.run_ret_out') as run_func:
             run_func.return_value = [0, self.vgs_output]
             assert self.vg_query_output == lvm.vg_query()
 
     def test_pv_create(self) -> None:
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 0
-            assert lvm.vg_create("lvm_test", "/dev/vda1")
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 1
-            assert not lvm.vg_create("lvm_test", "/dev/vda1")
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 0
+            assert lvm.vg_create('lvm_test', '/dev/vda1')
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 1
+            assert not lvm.vg_create('lvm_test', '/dev/vda1')
 
-    @patch("sts.lvm.pv_query")
+    @patch('sts.lvm.pv_query')
     def test_pv_remove(self, mock):  # noqa: ANN001, ANN201
         mock.return_value = self.vg_query_output
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 0
-            assert lvm.pv_remove("lvm_test")
-        with patch("sts.lvm.run") as run_func:
-            run_func.return_value.returncode = 1
-            assert not lvm.pv_remove("lvm_test")
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 0
+            assert lvm.pv_remove('lvm_test')
+        with patch('sts.lvm.run') as run_func:
+            run_func.return_value.rc = 1
+            assert not lvm.pv_remove('lvm_test')
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/md_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/md_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,99 +41,99 @@
 
     Number   Major   Minor   RaidDevice State
        0       7        0        0      active sync   /dev/sda
        1       7        1        1      inactive      /dev/sdb1
 """
 
 md0_info = {
-    "version": "1.2",
-    "creation_time": "Fri Nov 18 04:15:54 2022",
-    "raid_level": "raid0",
-    "array_size": "2093056 (2044.00 MiB 2143.29 MB)",
-    "raid_devices": "2",
-    "total_devices": "2",
-    "persistence": "Superblock is persistent",
-    "update_time": "Fri Nov 18 04:15:54 2022",
-    "state": "clean",
-    "active_devices": "2",
-    "working_devices": "2",
-    "failed_devices": "0",
-    "spare_devices": "0",
-    "layout": "-unknown-",
-    "chunk_size": "512K",
-    "name": "0",
-    "uuid": "05f704a3:70531edf:80b2414a:0de2efad",
-    "events": "0",
-    "storage_devices": {
-        "/dev/sda": {
-            "number": "0",
-            "major": "7",
-            "minor": "0",
-            "raid_device": "0",
-            "state": "active sync",
+    'version': '1.2',
+    'creation_time': 'Fri Nov 18 04:15:54 2022',
+    'raid_level': 'raid0',
+    'array_size': '2093056 (2044.00 MiB 2143.29 MB)',
+    'raid_devices': '2',
+    'total_devices': '2',
+    'persistence': 'Superblock is persistent',
+    'update_time': 'Fri Nov 18 04:15:54 2022',
+    'state': 'clean',
+    'active_devices': '2',
+    'working_devices': '2',
+    'failed_devices': '0',
+    'spare_devices': '0',
+    'layout': '-unknown-',
+    'chunk_size': '512K',
+    'name': '0',
+    'uuid': '05f704a3:70531edf:80b2414a:0de2efad',
+    'events': '0',
+    'storage_devices': {
+        '/dev/sda': {
+            'number': '0',
+            'major': '7',
+            'minor': '0',
+            'raid_device': '0',
+            'state': 'active sync',
         },
-        "/dev/sdb1": {
-            "number": "1",
-            "major": "7",
-            "minor": "1",
-            "raid_device": "1",
-            "state": "inactive",
+        '/dev/sdb1': {
+            'number': '1',
+            'major': '7',
+            'minor': '1',
+            'raid_device': '1',
+            'state': 'inactive',
         },
     },
 }
 
 
 class TestMD(unittest.TestCase):
-    @patch("sts.md.run_ret_out")
+    @patch('sts.md.run_ret_out')
     def test_md_query(self, run_func):  # noqa: ANN001, ANN201
         run_func.return_value = (0, mdstat_output)
 
-        assert md.md_query() == ["md0"]
+        assert md.md_query() == ['md0']
 
         assert run_func.call_count == 1
-        run_calls = [call("cat /proc/mdstat", return_output=True, verbose=False)]
+        run_calls = [call('cat /proc/mdstat', return_output=True)]
         run_func.assert_has_calls(run_calls)
 
-    @patch("sts.md._mdadm_query")
-    @patch("sts.md.md_query")
+    @patch('sts.md._mdadm_query')
+    @patch('sts.md.md_query')
     def test_md_get_info(self, md_query_func, mdadm_query_func):  # noqa: ANN001, ANN201
-        md_query_func.return_value = ["md0"]
+        md_query_func.return_value = ['md0']
         mdadm_query_func.return_value = mdadm_output
 
-        assert md.md_get_info("md0", verbose=True) == md0_info
+        assert md.md_get_info('md0') == md0_info
 
-    @patch("sts.md.md_get_info")
+    @patch('sts.md.md_get_info')
     def test_md_get_storage_dev(self, md_get_info_func):  # noqa: ANN001, ANN201
         md_get_info_func.return_value = md0_info
 
-        storage_devs = md.md_get_storage_dev("md0")
-        assert "/dev/sda" in storage_devs
-        assert "/dev/sdb1" in storage_devs
+        storage_devs = md.md_get_storage_dev('md0')
+        assert '/dev/sda' in storage_devs
+        assert '/dev/sdb1' in storage_devs
 
-    @patch("sts.md.run_ret_out")
+    @patch('sts.md.run_ret_out')
     def test_md_stop(self, run_func):  # noqa: ANN001, ANN201
-        run_func.return_value = (0, "")
-        assert md.md_stop("md0")
-        run_calls = [call("mdadm --stop /dev/md0", return_output=True, verbose=False)]
+        run_func.return_value = (0, '')
+        assert md.md_stop('md0')
+        run_calls = [call('mdadm --stop /dev/md0', return_output=True)]
         run_func.assert_has_calls(run_calls)
 
-    @patch("sts.md.run_ret_out")
+    @patch('sts.md.run_ret_out')
     def test_md_clean(self, run_func):  # noqa: ANN001, ANN201
-        run_func.return_value = (0, "")
-        assert md.md_clean("/dev/sda")
-        run_calls = [call("mdadm --zero-superblock /dev/sda", return_output=True, verbose=False)]
+        run_func.return_value = (0, '')
+        assert md.md_clean('/dev/sda')
+        run_calls = [call('mdadm --zero-superblock /dev/sda', return_output=True)]
         run_func.assert_has_calls(run_calls)
 
-    @patch("sts.md.run_ret_out")
-    @patch("sts.md.md_stop")
-    @patch("sts.md.md_get_storage_dev")
+    @patch('sts.md.run_ret_out')
+    @patch('sts.md.md_stop')
+    @patch('sts.md.md_get_storage_dev')
     def test_md_remove(self, get_sto_func, md_stop_func, run_func):  # noqa: ANN001, ANN201
-        run_func.return_value = (0, "")
+        run_func.return_value = (0, '')
         md_stop_func.return_value = True
-        get_sto_func.return_value = ["/dev/sda1", "/dev/sdb1"]
-        assert md.md_remove("md0", clean=True)
+        get_sto_func.return_value = ['/dev/sda1', '/dev/sdb1']
+        assert md.md_remove('md0', clean=True)
         run_calls = [
-            call("mdadm --remove /dev/md0", return_output=True, verbose=False),
-            call("mdadm --zero-superblock /dev/sda1", return_output=True, verbose=False),
-            call("mdadm --zero-superblock /dev/sdb1", return_output=True, verbose=False),
+            call('mdadm --remove /dev/md0', return_output=True),
+            call('mdadm --zero-superblock /dev/sda1', return_output=True),
+            call('mdadm --zero-superblock /dev/sdb1', return_output=True),
         ]
         run_func.assert_has_calls(run_calls)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/net_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/net_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import unittest
 from unittest.mock import patch
 
 from sts import net
-from sts.linux import is_docker
 
-MAC = "7E:CD:60:1E:AC:6E"
-NOTMAC = "7E:CD:60:1E:AC"
-BADMAC = "7ecd.601e.ac6e"
-LOWMAC = "7e:cd:60:1e:ac:6e"
-NOTVALID = "ThisIsNotValid"
-LOCALHOST = "127.0.0.1"
-NETMASK24 = "255.255.255.0"
-CIDR24 = "24"
-NOTIP = "256.256.256.256"
-IPV6 = "fd6f:60d2:2d9:0:b7e:b6e6:7bf5:c17e"
+MAC = '7E:CD:60:1E:AC:6E'
+NOTMAC = '7E:CD:60:1E:AC'
+BADMAC = '7ecd.601e.ac6e'
+LOWMAC = '7e:cd:60:1e:ac:6e'
+NOTVALID = 'ThisIsNotValid'
+LOCALHOST = '127.0.0.1'
+NETMASK24 = '255.255.255.0'
+CIDR24 = '24'
+NOTIP = '256.256.256.256'
+IPV6 = 'fd6f:60d2:2d9:0:b7e:b6e6:7bf5:c17e'
 
 
 class TestNet(unittest.TestCase):
     def test_is_mac(self) -> None:
         assert net.is_mac(MAC)
         assert not net.is_mac(NOTMAC)
 
@@ -32,21 +31,16 @@
         assert net.get_mac_of_nic(net.get_nics()[-1]) is not None
 
     def test_get_nic_of_mac(self) -> None:
         assert net.get_nic_of_mac(MAC) is None
         assert net.get_nic_of_mac(net.get_mac_of_nic(net.get_nics()[-1])) is not None
 
     def test_get_ip_address_of_nic(self) -> None:
-        assert net.get_ip_address_of_nic(NOTVALID) is None
-        assert net.get_ip_address_of_nic(net.get_nics()[-1]) is not None
-
-    def test_get_ipv6_address_of_nic(self) -> None:
-        assert net.get_ipv6_address_of_nic(NOTVALID) is None
-        if not is_docker():
-            assert net.get_ipv6_address_of_nic(net.get_nics()[-1]) is not None
+        assert net.get_ip_addresses_of_nic(NOTVALID) is None
+        assert net.get_ip_addresses_of_nic(net.get_nics()[-1]) is not None
 
     def test_get_nic_of_ip(self) -> None:
         assert net.get_nic_of_ip(NOTIP) is None
         assert net.get_nic_of_ip(LOCALHOST) is not None
 
     def test_driver_of_nic(self) -> None:
         assert net.driver_of_nic(NOTVALID) is None
@@ -85,25 +79,25 @@
         assert not net.nm_conn_up(NOTVALID)
 
     def test_nm_set_ip(self) -> None:
         assert not net.nm_set_ip(NOTVALID, NOTIP)
         assert not net.nm_set_ip(NOTVALID, IPV6)
 
     def test_nm_dev_mod_success(self) -> None:
-        with patch("sts.net.run_ret_out") as run_func:
-            run_func.return_value = [0, ""]
-            assert net.nm_dev_mod("enp17s0f1", "connection.autoconnect", "yes")
+        with patch('sts.net.run_ret_out') as run_func:
+            run_func.return_value = [0, '']
+            assert net.nm_dev_mod('enp17s0f1', 'connection.autoconnect', 'yes')
 
     def test_nm_dev_mod_failure(self) -> None:
-        with patch("sts.net.run_ret_out") as run_func:
-            run_func.return_value = [1, "Mocked failure"]
-            assert not net.nm_dev_mod("enp17s0f1", "connection.autoconnect", "yes")
+        with patch('sts.net.run_ret_out') as run_func:
+            run_func.return_value = [1, 'Mocked failure']
+            assert not net.nm_dev_mod('enp17s0f1', 'connection.autoconnect', 'yes')
 
     def test_nm_set_ip_success(self) -> None:
-        with patch("sts.net.run_ret_out") as run_func:
-            run_func.return_value = [0, ""]
-            assert net.nm_set_ip("enp17s0f1", "192.168.10.18", activate=False)
+        with patch('sts.net.run_ret_out') as run_func:
+            run_func.return_value = [0, '']
+            assert net.nm_set_ip('enp17s0f1', '192.168.10.18', activate=False)
 
     def test_nm_set_ip_failure(self) -> None:
-        with patch("sts.net.run_ret_out") as run_func:
-            run_func.return_value = [1, "Mocked failure"]
-            assert not net.nm_set_ip("enp17s0f1", "192.168.10.18", activate=False)
+        with patch('sts.net.run_ret_out') as run_func:
+            run_func.return_value = [1, 'Mocked failure']
+            assert not net.nm_set_ip('enp17s0f1', '192.168.10.18', activate=False)
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/persistent_vars_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 import unittest
 
 from sts.utils.persistent_vars import recursive_read_value
 
 
 class TestChangeType(unittest.TestCase):
     def test_to_float(self) -> None:
-        assert recursive_read_value("0.1") == 0.1
-        assert recursive_read_value("1.0") == 1.0
-        assert recursive_read_value("1.1") == 1.1
+        assert recursive_read_value('0.1') == 0.1
+        assert recursive_read_value('1.0') == 1.0
+        assert recursive_read_value('1.1') == 1.1
 
     def test_to_int(self) -> None:
-        assert recursive_read_value("0") == 0
-        assert recursive_read_value("1") == 1
-        assert recursive_read_value("1234") == 1234
+        assert recursive_read_value('0') == 0
+        assert recursive_read_value('1') == 1
+        assert recursive_read_value('1234') == 1234
 
     def test_to_str(self) -> None:
-        assert recursive_read_value("0123") == "0123"
-        assert recursive_read_value("string") == "string"
+        assert recursive_read_value('0123') == '0123'
+        assert recursive_read_value('string') == 'string'
 
     def test_to_none(self) -> None:
-        assert recursive_read_value("None") is None
+        assert recursive_read_value('None') is None
 
     def test_to_bool(self) -> None:
-        assert recursive_read_value("true") is True
-        assert recursive_read_value("false") is False
-        assert recursive_read_value("True") is True
-        assert recursive_read_value("False") is False
-        assert recursive_read_value("TRUE") is True
-        assert recursive_read_value("FALSE") is False
+        assert recursive_read_value('true') is True
+        assert recursive_read_value('false') is False
+        assert recursive_read_value('True') is True
+        assert recursive_read_value('False') is False
+        assert recursive_read_value('TRUE') is True
+        assert recursive_read_value('FALSE') is False
 
     def test_to_list(self) -> None:
-        assert recursive_read_value("[1, string]") == [1, "string"]
-        assert recursive_read_value("[None]") == [None]
-        assert recursive_read_value("['string', 0.1]") == ["string", 0.1]
+        assert recursive_read_value('[1, string]') == [1, 'string']
+        assert recursive_read_value('[None]') == [None]
+        assert recursive_read_value("['string', 0.1]") == ['string', 0.1]
         assert recursive_read_value("['/dev/sda', '/dev/sdb', '/dev/sdc']") == [
-            "/dev/sda",
-            "/dev/sdb",
-            "/dev/sdc",
+            '/dev/sda',
+            '/dev/sdb',
+            '/dev/sdc',
         ]
```

### Comparing `sts_libs-0.0.5.dev2/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.6.dev0/sts_libs/tests/scsi_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
+import logging
+
 import pytest
 
 from sts import scsi
 
 
 def test_query_scsi_hosts() -> None:
     hosts = scsi.get_hosts()
     if not hosts:
-        print("SKIP: Could not find scsi hosts")
+        logging.info('SKIP: Could not find scsi hosts')
         return
 
     for host in hosts:
-        print(f"Querying info for host {host}")
+        print(f'Querying info for host {host}')
         info = scsi.query_scsi_host_info(host)
         if not info:
-            pytest.fail(f"Could not query info for host: {host}")
+            pytest.fail(f'Could not query info for host: {host}')
         for inf in info:
-            print(f"\t{inf}: {info[inf]}")
+            print(f'\t{inf}: {info[inf]}')
 
     assert 1
 
 
 def test_query_scsi_disks() -> None:
     disks = scsi.query_all_scsi_disks()
     if not disks:
-        print("SKIP: Could not find scsi disks")
+        logging.info('SKIP: Could not find scsi disks')
         return
 
     for disk in disks:
-        print(f"INFO: details for scsi id: {disk}")
+        logging.info(f'details for scsi id: {disk}')
         disk_info = disks[disk]
         for info in disk_info:
-            print(f"\t{info}: {disk_info[info]}")
+            print(f'\t{info}: {disk_info[info]}')
 
     assert 1
```

### Comparing `sts_libs-0.0.5.dev2/.gitignore` & `sts_libs-0.0.6.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev2/LICENSE` & `sts_libs-0.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev2/PKG-INFO` & `sts_libs-0.0.6.dev0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.5.dev2
+Version: 0.0.6.dev0
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
@@ -15,32 +15,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Requires-Dist: configobj==5.0.8
-Requires-Dist: netifaces2==0.0.16
+Requires-Dist: pytest-testinfra
 Requires-Dist: pytest>=6.2.2
 Requires-Dist: six==1.16.0
-Requires-Dist: typing-extensions==4.5.0
 Description-Content-Type: text/markdown
 
 # sts-libs
 
-Libs for testing storage drivers and userspace utilities on rpm-based operating systems.
+Python library for simplifying the process of writing storage tests on RPM-based Linux distributions.
 
-## What is this?
-The goal is to be able to rapidly write new tests with ease.
+## About
+sts-libs is designed to work with [tmt](https://github.com/teemtee/tmt) and pytest.
 
 It started as an incompatible fork of [libsan](https://gitlab.com/rh-kernel-stqe/python-libsan)
 and [stqe](https://gitlab.com/rh-kernel-stqe/python-libsan) with many changes. Most notably:
  - Python 3.8+ only.
  - Minimum dependencies.
- - With [tmt](https://github.com/teemtee/tmt)-compatibility in mind.
+ - With tmt and pytest compatibility in mind.
  - One repository for both libs and tests.
 
+Going forward, the libs could become a pytest plugin and compliment others, like pytest-testinfra, with which there is currently some overlap.
+
 ## Who is this for?
-Fedora, CentOS, RHEL testers.
+Fedora, CentOS Stream, RHEL testers.
 
 ## How do I contribute?
 See [contributing](https://gitlab.com/rh-kernel-stqe/sts/docs/contributing.md) doc.
```

