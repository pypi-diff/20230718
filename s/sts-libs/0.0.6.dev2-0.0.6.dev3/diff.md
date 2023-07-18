# Comparing `tmp/sts_libs-0.0.6.dev2.tar.gz` & `tmp/sts_libs-0.0.6.dev3.tar.gz`

## Comparing `sts_libs-0.0.6.dev2.tar` & `sts_libs-0.0.6.dev3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/__about__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    41654 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    48750 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    45050 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    66092 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    36056 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35901 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42548 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17985 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    28199 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22450 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/log.py
--rw-r--r--   0        0        0    12226 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/LICENSE
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/pyproject.toml
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/sts_libs/README.md
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    41654 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    48813 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    45059 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    66092 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    36056 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35919 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42566 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17994 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    28271 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22459 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/log.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/LICENSE
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/pyproject.toml
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/sts_libs/README.md
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 sts_libs-0.0.6.dev3/PKG-INFO
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/dm.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/dmpd.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/fc.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/fio.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/iscsi.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             if not iscsiadm.iface_exists(iface=ifacename):
                 create_iscsi_iface(iface_name=ifacename)
             for n, v in iface.items():
                 if n == 'iscsi_ifacename':
                     continue
                 completed_process = iscsiadm.iface_update(iface=ifacename, name=n, value=str(v))
                 ret = completed_process.rc
-                out = completed_process.stdout
+                out = completed_process.stdout.rstrip()
                 if ret != 0:
                     logging.error(f'iscsi update command returned {ret}. Output: {out}')
                     return False
 
     if 'targets' in variables:
         for target in variables['targets']:
             if iscsiadm.discovery(**target) != 0:
@@ -397,15 +397,15 @@
         logging.error(f'Could not install {PACKAGE_NAME}')
         return False
 
     return True
 
 
 def get_iscsi_hosts() -> List[str]:
-    return run(f'ls {host_path}').stdout.splitlines()
+    return run(f'ls {host_path}').stdout.rstrip().splitlines()
 
 
 def get_iscsi_host_numbers() -> List[str]:
     hosts = get_iscsi_hosts()
     return [h.lstrip('host') for h in hosts]
 
 
@@ -418,15 +418,15 @@
     Dict:    Dict with all discovered targets
     None:    If some problem happened.
     """
     cp = run('iscsiadm -m discovery -P1')
     if cp.failed:
         # If no target is found iscsiadm returns error code
         return None
-    lines = cp.stdout.splitlines()
+    lines = cp.stdout.rstrip().splitlines()
 
     supported_discovery_modes = ['SENDTARGETS', 'iSNS', 'STATIC', 'FIRMWARE']
     supported_mode_type = {'SENDTARGETS': 'sendtargets', 'iSNS': 'isns'}
 
     discovery_info_dict = {}
     discovery_address = None
     disc_mode = None
@@ -714,15 +714,15 @@
 #            ses_dict["target_iqn"] = m.group(6)
 #            sessions[sid] = ses_dict
 #    return sessions_dict
 
 
 def get_all_session_ids() -> List[Optional[str]]:
     """Returns list of session ids."""
-    session_info = run('iscsiadm -m session -P1').stdout.splitlines()
+    session_info = run('iscsiadm -m session -P1').stdout.rstrip().splitlines()
     return [remove_prefix(id, '\t\tSID: ') for id in session_info if 'SID' in id]
 
 
 def query_iscsi_session(sid):  # noqa: ANN001, ANN201
     """Query information from a specific iSCSI session
     The arguments are:
     sid:      Session id
@@ -732,15 +732,15 @@
     """
     if not sid:
         logging.error('query_iscsi_session() - requires sid as argument')
         return None
 
     regex_session_scsi_id = '^[ \t]+scsi([0-9]+) Channel ([0-9]+) Id ([0-9])+ Lun: ([0-9]+)$'
 
-    lines = run(f'iscsiadm -m session -P3 -S -r {sid}').stdout.splitlines()
+    lines = run(f'iscsiadm -m session -P3 -S -r {sid}').stdout.rstrip().splitlines()
 
     session_info_dict = {}
     # dict with disk name and its status
     session_disks_dict = {}
     # store host number and status
     session_host_dict = {}
     for line in lines:
@@ -1148,15 +1148,15 @@
 
     for iface in ifaces:
         cmd = f'iscsiadm -m iface -I {iface}'
         result = run(cmd)
         if result.failed:
             logging.warning('Could not login to iSCSI target')
             continue
-        details = result.stdout.splitlines()
+        details = result.stdout.rstrip().splitlines()
         for info in details:
             m = iface_info_regex.match(info)
             if not m:
                 continue
             if iface not in list(all_iface_dict.keys()):
                 all_iface_dict[iface] = {}
             value = m.group(2)
@@ -1258,15 +1258,15 @@
         return False
 
     return True
 
 
 def get_iscsi_iface_names() -> List[str]:
     """Return a list with the name of all iSCSI interfaces on the host."""
-    ifaces = run('iscsiadm -m iface').stdout.splitlines()
+    ifaces = run('iscsiadm -m iface').stdout.rstrip().splitlines()
     return [i.split(' ')[0] for i in ifaces if 'iSCSI ERROR' not in i]  # bz1997710
 
 
 def set_iscsid_parameter(parameters: dict) -> bool:
     """Change parameter in iscsid.conf file and restarts iscsid service
     Use dictionary with parameter:value as argument.
     """
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/linux.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/linux.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
         driver_info[info] = output
 
     sys_driver_parameter = sysfs_driver_folder / 'parameters'
     if sys_driver_parameter.is_dir():
         # Need to add driver parameters
         param_files = list(sys_driver_parameter.iterdir())
         for param in param_files:
-            output = run(f'cat {sys_driver_parameter}/{param}').stdout
+            output = run(f'cat {sys_driver_parameter}/{param}').stdout.rstrip()
             if 'parameters' not in driver_info:
                 driver_info['parameters'] = {}
             driver_info['parameters'][param] = output
     return driver_info
 
 
 def mkdir(new_dir):  # noqa: ANN001, ANN201
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/lio.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/lio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/loopdev.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/lvm.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,15 +555,15 @@
         # need to remove new line character as print will add it
         line = line.rstrip('\n')  # noqa: PLW2901
         print(line)
 
 
 def get_lvm_config_options(all_params=False):  # noqa: ANN001, ANN201
     """Get all the configuration types from lvm.conf file."""
-    out = run('lvmconfig --type full').stdout
+    out = run('lvmconfig --type full').stdout.rstrip()
 
     options = {}
     category = ''
     for line in out.split('\n'):
         line = line.strip()  # noqa: PLW2901
         if not line or '}' in line:
             # skip empty or end of list line
@@ -582,15 +582,15 @@
     options_all = []
     for value in options.values():
         options_all.extend(value)
     return options_all
 
 
 def check_lvm_config(option):  # noqa: ANN001, ANN201
-    return run(f'lvs -o {option}').stdout
+    return run(f'lvs -o {option}').stdout.rstrip()
 
 
 def get_all_lvm_config_options():  # noqa: ANN201
     all_opts = check_lvm_config('asdf')  # needs just something that it doesn't know
     # we need to test_filter on lines that look like this
     # lvm_blahblah - explanation
     # and remove separators
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/md.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/mp.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,15 +976,15 @@
 
     Raises:
       IOError: Augeas save fails. Check if multipath.conf changes are valid.
     """
     matched_path = mpath_conf_match(path, value)
 
     if matched_path:
-        out = run(f'augtool -s rm "{matched_path}"').stdout
+        out = run(f'augtool -s rm "{matched_path}"').stdout.rstrip()
         if 'Saved 1 file(s)' not in out:
             logging.error(f'unable to set {path} to {value}')
             return False
 
     return True
 
 
@@ -1004,15 +1004,15 @@
     if not linux.install_package('augeas'):
         logging.error('Could not install augeas')
         return None
 
     full_path = path if path.startswith(aug_conf_path) else aug_conf_path + path
 
     # successfully matches also when end of path is not unique - path[*] value, but not path[*]/path value
-    out = run(f'augtool match "{full_path}" "{value}"').stdout
+    out = run(f'augtool match "{full_path}" "{value}"').stdout.rstrip()
 
     # augtool prints path when matched, return codes seems useless
     if aug_conf_path in out:
         # returning path, as it can be useful when modifying non-unique paths
         return out
     return None
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/net.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/net.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """Return list of interfaces with link/ether."""
     nics = get_nics()
     return [i for i in nics if get_mac_of_nic(i)]
 
 
 def get_mac_of_nic(nic: str) -> Union[str, None]:
     """Given a NIC name return its MAC address."""
-    cp = run(f'ip -o link show {nic}').stdout
+    cp = run(f'ip -o link show {nic}').stdout.rstrip()
     if not cp:
         return None
     ip_link = cp.split()
     try:
         mac = ip_link[ip_link.index('link/ether') + 1]
     except ValueError:
         return None
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,57 +321,57 @@
         logging.error('scsi_driver_of_host_id() - requires host_id parameter')
         return None
     scsi_drv_sysfs = f'/sys/class/scsi_host/host{host_id}/proc_name'
     if not Path(scsi_drv_sysfs).is_file():
         logging.error(f'{scsi_drv_sysfs} is not a valid path')
         return None
 
-    output = run(f'cat {scsi_drv_sysfs}').stdout
+    output = run(f'cat {scsi_drv_sysfs}').stdout.rstrip()
     scsi_driver = output
     if not scsi_driver or scsi_driver == '(null)':
         # Driver information was not exported, let try to find it out some other way
         lpfc_sysfs_file = f'/sys/class/scsi_host/host{host_id}/lpfc_drvr_version'
         if Path(lpfc_sysfs_file).is_file():
             return 'lpfc'
 
         driver_sysfs_file = f'/sys/class/scsi_host/host{host_id}/driver_name'
         if Path(driver_sysfs_file).is_file():
-            return run(f'cat {driver_sysfs_file}').stdout
+            return run(f'cat {driver_sysfs_file}').stdout.rstrip()
 
         model_sysfs_file = f'/sys/class/scsi_host/host{host_id}/model_name'
         if Path(model_sysfs_file).is_file():
-            output = run(f'cat {model_sysfs_file}').stdout
+            output = run(f'cat {model_sysfs_file}').stdout.rstrip()
             if re.match('^QLE', output):
                 return 'qla2xxx'
 
         symbolic_sysfs_file = f'/sys/class/fc_host/host{host_id}/symbolic_name'
         if Path(symbolic_sysfs_file).is_file():
-            output = run(f'cat {symbolic_sysfs_file}').stdout
+            output = run(f'cat {symbolic_sysfs_file}').stdout.rstrip()
             if re.search('bnx2fc', output):
                 return 'bnx2fc'
 
         pci_id = pci_id_of_host_id(host_id)
         if pci_id:
             lspci_regex = r'Kernel modules:\s+(\S+)'
             if not exists('lspci'):
                 logging.error("pciutils is not installed. Can't query driver name using pci_id.")
                 return None
             output = run(
                 f'lspci -s "{pci_id}" -v | grep "Kernel modules:"',
-            ).stdout
+            ).stdout.rstrip()
             if output:
                 m = re.search(lspci_regex, output)
                 if m:
                     return m.group(1)
 
         logging.error(f'Could not get driver name for SCSI host{host_id}')
         return None
     if scsi_driver == 'fcoe':
         drv_version_path = f'/sys/class/fc_host/host{host_id}/driver_version'
-        output = run(f'cat {drv_version_path}').stdout
+        output = run(f'cat {drv_version_path}').stdout.rstrip()
         if re.search('ixgbe', output):
             return 'ixgbe'
     return scsi_driver
 
 
 def pci_id_of_host_id(host_id):  # noqa: ANN001, ANN201
     """Usage
@@ -841,15 +841,15 @@
 
     sys_path = f'/sys/block/{scsi_disk}/device/state'
     if not Path(sys_path).is_file():
         logging.error(f'disk_sys_check() - No such file: {sys_path}')
         return None
 
     cmd = f'cat {sys_path} 2>/dev/null'
-    state = run(cmd).stdout
+    state = run(cmd).stdout.rstrip()
     if not state:
         logging.error(f'disk_sys_check() - Could not read from {sys_path}')
         return None
 
     return state
 
 
@@ -872,13 +872,13 @@
 
     sys_path = f'/sys/block/{scsi_disk}/device/timeout'
     if not Path(sys_path).is_file():
         logging.error(f'timeout_of_disk() - No such file: {sys_path}')
         return None
 
     cmd = f'cat {sys_path} 2>/dev/null'
-    timeout = run(cmd).stdout
+    timeout = run(cmd).stdout.rstrip()
     if not timeout:
         logging.error(f'timeout_of_disk() - Could not read from {sys_path}')
         return None
 
     return timeout
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/stratis.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/stratis.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/vdo.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 correct_vdo_device = True
             if correct_vdo_device and 'device:' in line:
                 # Now we have the device, just need to follow the link
                 device = line.split('device:').pop().strip()
                 break
 
     # now we might have /dev/disk/by-id/UUID, need to get something reasonable
-    data = run(f'ls -la {device}').stdout
+    data = run(f'ls -la {device}').stdout.rstrip()
     device = data.split('/').pop().strip()
 
     # format dm-X causes issues later on, where the device cannot be found using lsblk to check for size
     if device.startswith('dm-'):
         with Path(f'/sys/block/{device}/dm/name').open() as f:
             dev_name = f.readline().rstrip('\n')
         device = f'/dev/mapper/{dev_name}'
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/beaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     # backup the current full console.log
     # next time we run the test we will compare just
     # what has been appended to console.log
     run(f'mv -f {new_console_log_file} {prev_console_log_file}')
 
     logging.info(f'Checking for errors on {console_log_file}')
     for msg in error_mgs:
-        output = run(f"cat {console_log_file} | grep -i '{msg}'").stdout
+        output = run(f"cat {console_log_file} | grep -i '{msg}'").stdout.rstrip()
         if output:
             print(f'INFO found {msg} on {console_log_file}')
             log_submit(console_log_file)
             error = +1
 
     if error:
         return False
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/cmdline.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 from sts import host_init
 
 host = host_init()
 
 
 def run(cmd: str) -> CommandResult:
     logging.info(f"Running command: '{cmd}'")
-    cr: CommandResult = host.run(cmd)
-    if cr.stdout:
-        cr.stdout = cr.stdout.rstrip()
-    if cr.stderr:
-        cr.stderr = cr.stderr.rstrip()
-
     return host.run(cmd)
 
 
 def run_ret_out(
     cmd: str,
     return_output: bool = False,
 ) -> Union[int, Tuple[int, str]]:
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/logchecker.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def journalctl_timestamp() -> str:
     """Returns current time in journalctl-compatible format.
 
     Usage example:
         logging_start = journalctl_timestamp()
-        failure_logs = run(f"journalctl -S {logging_start}).stdout"
+        failure_logs = run(f"journalctl -S {logging_start}).stdout.rstrip()"
     """
     return datetime.now().isoformat(sep=' ', timespec='minutes')  # noqa: DTZ005 <- We want local timezone.
 
 
 def check_all():  # noqa: ANN201
     """Check for error on the system
     Returns:
@@ -136,26 +136,26 @@
     True if did not find any issue
     False if found some issue.
     """
     logging.info('Checking for tainted kernel')
 
     previous_tainted_file = '/tmp/previous-tainted'
 
-    tainted = run('cat /proc/sys/kernel/tainted').stdout
+    tainted = run('cat /proc/sys/kernel/tainted').stdout.rstrip()
 
     tainted_val = int(tainted)
     if tainted_val == 0:
         run('echo %d > %s' % (tainted_val, previous_tainted_file))
         return True
 
     logging.warning('Kernel is tainted!')
 
     if not Path(previous_tainted_file).is_file():
         run(f'echo {tainted_val} > {previous_tainted_file}')
-    prev_taint = run(f'cat {previous_tainted_file}').stdout
+    prev_taint = run(f'cat {previous_tainted_file}').stdout.rstrip()
     prev_taint_val = int(prev_taint)
     if prev_taint_val == tainted_val:
         logging.info('Kernel tainted has already been handled')
         return True
 
     run('echo %d > %s' % (tainted_val, previous_tainted_file))
 
@@ -171,15 +171,15 @@
         tainted_val /= 2
     # List all tainted bits that are defined
     print('List bit definition for tainted kernel')
     run('cat /usr/src/kernels/`uname -r`/include/linux/kernel.h | grep TAINT_')
 
     found_issue = False
     # try to find the module which tainted the kernel, tainted module have a mark between '('')'
-    output = run("cat /proc/modules | grep -e '(.*)' |  cut -d' ' -f1").stdout
+    output = run("cat /proc/modules | grep -e '(.*)' |  cut -d' ' -f1").stdout.rstrip()
     tainted_mods = output.split('\n')
     # For example during iscsi async_events scst tool loads an unsigned module
     # just ignores it, so we will ignore this tainted if there is no tainted
     # modules loaded
     if not tainted_mods:
         logging.info('ignoring tainted as the module is not loaded anymore')
     else:
@@ -257,15 +257,15 @@
 
     if not Path(previous_time_file).is_file():
         first_time = 'Jan 01 00:00:00'
         time = _date2num(first_time)
         run(f'echo {time} > {previous_time_file}')
 
     # Read the last time test ran
-    last_run = run(f'cat {previous_time_file}').stdout
+    last_run = run(f'cat {previous_time_file}').stdout.rstrip()
     logging.info(f'Checking for stack dump messages after: {last_run}')
 
     # Going to search the file for text that matches begin_tag until end_tag
     dump_regex = begin_tag + '(.*?)' + end_tag
     m = re.findall(dump_regex, log, re.MULTILINE)
     if m:
         logging.info(f'Checking if it is newer than: {last_run}')
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,10 +288,10 @@
 
     Returns:
       list.: List of persistent vars file names having the specified prefix
     """
     if exists_persistent_vars_file():
         variables = read_var(get_persistent_vars_file_name())
     else:
-        variables = run(f'ls -la {get_persistent_files_dir()}').stdout
+        variables = run(f'ls -la {get_persistent_files_dir()}').stdout.rstrip()
         variables = [line.split().pop() for line in variables.splitlines()[3:]]
     return [value for value in variables if value.startswith(prefix)]
```

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.6.dev3/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/cmdline_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/fio_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/linux_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/md_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/net_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.6.dev3/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/.gitignore` & `sts_libs-0.0.6.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/LICENSE` & `sts_libs-0.0.6.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/pyproject.toml` & `sts_libs-0.0.6.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/sts_libs/README.md` & `sts_libs-0.0.6.dev3/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.6.dev2/PKG-INFO` & `sts_libs-0.0.6.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.6.dev2
+Version: 0.0.6.dev3
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
```

