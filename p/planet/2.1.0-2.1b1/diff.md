# Comparing `tmp/planet-2.1.0.tar.gz` & `tmp/planet-2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-ytumiqim/planet-2.1.0.tar", last modified: Tue Jul 18 00:09:19 2023, max compression
+gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-vjwgfjic/planet-2.1b1.tar", last modified: Wed Jul 12 03:28:40 2023, max compression
```

## Comparing `planet-2.1.0.tar` & `planet-2.1b1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:09:19.000000 planet-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-18 00:08:56.000000 planet-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-18 00:09:19.000000 planet-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-18 00:08:56.000000 planet-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:09:19.000000 planet-2.1.0/planet/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 00:08:56.000000 planet-2.1.0/planet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 00:08:56.000000 planet-2.1.0/planet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-18 00:08:56.000000 planet-2.1.0/planet/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:09:19.000000 planet-2.1.0/planet/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-18 00:08:56.000000 planet-2.1.0/planet/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:09:19.000000 planet-2.1.0/planet/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 00:08:56.000000 planet-2.1.0/planet/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-07-18 00:08:56.000000 planet-2.1.0/planet/clients/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17602 2023-07-18 00:08:56.000000 planet-2.1.0/planet/clients/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-18 00:08:56.000000 planet-2.1.0/planet/clients/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-18 00:08:56.000000 planet-2.1.0/planet/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:09:19.000000 planet-2.1.0/planet/data/
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-18 00:08:56.000000 planet-2.1.0/planet/data/Feature.json
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 00:08:56.000000 planet-2.1.0/planet/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-07-18 00:08:56.000000 planet-2.1.0/planet/data/orders_product_bundle_2023-02-24.json
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-18 00:08:56.000000 planet-2.1.0/planet/data_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-18 00:08:56.000000 planet-2.1.0/planet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 00:08:56.000000 planet-2.1.0/planet/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-18 00:08:56.000000 planet-2.1.0/planet/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-18 00:08:56.000000 planet-2.1.0/planet/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-18 00:08:56.000000 planet-2.1.0/planet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-07-18 00:08:56.000000 planet-2.1.0/planet/order_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-18 00:08:56.000000 planet-2.1.0/planet/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-18 00:08:56.000000 planet-2.1.0/planet/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23853 2023-07-18 00:08:56.000000 planet-2.1.0/planet/subscription_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 00:09:19.000000 planet-2.1.0/planet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-18 00:09:19.000000 planet-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-18 00:08:56.000000 planet-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:40.000000 planet-2.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-12 03:28:22.000000 planet-2.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-12 03:28:40.000000 planet-2.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-12 03:28:22.000000 planet-2.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:40.000000 planet-2.1b1/planet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-12 03:28:22.000000 planet-2.1b1/planet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 03:28:22.000000 planet-2.1b1/planet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-12 03:28:22.000000 planet-2.1b1/planet/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:40.000000 planet-2.1b1/planet/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-12 03:28:22.000000 planet-2.1b1/planet/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:40.000000 planet-2.1b1/planet/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-12 03:28:22.000000 planet-2.1b1/planet/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-07-12 03:28:22.000000 planet-2.1b1/planet/clients/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17602 2023-07-12 03:28:22.000000 planet-2.1b1/planet/clients/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-12 03:28:22.000000 planet-2.1b1/planet/clients/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 03:28:22.000000 planet-2.1b1/planet/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:40.000000 planet-2.1b1/planet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-12 03:28:22.000000 planet-2.1b1/planet/data/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-12 03:28:22.000000 planet-2.1b1/planet/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-07-12 03:28:22.000000 planet-2.1b1/planet/data/orders_product_bundle_2023-02-24.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-12 03:28:22.000000 planet-2.1b1/planet/data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-12 03:28:22.000000 planet-2.1b1/planet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-12 03:28:22.000000 planet-2.1b1/planet/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-12 03:28:22.000000 planet-2.1b1/planet/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 03:28:22.000000 planet-2.1b1/planet/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 03:28:22.000000 planet-2.1b1/planet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-12 03:28:22.000000 planet-2.1b1/planet/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-12 03:28:22.000000 planet-2.1b1/planet/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-12 03:28:22.000000 planet-2.1b1/planet/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-07-12 03:28:22.000000 planet-2.1b1/planet/subscription_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 03:28:40.000000 planet-2.1b1/planet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 03:28:40.000000 planet-2.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-12 03:28:22.000000 planet-2.1b1/setup.py
```

### Comparing `planet-2.1.0/LICENSE` & `planet-2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/PKG-INFO` & `planet-2.1b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.1.0
+Version: 2.1b1
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.1.0/README.md` & `planet-2.1b1/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/__init__.py` & `planet-2.1b1/planet/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/auth.py` & `planet-2.1b1/planet/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/auth.py` & `planet-2.1b1/planet/cli/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/cli.py` & `planet-2.1b1/planet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/cmds.py` & `planet-2.1b1/planet/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/collect.py` & `planet-2.1b1/planet/cli/collect.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/data.py` & `planet-2.1b1/planet/cli/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/io.py` & `planet-2.1b1/planet/cli/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/options.py` & `planet-2.1b1/planet/cli/options.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/cli/orders.py` & `planet-2.1b1/planet/cli/orders.py`

 * *Files 6% similar despite different names*

```diff
@@ -249,35 +249,19 @@
     type=types.JSON(),
     help="""Toolchain JSON. Can be a json string, filename, or '-' for
     stdin.""")
 @click.option('--email',
               default=False,
               is_flag=True,
               help='Send email notification when order is complete.')
-@click.option('--archive-type',
-              type=click.Choice(['zip']),
-              help="Optionally zip archive each item bundle.")
-@click.option('--archive-filename',
-              default='{{name}}-{{order_id}}.zip',
-              show_default=True,
-              help="Templated filename for archived bundles or orders.")
-@click.option('--single-archive',
-              is_flag=True,
-              default=False,
-              show_default=True,
-              help="Optionally zip archive all item bundles together.")
 @click.option(
-    '--delivery',
     '--cloudconfig',
     type=types.JSON(),
-    help=("Delivery configuration, which may include credentials for a cloud "
-          "storage provider, to enable cloud delivery of data, and/or "
-          "parameters for bundling deliveries as zip archives. Can be a JSON "
-          "string, a filename, or '-' for stdin. The --cloudconfig option is "
-          "an alias for this use case."))
+    help="""Credentials for cloud storage provider to enable cloud delivery of
+    data. Can be a json string, filename, or '-' for stdin.""")
 @click.option(
     '--stac/--no-stac',
     default=True,
     is_flag=True,
     help="""Include or exclude metadata in SpatioTemporal Asset Catalog (STAC)
     format. Not specifying either defaults to including it (--stac), except
     for orders with google_earth_engine delivery""")
@@ -286,18 +270,15 @@
                   item_type,
                   bundle,
                   name,
                   ids,
                   clip,
                   tools,
                   email,
-                  archive_type,
-                  archive_filename,
-                  single_archive,
-                  delivery,
+                  cloudconfig,
                   stac,
                   pretty):
     """Generate an order request.
 
     This command provides support for building an order description used
     in creating an order. It outputs the order request, optionally
     pretty-printed.
@@ -318,20 +299,22 @@
         raise click.BadParameter("Specify only one of '--clip' or '--tools'")
     elif clip:
         try:
             tools = [planet.order_request.clip_tool(clip)]
         except planet.exceptions.ClientError as e:
             raise click.BadParameter(e)
 
-    delivery = planet.order_request.delivery(archive_type=archive_type,
-                                             archive_filename=archive_filename,
-                                             single_archive=single_archive,
-                                             cloud_config=delivery)
+    if cloudconfig:
+        delivery = planet.order_request.delivery(cloud_config=cloudconfig)
+        if "google_earth_engine" in cloudconfig:
+            stac = False
+    else:
+        delivery = None
 
-    if stac and "google_earth_engine" not in delivery:
+    if stac:
         stac_json = {'stac': {}}
     else:
         stac_json = {}
 
     request = planet.order_request.build_request(name,
                                                  products=[product],
                                                  delivery=delivery,
```

### Comparing `planet-2.1.0/planet/cli/subscriptions.py` & `planet-2.1b1/planet/cli/subscriptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -222,55 +222,34 @@
               required=True,
               type=str,
               help='Subscription name. Does not need to be unique.')
 @click.option('--source',
               required=True,
               type=types.JSON(),
               help='Source JSON. Can be a string, filename, or - for stdin.')
-@click.option(
-    '--delivery',
-    required=True,
-    type=types.JSON(),
-    help=("Delivery configuration, including credentials for a cloud "
-          "storage provider, to enable cloud delivery of data. Can be a "
-          "JSON string, a filename, or '-' for stdin. "))
+@click.option('--delivery',
+              required=True,
+              type=types.JSON(),
+              help='Delivery JSON. Can be a string, filename, or - for stdin.')
 @click.option(
     '--notifications',
     type=types.JSON(),
     help='Notifications JSON. Can be a string, filename, or - for stdin.')
 @click.option(
     '--tools',
     type=types.JSON(),
     help='Toolchain JSON. Can be a string, filename, or - for stdin.')
-@click.option(
-    '--clip-to-source',
-    is_flag=True,
-    default=False,
-    help="Clip to the source geometry without specifying a clip tool.")
 @pretty
-def request(name,
-            source,
-            delivery,
-            notifications,
-            tools,
-            clip_to_source,
-            pretty):
-    """Generate a subscriptions request.
-
-    Note: the next version of the Subscription API will remove the clip
-    tool option and always clip to the source geometry. Thus the
-    --clip-to-source option is a preview of the next API version's
-    default behavior.
-    """
+def request(name, source, delivery, notifications, tools, pretty):
+    """Generate a subscriptions request."""
     res = subscription_request.build_request(name,
                                              source,
                                              delivery,
                                              notifications=notifications,
-                                             tools=tools,
-                                             clip_to_source=clip_to_source)
+                                             tools=tools)
     echo_json(res, pretty)
 
 
 @subscriptions.command(epilog=valid_item_string)  # type: ignore
 @translate_exceptions
 @click.option('--item-types',
               required=True,
@@ -297,86 +276,25 @@
 @click.option('--rrule',
               type=str,
               help='iCalendar recurrance rule to specify recurrances.')
 @click.option(
     '--filter',
     type=types.JSON(),
     help='Search filter.  Can be a string, filename, or - for stdin.')
-@click.option(
-    '--publishing-stage',
-    'publishing_stages',
-    type=click.Choice(["preview", "standard", "finalized"]),
-    multiple=True,
-    help=("Subscribe to results at a particular publishing stage. Multiple "
-          "instances of this option are allowed."))
-@click.option('--time-range-type',
-              type=click.Choice(["acquired", "published"]),
-              help="Subscribe by acquisition time or time of publication.")
 @pretty
 def request_catalog(item_types,
                     asset_types,
                     geometry,
                     start_time,
                     end_time,
                     rrule,
                     filter,
-                    publishing_stages,
-                    time_range_type,
                     pretty):
     """Generate a subscriptions request catalog source description."""
-    res = subscription_request.catalog_source(
-        item_types,
-        asset_types,
-        geometry,
-        start_time,
-        end_time=end_time,
-        rrule=rrule,
-        filter=filter,
-        publishing_stages=publishing_stages,
-        time_range_type=time_range_type)
-    echo_json(res, pretty)
-
-
-@subscriptions.command()  # type: ignore
-@translate_exceptions
-@click.option(
-    '--var-type',
-    required=True,
-    help='Planetary variable type.',
-    type=click.Choice([
-        "biomass_proxy",
-        "land_surface_temperature",
-        "soil_water_content",
-        "vegetation_optical_depth"
-    ]),
-)
-@click.option('--var-id', required=True, help='Planetary variable id.')
-@click.option(
-    '--geometry',
-    required=True,
-    type=types.JSON(),
-    help="""Geometry of the area of interest of the subscription that will be
-    used to determine matches. Can be a string, filename, or - for stdin.""")
-@click.option('--start-time',
-              required=True,
-              type=types.DateTime(),
-              help='Date and time to begin subscription.')
-@click.option('--end-time',
-              type=types.DateTime(),
-              help='Date and time to end subscription.')
-@pretty
-def request_pv(var_type, var_id, geometry, start_time, end_time, pretty):
-    """Generate a Planetary Variable subscription source.
-
-    Planetary Variables come in 4 types and are further subdivided
-    within these types. See [Subscribing to Planetary
-    Variables](https://developers.planet.com/docs/subscriptions/pvs-subs/#planetary-variables-types-and-ids)
-    for details.
-    """
-    res = subscription_request.planetary_variable_source(
-        var_type,
-        var_id,
-        geometry,
-        start_time,
-        end_time=end_time,
-    )
+    res = subscription_request.catalog_source(item_types,
+                                              asset_types,
+                                              geometry,
+                                              start_time,
+                                              end_time=end_time,
+                                              rrule=rrule,
+                                              filter=filter)
     echo_json(res, pretty)
```

### Comparing `planet-2.1.0/planet/cli/types.py` & `planet-2.1b1/planet/cli/types.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/clients/__init__.py` & `planet-2.1b1/planet/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/clients/data.py` & `planet-2.1b1/planet/clients/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/clients/orders.py` & `planet-2.1b1/planet/clients/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/clients/subscriptions.py` & `planet-2.1b1/planet/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/constants.py` & `planet-2.1b1/planet/constants.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/data/Feature.json` & `planet-2.1b1/planet/data/Feature.json`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/data/README.md` & `planet-2.1b1/planet/data/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/data/orders_product_bundle_2023-02-24.json` & `planet-2.1b1/planet/data/orders_product_bundle_2023-02-24.json`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/data_filter.py` & `planet-2.1b1/planet/data_filter.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/exceptions.py` & `planet-2.1b1/planet/exceptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/geojson.py` & `planet-2.1b1/planet/geojson.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/http.py` & `planet-2.1b1/planet/http.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/io.py` & `planet-2.1b1/planet/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/models.py` & `planet-2.1b1/planet/models.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/order_request.py` & `planet-2.1b1/planet/order_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """Functionality for preparing order details for use in creating an order"""
 from __future__ import annotations  # https://stackoverflow.com/a/33533514
 import logging
-from typing import Any, Dict, List, Mapping, Optional, Union
+from typing import Optional, Any, Dict, List, Union
 
 from . import geojson, specs
 from .exceptions import ClientError
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -159,17 +159,17 @@
         val: bool = email
         notifications_dict['email'] = val
 
     return notifications_dict
 
 
 def delivery(archive_type: Optional[str] = None,
-             single_archive: Optional[bool] = False,
+             single_archive: bool = False,
              archive_filename: Optional[str] = None,
-             cloud_config: Optional[Mapping] = None) -> dict:
+             cloud_config: Optional[dict] = None) -> dict:
     """Order delivery configuration.
 
     Example:
         ```python
         amazon_s3_config = amazon_s3(
             'access_key',
             'secret_access_key',
@@ -192,29 +192,24 @@
             archive file that is received. Uses the template variables
             {{name}} and {{order_id}}. e.g. "{{name}}_{{order_id}}.zip".
         cloud_config: Cloud delivery configuration.
 
     Raises:
         planet.specs.SpecificationException: If archive_type is not valid.
     """
-    config: Dict[str, Any] = {}
-
     if archive_type:
         archive_type = specs.validate_archive_type(archive_type)
 
-        if archive_filename is None:
-            archive_filename = "{{name}}_{{order_id}}.zip"
+    fields = ['archive_type', 'single_archive', 'archive_filename']
+    values = [archive_type, single_archive, archive_filename]
 
-        config.update(archive_type=archive_type,
-                      archive_filename=archive_filename,
-                      single_archive=single_archive)
+    config = dict((k, v) for k, v in zip(fields, values) if v)
 
     if cloud_config:
         config.update(cloud_config)
-
     return config
 
 
 def amazon_s3(aws_access_key_id: str,
               aws_secret_access_key: str,
               bucket: str,
               aws_region: str,
```

### Comparing `planet-2.1.0/planet/reporting.py` & `planet-2.1b1/planet/reporting.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/specs.py` & `planet-2.1b1/planet/specs.py`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/planet/subscription_request.py` & `planet-2.1b1/planet/subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
     details = {
         "name": name, "source": dict(source), "delivery": dict(delivery)
     }
 
     if notifications:
         details['notifications'] = dict(notifications)
 
-    if tools or clip_to_source:
-        tool_list = [dict(tool) for tool in (tools or [])]
+    if tools:
+        tool_list = [dict(tool) for tool in tools]
 
         # If clip_to_source is True a clip configuration will be added
         # to the list of requested tools unless an existing clip tool
         # exists. In that case an exception is raised. NOTE: the next
         # version of the Subscription API will remove the clip tool
         # option and always clip to the source geometry. Thus this is a
         # preview of the next API version's default behavior.
```

### Comparing `planet-2.1.0/planet.egg-info/PKG-INFO` & `planet-2.1b1/planet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.1.0
+Version: 2.1b1
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.1.0/planet.egg-info/SOURCES.txt` & `planet-2.1b1/planet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planet-2.1.0/setup.py` & `planet-2.1b1/setup.py`

 * *Files identical despite different names*

