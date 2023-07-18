# Comparing `tmp/george-agent-package-0.0.3.tar.gz` & `tmp/george-agent-package-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "george-agent-package-0.0.3.tar", last modified: Tue Jul 18 17:42:49 2023, max compression
+gzip compressed data, was "george-agent-package-0.0.4.tar", last modified: Tue Jul 18 18:12:19 2023, max compression
```

## Comparing `george-agent-package-0.0.3.tar` & `george-agent-package-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:42:49.201703 george-agent-package-0.0.3/
--rw-rw-rw-   0        0        0       41 2023-07-18 16:55:30.000000 george-agent-package-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      108 2023-07-18 17:42:49.200688 george-agent-package-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 george-agent-package-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 17:42:49.152376 george-agent-package-0.0.3/george_agent_package/
--rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 george-agent-package-0.0.3/george_agent_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:42:49.186550 george-agent-package-0.0.3/george_agent_package/tools/
--rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 george-agent-package-0.0.3/george_agent_package/tools/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-07-18 16:55:46.000000 george-agent-package-0.0.3/george_agent_package/tools/agent_tool.py
--rw-rw-rw-   0        0        0      738 2023-07-18 16:55:48.000000 george-agent-package-0.0.3/george_agent_package/tools/math_tool_adapter.py
--rw-rw-rw-   0        0        0     1469 2023-07-18 16:55:49.000000 george-agent-package-0.0.3/george_agent_package/tools/mir_tool_adapter.py
--rw-rw-rw-   0        0        0     1071 2023-07-18 16:55:50.000000 george-agent-package-0.0.3/george_agent_package/tools/serp_tool_adapter.py
--rw-rw-rw-   0        0        0     5740 2023-07-18 17:04:21.000000 george-agent-package-0.0.3/george_agent_package/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:42:49.197050 george-agent-package-0.0.3/george_agent_package/yamls/
--rw-rw-rw-   0        0        0      714 2023-07-18 17:41:06.000000 george-agent-package-0.0.3/george_agent_package/yamls/agent_tool.yaml
--rw-rw-rw-   0        0        0      318 2023-07-18 16:55:53.000000 george-agent-package-0.0.3/george_agent_package/yamls/math_tool.yaml
--rw-rw-rw-   0        0        0      471 2023-07-18 17:41:49.000000 george-agent-package-0.0.3/george_agent_package/yamls/mir_tool.yaml
--rw-rw-rw-   0        0        0      318 2023-07-18 16:55:57.000000 george-agent-package-0.0.3/george_agent_package/yamls/serp_tool.yaml
-drwxrwxrwx   0        0        0        0 2023-07-18 17:42:49.171882 george-agent-package-0.0.3/george_agent_package.egg-info/
--rw-rw-rw-   0        0        0      108 2023-07-18 17:42:48.000000 george-agent-package-0.0.3/george_agent_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-07-18 17:42:49.000000 george-agent-package-0.0.3/george_agent_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:42:48.000000 george-agent-package-0.0.3/george_agent_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-18 17:42:48.000000 george-agent-package-0.0.3/george_agent_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-07-18 17:42:48.000000 george-agent-package-0.0.3/george_agent_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:42:49.202700 george-agent-package-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      418 2023-07-18 17:42:09.000000 george-agent-package-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:42:49.198047 george-agent-package-0.0.3/tests/
--rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 george-agent-package-0.0.3/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:19.298683 george-agent-package-0.0.4/
+-rw-rw-rw-   0        0        0       41 2023-07-18 16:55:30.000000 george-agent-package-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      108 2023-07-18 18:12:19.296672 george-agent-package-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:20:54.000000 george-agent-package-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:19.163316 george-agent-package-0.0.4/george_agent_package/
+-rw-rw-rw-   0        0        0       82 2023-07-14 17:20:54.000000 george-agent-package-0.0.4/george_agent_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:19.251710 george-agent-package-0.0.4/george_agent_package/tools/
+-rw-rw-rw-   0        0        0       67 2023-07-14 22:20:33.000000 george-agent-package-0.0.4/george_agent_package/tools/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-07-18 16:55:46.000000 george-agent-package-0.0.4/george_agent_package/tools/agent_tool.py
+-rw-rw-rw-   0        0        0      738 2023-07-18 16:55:48.000000 george-agent-package-0.0.4/george_agent_package/tools/math_tool_adapter.py
+-rw-rw-rw-   0        0        0     1469 2023-07-18 16:55:49.000000 george-agent-package-0.0.4/george_agent_package/tools/mir_tool_adapter.py
+-rw-rw-rw-   0        0        0     1071 2023-07-18 16:55:50.000000 george-agent-package-0.0.4/george_agent_package/tools/serp_tool_adapter.py
+-rw-rw-rw-   0        0        0     6151 2023-07-18 18:11:06.000000 george-agent-package-0.0.4/george_agent_package/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:19.284676 george-agent-package-0.0.4/george_agent_package/yamls/
+-rw-rw-rw-   0        0        0      714 2023-07-18 17:41:06.000000 george-agent-package-0.0.4/george_agent_package/yamls/agent_tool.yaml
+-rw-rw-rw-   0        0        0      318 2023-07-18 16:55:53.000000 george-agent-package-0.0.4/george_agent_package/yamls/math_tool.yaml
+-rw-rw-rw-   0        0        0      471 2023-07-18 17:41:49.000000 george-agent-package-0.0.4/george_agent_package/yamls/mir_tool.yaml
+-rw-rw-rw-   0        0        0      318 2023-07-18 16:55:57.000000 george-agent-package-0.0.4/george_agent_package/yamls/serp_tool.yaml
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:19.192683 george-agent-package-0.0.4/george_agent_package.egg-info/
+-rw-rw-rw-   0        0        0      108 2023-07-18 18:12:18.000000 george-agent-package-0.0.4/george_agent_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-07-18 18:12:19.000000 george-agent-package-0.0.4/george_agent_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:12:18.000000 george-agent-package-0.0.4/george_agent_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-18 18:12:18.000000 george-agent-package-0.0.4/george_agent_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-07-18 18:12:18.000000 george-agent-package-0.0.4/george_agent_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:12:19.298683 george-agent-package-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      418 2023-07-18 18:12:07.000000 george-agent-package-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:19.293672 george-agent-package-0.0.4/tests/
+-rw-rw-rw-   0        0        0      486 2023-07-18 16:55:59.000000 george-agent-package-0.0.4/tests/test_my_tool_1.py
```

### Comparing `george-agent-package-0.0.3/README.md` & `george-agent-package-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.3/george_agent_package/tools/agent_tool.py` & `george-agent-package-0.0.4/george_agent_package/tools/agent_tool.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.3/george_agent_package/tools/math_tool_adapter.py` & `george-agent-package-0.0.4/george_agent_package/tools/math_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.3/george_agent_package/tools/mir_tool_adapter.py` & `george-agent-package-0.0.4/george_agent_package/tools/mir_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.3/george_agent_package/tools/serp_tool_adapter.py` & `george-agent-package-0.0.4/george_agent_package/tools/serp_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.3/george_agent_package/tools/utils.py` & `george-agent-package-0.0.4/george_agent_package/tools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import ssl
 import openai
 from promptflow.connections import (
     AzureOpenAIConnection,
     SerpConnection,
     CustomConnection,
 )
+from langchain import LLMMathChain, SerpAPIWrapper
+from langchain.agents import Tool
 from langchain.chat_models import AzureChatOpenAI
 from serpapi import GoogleSearch
 from langchain.schema import BaseLanguageModel
 
 
 def collect_tools_from_directory(base_dir) -> dict:
     tools = {}
@@ -72,15 +74,22 @@
 
     @staticmethod
     def CreateAgentLLM(config: AzureOpenAIConnection, temperature: float = 0.7, model_name: str = "gpt-35-turbo") -> BaseLanguageModel:
         openai.api_base = config.api_base
         openai.api_type = config.api_type
         openai.api_version = config.api_version
         # todo: parameterize model_name and temperature
-        llm = AzureChatOpenAI(client=openai.ChatCompletion ,temperature= temperature, deployment_name=model_name, model_name=model_name, openai_api_key=config.api_key)
+        llm = AzureChatOpenAI(client=openai.ChatCompletion,
+                              temperature= temperature, 
+                              deployment_name=model_name,
+                              model_name=model_name, 
+                              openai_api_key=config.api_key,
+                              openai_api_base=config.api_base,
+                              openai_api_type=config.api_type,
+                              openai_api_version=config.api_version)
         return llm
     
     @staticmethod
     def CreateToolAdapter(config: ToolConfiguration, llm: BaseLanguageModel):
         if config.tool_type == ToolType.BUILT_IN:
             # Switch case on the NAME property
             if config.name == "serp-api":
```

### Comparing `george-agent-package-0.0.3/george_agent_package/yamls/agent_tool.yaml` & `george-agent-package-0.0.4/george_agent_package/yamls/agent_tool.yaml`

 * *Files identical despite different names*

### Comparing `george-agent-package-0.0.3/george_agent_package.egg-info/SOURCES.txt` & `george-agent-package-0.0.4/george_agent_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

