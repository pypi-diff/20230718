# Comparing `tmp/infoblox-discovery-0.1.1.tar.gz` & `tmp/infoblox-discovery-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoblox-discovery-0.1.1.tar", last modified: Mon Jul 17 09:58:54 2023, max compression
+gzip compressed data, was "infoblox-discovery-0.1.2.tar", last modified: Tue Jul 18 13:23:17 2023, max compression
```

## Comparing `infoblox-discovery-0.1.1.tar` & `infoblox-discovery-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/infoblox_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/file_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/fmglogging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/http_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/infoblox_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/infoblox_discovery/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 09:58:54.000000 infoblox-discovery-0.1.1/infoblox_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:58:54.535049 infoblox-discovery-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-17 09:58:18.000000 infoblox-discovery-0.1.1/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:23:17.384832 infoblox-discovery-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-18 13:23:17.384832 infoblox-discovery-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:23:17.384832 infoblox-discovery-0.1.2/infoblox_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/file_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/fmglogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/http_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/infoblox_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/infoblox_dns_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/infoblox_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/infoblox_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/infoblox_webendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/infoblox_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/infoblox_discovery/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:23:17.384832 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-18 13:23:17.000000 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 13:23:17.000000 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:23:17.000000 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:23:17.000000 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 13:23:17.000000 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 13:23:17.000000 infoblox-discovery-0.1.2/infoblox_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:23:17.384832 infoblox-discovery-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:23:17.384832 infoblox-discovery-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 13:22:42.000000 infoblox-discovery-0.1.2/tests/test_dummy.py
```

### Comparing `infoblox-discovery-0.1.1/LICENSE` & `infoblox-discovery-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/__init__.py` & `infoblox-discovery-0.1.2/infoblox_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/__main__.py` & `infoblox-discovery-0.1.2/infoblox_discovery/__main__.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/api.py` & `infoblox-discovery-0.1.2/infoblox_discovery/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 
 import urllib3
 from IPy import IP
 from infoblox_client import connector
 
 from infoblox_discovery.fmglogging import Log
 from infoblox_discovery.infoblox_dhcp import DHCP, dhcp_factory
-from infoblox_discovery.infoblox_dns import DNS, dns_factory
+from infoblox_discovery.infoblox_dns_server import DNSServer, dns_server_factory
+from infoblox_discovery.infoblox_zone import Zone, zone_factory
 from infoblox_discovery.infoblox_member import Member, member_factory
 from infoblox_discovery.infoblox_node import Node, node_factory
+from infoblox_discovery.infoblox_webendpoint import WebEndpoint, webendpoint_factory
 from infoblox_discovery.exceptions import DiscoveryException
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 log = Log(__name__)
 COMMON = "common"
 MEMBER = "member"
@@ -62,25 +64,27 @@
         self.opts = {'host': config.get('master'),
                      'username': config.get('username'),
                      'password': config.get('password'),
                      'wapi_version': config.get('wapi_version'),
                      'http_request_timeout': config.get('timeout', 60)}
         self.conn = connector.Connector(self.opts)
 
-    def get_infoblox_members(self) -> Tuple[Dict[str, Member], Dict[str, Node]]:
+    def get_infoblox_members(self) -> Tuple[Dict[str, Member], Dict[str, Node], Dict[str, DNSServer]]:
 
         return_fields_member = ['host_name', 'service_status', 'platform', 'enable_ha', 'node_info', 'ntp_setting',
                                 'extattrs']
         try:
             members_data = self.conn.get_object('member', return_fields=return_fields_member)
         except Exception as err:
             log.error(f"Could not fetch members - {str(err)}")
             raise DiscoveryException(f"Could not fetch members")
+
         members: Dict[str, Member] = {}
         nodes: Dict[str, Node] = {}
+        dns_servers: Dict[str: DNSServer] = {}
 
         for member_data in members_data:
             if self.exclusions[COMMON] in member_data['extattrs'] and \
                     member_data['extattrs'][self.exclusions[COMMON]]['value'] == 'True' \
                     or \
                     self.exclusions[MEMBER] in member_data['extattrs'] and \
                     member_data['extattrs'][self.exclusions[MEMBER]]['value'] == 'True':
@@ -91,26 +95,31 @@
             members[member.host_name] = member
 
             if member.enable_ha == 'true':
                 for node in member_data['node_info']:
                     node = node_factory(node, member.host_name, self.master)
                     nodes[node.ip] = node
 
-        return members, nodes
+            for service in member_data['service_status']:
+                if service['service'] == 'DNS' and service['status'] == 'WORKING':
+                    dns_server = dns_server_factory(member.host_name, self.master)
+                    dns_servers[member.host_name] = dns_server
+
+        return members, nodes, dns_servers
 
-    def get_infoblox_zones(self) -> Dict[str, DNS]:
+    def get_infoblox_zones(self) -> Dict[str, Zone]:
         return_fields_range = ['fqdn', 'disable', 'extattrs']
         query = {'view': 'External'}
         try:
             zones_data = self.conn.get_object('zone_auth', query, return_fields=return_fields_range)
         except Exception as err:
             log.error(f"Could not fetch zones - {str(err)}")
             raise DiscoveryException(f"Could not fetch zones")
 
-        all_dns: Dict[str: DNS] = {}
+        all_zones: Dict[str: Zone] = {}
         for zone_data in zones_data:
             log.debug(f"Dns zone {zone_data['fqdn']}")
             if self.exclusions[COMMON] in zone_data['extattrs'] and \
                     zone_data['extattrs'][self.exclusions[COMMON]]['value'] == 'True' \
                     or \
                     self.exclusions[ZONE] in zone_data['extattrs'] and \
                     zone_data['extattrs'][self.exclusions[ZONE]]['value'] == 'True' \
@@ -128,18 +137,18 @@
                 zone['name'] = ip.reverseName()
                 zone['address'] = ip.reverseName()
             else:
                 log.debug(f"dns zone {zone_data['fqdn']} - {zone_data['fqdn'].encode('idna').decode('utf-8')}")
                 zone['name'] = zone_data['fqdn']
                 zone['address'] = zone_data['fqdn'].encode('idna').decode("utf-8")
 
-            dns = dns_factory(zone['name'], self.master)
-            all_dns[dns.dns] = dns
+            z = zone_factory(zone['name'], self.master)
+            all_zones[z.zone] = z
 
-        return all_dns
+        return all_zones
 
     def get_infoblox_dhcp_ranges(self) -> Dict[str, DHCP]:
         return_fields_range = ['network', 'dhcp_utilization', 'dhcp_utilization_status', 'extattrs']
         query = {'network_view': 'default'}
 
         try:
             dhcp_ranges_data = self.conn.get_object('range', query, return_fields=return_fields_range, paging=True)
@@ -161,7 +170,38 @@
             if range in self.exclude_ranges:
                 continue
 
             dhcp = dhcp_factory(dhcp_range['network'], self.master)
             dhcp_ranges[dhcp.network] = dhcp
 
         return dhcp_ranges
+
+    def get_web_endpoints_by_networks(self, network)-> Dict[str, WebEndpoint]:
+
+        fqdn_by_network = self._get_fqdn_by_network(network)
+        web_endpoints: Dict[str, WebEndpoint] = {}
+        for fqdn in fqdn_by_network:
+            res = self._get_endpoint(fqdn)
+            for dns in res:
+                if 'External' in dns['_ref'] and 'dns_aliases' in dns:
+                    for alias in dns['dns_aliases']:
+                        web_endpoints[alias] = webendpoint_factory(alias, master=self.master)
+
+        return web_endpoints
+
+    def _get_fqdn_by_network(self, network):
+        return_fields_range = ['ip_address,names', 'objects', 'types']
+        query = {'network': network}
+        all_names = self.conn.get_object('ipv4address', query, return_fields=return_fields_range)
+
+        names = []
+        for name in all_names:
+            if 'HOST' in name['types']:
+                names.extend(name['names'])
+
+        return names
+
+    def _get_endpoint(self, dns_fqdn):
+        return_fields_range = ['dns_aliases']
+        query = {'name': dns_fqdn}
+        dns = self.conn.get_object('record:host', query, return_fields=return_fields_range)
+        return dns
```

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/cache.py` & `infoblox-discovery-0.1.2/infoblox_discovery/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 import time
 from typing import Dict, List, Any
 from infoblox_discovery.environments import DISCOVERY_CACHE_TTL
 from infoblox_discovery.fmglogging import Log
 
 log = Log(__name__)
 
-MEMBERS='members'
-NODES='nodes'
-ZONES='zones'
-DHCP_RANGES='dhcp_ranges'
-VALID_TYPES = [MEMBERS, NODES, ZONES, DHCP_RANGES]
+MEMBERS = 'members'
+NODES = 'nodes'
+ZONES = 'zones'
+DNS_SERVERS = 'dns_servers'
+DHCP_RANGES = 'dhcp_ranges'
+WEB_ENDPOINTS = 'web_endpoints'
+VALID_TYPES = [MEMBERS, NODES, ZONES, DHCP_RANGES, DNS_SERVERS, WEB_ENDPOINTS]
 
-MASTER='master'
+MASTER = 'master'
 
 
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
@@ -50,30 +52,30 @@
     def __init__(self):
         self._ttl: int = int(os.getenv(DISCOVERY_CACHE_TTL, "7200"))
         self._expire: int = 0
         # master->type-> data
         self._collect_count: Dict[str, int] = {}
         self._collect_time: Dict[str, int] = {}
         self._collect_count_failed: Dict[str, int] = {}
-        self._cache: Dict[str,Dict[str, List]] = {}
+        self._cache: Dict[str, Dict[str, List]] = {}
 
     def put(self, master: str, type: str, data: List[Any]):
         self._expire = time.time() + self._ttl
         if master not in self._cache:
             self._cache[master] = {}
         self._cache[master][type] = data
 
     def get(self, master: str, type: str) -> List[Any]:
-        if time.time() < self._expire and type in self._cache[master]:
+        if time.time() < self._expire and master in self._cache and type in self._cache[master]:
             log.info_fmt({"operation": "cache", "hit": True})
             return self._cache[master][type]
         log.info_fmt({"operation": "cache", "hit": False})
         return []
 
-    def get_all(self) -> Dict[str,Dict[str, List]]:
+    def get_all(self) -> Dict[str, Dict[str, List]]:
         return self._cache
 
     def set_collect_time(self, master, collect_time: int):
         self._collect_time[master] = collect_time
 
     def get_collect_time(self) -> Dict[str, int]:
         return self._collect_time
```

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/collector.py` & `infoblox-discovery-0.1.2/infoblox_discovery/collector.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/environments.py` & `infoblox-discovery-0.1.2/infoblox_discovery/environments.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/exceptions.py` & `infoblox-discovery-0.1.2/infoblox_discovery/exceptions.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/file_service_discovery.py` & `infoblox-discovery-0.1.2/infoblox_discovery/file_service_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from typing import List, Dict, Any
 
 import yaml
 
 from infoblox_discovery.environments import DISCOVERY_PROMETHEUS_SD_FILE_DIRECTORY, DISCOVERY_CONFIG
 from infoblox_discovery.api import InfoBlox
 from infoblox_discovery.fmglogging import Log
+from infoblox_discovery.cache import MEMBERS, NODES, ZONES, DHCP_RANGES, DNS_SERVERS
 
 
 log = Log(__name__)
 
 
 def file_service_discovery():
     # Run for as file service discovery
@@ -46,24 +47,25 @@
             config = yaml.safe_load(config_file)
 
         except yaml.YAMLError as err:
             print(err)
 
     for ib in config.get('infoblox'):
         infoblox = InfoBlox(ib)
-        if 'members' in ib.get('discovery'):
-            members, nodes = infoblox.get_infoblox_members()
-            write_sd_file(members, ib['master'], 'members')
-            write_sd_file(nodes, ib['master'], 'nodes')
-        if 'dns' in ib.get('discovery'):
-            dns = infoblox.get_infoblox_zones()
-            write_sd_file(dns, ib['master'], 'dns')
-        if 'dhcp' in ib.get('discovery'):
+        if MEMBERS in ib.get('discovery'):
+            members, nodes, dns_servers = infoblox.get_infoblox_members()
+            write_sd_file(members, ib['master'], MEMBERS)
+            write_sd_file(nodes, ib['master'], NODES)
+            write_sd_file(dns_servers, ib['master'], DNS_SERVERS)
+        if ZONES in ib.get('discovery'):
+            zones = infoblox.get_infoblox_zones()
+            write_sd_file(zones, ib['master'], ZONES)
+        if DHCP_RANGES in ib.get('discovery'):
             dhcp_ranges = infoblox.get_infoblox_dhcp_ranges()
-            write_sd_file(dhcp_ranges, ib['master'], 'dhcp_ranges')
+            write_sd_file(dhcp_ranges, ib['master'], DHCP_RANGES)
 
 
 def write_sd_file(objects, prefix: str, type: str):
     prometheus_file_sd: List[Any] = []
     for key, member in objects.items():
         prometheus_file_sd.append(member.as_prometheus_file_sd_entry())
```

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/fmglogging.py` & `infoblox-discovery-0.1.2/infoblox_discovery/fmglogging.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/http_service_discovery.py` & `infoblox-discovery-0.1.2/infoblox_discovery/http_service_discovery.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from prometheus_client import CollectorRegistry, Gauge
 from prometheus_client.exposition import CONTENT_TYPE_LATEST
 from prometheus_client.utils import INF, MINUS_INF
 from prometheus_fastapi_instrumentator import Instrumentator
 
 from infoblox_discovery.api import InfoBlox
-from infoblox_discovery.cache import Cache, MEMBERS, NODES, ZONES, DHCP_RANGES, MASTER, VALID_TYPES
+from infoblox_discovery.cache import Cache, MEMBERS, NODES, ZONES, DHCP_RANGES, DNS_SERVERS, MASTER, WEB_ENDPOINTS, VALID_TYPES
 from infoblox_discovery.collector import InfobloxCollector
 from infoblox_discovery.environments import DISCOVERY_BASIC_AUTH_USERNAME, DISCOVERY_BASIC_AUTH_PASSWORD, \
     DISCOVERY_BASIC_AUTH_ENABLED, DISCOVERY_LOG_LEVEL, DISCOVERY_HOST, DISCOVERY_PORT, DISCOVERY_FETCH_INTERVAL
 from infoblox_discovery.environments import DISCOVERY_CONFIG
 from infoblox_discovery.exceptions import DiscoveryException
 from infoblox_discovery.fmglogging import Log
 
@@ -90,17 +90,18 @@
     cache = Cache()
     for ib in config.get('infoblox'):
         start_time = time.time()
         infoblox = InfoBlox(ib)
         try:
             if MEMBERS in ib.get('discovery'):
                 try:
-                    members, nodes = infoblox.get_infoblox_members()
+                    members, nodes, dns_servers = infoblox.get_infoblox_members()
                     cache.put(ib[MASTER], MEMBERS, list(members.values()))
                     cache.put(ib[MASTER], NODES, list(nodes.values()))
+                    cache.put(ib[MASTER], DNS_SERVERS, list(dns_servers.values()))
                 except DiscoveryException:
                     log.error(f"Failed to get members for {ib[MASTER]}")
 
             if ZONES in ib.get('discovery'):
                 try:
                     dns = infoblox.get_infoblox_zones()
                     cache.put(ib[MASTER], ZONES, list(dns.values()))
@@ -110,17 +111,25 @@
             if DHCP_RANGES in ib.get('discovery'):
                 try:
                     dhcp_ranges = infoblox.get_infoblox_dhcp_ranges()
                     cache.put(ib[MASTER], DHCP_RANGES, list(dhcp_ranges.values()))
                 except DiscoveryException:
                     log.error(f"Failed to get dhcp ranges for {ib[MASTER]}")
 
+            if WEB_ENDPOINTS in ib.get('discovery') and ib.get(WEB_ENDPOINTS):
+                try:
+                    for network in ib.get(WEB_ENDPOINTS).get('networks'):
+                        web_endpoints = infoblox.get_web_endpoints_by_networks(network)
+                        cache.put(ib[MASTER], WEB_ENDPOINTS, list(web_endpoints.values()))
+                except DiscoveryException:
+                    log.error(f"Failed to get dhcp ranges for {ib[MASTER]}")
+
             end_time = time.time()
             cache.set_collect_time(ib[MASTER], int(end_time - start_time))
-            log.info(f"collect infoblox discovery from {ib[MASTER]} {end_time-start_time} sec")
+            log.info(f"Collect infoblox discovery from {ib[MASTER]} {end_time-start_time} sec")
         except DiscoveryException:
             cache.inc_collect_count_failed(ib[MASTER])
         finally:
             cache.inc_collect_count(ib[MASTER])
 
 
 @app.on_event("startup")
```

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dhcp.py` & `infoblox-discovery-0.1.2/infoblox_discovery/infoblox_dhcp.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_dns.py` & `infoblox-discovery-0.1.2/infoblox_discovery/infoblox_zone.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,30 +18,30 @@
     along with infoblox-discovery.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 from typing import Dict, Any, Tuple
 
 
-class DNS:
-    def __init__(self, dns: str):
-        self.dns: str = dns
+class Zone:
+    def __init__(self, zone: str):
+        self.zone: str = zone
         self.master: str = ''
 
     def _as_labels(self) -> Dict[str, str]:
         labels: Dict[str, str] = {}
         for k, v in self.__dict__.items():
-            if k != "dns":
+            if k != "zone":
                 labels[k] = v
         return labels
 
     def valid(self) -> Tuple[bool, str]:
         return True, ""
 
     def as_prometheus_file_sd_entry(self) -> Dict[str, Any]:
-        return {'targets': [f"{self.dns}"], 'labels': self._as_labels()}
+        return {'targets': [f"{self.zone}"], 'labels': self._as_labels()}
 
 
-def dns_factory(dns: str, master: str) -> DNS:
-    dns = DNS(dns=dns)
-    dns.master = master
-    return dns
+def zone_factory(zone_name: str, master: str) -> Zone:
+    zone = Zone(zone=zone_name)
+    zone.master = master
+    return zone
```

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_member.py` & `infoblox-discovery-0.1.2/infoblox_discovery/infoblox_member.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/infoblox_node.py` & `infoblox-discovery-0.1.2/infoblox_discovery/infoblox_node.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/metrics.py` & `infoblox-discovery-0.1.2/infoblox_discovery/metrics.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery/transform.py` & `infoblox-discovery-0.1.2/infoblox_discovery/transform.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/infoblox_discovery.egg-info/SOURCES.txt` & `infoblox-discovery-0.1.2/infoblox_discovery.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 infoblox_discovery/collector.py
 infoblox_discovery/environments.py
 infoblox_discovery/exceptions.py
 infoblox_discovery/file_service_discovery.py
 infoblox_discovery/fmglogging.py
 infoblox_discovery/http_service_discovery.py
 infoblox_discovery/infoblox_dhcp.py
-infoblox_discovery/infoblox_dns.py
+infoblox_discovery/infoblox_dns_server.py
 infoblox_discovery/infoblox_member.py
 infoblox_discovery/infoblox_node.py
+infoblox_discovery/infoblox_webendpoint.py
+infoblox_discovery/infoblox_zone.py
 infoblox_discovery/metrics.py
 infoblox_discovery/transform.py
 infoblox_discovery.egg-info/PKG-INFO
 infoblox_discovery.egg-info/SOURCES.txt
 infoblox_discovery.egg-info/dependency_links.txt
 infoblox_discovery.egg-info/not-zip-safe
 infoblox_discovery.egg-info/requires.txt
```

### Comparing `infoblox-discovery-0.1.1/setup.py` & `infoblox-discovery-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `infoblox-discovery-0.1.1/tests/test_dummy.py` & `infoblox-discovery-0.1.2/tests/test_dummy.py`

 * *Files identical despite different names*

