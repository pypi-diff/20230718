# Comparing `tmp/george-agent-package-0.0.1.tar.gz` & `tmp/george-agent-package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "george-agent-package-0.0.1.tar", last modified: Tue Jul 18 16:59:23 2023, max compression
+gzip compressed data, was "george-agent-package-0.0.2.tar", last modified: Tue Jul 18 17:05:46 2023, max compression
```

## Comparing `george-agent-package-0.0.1.tar` & `george-agent-package-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 16:59:23.488733 george-agent-package-0.0.1/
--rw-rw-rw-   0        0        0       41 2023-07-18 16:55:30.000000 george-agent-package-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      108 2023-07-18 16:59:23.487730 george-agent-package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 george-agent-package-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 16:59:23.430585 george-agent-package-0.0.1/george_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 george-agent-package-0.0.1/george_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:59:23.479730 george-agent-package-0.0.1/george_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 george-agent-package-0.0.1/george_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-07-18 16:55:46.000000 george-agent-package-0.0.1/george_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0      738 2023-07-18 16:55:48.000000 george-agent-package-0.0.1/george_agent_package/tools/math_tool_adapter.py
--rw-rw-rw-   0        0        0     1469 2023-07-18 16:55:49.000000 george-agent-package-0.0.1/george_agent_package/tools/mir_tool_adapter.py
--rw-rw-rw-   0        0        0     1071 2023-07-18 16:55:50.000000 george-agent-package-0.0.1/george_agent_package/tools/serp_tool_adapter.py
--rw-rw-rw-   0        0        0     5814 2023-07-18 16:56:59.000000 george-agent-package-0.0.1/george_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:59:23.483732 george-agent-package-0.0.1/george_agent_package/yamls/
--rw-rw-rw-   0        0        0      653 2023-07-18 16:55:52.000000 george-agent-package-0.0.1/george_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      318 2023-07-18 16:55:53.000000 george-agent-package-0.0.1/george_agent_package/yamls/math_tool.yaml
--rw-rw-rw-   0        0        0      415 2023-07-18 16:55:55.000000 george-agent-package-0.0.1/george_agent_package/yamls/mir_tool.yaml
--rw-rw-rw-   0        0        0      318 2023-07-18 16:55:57.000000 george-agent-package-0.0.1/george_agent_package/yamls/serp_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-07-18 16:59:23.467133 george-agent-package-0.0.1/george_agent_package.egg-info/
--rw-rw-rw-   0        0        0      108 2023-07-18 16:59:23.000000 george-agent-package-0.0.1/george_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-07-18 16:59:23.000000 george-agent-package-0.0.1/george_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 16:59:23.000000 george-agent-package-0.0.1/george_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-18 16:59:23.000000 george-agent-package-0.0.1/george_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-07-18 16:59:23.000000 george-agent-package-0.0.1/george_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 16:59:23.488733 george-agent-package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      418 2023-07-18 16:59:16.000000 george-agent-package-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:59:23.484732 george-agent-package-0.0.1/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 george-agent-package-0.0.1/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:05:46.949259 george-agent-package-0.0.2/
+-rw-rw-rw-   0        0        0       41 2023-07-18 16:55:30.000000 george-agent-package-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      108 2023-07-18 17:05:46.948260 george-agent-package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 george-agent-package-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:05:46.901976 george-agent-package-0.0.2/george_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 george-agent-package-0.0.2/george_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:05:46.939261 george-agent-package-0.0.2/george_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 george-agent-package-0.0.2/george_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-07-18 16:55:46.000000 george-agent-package-0.0.2/george_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0      738 2023-07-18 16:55:48.000000 george-agent-package-0.0.2/george_agent_package/tools/math_tool_adapter.py
+-rw-rw-rw-   0        0        0     1469 2023-07-18 16:55:49.000000 george-agent-package-0.0.2/george_agent_package/tools/mir_tool_adapter.py
+-rw-rw-rw-   0        0        0     1071 2023-07-18 16:55:50.000000 george-agent-package-0.0.2/george_agent_package/tools/serp_tool_adapter.py
+-rw-rw-rw-   0        0        0     5740 2023-07-18 17:04:21.000000 george-agent-package-0.0.2/george_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:05:46.944262 george-agent-package-0.0.2/george_agent_package/yamls/
+-rw-rw-rw-   0        0        0      653 2023-07-18 16:55:52.000000 george-agent-package-0.0.2/george_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      318 2023-07-18 16:55:53.000000 george-agent-package-0.0.2/george_agent_package/yamls/math_tool.yaml
+-rw-rw-rw-   0        0        0      415 2023-07-18 16:55:55.000000 george-agent-package-0.0.2/george_agent_package/yamls/mir_tool.yaml
+-rw-rw-rw-   0        0        0      318 2023-07-18 16:55:57.000000 george-agent-package-0.0.2/george_agent_package/yamls/serp_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-07-18 17:05:46.930263 george-agent-package-0.0.2/george_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      108 2023-07-18 17:05:46.000000 george-agent-package-0.0.2/george_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-07-18 17:05:46.000000 george-agent-package-0.0.2/george_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:05:46.000000 george-agent-package-0.0.2/george_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-18 17:05:46.000000 george-agent-package-0.0.2/george_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-07-18 17:05:46.000000 george-agent-package-0.0.2/george_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:05:46.950261 george-agent-package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      418 2023-07-18 17:05:30.000000 george-agent-package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:05:46.947264 george-agent-package-0.0.2/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 george-agent-package-0.0.2/tests/test_my_tool_1.py
```

### Comparing `george-agent-package-0.0.1/README.md` & `george-agent-package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.1/george_agent_package/tools/agent_tool.py` & `george-agent-package-0.0.2/george_agent_package/tools/agent_tool.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.1/george_agent_package/tools/math_tool_adapter.py` & `george-agent-package-0.0.2/george_agent_package/tools/math_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.1/george_agent_package/tools/mir_tool_adapter.py` & `george-agent-package-0.0.2/george_agent_package/tools/mir_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.1/george_agent_package/tools/serp_tool_adapter.py` & `george-agent-package-0.0.2/george_agent_package/tools/serp_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.1/george_agent_package/tools/utils.py` & `george-agent-package-0.0.2/george_agent_package/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 from enum import Enum
 from typing import Optional
 from promptflow.connections import CustomConnection, SerpConnection
 import urllib.error
 import json
 import ssl
-from promptflow.contracts.tool_config import ToolConfiguration, ToolType
 import openai
 from promptflow.connections import (
     AzureOpenAIConnection,
     SerpConnection,
     CustomConnection,
 )
 from langchain.chat_models import AzureChatOpenAI
```

### Comparing `george-agent-package-0.0.1/george_agent_package/yamls/agent_tool.yaml` & `george-agent-package-0.0.2/george_agent_package/yamls/agent_tool.yaml`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.1/george_agent_package.egg-info/SOURCES.txt` & `george-agent-package-0.0.2/george_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

