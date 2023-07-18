# Comparing `tmp/lcapygui-0.91.tar.gz` & `tmp/lcapygui-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcapygui-0.91.tar", last modified: Mon Jul 17 20:48:34 2023, max compression
+gzip compressed data, was "lcapygui-0.92.tar", last modified: Tue Jul 18 02:35:34 2023, max compression
```

## Comparing `lcapygui-0.91.tar` & `lcapygui-0.92.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.509561 lcapygui-0.91/
--rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-07-17 20:48:34.509561 lcapygui-0.91/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-07-17 20:48:34.000000 lcapygui-0.91/README.md
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.505561 lcapygui-0.91/lcapygui/
--rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/annotations.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.505561 lcapygui-0.91/lcapygui/components/
--rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/admittance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      341 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/bipole.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/bjt.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      315 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/capacitor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/cccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/ccvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    13524 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/component.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3762 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/connection.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/controlledcomponent.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/cpe.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3368 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/cpt_maker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/current_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      510 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/diode.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/ferritebead.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/impedance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      283 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/inductor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/jfet.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/mosfet.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3962 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/opamp.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      188 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/opencircuit.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/port.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      216 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/resistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4522 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/sketch.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/svgparse.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/transistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/vccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/vcvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/voltage_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      365 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/components/wire.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/node.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/nodes.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.505561 lcapygui-0.91/lcapygui/scripts/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/scripts/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1878 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/scripts/lcapytk.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.505561 lcapygui-0.91/lcapygui/ui/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1825 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/preferences.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.509561 lcapygui-0.91/lcapygui/ui/tk/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1220 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/approximate_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/cpt_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4980 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/cpt_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/drawing.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      768 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/edit_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2693 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/edit_values_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/equations_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      716 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/expr_attributes_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      425 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/expr_calc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    12941 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/expr_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/exprimage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/help_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/inspect_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2373 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/labelentries.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/lateximage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    23079 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/lcapytk.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/lcapytkm.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1174 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/limit_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2342 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/menu.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/message_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1631 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/multiplot_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/node_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/plot_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/plot_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4324 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/preferences_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1679 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/python_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4078 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/sketcher.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2490 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/state_space_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1189 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/subs_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      892 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/transfer_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2011 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/transfer_function_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1448 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/twoport_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3864 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/twoport_select_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      435 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/tk/working_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    20476 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/uimodelbase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    17327 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui/ui/uimodelmph.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:48:34.505561 lcapygui-0.91/lcapygui.egg-info/
--rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui.egg-info/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)     2628 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui.egg-info/SOURCES.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui.egg-info/dependency_links.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui.egg-info/entry_points.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui.egg-info/requires.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-07-17 20:48:34.000000 lcapygui-0.91/lcapygui.egg-info/top_level.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-07-17 20:48:34.000000 lcapygui-0.91/pyproject.toml
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-07-17 20:48:34.509561 lcapygui-0.91/setup.cfg
--rw-rw-r--   0 mph       (1000) mph       (1000)     1349 2023-07-17 20:48:34.000000 lcapygui-0.91/setup.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-07-18 02:35:34.188850 lcapygui-0.92/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-07-18 02:35:33.000000 lcapygui-0.92/README.md
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.184850 lcapygui-0.92/lcapygui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/annotations.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/components/
+-rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/admittance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      341 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/bipole.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/bjt.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      315 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/capacitor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/cccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/ccvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13524 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/component.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3762 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/connection.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/controlledcomponent.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/cpe.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3368 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/cpt_maker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/current_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      510 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/diode.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/ferritebead.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/impedance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      283 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/inductor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/jfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/mosfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3962 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/opamp.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      188 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/opencircuit.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/port.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      216 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/resistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4522 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/sketch.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/svgparse.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/transistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/vccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/vcvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/voltage_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      365 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/components/wire.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/node.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/nodes.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/scripts/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/scripts/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1878 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/scripts/lcapytk.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/ui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1825 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/preferences.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.188850 lcapygui-0.92/lcapygui/ui/tk/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1220 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/approximate_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/cpt_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4980 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/cpt_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/drawing.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      768 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/edit_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2693 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/edit_values_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/equations_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      716 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/expr_attributes_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      425 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/expr_calc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13041 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/expr_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/exprimage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/help_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/inspect_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2373 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/labelentries.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/lateximage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    23079 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/lcapytk.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/lcapytkm.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1174 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/limit_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2342 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/menu.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/message_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1631 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/multiplot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/node_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/plot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/plot_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4324 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/preferences_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1679 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/python_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4078 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/sketcher.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2490 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/state_space_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1189 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/subs_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      892 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/transfer_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2011 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/transfer_function_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1448 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/twoport_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3864 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/twoport_select_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      435 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/tk/working_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    20476 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/uimodelbase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    17327 2023-07-18 02:35:33.000000 lcapygui-0.92/lcapygui/ui/uimodelmph.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-18 02:35:34.184850 lcapygui-0.92/lcapygui.egg-info/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      934 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2628 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/SOURCES.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/dependency_links.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/entry_points.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/requires.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-07-18 02:35:34.000000 lcapygui-0.92/lcapygui.egg-info/top_level.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-07-18 02:35:33.000000 lcapygui-0.92/pyproject.toml
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-07-18 02:35:34.188850 lcapygui-0.92/setup.cfg
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1349 2023-07-18 02:35:33.000000 lcapygui-0.92/setup.py
```

### Comparing `lcapygui-0.91/PKG-INFO` & `lcapygui-0.92/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.91
+Version: 0.92
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.91/lcapygui/__init__.py` & `lcapygui-0.92/lcapygui/__init__.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/annotation.py` & `lcapygui-0.92/lcapygui/components/annotation.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/bjt.py` & `lcapygui-0.92/lcapygui/components/bjt.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/component.py` & `lcapygui-0.92/lcapygui/components/component.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/connection.py` & `lcapygui-0.92/lcapygui/components/connection.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/cpt_maker.py` & `lcapygui-0.92/lcapygui/components/cpt_maker.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/mosfet.py` & `lcapygui-0.92/lcapygui/components/mosfet.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/opamp.py` & `lcapygui-0.92/lcapygui/components/opamp.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/sketch.py` & `lcapygui-0.92/lcapygui/components/sketch.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/svgparse.py` & `lcapygui-0.92/lcapygui/components/svgparse.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/components/transistor.py` & `lcapygui-0.92/lcapygui/components/transistor.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/node.py` & `lcapygui-0.92/lcapygui/node.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/nodes.py` & `lcapygui-0.92/lcapygui/nodes.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/scripts/lcapytk.py` & `lcapygui-0.92/lcapygui/scripts/lcapytk.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/preferences.py` & `lcapygui-0.92/lcapygui/ui/preferences.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/approximate_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/approximate_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/cpt_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/cpt_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/cpt_properties_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/cpt_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/drawing.py` & `lcapygui-0.92/lcapygui/ui/tk/drawing.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/edit_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/edit_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/edit_values_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/edit_values_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/equations_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/equations_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/expr_attributes_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/expr_attributes_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/expr_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/expr_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     def __init__(self, expr, ui, title=''):
 
         super().__init__()
 
         self.report_callback_exception = ui.report_callback_exception
         self.expr = expr
         self.ui = ui
+        self.titlestr = title
         self.title(title)
 
         mdd = None
         if isinstance(expr, Matrix):
             nrows = expr.rows
             ncols = expr.cols
             delim = '' if nrows < 10 else ','
@@ -115,15 +116,15 @@
                           MenuItem('Magnitude', self.on_select),
                           MenuItem('dB', self.on_select),
                           MenuItem('Sign', self.on_select),
                           MenuItem('Phase degrees', self.on_select),
                           MenuItem('Phase radians', self.on_select),
                           ]),
             MenuDropdown('Format', 0,
-                         [MenuItem('ZPK', self.on_format),
+                         [MenuItem('Zero pole gain (ZPK)', self.on_format),
                           MenuItem('Canonical', self.on_format),
                           MenuItem('Time constant', self.on_format),
                           MenuItem('Time constant terms', self.on_format),
                           MenuItem('General', self.on_format),
                           MenuItem('Standard', self.on_format),
                           MenuItem('Partial fraction', self.on_format),
                           MenuItem('Polar', self.on_format),
@@ -185,32 +186,32 @@
     def apply_attribute(self, attributes, arg):
 
         try:
             attribute = attributes[arg]
 
             e = ExprCalc(self.expr)
             expr = e.attribute(attribute)
-            self.ui.show_expr_dialog(expr, title=self.title)
+            self.ui.show_expr_dialog(expr, title=self.titlestr)
         except Exception as e:
             self.ui.show_error_dialog(e)
 
     def apply_method(self, methods, arg):
 
         try:
             method = methods[arg]
 
             e = ExprCalc(self.expr)
             expr = e.method(method)
-            self.ui.show_expr_dialog(expr, title=self.title)
+            self.ui.show_expr_dialog(expr, title=self.titlestr)
         except Exception as e:
             self.ui.show_error_dialog(e)
 
     def on_attributes(self, arg):
 
-        self.ui.show_expr_attributes_dialog(self.expr, title=self.title)
+        self.ui.show_expr_attributes_dialog(self.expr, title=self.titlestr)
 
     def on_edit(self, arg):
 
         self.ui.show_edit_dialog(self.expr)
 
     def on_edit_python(self, arg):
 
@@ -219,15 +220,15 @@
     def on_format(self, arg):
 
         formats = {'Canonical': 'canonical',
                    'Standard': 'standard',
                    'General': 'general',
                    'Time constant': 'timeconst',
                    'Time constant terms': 'timeconst_terms',
-                   'ZPK': 'ZPK',
+                   'Zero pole gain (ZPK)': 'ZPK',
                    'Partial fraction': 'partfrac',
                    'Time constant': 'timeconst',
                    'Polar': 'polar',
                    'Cartesian': 'cartesian'}
 
         if arg in ('Polar', 'Cartesian'):
             # What was I thinking?
@@ -250,36 +251,36 @@
                     'Simplify Heaviside': 'simplify_heaviside',
                     'Simplify rect': 'simplify_rect',
                     'Cancel terms': 'cancel_terms',
                     'Rationalize denominator': 'rationalize_denominator'}
 
         try:
             if arg == 'Approximate':
-                self.ui.show_approximate_dialog(self.expr, title=self.title)
+                self.ui.show_approximate_dialog(self.expr, title=self.titlestr)
             elif arg == 'Evaluate':
                 self.ui.show_expr_dialog(
-                    self.expr.evaluate(), title=self.title)
+                    self.expr.evaluate(), title=self.titlestr)
             elif arg == 'Limit':
-                self.ui.show_limit_dialog(self.expr, title=self.title)
+                self.ui.show_limit_dialog(self.expr, title=self.titlestr)
             elif arg == 'Parameterize':
                 self.ui.show_expr_dialog(ExprTuple(self.expr.parameterize()),
-                                         title=self.title)
+                                         title=self.titlestr)
             elif arg == 'Poles':
                 self.ui.show_expr_dialog(
-                    self.expr.poles(), title=self.title)
+                    self.expr.poles(), title=self.titlestr)
             elif arg in simplify:
                 self.apply_method(simplify, arg)
             elif arg == 'Solve':
                 self.ui.show_expr_dialog(
-                    self.expr.solve(), title=self.title)
+                    self.expr.solve(), title=self.titlestr)
             elif arg == 'Substitute':
-                self.ui.show_subs_dialog(self.expr, title=self.title)
+                self.ui.show_subs_dialog(self.expr, title=self.titlestr)
             elif arg == 'Zeros':
                 self.ui.show_expr_dialog(
-                    self.expr.zeros(), title=self.title)
+                    self.expr.zeros(), title=self.titlestr)
         except Exception as e:
             self.ui.show_error_dialog(e)
 
     def on_save_latex(self, arg):
 
         pathname = self.ui.save_file_dialog('expr.tex', doc='LaTeX file',
                                             ext='*.tex')
@@ -322,15 +323,15 @@
             c = arg[1]
 
         row = int(r) - 1
         col = int(c) - 1
 
         e = ExprCalc(self.expr)
         expr = e.eval('[%s, %d]' % (row, col))
-        self.ui.show_expr_dialog(expr, title=self.title)
+        self.ui.show_expr_dialog(expr, title=self.titlestr)
 
     def on_plot(self, arg):
 
         if not isinstance(self.expr, Expr):
             self.ui.info_dialog('Cannot plot expression')
             return
```

### Comparing `lcapygui-0.91/lcapygui/ui/tk/help_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/help_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/inspect_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/inspect_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/labelentries.py` & `lcapygui-0.92/lcapygui/ui/tk/labelentries.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/lateximage.py` & `lcapygui-0.92/lcapygui/ui/tk/lateximage.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/lcapytk.py` & `lcapygui-0.92/lcapygui/ui/tk/lcapytk.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/lcapytkm.py` & `lcapygui-0.92/lcapygui/ui/tk/lcapytkm.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/limit_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/limit_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/menu.py` & `lcapygui-0.92/lcapygui/ui/tk/menu.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/multiplot_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/multiplot_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/node_properties_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/node_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/plot_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/plot_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/plot_properties_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/plot_properties_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/preferences_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/python_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/python_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/sketcher.py` & `lcapygui-0.92/lcapygui/ui/tk/sketcher.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/state_space_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/state_space_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/subs_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/subs_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/transfer_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/transfer_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/transfer_function_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/transfer_function_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/twoport_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/twoport_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/tk/twoport_select_dialog.py` & `lcapygui-0.92/lcapygui/ui/tk/twoport_select_dialog.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/uimodelbase.py` & `lcapygui-0.92/lcapygui/ui/uimodelbase.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui/ui/uimodelmph.py` & `lcapygui-0.92/lcapygui/ui/uimodelmph.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/lcapygui.egg-info/PKG-INFO` & `lcapygui-0.92/lcapygui.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.91
+Version: 0.92
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.91/lcapygui.egg-info/SOURCES.txt` & `lcapygui-0.92/lcapygui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lcapygui-0.91/setup.py` & `lcapygui-0.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name='lcapygui',
     packages=find_packages(include=[
         "lcapygui",
         "lcapygui.*"
     ]),
-    version="0.91",
+    version="0.92",
     description="A GUI for lcapy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Michael Hayes, Jordan Hay",
     license="MIT",
     url="https://github.com/mph-/lcapy-gui",
     project_urls={
```

