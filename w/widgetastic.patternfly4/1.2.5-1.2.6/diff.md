# Comparing `tmp/widgetastic.patternfly4-1.2.5-py3-none-any.whl.zip` & `tmp/widgetastic.patternfly4-1.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 54783 bytes, number of entries: 37
+Zip file size: 54800 bytes, number of entries: 37
 -rw-r--r--  2.0 unx     3649 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/__init__.py
 -rw-r--r--  2.0 unx     2600 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/alert.py
 -rw-r--r--  2.0 unx     2040 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/breadcrumb.py
 -rw-r--r--  2.0 unx     6719 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/bulletchart.py
 -rw-r--r--  2.0 unx     3623 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/button.py
 -rw-r--r--  2.0 unx     3317 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/calendarmonth.py
 -rw-r--r--  2.0 unx     1667 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/card.py
@@ -28,12 +28,12 @@
 -rw-r--r--  2.0 unx     2315 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/radio.py
 -rw-r--r--  2.0 unx     5494 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/select.py
 -rw-r--r--  2.0 unx     3139 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/slider.py
 -rw-r--r--  2.0 unx     1844 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/switch.py
 -rw-r--r--  2.0 unx    17003 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/table.py
 -rw-r--r--  2.0 unx     2110 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/tabs.py
 -rw-r--r--  2.0 unx      952 b- defN 20-Feb-02 00:00 widgetastic_patternfly4/title.py
-?rw-r--r--  2.0 unx    18056 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11357 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     3411 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.5.dist-info/RECORD
-37 files, 162477 bytes uncompressed, 49233 bytes compressed:  69.7%
+?rw-r--r--  2.0 unx    18132 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11357 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     3411 b- defN 20-Feb-02 00:00 widgetastic.patternfly4-1.2.6.dist-info/RECORD
+37 files, 162553 bytes uncompressed, 49250 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -93,20 +93,20 @@
 
 Filename: widgetastic_patternfly4/tabs.py
 Comment: 
 
 Filename: widgetastic_patternfly4/title.py
 Comment: 
 
-Filename: widgetastic.patternfly4-1.2.5.dist-info/METADATA
+Filename: widgetastic.patternfly4-1.2.6.dist-info/METADATA
 Comment: 
 
-Filename: widgetastic.patternfly4-1.2.5.dist-info/WHEEL
+Filename: widgetastic.patternfly4-1.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: widgetastic.patternfly4-1.2.5.dist-info/licenses/LICENSE
+Filename: widgetastic.patternfly4-1.2.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: widgetastic.patternfly4-1.2.5.dist-info/RECORD
+Filename: widgetastic.patternfly4-1.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## widgetastic_patternfly4/ouia.py

```diff
@@ -149,9 +149,9 @@
     OUIA_COMPONENT_TYPE = "PF4/Text"
 
 
 class TextInput(BaseOuiaTextInput):
     OUIA_COMPONENT_TYPE = "PF4/TextInput"
 
 
-class clipboardcopy(BaseClipboardCopy, OUIAGenericWidget):
+class ClipboardCopy(BaseClipboardCopy, OUIAGenericWidget):
     OUIA_COMPONENT_TYPE = "PF4/ClipboardCopy"
```

## Comparing `widgetastic.patternfly4-1.2.5.dist-info/METADATA` & `widgetastic.patternfly4-1.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgetastic.patternfly4
-Version: 1.2.5
+Version: 1.2.6
 Summary: Patternfly4 widget library for Widgetastic.
 Project-URL: repository, https://github.com/RedHatQE/widgetastic.patternfly4
 Maintainer-email: Raoul Snyman <rsnyman@redhat.com>, Nikhil Dhandre <ndhandre@redhat.com>, Egor Shamardin <eshamard@redhat.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -248,14 +248,16 @@
 
 Calendar month - <https://www.patternfly.org/v4/components/calendar-month>
 
 Card - <https://www.patternfly.org/v4/components/card>
 
 Chip Group - <https://www.patternfly.org/v4/components/chip-group>
 
+Clipboard copy - <https://www.patternfly.org/v4/components/clipboard-copy>
+
 Context Selector - <https://www.patternfly.org/v4/components/context-selector>
 
 Description list - <https://www.patternfly.org/v4/components/description-list>
 
 Donut Chart - <https://www.patternfly.org/v4/charts/donut-chart>
 
 Dual list selector - <https://www.patternfly.org/v4/components/dual-list-selector>
```

## Comparing `widgetastic.patternfly4-1.2.5.dist-info/licenses/LICENSE` & `widgetastic.patternfly4-1.2.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `widgetastic.patternfly4-1.2.5.dist-info/RECORD` & `widgetastic.patternfly4-1.2.6.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 widgetastic_patternfly4/duallistselector.py,sha256=TZLH6OXIt6SXhrtICjjAp-ZvTeDT1_vCFOZ4qD2PpDQ,4866
 widgetastic_patternfly4/formselect.py,sha256=f3K2pT8xLWBJLozSyhHms54_NP4zo387fKIP2V23yDQ,3646
 widgetastic_patternfly4/linechart.py,sha256=ogAy7Gy8soCQ0NJG9WirCNP_BVugL3l_8CZV-lWwfKk,3650
 widgetastic_patternfly4/menu.py,sha256=C-1tyjoAAGogFVuXAdey_D41EUICENSEYR5PwfZ5lvk,7943
 widgetastic_patternfly4/modal.py,sha256=R7kJODGw4Wam98qK6t7DBbMWKbpRV3eL0S-yLR5kf8E,2034
 widgetastic_patternfly4/navigation.py,sha256=pnck5PxV831ri1Rg7G7cIVDWjYOeMCPXUrXiEP7K6sI,5355
 widgetastic_patternfly4/optionsmenu.py,sha256=rd_KeFDJYF6kpccm2_hvvSuWuaH0RIV-lhHA92goe24,1149
-widgetastic_patternfly4/ouia.py,sha256=hgM-E964lQ0NOwkupK-zFpQkXeflutmfsT2gxxFCTto,4665
+widgetastic_patternfly4/ouia.py,sha256=_L61C19Gs1Z4oZFRpcGEQVa59ulenkqw-YBoXq05H-k,4665
 widgetastic_patternfly4/pagination.py,sha256=-5pfgzMoK0SfmKO6eCSExI-wt1i25H-6eet4if02hHU,8729
 widgetastic_patternfly4/piechart.py,sha256=exCNtYj7zWpv4IZhYu54BiCLJrUkMXpOP1dyANxqYo4,221
 widgetastic_patternfly4/popover.py,sha256=MX6AMAgUmbJESV75QuONHeNUKQeCwfxRrPeZDYnhI1M,2200
 widgetastic_patternfly4/progress.py,sha256=nvjuIC-2A59ZKmGptBV5dZNKKXpIKyb1ahiDHGIzVVM,1389
 widgetastic_patternfly4/radio.py,sha256=nbR7avFbvpU1FPQq-BemPCyGtqNzDkKSuLpqB28bVT8,2315
 widgetastic_patternfly4/select.py,sha256=gA0naRNI-KapFMtqeL7RTq24104mJGrTqazqhm_hoow,5494
 widgetastic_patternfly4/slider.py,sha256=IgTWuDx3O1yEgK9nvgCJJxz4dD6v8sEi1XRzfn2D5ms,3139
 widgetastic_patternfly4/switch.py,sha256=8ayElBvJfZHl7-bdmmdqwS09DI87SA0hTdVvdQqg8h4,1844
 widgetastic_patternfly4/table.py,sha256=1uisGbL4Mz59PWGynq6A2wvNkSj6Fwnqua1rfhKac8w,17003
 widgetastic_patternfly4/tabs.py,sha256=Ts1gVGA9fmMGX-sGR4uo6vTM-pMSCgNg9crVsDiId0Q,2110
 widgetastic_patternfly4/title.py,sha256=3qWqHWLcvv3VlaRBNiDGB1BSEg3hHcK48pJK1veZdxY,952
-widgetastic.patternfly4-1.2.5.dist-info/METADATA,sha256=whdG0SO9h3Wj2W0sxMwlBnWYXretpc7V2YgIcGsDXfw,18056
-widgetastic.patternfly4-1.2.5.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-widgetastic.patternfly4-1.2.5.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-widgetastic.patternfly4-1.2.5.dist-info/RECORD,,
+widgetastic.patternfly4-1.2.6.dist-info/METADATA,sha256=KJr5jmJeyHfpXD1BlMITOhle3Cr0ewm7xgeVvAQOGqY,18132
+widgetastic.patternfly4-1.2.6.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+widgetastic.patternfly4-1.2.6.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+widgetastic.patternfly4-1.2.6.dist-info/RECORD,,
```

