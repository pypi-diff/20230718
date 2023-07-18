# Comparing `tmp/mapchete-2023.7.0.tar.gz` & `tmp/mapchete-2023.7.1.tar.gz`

## Comparing `mapchete-2023.7.0.tar` & `mapchete-2023.7.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/__init__.py
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_core.py
--rw-r--r--   0        0        0    25534 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_registered.py
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/_user_process.py
--rw-r--r--   0        0        0    49580 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/errors.py
--rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/log.py
--rw-r--r--   0        0        0    25327 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/path.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/stac.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/testing.py
--rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/tile.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/types.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/main.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_json.py
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_misc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/_path.py
--rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/raster.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/settings.py
--rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.7.0/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.7.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.7.0/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.7.0/README.rst
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 mapchete-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 mapchete-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/__init__.py
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_core.py
+-rw-r--r--   0        0        0    25534 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_registered.py
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/_user_process.py
+-rw-r--r--   0        0        0    49580 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/errors.py
+-rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/log.py
+-rw-r--r--   0        0        0    25327 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/path.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/stac.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/testing.py
+-rw-r--r--   0        0        0    17045 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/tile.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    16135 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/raster.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/settings.py
+-rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.7.1/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.7.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.7.1/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.7.1/README.rst
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 mapchete-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 mapchete-2023.7.1/PKG-INFO
```

### Comparing `mapchete-2023.7.0/mapchete/__init__.py` & `mapchete-2023.7.1/mapchete/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.7.0"
+__version__ = "2023.7.1"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.7.0/mapchete/_core.py` & `mapchete-2023.7.1/mapchete/_core.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/_executor.py` & `mapchete-2023.7.1/mapchete/_executor.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/_processing.py` & `mapchete-2023.7.1/mapchete/_processing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/_registered.py` & `mapchete-2023.7.1/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/_tasks.py` & `mapchete-2023.7.1/mapchete/_tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/_timer.py` & `mapchete-2023.7.1/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/_user_process.py` & `mapchete-2023.7.1/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/config.py` & `mapchete-2023.7.1/mapchete/config.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/errors.py` & `mapchete-2023.7.1/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/index.py` & `mapchete-2023.7.1/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/log.py` & `mapchete-2023.7.1/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/path.py` & `mapchete-2023.7.1/mapchete/path.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/stac.py` & `mapchete-2023.7.1/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/testing.py` & `mapchete-2023.7.1/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/tile.py` & `mapchete-2023.7.1/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/types.py` & `mapchete-2023.7.1/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/validate.py` & `mapchete-2023.7.1/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/options.py` & `mapchete-2023.7.1/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/convert.py` & `mapchete-2023.7.1/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/cp.py` & `mapchete-2023.7.1/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/execute.py` & `mapchete-2023.7.1/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/formats.py` & `mapchete-2023.7.1/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/index.py` & `mapchete-2023.7.1/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/processes.py` & `mapchete-2023.7.1/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/rm.py` & `mapchete-2023.7.1/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/serve.py` & `mapchete-2023.7.1/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/cli/default/stac.py` & `mapchete-2023.7.1/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commands/_convert.py` & `mapchete-2023.7.1/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commands/_cp.py` & `mapchete-2023.7.1/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commands/_execute.py` & `mapchete-2023.7.1/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commands/_index.py` & `mapchete-2023.7.1/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commands/_rm.py` & `mapchete-2023.7.1/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commons/clip.py` & `mapchete-2023.7.1/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commons/contours.py` & `mapchete-2023.7.1/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/commons/hillshade.py` & `mapchete-2023.7.1/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/__init__.py` & `mapchete-2023.7.1/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/base.py` & `mapchete-2023.7.1/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/loaders.py` & `mapchete-2023.7.1/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/tools.py` & `mapchete-2023.7.1/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.7.1/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.7.1/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/geobuf.py` & `mapchete-2023.7.1/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/geojson.py` & `mapchete-2023.7.1/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/gtiff.py` & `mapchete-2023.7.1/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.7.1/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/png.py` & `mapchete-2023.7.1/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.7.1/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/raster_file.py` & `mapchete-2023.7.1/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/formats/default/tile_directory.py` & `mapchete-2023.7.1/mapchete/formats/default/tile_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,16 +388,20 @@
         tile_directory_zoom=None,
         fallback_to_higher_zoom=False,
         matching_method="gdal",
         matching_precision=8,
         matching_max_zoom=None,
     ):
         # determine tile bounds in TileDirectory CRS
+        # NOTE: because fiona/OGR cannot handle geometries crossing the antimeridian,
+        # we have to clip the source bounds to the CRS bounds.
         _geom = reproject_geometry(
-            self.tile.bbox, src_crs=self.tile.tp.crs, dst_crs=self._td_pyramid.crs
+            self.tile.bbox.intersection(box(*self.tile.buffered_tp.bounds)),
+            src_crs=self.tile.tp.crs,
+            dst_crs=self._td_pyramid.crs,
         )
         if _geom.is_empty:  # pragma: no cover
             logger.debug(
                 "tile %s reprojected to %s is empty", self.tile, self._td_pyramid
             )
             return []
         td_bounds = _geom.bounds
@@ -410,15 +414,14 @@
                 matching_method=matching_method,
                 precision=matching_precision,
             )
             if matching_max_zoom is not None:
                 zoom = min([zoom, matching_max_zoom])
         else:
             zoom = tile_directory_zoom
-
         if fallback_to_higher_zoom:
             tiles_paths = []
             # check if tiles exist otherwise try higher zoom level
             while len(tiles_paths) == 0 and zoom >= 0:
                 tiles_paths = _get_tiles_paths(
                     basepath=self._basepath,
                     ext=self._ext,
```

### Comparing `mapchete-2023.7.0/mapchete/formats/default/vector_file.py` & `mapchete-2023.7.1/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/__init__.py` & `mapchete-2023.7.1/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/_geometry_operations.py` & `mapchete-2023.7.1/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/_json.py` & `mapchete-2023.7.1/mapchete/io/_json.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/_misc.py` & `mapchete-2023.7.1/mapchete/io/_misc.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/raster.py` & `mapchete-2023.7.1/mapchete/io/raster.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/settings.py` & `mapchete-2023.7.1/mapchete/io/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/io/vector.py` & `mapchete-2023.7.1/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/processes/__init__.py` & `mapchete-2023.7.1/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/processes/contours.py` & `mapchete-2023.7.1/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/processes/convert.py` & `mapchete-2023.7.1/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/processes/hillshade.py` & `mapchete-2023.7.1/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/processes/examples/example_process.py` & `mapchete-2023.7.1/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/static/index.html` & `mapchete-2023.7.1/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/mapchete/static/process_template.py` & `mapchete-2023.7.1/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/LICENSE` & `mapchete-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/README.rst` & `mapchete-2023.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/pyproject.toml` & `mapchete-2023.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2023.7.0/PKG-INFO` & `mapchete-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

