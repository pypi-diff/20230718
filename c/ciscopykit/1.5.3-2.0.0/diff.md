# Comparing `tmp/ciscopykit-1.5.3.tar.gz` & `tmp/ciscopykit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-1.5.3.tar", last modified: Sun Jul 16 17:07:34 2023, max compression
+gzip compressed data, was "ciscopykit-2.0.0.tar", last modified: Tue Jul 18 08:49:29 2023, max compression
```

## Comparing `ciscopykit-1.5.3.tar` & `ciscopykit-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.584844 ciscopykit-1.5.3/ciscopykit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.584844 ciscopykit-1.5.3/ciscopykit/help/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/help/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/lan_security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/dhcp_snooping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/dynamic_arp_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/stp_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/switchport_security.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/vlan_security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/dhcp_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/pat_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/switch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/l2_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/l3_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/templates/generate_router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/vlan/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/vlan/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.584844 ciscopykit-1.5.3/ciscopykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.620225 ciscopykit-2.0.0/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.620225 ciscopykit-2.0.0/ciscopykit/help/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/help/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.620225 ciscopykit-2.0.0/ciscopykit/lan_security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/dhcp_snooping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/dynamic_arp_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/stp_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/switchport_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/lan_security/vlan_security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/ciscopykit/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/services/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/services/dhcp_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/services/pat_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/ciscopykit/switch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/switch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/switch/l2_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/switch/l3_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/switch/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/ciscopykit/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/vlan/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/ciscopykit/vlan/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:29.620225 ciscopykit-2.0.0/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-18 08:49:29.000000 ciscopykit-2.0.0/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 08:49:29.000000 ciscopykit-2.0.0/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:49:29.000000 ciscopykit-2.0.0/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 08:49:29.000000 ciscopykit-2.0.0/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-18 08:49:29.000000 ciscopykit-2.0.0/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 08:49:29.000000 ciscopykit-2.0.0/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:49:29.624225 ciscopykit-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-18 08:49:10.000000 ciscopykit-2.0.0/setup.py
```

### Comparing `ciscopykit-1.5.3/LICENSE.md` & `ciscopykit-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/PKG-INFO` & `ciscopykit-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.5.3
+Version: 2.0.0
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.5.3/README.md` & `ciscopykit-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/app.py` & `ciscopykit-2.0.0/ciscopykit/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/device.py` & `ciscopykit-2.0.0/ciscopykit/device.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/entry_point.py` & `ciscopykit-2.0.0/ciscopykit/entry_point.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/interface.py` & `ciscopykit-2.0.0/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/lan_security/dhcp_snooping.py` & `ciscopykit-2.0.0/ciscopykit/lan_security/dhcp_snooping.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+"""
+Module: dhcp_snooping
+
+This module provides a function to generate a DHCP snooping configuration for an IOS device.
+
+Function:
+- generate_dhcp_snooping_config(interface, trust_ports): Generates a DHCP snooping configuration for an IOS device.
+
+Args:
+- interface (str): The interface on which DHCP snooping should be enabled.
+- trust_ports (list): A list of interfaces that should be trusted by DHCP snooping.
+
+Returns:
+- str: The DHCP snooping configuration that can be copied and pasted onto an IOS device.
+
+Raises:
+- ValueError: If interface or trust_ports are not provided.
+
+Usage:
+    interface = 'GigabitEthernet0/1'
+    trust_ports = ['GigabitEthernet0/2', 'GigabitEthernet0/3']
+    dhcp_snooping_config = generate_dhcp_snooping_config(interface, trust_ports)
+    print(dhcp_snooping_config)
+
+"""
+
 def generate_dhcp_snooping_config(interface, trust_ports):
     """
     Generates a DHCP snooping configuration for an IOS device.
 
     Args:
         interface (str): The interface on which DHCP snooping should be enabled.
         trust_ports (list): A list of interfaces that should be trusted by DHCP snooping.
```

### Comparing `ciscopykit-1.5.3/ciscopykit/lan_security/stp_security.py` & `ciscopykit-2.0.0/ciscopykit/lan_security/stp_security.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+Module: stp_security
+
+This module provides functions to configure Spanning Tree Protocol (STP) security features such as PortFast and BPDU Guard.
+
+Functions:
+- configure_portfast_default(): Configures PortFast on all access ports by default.
+- configure_bpdu_guard(interface): Configures BPDU Guard on the specified interface.
+- configure_stp_security(interface): Configures PortFast and BPDU Guard on the specified interface.
+
+Raises:
+- ValueError: If the interface name is not valid.
+"""
+
+
 def configure_portfast_default():
     """
     Configures PortFast on all access ports by default.
 
     Returns:
         str: The configuration command for enabling PortFast by default.
     """
@@ -18,15 +33,16 @@
 
     Returns:
         str: The configuration command for enabling BPDU Guard on the interface.
 
     Raises:
         ValueError: If the interface name is not valid.
     """
-    valid_interface_types = ["GigabitEthernet", "FastEthernet", "Ethernet", "Serial", "Portchannel", "VLAN"]
+    valid_interface_types = [
+        "GigabitEthernet", "FastEthernet", "Ethernet", "Serial", "Portchannel", "VLAN"]
     interface_type = interface.split()[0]
 
     if interface_type not in valid_interface_types:
         raise ValueError(
             f"Invalid interface name. The interface type must be one of: {', '.join(valid_interface_types)}"
         )
 
@@ -44,15 +60,16 @@
 
     Returns:
         str: The configuration commands for enabling PortFast and BPDU Guard on the interface.
 
     Raises:
         ValueError: If the interface name is not valid.
     """
-    valid_interface_types = ["GigabitEthernet", "FastEthernet", "Ethernet", "Serial", "Portchannel", "VLAN"]
+    valid_interface_types = [
+        "GigabitEthernet", "FastEthernet", "Ethernet", "Serial", "Portchannel", "VLAN"]
     interface_type = interface.split()[0]
 
     if interface_type not in valid_interface_types:
         raise ValueError(
             f"Invalid interface name. The interface type must be one of: {', '.join(valid_interface_types)}"
         )
```

### Comparing `ciscopykit-1.5.3/ciscopykit/lan_security/switchport_security.py` & `ciscopykit-2.0.0/ciscopykit/lan_security/switchport_security.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+"""
+Module: switchport_security
+
+This module provides a function to generate the configuration command for switchport security.
+
+Function:
+- generate_switchport_security_config(interface, max_mac, violation_action='restrict', aging_time=None, sticky_mac=True):
+    Generates the configuration command for switchport security.
+
+    Args:
+        interface (str): Interface name.
+        max_mac (int): Maximum number of MAC addresses to be learned.
+        violation_action (str, optional): Violation action. Can be 'restrict', 'protect', or 'shutdown'. (default: 'restrict')
+        aging_time (int, optional): Aging time for dynamically learned secure MAC addresses in minutes. (default: None)
+        sticky_mac (bool, optional): Whether to enable sticky MAC address. (default: True)
+
+    Returns:
+        str: Configuration command for switchport security.
+
+    Raises:
+        ValueError: If the violation action is not one of 'restrict', 'protect', or 'shutdown'.
+"""
+
+
 def generate_switchport_security_config(interface, max_mac, violation_action='restrict', aging_time=None, sticky_mac=True):
     """
     Generate the configuration command for switchport security.
 
     Args:
         interface (str): Interface name.
         max_mac (int): Maximum number of MAC addresses to be learned.
@@ -12,24 +36,23 @@
     Returns:
         str: Configuration command for switchport security.
 
     Raises:
         ValueError: If the violation action is not one of 'restrict', 'protect', or 'shutdown'.
     """
     if violation_action not in ['restrict', 'protect', 'shutdown']:
-        raise ValueError("Invalid violation action. It must be 'restrict', 'protect', or 'shutdown'.")
+        raise ValueError(
+            "Invalid violation action. It must be 'restrict', 'protect', or 'shutdown'.")
 
     command = f"interface {interface}\n"
     command += " switchport mode access\n"
     command += " switchport port-security\n"
     command += f" switchport port-security maximum {max_mac}\n"
     command += f" switchport port-security violation {violation_action}\n"
 
     if aging_time is not None:
         command += f" switchport port-security aging time {aging_time}\n"
 
     if sticky_mac:
         command += " switchport port-security mac-address sticky\n"
 
     return command
-
-
```

### Comparing `ciscopykit-1.5.3/ciscopykit/services/app.py` & `ciscopykit-2.0.0/ciscopykit/services/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/services/dhcp_service.py` & `ciscopykit-2.0.0/ciscopykit/services/dhcp_service.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/services/pat_service.py` & `ciscopykit-2.0.0/ciscopykit/services/pat_service.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/switch/app.py` & `ciscopykit-2.0.0/ciscopykit/switch/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/switch/l3_switch.py` & `ciscopykit-2.0.0/ciscopykit/switch/l3_switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/switch/switch.py` & `ciscopykit-2.0.0/ciscopykit/switch/switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/templates/generate_router_config.py` & `ciscopykit-2.0.0/ciscopykit/templates/generate_router_config.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/vlan/app.py` & `ciscopykit-2.0.0/ciscopykit/vlan/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit/vlan/vlan.py` & `ciscopykit-2.0.0/ciscopykit/vlan/vlan.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/ciscopykit.egg-info/PKG-INFO` & `ciscopykit-2.0.0/ciscopykit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.5.3
+Version: 2.0.0
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.5.3/ciscopykit.egg-info/SOURCES.txt` & `ciscopykit-2.0.0/ciscopykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.3/setup.py` & `ciscopykit-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='1.5.3',
+    version='2.0.0',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
     description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
     long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
     url='https://github.com/Vincent-de-Torres-Portfolio/ciscopykit',
     packages=find_packages(),
     classifiers=[
```

