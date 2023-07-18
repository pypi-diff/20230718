# Comparing `tmp/fastapi_mail-1.3.1.tar.gz` & `tmp/fastapi_mail-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mail-1.3.1.tar", max compression
+gzip compressed data, was "fastapi_mail-1.4.0.tar", max compression
```

## Comparing `fastapi_mail-1.3.1.tar` & `fastapi_mail-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1072 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/LICENSE
--rwxr-xr-x   0        0        0     3407 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/README.md
--rwxr-xr-x   0        0        0      385 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/__init__.py
--rw-r--r--   0        0        0     1127 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/config.py
--rw-r--r--   0        0        0     1848 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/connection.py
--rw-r--r--   0        0        0      122 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/email_utils/__init__.py
--rw-r--r--   0        0        0    16451 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/email_utils/email_check.py
--rwxr-xr-x   0        0        0      530 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/errors.py
--rwxr-xr-x   0        0        0     4004 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/fastmail.py
--rw-r--r--   0        0        0     5731 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/msg.py
--rw-r--r--   0        0        0        0 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/py.typed
--rw-r--r--   0        0        0     3354 2023-07-01 12:52:26.653248 fastapi_mail-1.3.1/fastapi_mail/schemas.py
--rw-r--r--   0        0        0     1871 2023-07-01 12:52:43.601124 fastapi_mail-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4670 1970-01-01 00:00:00.000000 fastapi_mail-1.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/LICENSE
+-rwxr-xr-x   0        0        0     3407 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/README.md
+-rwxr-xr-x   0        0        0      385 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/config.py
+-rw-r--r--   0        0        0     1848 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/connection.py
+-rw-r--r--   0        0        0      122 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/email_utils/__init__.py
+-rw-r--r--   0        0        0    16777 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/email_utils/email_check.py
+-rwxr-xr-x   0        0        0      530 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/errors.py
+-rwxr-xr-x   0        0        0     4004 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/fastmail.py
+-rw-r--r--   0        0        0     5731 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/msg.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/py.typed
+-rw-r--r--   0        0        0     3388 2023-07-18 06:40:33.911708 fastapi_mail-1.4.0/fastapi_mail/schemas.py
+-rw-r--r--   0        0        0     1899 2023-07-18 06:40:54.415835 fastapi_mail-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 fastapi_mail-1.4.0/PKG-INFO
```

### Comparing `fastapi_mail-1.3.1/LICENSE` & `fastapi_mail-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.3.1/README.md` & `fastapi_mail-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.3.1/fastapi_mail/config.py` & `fastapi_mail-1.4.0/fastapi_mail/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from aiosmtplib.api import DEFAULT_TIMEOUT
 from jinja2 import Environment, FileSystemLoader
-from pydantic import BaseSettings as Settings
 from pydantic import DirectoryPath, EmailStr, conint
+from pydantic_settings import BaseSettings as Settings
 
 
 class ConnectionConfig(Settings):
     MAIL_USERNAME: str
     MAIL_PASSWORD: str
     MAIL_PORT: int
     MAIL_SERVER: str
```

### Comparing `fastapi_mail-1.3.1/fastapi_mail/connection.py` & `fastapi_mail-1.4.0/fastapi_mail/connection.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.3.1/fastapi_mail/email_utils/email_check.py` & `fastapi_mail-1.4.0/fastapi_mail/email_utils/email_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Set, Union
 
 import dns.exception
 import dns.resolver
+from email_validator import EmailNotValidError, validate_email
 
 try:
     from redis import asyncio as aioredis
 
     redis_lib = True
 except ImportError:
     redis_lib = False
@@ -15,16 +16,14 @@
 try:
     import httpx
 
     request_lib = True
 except ImportError:
     request_lib = False
 
-from pydantic import EmailStr
-
 from fastapi_mail.errors import ApiError, DBProvaiderError
 
 
 class AbstractEmailChecker(ABC):
     @abstractmethod
     def validate_email(self, email: str) -> bool:
         pass
@@ -164,15 +163,19 @@
             }
             await self.redis_client.hset("temp_domains", mapping=kwargs)
 
         return True
 
     def validate_email(self, email: str) -> bool:
         """Validate email address"""
-        EmailStr.validate(email)
+        try:
+            emailinfo = validate_email(email, check_deliverability=False)
+            email = emailinfo.normalized
+        except EmailNotValidError:
+            raise EmailNotValidError
         return True
 
     async def fetch_temp_email_domains(self) -> Union[List[str], Any]:
         """Async request to source param resource"""
         async with httpx.AsyncClient() as client:
             response = await client.get(self.source)
             if self.redis_enabled:
@@ -366,17 +369,21 @@
             "Response status code is {}, error msg {}".format(
                 response.status_code, response.text
             )
         )
 
     def validate_email(self, email: str) -> bool:
         """Validate email address"""
-        if EmailStr.validate(email):
-            return True
-        return False
+
+        try:
+            emailinfo = validate_email(email, check_deliverability=False)
+            email = emailinfo.normalized
+        except EmailNotValidError:
+            return False
+        return True
 
     def catch_all_check(self) -> bool:
         """
         Tells you whether or not this mail server has a “catch-all” address.
         This refers to a special type of address that can receive emails for any number of
         non-existent email addresses under a particular domain.
         Catch-all addresses are common in businesses where if you send an email to test@hi.com and
```

### Comparing `fastapi_mail-1.3.1/fastapi_mail/errors.py` & `fastapi_mail-1.4.0/fastapi_mail/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.3.1/fastapi_mail/fastmail.py` & `fastapi_mail-1.4.0/fastapi_mail/fastmail.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.3.1/fastapi_mail/msg.py` & `fastapi_mail-1.4.0/fastapi_mail/msg.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.3.1/fastapi_mail/schemas.py` & `fastapi_mail-1.4.0/fastapi_mail/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from enum import Enum
 from io import BytesIO
 from mimetypes import MimeTypes
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, EmailStr, root_validator, validator
+from pydantic import BaseModel, ConfigDict, EmailStr, field_validator, model_validator
 from starlette.datastructures import Headers, UploadFile
 
 from fastapi_mail.errors import WrongFile
 
 
 class MultipartSubtypeEnum(Enum):
     """
@@ -44,15 +44,15 @@
     bcc: List[EmailStr] = []
     reply_to: List[EmailStr] = []
     charset: str = "utf-8"
     subtype: MessageType
     multipart_subtype: MultipartSubtypeEnum = MultipartSubtypeEnum.mixed
     headers: Optional[Dict] = None
 
-    @validator("attachments")
+    @field_validator("attachments")
     def validate_file(cls, v):
         temp = []
         mime = MimeTypes()
 
         for file in v:
             file_meta = None
             if isinstance(file, dict):
@@ -84,21 +84,20 @@
                 temp.append((file, file_meta))
             else:
                 raise WrongFile(
                     "attachments field type incorrect, must be UploadFile or path"
                 )
         return temp
 
-    @root_validator
+    @model_validator(mode="after")
     def validate_alternative_body(cls, values):
         """
         Validate alternative_body field
         """
         if (
-            values["multipart_subtype"] != MultipartSubtypeEnum.alternative
-            and values["alternative_body"]
+            values.multipart_subtype != MultipartSubtypeEnum.alternative
+            and values.alternative_body
         ):
-            values["alternative_body"] = None
+            values.alternative_body = None
         return values
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
```

### Comparing `fastapi_mail-1.3.1/pyproject.toml` & `fastapi_mail-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mail"
-version = "1.3.1"
+version = "1.4.0"
 description = "Simple lightweight mail library for FastApi"
 authors = ["Sabuhi Shukurov <sabuhi.shukurov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sabuhish/fastapi-mail"
 repository = "https://github.com/sabuhish/fastapi-mail"
 classifiers = [
@@ -17,16 +17,17 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"  # flake wants 3.8.1 minimum for some reason
 Jinja2 = "^3.0"
 aiosmtplib = "^2.0"
-pydantic = "^1.8"
-email-validator = "^1.1"
+pydantic = "^2.0"
+pydantic_settings = "^2.0"
+email-validator = "^2.0"
 blinker = "^1.5"
 httpx = {extras = ["httpx"], version = "^0.23", optional = true}
 redis = {extras = ["redis"], version = "^4.3", optional = true}
 starlette = ">=0.24,<1.0"  # caret behaviour on 0.x is to lock to 0.x.*
 
 [tool.poetry.extras]
 httpx = ["httpx"]
@@ -44,15 +45,15 @@
 mypy = "0.971"
 typed-ast = "^1.4"
 regex = "2022.7.9"
 fakeredis = "^2.0"
 httpx = "^0.23"
 redis = "^4.3"
 uvicorn = "^0.20"
-fastapi = "^0.92"
+fastapi = "^0.100"
 types-redis = "^4.3.21"
 flake8 = "^6.0"
 black = "^22.3"
 
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
```

### Comparing `fastapi_mail-1.3.1/PKG-INFO` & `fastapi_mail-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mail
-Version: 1.3.1
+Version: 1.4.0
 Summary: Simple lightweight mail library for FastApi
 Home-page: https://github.com/sabuhish/fastapi-mail
 License: MIT
 Author: Sabuhi Shukurov
 Author-email: sabuhi.shukurov@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Intended Audience :: Developers
@@ -18,17 +18,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: httpx
 Provides-Extra: redis
 Requires-Dist: Jinja2 (>=3.0,<4.0)
 Requires-Dist: aiosmtplib (>=2.0,<3.0)
 Requires-Dist: blinker (>=1.5,<2.0)
-Requires-Dist: email-validator (>=1.1,<2.0)
+Requires-Dist: email-validator (>=2.0,<3.0)
 Requires-Dist: httpx[httpx] (>=0.23,<0.24) ; extra == "httpx"
-Requires-Dist: pydantic (>=1.8,<2.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic_settings (>=2.0,<3.0)
 Requires-Dist: redis[redis] (>=4.3,<5.0) ; extra == "redis"
 Requires-Dist: starlette (>=0.24,<1.0)
 Project-URL: Repository, https://github.com/sabuhish/fastapi-mail
 Description-Content-Type: text/markdown
 
 
 # Fastapi-mail
```

