# Comparing `tmp/pyPreservica-2.0.5.tar.gz` & `tmp/pyPreservica-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-2.0.5.tar", last modified: Thu Jul 13 17:40:05 2023, max compression
+gzip compressed data, was "pyPreservica-2.0.6.tar", last modified: Tue Jul 18 08:17:06 2023, max compression
```

## Comparing `pyPreservica-2.0.5.tar` & `pyPreservica-2.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:40:05.771385 pyPreservica-2.0.5/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-07-13 17:40:05.771385 pyPreservica-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:40:05.718011 pyPreservica-2.0.5/pyPreservica/
--rw-rw-rw-   0        0        0     1085 2023-07-13 17:36:18.000000 pyPreservica-2.0.5/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37810 2023-07-13 09:10:01.000000 pyPreservica-2.0.5/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.5/pyPreservica/authorityAPI.py
--rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.5/pyPreservica/common.py
--rw-rw-rw-   0        0        0    17206 2023-07-13 17:36:18.000000 pyPreservica-2.0.5/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105749 2023-07-05 09:27:42.000000 pyPreservica-2.0.5/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.5/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.5/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.5/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.5/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.5/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.5/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.5/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:40:05.755790 pyPreservica-2.0.5/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 17:40:03.000000 pyPreservica-2.0.5/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 17:40:05.771385 pyPreservica-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-07-13 17:36:18.000000 pyPreservica-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:17:06.083390 pyPreservica-2.0.6/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-07-18 08:17:06.083390 pyPreservica-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 08:17:06.045639 pyPreservica-2.0.6/pyPreservica/
+-rw-rw-rw-   0        0        0     1085 2023-07-18 07:55:48.000000 pyPreservica-2.0.6/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37810 2023-07-13 09:10:01.000000 pyPreservica-2.0.6/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.6/pyPreservica/authorityAPI.py
+-rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.6/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    17206 2023-07-13 17:36:18.000000 pyPreservica-2.0.6/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   108094 2023-07-18 08:00:57.000000 pyPreservica-2.0.6/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.6/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.6/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.6/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.6/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92457 2023-07-14 10:50:52.000000 pyPreservica-2.0.6/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.6/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.6/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:17:06.067764 pyPreservica-2.0.6/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-07-18 08:17:04.000000 pyPreservica-2.0.6/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-18 08:17:05.000000 pyPreservica-2.0.6/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:17:04.000000 pyPreservica-2.0.6/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-18 08:17:04.000000 pyPreservica-2.0.6/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 08:17:04.000000 pyPreservica-2.0.6/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:17:06.083390 pyPreservica-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-07-18 07:55:48.000000 pyPreservica-2.0.6/setup.py
```

### Comparing `pyPreservica-2.0.5/LICENSE.txt` & `pyPreservica-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/PKG-INFO` & `pyPreservica-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.5/README.md` & `pyPreservica-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/__init__.py` & `pyPreservica-2.0.6/pyPreservica/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 from .authorityAPI import AuthorityAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-2.0.5/pyPreservica/adminAPI.py` & `pyPreservica-2.0.6/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/authorityAPI.py` & `pyPreservica-2.0.6/pyPreservica/authorityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/common.py` & `pyPreservica-2.0.6/pyPreservica/common.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/contentAPI.py` & `pyPreservica-2.0.6/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/entityAPI.py` & `pyPreservica-2.0.6/pyPreservica/entityAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 author:     James Carr
 licence:    Apache License 2.0
 
 """
 import uuid
 import xml.etree.ElementTree
 from datetime import datetime, timedelta, timezone
+from io import BytesIO
 from time import sleep
 from typing import Any, Generator, Tuple, Iterable, Union
 
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
@@ -42,21 +43,60 @@
 
              :return: dict of security tags
              :rtype:  dict
          """
 
         return self.security_tags_base(with_permissions=with_permissions)
 
-    def bitstream_content(self, bitstream: Bitstream, filename: str) -> int:
+    def bitstream_bytes(self, bitstream: Bitstream, chunk_size: int = CHUNK_SIZE) -> BytesIO:
+        """
+                Download a file represented as a Bitstream to a byteIO array
+
+                Returns the byteIO
+                Returns None if the file does not contain the correct number of bytes (default 2k)
+
+                :param chunk_size: The buffer copy chunk size in bytes default
+                :param bitstream: A Bitstream object
+                :type bitstream: Bitstream
+
+                :return: The file in bytes
+                :rtype: byteIO
+        """
+        if not isinstance(bitstream, Bitstream):
+            logger.error("bitstream_content argument is not a Bitstream object")
+            raise RuntimeError("bitstream_bytes argument is not a Bitstream object")
+        with self.session.get(bitstream.content_url, headers={HEADER_TOKEN: self.token}, stream=True) as request:
+            if request.status_code == requests.codes.unauthorized:
+                self.token = self.__token__()
+                return self.bitstream_bytes(bitstream)
+            elif request.status_code == requests.codes.ok:
+                file_bytes = BytesIO()
+                for chunk in request.iter_content(chunk_size=chunk_size):
+                    file_bytes.write(chunk)
+                file_bytes.seek(0)
+                if file_bytes.getbuffer().nbytes == bitstream.length:
+                    logger.debug(f"Downloaded {bitstream.length} bytes from {bitstream.filename}")
+                    return file_bytes
+                else:
+                    logger.error("Downloaded file size did not match the Preservica held value")
+                    return None
+            else:
+                exception = HTTPException(bitstream.filename, request.status_code, request.url, "bitstream_content",
+                                          request.content.decode('utf-8'))
+                logger.error(exception)
+                raise exception
+
+    def bitstream_content(self, bitstream: Bitstream, filename: str, chunk_size: int = CHUNK_SIZE) -> int:
         """
         Download a file represented as a Bitstream to a local filename
 
         Returns the number of bytes written to the file
         Returns None if the file does not contain the correct number of bytes
 
+        :param chunk_size: The buffer copy chunk size in bytes default
         :param bitstream: A Bitstream object
         :type bitstream: Bitstream
 
         :param filename: The filename to write the bytes to
         :type filename: str
 
         :return: The size of the file in bytes
@@ -69,15 +109,15 @@
             raise RuntimeError("bitstream_content argument is not a Bitstream object")
         with self.session.get(bitstream.content_url, headers={HEADER_TOKEN: self.token}, stream=True) as request:
             if request.status_code == requests.codes.unauthorized:
                 self.token = self.__token__()
                 return self.bitstream_content(bitstream, filename)
             elif request.status_code == requests.codes.ok:
                 with open(filename, 'wb') as file:
-                    for chunk in request.iter_content(chunk_size=CHUNK_SIZE):
+                    for chunk in request.iter_content(chunk_size=chunk_size):
                         file.write(chunk)
                     file.flush()
                 if os.path.getsize(filename) == bitstream.length:
                     logger.debug(f"Downloaded {bitstream.length} bytes into {filename}")
                     return bitstream.length
                 else:
                     logger.error("Download file size did not match the Preservica held value")
@@ -174,16 +214,17 @@
         xml.etree.ElementTree.SubElement(xml_object, "IncludeMetadata").text = include_metadata
         xml.etree.ElementTree.SubElement(xml_object, "IncludedGenerations").text = include_generation
         xml.etree.ElementTree.SubElement(xml_object, "IncludeParentHierarchy").text = include_parent.lower()
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
 
         logger.debug(xml_request)
 
-        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/exports',
-                                    headers=headers, data=xml_request)
+        request = self.session.post(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/exports',
+            headers=headers, data=xml_request)
 
         if request.status_code == requests.codes.accepted:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.__export_opex_start__(entity, IncludeContent=include_content,
                                               IncludeMetadata=include_metadata, IncludedGenerations=include_generation,
@@ -339,16 +380,17 @@
              :param identifier_value: The value of the identifier to delete.
           """
 
         if (self.major_version < 7) and (self.minor_version < 1):
             raise RuntimeError("delete_identifiers API call is not available when connected to a v6.0 System")
 
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
-                                   headers=headers)
+        request = self.session.get(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
+            headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             identifier_list = entity_response.findall(f'.//{{{self.xip_ns}}}Identifier')
             for identifier_element in identifier_list:
                 _ref = _type = _value = _aipid = None
                 for identifier in identifier_element:
@@ -385,16 +427,17 @@
 
              Returns the set of external identifiers on the entity
 
              :param entity: The entity
              :type  entity: Entity
           """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
-                                   headers=headers)
+        request = self.session.get(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/identifiers',
+            headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             identifier_list = entity_response.findall(f'.//{{{self.xip_ns}}}Identifier')
             result = set()
             for identifier in identifier_list:
@@ -473,15 +516,16 @@
         xml_object = xml.etree.ElementTree.Element('Identifier', {"xmlns": self.xip_ns})
         xml.etree.ElementTree.SubElement(xml_object, "Type").text = identifier_type
         xml.etree.ElementTree.SubElement(xml_object, "Value").text = identifier_value
         xml.etree.ElementTree.SubElement(xml_object, "Entity").text = entity.reference
         end_point = f"/{entity.path}/{entity.reference}/identifiers"
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request,
+                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_string = str(request.content.decode("utf-8"))
             identifier_response = xml.etree.ElementTree.fromstring(xml_string)
             aip_id = identifier_response.find(f'.//{{{self.xip_ns}}}ApiId')
             if hasattr(aip_id, 'text'):
                 return aip_id.text
             else:
@@ -585,15 +629,16 @@
         """
 
         headers = {HEADER_TOKEN: self.token}
         end_point = f"{entity.path}/{entity.reference}/links"
 
         if next_page is None:
             params = {'start': '0', 'max': str(maximum)}
-            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{end_point}', headers=headers, params=params)
+            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{end_point}', headers=headers,
+                                       params=params)
         else:
             request = self.session.get(next_page, headers=headers)
 
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
@@ -656,15 +701,16 @@
         xml.etree.ElementTree.SubElement(xml_object, "Type").text = relationship_type
         xml.etree.ElementTree.SubElement(xml_object, "FromEntity").text = from_entity.reference
         xml.etree.ElementTree.SubElement(xml_object, "ToEntity").text = to_entity.reference
 
         end_point = f"/{from_entity.path}/{from_entity.reference}/links"
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request,
+                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_string = str(request.content.decode("utf-8"))
             logger.debug(xml_string)
             link_response = xml.etree.ElementTree.fromstring(xml_string)
             relation = link_response.find(f'.//{{{self.xip_ns}}}Link')
             relation_type = relation.find(f'.//{{{self.xip_ns}}}Type')
             return relation_type.text
@@ -771,15 +817,16 @@
             tree = xml.etree.ElementTree.parse(data)
             content.append(tree.getroot())
         else:
             raise RuntimeError("Unknown data type")
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         end_point = f"/{entity.path}/{entity.reference}/metadata"
         logger.debug(xml_request)
-        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity{end_point}', data=xml_request,
+                                    headers=headers)
         if request.status_code == requests.codes.ok:
             return self.entity(entity_type=entity.entity_type, reference=entity.reference)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_metadata(entity, schema, data)
         else:
             exception = HTTPException(entity.reference, request.status_code, request.url, "add_metadata",
@@ -865,16 +912,17 @@
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
         if isinstance(entity, Asset) and dest_folder is None:
             raise RuntimeError(entity.reference, "Only folders can be moved to the root of the repository")
         if dest_folder is not None:
             data = dest_folder.reference
         else:
             data = "@root@"
-        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
-                                   data=data, headers=headers)
+        request = self.session.put(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
+            data=data, headers=headers)
         if request.status_code == requests.codes.accepted:
             return request.content.decode()
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.move_async(entity, dest_folder)
         else:
             exception = HTTPException(entity.reference, request.status_code, request.url, "move_async",
@@ -915,16 +963,17 @@
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain'}
         if isinstance(entity, Asset) and dest_folder is None:
             raise RuntimeError(entity.reference, "Only folders can be moved to the root of the repository")
         if dest_folder is not None:
             data = dest_folder.reference
         else:
             data = "@root@"
-        request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
-                                   data=data, headers=headers)
+        request = self.session.put(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/parent-ref',
+            data=data, headers=headers)
         if request.status_code == requests.codes.accepted:
             sleep_sec = 1
             while True:
                 status = self.get_async_progress(request.content.decode("utf-8"))
                 if status != "ACTIVE":
                     return self.entity(entity.entity_type, entity.reference)
                 else:
@@ -1166,15 +1215,16 @@
         xml.etree.ElementTree.SubElement(io_object, "SecurityTag").text = str(security_tag)
         xml.etree.ElementTree.SubElement(io_object, "Parent").text = parent.reference
         rep_object = xml.etree.ElementTree.SubElement(xip_object, "Representation")
         xml.etree.ElementTree.SubElement(rep_object, "Type").text = "Physical"
 
         xml_request = xml.etree.ElementTree.tostring(xip_object, encoding='utf-8')
 
-        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/{IO_PATH}', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/entity/{IO_PATH}', data=xml_request,
+                                    headers=headers)
         if request.status_code == requests.codes.ok:
             xml_string = str(request.content.decode("utf-8"))
             entity = self.entity_from_string(xml_string)
             return Asset(entity['reference'], entity['title'], entity['description'],
                          entity['security_tag'], entity['parent'],
                          entity['metadata'])
         elif request.status_code == requests.codes.unauthorized:
@@ -1523,15 +1573,16 @@
 
         Returns list
 
         :param content_object:
         """
         headers = {HEADER_TOKEN: self.token}
         request = self.session.get(
-            f'{self.protocol}://{self.server}/api/entity/{CO_PATH}/{content_object.reference}/generations', headers=headers)
+            f'{self.protocol}://{self.server}/api/entity/{CO_PATH}/{content_object.reference}/generations',
+            headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             generations = entity_response.findall(f'.//{{{self.entity_ns}}}Generation')
             result = []
             for g in generations:
                 if hasattr(g, 'text'):
@@ -1577,16 +1628,17 @@
 
         :param asset:   The asset
         :returns set[Representation]
         """
         headers = {HEADER_TOKEN: self.token}
         if not isinstance(asset, Asset):
             return None
-        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{asset.path}/{asset.reference}/representations',
-                                   headers=headers)
+        request = self.session.get(
+            f'{self.protocol}://{self.server}/api/entity/{asset.path}/{asset.reference}/representations',
+            headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             representations = entity_response.findall(f'.//{{{self.entity_ns}}}Representation')
             result = set()
             for r in representations:
                 representation = Representation(asset, r.get('type'), r.get("name", None), r.text)
@@ -1612,16 +1664,17 @@
             raise RuntimeError("Thumbnail API is only available when connected to a v6.2 System")
 
         if isinstance(entity, ContentObject):
             raise RuntimeError("Thumbnails cannot be added to Content Objects")
 
         headers = {HEADER_TOKEN: self.token}
 
-        request = self.session.delete(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
-                                      headers=headers)
+        request = self.session.delete(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
+            headers=headers)
         if request.status_code == requests.codes.no_content:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.remove_thumbnail(entity)
         else:
             exception = HTTPException(entity.reference, request.status_code, request.url,
@@ -1642,16 +1695,17 @@
 
         if isinstance(entity, ContentObject):
             raise RuntimeError("Thumbnails cannot be added to Content Objects")
 
         headers = {HEADER_TOKEN: self.token}  # , 'Content-Type': 'application/octet-stream'}
 
         with open(image_file, 'rb') as fd:
-            request = self.session.put(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
-                                       data=fd, headers=headers)
+            request = self.session.put(
+                f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/preview',
+                data=fd, headers=headers)
 
         if request.status_code == requests.codes.no_content:
             return str(request.content.decode('utf-8'))
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_thumbnail(entity, image_file)
         else:
@@ -1667,16 +1721,17 @@
         if self.major_version < 7 and self.minor_version < 1:
             logger.error("Entity events is only available when connected to a v6.1 System")
             raise RuntimeError("Entity events is only available when connected to a v6.1 System")
 
         headers = {HEADER_TOKEN: self.token}
         params = {'start': str(0), 'max': str(maximum)}
 
-        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/event-actions',
-                                   params=params, headers=headers)
+        request = self.session.get(
+            f'{self.protocol}://{self.server}/api/entity/{entity.path}/{entity.reference}/event-actions',
+            params=params, headers=headers)
 
         if request.status_code == requests.codes.ok:
             pass
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self._event_actions(entity, maximum=maximum)
         else:
@@ -1831,15 +1886,16 @@
             params["types"] = kwargs.get("type")
         if "from_date" in kwargs:
             params["from"] = kwargs.get("from_date")
         if "to_date" in kwargs:
             params["to"] = kwargs.get("to_date")
 
         if next_page is None:
-            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/events', params=params, headers=headers)
+            request = self.session.get(f'{self.protocol}://{self.server}/api/entity/events', params=params,
+                                       headers=headers)
         else:
             request = self.session.get(next_page, headers=headers)
 
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
@@ -2102,23 +2158,25 @@
                             xml_object = xml.etree.ElementTree.Element('DeletionAction ', {"xmlns:xip": self.xip_ns,
                                                                                            "xmlns": self.entity_ns})
                             approval_el = xml.etree.ElementTree.SubElement(xml_object, "Approval")
                             xml.etree.ElementTree.SubElement(approval_el, "Approved").text = "true"
                             xml.etree.ElementTree.SubElement(approval_el, "Comment").text = supervisor_comment
                             xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
                             logger.debug(xml_request)
-                            approve = self.session.put(f"{self.protocol}://{self.server}/api/entity/actions/deletions/{progress}",
-                                                       data=xml_request, headers=headers)
+                            approve = self.session.put(
+                                f"{self.protocol}://{self.server}/api/entity/actions/deletions/{progress}",
+                                data=xml_request, headers=headers)
                             if approve.status_code == requests.codes.accepted:
                                 return entity.reference
                             else:
                                 logger.error(approve.content.decode('utf-8'))
                                 raise RuntimeError(approve.status_code, "delete_asset failed during approval")
                         sleep(2.0)
-                req = self.session.get(f"{self.protocol}://{self.server}/api/entity/progress/{progress}", headers=headers)
+                req = self.session.get(f"{self.protocol}://{self.server}/api/entity/progress/{progress}",
+                                       headers=headers)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self._delete_entity(entity, operator_comment, supervisor_comment)
         if request.status_code == requests.codes.unprocessable:
             logger.error(request.content.decode('utf-8'))
             raise RuntimeError(request.status_code, "no active workflow context for full deletion exists in the system")
         if request.status_code == requests.codes.forbidden:
```

### Comparing `pyPreservica-2.0.5/pyPreservica/monitorAPI.py` & `pyPreservica-2.0.6/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/opex.py` & `pyPreservica-2.0.6/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/parAPI.py` & `pyPreservica-2.0.6/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/retentionAPI.py` & `pyPreservica-2.0.6/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/uploadAPI.py` & `pyPreservica-2.0.6/pyPreservica/uploadAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1407,15 +1407,15 @@
                     logger.error("No valid TWITTER_SECRET_KEY found in method arguments, "
                                  "environment variables or credentials.properties file")
                     raise RuntimeError("No valid TWITTER_SECRET_KEY found in method arguments, "
                                        "environment variables or credentials.properties file")
 
         api = None
         try:
-            auth = tweepy.AppAuthHandler(twitter_consumer_key, twitter_secret_key)
+            auth = tweepy.OAuth2AppHandler(twitter_consumer_key, twitter_secret_key)
             api = tweepy.API(auth, wait_on_rate_limit=True)
         except TweepError:
             logger.error("No valid Twitter API keys. Could not authenticate")
             raise RuntimeError("No valid Twitter API keys. Could not authenticate")
         if api is not None:
             logger.debug(api)
             for tweet in tweepy.Cursor(api.user_timeline, id=twitter_user).items(int(num_tweets)):
```

### Comparing `pyPreservica-2.0.5/pyPreservica/webHooksAPI.py` & `pyPreservica-2.0.6/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica/workflowAPI.py` & `pyPreservica-2.0.6/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.0.6/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.5/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.0.6/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.5/setup.py` & `pyPreservica-2.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="2.0.5",
+    version="2.0.6",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

