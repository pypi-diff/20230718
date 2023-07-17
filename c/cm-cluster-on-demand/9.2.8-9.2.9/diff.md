# Comparing `tmp/cm-cluster-on-demand-9.2.8.tar.gz` & `tmp/cm-cluster-on-demand-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm-cluster-on-demand-9.2.8.tar", last modified: Tue Dec 27 18:19:24 2022, max compression
+gzip compressed data, was "cm-cluster-on-demand-9.2.9.tar", last modified: Mon Feb 20 12:11:25 2023, max compression
```

## Comparing `cm-cluster-on-demand-9.2.8.tar` & `cm-cluster-on-demand-9.2.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.401296 cm-cluster-on-demand-9.2.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       98 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1154 2022-12-27 18:19:24.401296 cm-cluster-on-demand-9.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)      614 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.397296 cm-cluster-on-demand-9.2.8/clusterondemand/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/clusterondemand/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/clusterondemand/_version.py
--rw-r--r--   0 root         (0) root         (0)     3654 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/accept_eula.py
--rw-r--r--   0 root         (0) root         (0)     2595 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/bcm_version.py
--rw-r--r--   0 root         (0) root         (0)     3770 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/brightsetup.py
--rw-r--r--   0 root         (0) root         (0)     2319 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cidr.py
--rw-r--r--   0 root         (0) root         (0)     1455 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.397296 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/
--rw-r--r--   0 root         (0) root         (0)      776 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/cloudconfig.py
--rw-r--r--   0 root         (0) root         (0)     5720 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/headcommands.py
--rw-r--r--   0 root         (0) root         (0)    11514 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/headfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.397296 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/tests/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5849 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/clustercreate.py
--rw-r--r--   0 root         (0) root         (0)     3297 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/clusternameprefix.py
--rw-r--r--   0 root         (0) root         (0)    11756 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/cmclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.397296 cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2014 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/datetimefunctions.py
--rw-r--r--   0 root         (0) root         (0)     7311 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/sortingutils.py
--rw-r--r--   0 root         (0) root         (0)     9938 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/command_runner.py
--rw-r--r--   0 root         (0) root         (0)     2326 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/configdump.py
--rw-r--r--   0 root         (0) root         (0)     2332 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/configshow.py
--rw-r--r--   0 root         (0) root         (0)    22161 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5626 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/configuration_validation.py
--rw-r--r--   0 root         (0) root         (0)     1291 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/const.py
--rw-r--r--   0 root         (0) root         (0)     1293 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/contextmanagers.py
--rw-r--r--   0 root         (0) root         (0)     5212 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/copyfile.py
--rw-r--r--   0 root         (0) root         (0)     1158 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/decorators.py
--rw-r--r--   0 root         (0) root         (0)    33133 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/clusterondemand/eula.txt
--rw-r--r--   0 root         (0) root         (0)     1482 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10029 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/findclusters.py
--rw-r--r--   0 root         (0) root         (0)     2496 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/imagemanifest.py
--rw-r--r--   0 root         (0) root         (0)     3518 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/imagerepo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.397296 cm-cluster-on-demand-9.2.8/clusterondemand/images/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5110 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/distro_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.397296 cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2753 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/byid.py
--rw-r--r--   0 root         (0) root         (0)     1727 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/packagegroups.py
--rw-r--r--   0 root         (0) root         (0)     1085 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/tags.py
--rw-r--r--   0 root         (0) root         (0)    26243 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/find.py
--rw-r--r--   0 root         (0) root         (0)     4576 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/queryparser.py
--rw-r--r--   0 root         (0) root         (0)      938 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/images/utils.py
--rw-r--r--   0 root         (0) root         (0)     5608 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/imagetable.py
--rw-r--r--   0 root         (0) root         (0)     2089 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     4564 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/inbound_traffic_rule.py
--rw-r--r--   0 root         (0) root         (0)     2043 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/ip.py
--rw-r--r--   0 root         (0) root         (0)     1412 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/localpath.py
--rw-r--r--   0 root         (0) root         (0)     2084 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     3423 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/paramvalidation.py
--rw-r--r--   0 root         (0) root         (0)     2166 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/reporting_reader.py
--rw-r--r--   0 root         (0) root         (0)     7291 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/setup_logging.py
--rw-r--r--   0 root         (0) root         (0)    31163 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/ssh.py
--rw-r--r--   0 root         (0) root         (0)     5286 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/ssh_key.py
--rw-r--r--   0 root         (0) root         (0)     8223 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/summary.py
--rw-r--r--   0 root         (0) root         (0)     2583 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/tabcompletion_generate.py
--rw-r--r--   0 root         (0) root         (0)     3054 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/tags.py
--rw-r--r--   0 root         (0) root         (0)    20280 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/testutils.py
--rw-r--r--   0 root         (0) root         (0)     2150 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/text.py
--rw-r--r--   0 root         (0) root         (0)     5879 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/tracing.py
--rw-r--r--   0 root         (0) root         (0)    20843 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/utils.py
--rw-r--r--   0 root         (0) root         (0)      143 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/clusterondemand/version-info.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/version.py
--rw-r--r--   0 root         (0) root         (0)     1828 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/vlan.py
--rw-r--r--   0 root         (0) root         (0)     8558 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/clusterondemand/wait_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.401296 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1154 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2615 2022-12-27 18:19:24.000000 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      195 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2022-12-27 18:19:23.000000 cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.401296 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/image.py
--rw-r--r--   0 root         (0) root         (0)     4307 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:24.401296 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/tests/
--rw-r--r--   0 root         (0) root         (0)     1133 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/tests/image_repo_full.yaml
--rw-r--r--   0 root         (0) root         (0)       11 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/tests/image_repo_ver1.yaml
--rw-r--r--   0 root         (0) root         (0)       11 2022-12-27 18:19:08.000000 cm-cluster-on-demand-9.2.8/cmbrightimagerepo/tests/image_repo_ver2.yaml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 18:19:24.401296 cm-cluster-on-demand-9.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2657 2022-12-27 18:19:11.000000 cm-cluster-on-demand-9.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      614 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.587799 cm-cluster-on-demand-9.2.9/clusterondemand/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/clusterondemand/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-02-20 12:11:24.000000 cm-cluster-on-demand-9.2.9/clusterondemand/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/accept_eula.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/bcm_version.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/brightsetup.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cidr.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.587799 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/
+-rw-r--r--   0 root         (0) root         (0)      776 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/cloudconfig.py
+-rw-r--r--   0 root         (0) root         (0)     5720 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/headcommands.py
+-rw-r--r--   0 root         (0) root         (0)    11514 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/headfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/tests/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5849 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/clustercreate.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/clusternameprefix.py
+-rw-r--r--   0 root         (0) root         (0)    11756 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/cmclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/datetimefunctions.py
+-rw-r--r--   0 root         (0) root         (0)     7311 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/sortingutils.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/command_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/configdump.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/configshow.py
+-rw-r--r--   0 root         (0) root         (0)    22322 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5626 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/configuration_validation.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/const.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/contextmanagers.py
+-rw-r--r--   0 root         (0) root         (0)     5212 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/copyfile.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    33133 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/clusterondemand/eula.txt
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/findclusters.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/imagemanifest.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/imagerepo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/clusterondemand/images/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/distro_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/byid.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/packagegroups.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/tags.py
+-rw-r--r--   0 root         (0) root         (0)    26243 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/find.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/queryparser.py
+-rw-r--r--   0 root         (0) root         (0)      938 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/images/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/imagetable.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4564 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/inbound_traffic_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/ip.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/localpath.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/paramvalidation.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/reporting_reader.py
+-rw-r--r--   0 root         (0) root         (0)     7291 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/setup_logging.py
+-rw-r--r--   0 root         (0) root         (0)    31163 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     5286 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/ssh_key.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/summary.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/tabcompletion_generate.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20280 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/testutils.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/text.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/tracing.py
+-rw-r--r--   0 root         (0) root         (0)    20843 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/utils.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-02-20 12:11:24.000000 cm-cluster-on-demand-9.2.9/clusterondemand/version-info.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/version.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/vlan.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/clusterondemand/wait_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-02-20 12:11:25.000000 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-02-20 12:11:25.000000 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 12:11:25.000000 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-02-20 12:11:25.000000 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-02-20 12:11:25.000000 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-02-20 12:11:25.000000 cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/image.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/tests/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/tests/image_repo_full.yaml
+-rw-r--r--   0 root         (0) root         (0)       11 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/tests/image_repo_ver1.yaml
+-rw-r--r--   0 root         (0) root         (0)       11 2023-02-20 12:11:10.000000 cm-cluster-on-demand-9.2.9/cmbrightimagerepo/tests/image_repo_ver2.yaml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-20 12:11:25.591799 cm-cluster-on-demand-9.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-02-20 12:11:13.000000 cm-cluster-on-demand-9.2.9/setup.py
```

### Comparing `cm-cluster-on-demand-9.2.8/LICENSE` & `cm-cluster-on-demand-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-9.2.8/PKG-INFO` & `cm-cluster-on-demand-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Cluster on Demand Utility
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-9.2.8/__init__.py` & `cm-cluster-on-demand-9.2.9/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/__init__.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/accept_eula.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/accept_eula.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/bcm_version.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/bcm_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from six.moves import map
 
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/brightsetup.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/brightsetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cidr.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cidr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cli.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/__init__.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/cloudconfig.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/cloudconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/headcommands.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/headcommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/headfiles.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/headfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cloudconfig/tests/__init__.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cloudconfig/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/clustercreate.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/clustercreate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/clusternameprefix.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/clusternameprefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/cmclient.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/cmclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/__init__.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/datetimefunctions.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/datetimefunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/codoutput/sortingutils.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/codoutput/sortingutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/command_runner.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/command_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/configdump.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/configdump.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/configshow.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/configshow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/configuration.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -443,14 +443,19 @@
     "output_format",
     flags=["-f"],
     default="table",
     choices=["table", "csv", "value", "yaml"],
     help="Output format for lists")
 
 sshconfig_ns = ConfigNamespace("sshconfig", "SSH local configuration")
+sshconfig_ns.add_parameter(
+    "ssh_config_path",
+    help="Path to local ssh config to save COD cluster ssh configuration in.",
+    default="~/.ssh/config",
+)
 sshconfig_ns.add_switch_parameter(
     "update_ssh_config",
     help="Updates the contents of ~/.ssh/config, this is used to maintain the local ssh configuration "
          "access with ssh, scp and related tools.",
 )
 sshconfig_ns.add_parameter(
     "ssh_config_alias_prefix",
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/configuration_validation.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/configuration_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/const.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/contextmanagers.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/contextmanagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/copyfile.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/copyfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/decorators.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/eula.txt` & `cm-cluster-on-demand-9.2.9/clusterondemand/eula.txt`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/exceptions.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/findclusters.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/findclusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/imagemanifest.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/imagemanifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/imagerepo.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/imagerepo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/__init__.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/distro_family.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/distro_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/__init__.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/byid.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/byid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/packagegroups.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/packagegroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/filters/tags.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/filters/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/find.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/find.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/queryparser.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/queryparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/images/utils.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/images/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/imagetable.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/imagetable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/import_utils.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/inbound_traffic_rule.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/inbound_traffic_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/ip.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/localpath.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/localpath.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/node_definition.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/node_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/paramvalidation.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/paramvalidation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/reporting_reader.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/reporting_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/setup_logging.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/setup_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/ssh.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/ssh_key.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/ssh_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/summary.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/tabcompletion_generate.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/tabcompletion_generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/tags.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/testutils.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/testutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/text.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/tracing.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/utils.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/version.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/vlan.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/vlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/clusterondemand/wait_helpers.py` & `cm-cluster-on-demand-9.2.9/clusterondemand/wait_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/PKG-INFO` & `cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Cluster on Demand Utility
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-9.2.8/cm_cluster_on_demand.egg-info/SOURCES.txt` & `cm-cluster-on-demand-9.2.9/cm_cluster_on_demand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-9.2.8/cmbrightimagerepo/__init__.py` & `cm-cluster-on-demand-9.2.9/cmbrightimagerepo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/cmbrightimagerepo/image.py` & `cm-cluster-on-demand-9.2.9/cmbrightimagerepo/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/cmbrightimagerepo/repository.py` & `cm-cluster-on-demand-9.2.9/cmbrightimagerepo/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-9.2.8/cmbrightimagerepo/tests/image_repo_full.yaml` & `cm-cluster-on-demand-9.2.9/cmbrightimagerepo/tests/image_repo_full.yaml`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-9.2.8/setup.py` & `cm-cluster-on-demand-9.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

