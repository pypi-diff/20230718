# Comparing `tmp/pyocient-2.0.0.tar.gz` & `tmp/pyocient-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyocient-2.0.0.tar", last modified: Wed May 24 09:33:51 2023, max compression
+gzip compressed data, was "pyocient-3.0.3.tar", last modified: Mon Jul 17 10:40:26 2023, max compression
```

## Comparing `pyocient-2.0.0.tar` & `pyocient-3.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:51.914239 pyocient-2.0.0/
--r-xr-xr-x   0 buildfarm  (1789) users      (100)      581 2023-05-24 09:33:50.000000 pyocient-2.0.0/LICENSE.txt
--rw-r--r--   0 buildfarm  (1789) users      (100)     2178 2023-05-24 09:33:51.914239 pyocient-2.0.0/PKG-INFO
--r-xr-xr-x   0 buildfarm  (1789) users      (100)     1247 2023-05-24 09:33:50.000000 pyocient-2.0.0/README.md
-drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:51.914239 pyocient-2.0.0/pyocient/
--r-xr-xr-x   0 buildfarm  (1789) users      (100)    45506 2023-04-28 19:29:28.000000 pyocient-2.0.0/pyocient/ClientWireProtocol_pb2.py
--r-xr-xr-x   0 buildfarm  (1789) users      (100)     2656 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/__init__.py
--r-xr-xr-x   0 buildfarm  (1789) users      (100)   107955 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/api.py
--r-xr-xr-x   0 buildfarm  (1789) users      (100)    18021 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/cli.py
--r-xr-xr-x   0 buildfarm  (1789) users      (100)       21 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/pkg_version.py
--rw-r--r--   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:50.000000 pyocient-2.0.0/pyocient/py.typed
-drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:51.914239 pyocient-2.0.0/pyocient.egg-info/
--rw-r--r--   0 buildfarm  (1789) users      (100)     2178 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/PKG-INFO
--rw-r--r--   0 buildfarm  (1789) users      (100)      354 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/SOURCES.txt
--rw-r--r--   0 buildfarm  (1789) users      (100)        1 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/dependency_links.txt
--rw-r--r--   0 buildfarm  (1789) users      (100)       48 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/entry_points.txt
--rw-r--r--   0 buildfarm  (1789) users      (100)       89 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/requires.txt
--rw-r--r--   0 buildfarm  (1789) users      (100)        9 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/top_level.txt
--rw-r--r--   0 buildfarm  (1789) users      (100)       38 2023-05-24 09:33:51.914239 pyocient-2.0.0/setup.cfg
--r-xr-xr-x   0 buildfarm  (1789) users      (100)     1941 2023-05-24 09:33:50.000000 pyocient-2.0.0/setup.py
+drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-07-17 10:40:26.701946 pyocient-3.0.3/
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)      581 2023-07-10 10:49:05.000000 pyocient-3.0.3/LICENSE.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)     1965 2023-07-17 10:40:26.701946 pyocient-3.0.3/PKG-INFO
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)     1247 2023-07-10 10:49:05.000000 pyocient-3.0.3/README.md
+drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-07-17 10:40:26.697945 pyocient-3.0.3/pyocient/
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)    38506 2023-06-14 15:14:46.000000 pyocient-3.0.3/pyocient/ClientWireProtocol_pb2.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)     2780 2023-06-09 15:42:52.000000 pyocient-3.0.3/pyocient/__init__.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)   107792 2023-07-07 14:55:59.000000 pyocient-3.0.3/pyocient/api.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)    22612 2023-07-13 20:02:28.000000 pyocient-3.0.3/pyocient/cli.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)       21 2023-07-15 12:50:53.000000 pyocient-3.0.3/pyocient/pkg_version.py
+-rw-r--r--   0 buildfarm  (1789) users      (100)        0 2023-07-17 10:40:24.000000 pyocient-3.0.3/pyocient/py.typed
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)    11098 2023-07-10 16:08:52.000000 pyocient-3.0.3/pyocient/text2sql.py
+drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-07-17 10:40:26.701946 pyocient-3.0.3/pyocient.egg-info/
+-rw-r--r--   0 buildfarm  (1789) users      (100)     1965 2023-07-17 10:40:26.000000 pyocient-3.0.3/pyocient.egg-info/PKG-INFO
+-rw-r--r--   0 buildfarm  (1789) users      (100)      375 2023-07-17 10:40:26.000000 pyocient-3.0.3/pyocient.egg-info/SOURCES.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)        1 2023-07-17 10:40:26.000000 pyocient-3.0.3/pyocient.egg-info/dependency_links.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)       47 2023-07-17 10:40:26.000000 pyocient-3.0.3/pyocient.egg-info/entry_points.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)      144 2023-07-17 10:40:26.000000 pyocient-3.0.3/pyocient.egg-info/requires.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)        9 2023-07-17 10:40:26.000000 pyocient-3.0.3/pyocient.egg-info/top_level.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)       38 2023-07-17 10:40:26.701946 pyocient-3.0.3/setup.cfg
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)     2050 2023-07-10 10:49:05.000000 pyocient-3.0.3/setup.py
```

### Comparing `pyocient-2.0.0/LICENSE.txt` & `pyocient-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyocient-2.0.0/README.md` & `pyocient-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyocient-2.0.0/pyocient/ClientWireProtocol_pb2.py` & `pyocient-3.0.3/pyocient/ClientWireProtocol_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'sharedMessages/clientWireProtocol.proto\x12\nxg.cmdcomp\x1a\x1egoogle/protobuf/wrappers.proto\"\xa2\x01\n\x10\x43lientConnection\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x11\n\tsessionID\x18\x07 \x01(\t\"\xba\x01\n\x13\x43lientConnectionGCM\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x11\n\tsessionID\x18\x07 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x08 \x01(\x08\"\x95\x01\n\x13\x43lientConnectionSSO\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x11\n\tsessionID\x18\x06 \x01(\t\"\xf8\x01\n\x1d\x43lientConnectionSecurityToken\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x11\n\tsessionID\x18\x06 \x01(\t\x12\x15\n\rsecurityToken\x18\x07 \x01(\t\x12\x16\n\x0etokenSignature\x18\x08 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\t \x01(\t\x12\r\n\x05\x66orce\x18\n \x01(\x08\"j\n\x18\x43lientConnectionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"m\n\x1b\x43lientConnectionGCMResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"u\n\x1b\x43lientConnectionSSOResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x11\n\trequestId\x18\x02 \x01(\t\x12\x0f\n\x07\x61uthUrl\x18\x03 \x01(\t\"\xfb\x01\n%ClientConnectionSecurityTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"P\n\x11\x43lientConnection2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\"h\n\x14\x43lientConnectionGCM2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x05 \x01(\x08\"8\n\x14\x43lientConnectionSSO2\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"K\n\rSecurityToken\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x11\n\tsignature\x18\x02 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\x03 \x01(\t\"X\n\x0bSessionInfo\x12\x17\n\x0fserverSessionId\x18\x01 \x01(\t\x12\x30\n\rsecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\" \n\x1e\x43lientConnectionRefreshSession\"\x8a\x01\n&ClientConnectionRefreshSessionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12,\n\x0bsessionInfo\x18\x02 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfo\"S\n\x1c\x43lientConnectionRefreshToken\x12\x33\n\x10oldSecurityToken\x18\x01 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\x8f\x01\n$ClientConnectionRefreshTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x33\n\x10newSecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\")\n\x16SecondaryInterfaceList\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x03(\t\"\xa1\x02\n\x19\x43lientConnection2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\x12\x30\n\rsecurityToken\x18\x08 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\xa4\x02\n\x1c\x43lientConnectionGCM2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\x12\x30\n\rsecurityToken\x18\x08 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\xbd\x02\n\x1c\x43lientConnectionSSO2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12 \n\x16pollingIntervalSeconds\x18\x02 \x01(\x05H\x00\x12.\n\x0bsessionInfo\x18\x03 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfoH\x00\x12\x10\n\x08redirect\x18\x04 \x01(\x08\x12\x14\n\x0credirectHost\x18\x05 \x01(\t\x12\x14\n\x0credirectPort\x18\x06 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x07 \x03(\t\x12\x35\n\tsecondary\x18\x08 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceListB\x10\n\x0eresponse_oneof\"F\n\x13OpenIDAuthenticator\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x10\n\x08\x63lientId\x18\x02 \x01(\t\x12\r\n\x05scope\x18\x03 \x03(\t\"a\n\rAuthenticator\x12>\n\x13openidauthenticator\x18\x01 \x01(\x0b\x32\x1f.xg.cmdcomp.OpenIDAuthenticatorH\x00\x42\x10\n\x0eresponse_oneof\"\'\n\x13\x46\x65tchAuthenticators\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\"\x83\x01\n\x1b\x46\x65tchAuthenticatorsResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x30\n\rauthenticator\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.Authenticator\"\x0b\n\tGetSchema\"W\n\x11GetSchemaResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0e\n\x06schema\x18\x02 \x01(\t\"\x1b\n\tSetSchema\x12\x0e\n\x06schema\x18\x01 \x01(\t\"%\n\x0f\x43loseConnection\x12\x12\n\nendSession\x18\x01 \x01(\x08\"\x10\n\x0eTestConnection\" \n\rAttachToQuery\x12\x0f\n\x07queryId\x18\x01 \x01(\t\"\x1f\n\tFetchData\x12\x12\n\nfetch_size\x18\x01 \x01(\x0f\"A\n\tResultSet\x12\x10\n\x08numParts\x18\x01 \x01(\x05\x12\x13\n\x0b\x62lobLengths\x18\x02 \x03(\x05\x12\r\n\x05\x62lobs\x18\x03 \x03(\x0c\"r\n\x11\x46\x65tchDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12)\n\nresult_set\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSet\"\x0f\n\rFetchMetadata\"\xb9\x02\n\x15\x46\x65tchMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x41\n\x08\x63ols2pos\x18\x02 \x03(\x0b\x32/.xg.cmdcomp.FetchMetadataResponse.Cols2posEntry\x12\x45\n\ncols2Types\x18\x03 \x03(\x0b\x32\x31.xg.cmdcomp.FetchMetadataResponse.Cols2TypesEntry\x1a/\n\rCols2posEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0f:\x02\x38\x01\x1a\x31\n\x0f\x43ols2TypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xde\x04\n\x13\x46\x65tchSystemMetadata\x12@\n\x04\x63\x61ll\x18\x01 \x01(\x0e\x32\x32.xg.cmdcomp.FetchSystemMetadata.SystemMetadataCall\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x04 \x01(\t\x12\x0c\n\x04view\x18\x05 \x01(\t\x12\x0c\n\x04test\x18\x06 \x01(\x08\"\xb9\x03\n\x12SystemMetadataCall\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bGET_SCHEMAS\x10\x01\x12\x0e\n\nGET_TABLES\x10\x02\x12\x15\n\x11GET_SYSTEM_TABLES\x10\x0e\x12\x18\n\x14GET_TABLE_PRIVILEGES\x10\x0f\x12\x19\n\x15GET_COLUMN_PRIVILEGES\x10\x10\x12\r\n\tGET_VIEWS\x10\x19\x12\x0f\n\x0bGET_COLUMNS\x10\x03\x12\x12\n\x0eGET_INDEX_INFO\x10\x04\x12\x11\n\rGET_TYPE_INFO\x10\x05\x12\x14\n\x10GET_SQL_KEYWORDS\x10\x06\x12\x19\n\x15GET_NUMERIC_FUNCTIONS\x10\x07\x12\x18\n\x14GET_STRING_FUNCTIONS\x10\x08\x12\x1b\n\x17GET_TIME_DATE_FUNCTIONS\x10\t\x12\x18\n\x14GET_SYSTEM_FUNCTIONS\x10\n\x12 \n\x1cGET_DATABASE_PRODUCT_VERSION\x10\x0b\x12\x1e\n\x1aGET_DATABASE_MAJOR_VERSION\x10\x0c\x12\x1e\n\x1aGET_DATABASE_MINOR_VERSION\x10\r\"\xbb\x01\n\x1b\x46\x65tchSystemMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12/\n\x0eresult_set_val\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSetH\x00\x12\x14\n\nstring_val\x18\x03 \x01(\tH\x00\x12\x11\n\x07int_val\x18\x04 \x01(\x0fH\x00\x42\x0e\n\x0cresult_oneof\"\x10\n\x0e\x43loseResultSet\"w\n\x0c\x45xecuteQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x15\n\rforceRedirect\x18\x03 \x01(\x08\x12\x34\n\x0fperformanceMode\x18\x04 \x01(\x0e\x32\x1b.xg.cmdcomp.PerformanceMode\"\xb3\x01\n\x14\x45xecuteQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x0f\n\x07queryId\x18\x05 \x01(\t\x12\x18\n\x10numClientThreads\x18\x06 \x01(\x07\"+\n\rExecuteUpdate\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x15\x45xecuteUpdateResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x16\n\x0eupdateRowCount\x18\x02 \x01(\x0f\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"W\n\x0e\x45xecuteExplain\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\xdc\x01\n\x16\x45xecuteExplainForSpark\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32\x33.xg.cmdcomp.ExecuteExplainForSpark.PartitioningType\x12\x19\n\x11partitioningParam\x18\x03 \x01(\x0f\x12\r\n\x05\x66orce\x18\x04 \x01(\x08\"H\n\x10PartitioningType\x12\x18\n\x14INVALID_PARTITIONING\x10\x00\x12\x0b\n\x07\x42Y_SIZE\x10\x01\x12\r\n\tBY_NUMBER\x10\x02\"\x9b\x01\n\x19\x45xplainResponseStringPlan\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0c\n\x04plan\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"V\n\x15\x42\x65ginQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x16\n\x0eserviceClassId\x18\x02 \x01(\t\x12\x0f\n\x07queryId\x18\x03 \x01(\t\"W\n\x16\x46inishQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x16\n\x0eserviceClassId\x18\x02 \x01(\t\x12\x0f\n\x07queryId\x18\x03 \x01(\t\"\xd3\x01\n\x19\x42roadcastQueryConcurrency\x12\x14\n\x0cnodeEndpoint\x18\x01 \x01(\t\x12\x61\n\x16serviceClassIdToCounts\x18\x02 \x03(\x0b\x32\x41.xg.cmdcomp.BroadcastQueryConcurrency.ServiceClassIdToCountsEntry\x1a=\n\x1bServiceClassIdToCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"N\n\x18QueryConcurrencyResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x13\n\x11SystemWideQueries\"x\n\x19SystemWideQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\x87\x02\n\x0cLocalQueries\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\r\n\x05token\x18\x04 \x01(\x0c\x12\x15\n\tsignature\x18\x05 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x07 \x01(\x0c\x12\x14\n\x08username\x18\x08 \x01(\x0c\x42\x02\x18\x01\x12\x11\n\tcompleted\x18\t \x01(\x08\x12\x10\n\x04user\x18\n \x01(\x0c\x42\x02\x18\x01\x42\x15\n\x13one_identity_option\"s\n\x14LocalQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\xd7\x03\n\rSysQueriesRow\x12\x10\n\x08query_id\x18\x01 \x01(\t\x12\x1a\n\x12\x65\x66\x66\x65\x63tive_priority\x18\x02 \x01(\x02\x12\x1a\n\x12\x65stimated_time_sec\x18\x03 \x01(\x05\x12\x0e\n\x06userid\x18\x04 \x01(\t\x12\x10\n\x08sql_text\x18\x05 \x01(\t\x12\x18\n\x10\x65lapsed_time_sec\x18\x06 \x01(\x05\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x14\n\x0cquery_server\x18\x08 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\t \x01(\t\x12\x10\n\x08remoteIP\x18\n \x01(\t\x12\x15\n\rservice_class\x18\x0b \x01(\t\x12\x1d\n\x15\x65stimated_result_rows\x18\x0c \x01(\x03\x12\x1d\n\x15\x65stimated_result_size\x18\r \x01(\x03\x12\x11\n\tsent_rows\x18\x0e \x01(\x03\x12\x12\n\nsent_bytes\x18\x0f \x01(\x03\x12\x18\n\x10initial_priority\x18\x10 \x01(\x02\x12\"\n\x1ainitial_effective_priority\x18\x11 \x01(\x02\x12\x1e\n\x16priority_adjust_factor\x18\x12 \x01(\x02\x12\x1c\n\x14priority_adjust_time\x18\x13 \x01(\r\"\x1c\n\x1aSystemWideCompletedQueries\"}\n\x18\x43ompletedQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12-\n\x04rows\x18\x02 \x03(\x0b\x32\x1f.xg.cmdcomp.CompletedQueriesRow\"\xc0\x05\n\x13\x43ompletedQueriesRow\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x31\n\x0b\x64\x61tabase_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x16\n\x0e\x63lient_version\x18\x03 \x01(\t\x12\x11\n\tclient_ip\x18\x04 \x01(\t\x12\x0b\n\x03sql\x18\x05 \x01(\t\x12\x17\n\x0ftimestamp_start\x18\x06 \x01(\x04\x12\x12\n\ntime_start\x18\x07 \x01(\t\x12\x1a\n\x12timestamp_complete\x18\x08 \x01(\x04\x12\x15\n\rtime_complete\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\x05\x12\r\n\x05state\x18\x0b \x01(\t\x12\x0e\n\x06reason\x18\x0c \x01(\t\x12\x1c\n\x14timestamp_exec_start\x18\r \x01(\x04\x12\x17\n\x0ftime_exec_start\x18\x0e \x01(\t\x12\x0c\n\x04uuid\x18\x0f \x01(\t\x12 \n\x18\x66inal_effective_priority\x18\x10 \x01(\x01\x12\x15\n\rcost_estimate\x18\x11 \x01(\x01\x12\x18\n\x10plan_parallelism\x18\x12 \x01(\r\x12\x16\n\x0eheuristic_cost\x18\x13 \x01(\x01\x12\x15\n\rpso_threshold\x18\x14 \x01(\x03\x12\x15\n\rrows_returned\x18\x15 \x01(\x04\x12\x16\n\x0e\x62ytes_returned\x18\x16 \x01(\x04\x12\x0f\n\x07runtime\x18\x17 \x01(\x04\x12 \n\x18temp_disk_space_consumed\x18\x18 \x01(\x04\x12\x1e\n\x16priority_adjust_factor\x18\x19 \x01(\x02\x12\x1c\n\x14priority_adjust_time\x18\x1a \x01(\r\x12\x18\n\x10initial_priority\x18\x1b \x01(\x02\x12\"\n\x1ainitial_effective_priority\x18\x1c \x01(\x02\"0\n\rLoadBroadcast\x12\x11\n\tcmdcompId\x18\x01 \x01(\t\x12\x0c\n\x04load\x18\x02 \x01(\x01\"3\n\x13\x43\x61\x63heTableReference\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8d\x02\n\nCacheEntry\x12\x10\n\x08\x63md_time\x18\x01 \x01(\x04\x12\x12\n\nquery_uuid\x18\x02 \x01(\t\x12\x12\n\nquery_hash\x18\x03 \x01(\x04\x12-\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1d.xg.cmdcomp.CacheEntry.Action\x12\x15\n\rdatabase_uuid\x18\x05 \x01(\t\x12\x17\n\x0fmax_cached_time\x18\x06 \x01(\x04\x12:\n\x11referenced_tables\x18\x07 \x03(\x0b\x32\x1f.xg.cmdcomp.CacheTableReference\"*\n\x06\x41\x63tion\x12\x0b\n\x07INVALID\x10\x00\x12\x07\n\x03\x41\x44\x44\x10\x01\x12\n\n\x06REMOVE\x10\x02\"X\n\x0bUpdateCache\x12\x13\n\x0bserver_uuid\x18\x01 \x01(\t\x12\r\n\x05\x63lear\x18\x02 \x01(\x08\x12%\n\x05\x65ntry\x18\x03 \x03(\x0b\x32\x16.xg.cmdcomp.CacheEntry\"-\n\nClearCache\x12\x11\n\tall_nodes\x18\x01 \x01(\x08\x12\x0c\n\x04user\x18\x04 \x01(\x0c\"\x89\x1f\n\x07Request\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.xg.cmdcomp.Request.RequestType\x12\x39\n\x11\x63lient_connection\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.ClientConnectionH\x00\x12;\n\x12\x63lient_connection2\x18\x03 \x01(\x0b\x32\x1d.xg.cmdcomp.ClientConnection2H\x00\x12+\n\nget_schema\x18\x04 \x01(\x0b\x32\x15.xg.cmdcomp.GetSchemaH\x00\x12\x37\n\x10\x63lose_connection\x18\x05 \x01(\x0b\x32\x1b.xg.cmdcomp.CloseConnectionH\x00\x12+\n\nset_schema\x18\x06 \x01(\x0b\x32\x15.xg.cmdcomp.SetSchemaH\x00\x12\x35\n\x0ftest_connection\x18\x07 \x01(\x0b\x32\x1a.xg.cmdcomp.TestConnectionH\x00\x12+\n\nfetch_data\x18\x08 \x01(\x0b\x32\x15.xg.cmdcomp.FetchDataH\x00\x12\x33\n\x0e\x66\x65tch_metadata\x18\t \x01(\x0b\x32\x19.xg.cmdcomp.FetchMetadataH\x00\x12\x36\n\x10\x63lose_result_set\x18\n \x01(\x0b\x32\x1a.xg.cmdcomp.CloseResultSetH\x00\x12\x31\n\rexecute_query\x18\x0b \x01(\x0b\x32\x18.xg.cmdcomp.ExecuteQueryH\x00\x12\x35\n\x0f\x65xecute_explain\x18\x0c \x01(\x0b\x32\x1a.xg.cmdcomp.ExecuteExplainH\x00\x12G\n\x19\x65xecute_explain_for_spark\x18\r \x01(\x0b\x32\".xg.cmdcomp.ExecuteExplainForSparkH\x00\x12\x33\n\x0e\x65xecute_update\x18\x0e \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteUpdateH\x00\x12\x33\n\x0eload_broadcast\x18\x0f \x01(\x0b\x32\x19.xg.cmdcomp.LoadBroadcastH\x00\x12@\n\x15\x66\x65tch_system_metadata\x18\x10 \x01(\x0b\x32\x1f.xg.cmdcomp.FetchSystemMetadataH\x00\x12/\n\x0c\x63\x61ncel_query\x18\x11 \x01(\x0b\x32\x17.xg.cmdcomp.CancelQueryH\x00\x12:\n\x12local_cancel_query\x18\x1c \x01(\x0b\x32\x1c.xg.cmdcomp.LocalCancelQueryH\x00\x12<\n\x13system_wide_queries\x18\x12 \x01(\x0b\x32\x1d.xg.cmdcomp.SystemWideQueriesH\x00\x12\x31\n\rlocal_queries\x18\x13 \x01(\x0b\x32\x18.xg.cmdcomp.LocalQueriesH\x00\x12O\n\x1dsystem_wide_completed_queries\x18\x1f \x01(\x0b\x32&.xg.cmdcomp.SystemWideCompletedQueriesH\x00\x12/\n\x0c\x65xecute_plan\x18\x14 \x01(\x0b\x32\x17.xg.cmdcomp.ExecutePlanH\x00\x12/\n\x0c\x65xplain_plan\x18\x15 \x01(\x0b\x32\x17.xg.cmdcomp.ExplainPlanH\x00\x12)\n\tlist_plan\x18\x16 \x01(\x0b\x32\x14.xg.cmdcomp.ListPlanH\x00\x12+\n\nkill_query\x18\x17 \x01(\x0b\x32\x15.xg.cmdcomp.KillQueryH\x00\x12\x36\n\x10local_kill_query\x18\x1d \x01(\x0b\x32\x1a.xg.cmdcomp.LocalKillQueryH\x00\x12<\n\x13\x65xecute_inline_plan\x18\x18 \x01(\x0b\x32\x1d.xg.cmdcomp.ExecuteInlinePlanH\x00\x12\x37\n\x0e\x66orce_external\x18\x19 \x01(\x0b\x32\x19.xg.cmdcomp.ForceExternalB\x02\x18\x01H\x00\x12\x33\n\x0e\x65xecute_export\x18\x1a \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteExportH\x00\x12%\n\x07set_pso\x18\x1b \x01(\x0b\x32\x12.xg.cmdcomp.SetPSOH\x00\x12\x34\n\x0f\x61ttach_to_query\x18\x1e \x01(\x0b\x32\x19.xg.cmdcomp.AttachToQueryH\x00\x12\x44\n\x17\x62\x65gin_query_concurrency\x18  \x01(\x0b\x32!.xg.cmdcomp.BeginQueryConcurrencyH\x00\x12\x46\n\x18\x66inish_query_concurrency\x18! \x01(\x0b\x32\".xg.cmdcomp.FinishQueryConcurrencyH\x00\x12L\n\x1b\x62roadcast_query_concurrency\x18\" \x01(\x0b\x32%.xg.cmdcomp.BroadcastQueryConcurrencyH\x00\x12\x31\n\rset_parameter\x18# \x01(\x0b\x32\x18.xg.cmdcomp.SetParameterH\x00\x12>\n\x10\x65xplain_pipeline\x18$ \x01(\x0b\x32\".xg.cmdcomp.ExplainPipelineRequestH\x00\x12@\n\x15\x63lient_connection_gcm\x18% \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionGCMH\x00\x12\x42\n\x16\x63lient_connection_gcm2\x18& \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionGCM2H\x00\x12\x36\n\ncheck_data\x18\' \x01(\x0b\x32\x1c.xg.cmdcomp.CheckDataRequestB\x02\x18\x01H\x00\x12/\n\x0cupdate_cache\x18( \x01(\x0b\x32\x17.xg.cmdcomp.UpdateCacheH\x00\x12-\n\x0b\x63lear_cache\x18) \x01(\x0b\x32\x16.xg.cmdcomp.ClearCacheH\x00\x12@\n\x15\x63lient_connection_sso\x18* \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionSSOH\x00\x12\x42\n\x16\x63lient_connection_sso2\x18+ \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionSSO2H\x00\x12U\n client_connection_security_token\x18, \x01(\x0b\x32).xg.cmdcomp.ClientConnectionSecurityTokenH\x00\x12W\n!client_connection_refresh_session\x18- \x01(\x0b\x32*.xg.cmdcomp.ClientConnectionRefreshSessionH\x00\x12S\n\x1f\x63lient_connection_refresh_token\x18. \x01(\x0b\x32(.xg.cmdcomp.ClientConnectionRefreshTokenH\x00\x12\x42\n\x16local_invalidate_stats\x18/ \x01(\x0b\x32 .xg.cmdcomp.LocalInvalidateStatsH\x00\x12?\n\x14\x66\x65tch_authenticators\x18\x33 \x01(\x0b\x32\x1f.xg.cmdcomp.FetchAuthenticatorsH\x00\"\xdb\x08\n\x0bRequestType\x12\x0b\n\x07INVALID\x10\x00\x12\x15\n\x11\x43LIENT_CONNECTION\x10\x01\x12\x16\n\x12\x43LIENT_CONNECTION2\x10\x02\x12\x0e\n\nGET_SCHEMA\x10\x03\x12\x14\n\x10\x43LOSE_CONNECTION\x10\x04\x12\x0e\n\nSET_SCHEMA\x10\x05\x12\x13\n\x0fTEST_CONNECTION\x10\x06\x12\x0e\n\nFETCH_DATA\x10\x07\x12\x12\n\x0e\x46\x45TCH_METADATA\x10\x08\x12\x14\n\x10\x43LOSE_RESULT_SET\x10\t\x12\x11\n\rEXECUTE_QUERY\x10\n\x12\x13\n\x0f\x45XECUTE_EXPLAIN\x10\x0b\x12\x1d\n\x19\x45XECUTE_EXPLAIN_FOR_SPARK\x10\x0c\x12\x12\n\x0e\x45XECUTE_UPDATE\x10\r\x12\x12\n\x0eLOAD_BROADCAST\x10\x0e\x12\x19\n\x15\x46\x45TCH_SYSTEM_METADATA\x10\x0f\x12\x10\n\x0c\x43\x41NCEL_QUERY\x10\x10\x12\x16\n\x12LOCAL_CANCEL_QUERY\x10\x1b\x12\x17\n\x13SYSTEM_WIDE_QUERIES\x10\x11\x12\x11\n\rLOCAL_QUERIES\x10\x12\x12!\n\x1dSYSTEM_WIDE_COMPLETED_QUERIES\x10\x1e\x12\x10\n\x0c\x45XECUTE_PLAN\x10\x13\x12\x10\n\x0c\x45XPLAIN_PLAN\x10\x14\x12\r\n\tLIST_PLAN\x10\x15\x12\x0e\n\nKILL_QUERY\x10\x16\x12\x14\n\x10LOCAL_KILL_QUERY\x10\x1c\x12\x17\n\x13\x45XECUTE_INLINE_PLAN\x10\x17\x12\x12\n\x0e\x46ORCE_EXTERNAL\x10\x18\x12\x12\n\x0e\x45XECUTE_EXPORT\x10\x19\x12\x0b\n\x07SET_PSO\x10\x1a\x12\x13\n\x0f\x41TTACH_TO_QUERY\x10\x1d\x12\x1b\n\x17\x42\x45GIN_QUERY_CONCURRENCY\x10\x1f\x12\x1c\n\x18\x46INISH_QUERY_CONCURRENCY\x10 \x12\x1f\n\x1b\x42ROADCAST_QUERY_CONCURRENCY\x10!\x12\x11\n\rSET_PARAMETER\x10\"\x12\x14\n\x10\x45XPLAIN_PIPELINE\x10#\x12\x19\n\x15\x43LIENT_CONNECTION_GCM\x10$\x12\x1a\n\x16\x43LIENT_CONNECTION_GCM2\x10%\x12\x0e\n\nCHECK_DATA\x10&\x12\x10\n\x0cUPDATE_CACHE\x10\'\x12\x0f\n\x0b\x43LEAR_CACHE\x10(\x12\x19\n\x15\x43LIENT_CONNECTION_SSO\x10)\x12\x1a\n\x16\x43LIENT_CONNECTION_SSO2\x10*\x12$\n CLIENT_CONNECTION_SECURITY_TOKEN\x10+\x12%\n!CLIENT_CONNECTION_REFRESH_SESSION\x10,\x12#\n\x1f\x43LIENT_CONNECTION_REFRESH_TOKEN\x10-\x12\x1a\n\x16LOCAL_INVALIDATE_STATS\x10.\x12\x18\n\x14\x46\x45TCH_AUTHENTICATORS\x10\x32\x42\x0f\n\rrequest_oneof\"\xe0\x01\n\x14\x43onfirmationResponse\x12;\n\x04type\x18\x01 \x01(\x0e\x32-.xg.cmdcomp.ConfirmationResponse.ResponseType\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x11\n\tsql_state\x18\x03 \x01(\t\x12\x13\n\x0bvendor_code\x18\x04 \x01(\x0f\"S\n\x0cResponseType\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bRESPONSE_OK\x10\x01\x12\x11\n\rRESPONSE_WARN\x10\x02\x12\x12\n\x0eRESPONSE_ERROR\x10\x03\")\n\x0b\x45xecutePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"/\n\x11\x45xecuteInlinePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"T\n\x0b\x45xplainPlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\"\n\rForceExternal\x12\r\n\x05\x66orce\x18\x01 \x01(\x08:\x02\x18\x01\"\n\n\x08ListPlan\"\x96\x01\n\x10ListPlanResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08planName\x18\x02 \x03(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"\x1a\n\x0b\x43\x61ncelQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"I\n\x13\x43\x61ncelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\xdd\x01\n\x10LocalCancelQuery\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x0b\n\x03sql\x18\x03 \x01(\t\x12\x10\n\x04user\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\r\n\x05token\x18\x05 \x01(\x0c\x12\x15\n\tsignature\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x07 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x08 \x01(\x0c\x42\x15\n\x13one_identity_option\"N\n\x18LocalCancelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x18\n\tKillQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"G\n\x11KillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\xdb\x01\n\x0eLocalKillQuery\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x0b\n\x03sql\x18\x03 \x01(\t\x12\x10\n\x04user\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\r\n\x05token\x18\x05 \x01(\x0c\x12\x15\n\tsignature\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x07 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x08 \x01(\x0c\x42\x15\n\x13one_identity_option\"L\n\x16LocalKillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"o\n\x14LocalInvalidateStats\x12\r\n\x05token\x18\x01 \x01(\x0c\x12\x11\n\tsignature\x18\x02 \x01(\x0c\x12\x1a\n\x12issuer_fingerprint\x18\x03 \x01(\x0c\x12\x19\n\x11invalidation_uuid\x18\x04 \x01(\t\"R\n\x1cLocalInvalidateStatsResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"+\n\rExecuteExport\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa2\x01\n\x15\x45xecuteExportResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x17\n\x0f\x65xportStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"4\n\x16\x45xplainPipelineRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa6\x01\n\x17\x45xplainPipelineResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x19\n\x11pipelineStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\".\n\x10\x43heckDataRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x11\x43heckDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x1a\n\x12\x63heckDataStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"*\n\x06SetPSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x12\r\n\x05reset\x18\x02 \x01(\x08\"\xf0\n\n\x0cSetParameter\x12\r\n\x05reset\x18\x01 \x01(\x08\x12\x35\n\rpso_threshold\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.SetParameter.PSOH\x00\x12\x36\n\trow_limit\x18\x03 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.RowLimitH\x00\x12\x38\n\ntime_limit\x18\x04 \x01(\x0b\x32\".xg.cmdcomp.SetParameter.TimeLimitH\x00\x12\x44\n\x0ftemp_disk_limit\x18\x05 \x01(\x0b\x32).xg.cmdcomp.SetParameter.MaxTempDiskLimitH\x00\x12\x35\n\x08priority\x18\x06 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.PriorityH\x00\x12;\n\x0b\x63oncurrency\x18\x07 \x01(\x0b\x32$.xg.cmdcomp.SetParameter.ConcurrencyH\x00\x12\x34\n\x08pso_seed\x18\x08 \x01(\x0b\x32 .xg.cmdcomp.SetParameter.PSOSeedH\x00\x12P\n\x17result_set_column_limit\x18\t \x01(\x0b\x32-.xg.cmdcomp.SetParameter.ResultSetColumnLimitH\x00\x12@\n\x0e\x66orce_external\x18\n \x01(\x0b\x32&.xg.cmdcomp.SetParameter.ForceExternalH\x00\x12O\n\x16priority_adjust_factor\x18\x0b \x01(\x0b\x32-.xg.cmdcomp.SetParameter.PriorityAdjustFactorH\x00\x12K\n\x14priority_adjust_time\x18\x0c \x01(\x0b\x32+.xg.cmdcomp.SetParameter.PriorityAdjustTimeH\x00\x12G\n\x12service_class_name\x18\r \x01(\x0b\x32).xg.cmdcomp.SetParameter.ServiceClassNameH\x00\x12@\n\x0ememory_tracing\x18\x0e \x01(\x0b\x32&.xg.cmdcomp.SetParameter.MemoryTracingH\x00\x1a\x18\n\x03PSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x1a\x1c\n\x08RowLimit\x12\x10\n\x08rowLimit\x18\x01 \x01(\x03\x1a\x1e\n\tTimeLimit\x12\x11\n\ttimeLimit\x18\x01 \x01(\x03\x1a)\n\x10MaxTempDiskLimit\x12\x15\n\rtempDiskLimit\x18\x01 \x01(\x03\x1a\x34\n\x14ResultSetColumnLimit\x12\x1c\n\x14resultSetColumnLimit\x18\x01 \x01(\x03\x1a\x1c\n\x08Priority\x12\x10\n\x08priority\x18\x01 \x01(\x01\x1a\"\n\x0b\x43oncurrency\x12\x13\n\x0b\x63oncurrency\x18\x01 \x01(\x03\x1a\x17\n\x07PSOSeed\x12\x0c\n\x04seed\x18\x01 \x01(\x04\x1a\x1e\n\rForceExternal\x12\r\n\x05is_on\x18\x01 \x01(\x08\x1a\x36\n\x14PriorityAdjustFactor\x12\x1e\n\x16priority_adjust_factor\x18\x01 \x01(\x01\x1a\x32\n\x12PriorityAdjustTime\x12\x1c\n\x14priority_adjust_time\x18\x01 \x01(\r\x1a.\n\x10ServiceClassName\x12\x1a\n\x12service_class_name\x18\x01 \x01(\t\x1a\x1e\n\rMemoryTracing\x12\r\n\x05is_on\x18\x01 \x01(\x08\x42\x0b\n\tParameter*4\n\x0fPerformanceMode\x12\x07\n\x03OFF\x10\x00\x12\x18\n\x14ROOT_OP_INST_DISCARD\x10\x01*/\n\rExplainFormat\x12\t\n\x05PROTO\x10\x00\x12\x08\n\x04JSON\x10\x01\x12\t\n\x05\x44\x45\x42UG\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'sharedMessages/clientWireProtocol.proto\x12\nxg.cmdcomp\x1a\x1egoogle/protobuf/wrappers.proto\"\xbe\x01\n\x10\x43lientConnection\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x1a\n\x12patchClientVersion\x18\x08 \x01(\t\x12\x11\n\tsessionID\x18\x07 \x01(\t\"\xd6\x01\n\x13\x43lientConnectionGCM\x12\x0e\n\x06userid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x10\n\x08\x63lientid\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x06 \x01(\x05\x12\x1a\n\x12patchClientVersion\x18\t \x01(\t\x12\x11\n\tsessionID\x18\x07 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x08 \x01(\x08\"\xb1\x01\n\x13\x43lientConnectionSSO\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12patchClientVersion\x18\x07 \x01(\t\x12\x11\n\tsessionID\x18\x06 \x01(\t\"\x94\x02\n\x1d\x43lientConnectionSecurityToken\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x10\n\x08\x63lientid\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1a\n\x12majorClientVersion\x18\x04 \x01(\x05\x12\x1a\n\x12minorClientVersion\x18\x05 \x01(\x05\x12\x1a\n\x12patchClientVersion\x18\x0b \x01(\t\x12\x11\n\tsessionID\x18\x06 \x01(\t\x12\x15\n\rsecurityToken\x18\x07 \x01(\t\x12\x16\n\x0etokenSignature\x18\x08 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\t \x01(\t\x12\r\n\x05\x66orce\x18\n \x01(\x08\"j\n\x18\x43lientConnectionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"m\n\x1b\x43lientConnectionGCMResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\n\n\x02iv\x18\x02 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x03 \x01(\t\"u\n\x1b\x43lientConnectionSSOResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x11\n\trequestId\x18\x02 \x01(\t\x12\x0f\n\x07\x61uthUrl\x18\x03 \x01(\t\"\xfb\x01\n%ClientConnectionSecurityTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\"P\n\x11\x43lientConnection2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\"h\n\x14\x43lientConnectionGCM2\x12\x0e\n\x06\x63ipher\x18\x01 \x01(\x0c\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0c\n\x04hmac\x18\x03 \x01(\x0c\x12\x0e\n\x06pubKey\x18\x04 \x01(\t\x12\x13\n\x0b\x65xplicitSSO\x18\x05 \x01(\x08\"8\n\x14\x43lientConnectionSSO2\x12\x11\n\trequestId\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"K\n\rSecurityToken\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x11\n\tsignature\x18\x02 \x01(\t\x12\x19\n\x11issuerFingerprint\x18\x03 \x01(\t\"X\n\x0bSessionInfo\x12\x17\n\x0fserverSessionId\x18\x01 \x01(\t\x12\x30\n\rsecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\" \n\x1e\x43lientConnectionRefreshSession\"\x8a\x01\n&ClientConnectionRefreshSessionResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12,\n\x0bsessionInfo\x18\x02 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfo\"S\n\x1c\x43lientConnectionRefreshToken\x12\x33\n\x10oldSecurityToken\x18\x01 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\x8f\x01\n$ClientConnectionRefreshTokenResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x33\n\x10newSecurityToken\x18\x02 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\")\n\x16SecondaryInterfaceList\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x03(\t\"\xa1\x02\n\x19\x43lientConnection2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\x12\x30\n\rsecurityToken\x18\x08 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\xa4\x02\n\x1c\x43lientConnectionGCM2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x05 \x03(\t\x12\x35\n\tsecondary\x18\x06 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceList\x12\x17\n\x0fserverSessionId\x18\x07 \x01(\t\x12\x30\n\rsecurityToken\x18\x08 \x01(\x0b\x32\x19.xg.cmdcomp.SecurityToken\"\xbd\x02\n\x1c\x43lientConnectionSSO2Response\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12 \n\x16pollingIntervalSeconds\x18\x02 \x01(\x05H\x00\x12.\n\x0bsessionInfo\x18\x03 \x01(\x0b\x32\x17.xg.cmdcomp.SessionInfoH\x00\x12\x10\n\x08redirect\x18\x04 \x01(\x08\x12\x14\n\x0credirectHost\x18\x05 \x01(\t\x12\x14\n\x0credirectPort\x18\x06 \x01(\x07\x12\x10\n\x08\x63mdcomps\x18\x07 \x03(\t\x12\x35\n\tsecondary\x18\x08 \x03(\x0b\x32\".xg.cmdcomp.SecondaryInterfaceListB\x10\n\x0eresponse_oneof\"F\n\x13OpenIDAuthenticator\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x10\n\x08\x63lientId\x18\x02 \x01(\t\x12\r\n\x05scope\x18\x03 \x03(\t\"a\n\rAuthenticator\x12>\n\x13openidauthenticator\x18\x01 \x01(\x0b\x32\x1f.xg.cmdcomp.OpenIDAuthenticatorH\x00\x42\x10\n\x0eresponse_oneof\"\'\n\x13\x46\x65tchAuthenticators\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\"\x83\x01\n\x1b\x46\x65tchAuthenticatorsResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x30\n\rauthenticator\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.Authenticator\"\x0b\n\tGetSchema\"W\n\x11GetSchemaResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0e\n\x06schema\x18\x02 \x01(\t\"\x1b\n\tSetSchema\x12\x0e\n\x06schema\x18\x01 \x01(\t\"%\n\x0f\x43loseConnection\x12\x12\n\nendSession\x18\x01 \x01(\x08\"\x10\n\x0eTestConnection\" \n\rAttachToQuery\x12\x0f\n\x07queryId\x18\x01 \x01(\t\"\x1f\n\tFetchData\x12\x12\n\nfetch_size\x18\x01 \x01(\x0f\"A\n\tResultSet\x12\x10\n\x08numParts\x18\x01 \x01(\x05\x12\x13\n\x0b\x62lobLengths\x18\x02 \x03(\x05\x12\r\n\x05\x62lobs\x18\x03 \x03(\x0c\"r\n\x11\x46\x65tchDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12)\n\nresult_set\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSet\"\x0f\n\rFetchMetadata\"\xb9\x02\n\x15\x46\x65tchMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x41\n\x08\x63ols2pos\x18\x02 \x03(\x0b\x32/.xg.cmdcomp.FetchMetadataResponse.Cols2posEntry\x12\x45\n\ncols2Types\x18\x03 \x03(\x0b\x32\x31.xg.cmdcomp.FetchMetadataResponse.Cols2TypesEntry\x1a/\n\rCols2posEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0f:\x02\x38\x01\x1a\x31\n\x0f\x43ols2TypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xde\x04\n\x13\x46\x65tchSystemMetadata\x12@\n\x04\x63\x61ll\x18\x01 \x01(\x0e\x32\x32.xg.cmdcomp.FetchSystemMetadata.SystemMetadataCall\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\r\n\x05table\x18\x03 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x04 \x01(\t\x12\x0c\n\x04view\x18\x05 \x01(\t\x12\x0c\n\x04test\x18\x06 \x01(\x08\"\xb9\x03\n\x12SystemMetadataCall\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bGET_SCHEMAS\x10\x01\x12\x0e\n\nGET_TABLES\x10\x02\x12\x15\n\x11GET_SYSTEM_TABLES\x10\x0e\x12\x18\n\x14GET_TABLE_PRIVILEGES\x10\x0f\x12\x19\n\x15GET_COLUMN_PRIVILEGES\x10\x10\x12\r\n\tGET_VIEWS\x10\x19\x12\x0f\n\x0bGET_COLUMNS\x10\x03\x12\x12\n\x0eGET_INDEX_INFO\x10\x04\x12\x11\n\rGET_TYPE_INFO\x10\x05\x12\x14\n\x10GET_SQL_KEYWORDS\x10\x06\x12\x19\n\x15GET_NUMERIC_FUNCTIONS\x10\x07\x12\x18\n\x14GET_STRING_FUNCTIONS\x10\x08\x12\x1b\n\x17GET_TIME_DATE_FUNCTIONS\x10\t\x12\x18\n\x14GET_SYSTEM_FUNCTIONS\x10\n\x12 \n\x1cGET_DATABASE_PRODUCT_VERSION\x10\x0b\x12\x1e\n\x1aGET_DATABASE_MAJOR_VERSION\x10\x0c\x12\x1e\n\x1aGET_DATABASE_MINOR_VERSION\x10\r\"\xbb\x01\n\x1b\x46\x65tchSystemMetadataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12/\n\x0eresult_set_val\x18\x02 \x01(\x0b\x32\x15.xg.cmdcomp.ResultSetH\x00\x12\x14\n\nstring_val\x18\x03 \x01(\tH\x00\x12\x11\n\x07int_val\x18\x04 \x01(\x0fH\x00\x42\x0e\n\x0cresult_oneof\"\x10\n\x0e\x43loseResultSet\"w\n\x0c\x45xecuteQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x15\n\rforceRedirect\x18\x03 \x01(\x08\x12\x34\n\x0fperformanceMode\x18\x04 \x01(\x0e\x32\x1b.xg.cmdcomp.PerformanceMode\"\xb3\x01\n\x14\x45xecuteQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08redirect\x18\x02 \x01(\x08\x12\x14\n\x0credirectHost\x18\x03 \x01(\t\x12\x14\n\x0credirectPort\x18\x04 \x01(\x07\x12\x0f\n\x07queryId\x18\x05 \x01(\t\x12\x18\n\x10numClientThreads\x18\x06 \x01(\x07\"+\n\rExecuteUpdate\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x15\x45xecuteUpdateResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x16\n\x0eupdateRowCount\x18\x02 \x01(\x0f\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"W\n\x0e\x45xecuteExplain\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\xdc\x01\n\x16\x45xecuteExplainForSpark\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\x41\n\x04type\x18\x02 \x01(\x0e\x32\x33.xg.cmdcomp.ExecuteExplainForSpark.PartitioningType\x12\x19\n\x11partitioningParam\x18\x03 \x01(\x0f\x12\r\n\x05\x66orce\x18\x04 \x01(\x08\"H\n\x10PartitioningType\x12\x18\n\x14INVALID_PARTITIONING\x10\x00\x12\x0b\n\x07\x42Y_SIZE\x10\x01\x12\r\n\tBY_NUMBER\x10\x02\"\x9b\x01\n\x19\x45xplainResponseStringPlan\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x0c\n\x04plan\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"N\n\x18QueryConcurrencyResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x13\n\x11SystemWideQueries\"x\n\x19SystemWideQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\x87\x02\n\x0cLocalQueries\x12\x14\n\x08identity\x18\x01 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\ruuid_identity\x18\x02 \x01(\x0c\x42\x02\x18\x01H\x00\x12\x10\n\x08\x64\x61tabase\x18\x03 \x01(\t\x12\r\n\x05token\x18\x04 \x01(\x0c\x12\x15\n\tsignature\x18\x05 \x01(\x0c\x42\x02\x18\x01\x12\x1e\n\x12issuer_certificate\x18\x06 \x01(\x0c\x42\x02\x18\x01\x12\x1a\n\x12issuer_fingerprint\x18\x07 \x01(\x0c\x12\x14\n\x08username\x18\x08 \x01(\x0c\x42\x02\x18\x01\x12\x11\n\tcompleted\x18\t \x01(\x08\x12\x10\n\x04user\x18\n \x01(\x0c\x42\x02\x18\x01\x42\x15\n\x13one_identity_option\"s\n\x14LocalQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\'\n\x04rows\x18\x02 \x03(\x0b\x32\x19.xg.cmdcomp.SysQueriesRow\"\xd7\x03\n\rSysQueriesRow\x12\x10\n\x08query_id\x18\x01 \x01(\t\x12\x1a\n\x12\x65\x66\x66\x65\x63tive_priority\x18\x02 \x01(\x02\x12\x1a\n\x12\x65stimated_time_sec\x18\x03 \x01(\x05\x12\x0e\n\x06userid\x18\x04 \x01(\t\x12\x10\n\x08sql_text\x18\x05 \x01(\t\x12\x18\n\x10\x65lapsed_time_sec\x18\x06 \x01(\x05\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x14\n\x0cquery_server\x18\x08 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\t \x01(\t\x12\x10\n\x08remoteIP\x18\n \x01(\t\x12\x15\n\rservice_class\x18\x0b \x01(\t\x12\x1d\n\x15\x65stimated_result_rows\x18\x0c \x01(\x03\x12\x1d\n\x15\x65stimated_result_size\x18\r \x01(\x03\x12\x11\n\tsent_rows\x18\x0e \x01(\x03\x12\x12\n\nsent_bytes\x18\x0f \x01(\x03\x12\x18\n\x10initial_priority\x18\x10 \x01(\x02\x12\"\n\x1ainitial_effective_priority\x18\x11 \x01(\x02\x12\x1e\n\x16priority_adjust_factor\x18\x12 \x01(\x02\x12\x1c\n\x14priority_adjust_time\x18\x13 \x01(\r\"\x1c\n\x1aSystemWideCompletedQueries\"}\n\x18\x43ompletedQueriesResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12-\n\x04rows\x18\x02 \x03(\x0b\x32\x1f.xg.cmdcomp.CompletedQueriesRow\"\xc0\x05\n\x13\x43ompletedQueriesRow\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x31\n\x0b\x64\x61tabase_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x16\n\x0e\x63lient_version\x18\x03 \x01(\t\x12\x11\n\tclient_ip\x18\x04 \x01(\t\x12\x0b\n\x03sql\x18\x05 \x01(\t\x12\x17\n\x0ftimestamp_start\x18\x06 \x01(\x04\x12\x12\n\ntime_start\x18\x07 \x01(\t\x12\x1a\n\x12timestamp_complete\x18\x08 \x01(\x04\x12\x15\n\rtime_complete\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\x05\x12\r\n\x05state\x18\x0b \x01(\t\x12\x0e\n\x06reason\x18\x0c \x01(\t\x12\x1c\n\x14timestamp_exec_start\x18\r \x01(\x04\x12\x17\n\x0ftime_exec_start\x18\x0e \x01(\t\x12\x0c\n\x04uuid\x18\x0f \x01(\t\x12 \n\x18\x66inal_effective_priority\x18\x10 \x01(\x01\x12\x15\n\rcost_estimate\x18\x11 \x01(\x01\x12\x18\n\x10plan_parallelism\x18\x12 \x01(\r\x12\x16\n\x0eheuristic_cost\x18\x13 \x01(\x01\x12\x15\n\rpso_threshold\x18\x14 \x01(\x03\x12\x15\n\rrows_returned\x18\x15 \x01(\x04\x12\x16\n\x0e\x62ytes_returned\x18\x16 \x01(\x04\x12\x0f\n\x07runtime\x18\x17 \x01(\x04\x12 \n\x18temp_disk_space_consumed\x18\x18 \x01(\x04\x12\x1e\n\x16priority_adjust_factor\x18\x19 \x01(\x02\x12\x1c\n\x14priority_adjust_time\x18\x1a \x01(\r\x12\x18\n\x10initial_priority\x18\x1b \x01(\x02\x12\"\n\x1ainitial_effective_priority\x18\x1c \x01(\x02\"\x1f\n\nClearCache\x12\x11\n\tall_nodes\x18\x01 \x01(\x08\"\xc3\x19\n\x07Request\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.xg.cmdcomp.Request.RequestType\x12\x39\n\x11\x63lient_connection\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.ClientConnectionH\x00\x12;\n\x12\x63lient_connection2\x18\x03 \x01(\x0b\x32\x1d.xg.cmdcomp.ClientConnection2H\x00\x12+\n\nget_schema\x18\x04 \x01(\x0b\x32\x15.xg.cmdcomp.GetSchemaH\x00\x12\x37\n\x10\x63lose_connection\x18\x05 \x01(\x0b\x32\x1b.xg.cmdcomp.CloseConnectionH\x00\x12+\n\nset_schema\x18\x06 \x01(\x0b\x32\x15.xg.cmdcomp.SetSchemaH\x00\x12\x35\n\x0ftest_connection\x18\x07 \x01(\x0b\x32\x1a.xg.cmdcomp.TestConnectionH\x00\x12+\n\nfetch_data\x18\x08 \x01(\x0b\x32\x15.xg.cmdcomp.FetchDataH\x00\x12\x33\n\x0e\x66\x65tch_metadata\x18\t \x01(\x0b\x32\x19.xg.cmdcomp.FetchMetadataH\x00\x12\x36\n\x10\x63lose_result_set\x18\n \x01(\x0b\x32\x1a.xg.cmdcomp.CloseResultSetH\x00\x12\x31\n\rexecute_query\x18\x0b \x01(\x0b\x32\x18.xg.cmdcomp.ExecuteQueryH\x00\x12\x35\n\x0f\x65xecute_explain\x18\x0c \x01(\x0b\x32\x1a.xg.cmdcomp.ExecuteExplainH\x00\x12G\n\x19\x65xecute_explain_for_spark\x18\r \x01(\x0b\x32\".xg.cmdcomp.ExecuteExplainForSparkH\x00\x12\x33\n\x0e\x65xecute_update\x18\x0e \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteUpdateH\x00\x12@\n\x15\x66\x65tch_system_metadata\x18\x10 \x01(\x0b\x32\x1f.xg.cmdcomp.FetchSystemMetadataH\x00\x12/\n\x0c\x63\x61ncel_query\x18\x11 \x01(\x0b\x32\x17.xg.cmdcomp.CancelQueryH\x00\x12<\n\x13system_wide_queries\x18\x12 \x01(\x0b\x32\x1d.xg.cmdcomp.SystemWideQueriesH\x00\x12\x31\n\rlocal_queries\x18\x13 \x01(\x0b\x32\x18.xg.cmdcomp.LocalQueriesH\x00\x12O\n\x1dsystem_wide_completed_queries\x18\x1f \x01(\x0b\x32&.xg.cmdcomp.SystemWideCompletedQueriesH\x00\x12/\n\x0c\x65xecute_plan\x18\x14 \x01(\x0b\x32\x17.xg.cmdcomp.ExecutePlanH\x00\x12/\n\x0c\x65xplain_plan\x18\x15 \x01(\x0b\x32\x17.xg.cmdcomp.ExplainPlanH\x00\x12)\n\tlist_plan\x18\x16 \x01(\x0b\x32\x14.xg.cmdcomp.ListPlanH\x00\x12+\n\nkill_query\x18\x17 \x01(\x0b\x32\x15.xg.cmdcomp.KillQueryH\x00\x12<\n\x13\x65xecute_inline_plan\x18\x18 \x01(\x0b\x32\x1d.xg.cmdcomp.ExecuteInlinePlanH\x00\x12\x37\n\x0e\x66orce_external\x18\x19 \x01(\x0b\x32\x19.xg.cmdcomp.ForceExternalB\x02\x18\x01H\x00\x12\x33\n\x0e\x65xecute_export\x18\x1a \x01(\x0b\x32\x19.xg.cmdcomp.ExecuteExportH\x00\x12%\n\x07set_pso\x18\x1b \x01(\x0b\x32\x12.xg.cmdcomp.SetPSOH\x00\x12\x34\n\x0f\x61ttach_to_query\x18\x1e \x01(\x0b\x32\x19.xg.cmdcomp.AttachToQueryH\x00\x12\x31\n\rset_parameter\x18# \x01(\x0b\x32\x18.xg.cmdcomp.SetParameterH\x00\x12>\n\x10\x65xplain_pipeline\x18$ \x01(\x0b\x32\".xg.cmdcomp.ExplainPipelineRequestH\x00\x12@\n\x15\x63lient_connection_gcm\x18% \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionGCMH\x00\x12\x42\n\x16\x63lient_connection_gcm2\x18& \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionGCM2H\x00\x12\x36\n\ncheck_data\x18\' \x01(\x0b\x32\x1c.xg.cmdcomp.CheckDataRequestB\x02\x18\x01H\x00\x12-\n\x0b\x63lear_cache\x18) \x01(\x0b\x32\x16.xg.cmdcomp.ClearCacheH\x00\x12@\n\x15\x63lient_connection_sso\x18* \x01(\x0b\x32\x1f.xg.cmdcomp.ClientConnectionSSOH\x00\x12\x42\n\x16\x63lient_connection_sso2\x18+ \x01(\x0b\x32 .xg.cmdcomp.ClientConnectionSSO2H\x00\x12U\n client_connection_security_token\x18, \x01(\x0b\x32).xg.cmdcomp.ClientConnectionSecurityTokenH\x00\x12W\n!client_connection_refresh_session\x18- \x01(\x0b\x32*.xg.cmdcomp.ClientConnectionRefreshSessionH\x00\x12S\n\x1f\x63lient_connection_refresh_token\x18. \x01(\x0b\x32(.xg.cmdcomp.ClientConnectionRefreshTokenH\x00\x12?\n\x14\x66\x65tch_authenticators\x18\x33 \x01(\x0b\x32\x1f.xg.cmdcomp.FetchAuthenticatorsH\x00\"\x8f\x07\n\x0bRequestType\x12\x0b\n\x07INVALID\x10\x00\x12\x15\n\x11\x43LIENT_CONNECTION\x10\x01\x12\x16\n\x12\x43LIENT_CONNECTION2\x10\x02\x12\x0e\n\nGET_SCHEMA\x10\x03\x12\x14\n\x10\x43LOSE_CONNECTION\x10\x04\x12\x0e\n\nSET_SCHEMA\x10\x05\x12\x13\n\x0fTEST_CONNECTION\x10\x06\x12\x0e\n\nFETCH_DATA\x10\x07\x12\x12\n\x0e\x46\x45TCH_METADATA\x10\x08\x12\x14\n\x10\x43LOSE_RESULT_SET\x10\t\x12\x11\n\rEXECUTE_QUERY\x10\n\x12\x13\n\x0f\x45XECUTE_EXPLAIN\x10\x0b\x12\x1d\n\x19\x45XECUTE_EXPLAIN_FOR_SPARK\x10\x0c\x12\x12\n\x0e\x45XECUTE_UPDATE\x10\r\x12\x19\n\x15\x46\x45TCH_SYSTEM_METADATA\x10\x0f\x12\x10\n\x0c\x43\x41NCEL_QUERY\x10\x10\x12\x17\n\x13SYSTEM_WIDE_QUERIES\x10\x11\x12\x11\n\rLOCAL_QUERIES\x10\x12\x12!\n\x1dSYSTEM_WIDE_COMPLETED_QUERIES\x10\x1e\x12\x10\n\x0c\x45XECUTE_PLAN\x10\x13\x12\x10\n\x0c\x45XPLAIN_PLAN\x10\x14\x12\r\n\tLIST_PLAN\x10\x15\x12\x0e\n\nKILL_QUERY\x10\x16\x12\x17\n\x13\x45XECUTE_INLINE_PLAN\x10\x17\x12\x12\n\x0e\x46ORCE_EXTERNAL\x10\x18\x12\x12\n\x0e\x45XECUTE_EXPORT\x10\x19\x12\x0b\n\x07SET_PSO\x10\x1a\x12\x13\n\x0f\x41TTACH_TO_QUERY\x10\x1d\x12\x11\n\rSET_PARAMETER\x10\"\x12\x14\n\x10\x45XPLAIN_PIPELINE\x10#\x12\x19\n\x15\x43LIENT_CONNECTION_GCM\x10$\x12\x1a\n\x16\x43LIENT_CONNECTION_GCM2\x10%\x12\x0e\n\nCHECK_DATA\x10&\x12\x0f\n\x0b\x43LEAR_CACHE\x10(\x12\x19\n\x15\x43LIENT_CONNECTION_SSO\x10)\x12\x1a\n\x16\x43LIENT_CONNECTION_SSO2\x10*\x12$\n CLIENT_CONNECTION_SECURITY_TOKEN\x10+\x12%\n!CLIENT_CONNECTION_REFRESH_SESSION\x10,\x12#\n\x1f\x43LIENT_CONNECTION_REFRESH_TOKEN\x10-\x12\x18\n\x14\x46\x45TCH_AUTHENTICATORS\x10\x32\x42\x0f\n\rrequest_oneof\"\xe0\x01\n\x14\x43onfirmationResponse\x12;\n\x04type\x18\x01 \x01(\x0e\x32-.xg.cmdcomp.ConfirmationResponse.ResponseType\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x11\n\tsql_state\x18\x03 \x01(\t\x12\x13\n\x0bvendor_code\x18\x04 \x01(\x0f\"S\n\x0cResponseType\x12\x0b\n\x07INVALID\x10\x00\x12\x0f\n\x0bRESPONSE_OK\x10\x01\x12\x11\n\rRESPONSE_WARN\x10\x02\x12\x12\n\x0eRESPONSE_ERROR\x10\x03\")\n\x0b\x45xecutePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"/\n\x11\x45xecuteInlinePlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"T\n\x0b\x45xplainPlan\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12)\n\x06\x66ormat\x18\x03 \x01(\x0e\x32\x19.xg.cmdcomp.ExplainFormat\"\"\n\rForceExternal\x12\r\n\x05\x66orce\x18\x01 \x01(\x08:\x02\x18\x01\"\n\n\x08ListPlan\"\x96\x01\n\x10ListPlanResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x10\n\x08planName\x18\x02 \x03(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"\x1a\n\x0b\x43\x61ncelQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"I\n\x13\x43\x61ncelQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"\x18\n\tKillQuery\x12\x0b\n\x03sql\x18\x01 \x01(\t\"G\n\x11KillQueryResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\"+\n\rExecuteExport\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa2\x01\n\x15\x45xecuteExportResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x17\n\x0f\x65xportStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"4\n\x16\x45xplainPipelineRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa6\x01\n\x17\x45xplainPipelineResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x19\n\x11pipelineStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\".\n\x10\x43heckDataRequest\x12\x0b\n\x03sql\x18\x01 \x01(\t\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xa1\x01\n\x11\x43heckDataResponse\x12\x32\n\x08response\x18\x01 \x01(\x0b\x32 .xg.cmdcomp.ConfirmationResponse\x12\x1a\n\x12\x63heckDataStatement\x18\x02 \x01(\t\x12\x10\n\x08redirect\x18\x03 \x01(\x08\x12\x14\n\x0credirectHost\x18\x04 \x01(\t\x12\x14\n\x0credirectPort\x18\x05 \x01(\x07\"*\n\x06SetPSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x12\r\n\x05reset\x18\x02 \x01(\x08\"\xf0\n\n\x0cSetParameter\x12\r\n\x05reset\x18\x01 \x01(\x08\x12\x35\n\rpso_threshold\x18\x02 \x01(\x0b\x32\x1c.xg.cmdcomp.SetParameter.PSOH\x00\x12\x36\n\trow_limit\x18\x03 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.RowLimitH\x00\x12\x38\n\ntime_limit\x18\x04 \x01(\x0b\x32\".xg.cmdcomp.SetParameter.TimeLimitH\x00\x12\x44\n\x0ftemp_disk_limit\x18\x05 \x01(\x0b\x32).xg.cmdcomp.SetParameter.MaxTempDiskLimitH\x00\x12\x35\n\x08priority\x18\x06 \x01(\x0b\x32!.xg.cmdcomp.SetParameter.PriorityH\x00\x12;\n\x0b\x63oncurrency\x18\x07 \x01(\x0b\x32$.xg.cmdcomp.SetParameter.ConcurrencyH\x00\x12\x34\n\x08pso_seed\x18\x08 \x01(\x0b\x32 .xg.cmdcomp.SetParameter.PSOSeedH\x00\x12P\n\x17result_set_column_limit\x18\t \x01(\x0b\x32-.xg.cmdcomp.SetParameter.ResultSetColumnLimitH\x00\x12@\n\x0e\x66orce_external\x18\n \x01(\x0b\x32&.xg.cmdcomp.SetParameter.ForceExternalH\x00\x12O\n\x16priority_adjust_factor\x18\x0b \x01(\x0b\x32-.xg.cmdcomp.SetParameter.PriorityAdjustFactorH\x00\x12K\n\x14priority_adjust_time\x18\x0c \x01(\x0b\x32+.xg.cmdcomp.SetParameter.PriorityAdjustTimeH\x00\x12G\n\x12service_class_name\x18\r \x01(\x0b\x32).xg.cmdcomp.SetParameter.ServiceClassNameH\x00\x12@\n\x0ememory_tracing\x18\x0e \x01(\x0b\x32&.xg.cmdcomp.SetParameter.MemoryTracingH\x00\x1a\x18\n\x03PSO\x12\x11\n\tthreshold\x18\x01 \x01(\x03\x1a\x1c\n\x08RowLimit\x12\x10\n\x08rowLimit\x18\x01 \x01(\x03\x1a\x1e\n\tTimeLimit\x12\x11\n\ttimeLimit\x18\x01 \x01(\x03\x1a)\n\x10MaxTempDiskLimit\x12\x15\n\rtempDiskLimit\x18\x01 \x01(\x03\x1a\x34\n\x14ResultSetColumnLimit\x12\x1c\n\x14resultSetColumnLimit\x18\x01 \x01(\x03\x1a\x1c\n\x08Priority\x12\x10\n\x08priority\x18\x01 \x01(\x01\x1a\"\n\x0b\x43oncurrency\x12\x13\n\x0b\x63oncurrency\x18\x01 \x01(\x03\x1a\x17\n\x07PSOSeed\x12\x0c\n\x04seed\x18\x01 \x01(\x04\x1a\x1e\n\rForceExternal\x12\r\n\x05is_on\x18\x01 \x01(\x08\x1a\x36\n\x14PriorityAdjustFactor\x12\x1e\n\x16priority_adjust_factor\x18\x01 \x01(\x01\x1a\x32\n\x12PriorityAdjustTime\x12\x1c\n\x14priority_adjust_time\x18\x01 \x01(\r\x1a.\n\x10ServiceClassName\x12\x1a\n\x12service_class_name\x18\x01 \x01(\t\x1a\x1e\n\rMemoryTracing\x12\r\n\x05is_on\x18\x01 \x01(\x08\x42\x0b\n\tParameter*4\n\x0fPerformanceMode\x12\x07\n\x03OFF\x10\x00\x12\x18\n\x14ROOT_OP_INST_DISCARD\x10\x01*/\n\rExplainFormat\x12\t\n\x05PROTO\x10\x00\x12\x08\n\x04JSON\x10\x01\x12\t\n\x05\x44\x45\x42UG\x10\x02*1\n\x0cServerSignal\x12\x0b\n\x07INVALID\x10\x00\x12\x14\n\x07QUIESCE\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x42\x17\n\x15\x63om.ocient.jdbc.protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sharedMessages.clientWireProtocol_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\025com.ocient.jdbc.proto'
   _FETCHMETADATARESPONSE_COLS2POSENTRY._options = None
   _FETCHMETADATARESPONSE_COLS2POSENTRY._serialized_options = b'8\001'
   _FETCHMETADATARESPONSE_COLS2TYPESENTRY._options = None
   _FETCHMETADATARESPONSE_COLS2TYPESENTRY._serialized_options = b'8\001'
-  _BROADCASTQUERYCONCURRENCY_SERVICECLASSIDTOCOUNTSENTRY._options = None
-  _BROADCASTQUERYCONCURRENCY_SERVICECLASSIDTOCOUNTSENTRY._serialized_options = b'8\001'
   _LOCALQUERIES.fields_by_name['identity']._options = None
   _LOCALQUERIES.fields_by_name['identity']._serialized_options = b'\030\001'
   _LOCALQUERIES.fields_by_name['uuid_identity']._options = None
   _LOCALQUERIES.fields_by_name['uuid_identity']._serialized_options = b'\030\001'
   _LOCALQUERIES.fields_by_name['signature']._options = None
   _LOCALQUERIES.fields_by_name['signature']._serialized_options = b'\030\001'
   _LOCALQUERIES.fields_by_name['issuer_certificate']._options = None
@@ -42,252 +41,204 @@
   _LOCALQUERIES.fields_by_name['user']._serialized_options = b'\030\001'
   _REQUEST.fields_by_name['force_external']._options = None
   _REQUEST.fields_by_name['force_external']._serialized_options = b'\030\001'
   _REQUEST.fields_by_name['check_data']._options = None
   _REQUEST.fields_by_name['check_data']._serialized_options = b'\030\001'
   _FORCEEXTERNAL._options = None
   _FORCEEXTERNAL._serialized_options = b'\030\001'
-  _LOCALCANCELQUERY.fields_by_name['identity']._options = None
-  _LOCALCANCELQUERY.fields_by_name['identity']._serialized_options = b'\030\001'
-  _LOCALCANCELQUERY.fields_by_name['uuid_identity']._options = None
-  _LOCALCANCELQUERY.fields_by_name['uuid_identity']._serialized_options = b'\030\001'
-  _LOCALCANCELQUERY.fields_by_name['user']._options = None
-  _LOCALCANCELQUERY.fields_by_name['user']._serialized_options = b'\030\001'
-  _LOCALCANCELQUERY.fields_by_name['signature']._options = None
-  _LOCALCANCELQUERY.fields_by_name['signature']._serialized_options = b'\030\001'
-  _LOCALCANCELQUERY.fields_by_name['issuer_certificate']._options = None
-  _LOCALCANCELQUERY.fields_by_name['issuer_certificate']._serialized_options = b'\030\001'
-  _LOCALKILLQUERY.fields_by_name['identity']._options = None
-  _LOCALKILLQUERY.fields_by_name['identity']._serialized_options = b'\030\001'
-  _LOCALKILLQUERY.fields_by_name['uuid_identity']._options = None
-  _LOCALKILLQUERY.fields_by_name['uuid_identity']._serialized_options = b'\030\001'
-  _LOCALKILLQUERY.fields_by_name['user']._options = None
-  _LOCALKILLQUERY.fields_by_name['user']._serialized_options = b'\030\001'
-  _LOCALKILLQUERY.fields_by_name['signature']._options = None
-  _LOCALKILLQUERY.fields_by_name['signature']._serialized_options = b'\030\001'
-  _LOCALKILLQUERY.fields_by_name['issuer_certificate']._options = None
-  _LOCALKILLQUERY.fields_by_name['issuer_certificate']._serialized_options = b'\030\001'
-  _globals['_PERFORMANCEMODE']._serialized_start=16641
-  _globals['_PERFORMANCEMODE']._serialized_end=16693
-  _globals['_EXPLAINFORMAT']._serialized_start=16695
-  _globals['_EXPLAINFORMAT']._serialized_end=16742
+  _globals['_PERFORMANCEMODE']._serialized_start=14372
+  _globals['_PERFORMANCEMODE']._serialized_end=14424
+  _globals['_EXPLAINFORMAT']._serialized_start=14426
+  _globals['_EXPLAINFORMAT']._serialized_end=14473
+  _globals['_SERVERSIGNAL']._serialized_start=14475
+  _globals['_SERVERSIGNAL']._serialized_end=14524
   _globals['_CLIENTCONNECTION']._serialized_start=88
-  _globals['_CLIENTCONNECTION']._serialized_end=250
-  _globals['_CLIENTCONNECTIONGCM']._serialized_start=253
-  _globals['_CLIENTCONNECTIONGCM']._serialized_end=439
-  _globals['_CLIENTCONNECTIONSSO']._serialized_start=442
-  _globals['_CLIENTCONNECTIONSSO']._serialized_end=591
-  _globals['_CLIENTCONNECTIONSECURITYTOKEN']._serialized_start=594
-  _globals['_CLIENTCONNECTIONSECURITYTOKEN']._serialized_end=842
-  _globals['_CLIENTCONNECTIONRESPONSE']._serialized_start=844
-  _globals['_CLIENTCONNECTIONRESPONSE']._serialized_end=950
-  _globals['_CLIENTCONNECTIONGCMRESPONSE']._serialized_start=952
-  _globals['_CLIENTCONNECTIONGCMRESPONSE']._serialized_end=1061
-  _globals['_CLIENTCONNECTIONSSORESPONSE']._serialized_start=1063
-  _globals['_CLIENTCONNECTIONSSORESPONSE']._serialized_end=1180
-  _globals['_CLIENTCONNECTIONSECURITYTOKENRESPONSE']._serialized_start=1183
-  _globals['_CLIENTCONNECTIONSECURITYTOKENRESPONSE']._serialized_end=1434
-  _globals['_CLIENTCONNECTION2']._serialized_start=1436
-  _globals['_CLIENTCONNECTION2']._serialized_end=1516
-  _globals['_CLIENTCONNECTIONGCM2']._serialized_start=1518
-  _globals['_CLIENTCONNECTIONGCM2']._serialized_end=1622
-  _globals['_CLIENTCONNECTIONSSO2']._serialized_start=1624
-  _globals['_CLIENTCONNECTIONSSO2']._serialized_end=1680
-  _globals['_SECURITYTOKEN']._serialized_start=1682
-  _globals['_SECURITYTOKEN']._serialized_end=1757
-  _globals['_SESSIONINFO']._serialized_start=1759
-  _globals['_SESSIONINFO']._serialized_end=1847
-  _globals['_CLIENTCONNECTIONREFRESHSESSION']._serialized_start=1849
-  _globals['_CLIENTCONNECTIONREFRESHSESSION']._serialized_end=1881
-  _globals['_CLIENTCONNECTIONREFRESHSESSIONRESPONSE']._serialized_start=1884
-  _globals['_CLIENTCONNECTIONREFRESHSESSIONRESPONSE']._serialized_end=2022
-  _globals['_CLIENTCONNECTIONREFRESHTOKEN']._serialized_start=2024
-  _globals['_CLIENTCONNECTIONREFRESHTOKEN']._serialized_end=2107
-  _globals['_CLIENTCONNECTIONREFRESHTOKENRESPONSE']._serialized_start=2110
-  _globals['_CLIENTCONNECTIONREFRESHTOKENRESPONSE']._serialized_end=2253
-  _globals['_SECONDARYINTERFACELIST']._serialized_start=2255
-  _globals['_SECONDARYINTERFACELIST']._serialized_end=2296
-  _globals['_CLIENTCONNECTION2RESPONSE']._serialized_start=2299
-  _globals['_CLIENTCONNECTION2RESPONSE']._serialized_end=2588
-  _globals['_CLIENTCONNECTIONGCM2RESPONSE']._serialized_start=2591
-  _globals['_CLIENTCONNECTIONGCM2RESPONSE']._serialized_end=2883
-  _globals['_CLIENTCONNECTIONSSO2RESPONSE']._serialized_start=2886
-  _globals['_CLIENTCONNECTIONSSO2RESPONSE']._serialized_end=3203
-  _globals['_OPENIDAUTHENTICATOR']._serialized_start=3205
-  _globals['_OPENIDAUTHENTICATOR']._serialized_end=3275
-  _globals['_AUTHENTICATOR']._serialized_start=3277
-  _globals['_AUTHENTICATOR']._serialized_end=3374
-  _globals['_FETCHAUTHENTICATORS']._serialized_start=3376
-  _globals['_FETCHAUTHENTICATORS']._serialized_end=3415
-  _globals['_FETCHAUTHENTICATORSRESPONSE']._serialized_start=3418
-  _globals['_FETCHAUTHENTICATORSRESPONSE']._serialized_end=3549
-  _globals['_GETSCHEMA']._serialized_start=3551
-  _globals['_GETSCHEMA']._serialized_end=3562
-  _globals['_GETSCHEMARESPONSE']._serialized_start=3564
-  _globals['_GETSCHEMARESPONSE']._serialized_end=3651
-  _globals['_SETSCHEMA']._serialized_start=3653
-  _globals['_SETSCHEMA']._serialized_end=3680
-  _globals['_CLOSECONNECTION']._serialized_start=3682
-  _globals['_CLOSECONNECTION']._serialized_end=3719
-  _globals['_TESTCONNECTION']._serialized_start=3721
-  _globals['_TESTCONNECTION']._serialized_end=3737
-  _globals['_ATTACHTOQUERY']._serialized_start=3739
-  _globals['_ATTACHTOQUERY']._serialized_end=3771
-  _globals['_FETCHDATA']._serialized_start=3773
-  _globals['_FETCHDATA']._serialized_end=3804
-  _globals['_RESULTSET']._serialized_start=3806
-  _globals['_RESULTSET']._serialized_end=3871
-  _globals['_FETCHDATARESPONSE']._serialized_start=3873
-  _globals['_FETCHDATARESPONSE']._serialized_end=3987
-  _globals['_FETCHMETADATA']._serialized_start=3989
-  _globals['_FETCHMETADATA']._serialized_end=4004
-  _globals['_FETCHMETADATARESPONSE']._serialized_start=4007
-  _globals['_FETCHMETADATARESPONSE']._serialized_end=4320
-  _globals['_FETCHMETADATARESPONSE_COLS2POSENTRY']._serialized_start=4222
-  _globals['_FETCHMETADATARESPONSE_COLS2POSENTRY']._serialized_end=4269
-  _globals['_FETCHMETADATARESPONSE_COLS2TYPESENTRY']._serialized_start=4271
-  _globals['_FETCHMETADATARESPONSE_COLS2TYPESENTRY']._serialized_end=4320
-  _globals['_FETCHSYSTEMMETADATA']._serialized_start=4323
-  _globals['_FETCHSYSTEMMETADATA']._serialized_end=4929
-  _globals['_FETCHSYSTEMMETADATA_SYSTEMMETADATACALL']._serialized_start=4488
-  _globals['_FETCHSYSTEMMETADATA_SYSTEMMETADATACALL']._serialized_end=4929
-  _globals['_FETCHSYSTEMMETADATARESPONSE']._serialized_start=4932
-  _globals['_FETCHSYSTEMMETADATARESPONSE']._serialized_end=5119
-  _globals['_CLOSERESULTSET']._serialized_start=5121
-  _globals['_CLOSERESULTSET']._serialized_end=5137
-  _globals['_EXECUTEQUERY']._serialized_start=5139
-  _globals['_EXECUTEQUERY']._serialized_end=5258
-  _globals['_EXECUTEQUERYRESPONSE']._serialized_start=5261
-  _globals['_EXECUTEQUERYRESPONSE']._serialized_end=5440
-  _globals['_EXECUTEUPDATE']._serialized_start=5442
-  _globals['_EXECUTEUPDATE']._serialized_end=5485
-  _globals['_EXECUTEUPDATERESPONSE']._serialized_start=5488
-  _globals['_EXECUTEUPDATERESPONSE']._serialized_end=5649
-  _globals['_EXECUTEEXPLAIN']._serialized_start=5651
-  _globals['_EXECUTEEXPLAIN']._serialized_end=5738
-  _globals['_EXECUTEEXPLAINFORSPARK']._serialized_start=5741
-  _globals['_EXECUTEEXPLAINFORSPARK']._serialized_end=5961
-  _globals['_EXECUTEEXPLAINFORSPARK_PARTITIONINGTYPE']._serialized_start=5889
-  _globals['_EXECUTEEXPLAINFORSPARK_PARTITIONINGTYPE']._serialized_end=5961
-  _globals['_EXPLAINRESPONSESTRINGPLAN']._serialized_start=5964
-  _globals['_EXPLAINRESPONSESTRINGPLAN']._serialized_end=6119
-  _globals['_BEGINQUERYCONCURRENCY']._serialized_start=6121
-  _globals['_BEGINQUERYCONCURRENCY']._serialized_end=6207
-  _globals['_FINISHQUERYCONCURRENCY']._serialized_start=6209
-  _globals['_FINISHQUERYCONCURRENCY']._serialized_end=6296
-  _globals['_BROADCASTQUERYCONCURRENCY']._serialized_start=6299
-  _globals['_BROADCASTQUERYCONCURRENCY']._serialized_end=6510
-  _globals['_BROADCASTQUERYCONCURRENCY_SERVICECLASSIDTOCOUNTSENTRY']._serialized_start=6449
-  _globals['_BROADCASTQUERYCONCURRENCY_SERVICECLASSIDTOCOUNTSENTRY']._serialized_end=6510
-  _globals['_QUERYCONCURRENCYRESPONSE']._serialized_start=6512
-  _globals['_QUERYCONCURRENCYRESPONSE']._serialized_end=6590
-  _globals['_SYSTEMWIDEQUERIES']._serialized_start=6592
-  _globals['_SYSTEMWIDEQUERIES']._serialized_end=6611
-  _globals['_SYSTEMWIDEQUERIESRESPONSE']._serialized_start=6613
-  _globals['_SYSTEMWIDEQUERIESRESPONSE']._serialized_end=6733
-  _globals['_LOCALQUERIES']._serialized_start=6736
-  _globals['_LOCALQUERIES']._serialized_end=6999
-  _globals['_LOCALQUERIESRESPONSE']._serialized_start=7001
-  _globals['_LOCALQUERIESRESPONSE']._serialized_end=7116
-  _globals['_SYSQUERIESROW']._serialized_start=7119
-  _globals['_SYSQUERIESROW']._serialized_end=7590
-  _globals['_SYSTEMWIDECOMPLETEDQUERIES']._serialized_start=7592
-  _globals['_SYSTEMWIDECOMPLETEDQUERIES']._serialized_end=7620
-  _globals['_COMPLETEDQUERIESRESPONSE']._serialized_start=7622
-  _globals['_COMPLETEDQUERIESRESPONSE']._serialized_end=7747
-  _globals['_COMPLETEDQUERIESROW']._serialized_start=7750
-  _globals['_COMPLETEDQUERIESROW']._serialized_end=8454
-  _globals['_LOADBROADCAST']._serialized_start=8456
-  _globals['_LOADBROADCAST']._serialized_end=8504
-  _globals['_CACHETABLEREFERENCE']._serialized_start=8506
-  _globals['_CACHETABLEREFERENCE']._serialized_end=8557
-  _globals['_CACHEENTRY']._serialized_start=8560
-  _globals['_CACHEENTRY']._serialized_end=8829
-  _globals['_CACHEENTRY_ACTION']._serialized_start=8787
-  _globals['_CACHEENTRY_ACTION']._serialized_end=8829
-  _globals['_UPDATECACHE']._serialized_start=8831
-  _globals['_UPDATECACHE']._serialized_end=8919
-  _globals['_CLEARCACHE']._serialized_start=8921
-  _globals['_CLEARCACHE']._serialized_end=8966
-  _globals['_REQUEST']._serialized_start=8969
-  _globals['_REQUEST']._serialized_end=12946
-  _globals['_REQUEST_REQUESTTYPE']._serialized_start=11814
-  _globals['_REQUEST_REQUESTTYPE']._serialized_end=12929
-  _globals['_CONFIRMATIONRESPONSE']._serialized_start=12949
-  _globals['_CONFIRMATIONRESPONSE']._serialized_end=13173
-  _globals['_CONFIRMATIONRESPONSE_RESPONSETYPE']._serialized_start=13090
-  _globals['_CONFIRMATIONRESPONSE_RESPONSETYPE']._serialized_end=13173
-  _globals['_EXECUTEPLAN']._serialized_start=13175
-  _globals['_EXECUTEPLAN']._serialized_end=13216
-  _globals['_EXECUTEINLINEPLAN']._serialized_start=13218
-  _globals['_EXECUTEINLINEPLAN']._serialized_end=13265
-  _globals['_EXPLAINPLAN']._serialized_start=13267
-  _globals['_EXPLAINPLAN']._serialized_end=13351
-  _globals['_FORCEEXTERNAL']._serialized_start=13353
-  _globals['_FORCEEXTERNAL']._serialized_end=13387
-  _globals['_LISTPLAN']._serialized_start=13389
-  _globals['_LISTPLAN']._serialized_end=13399
-  _globals['_LISTPLANRESPONSE']._serialized_start=13402
-  _globals['_LISTPLANRESPONSE']._serialized_end=13552
-  _globals['_CANCELQUERY']._serialized_start=13554
-  _globals['_CANCELQUERY']._serialized_end=13580
-  _globals['_CANCELQUERYRESPONSE']._serialized_start=13582
-  _globals['_CANCELQUERYRESPONSE']._serialized_end=13655
-  _globals['_LOCALCANCELQUERY']._serialized_start=13658
-  _globals['_LOCALCANCELQUERY']._serialized_end=13879
-  _globals['_LOCALCANCELQUERYRESPONSE']._serialized_start=13881
-  _globals['_LOCALCANCELQUERYRESPONSE']._serialized_end=13959
-  _globals['_KILLQUERY']._serialized_start=13961
-  _globals['_KILLQUERY']._serialized_end=13985
-  _globals['_KILLQUERYRESPONSE']._serialized_start=13987
-  _globals['_KILLQUERYRESPONSE']._serialized_end=14058
-  _globals['_LOCALKILLQUERY']._serialized_start=14061
-  _globals['_LOCALKILLQUERY']._serialized_end=14280
-  _globals['_LOCALKILLQUERYRESPONSE']._serialized_start=14282
-  _globals['_LOCALKILLQUERYRESPONSE']._serialized_end=14358
-  _globals['_LOCALINVALIDATESTATS']._serialized_start=14360
-  _globals['_LOCALINVALIDATESTATS']._serialized_end=14471
-  _globals['_LOCALINVALIDATESTATSRESPONSE']._serialized_start=14473
-  _globals['_LOCALINVALIDATESTATSRESPONSE']._serialized_end=14555
-  _globals['_EXECUTEEXPORT']._serialized_start=14557
-  _globals['_EXECUTEEXPORT']._serialized_end=14600
-  _globals['_EXECUTEEXPORTRESPONSE']._serialized_start=14603
-  _globals['_EXECUTEEXPORTRESPONSE']._serialized_end=14765
-  _globals['_EXPLAINPIPELINEREQUEST']._serialized_start=14767
-  _globals['_EXPLAINPIPELINEREQUEST']._serialized_end=14819
-  _globals['_EXPLAINPIPELINERESPONSE']._serialized_start=14822
-  _globals['_EXPLAINPIPELINERESPONSE']._serialized_end=14988
-  _globals['_CHECKDATAREQUEST']._serialized_start=14990
-  _globals['_CHECKDATAREQUEST']._serialized_end=15036
-  _globals['_CHECKDATARESPONSE']._serialized_start=15039
-  _globals['_CHECKDATARESPONSE']._serialized_end=15200
-  _globals['_SETPSO']._serialized_start=15202
-  _globals['_SETPSO']._serialized_end=15244
-  _globals['_SETPARAMETER']._serialized_start=15247
-  _globals['_SETPARAMETER']._serialized_end=16639
-  _globals['_SETPARAMETER_PSO']._serialized_start=16132
-  _globals['_SETPARAMETER_PSO']._serialized_end=16156
-  _globals['_SETPARAMETER_ROWLIMIT']._serialized_start=16158
-  _globals['_SETPARAMETER_ROWLIMIT']._serialized_end=16186
-  _globals['_SETPARAMETER_TIMELIMIT']._serialized_start=16188
-  _globals['_SETPARAMETER_TIMELIMIT']._serialized_end=16218
-  _globals['_SETPARAMETER_MAXTEMPDISKLIMIT']._serialized_start=16220
-  _globals['_SETPARAMETER_MAXTEMPDISKLIMIT']._serialized_end=16261
-  _globals['_SETPARAMETER_RESULTSETCOLUMNLIMIT']._serialized_start=16263
-  _globals['_SETPARAMETER_RESULTSETCOLUMNLIMIT']._serialized_end=16315
-  _globals['_SETPARAMETER_PRIORITY']._serialized_start=16317
-  _globals['_SETPARAMETER_PRIORITY']._serialized_end=16345
-  _globals['_SETPARAMETER_CONCURRENCY']._serialized_start=16347
-  _globals['_SETPARAMETER_CONCURRENCY']._serialized_end=16381
-  _globals['_SETPARAMETER_PSOSEED']._serialized_start=16383
-  _globals['_SETPARAMETER_PSOSEED']._serialized_end=16406
-  _globals['_SETPARAMETER_FORCEEXTERNAL']._serialized_start=16408
-  _globals['_SETPARAMETER_FORCEEXTERNAL']._serialized_end=16438
-  _globals['_SETPARAMETER_PRIORITYADJUSTFACTOR']._serialized_start=16440
-  _globals['_SETPARAMETER_PRIORITYADJUSTFACTOR']._serialized_end=16494
-  _globals['_SETPARAMETER_PRIORITYADJUSTTIME']._serialized_start=16496
-  _globals['_SETPARAMETER_PRIORITYADJUSTTIME']._serialized_end=16546
-  _globals['_SETPARAMETER_SERVICECLASSNAME']._serialized_start=16548
-  _globals['_SETPARAMETER_SERVICECLASSNAME']._serialized_end=16594
-  _globals['_SETPARAMETER_MEMORYTRACING']._serialized_start=16596
-  _globals['_SETPARAMETER_MEMORYTRACING']._serialized_end=16626
+  _globals['_CLIENTCONNECTION']._serialized_end=278
+  _globals['_CLIENTCONNECTIONGCM']._serialized_start=281
+  _globals['_CLIENTCONNECTIONGCM']._serialized_end=495
+  _globals['_CLIENTCONNECTIONSSO']._serialized_start=498
+  _globals['_CLIENTCONNECTIONSSO']._serialized_end=675
+  _globals['_CLIENTCONNECTIONSECURITYTOKEN']._serialized_start=678
+  _globals['_CLIENTCONNECTIONSECURITYTOKEN']._serialized_end=954
+  _globals['_CLIENTCONNECTIONRESPONSE']._serialized_start=956
+  _globals['_CLIENTCONNECTIONRESPONSE']._serialized_end=1062
+  _globals['_CLIENTCONNECTIONGCMRESPONSE']._serialized_start=1064
+  _globals['_CLIENTCONNECTIONGCMRESPONSE']._serialized_end=1173
+  _globals['_CLIENTCONNECTIONSSORESPONSE']._serialized_start=1175
+  _globals['_CLIENTCONNECTIONSSORESPONSE']._serialized_end=1292
+  _globals['_CLIENTCONNECTIONSECURITYTOKENRESPONSE']._serialized_start=1295
+  _globals['_CLIENTCONNECTIONSECURITYTOKENRESPONSE']._serialized_end=1546
+  _globals['_CLIENTCONNECTION2']._serialized_start=1548
+  _globals['_CLIENTCONNECTION2']._serialized_end=1628
+  _globals['_CLIENTCONNECTIONGCM2']._serialized_start=1630
+  _globals['_CLIENTCONNECTIONGCM2']._serialized_end=1734
+  _globals['_CLIENTCONNECTIONSSO2']._serialized_start=1736
+  _globals['_CLIENTCONNECTIONSSO2']._serialized_end=1792
+  _globals['_SECURITYTOKEN']._serialized_start=1794
+  _globals['_SECURITYTOKEN']._serialized_end=1869
+  _globals['_SESSIONINFO']._serialized_start=1871
+  _globals['_SESSIONINFO']._serialized_end=1959
+  _globals['_CLIENTCONNECTIONREFRESHSESSION']._serialized_start=1961
+  _globals['_CLIENTCONNECTIONREFRESHSESSION']._serialized_end=1993
+  _globals['_CLIENTCONNECTIONREFRESHSESSIONRESPONSE']._serialized_start=1996
+  _globals['_CLIENTCONNECTIONREFRESHSESSIONRESPONSE']._serialized_end=2134
+  _globals['_CLIENTCONNECTIONREFRESHTOKEN']._serialized_start=2136
+  _globals['_CLIENTCONNECTIONREFRESHTOKEN']._serialized_end=2219
+  _globals['_CLIENTCONNECTIONREFRESHTOKENRESPONSE']._serialized_start=2222
+  _globals['_CLIENTCONNECTIONREFRESHTOKENRESPONSE']._serialized_end=2365
+  _globals['_SECONDARYINTERFACELIST']._serialized_start=2367
+  _globals['_SECONDARYINTERFACELIST']._serialized_end=2408
+  _globals['_CLIENTCONNECTION2RESPONSE']._serialized_start=2411
+  _globals['_CLIENTCONNECTION2RESPONSE']._serialized_end=2700
+  _globals['_CLIENTCONNECTIONGCM2RESPONSE']._serialized_start=2703
+  _globals['_CLIENTCONNECTIONGCM2RESPONSE']._serialized_end=2995
+  _globals['_CLIENTCONNECTIONSSO2RESPONSE']._serialized_start=2998
+  _globals['_CLIENTCONNECTIONSSO2RESPONSE']._serialized_end=3315
+  _globals['_OPENIDAUTHENTICATOR']._serialized_start=3317
+  _globals['_OPENIDAUTHENTICATOR']._serialized_end=3387
+  _globals['_AUTHENTICATOR']._serialized_start=3389
+  _globals['_AUTHENTICATOR']._serialized_end=3486
+  _globals['_FETCHAUTHENTICATORS']._serialized_start=3488
+  _globals['_FETCHAUTHENTICATORS']._serialized_end=3527
+  _globals['_FETCHAUTHENTICATORSRESPONSE']._serialized_start=3530
+  _globals['_FETCHAUTHENTICATORSRESPONSE']._serialized_end=3661
+  _globals['_GETSCHEMA']._serialized_start=3663
+  _globals['_GETSCHEMA']._serialized_end=3674
+  _globals['_GETSCHEMARESPONSE']._serialized_start=3676
+  _globals['_GETSCHEMARESPONSE']._serialized_end=3763
+  _globals['_SETSCHEMA']._serialized_start=3765
+  _globals['_SETSCHEMA']._serialized_end=3792
+  _globals['_CLOSECONNECTION']._serialized_start=3794
+  _globals['_CLOSECONNECTION']._serialized_end=3831
+  _globals['_TESTCONNECTION']._serialized_start=3833
+  _globals['_TESTCONNECTION']._serialized_end=3849
+  _globals['_ATTACHTOQUERY']._serialized_start=3851
+  _globals['_ATTACHTOQUERY']._serialized_end=3883
+  _globals['_FETCHDATA']._serialized_start=3885
+  _globals['_FETCHDATA']._serialized_end=3916
+  _globals['_RESULTSET']._serialized_start=3918
+  _globals['_RESULTSET']._serialized_end=3983
+  _globals['_FETCHDATARESPONSE']._serialized_start=3985
+  _globals['_FETCHDATARESPONSE']._serialized_end=4099
+  _globals['_FETCHMETADATA']._serialized_start=4101
+  _globals['_FETCHMETADATA']._serialized_end=4116
+  _globals['_FETCHMETADATARESPONSE']._serialized_start=4119
+  _globals['_FETCHMETADATARESPONSE']._serialized_end=4432
+  _globals['_FETCHMETADATARESPONSE_COLS2POSENTRY']._serialized_start=4334
+  _globals['_FETCHMETADATARESPONSE_COLS2POSENTRY']._serialized_end=4381
+  _globals['_FETCHMETADATARESPONSE_COLS2TYPESENTRY']._serialized_start=4383
+  _globals['_FETCHMETADATARESPONSE_COLS2TYPESENTRY']._serialized_end=4432
+  _globals['_FETCHSYSTEMMETADATA']._serialized_start=4435
+  _globals['_FETCHSYSTEMMETADATA']._serialized_end=5041
+  _globals['_FETCHSYSTEMMETADATA_SYSTEMMETADATACALL']._serialized_start=4600
+  _globals['_FETCHSYSTEMMETADATA_SYSTEMMETADATACALL']._serialized_end=5041
+  _globals['_FETCHSYSTEMMETADATARESPONSE']._serialized_start=5044
+  _globals['_FETCHSYSTEMMETADATARESPONSE']._serialized_end=5231
+  _globals['_CLOSERESULTSET']._serialized_start=5233
+  _globals['_CLOSERESULTSET']._serialized_end=5249
+  _globals['_EXECUTEQUERY']._serialized_start=5251
+  _globals['_EXECUTEQUERY']._serialized_end=5370
+  _globals['_EXECUTEQUERYRESPONSE']._serialized_start=5373
+  _globals['_EXECUTEQUERYRESPONSE']._serialized_end=5552
+  _globals['_EXECUTEUPDATE']._serialized_start=5554
+  _globals['_EXECUTEUPDATE']._serialized_end=5597
+  _globals['_EXECUTEUPDATERESPONSE']._serialized_start=5600
+  _globals['_EXECUTEUPDATERESPONSE']._serialized_end=5761
+  _globals['_EXECUTEEXPLAIN']._serialized_start=5763
+  _globals['_EXECUTEEXPLAIN']._serialized_end=5850
+  _globals['_EXECUTEEXPLAINFORSPARK']._serialized_start=5853
+  _globals['_EXECUTEEXPLAINFORSPARK']._serialized_end=6073
+  _globals['_EXECUTEEXPLAINFORSPARK_PARTITIONINGTYPE']._serialized_start=6001
+  _globals['_EXECUTEEXPLAINFORSPARK_PARTITIONINGTYPE']._serialized_end=6073
+  _globals['_EXPLAINRESPONSESTRINGPLAN']._serialized_start=6076
+  _globals['_EXPLAINRESPONSESTRINGPLAN']._serialized_end=6231
+  _globals['_QUERYCONCURRENCYRESPONSE']._serialized_start=6233
+  _globals['_QUERYCONCURRENCYRESPONSE']._serialized_end=6311
+  _globals['_SYSTEMWIDEQUERIES']._serialized_start=6313
+  _globals['_SYSTEMWIDEQUERIES']._serialized_end=6332
+  _globals['_SYSTEMWIDEQUERIESRESPONSE']._serialized_start=6334
+  _globals['_SYSTEMWIDEQUERIESRESPONSE']._serialized_end=6454
+  _globals['_LOCALQUERIES']._serialized_start=6457
+  _globals['_LOCALQUERIES']._serialized_end=6720
+  _globals['_LOCALQUERIESRESPONSE']._serialized_start=6722
+  _globals['_LOCALQUERIESRESPONSE']._serialized_end=6837
+  _globals['_SYSQUERIESROW']._serialized_start=6840
+  _globals['_SYSQUERIESROW']._serialized_end=7311
+  _globals['_SYSTEMWIDECOMPLETEDQUERIES']._serialized_start=7313
+  _globals['_SYSTEMWIDECOMPLETEDQUERIES']._serialized_end=7341
+  _globals['_COMPLETEDQUERIESRESPONSE']._serialized_start=7343
+  _globals['_COMPLETEDQUERIESRESPONSE']._serialized_end=7468
+  _globals['_COMPLETEDQUERIESROW']._serialized_start=7471
+  _globals['_COMPLETEDQUERIESROW']._serialized_end=8175
+  _globals['_CLEARCACHE']._serialized_start=8177
+  _globals['_CLEARCACHE']._serialized_end=8208
+  _globals['_REQUEST']._serialized_start=8211
+  _globals['_REQUEST']._serialized_end=11478
+  _globals['_REQUEST_REQUESTTYPE']._serialized_start=10550
+  _globals['_REQUEST_REQUESTTYPE']._serialized_end=11461
+  _globals['_CONFIRMATIONRESPONSE']._serialized_start=11481
+  _globals['_CONFIRMATIONRESPONSE']._serialized_end=11705
+  _globals['_CONFIRMATIONRESPONSE_RESPONSETYPE']._serialized_start=11622
+  _globals['_CONFIRMATIONRESPONSE_RESPONSETYPE']._serialized_end=11705
+  _globals['_EXECUTEPLAN']._serialized_start=11707
+  _globals['_EXECUTEPLAN']._serialized_end=11748
+  _globals['_EXECUTEINLINEPLAN']._serialized_start=11750
+  _globals['_EXECUTEINLINEPLAN']._serialized_end=11797
+  _globals['_EXPLAINPLAN']._serialized_start=11799
+  _globals['_EXPLAINPLAN']._serialized_end=11883
+  _globals['_FORCEEXTERNAL']._serialized_start=11885
+  _globals['_FORCEEXTERNAL']._serialized_end=11919
+  _globals['_LISTPLAN']._serialized_start=11921
+  _globals['_LISTPLAN']._serialized_end=11931
+  _globals['_LISTPLANRESPONSE']._serialized_start=11934
+  _globals['_LISTPLANRESPONSE']._serialized_end=12084
+  _globals['_CANCELQUERY']._serialized_start=12086
+  _globals['_CANCELQUERY']._serialized_end=12112
+  _globals['_CANCELQUERYRESPONSE']._serialized_start=12114
+  _globals['_CANCELQUERYRESPONSE']._serialized_end=12187
+  _globals['_KILLQUERY']._serialized_start=12189
+  _globals['_KILLQUERY']._serialized_end=12213
+  _globals['_KILLQUERYRESPONSE']._serialized_start=12215
+  _globals['_KILLQUERYRESPONSE']._serialized_end=12286
+  _globals['_EXECUTEEXPORT']._serialized_start=12288
+  _globals['_EXECUTEEXPORT']._serialized_end=12331
+  _globals['_EXECUTEEXPORTRESPONSE']._serialized_start=12334
+  _globals['_EXECUTEEXPORTRESPONSE']._serialized_end=12496
+  _globals['_EXPLAINPIPELINEREQUEST']._serialized_start=12498
+  _globals['_EXPLAINPIPELINEREQUEST']._serialized_end=12550
+  _globals['_EXPLAINPIPELINERESPONSE']._serialized_start=12553
+  _globals['_EXPLAINPIPELINERESPONSE']._serialized_end=12719
+  _globals['_CHECKDATAREQUEST']._serialized_start=12721
+  _globals['_CHECKDATAREQUEST']._serialized_end=12767
+  _globals['_CHECKDATARESPONSE']._serialized_start=12770
+  _globals['_CHECKDATARESPONSE']._serialized_end=12931
+  _globals['_SETPSO']._serialized_start=12933
+  _globals['_SETPSO']._serialized_end=12975
+  _globals['_SETPARAMETER']._serialized_start=12978
+  _globals['_SETPARAMETER']._serialized_end=14370
+  _globals['_SETPARAMETER_PSO']._serialized_start=13863
+  _globals['_SETPARAMETER_PSO']._serialized_end=13887
+  _globals['_SETPARAMETER_ROWLIMIT']._serialized_start=13889
+  _globals['_SETPARAMETER_ROWLIMIT']._serialized_end=13917
+  _globals['_SETPARAMETER_TIMELIMIT']._serialized_start=13919
+  _globals['_SETPARAMETER_TIMELIMIT']._serialized_end=13949
+  _globals['_SETPARAMETER_MAXTEMPDISKLIMIT']._serialized_start=13951
+  _globals['_SETPARAMETER_MAXTEMPDISKLIMIT']._serialized_end=13992
+  _globals['_SETPARAMETER_RESULTSETCOLUMNLIMIT']._serialized_start=13994
+  _globals['_SETPARAMETER_RESULTSETCOLUMNLIMIT']._serialized_end=14046
+  _globals['_SETPARAMETER_PRIORITY']._serialized_start=14048
+  _globals['_SETPARAMETER_PRIORITY']._serialized_end=14076
+  _globals['_SETPARAMETER_CONCURRENCY']._serialized_start=14078
+  _globals['_SETPARAMETER_CONCURRENCY']._serialized_end=14112
+  _globals['_SETPARAMETER_PSOSEED']._serialized_start=14114
+  _globals['_SETPARAMETER_PSOSEED']._serialized_end=14137
+  _globals['_SETPARAMETER_FORCEEXTERNAL']._serialized_start=14139
+  _globals['_SETPARAMETER_FORCEEXTERNAL']._serialized_end=14169
+  _globals['_SETPARAMETER_PRIORITYADJUSTFACTOR']._serialized_start=14171
+  _globals['_SETPARAMETER_PRIORITYADJUSTFACTOR']._serialized_end=14225
+  _globals['_SETPARAMETER_PRIORITYADJUSTTIME']._serialized_start=14227
+  _globals['_SETPARAMETER_PRIORITYADJUSTTIME']._serialized_end=14277
+  _globals['_SETPARAMETER_SERVICECLASSNAME']._serialized_start=14279
+  _globals['_SETPARAMETER_SERVICECLASSNAME']._serialized_end=14325
+  _globals['_SETPARAMETER_MEMORYTRACING']._serialized_start=14327
+  _globals['_SETPARAMETER_MEMORYTRACING']._serialized_end=14357
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyocient-2.0.0/pyocient/__init__.py` & `pyocient-3.0.3/pyocient/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,22 +52,25 @@
     IntegrityError,
     InterfaceError,
     InternalError,
     MalformedURL,
     NotSupportedError,
     OperationalError,
     ProgrammingError,
+    SecurityToken,
     SQLException,
     Time,
     TimeFromTicks,
     Timestamp,
     TimestampFromTicks,
+    TypeCodes,
     Warning,
     apilevel,
     connect,
+    custom_type_to_json,
     paramstyle,
     threadsafety,
 )
 from pyocient.pkg_version import __version__
 
 __version_info__ = tuple(int(v) for v in __version__.split("."))
 
@@ -88,18 +91,21 @@
     "IntegrityError",
     "InterfaceError",
     "InternalError",
     "MalformedURL",
     "NotSupportedError",
     "OperationalError",
     "ProgrammingError",
+    "SecurityToken",
     "SQLException",
     "Time",
     "TimeFromTicks",
     "Timestamp",
     "TimestampFromTicks",
+    "TypeCodes",
     "Warning",
     "apilevel",
     "connect",
+    "custom_type_to_json",
     "paramstyle",
     "threadsafety",
 ]
```

### Comparing `pyocient-2.0.0/pyocient/api.py` & `pyocient-3.0.3/pyocient/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 #!/usr/bin/env python3
 
+# Lots of names/attributes in message definitions are not visible to mypy. This
+# is a catch-all that makes mypy not complain about the usage of names or
+# attributes that do not seem to be defined. Unfortunately, I have not found a
+# comment syntax that scopes this specifically to the "proto" import(s).
+# mypy: disable-error-code="attr-defined,name-defined"
+
+
+from __future__ import annotations
+
 import configparser
 import datetime
 import decimal
 import ipaddress
+import json
 import logging
 import re
 import socket
 import ssl
 import struct
-
-# pylint: disable=too-many-lines
 import sys
 import uuid
 from collections import namedtuple
+from dataclasses import dataclass
+from enum import IntEnum
 from math import isinf
 from time import sleep, time_ns
 from types import TracebackType
 from typing import (
     Any,
     Callable,
+    Dict,
     Generic,
     Iterable,
     List,
     Mapping,
+    MutableMapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 from warnings import warn
 
-import dsnparse  # type: ignore
+import dsnparse  # type: ignore[import]
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, hmac, padding, serialization
 from cryptography.hazmat.primitives.asymmetric.dh import DHPublicKey
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.serialization import load_pem_public_key
 from google.protobuf.internal.containers import RepeatedCompositeFieldContainer
 from google.protobuf.message import Message
@@ -58,31 +70,31 @@
 DRIVER_ID = "pyocient"
 PROTOCOL_VERSION = "7.0.1"
 SESSION_EXPIRED_CODE = -733
 
 parts = version.split(".")
 version_major = int(parts[0])
 version_minor = int(parts[1])
+version_patch = parts[2]
 
 
+@dataclass
 class SQLException(Exception):
     """Base exception for all Ocient exceptions.
 
     Attributes:
 
     - sql_state: The SQLSTATE defined in the SQL standard
     - reason: A string description of the exception
     - vendor_code: An Ocient specific error code
     """
 
-    def __init__(self, reason: str = "", sql_state: str = "00000", vendor_code: int = 0) -> None:
-        super().__init__()
-        self.sql_state = sql_state
-        self.reason = reason
-        self.vendor_code = vendor_code
+    reason: str = "The operation completed successfully"
+    sql_state: str = "00000"
+    vendor_code: int = 0
 
     def __str__(self) -> str:
         return f"State: {self.sql_state} Code: {self.vendor_code} Reason: {self.reason}"
 
 
 #########################################################################
 # Database API 2.0 exceptions.  These are required by PEM 249
@@ -151,19 +163,17 @@
 class MalformedURL(DatabaseError):
     """Exception raised in case a malformed DSN is received"""
 
     def __init__(self, reason: str) -> None:
         super().__init__(sql_state="08001", vendor_code=-200, reason=reason)
 
 
-class TypeCodes:  # pylint: disable=too-few-public-methods
+class TypeCodes(IntEnum):
     """
     Database column type codes
-
-    :meta private:
     """
 
     DEM = 0
     INT = 1
     LONG = 2
     FLOAT = 3
     DOUBLE = 4
@@ -186,24 +196,15 @@
     TIMESTAMP_NANOS = 20
     TIME_NANOS = 21
     TUPLE = 22
     ST_LINESTRING = 23
     ST_POLYGON = 24
 
     @classmethod
-    def to_type(cls, typestr: str) -> int:
-        """Given a string type, return its type code"""
-        if hasattr(cls, typestr):
-            attr = getattr(cls, typestr)
-            if isinstance(attr, int):
-                return attr
-        raise Error(f"Unknown column type {typestr}")
-
-    @classmethod
-    def cls_to_type(cls, pclass: object) -> int:
+    def cls_to_type(cls, pclass: object) -> TypeCodes:
         if pclass == str:
             return cls.STRING
         elif pclass == int:
             return cls.INT
         elif pclass == float:
             return cls.FLOAT
         elif pclass == uuid.UUID:
@@ -221,98 +222,98 @@
 _unpack_float = struct.Struct("!f").unpack_from
 _unpack_double = struct.Struct("!d").unpack_from
 _unpack_bool = struct.Struct("?").unpack_from
 _unpack_char = struct.Struct("c").unpack_from
 
 # easy conversions we can do with structs
 _type_map = {
-    TypeCodes.INT: (struct.calcsize("!i"), _unpack_int),
-    TypeCodes.LONG: (struct.calcsize("!q"), _unpack_long),
-    TypeCodes.FLOAT: (struct.calcsize("!f"), _unpack_float),
-    TypeCodes.DOUBLE: (struct.calcsize("!d"), _unpack_double),
-    TypeCodes.BOOLEAN: (struct.calcsize("?"), _unpack_bool),
-    TypeCodes.SHORT: (struct.calcsize("!h"), _unpack_short),
+    TypeCodes.INT.value: (struct.calcsize("!i"), _unpack_int),
+    TypeCodes.LONG.value: (struct.calcsize("!q"), _unpack_long),
+    TypeCodes.FLOAT.value: (struct.calcsize("!f"), _unpack_float),
+    TypeCodes.DOUBLE.value: (struct.calcsize("!d"), _unpack_double),
+    TypeCodes.BOOLEAN.value: (struct.calcsize("?"), _unpack_bool),
+    TypeCodes.SHORT.value: (struct.calcsize("!h"), _unpack_short),
 }
 
 
 #########################################################################
 # Database API 2.0 types.  These are required by PEM 249
 #########################################################################
 Binary = bytes  # : :meta private:
-STRING = TypeCodes.STRING  # : :meta private:
-BINARY = TypeCodes.BINARY  # : :meta private:
-NUMBER = TypeCodes.INT  # : :meta private:
-DATETIME = TypeCodes.TIMESTAMP  # : :meta private:
-ROWID = TypeCodes.INT  # : :meta private:
+STRING = TypeCodes.STRING.value  # : :meta private:
+BINARY = TypeCodes.BINARY.value  # : :meta private:
+NUMBER = TypeCodes.INT.value  # : :meta private:
+DATETIME = TypeCodes.TIMESTAMP.value  # : :meta private:
+ROWID = TypeCodes.INT.value  # : :meta private:
 
 #########################################################################
 # Import our google protobuf message definitions
 #########################################################################
 try:
     from sharedMessages import clientWireProtocol_pb2 as proto
 except ImportError:
-    import pyocient.ClientWireProtocol_pb2 as proto
+    import pyocient.ClientWireProtocol_pb2 as proto  # type: ignore[import,no-redef]
 
 #########################################################################
 # Lightweight GIS classes
 #########################################################################
 
 
-class _STPoint:
+class STPoint:
     def __init__(self, long: float, lat: float) -> None:
         self.long = long
         self.lat = lat
 
     def wkt_inner(self) -> str:
         return str(self.long) + " " + str(self.lat)
 
     def __repr__(self) -> str:
         if isinf(self.long) or isinf(self.lat):
             return "POINT EMPTY"
         return "POINT(" + self.wkt_inner() + ")"
 
     def __eq__(self, other: object) -> bool:
-        if isinstance(other, _STPoint):
+        if isinstance(other, STPoint):
             return self.long == other.long and self.lat == other.lat
         return NotImplemented
 
 
-def _linestring_wkt_inner(points: List[_STPoint]) -> str:
+def _linestring_wkt_inner(points: List[STPoint]) -> str:
     return "(" + ", ".join((p.wkt_inner() for p in points)) + ")"
 
 
-class _STLinestring:
-    def __init__(self, points: List[_STPoint]) -> None:
+class STLinestring:
+    def __init__(self, points: List[STPoint]) -> None:
         self.points = points
 
     def __repr__(self) -> str:
         if not self.points:
             return "LINESTRING EMPTY"
         return "LINESTRING" + _linestring_wkt_inner(self.points)
 
     def __eq__(self, other: object) -> bool:
         # strict equality, not semantic
-        if isinstance(other, _STLinestring):
+        if isinstance(other, STLinestring):
             return self.points == other.points
         return NotImplemented
 
 
-class _STPolygon:
-    def __init__(self, exterior: List[_STPoint], holes: List[List[_STPoint]]) -> None:
+class STPolygon:
+    def __init__(self, exterior: List[STPoint], holes: List[List[STPoint]]) -> None:
         self.exterior = exterior
         self.holes = holes
 
     def __repr__(self) -> str:
         if not self.exterior:
             return "POLYGON EMPTY"
         return "POLYGON(" + ", ".join((_linestring_wkt_inner(pl) for pl in [self.exterior] + self.holes)) + ")"
 
     def __eq__(self, other: object) -> bool:
         # strict equality, not semantic
-        if isinstance(other, _STPolygon):
+        if isinstance(other, STPolygon):
             return self.exterior == other.exterior and self.holes == other.holes
         return NotImplemented
 
 
 #########################################################################
 # Build supported request/response type mappings
 #########################################################################
@@ -332,86 +333,86 @@
         raise NotImplementedError
 
 
 class _ExecuteQueryFactory(_OcientRequestFactory[proto.ExecuteQueryResponse]):
     def request(self, operation: str) -> proto.Request:
         """Generates a fully populated EXECUTE_QUERY request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("EXECUTE_QUERY")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("EXECUTE_QUERY")
         req.execute_query.sql = operation
         req.execute_query.force = False
         return req
 
     def response(self) -> proto.ExecuteQueryResponse:
         """Generates a fully populated EXECUTE_QUERY response protobuf"""
         return proto.ExecuteQueryResponse()
 
 
 class _ExecuteExplainFactory(_OcientRequestFactory[proto.ExplainResponseStringPlan]):
     def request(self, operation: str) -> proto.Request:
         """Generates a fully populated EXECUTE_EXPLAIN request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("EXECUTE_EXPLAIN")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
-        req.execute_explain.format = proto.ExplainFormat.JSON  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("EXECUTE_EXPLAIN")
+        req.execute_explain.format = proto.ExplainFormat.JSON
         splitted = operation.split(maxsplit=1)
         if len(splitted) == 2:
             req.execute_explain.sql = splitted[1]
         return req
 
     def response(self) -> proto.ExplainResponseStringPlan:
         """Generates a fully populated EXECUTE_EXPLAIN response protobuf"""
         return proto.ExplainResponseStringPlan()
 
 
 class _ExecuteExportFactory(_OcientRequestFactory[proto.ExecuteExportResponse]):
     def request(self, operation: str) -> proto.Request:
         """Generates a fully populated EXECUTE_EXPORT request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("EXECUTE_EXPORT")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("EXECUTE_EXPORT")
         req.execute_export.sql = operation
         return req
 
     def response(self) -> proto.ExecuteExportResponse:
         """Generates a fully populated EXECUTE_EXPORT response protobuf"""
         return proto.ExecuteExportResponse()
 
 
 class _ExplainPipelineFactory(_OcientRequestFactory[proto.ExplainPipelineResponse]):
     def request(self, operation: str) -> proto.Request:
         """Generates a fully populated EXPLAIN_PIPELINE request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("EXPLAIN_PIPELINE")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("EXPLAIN_PIPELINE")
         req.explain_pipeline.sql = operation
         return req
 
     def response(self) -> proto.ExplainPipelineResponse:
         """Generates a fully populated EXPLAIN_PIPELINE response protobuf"""
         return proto.ExplainPipelineResponse()
 
 
 class _CheckDataFactory(_OcientRequestFactory[proto.CheckDataResponse]):
     """NOTE: this command is deprecated"""
 
     def request(self, operation: str) -> proto.Request:
         """Generates a fully populated CHECK_DATA request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("CHECK_DATA")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("CHECK_DATA")
         req.check_data.sql = operation
         return req
 
     def response(self) -> proto.CheckDataResponse:
         """Generates a fully populated CHECK_DATA response protobuf"""
         return proto.CheckDataResponse()
 
 
 class _ForceExternalFactory(_OcientRequestFactory[proto.ConfirmationResponse]):
     def request(self, operation: str) -> proto.Request:
         """Generates a fully populated FORCE_EXTERNAL request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("SET_PARAMETER")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("SET_PARAMETER")
         sp = req.set_parameter
         if operation.endswith("on"):
             sp.force_external.is_on = True
         elif operation.endswith("off"):
             sp.force_external.is_on = False
         else:
             raise ProgrammingError('Format must be "FORCE EXTERNAL (on|off)"')
@@ -422,60 +423,63 @@
         return proto.ConfirmationResponse()
 
 
 class _SetSchemaFactory(_OcientRequestFactory[proto.ConfirmationResponse]):
     def request(self, schema: str) -> proto.Request:
         """Generates a fully populated SET SCHEMA request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("SET_SCHEMA")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("SET_SCHEMA")
         req.set_schema.schema = schema
         return req
 
     def response(self) -> proto.ConfirmationResponse:
         """Generates SET_SCHEMA response protobuf"""
         return proto.ConfirmationResponse()
 
 
 class _GetSchemaFactory(_OcientRequestFactory[proto.GetSchemaResponse]):
-    def request(self) -> proto.Request:  # type: ignore
+    def request(self) -> proto.Request:  # type: ignore[name-defined, override]
         """Generates a fully populated GET SCHEMA request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("GET_SCHEMA")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("GET_SCHEMA")
         return req
 
     def response(self) -> proto.GetSchemaResponse:
         """Generates SET_SCHEMA response protobuf"""
         return proto.GetSchemaResponse()
 
 
 class _ClearCacheFactory(_OcientRequestFactory[proto.ConfirmationResponse]):
-    def request(self) -> proto.Request:  # type: ignore
+    def request(self) -> proto.Request:  # type: ignore[name-defined, override]
         """Generates a fully populated CLEAR CACHE request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("CLEAR_CACHE")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("CLEAR_CACHE")
         req.clear_cache.all_nodes = True
         return req
 
     def response(self) -> proto.ConfirmationResponse:
         """Generates SET_SCHEMA response protobuf"""
         return proto.ConfirmationResponse()
 
 
 class _SetParameterFactory(_OcientRequestFactory[proto.ConfirmationResponse]):
-    def request(self, op: str, val: Union[int, str, float]) -> proto.Request:  # type: ignore
+    def request(self, op: str, val: Union[int, str, float]) -> proto.Request:  # type: ignore[name-defined, override]
         """Generates a fully populated SET PARAMETER request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("SET_PARAMETER")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("SET_PARAMETER")
 
         sp = req.set_parameter
 
         if type(val) == str and val.lower() == "reset":
             # Resets handled in cmdCompServer. Set val to 0 as a Parameter still needs to be set for flow control, and most require number values
             sp.reset = True
-            val = 0 if op != "SERVICECLASS" else val
+            if op in ["MAXROWS", "MAXTIME", "MAXTEMPDISK", "PARALLELISM", "PSO", "ADJUSTTIME"]:
+                val = 0
+            elif op in ["PRIORITY", "ADJUSTFACTOR"]:
+                val = 0.0
 
         # Set the appropriate parameter
         # proto field assignments are type checked at runtime
         if op == "MAXROWS":
             assert isinstance(val, int)
             sp.row_limit.rowLimit = val
         elif op == "MAXTIME":
@@ -512,41 +516,41 @@
         return proto.ConfirmationResponse()
 
 
 class _CancelQueryFactory(_OcientRequestFactory[proto.CancelQueryResponse]):
     def request(self, id: str) -> proto.Request:
         """Generates a fully populated CANCEL QUERY request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("CANCEL_QUERY")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("CANCEL_QUERY")
         req.cancel_query.sql = id
         return req
 
     def response(self) -> proto.CancelQueryResponse:
         """Generates a CANCEL_QUERY response protobuf"""
         return proto.CancelQueryResponse()
 
 
 class _KillQueryFactory(_OcientRequestFactory[proto.KillQueryResponse]):
     def request(self, id: str) -> proto.Request:
         """Generates a fully populated KILL QUERY request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("KILL_QUERY")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("KILL_QUERY")
         req.kill_query.sql = id
         return req
 
     def response(self) -> proto.KillQueryResponse:
         """Generates a KILL_QUERY response protobuf"""
         return proto.KillQueryResponse()
 
 
 class _GetSystemMetadataFactory(_OcientRequestFactory[proto.FetchSystemMetadataResponse]):
-    def request(self, op: proto.FetchSystemMetadata.SystemMetadataCall, schema: Optional[str], table: Optional[str], column: Optional[str], view: Optional[str]) -> proto.Request:  # type: ignore
+    def request(self, op: proto.FetchSystemMetadata.SystemMetadataCall, schema: Optional[str], table: Optional[str], column: Optional[str], view: Optional[str]) -> proto.Request:  # type: ignore[name-defined, override]
         """Generates a fully populated GET_SYSTEM_METADATA request protobuf"""
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("FETCH_SYSTEM_METADATA")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("FETCH_SYSTEM_METADATA")
         req.fetch_system_metadata.call = op
 
         if schema is not None:
             req.fetch_system_metadata.schema = schema
         if table is not None:
             req.fetch_system_metadata.table = table
         if column is not None:
@@ -693,41 +697,27 @@
 
 
 # Sessions code
 
 # Used for representing a session created with a security token sign in
 
 
+@dataclass
 class SecurityToken:
-    def __init__(self, tokenData: str, tokenSignature: str, issuerFingerprint: str) -> None:
-        self.tokenData = tokenData
-        self.tokenSignature = tokenSignature
-        self.issuerFingerprint = issuerFingerprint
-
-
-# Used for representing a session created with a user and password sign in.
-
-
-class UserAndPassword:
-    def __init__(self, user: str, password: str) -> None:
-        self.user = user
-        self.password = password
-
+    """A security token that can be retrieved from a connection object using the
+    attribute `security_token` and may be used on subsequent connection calls
+    """
 
-class Session:
-    def __init__(
-        self, securityToken: Optional[SecurityToken] = None, userAndPassword: Optional[UserAndPassword] = None
-    ) -> None:
-        # Only one of these should be instantiated. The other MUST be none.
-        if (securityToken is None and userAndPassword is None) or (
-            securityToken is not None and userAndPassword is not None
-        ):
-            raise ValueError("Exactly one of securityToken and userAndPassword must be specified")
-        self.securityToken = securityToken
-        self.userAndPassword = userAndPassword
+    token_data: str
+    token_signature: str
+    issuer_fingerprint: str
+
+    @staticmethod
+    def from_json(json_dct: Dict[str, Any]) -> SecurityToken:
+        return SecurityToken(json_dct["token_data"], json_dct["token_signature"], json_dct["issuer_fingerprint"])
 
 
 class Connection:
     """A connection to the Ocient database. Normally constructed by
     calling the module `connect()` call, but can be constructed
     directly
     """
@@ -747,22 +737,20 @@
 
     hosts: List[str] = []
     port = None
     database = None
     tls = None
     force = None
     handshake = None
-    user = None
-    password = None
     secondary_interfaces: Optional[List[List[Tuple[str, int]]]] = None
     secondary_index = -1
     sock: Optional[Union[socket.socket, ssl.SSLSocket]] = None
     session_id = str(uuid.uuid1())
 
-    session = None
+    security_token: Optional[SecurityToken] = None
     serverSessionId = None
 
     # Whether the next execute query run on this connection will be redirected. Does nothing if force is set to true
     force_next_redirect = False
 
     # Sessions code end
 
@@ -801,32 +789,41 @@
         password: Optional[str] = None,
         host: Optional[str] = None,
         database: Optional[str] = None,
         tls: Optional[Union[str, int]] = None,
         handshake: Optional[int] = None,
         force: Optional[bool] = None,
         configfile: Optional[str] = None,
-        session: Optional[Session] = None,
+        security_token: Optional[SecurityToken] = None,
     ) -> None:
         # pylint: disable=too-many-arguments,no-member
         """Connection parameters can be specified as part of the dsn,
         using keyword arguments or both.  If both are specified, the keyword
         parameter overrides the value in the dsn.
 
         The Ocient DSN is of the format:
         `ocient://user:password@[host][:port][/database][?param1=value1&...]`
 
-        `user` and `password` must be supplied.  `host` defaults to localhost,
+        `user` and `password` may be supplied if SSO or a security token are not
+        provided.  `host` defaults to localhost,
         port defaults to 4050, database defaults to `system` and `tls` defaults
         to `off`.
 
         Multiple hosts may be specified, separated by a comma, in which case the
         hosts will be tried in order  Thus an example DSN might be
         `ocient://someone:somepassword@host1,host2:4051/mydb`
 
+        A security token may be used from a previous connection.  For example:
+
+            con1 = connect(host="foo", user="bar", password="baz")
+            sectoken = con1.security_token
+            con1.close()
+            ...
+            con2 = connect(host="foo", security_token=con1.sectoken)
+
         configfile is the name of a configuration file in INI format, where each
         section is either default, or a pattern that matches the host and optionally
         database. sections are matched in order, so more specific sections should
         precede less specific sections::
 
             [DEFAULT]
             tls = unverified
@@ -857,15 +854,15 @@
         - tls: Which can have the values "off", "unverified", or "on" in the dsn,
             or Connection.TLS_NONE, Connection.TLS_UNVERIFIED, or
             Connection.TLS_ON as a keyword parameter.
         - force: True or False, whether to force the connection to remain on this
             server
         """
         # pylint: disable=no-member
-        self._parse_args(dsn, user, password, host, database, tls, handshake, force, configfile)
+        user, password = self._parse_args(dsn, user, password, host, database, tls, handshake, force, configfile)
         assert self.port is not None
 
         saved_exc: Optional[Exception] = None
         for one_host in self.hosts:
             try:
                 logger.info(f"Trying to connect to {one_host}:{self.port}")
                 self.sock = socket.create_connection((one_host, self.port))
@@ -879,26 +876,25 @@
 
         if saved_exc is not None:
             raise Error(f"Unable to connect to {','.join(self.hosts)}:{self.port}: {str(saved_exc)}") from saved_exc
 
         self._sslize_connection()
 
         self._buffer: bytes = b""
-        self.session = session
-        if self.handshake == self.HANDSHAKE_SSO:
-            if self.user or self.password:
+        self.security_token = security_token
+        if self.security_token is not None:
+            self._client_handshake_security_token()
+        elif self.handshake == self.HANDSHAKE_SSO:
+            if user or password:
                 # If either are non-empty, use the CBC_GCM.
-                self._client_handshake_CBC_GCM(is_explicit_sso=True, force=self.force)
+                self._client_handshake_CBC_GCM(user=user, password=password, is_explicit_sso=True, force=self.force)
             else:
-                if self.session is not None and self.session.securityToken is not None:
-                    self._client_handshake_security_token()
-                else:
-                    self._client_handshake_SSO()
+                self._client_handshake_SSO()
         else:
-            self._client_handshake_CBC_GCM(is_explicit_sso=False, force=self.force)
+            self._client_handshake_CBC_GCM(user=user, password=password, is_explicit_sso=False, force=self.force)
 
     def __enter__(self) -> "Connection":
         return self
 
     def __exit__(
         self, exc_type: Optional[Type[BaseException]], exc_val: Optional[BaseException], exc_tb: Optional[TracebackType]
     ) -> None:
@@ -929,33 +925,36 @@
         """
         assert self.database is not None
         client_connection_message.database = self.database
         client_connection_message.clientid = DRIVER_ID
         client_connection_message.version = PROTOCOL_VERSION
         client_connection_message.majorClientVersion = version_major
         client_connection_message.minorClientVersion = version_minor
+        client_connection_message.patchClientVersion = version_patch
         client_connection_message.sessionID = self.session_id
 
-    def _client_handshake_CBC_GCM(self, is_explicit_sso: bool = False, force: bool = False) -> None:
+    def _client_handshake_CBC_GCM(
+        self, user: Optional[str], password: Optional[str], is_explicit_sso: bool = False, force: bool = False
+    ) -> None:
         while True:
             ##################################################################
             # Send the CLIENT_CONNECTION request
             ##################################################################
             client_connection: Union[proto.ClientConnection, proto.ClientConnectionGCM]
             req = proto.Request()
             if self.handshake == self.HANDSHAKE_CBC:
                 req.type = req.CLIENT_CONNECTION
                 client_connection = req.client_connection
             else:
                 # Should be GCM
                 req.type = req.CLIENT_CONNECTION_GCM
                 client_connection = req.client_connection_gcm
                 client_connection.explicitSSO = is_explicit_sso
-            assert self.user is not None
-            client_connection.userid = self.user
+            if user is not None:
+                client_connection.userid = user
             self._initialize_client_connection(client_connection)
 
             _send_msg(self, req)
 
             ##################################################################
             # Get the CLIENT_CONNECTION response and process it
             ##################################################################
@@ -974,15 +973,15 @@
 
             peer_key = load_pem_public_key(
                 rsp1.pubKey.encode(encoding="UTF-8", errors="strict"),
                 backend=default_backend(),
             )
             if not isinstance(peer_key, DHPublicKey):
                 raise Error(f"Public key was not DHPublicKey, was: {type(peer_key)}")
-            (cipher, generated_hmac, public_key) = self._encryption_routine(rsp1.iv, peer_key)
+            (cipher, generated_hmac, public_key) = self._encryption_routine(password, rsp1.iv, peer_key)
 
             ##################################################################
             # Send the CLIENT_CONNECTION2 request
             ##################################################################
             req = proto.Request()
             if self.handshake == self.HANDSHAKE_CBC:
                 req.type = req.CLIENT_CONNECTION2
@@ -1018,15 +1017,20 @@
                 rsp2 = _recv_msg(self, proto.ClientConnectionGCM2Response())
 
             if rsp2.response.type == proto.ConfirmationResponse.RESPONSE_WARN:
                 warn(rsp2.response.reason)
             elif rsp2.response.type == proto.ConfirmationResponse.RESPONSE_OK:
                 # Save the server session id
                 self.serverSessionId = rsp2.serverSessionId
-                self.session = Session(userAndPassword=UserAndPassword(self.user, self.password))
+                received_token = rsp2.securityToken
+                self.security_token = SecurityToken(
+                    received_token.data,
+                    received_token.signature,
+                    received_token.issuerFingerprint,
+                )
                 logger.info(f"Connected to server session Id: {self.serverSessionId}")
                 # Save secondary interfaces.
                 self._save_secondary_interfaces(rsp2.secondary)
 
                 # Redirect the connection
                 if rsp2.redirect:
                     assert self.sock is not None
@@ -1035,15 +1039,17 @@
                     logger.debug(
                         f"Redirecting connection to {rsp2.redirectHost}:{rsp2.redirectPort}, which maps to {mapped_host}:{mapped_port}"
                     )
                     self.sock = socket.create_connection((mapped_host, mapped_port))
                     logger.info(f"Connected to {mapped_host}:{mapped_port} on socket {self.sock}")
                     self._sslize_connection()
 
-                    return self._client_handshake_CBC_GCM(is_explicit_sso, True)
+                    return self._client_handshake_CBC_GCM(
+                        user=user, password=password, is_explicit_sso=is_explicit_sso, force=force
+                    )
 
                 break
 
             # there is something broken in our handshake...retry
             if rsp2.response.vendor_code == -202:
                 logger.debug("Handshake error...retrying")
                 continue
@@ -1126,20 +1132,18 @@
                 # Success
                 waitFor = 0
                 keepPolling = False
 
         self.serverSessionId = rsp.sessionInfo.serverSessionId
         logger.debug(f"Connected to server session Id: {self.serverSessionId}")
         received_token = rsp.sessionInfo.securityToken
-        self.session = Session(
-            securityToken=SecurityToken(
-                received_token.data,
-                received_token.signature,
-                received_token.issuerFingerprint,
-            )
+        self.security_token = SecurityToken(
+            received_token.data,
+            received_token.signature,
+            received_token.issuerFingerprint,
         )
 
         # Save secondary interfaces.
         self._save_secondary_interfaces(rsp.secondary)
 
         # Redirect the connection
         if rsp.redirect:
@@ -1153,28 +1157,27 @@
             logger.info(f"Connected to {mapped_host}:{mapped_port} on socket {self.sock}")
             self._sslize_connection()
 
             return self._client_handshake_security_token(True)
 
     def _client_handshake_security_token(self, force: bool = False) -> None:
         """Once a connection acquires a security token, it can use that to log in. This handshake only
-        sends 1 message whereas the other handshakes send 2. self.session.securityToken must be set.
+        sends 1 message whereas the other handshakes send 2. self.security_token must be set.
         """
         while True:
             req = proto.Request()
             req.type = req.CLIENT_CONNECTION_SECURITY_TOKEN
             client_connection = req.client_connection_security_token
 
             self._initialize_client_connection(client_connection)
             # Attach the security token used to log in
-            assert self.session is not None
-            assert self.session.securityToken is not None
-            client_connection.securityToken = self.session.securityToken.tokenData
-            client_connection.tokenSignature = self.session.securityToken.tokenSignature
-            client_connection.issuerFingerprint = self.session.securityToken.issuerFingerprint
+            assert self.security_token is not None
+            client_connection.securityToken = self.security_token.token_data
+            client_connection.tokenSignature = self.security_token.token_signature
+            client_connection.issuerFingerprint = self.security_token.issuer_fingerprint
             client_connection.force = force
 
             _send_msg(self, req)
 
             rsp = _recv_msg(self, proto.ClientConnectionSecurityTokenResponse())
 
             if rsp.response.type == proto.ConfirmationResponse.RESPONSE_WARN:
@@ -1246,35 +1249,37 @@
                     break
 
         logger.debug(
             f"Saving secondary interfaces: index {self.secondary_index} interfaces: {self.secondary_interfaces}"
         )
 
     def _encryption_routine(
-        self, initialization_vector: bytes, peer_key: DHPublicKey
+        self, password: Optional[str], initialization_vector: bytes, peer_key: DHPublicKey
     ) -> Tuple[bytes, bytes, DHPublicKey]:
         """Internal routine to do the encryption handshake of
         the password
         CBC is the previous form of encryption. We now use GCM by default.
         """
+
+        if password is None:
+            raise Error("Missing password")
         # Create our keys using the parameters from the peer key
         params = peer_key.parameters()
         private_key = params.generate_private_key()
 
         # Create a shared key
         shared_key = private_key.exchange(peer_key)
 
         key = _hash_key(shared_key, b"\0")
         mac_key = _hash_key(shared_key, b"\1")
 
-        assert self.password is not None
         if self.handshake == self.HANDSHAKE_CBC:
             # Pad the plaintext password out using PKCS7
             padder = padding.PKCS7(128).padder()
-            padded_data = padder.update(self.password.encode(encoding="UTF-8", errors="strict"))
+            padded_data = padder.update(password.encode(encoding="UTF-8", errors="strict"))
             padded_data += padder.finalize()
 
             # Encrypt the padded plaintext password using AES CBC and the key
             # we got from our KDF
             encryptor = Cipher(
                 algorithms.AES(key),
                 modes.CBC(initialization_vector),
@@ -1287,15 +1292,15 @@
         else:
             encryptor = Cipher(
                 algorithms.AES(key),
                 modes.GCM(initialization_vector),
                 backend=default_backend(),
             ).encryptor()
             # We do not use AAD
-            cipher = encryptor.update(self.password.encode(encoding="UTF-8", errors="strict")) + encryptor.finalize()
+            cipher = encryptor.update(password.encode(encoding="UTF-8", errors="strict")) + encryptor.finalize()
             # Server side expects that the tag is at the end of the cipher text.
             cipher += encryptor.tag
 
         # Now create an HMAC using the other KDF derived key and the
         # encrypted password
         hasher = hmac.HMAC(mac_key, hashes.SHA256(), backend=default_backend())
         hasher.update(cipher)
@@ -1310,91 +1315,75 @@
         password: Optional[str],
         host: Optional[str],
         database: Optional[str],
         tls: Optional[Union[str, int]],
         handshake: Optional[int],
         force: Optional[bool],
         configfile: Optional[str],
-    ) -> None:  # pylint: disable=too-many-arguments
+    ) -> Tuple[Optional[str], Optional[str]]:  # pylint: disable=too-many-arguments
         """Internal routine to resolve function arguments, config file, and dsn"""
         # pylint: disable=no-member,too-many-branches,too-many-statements
-        # First, parse the DSN if it exists
+        # First, parse the DSN if it exists and store the values in the dsnparams dictionary
+        dsnparams = {}
         if dsn is not None:
             parsed = dsnparse.parse(dsn)
 
             if parsed.scheme and parsed.scheme.lower() != "ocient":
                 raise MalformedURL(f"Invalid DSN scheme: {parsed.scheme}")
 
-            for attr in ["database", "user", "password", "port"]:
-                setattr(self, attr, getattr(parsed, attr))
+            dsnparams = {attr: getattr(parsed, attr) for attr in ["database", "user", "password", "port"]}
 
             if parsed.host:
-                self.hosts = parsed.host.split(",")
+                dsnparams["hosts"] = parsed.host.split(",")
 
-            if self.database is not None and len(self.database) == 0:
-                self.database = None
-            if self.database is not None and self.database[0] == "/":
-                self.database = self.database[1:]
+            if "database" in dsnparams:
+                if len(dsnparams["database"]) == 0:
+                    del dsnparams["database"]
+                elif dsnparams["database"].startswith("/"):
+                    dsnparams["database"] = dsnparams["database"][1:]
 
             if "tls" in parsed.query:
-                self.tls = parsed.query["tls"]
+                dsnparams["tls"] = parsed.query["tls"]
 
             if "force" in parsed.query:
                 shouldForce = parsed.query["force"]
                 if shouldForce.upper() == "TRUE":
-                    self.force = True
+                    dsnparams["force"] = True
                 elif shouldForce.upper() == "FALSE":
-                    self.force = False
+                    dsnparams["force"] = False
                 else:
                     raise MalformedURL(f"Invalid force string: {shouldForce}")
 
-            if force is not None:
-                self.force = force
-
             if "handshake" in parsed.query:
-                handshake = parsed.query["handshake"].lower()
+                dsnparams["handshake"] = parsed.query["handshake"].lower()
 
-            if self.user is None:
-                self.user = ""
+            dsnparams = {k: v for k, v in dsnparams.items() if v is not None}
 
-            if self.password is None:
-                self.password = ""
+        connectparams: Mapping[str, object] = {
+            "user": user,
+            "password": password,
+            "database": database,
+            "tls": tls,
+            "handshake": handshake,
+            "force": force,
+        }
 
-        # Now override the DSN values with any values passed in as parameters
-        if user is not None:
-            self.user = user
-
-        if password is not None:
-            self.password = password
+        connectparams = {k: v for k, v in connectparams.items() if v is not None}
 
         if host:
             # Handle host:port
             parts = host.split(":")
             if len(parts) == 1:
-                self.hosts = parts[0].split(",")
+                connectparams["hosts"] = parts[0].split(",")
             elif len(parts) == 2:
-                self.hosts = parts[0].split(",")
-                self.port = int(parts[1])
+                connectparams["hosts"] = parts[0].split(",")
+                connectparams["port"] = int(parts[1])
             else:
                 raise MalformedURL(f"Invalid host value: {host}")
 
-        if database:
-            self.database = database
-
-        if tls is not None:
-            self.tls = tls
-
-        if handshake is not None:
-            self.handshake = handshake
-
-        # Set the default host now, since we use that as a key into the
-        # config file
-        if not self.hosts:
-            self.hosts = [self.DEFAULT_HOST]
-
         # Now build a configparser with default values
         config = configparser.ConfigParser(
             defaults={
                 "port": str(self.DEFAULT_PORT),
                 "database": self.DEFAULT_DATABASE,
                 "tls": "unverified",
                 "force": "false",
@@ -1404,75 +1393,80 @@
         )
         configvals = None
 
         # If we have a config file try loading that
         if configfile is not None:
             config.read(configfile)
 
+            lookup_host = dsnparams.get("hosts", None) or connectparams.get("hosts", None) or [self.DEFAULT_HOST]
+
             # Work out the host/database if we know it
-            host_db = ",".join(self.hosts)
+            host_db = ",".join(lookup_host)  # type: ignore[arg-type]
             if self.database is not None:
                 host_db = host_db + "/" + self.database
 
             # Try and match each section in the INI file with the host/database
             for s in config.sections():
                 if re.match(s, host_db):
                     configvals = config[s]
                     break
 
         # if we didn't find a matching host (or there is no file). use the defaults
         if configvals is None:
             configvals = config["DEFAULT"]
-        # Force is not places here so it can get parsed below.
-        for attr in ["port", "database", "tls", "handshake"]:
-            if getattr(self, attr) is None:
-                setattr(self, attr, configvals[attr])
 
-        if not self.user:
-            self.user = str(configvals.get("user", ""))
+        configparams: MutableMapping[str, object] = dict(configvals)
+
+        connectparams = {k: v for k, v in connectparams.items() if v != ""}
 
-        if not self.password:
-            self.password = str(configvals.get("password", ""))
+        if isinstance(configparams["force"], str) and configparams["force"].upper() == "TRUE":
+            configparams["force"] = True
+        else:
+            configparams["force"] = False
+
+        defaultparams = {"user": None, "password": None, "hosts": [self.DEFAULT_HOST]}
 
-        if self.force is None:
-            self.force = configvals.getboolean("force")
+        # This will merge the values we get from the config file with
+        # the values from the DSN, with the values explicitly passed in
+        # as parameters to this function
+        params: MutableMapping[str, Any] = {**defaultparams, **configparams, **dsnparams, **connectparams}
 
         # And finally tidy up some things
-        if isinstance(self.port, str):
-            self.port = int(self.port)
+        if isinstance(params["port"], str):
+            params["port"] = int(params["port"])
 
-        if isinstance(self.tls, str):
-            if self.tls.lower() == "off":
-                self.tls = self.TLS_NONE
-            elif self.tls.lower() == "unverified":
-                self.tls = self.TLS_UNVERIFIED
-            elif self.tls.lower() == "on":
-                self.tls = self.TLS_ON
-            else:
-                raise MalformedURL(f"Invalid tls value: {self.tls}")
-        elif isinstance(self.tls, list):
-            raise MalformedURL(f"Multiple TLS values detected: {self.tls}")
+        if isinstance(params["tls"], str):
+            if params["tls"].lower() == "off":
+                params["tls"] = self.TLS_NONE
+            elif params["tls"].lower() == "unverified":
+                params["tls"] = self.TLS_UNVERIFIED
+            elif params["tls"].lower() == "on":
+                params["tls"] = self.TLS_ON
+            else:
+                raise MalformedURL(f"Invalid tls value: {params['tls']}")
+        elif isinstance(params["tls"], list):
+            raise MalformedURL(f"Multiple TLS values detected: {params['tls']}")
 
-        if isinstance(self.handshake, str):
-            if self.handshake.lower() == "cbc":
+        if isinstance(params["handshake"], str):
+            if params["handshake"].lower() == "cbc":
                 self.handshake = self.HANDSHAKE_CBC
-            elif self.handshake.lower() == "sso":
-                self.handshake = self.HANDSHAKE_SSO
+            elif params["handshake"].lower() == "sso":
+                params["handshake"] = self.HANDSHAKE_SSO
             # If they didn't specify handshake, it will be blank and thus should be GCM.
-            elif self.handshake.lower() == "gcm" or self.handshake.lower() == "":
-                self.handshake = self.HANDSHAKE_GCM
+            elif params["handshake"].lower() == "gcm" or params["handshake"].lower() == "":
+                params["handshake"] = self.HANDSHAKE_GCM
             else:
-                print(self.handshake)
-                raise MalformedURL(f"Invalid handshake value: {self.handshake}")
+                raise MalformedURL(f"Invalid handshake value: {params['handshake']}")
 
-        # Don't assert a user parameter has been set. An empty
-        # string for this field is used for authenticating SSO users
+        # Set our parameters, except for user and password
+        for attr in ["database", "hosts", "port", "tls", "force", "handshake"]:
+            setattr(self, attr, params[attr])
 
-        # Don't assert a password parameter has been set. At empty
-        # user and password is for authentication flow with SSO.
+        # return the user and password as return values
+        return params["user"], params["password"]
 
     def close(self) -> None:
         """Close the connection. Subsequent queries on this connection
         will fail
         """
         if not self.sock:
             raise Error("No connection")
@@ -1501,15 +1495,18 @@
         """Return a new cursor for this connection"""
         if not self.sock:
             raise Error("No connection")
         return Cursor(self)
 
     def __del__(self) -> None:
         if self.sock is not None:
-            self.close()
+            try:
+                self.close()
+            except Exception:
+                pass
 
     def resolve_new_endpoint(self, new_host: str, new_port: int) -> Tuple[str, int]:
         """
         Handles mapping to a secondary interface based on the secondary interface mapping saved on this connection.
 
         Args:
             new_host[string]: the new host to be remapped
@@ -1555,22 +1552,20 @@
             [Connection]: A new connection.
         """
         remapped_host, remapped_port = self.resolve_new_endpoint(new_host, new_port)
         new_endpoint = f"{remapped_host}:{remapped_port}"
         logger.debug(f"Redirecting connection to {new_host}:{new_port}, which maps to {remapped_host}:{remapped_port}")
 
         return Connection(
-            user=self.user,
-            password=self.password,
             host=new_endpoint,
             database=self.database,
             tls=self.tls,
             handshake=self.handshake,
             force=self.force,
-            session=self.session,
+            security_token=self.security_token,
         )
 
     def refresh(self) -> None:
         """
         Used to refresh the session associated with this connection. The server will
         return a new server session id and security token.
         """
@@ -1585,27 +1580,19 @@
         if rsp.response.type == proto.ConfirmationResponse.RESPONSE_WARN:
             warn(rsp.response.reason)
         elif rsp.response.type == proto.ConfirmationResponse.RESPONSE_OK:
             # Capture the session id
             self.serverSessionId = rsp.sessionInfo.serverSessionId
             logger.debug(f"Connected to server session Id: {self.serverSessionId}")
             received_token = rsp.sessionInfo.securityToken
-            if self.session is not None and self.session.securityToken is not None:
-                self.session = Session(
-                    securityToken=SecurityToken(
-                        received_token.data,
-                        received_token.signature,
-                        received_token.issuerFingerprint,
-                    )
-                )
-            else:
-                # Ignore the security token
-                assert self.user is not None
-                assert self.password is not None
-                self.session = Session(userAndPassword=UserAndPassword(self.user, self.password))
+            self.security_token = SecurityToken(
+                received_token.data,
+                received_token.signature,
+                received_token.issuerFingerprint,
+            )
             return
         # Something bad happened with the refresh attempt.
         raise _convert_exception(rsp.response)
 
 
 class Cursor:
     # pylint: disable=too-many-instance-attributes
@@ -1896,35 +1883,33 @@
 
         # generate the appropriate request
         req = factory.request(operation)
 
         # Loop while we retry redirects and reconnects
         while True:
             assert self.connection.force is not None
-            if req.type == proto.Request.RequestType.Value("EXECUTE_QUERY"):  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+            if req.type == proto.Request.RequestType.Value("EXECUTE_QUERY"):
                 req.execute_query.force = self.connection.force
                 req.execute_query.forceRedirect = self.connection.force_next_redirect
                 self.connection.force_next_redirect = False
-            elif req.type == proto.Request.RequestType.Value("EXECUTE_EXPLAIN"):  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+            elif req.type == proto.Request.RequestType.Value("EXECUTE_EXPLAIN"):
                 req.execute_explain.force = self.connection.force
             try:
                 _send_msg(self.connection, req)
 
                 rsp = _recv_msg(self.connection, factory.response())
             except IOError:
                 # remake our connection
                 self.connection = Connection(
-                    user=self.connection.user,
-                    password=self.connection.password,
+                    security_token=self.connection.security_token,
                     host=f"{','.join(self.connection.hosts)}:{self.connection.port}",
                     database=self.connection.database,
                     tls=self.connection.tls,
                     handshake=self.connection.handshake,
                     force=self.connection.force,
-                    session=self.connection.session,
                 )
 
                 continue
 
             if rsp.response.type == proto.ConfirmationResponse.RESPONSE_WARN:
                 warn(rsp.response.reason)
             elif not rsp.response.type == proto.ConfirmationResponse.RESPONSE_OK:
@@ -1952,36 +1937,36 @@
         self.rownumber = 0
 
         if query_type in ["SELECT", "WITH", "SHOW"]:
             self._get_result_metadata()
 
         elif query_type == "EXPORT":
             self.description = [
-                ("export", TypeCodes.CHAR, None, None, None, None, None)
+                ("export", TypeCodes.CHAR.value, None, None, None, None, None)
             ]  # display_size  # internal_size  # precision  # scale  # null_ok
-            self.resultset_tuple = namedtuple("Row", ("export",))  # type: ignore
+            self.resultset_tuple = namedtuple("Row", ("export",))  # type: ignore[misc]
             self.generated_result = rsp.exportStatement
         elif query_type == "EXPLAIN":
             self.description = [
-                ("explain", TypeCodes.CHAR, None, None, None, None, None)
+                ("explain", TypeCodes.CHAR.value, None, None, None, None, None)
             ]  # display_size  # internal_size  # precision  # scale  # null_ok
-            self.resultset_tuple = namedtuple("Row", ("explain",))  # type: ignore
+            self.resultset_tuple = namedtuple("Row", ("explain",))  # type: ignore[misc]
             self.generated_result = rsp.plan
         elif query_type == "EXPLAIN PIPELINE":
             self.description = [
-                ("explain_pipeline", TypeCodes.CHAR, None, None, None, None, None)
+                ("explain_pipeline", TypeCodes.CHAR.value, None, None, None, None, None)
             ]  # display_size  # internal_size  # precision  # scale  # null_ok
-            self.resultset_tuple = namedtuple("Row", ("explain_pipeline",))  # type: ignore
+            self.resultset_tuple = namedtuple("Row", ("explain_pipeline",))  # type: ignore[misc]
             self.generated_result = rsp.pipelineStatement
         elif query_type == "CHECK":
             # The result of the CHECK DATA statement is a string with a lot of linefeeds. TODO convert it to something reasonable
             self.description = [
-                ("result", TypeCodes.CHAR, None, None, None, None, None),
+                ("result", TypeCodes.CHAR.value, None, None, None, None, None),
             ]  # display_size  # internal_size  # precision  # scale  # null_ok
-            self.resultset_tuple = namedtuple("Row", ("result",))  # type: ignore
+            self.resultset_tuple = namedtuple("Row", ("result",))  # type: ignore[misc]
             self.generated_result = rsp.checkDataStatement
 
     # After list all queries and list all completed queries have been remapped, this is no longer used. But it can be used for other things.
     # Ex: list tables, list views, list table privileges. None of these are implemented yet.
     def _execute_list(self, operation: str = "LIST ALL QUERIES") -> None:
         """Execute LIST_ALL_QUERIES"""
         # pylint: disable=no-member
@@ -1998,22 +1983,20 @@
             try:
                 _send_msg(self.connection, req)
 
                 rsp = _recv_msg(self.connection, factory.response())
             except IOError:
                 # remake our connection
                 self.connection = Connection(
-                    user=self.connection.user,
-                    password=self.connection.password,
+                    security_token=self.connection.security_token,
                     host=f"{','.join(self.connection.hosts)}:{self.connection.port}",
                     database=self.connection.database,
                     tls=self.connection.tls,
                     handshake=self.connection.handshake,
                     force=self.connection.force,
-                    session=self.connection.session,
                 )
 
                 continue
             break
 
         if rsp.response.type == proto.ConfirmationResponse.RESPONSE_WARN:
             warn(rsp.response.reason)
@@ -2036,15 +2019,15 @@
 
         # Create the column descriptions
         row = rows[0]
         for field in row._fields:
             self.description.append(
                 (
                     field,
-                    TypeCodes.cls_to_type(row._field_types[field]),
+                    TypeCodes.cls_to_type(row._field_types[field]).value,
                     None,
                     None,
                     None,
                     None,
                     None,
                 )  # display_size  # internal_size  # precision  # scale  # null_ok
             )
@@ -2074,24 +2057,24 @@
         colnames = []
         for i in range(len(cols)):  # pylint: disable=consider-using-enumerate
             name = cols[i]
             # This tuple is defined in PEP 249
             self.description.append(
                 (
                     name,
-                    TypeCodes.to_type(rsp.cols2Types[name]),
+                    TypeCodes[rsp.cols2Types[name]].value,
                     None,
                     None,
                     None,
                     None,
                     None,
                 )
             )  # display_size  # internal_size  # precision  # scale  # null_ok
             colnames.append(name)
-        self.resultset_tuple = namedtuple("Row", colnames, rename=True)  # type: ignore
+        self.resultset_tuple = namedtuple("Row", colnames, rename=True)  # type: ignore[assignment, misc]
 
     def _execute_update(self, operation: str) -> None:
         """Execute an update statement"""
         # pylint: disable=no-member
         # While we are redirecting...
 
         # There is no resultset data from an update
@@ -2107,22 +2090,20 @@
             try:
                 _send_msg(self.connection, req)
 
                 rsp = _recv_msg(self.connection, proto.ExecuteUpdateResponse())
             except IOError:
                 # remake our connection
                 self.connection = Connection(
-                    user=self.connection.user,
-                    password=self.connection.password,
+                    security_token=self.connection.security_token,
                     host=f"{','.join(self.connection.hosts)}:{self.connection.port}",
                     database=self.connection.database,
                     tls=self.connection.tls,
                     handshake=self.connection.handshake,
                     force=self.connection.force,
-                    session=self.connection.session,
                 )
 
                 continue
 
             if rsp.response.type == proto.ConfirmationResponse.RESPONSE_WARN:
                 warn(rsp.response.reason)
             elif not rsp.response.type == proto.ConfirmationResponse.RESPONSE_OK:
@@ -2248,27 +2229,27 @@
                 # and try again
                 self._execute_get_schema()
                 return
             else:
                 raise _convert_exception(rsp.response)
 
         self.description = [
-            ("schema", TypeCodes.CHAR, None, None, None, None, None)
+            ("schema", TypeCodes.CHAR.value, None, None, None, None, None)
         ]  # display_size  # internal_size  # precision  # scale  # null_ok
 
         Row = namedtuple("Row", ("schema",))
         self.list_result = [Row._make((rsp.schema,))]
 
     # If we need to implement more of these sorts of custom commands, consider
     # making a factory for the description and results.
     def _execute_get_server_session_id(self) -> None:
         if self.connection.serverSessionId is None:
             raise Error(reason=f"Connection {self.connection} for cursor {self} has no serverSessionId")
         self.description = [
-            ("server_session_id", TypeCodes.CHAR, None, None, None, None, None)
+            ("server_session_id", TypeCodes.CHAR.value, None, None, None, None, None)
         ]  # display_size  # internal_size  # precision  # scale  # null_ok
         Row = namedtuple("Row", ("server_session_id",))
         self.list_result = [Row._make((self.connection.serverSessionId,))]
 
     def _execute_get(self, params: Sequence[str]) -> None:
         if len(params) == 1 and params[0].upper() == "SCHEMA":
             self._execute_get_schema()
@@ -2365,17 +2346,17 @@
             self._get_result_metadata()
 
             for blob in rsp.result_set_val.blobs:
                 self._buffers.append(blob)
             return None
 
         if rsp.HasField("string_val"):
-            return rsp.string_val
+            return rsp.string_val  # type: ignore[no-any-return]
 
-        return rsp.int_val
+        return rsp.int_val  # type: ignore[no-any-return]
 
     def _get_more_data(self) -> None:
         """Internal routine to get more data from a query"""
         # pylint: disable=no-member
         req = proto.Request()
         req.type = req.FETCH_DATA
         req.fetch_data.fetch_size = self.arraysize
@@ -2607,15 +2588,15 @@
         if coltype == TypeCodes.UUID:
             self._offset += 16
             return uuid.UUID(bytes=self._buf()[self._offset - 16 : self._offset])
 
         if coltype == TypeCodes.ST_POINT:
             long = self._get_double()
             lat = self._get_double()
-            return _STPoint(long, lat)
+            return STPoint(long, lat)
 
         if coltype == TypeCodes.DATE:
             d = datetime.datetime.utcfromtimestamp(self._get_long() / 1000.0)
             return datetime.date(d.year, d.month, d.day)
 
         if coltype == TypeCodes.IP:
             off = self._offset
@@ -2648,35 +2629,35 @@
 
         if coltype == TypeCodes.ST_LINESTRING:
             points = []
             num_elements = self._get_int()
             for i in range(num_elements):
                 long = self._get_double()
                 lat = self._get_double()
-                points.append(_STPoint(long, lat))
-            return _STLinestring(points)
+                points.append(STPoint(long, lat))
+            return STLinestring(points)
 
         if coltype == TypeCodes.ST_POLYGON:
             exterior = []
             num_elements = self._get_int()
             for i in range(num_elements):
                 long = self._get_double()
                 lat = self._get_double()
-                exterior.append(_STPoint(long, lat))
+                exterior.append(STPoint(long, lat))
             holes = []
             num_rings = self._get_int()
             for i in range(num_rings):
                 num_elements = self._get_int()
                 ring = []
                 for j in range(num_elements):
                     long = self._get_double()
                     lat = self._get_double()
-                    ring.append(_STPoint(long, lat))
+                    ring.append(STPoint(long, lat))
                 holes.append(ring)
-            return _STPolygon(exterior, holes)
+            return STPolygon(exterior, holes)
 
         self.end_of_data = True
         raise Error(reason=f"Unknown column type {coltype}")
 
     def _get_byte(self) -> int:
         offset = self._offset
         self._offset += 1
@@ -2724,15 +2705,15 @@
             else:
                 array.append(self._decode_entry())
 
         return array
 
     def _close_resultset(self) -> None:
         req = proto.Request()
-        req.type = proto.Request.RequestType.Value("CLOSE_RESULT_SET")  # type: ignore # https://github.com/protocolbuffers/protobuf/issues/10240
+        req.type = proto.Request.RequestType.Value("CLOSE_RESULT_SET")
 
         _send_msg(self.connection, req)
 
         rsp = _recv_msg(self.connection, proto.ConfirmationResponse())
 
         if rsp.type == proto.ConfirmationResponse.RESPONSE_WARN:
             warn(rsp.reason)
@@ -2743,24 +2724,51 @@
         num_elements = self._get_int()
         restuple: Tuple[object, ...] = ()
         for _ in range(num_elements):
             restuple += (self._decode_entry(),)
         return restuple
 
 
+def custom_type_to_json(obj: object) -> Union[str, List[int]]:
+    """Helper function to convert types returned from queries to
+    JSON values.  Typically invoked passed as the `default` parameter
+    to json.dumps as in:
+
+    `json.dumps(some_rows, default=custom_type_to_json)`
+    """
+    if isinstance(obj, decimal.Decimal):
+        return str(obj)
+
+    if isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
+        return obj.isoformat()
+
+    if isinstance(obj, bytes):
+        return list(obj)
+
+    if isinstance(obj, (uuid.UUID, ipaddress.IPv4Address, ipaddress.IPv6Address)):
+        return str(obj)
+
+    if isinstance(obj, (STPoint, STLinestring, STPolygon)):
+        # TODO GeoJSON??
+        return str(obj)
+
+    raise TypeError(f"Unknown type {obj.__class__.__name__}")
+
+
 def connect(
     dsn: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     host: Optional[str] = None,
     database: Optional[str] = None,
     tls: Optional[Union[int, str]] = None,
     force: Optional[bool] = None,
     handshake: Optional[Union[int, str]] = "gcm",
     configfile: Optional[str] = None,
+    security_token: Optional[SecurityToken] = None,
 ) -> Connection:
     # pylint: disable=too-many-arguments
     """Create a new database connection.
 
     The connection parameters can be specified as part of the dsn,
     using keyword arguments or both.  If both are specified, the keyword
     parameter overrides the value in the dsn.
@@ -2814,8 +2822,8 @@
         "database": database,
         "tls": tls,
         "handshake": handshake,
     }
 
     logger.debug(f"Connect {params}")
 
-    return Connection(dsn, user, password, host, database, tls, handshake, force, configfile)
+    return Connection(dsn, user, password, host, database, tls, handshake, force, configfile, security_token)
```

### Comparing `pyocient-2.0.0/pyocient/cli.py` & `pyocient-3.0.3/pyocient/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,21 @@
-import datetime
-import decimal
-import ipaddress
 import logging
 import os
 import pathlib
+import re
 import sys
-import uuid
 import warnings
 from time import time_ns
 from typing import TYPE_CHECKING, Callable, List, NamedTuple, Optional, Tuple, Union
 
-from prompt_toolkit.history import FileHistory
+from prompt_toolkit.history import FileHistory, History
 
-from pyocient.api import Connection, SQLException, TypeCodes, _STLinestring, _STPoint, _STPolygon, connect
+from pyocient.api import Connection, SQLException, TypeCodes, connect, custom_type_to_json
 from pyocient.pkg_version import __version__ as version
-
-
-def _custom_type_to_json(obj: object) -> Union[str, List[int]]:
-    """Helper function to convert types returned from queries to
-    JSON values.  Typically invoked passed as the `default` parameter
-    to json.dumps as in:
-
-    `json.dumps(some_rows, default=_custom_type_to_json)`
-    """
-    if isinstance(obj, decimal.Decimal):
-        return str(obj)
-
-    if isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
-        return obj.isoformat()
-
-    if isinstance(obj, bytes):
-        return list(obj)
-
-    if isinstance(obj, (uuid.UUID, ipaddress.IPv4Address, ipaddress.IPv6Address)):
-        return str(obj)
-
-    if isinstance(obj, (_STPoint, _STLinestring, _STPolygon)):
-        # TODO GeoJSON??
-        return str(obj)
-
-    print(f"type_to_string got called for type {type(obj)}", file=sys.stderr)
-    return f"placeholder for {type(obj)}"
+from pyocient.text2sql import DEFAULT_MODELS_BY_BACKEND, text2sql
 
 
 class IgnoreSpaceFileHistory(FileHistory):
     def __init__(self, filename: str):
         super().__init__(filename=filename)
 
     def _is_sensitive_cmd(self, string: str) -> bool:
@@ -162,14 +133,21 @@
         "-l",
         "--loglevel",
         type=str,
         default="critical",
         choices=["critical", "error", "warning", "info", "debug"],
         help="Logging level, defaults to critical",
     )
+    parser.add_argument(
+        "-r",
+        "--rows",
+        type=int,
+        default=sys.maxsize,
+        help="Number of rows to fetch at a time. Note that for JSON and table format output, the output will appear in blocks of this size",
+    )
     parser.add_argument("--logfile", type=FileType("a"), default=sys.stdout, help="Log file")
     parser.add_argument("-t", "--time", action="store_true", help="Output query time")
     parser.add_argument(
         "dsn",
         nargs="?",
         help="DSN of the form ocient://user:password@[host][:port][/database][?param1=value1&...]",
     )
@@ -189,27 +167,74 @@
     )
     parser.add_argument(
         "--nohistory",
         action="store_true",
         help="When using pyocient interactively, do not store command history",
     )
 
+    group = parser.add_argument_group("Text-to-SQL")
+
+    group.add_argument(
+        "--llm-backend",
+        type=str,
+        choices=["openai", "anthropic"],
+        default="openai",
+        help=(
+            "Backend to use for LLM tasks. Each backend requires its own API"
+            ' key to be set in the environment. For "openai", set'
+            ' OPENAI_API_KEY. For "anthropic", set ANTHROPIC_API_KEY. (default:'
+            " openai)"
+        ),
+    )
+    group.add_argument(
+        "--llm-model",
+        type=str,
+        default=None,
+        help=f"Model to use with selected backend. (defaults: {DEFAULT_MODELS_BY_BACKEND})",
+    )
+    group.add_argument(
+        "--llm-temperature",
+        type=float,
+        default=0.2,
+        help=(
+            "Temperature for LLM (0.0-1.0). A temperature of zero should return"
+            " the same results every time, even if incorrect. A higher"
+            " temperature will be more likely to generate different answers on"
+            " subsequent submissions of the same question (default: 0.2)"
+        ),
+    )
+    group.add_argument(
+        "--prompt-with-system-catalog",
+        action="store_true",
+        help=(
+            "If set, include all system catalog tables in the LLM prompt. Note"
+            " that this significantly increases the size of the prompt, by"
+            " approximately 10,000 tokens depending on the model selected."
+            " Including catalog tables in the prompt may enable a generic"
+            " model to answer introspective/monitoring queries about Ocient."
+            " (default: False)"
+        ),
+    )
+
     return parser
 
 
 def main() -> int:
     import csv
     import json
     from argparse import Namespace
 
-    from pygments.lexers.sql import SqlLexer  # type: ignore
-    from pygments.token import Token  # type: ignore
+    from pygments.lexers.sql import SqlLexer
+    from pygments.token import Token
     from tabulate import tabulate
 
-    args = argparser().parse_args(sys.argv[1:])
+    try:
+        args = argparser().parse_args(sys.argv[1:])
+    except SystemExit as e:
+        return os.EX_USAGE
 
     log_level = getattr(logging, args.loglevel.upper(), None)
 
     # Ensure that warnings are always displayed
     warnings.simplefilter("always", UserWarning)
 
     if not isinstance(log_level, int):
@@ -235,41 +260,47 @@
         return input
 
     def _do_line(
         args: Namespace,
         connection: Optional[Connection],
         text: str,
         sql_stmt: str,
-        query_fn: Callable[[Namespace, Optional[Connection], str], Tuple[Optional[Connection], int]],
+        history: Optional[History],
+        query_fn: Callable[[Namespace, Optional[Connection], str, Optional[History]], Tuple[Optional[Connection], int]],
     ) -> Tuple[str, Optional[Connection], int]:
         new_connection = connection
+        return_code = os.EX_OK
+
         for token_type, token_val in lexer.get_tokens(text):
             if token_type == Token.Punctuation and token_val == ";":
-                (new_connection, return_code) = query_fn(args, new_connection, sql_stmt)
+                (new_connection, return_code) = query_fn(args, new_connection, sql_stmt, history)
                 sql_stmt = ""
             else:
                 sql_stmt += token_val
 
         return (sql_stmt, new_connection, return_code)
 
-    def _do_query(args: Namespace, connection: Optional[Connection], query: str) -> Tuple[Optional[Connection], int]:
+    def _do_query(
+        args: Namespace, connection: Optional[Connection], query: str, history: Optional[History]
+    ) -> Tuple[Optional[Connection], int]:
 
         if args.echo:
             print(query, file=args.outfile)
 
         # First, see if this is something we should handle here in the CLI
         tokens = [
             token
             for (token_type, token) in lexer.get_tokens(query)
             if token_type
             in (
                 Token.Keyword,
                 Token.Name,
                 Token.Literal.String.Symbol,
                 Token.Literal.String.Single,
+                Token.Literal.Number.Integer,
             )
         ]
 
         # connect to statement
         if len(tokens) > 1 and tokens[0].lower() == "connect" and tokens[1].lower() == "to":
             try:
                 if len(tokens) == 7:
@@ -308,92 +339,150 @@
             elif echo_val in ["off", "false", 0]:
                 args.echo = False
                 return (connection, os.EX_OK)
             else:
                 print("Invalid echo statement", file=sys.stderr)
                 return (connection, os.EX_DATAERR)
 
+        # set rows
+        if len(tokens) > 2 and tokens[0].lower() == "set" and tokens[1].lower() == "rows":
+            try:
+                args.rows = int(tokens[2])
+            except ValueError as verr:
+                print(f"Invalid rows value: {tokens[2]}", file=sys.stderr)
+                return (connection, os.EX_DATAERR)
+            return (connection, os.EX_OK)
+
         # source
         if len(tokens) > 0 and tokens[0].lower() == "source":
             if len(tokens) != 2:
                 print("Invalid SOURCE statement", file=sys.stderr)
                 return (connection, os.EX_DATAERR)
 
             try:
                 with open(_unquote(tokens[1]), mode="r") as f:
-                    (sql_stmt, connection, return_code) = _do_line(args, connection, f.read(), "", _do_query)
+                    (sql_stmt, connection, return_code) = _do_line(args, connection, f.read(), "", history, _do_query)
                 if len(sql_stmt.strip()):
-                    connection, return_code = _do_query(args, connection, sql_stmt)
+                    connection, return_code = _do_query(args, connection, sql_stmt, history)
                 return (connection, return_code)
             except Exception as e:
                 print(e, file=sys.stderr)
                 return (connection, os.EX_OSERR)
 
         # quit
         if len(tokens) > 0 and tokens[0].lower() == "quit":
-            sys.exit(os.EX_OK)
+            if connection:
+                connection.close()
+            raise EOFError()
 
         if connection is None:
             print(f"No active connection", file=sys.stderr)
             return (connection, os.EX_UNAVAILABLE)
 
+        # text2sql (requires active connection)
+        text2sql_query = query.lstrip()
+        if text2sql_query and text2sql_query[0] == "?":
+            text2sql_query = text2sql_query[1:].lstrip()
+            if not text2sql_query:
+                return (connection, os.EX_OK)
+            try:
+                answer = text2sql(
+                    connection,
+                    text2sql_query,
+                    backend=args.llm_backend,
+                    model=args.llm_model,
+                    temperature=args.llm_temperature,
+                    with_sys_catalog=args.prompt_with_system_catalog,
+                ).lstrip()
+            except Exception as e:
+                print(f"{type(e).__name__}:", e, file=sys.stderr)
+                return (connection, os.EX_OSERR)
+            is_sql = re.match(r"[A-Z]{3,}", answer) is not None and not answer.startswith("SQL")
+            if is_sql:
+                answer, _, _ = answer.partition(";")
+                is_explainable = answer.startswith(("SELECT ", "WITH ", "SHOW "))
+                if is_explainable:
+                    # Run an EXPLAIN on the query and see if it's valid
+                    old_outfile = args.outfile
+                    with open(os.devnull, "w") as f:
+                        args.outfile = f
+                        try:
+                            connection, return_code = _do_query(args, connection, f"EXPLAIN {answer}", history)
+                        finally:
+                            args.outfile = old_outfile
+                        if return_code != os.EX_OK:
+                            print(f"{answer}\nA syntactically invalid query was generated.", file=args.outfile)
+                            return connection, return_code
+                # Prompt user to run the query (may be invalid DDL!)
+                # HACK `input` might not play nice with prompt_toolkit?
+                response = input(f"{answer}\nRun this query? (y/n): ").lower()
+                if response == "y":
+                    if history is not None:
+                        history.append_string(f"{answer};")
+                    return _do_query(args, connection, answer, history)
+                return (connection, os.EX_OK)
+            else:
+                # Response is almost certainly not a SQL query, print it verbatim.
+                print(answer, file=args.outfile)
+                return (connection, os.EX_OK)
+
         # OK, if we fall through to here, have the normal library handle it
         if args.time:
             starttime = time_ns()
 
         cursor = connection.cursor()
 
         result: Optional[List[NamedTuple]]
         try:
             cursor.execute(query)
 
             if cursor.description:
-                result = cursor.fetchall()
+                result = cursor.fetchmany(args.rows)
             else:
                 result = None
         except SQLException as e:
             print(e, file=sys.stderr)
             return (cursor.connection, os.EX_DATAERR)
         except KeyboardInterrupt:
             print("Operation interrupted.", file=sys.stderr)
             cur_conn = cursor.connection
             cur_conn.close()
             return (
                 Connection(
-                    user=cur_conn.user,
-                    password=cur_conn.password,
+                    security_token=cur_conn.security_token,
                     host=",".join(cur_conn.hosts),
                     database=cur_conn.database,
                     tls=cur_conn.tls,
                     handshake=cur_conn.handshake,
                     force=cur_conn.force,
-                    session=cur_conn.session,
                 ),
                 os.EX_IOERR,
             )
 
         if args.time:
             endtime = time_ns()
 
         if cursor.description is None:
             print("OK", file=args.outfile)
 
         elif args.outfile is not None:
+            colnames = [c[0] for c in cursor.description]
+            binary_column_idxs = [i for i, col in enumerate(cursor.description) if col[1] == TypeCodes.BINARY]
+
             if cursor.generated_result and cursor.description[0][0] == "explain":
                 to_dump = [{"explain": json.loads(cursor.generated_result)}]
 
                 print(
-                    json.dumps(to_dump, indent=4, default=_custom_type_to_json),
+                    json.dumps(to_dump, indent=4, default=custom_type_to_json),
                     file=args.outfile,
                 )
                 result = None
 
-            if result:
+            while result:
                 # Preprocess bytes objects into desired str output, default to hex
-                binary_column_idxs = [i for i, col in enumerate(cursor.description) if col[1] == TypeCodes.BINARY]
                 if binary_column_idxs:
                     for i, row in enumerate(result):
                         for col_idx in binary_column_idxs:
                             col = row[col_idx]
                             if col is not None:
                                 assert isinstance(col, bytes)
                                 # N.B. this line relies on the assumption (true today) that
@@ -401,43 +490,45 @@
                                 #      `cursor.description` tuples. This assumption allows
                                 #      this line to look up the NamedTuple field name, which
                                 #      importantly may differ from the column name due to
                                 #      `rename=True` in the NamedTuple constructor, by its
                                 #      column index.
                                 result[i] = row._replace(**{row._fields[col_idx]: col.hex()})
 
-                colnames = [c[0] for c in cursor.description]
-
                 if args.format == "json":
                     dict_result = [row._asdict() for row in result]
 
                     print(
-                        json.dumps(dict_result, indent=4, default=_custom_type_to_json),
+                        json.dumps(dict_result, indent=4, default=custom_type_to_json),
                         file=args.outfile,
                     )
                 elif args.format == "table":
                     print(
                         tabulate(
                             result,
                             headers=colnames,
                             tablefmt="psql",
                         ),
                         file=args.outfile,
                     )
                 elif args.format == "csv":
-                    csv.writer(args.outfile, quoting=csv.QUOTE_ALL).writerow(colnames)
+                    if colnames:
+                        csv.writer(args.outfile, quoting=csv.QUOTE_ALL).writerow(colnames)
                     writer = csv.writer(args.outfile)
                     for row in result:
                         writer.writerow(row)
 
+                colnames = []
+                result = cursor.fetchmany(args.rows)
+
         if args.time:
             endtime = time_ns()
             print(f"Execution time: {(endtime - starttime)/1000000000:.3f} seconds", file=args.outfile)
 
-        if cursor.description and args.outfile.isatty():
+        if cursor.description and args.outfile and args.outfile.isatty():
             print(f"Fetched {cursor.rowcount} rows")
         # If we don't return this connection, then we end up using the old connection which we could have been redirected
         return (cursor.connection, os.EX_OK)
 
     def _do_repl(args: Namespace, connection: Optional[Connection]) -> None:
         from pathlib import Path
 
@@ -471,42 +562,55 @@
             try:
                 text = session.prompt("> ")
             except KeyboardInterrupt:
                 sql_stmt = ""
                 continue
             except EOFError:
                 break
-            (sql_stmt, connection, return_code) = _do_line(args, connection, text, sql_stmt, _do_query)
+            (sql_stmt, connection, return_code) = _do_line(args, connection, text, sql_stmt, history, _do_query)
 
         if len(sql_stmt.strip()):
-            (connection, return_code) = _do_query(args, connection, sql_stmt)
+            (connection, return_code) = _do_query(args, connection, sql_stmt, history)
 
         print("GoodBye!", file=args.outfile)
 
     return_code = os.EX_OK
+    connection = None
     try:
         if args.dsn:
             connection = connect(args.dsn, configfile=args.configfile)
-        else:
-            connection = None
 
         if args.sql:
-            (connection, return_code) = _do_query(args, connection, args.sql)
+            (connection, return_code) = _do_query(args, connection, args.sql, None)
         elif args.infile:
-            (sql_stmt, connection, return_code) = _do_line(args, connection, args.infile.read(), sql_stmt, _do_query)
+            (sql_stmt, connection, return_code) = _do_line(
+                args, connection, args.infile.read(), sql_stmt, None, _do_query
+            )
             if len(sql_stmt.strip()):
-                (connection, return_code) = _do_query(args, connection, sql_stmt)
+                (connection, return_code) = _do_query(args, connection, sql_stmt, None)
         elif sys.stdin.isatty():
             _do_repl(args, connection)
         else:
-            (sql_stmt, connection, return_code) = _do_line(args, connection, sys.stdin.read(), sql_stmt, _do_query)
+            (sql_stmt, connection, return_code) = _do_line(
+                args, connection, sys.stdin.read(), sql_stmt, None, _do_query
+            )
+            if len(sql_stmt.strip()):
+                (connection, return_code) = _do_query(args, connection, sql_stmt, None)
 
     except SQLException as exc:
         print(f"Error: {exc.reason}", file=sys.stderr)
         return_code = os.EX_DATAERR
+    except EOFError:
+        return_code = os.EX_OK
+    finally:
+        if connection:
+            try:
+                connection.close()
+            except SQLException:
+                pass
 
     return return_code
 
 
 if __name__ == "__main__":
     return_code = main()
     sys.exit(return_code)
```

### Comparing `pyocient-2.0.0/setup.py` & `pyocient-3.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         "dsnparse<=0.1.15",
         "prompt-toolkit",
         "pygments",
         "tabulate",
         "cryptography",
         "protobuf>=3.20.0,<=4.22.0",
     ],
+    extras_require={
+        "anthropic": ["anthropic>=0.3.0"],
+        "openai": ["openai>=0.27.0"],
+    },
     packages=["pyocient"],
     package_data={"pyocient": ["py.typed"]},
     entry_points={
         "console_scripts": [
             "pyocient=pyocient.cli:main",
         ],
     },
```

