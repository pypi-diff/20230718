# Comparing `tmp/imio.events.core-1.1.7.tar.gz` & `tmp/imio.events.core-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.events.core-1.1.7.tar", last modified: Mon Jul  3 11:55:03 2023, max compression
+gzip compressed data, was "imio.events.core-1.1.8.tar", last modified: Tue Jul 18 09:42:30 2023, max compression
```

## Comparing `imio.events.core-1.1.7.tar` & `imio.events.core-1.1.8.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3323 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6377 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.323803 imio.events.core-1.1.7/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      691 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/browser/json_recurrence.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/browser/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      850 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/contents/agenda/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/agenda/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/agenda/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/agenda/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio/events/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/entity/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/contents/event/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/event/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/event/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6641 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/event/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/event/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8341 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/event/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4323 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/event/views.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/folder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/contents/folder/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.323803 imio.events.core-1.1.7/src/imio/events/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/faceted/config/events.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.323803 imio.events.core-1.1.7/src/imio/events/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      685 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/taxonomies/event_public.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1386 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1583 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1659 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Event.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/rest/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/rest/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/rest/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3059 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/rest/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5607 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/resources/plone.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_agenda.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1573 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14464 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_event.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_folder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_indexes.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_rest.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7479 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3567 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.323803 imio.events.core-1.1.7/src/imio/events/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/upgrades/profiles/1002_to_1003/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.331803 imio.events.core-1.1.7/src/imio/events/core/upgrades/profiles/1005_to_1006/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3772 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4548 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1006 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio/events/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-03 11:55:03.327803 imio.events.core-1.1.7/src/imio.events.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6377 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4317 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-07-03 11:55:03.000000 imio.events.core-1.1.7/src/imio.events.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3438 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6492 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.957409 imio.events.core-1.1.8/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      691 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/json_recurrence.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      850 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/entity/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/entity/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/entity/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/entity/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/event/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6641 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/serializer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8341 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4323 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/folder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/folder/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/converters.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/events/core/faceted/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/faceted/config/events.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/overrides.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/events/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      685 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/event_public.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1386 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1583 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1659 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Event.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/rest/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/rest/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/rest/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3792 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/rest/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5607 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/resources/plone.png
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_agenda.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1573 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_entity.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14464 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_event.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_multilingual.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7479 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3567 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1002_to_1003/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1005_to_1006/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3772 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4548 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1006 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio.events.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6492 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4317 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/top_level.txt
```

### Comparing `imio.events.core-1.1.7/CHANGES.rst` & `imio.events.core-1.1.8/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.8 (2023-07-18)
+------------------
+
+- Add logs in endpoint. Help us to find why agenda go slowlier
+  [boulch]
+
+
 1.1.7 (2023-07-03)
 ------------------
 
 - Avoid infinite loop with bad recurrence RRULE expression (`INTERVAL=0"`)
   See https://github.com/plone/plone.formwidget.recurrence/issues/39
   [laulaz]
```

### Comparing `imio.events.core-1.1.7/DEVELOP.rst` & `imio.events.core-1.1.8/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/LICENSE.GPL` & `imio.events.core-1.1.8/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/LICENSE.rst` & `imio.events.core-1.1.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/PKG-INFO` & `imio.events.core-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.1.7
+Version: 1.1.8
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
@@ -119,14 +119,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.8 (2023-07-18)
+------------------
+
+- Add logs in endpoint. Help us to find why agenda go slowlier
+  [boulch]
+
+
 1.1.7 (2023-07-03)
 ------------------
 
 - Avoid infinite loop with bad recurrence RRULE expression (`INTERVAL=0"`)
   See https://github.com/plone/plone.formwidget.recurrence/issues/39
   [laulaz]
```

### Comparing `imio.events.core-1.1.7/README.rst` & `imio.events.core-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/docs/conf.py` & `imio.events.core-1.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/setup.cfg` & `imio.events.core-1.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/setup.py` & `imio.events.core-1.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.events.core",
-    version="1.1.7",
+    version="1.1.8",
     description="Core product for iMio events website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.events.core-1.1.7/src/imio/events/core/browser/configure.zcml` & `imio.events.core-1.1.8/src/imio/events/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/browser/json_recurrence.py` & `imio.events.core-1.1.8/src/imio/events/core/browser/json_recurrence.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/browser/utils.py` & `imio.events.core-1.1.8/src/imio/events/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/configure.zcml` & `imio.events.core-1.1.8/src/imio/events/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/agenda/content.py` & `imio.events.core-1.1.8/src/imio/events/core/contents/agenda/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/entity/content.py` & `imio.events.core-1.1.8/src/imio/events/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/event/configure.zcml` & `imio.events.core-1.1.8/src/imio/events/core/contents/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/event/content.py` & `imio.events.core-1.1.8/src/imio/events/core/contents/event/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/event/serializer.py` & `imio.events.core-1.1.8/src/imio/events/core/contents/event/serializer.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/event/view.pt` & `imio.events.core-1.1.8/src/imio/events/core/contents/event/view.pt`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/contents/event/views.py` & `imio.events.core-1.1.8/src/imio/events/core/contents/event/views.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/faceted/config/events.xml` & `imio.events.core-1.1.8/src/imio/events/core/faceted/config/events.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/indexers.py` & `imio.events.core-1.1.8/src/imio/events/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/indexers.zcml` & `imio.events.core-1.1.8/src/imio/events/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/permissions.zcml` & `imio.events.core-1.1.8/src/imio/events/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/catalog.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/metadata.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/registry.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/rolemap.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/taxonomies/event_public.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/event_public.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Entity.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Event.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Event.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles/default/types/imio.events.Folder.xml` & `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/profiles.zcml` & `imio.events.core-1.1.8/src/imio/events/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/rest/endpoint.py` & `imio.events.core-1.1.8/src/imio/events/core/rest/endpoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from plone.restapi.batching import HypermediaBatch
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.search.handler import SearchHandler
 from plone.restapi.search.utils import unflatten_dotted_dict
 from plone.restapi.services import Service
 from zope.component import getMultiAdapter
 
+import logging
+import time
+
+logger = logging.getLogger("imio.events.core")
+
 
 class EventsEndpointGet(Service):
     def reply(self):
         query = self.request.form.copy()
         query = unflatten_dotted_dict(query)
         return EventsEndpointHandler(self.context, self.request).search(query)
 
@@ -24,15 +29,14 @@
     # we receive b_size and b_start from smartweb with values already set
     # So we ignore these values but we must stock these to use it ...
     ignored_params = ["b_size", "b_start"]
 
     def search(self, query=None):
         if query is None:
             query = {}
-
         b_size = query.get("b_size") or 20
         b_start = query.get("b_start") or 0
 
         for param in self.ignored_params:
             if param in query:
                 del query[param]
 
@@ -45,18 +49,21 @@
         query["portal_type"] = "imio.events.Event"
         query["review_state"] = "published"
         query["b_size"] = 10000
 
         # Only future events
         today = date.today().isoformat()
         query["event_dates"] = {"query": today, "range": "min"}
-
+        tps1 = time.time()
         self._constrain_query_by_path(query)
+        tps2 = time.time()
         query = self._parse_query(query)
+        tps3 = time.time()
         lazy_resultset = self.catalog.searchResults(**query)
+        tps4 = time.time()
         if "metadata_fields" not in self.request.form:
             self.request.form["metadata_fields"] = []
         self.request.form["metadata_fields"] += [
             "recurrence",
             "whole_day",
             "first_start",
             "first_end",
@@ -64,21 +71,32 @@
         ]
         # ISerializeToJson use a default request batch so we force a "full" b_size and a "zero" b_start
         self.request.form["b_size"] = 10000
         self.request.form["b_start"] = 0
         results = getMultiAdapter((lazy_resultset, self.request), ISerializeToJson)(
             fullobjects=fullobjects
         )
+        tps5 = time.time()
         expanded_occurences = expand_occurences(results.get("items"))
         sorted_expanded_occurences = sorted(expanded_occurences, key=get_start_date)
+        tps6 = time.time()
 
         # It's time to get real b_size/b_start from the smartweb query
         self.request.form["b_size"] = b_size
         self.request.form["b_start"] = b_start
         batch = HypermediaBatch(self.request, sorted_expanded_occurences)
+        tps7 = time.time()
+        logger.info(f"query : {results['@id']}")
+        logger.info(f"time constrain_query_by_path : {tps2 - tps1}")
+        logger.info(f"time _parse_query : {tps3 - tps2}")
+        logger.info(f"time catalog lazy_resultset : {tps4 - tps3}")
+        logger.info(f"time MultiAdapter fullobj : {tps5 - tps4}")
+        logger.info(f"time occurences : {tps6 - tps5}")
+        logger.info(f"time batch : {tps7 - tps6}")
+        logger.info(f"time (total) : {tps7 - tps1}")
 
         results = {}
         results["@id"] = batch.canonical_url
         results["items_total"] = batch.items_total
         links = batch.links
         if links:
             results["batching"] = links
```

### Comparing `imio.events.core-1.1.7/src/imio/events/core/setuphandlers.py` & `imio.events.core-1.1.8/src/imio/events/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/subscribers.py` & `imio.events.core-1.1.8/src/imio/events/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/subscribers.zcml` & `imio.events.core-1.1.8/src/imio/events/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/testing.py` & `imio.events.core-1.1.8/src/imio/events/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/resources/plone.png` & `imio.events.core-1.1.8/src/imio/events/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot` & `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot` & `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot` & `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/robot/test_example.robot` & `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_agenda.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_agenda.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_cropping.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_entity.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_event.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_folder.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_indexes.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_local_roles.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_multilingual.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_rest.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_robot.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_setup.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_utils.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/tests/test_vocabularies.py` & `imio.events.core-1.1.8/src/imio/events/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/upgrades/configure.zcml` & `imio.events.core-1.1.8/src/imio/events/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml` & `imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/upgrades/upgrades.py` & `imio.events.core-1.1.8/src/imio/events/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/utils.py` & `imio.events.core-1.1.8/src/imio/events/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/vocabularies.py` & `imio.events.core-1.1.8/src/imio/events/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio/events/core/vocabularies.zcml` & `imio.events.core-1.1.8/src/imio/events/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.7/src/imio.events.core.egg-info/PKG-INFO` & `imio.events.core-1.1.8/src/imio.events.core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.1.7
+Version: 1.1.8
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
@@ -119,14 +119,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.8 (2023-07-18)
+------------------
+
+- Add logs in endpoint. Help us to find why agenda go slowlier
+  [boulch]
+
+
 1.1.7 (2023-07-03)
 ------------------
 
 - Avoid infinite loop with bad recurrence RRULE expression (`INTERVAL=0"`)
   See https://github.com/plone/plone.formwidget.recurrence/issues/39
   [laulaz]
```

### Comparing `imio.events.core-1.1.7/src/imio.events.core.egg-info/SOURCES.txt` & `imio.events.core-1.1.8/src/imio.events.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

