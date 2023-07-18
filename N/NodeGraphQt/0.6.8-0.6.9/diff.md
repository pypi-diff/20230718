# Comparing `tmp/NodeGraphQt-0.6.8.tar.gz` & `tmp/NodeGraphQt-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.6.8.tar", last modified: Fri Jul 14 08:11:28 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.9.tar", last modified: Tue Jul 18 09:34:49 2023, max compression
```

## Comparing `NodeGraphQt-0.6.8.tar` & `NodeGraphQt-0.6.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.608956 NodeGraphQt-0.6.8/NodeGraphQt/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.612956 NodeGraphQt-0.6.8/NodeGraphQt/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)   101486 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.612956 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.616956 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.616956 NodeGraphQt-0.6.8/NodeGraphQt/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/backdrop_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/port_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/pkg_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_backdrop.py
--rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_text_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/NodeGraphQt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/NodeGraphQt/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/icons/node_base.png
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/tab_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    54896 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer_nav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.612956 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.608956 NodeGraphQt-0.6.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/examples/hotkeys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/hotkeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/hotkeys/hotkey_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/examples/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/basic_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/custom_ports_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/widget_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 08:11:28.624957 NodeGraphQt-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.548896 NodeGraphQt-0.6.9/NodeGraphQt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.552896 NodeGraphQt-0.6.9/NodeGraphQt/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101486 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/base/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.552896 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.552896 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.552896 NodeGraphQt-0.6.9/NodeGraphQt/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/nodes/backdrop_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/nodes/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/nodes/base_node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/nodes/port_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/pkg_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_port_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_port_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_text_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/NodeGraphQt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/NodeGraphQt/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/icons/node_base.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/node_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/node_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/tab_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54896 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/NodeGraphQt/widgets/viewer_nav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.548896 NodeGraphQt-0.6.9/NodeGraphQt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-18 09:34:49.000000 NodeGraphQt-0.6.9/NodeGraphQt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-18 09:34:49.000000 NodeGraphQt-0.6.9/NodeGraphQt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:34:49.000000 NodeGraphQt-0.6.9/NodeGraphQt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:34:49.000000 NodeGraphQt-0.6.9/NodeGraphQt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 09:34:49.000000 NodeGraphQt-0.6.9/NodeGraphQt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.548896 NodeGraphQt-0.6.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/examples/hotkeys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/hotkeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/hotkeys/hotkey_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/examples/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/nodes/basic_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/nodes/custom_ports_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/examples/nodes/widget_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 09:34:49.556896 NodeGraphQt-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 09:34:41.000000 NodeGraphQt-0.6.9/setup.py
```

### Comparing `NodeGraphQt-0.6.8/LICENSE.md` & `NodeGraphQt-0.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.9/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,15 +389,15 @@
 
         Args:
             name (str): name of the property.
             value (object): property data (python built in types).
             push_undo (bool): register the command to the undo stack. (default: True)
         """
 
-        # prevent signals from causing a infinite loop.
+        # prevent signals from causing an infinite loop.
         if self.get_property(name) == value:
             return
 
         # prevent nodes from have the same name.
         if self.graph and name == 'name':
             value = self.graph.get_unique_name(value)
             self.NODE_NAME = value
```

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/base/port.py` & `NodeGraphQt-0.6.9/NodeGraphQt/base/port.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,19 @@
         """
         Sets weather the port should be visible or not.
 
         Args:
             visible (bool): true if visible.
             push_undo (bool): register the command to the undo stack. (default: True)
         """
+
+        # prevent signals from causing an infinite loop.
+        if visible == self.visible():
+            return
+
         undo_cmd = PortVisibleCmd(self, visible)
         if push_undo:
             undo_stack = self.node().graph.undo_stack()
             undo_stack.push(undo_cmd)
         else:
             undo_cmd.redo()
 
@@ -161,16 +166,20 @@
         Sets the port locked state. When locked pipe connections can't be
         connected or disconnected from this port.
 
         Args:
             state (Bool): port lock state.
             connected_ports (Bool): apply to lock state to connected ports.
             push_undo (bool): register the command to the undo stack. (default: True)
-
         """
+
+        # prevent signals from causing an infinite loop.
+        if state == self.locked():
+            return
+
         graph = self.node().graph
         undo_stack = graph.undo_stack()
         if state:
             undo_cmd = PortLockedCmd(self)
         else:
             undo_cmd = PortUnlockedCmd(self)
         if push_undo:
@@ -436,15 +445,15 @@
 
         Args:
             port_name (str): name of the port.
             port_type (str): port type.
             node_type (str): port node type.
         """
         # storing the connection constrain at the graph level instead of the
-        # port level so we don't serialize the same data for every port
+        # port level, so we don't serialize the same data for every port
         # instance.
         self.node().add_reject_port_type(
             port=self,
             port_type_data={
                 'port_name': port_name,
                 'port_type': port_type,
                 'node_type': node_type,
```

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.9/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,62 +137,57 @@
 
 class _PortConnectionsContainer(QtWidgets.QWidget):
     """
     Port connection container widget that displays node ports and connections
     under a tab in the ``NodePropWidget`` widget.
     """
 
-    ingroup_visible_toggled = QtCore.Signal(bool)
-    outgroup_visible_toggled = QtCore.Signal(bool)
-
     def __init__(self, parent=None, node=None):
         super(_PortConnectionsContainer, self).__init__(parent)
         self._node = node
         self._ports = {}
 
-        in_group, self.in_tree = self._build_tree_group('Input Ports')
-        in_group.setToolTip('Display input port connections')
+        self.input_group, self.input_tree = self._build_tree_group(
+            'Input Ports'
+        )
+        self.input_group.setToolTip('Display input port connections')
         for _, port in node.inputs().items():
-            self._build_row(self.in_tree, port)
-        for col in range(self.in_tree.columnCount()):
-            self.in_tree.resizeColumnToContents(col)
+            self._build_row(self.input_tree, port)
+        for col in range(self.input_tree.columnCount()):
+            self.input_tree.resizeColumnToContents(col)
 
-        out_group, self.out_tree = self._build_tree_group('Output Ports')
-        out_group.setToolTip('Display output port connections')
+        self.output_group, self.output_tree = self._build_tree_group(
+            'Output Ports'
+        )
+        self.output_group.setToolTip('Display output port connections')
         for _, port in node.outputs().items():
-            self._build_row(self.out_tree, port)
-        for col in range(self.out_tree.columnCount()):
-            self.out_tree.resizeColumnToContents(col)
+            self._build_row(self.output_tree, port)
+        for col in range(self.output_tree.columnCount()):
+            self.output_tree.resizeColumnToContents(col)
 
         layout = QtWidgets.QVBoxLayout(self)
-        layout.addWidget(in_group)
-        layout.addWidget(out_group)
+        layout.addWidget(self.input_group)
+        layout.addWidget(self.output_group)
         layout.addStretch()
 
-        # wire up signals & slots
-        in_group.clicked.connect(
-            lambda x: self.ingroup_visible_toggled.emit(x)
-        )
-        out_group.clicked.connect(
-            lambda x: self.outgroup_visible_toggled.emit(x)
-        )
-
-        in_group.setChecked(False)
-        self.in_tree.setVisible(False)
-        out_group.setChecked(False)
-        self.out_tree.setVisible(False)
+        self.input_group.setChecked(False)
+        self.input_tree.setVisible(False)
+        self.output_group.setChecked(False)
+        self.output_tree.setVisible(False)
 
     def __repr__(self):
         return '<{} object at {}>'.format(
             self.__class__.__name__, hex(id(self))
         )
 
     @staticmethod
     def _build_tree_group(title):
         """
+        Build the ports group box and ports tree widget.
+
         Args:
             title (str): group box title.
 
         Returns:
             tuple(QtWidgets.QGroupBox, QtWidgets.QTreeWidget): widgets.
         """
         group_box = QtWidgets.QGroupBox()
@@ -214,17 +209,19 @@
 
         group_box.layout().addWidget(tree_widget)
 
         return group_box, tree_widget
 
     def _build_row(self, tree, port):
         """
+        Builds a new row in the parent ports tree widget.
+
         Args:
-            tree (QtWidgets.QTreeWidget):
-            port (NodeGraphQt.Port):
+            tree (QtWidgets.QTreeWidget): parent port tree widget.
+            port (NodeGraphQt.Port): port object.
         """
         item = QtWidgets.QTreeWidgetItem(tree)
         item.setFlags(item.flags() & ~QtCore.Qt.ItemIsSelectable)
         item.setText(1, port.name())
         item.setToolTip(0, 'Lock Port')
         item.setToolTip(1, 'Port Name')
         item.setToolTip(2, 'Select connected port.')
@@ -241,23 +238,23 @@
         for cp in port.connected_ports():
             item_name = '{} : "{}"'.format(cp.name(), cp.node().name())
             self._ports[item_name] = cp
             combo.addItem(item_name)
         tree.setItemWidget(item, 2, combo)
 
         focus_btn = QtWidgets.QPushButton()
-        focus_btn.setIcon(QtGui.QIcon(tree.style().standardPixmap(
-            QtWidgets.QStyle.SP_DialogYesButton
-        )))
+        focus_btn.setIcon(QtGui.QIcon(
+            tree.style().standardPixmap(QtWidgets.QStyle.SP_DialogYesButton)
+        ))
         focus_btn.clicked.connect(
-            lambda: self._on_focus_on_node(self._ports.get(combo.currentText()))
+            lambda: self._on_focus_to_node(self._ports.get(combo.currentText()))
         )
         tree.setItemWidget(item, 3, focus_btn)
 
-    def _on_focus_on_node(self, port):
+    def _on_focus_to_node(self, port):
         """
         Slot function emits the node is of the connected port.
 
         Args:
             port (NodeGraphQt.Port): connected port.
         """
         if port:
@@ -276,17 +273,14 @@
         node (NodeGraphQt.BaseNode): node.
     """
 
     #: signal (node_id, prop_name, prop_value)
     property_changed = QtCore.Signal(str, str, object)
     property_closed = QtCore.Signal(str)
 
-    # emitted when a widget is shown or hidden. (node_id, visible, widget)
-    widget_visible_changed = QtCore.Signal(str, bool, QtWidgets.QWidget)
-
     def __init__(self, parent=None, node=None):
         super(NodePropWidget, self).__init__(parent)
         self.__node_id = node.id
         self.__tab_windows = {}
         self.__tab = QtWidgets.QTabWidget()
 
         close_btn = QtWidgets.QPushButton()
@@ -318,25 +312,15 @@
         name_layout.addWidget(close_btn)
         layout = QtWidgets.QVBoxLayout(self)
         layout.setSpacing(4)
         layout.addLayout(name_layout)
         layout.addWidget(self.__tab)
         layout.addWidget(self.type_wgt)
 
-        self._ports_container = self._read_node(node)
-        self._ports_container.ingroup_visible_toggled.connect(
-            lambda v: self.widget_visible_changed.emit(
-                self.__node_id, v, self._ports_container.in_tree
-            )
-        )
-        self._ports_container.outgroup_visible_toggled.connect(
-            lambda v: self.widget_visible_changed.emit(
-                self.__node_id, v, self._ports_container.out_tree
-            )
-        )
+        self._port_connections = self._read_node(node)
 
     def __repr__(self):
         return '<{} object at {}>'.format(
             self.__class__.__name__, hex(id(self))
         )
 
     def _on_close(self):
@@ -475,23 +459,32 @@
         """
         get property widget.
 
         Args:
             name (str): property name.
 
         Returns:
-            QtWidgets.QWidget: property widget.
+            NodeGraphQt.custom_widgets.properties_bin.prop_widgets_abstract.BaseProperty: property widget.
         """
         if name == 'name':
             return self.name_wgt
         for tab_name, prop_win in self.__tab_windows.items():
             widget = prop_win.get_widget(name)
             if widget:
                 return widget
 
+    def get_port_connection_widget(self):
+        """
+        Returns the ports connections container widget.
+
+        Returns:
+            _PortConnectionsContainer: port container widget.
+        """
+        return self._port_connections
+
 
 class PropertiesBinWidget(QtWidgets.QWidget):
     """
     The :class:`NodeGraphQt.PropertiesBinWidget` is a list widget for displaying
     and editing a nodes properties.
 
     .. inheritance-diagram:: NodeGraphQt.PropertiesBinWidget
@@ -533,14 +526,17 @@
         self._limit.setToolTip('Set display nodes limit.')
         self._limit.setMaximum(10)
         self._limit.setMinimum(0)
         self._limit.setValue(2)
         self._limit.valueChanged.connect(self.__on_limit_changed)
         self.resize(450, 400)
 
+        # this attribute to block signals if for the "on_property_changed" signal
+        # in case devs that don't implemented the ".prop_widgets_abstract.BaseProperty"
+        # widget is not implemented properly to prevent infinite loop.
         self._block_signal = False
 
         self._lock = False
         self._btn_lock = QtWidgets.QPushButton('Lock')
         self._btn_lock.setToolTip(
             'Lock the properties bin prevent nodes from being loaded.')
         self._btn_lock.clicked.connect(self.lock_bin)
@@ -567,15 +563,15 @@
         node_graph.property_changed.connect(self.__on_graph_property_changed)
 
     def __repr__(self):
         return '<{} object at {}>'.format(
             self.__class__.__name__, hex(id(self))
         )
 
-    def __on_widget_visible_changed(self, node_id, visible, tree_widget):
+    def __on_port_tree_visible_changed(self, node_id, visible, tree_widget):
         """
         Triggered when the visibility of the port tree widget changes we
         resize the property list table row.
 
         Args:
             node_id (str): node id.
             visible (bool): visibility state.
@@ -631,19 +627,19 @@
             prop_name (str): node property name.
             prop_value (object): node property value.
         """
         properties_widget = self.prop_widget(node)
         if not properties_widget:
             return
 
-        property_window = properties_widget.get_widget(prop_name)
+        property_widget = properties_widget.get_widget(prop_name)
 
-        if property_window and prop_value != property_window.get_value():
+        if property_widget and prop_value != property_widget.get_value():
             self._block_signal = True
-            property_window.set_value(prop_value)
+            property_widget.set_value(prop_value)
             self._block_signal = False
 
     def __on_property_widget_changed(self, node_id, prop_name, prop_value):
         """
         Slot function triggered when a property widget value has changed.
 
         Args:
@@ -687,20 +683,30 @@
             self._prop_list.removeRow(rows - 1)
 
         itm_find = self._prop_list.findItems(node.id, QtCore.Qt.MatchExactly)
         if itm_find:
             self._prop_list.removeRow(itm_find[0].row())
 
         self._prop_list.insertRow(0)
+
         prop_widget = NodePropWidget(node=node)
-        prop_widget.property_changed.connect(self.__on_property_widget_changed)
         prop_widget.property_closed.connect(self.__on_prop_close)
-        prop_widget.widget_visible_changed.connect(
-            self.__on_widget_visible_changed
+        prop_widget.property_changed.connect(self.__on_property_widget_changed)
+        port_connections = prop_widget.get_port_connection_widget()
+        port_connections.input_group.clicked.connect(
+            lambda v: self.__on_port_tree_visible_changed(
+                prop_widget.node_id(), v, port_connections.input_tree
+            )
         )
+        port_connections.output_group.clicked.connect(
+            lambda v: self.__on_port_tree_visible_changed(
+                prop_widget.node_id(), v, port_connections.output_tree
+            )
+        )
+
         self._prop_list.setCellWidget(0, 0, prop_widget)
 
         item = QtWidgets.QTableWidgetItem(node.id)
         self._prop_list.setItem(0, 0, item)
         self._prop_list.selectRow(0)
 
     def remove_node(self, node):
```

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.9/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.9/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.9/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.9/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.9/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.9/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.9/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.9/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.9/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.8
+Version: 0.6.9
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.8 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.9 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.8/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.9/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/PKG-INFO` & `NodeGraphQt-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.8
+Version: 0.6.9
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.8 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.9 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.8/README.md` & `NodeGraphQt-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.9/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.9/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.9/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.9/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.8/setup.cfg` & `NodeGraphQt-0.6.9/setup.cfg`

 * *Files identical despite different names*

