# Comparing `tmp/dynamic-llm-0.0.5.tar.gz` & `tmp/dynamic-llm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-llm-0.0.5.tar", last modified: Sat Jul 15 14:39:38 2023, max compression
+gzip compressed data, was "dynamic-llm-0.0.6.tar", last modified: Tue Jul 18 18:11:48 2023, max compression
```

## Comparing `dynamic-llm-0.0.5.tar` & `dynamic-llm-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.185987 dynamic-llm-0.0.5/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      655 2023-07-15 14:39:38.185886 dynamic-llm-0.0.5/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)     7836 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/README.md
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.183187 dynamic-llm-0.0.5/dynamic/
--rw-r--r--   0 omarwaseem   (501) staff       (20)       83 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.183671 dynamic-llm-0.0.5/dynamic/classes/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/classes/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1331 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/classes/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/classes/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/classes/logger.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-llm-0.0.5/dynamic/classes/message.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1474 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/decorator.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.184010 dynamic-llm-0.0.5/dynamic/protocols/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/protocols/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)    10232 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/protocols/server.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-llm-0.0.5/dynamic/protocols/ws.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.184109 dynamic-llm-0.0.5/dynamic/request/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/request/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.184182 dynamic-llm-0.0.5/dynamic/response/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/response/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.184552 dynamic-llm-0.0.5/dynamic/router/
--rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/router/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     3851 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/router/file_routes_builder.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/router/get_file_routes.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2552 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/router/router.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.184906 dynamic-llm-0.0.5/dynamic/runners/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-llm-0.0.5/dynamic/runners/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      603 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/callable.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.185313 dynamic-llm-0.0.5/dynamic/runners/langchain/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      174 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/langchain/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1472 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/langchain/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      687 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/langchain/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      202 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/langchain/config.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      316 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/runner.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      847 2023-07-08 22:39:44.000000 dynamic-llm-0.0.5/dynamic/runners/utils.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1378 2023-07-15 14:38:48.000000 dynamic-llm-0.0.5/dynamic/start_server.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.185409 dynamic-llm-0.0.5/dynamic/static/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-llm-0.0.5/dynamic/static/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.185765 dynamic-llm-0.0.5/dynamic_llm.egg-info/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      655 2023-07-15 14:39:38.000000 dynamic-llm-0.0.5/dynamic_llm.egg-info/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)      910 2023-07-15 14:39:38.000000 dynamic-llm-0.0.5/dynamic_llm.egg-info/SOURCES.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-15 14:39:38.000000 dynamic-llm-0.0.5/dynamic_llm.egg-info/dependency_links.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-15 14:39:38.000000 dynamic-llm-0.0.5/dynamic_llm.egg-info/top_level.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)      596 2023-07-15 14:39:20.000000 dynamic-llm-0.0.5/pyproject.toml
--rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-15 14:39:38.186018 dynamic-llm-0.0.5/setup.cfg
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1046 2023-07-15 14:39:16.000000 dynamic-llm-0.0.5/setup.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.817328 dynamic-llm-0.0.6/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      655 2023-07-18 18:11:48.817219 dynamic-llm-0.0.6/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     9150 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/README.md
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.814679 dynamic-llm-0.0.6/dynamic/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       83 2023-07-15 14:38:48.000000 dynamic-llm-0.0.6/dynamic/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.815054 dynamic-llm-0.0.6/dynamic/classes/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/classes/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2260 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/dynamic/classes/dynamic_agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/classes/logger.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-llm-0.0.6/dynamic/classes/message.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1483 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/dynamic/decorator.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.815321 dynamic-llm-0.0.6/dynamic/protocols/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/protocols/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)    10643 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/dynamic/protocols/server.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2165 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/dynamic/protocols/ws.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.815415 dynamic-llm-0.0.6/dynamic/request/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/request/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.815497 dynamic-llm-0.0.6/dynamic/response/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/response/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.815866 dynamic-llm-0.0.6/dynamic/router/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/router/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     3851 2023-07-15 14:38:48.000000 dynamic-llm-0.0.6/dynamic/router/file_routes_builder.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/router/get_file_routes.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2552 2023-07-15 14:38:48.000000 dynamic-llm-0.0.6/dynamic/router/router.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.816217 dynamic-llm-0.0.6/dynamic/runners/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-llm-0.0.6/dynamic/runners/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      603 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/runners/callable.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.816593 dynamic-llm-0.0.6/dynamic/runners/langchain/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      174 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/runners/langchain/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1481 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/dynamic/runners/langchain/agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      687 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/runners/langchain/chain.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      202 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/runners/langchain/config.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      316 2023-07-08 22:39:44.000000 dynamic-llm-0.0.6/dynamic/runners/runner.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      856 2023-07-18 18:07:35.000000 dynamic-llm-0.0.6/dynamic/runners/utils.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1378 2023-07-15 14:38:48.000000 dynamic-llm-0.0.6/dynamic/start_server.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.816688 dynamic-llm-0.0.6/dynamic/static/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-llm-0.0.6/dynamic/static/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-18 18:11:48.817067 dynamic-llm-0.0.6/dynamic_llm.egg-info/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      655 2023-07-18 18:11:48.000000 dynamic-llm-0.0.6/dynamic_llm.egg-info/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      893 2023-07-18 18:11:48.000000 dynamic-llm-0.0.6/dynamic_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-18 18:11:48.000000 dynamic-llm-0.0.6/dynamic_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-18 18:11:48.000000 dynamic-llm-0.0.6/dynamic_llm.egg-info/top_level.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      596 2023-07-18 18:11:29.000000 dynamic-llm-0.0.6/pyproject.toml
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-18 18:11:48.817359 dynamic-llm-0.0.6/setup.cfg
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1046 2023-07-18 18:11:27.000000 dynamic-llm-0.0.6/setup.py
```

### Comparing `dynamic-llm-0.0.5/PKG-INFO` & `dynamic-llm-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-llm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-llm-0.0.5/README.md` & `dynamic-llm-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 
 ## What is Dynamic?
 
 Easy-to-use framework to enable building, deploying, and scaling LLM applications.
 
 ## Table of Contents
 
-1. [Getting Started](#getting-started)
+1. [Getting Started](#1-getting-started)
 
-   a. [Installation](#installation)
+   a. [Installation](#a-installation)
 
-2. [Building Your Application](#building-your-application)
+2. [Building Your Application](#2-building-your-application)
 
-   a. [Dynamic Alpha - what can you do?](#dynamic-alpha---what-can-you-do)
+   a. [Dynamic Alpha - what can you do?](#a-dynamic-alpha---what-can-you-do)
 
-   b. [Project Structure](#project-structure)
+   b. [Project Structure](#b-project-structure)
 
-   c. [Routing](#routing)
+   c. [Routing](#c-routing)
 
-   d. [Callables](#callables)
+   d. [Websockets](#d-websockets)
 
-   e. [Langchain Agents](#langchain-agents)
+3. [Concepts](#3-concepts)
 
-   f. [Langchain Chains](#langchain-chains)
+   a. [LLM Operators](#a-llm-operators)
 
-## Getting Started
+## 1. Getting Started
 
-### Installation
+### a. Installation
 
 With python versions 3.6+, run the following to install the `dynamic` module. It is recommended that you have a virtual environment set up in your project as well before doing this.
 
 ```bash
 pip install dynamic-sh
 ```
 
@@ -58,27 +58,27 @@
 3. **(optional)** Test that the module is functional in your console by running:
 
 ```bash
 $ python -c "import dynamic"
 ```
 -->
 
-## Building Your Application
+## 2. Building Your Application
 
-### Dynamic Alpha - what can you do?
+### a. Dynamic Alpha - what can you do?
 
 As of right now, the following features for an API built on dynamic are available:
 
 1. Simple, normal `GET`, `PUT`, `POST`, and `DELETE` endpoints are represented by a callable function.
 
 2. Given a langchain chain or agent, a simple endpoint will be generated that will return agent/chain output given a prompt.
 
 3. Given an agent, a websocket endpoint can be generated that will stream all of the agent's output in real-time.
 
-### Project Structure
+### b. Project Structure
 
 Typically your root directory should have a server/app script that initiates your server. And then if you opt for file-based routing, a folder named `routes` in which the endpoint logic is stored. More details on routing will be in the next section.
 
 ```bash
 # example file structure tree
 .
 └── my_app/
@@ -97,15 +97,15 @@
     start_server()
 ```
 
 Run with `python app.py`.
 
 Besides these details, the project structure has no other requirements or restrictions.
 
-### Routing
+### c. Routing
 
 There are two routing options, file-based and non file-based routing. Dynamic does not restrict you from using one or the other or both.
 
 #### File-based routing
 
 This is the **recommended** method of routing.
 
@@ -151,15 +151,26 @@
 def handle_all() -> typing.Dict[str, str]:
     return dict(message="handle all")
 
 @dynamic(methods=["DELETE"])
 def delete():
     return dict(message="Ran delete()")
 ```
+```python
+# /example/routes/file_based_agent.py
+
+streaming_agent = DynamicAgent(
+    tool_list=tool_list, llm=llm, agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION, verbose=True,
+)
 
+# this agent will be sitting on the websocket "ws://<host>:<port>/file_based_agent"
+@dynamic(streaming=True)
+def agent():
+    return streaming_agent
+```
 See [the example app](./example/) for more route examples.
 
 #### Non file-based routing
 
 Simply put, these are routes that are manually defined into `start_server`.
 
 ##### Non-streaming/inline
@@ -229,18 +240,18 @@
 ##### Streaming
 
 Setting up a streaming agent is nearly identical, except you must also:
 
 - declare `streaming=True` when defining your langchain llms and dynamic `Route`
 - declare your agent using `DynamicAgent` rather than `initialize_agent`
 
-(**Note**: Langchain yet has streaming support for chains, so for the time being)
+(**Note**: Langchain yet has streaming support for chains, so for the time being only `Agents` are supported)
 
 ```python
-from dynamic.classes.agent import DynamicAgent
+from dynamic.classes.dynamic_agent  import DynamicAgent
 
 llm = OpenAI(temperature=0, verbose=True, streaming=True) # declare llm with streaming
 
 tool_list = ["google-serper"]
 
 # if you want to use streaming over websocket, your agent must be decalared with a DynamicAgent
 streaming_agent = DynamicAgent(
@@ -264,7 +275,39 @@
 ```
 {
     "config": {
         "input": <agent_prompt_here>
     }
 }
 ```
+
+#### d. Websockets
+
+##### Security
+
+Most of the server-side websocket setup is done automatically for you with Dynamic ⚡️ (yay 🎉). The rest, that is client-side, depends on the websocket library/client you use to connect to your Dynamic Websocket. Please be **aware** there is one expectation from Dynamic.
+
+Dynamic expects there to be an acknowledge message sent from the client within 10 seconds of connecting. At the moment, there is no expected format, but as a layer of acknowledged connection and security, there is this expectation, otherwise, your connection will be closed.
+
+Here is a simple example:
+
+```javascript
+var ws = new WebSocket("ws://localhost:8000/agent");
+
+ws.onopen = function(event) {
+    console.log("Sending acknowledge message on connection open...")
+    ws.send("ack msg")
+}
+ws.onmessage = function(event) {
+    ...
+};
+```
+
+## 3. Concepts
+
+### a. LLM Operators
+
+TODO
+
+#### Inline vs Streaming
+
+TODO
```

### Comparing `dynamic-llm-0.0.5/dynamic/classes/message.py` & `dynamic-llm-0.0.6/dynamic/classes/message.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic/decorator.py` & `dynamic-llm-0.0.6/dynamic/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from functools import wraps
 from typing import Callable, List, Optional
 from inspect import iscoroutinefunction
 
-from dynamic.classes.agent import DynamicAgent
+from dynamic.classes.dynamic_agent  import DynamicAgent
 
 def dynamic(
         func: Optional[Callable] = None,
         streaming: bool = False,
         methods: List[str] = ["GET"]
     ):
     """Dynamic wrapper to declare endpoints"""
```

### Comparing `dynamic-llm-0.0.5/dynamic/protocols/server.py` & `dynamic-llm-0.0.6/dynamic/protocols/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from fastapi import FastAPI, WebSocket, WebSocketDisconnect, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.staticfiles import StaticFiles
 from starlette.responses import FileResponse
 import uvicorn
 
 # dynamic
-from dynamic.classes.agent import DynamicAgent
+from dynamic.classes.dynamic_agent  import DynamicAgent
 from dynamic.classes.message import BaseMessage, ErrorMessage, ClientMessage, ServerMessage
 from dynamic.router import Router, Route
 from dynamic.runners.utils import get_runner
-from dynamic.protocols.ws import ConnectionManager
+from dynamic.protocols.ws import ConnectionManager, WebSocketAckTimeoutError
 
 # Exceptions
 class RouteNotFound(Exception):
     pass
 
 parent_dir_path = os.path.dirname(os.path.realpath(__file__))
 
@@ -124,15 +124,14 @@
     async def websocket_handler(self, websocket: WebSocket):
         path = websocket.scope.get("path")
         if path is None:
             raise RouteNotFound("Websocket recieved a request without a path declared.")
         async def handle_msg(recieved_message: ClientMessage) -> Union[ServerMessage, ErrorMessage]:
             logging.info(f"Processing message(id={recieved_message.id}) for route {path}")
             try:
-                # TODO: Remove self.routes and route data
 
                 # build runner and run incoming input
                 route = self.router.get_route(path)
                 if not route:
                     err_message = f"Server's router does not have path, {path}"
                     logging.error(err_message)
                     raise RouteNotFound(err_message)
@@ -141,20 +140,21 @@
                 
                 handle = route.handle
                 runner = route.runner
                 streaming = route.streaming
                 runner_config_type = route.runner_config_type
                 config = runner_config_type(**recieved_message.config)
                 
+                # TODO: Add a seperate try/catch for runner arun
                 output = await runner(handle, config, websocket=websocket, streaming=streaming).arun()
 
                 # return processed message
                 return ServerMessage(content=output)
             except ValueError as e:
-                err_content = f"ERROR: ValueError while processing Message(id={recieved_message.id}) on route path ({path})."
+                err_content = f"ERROR: ValueError while processing {recieved_message.__class__.__name__}(id={recieved_message.id}) on route path ({path}). Message values: {recieved_message.to_dict()}"
                 logging.error(err_content)
                 traceback.print_exc()
                 return ErrorMessage(content=err_content, error=e)
             except Exception as e:
                 err_content = f"ERROR: Unknown Error while processing Message(id={recieved_message.id}) on route path ({path})."
                 logging.error(err_content)
                 traceback.print_exc()
@@ -163,15 +163,20 @@
         async def send_msg(message: BaseMessage, broadcast: bool = False) -> None:
             logging.info(f"Sending message {message.to_json_dump()}")
             if broadcast:
                 await self.connection_manager.broadcast(message)
             else:
                 await self.connection_manager.send_message(websocket, message)
 
-        websocket_id = await self.connection_manager.connect(websocket)
+        
+        try:
+            websocket_id = await self.connection_manager.connect(websocket)
+        except WebSocketAckTimeoutError as e:
+            raise e
+
         while True:
             try:
                 received_json = await websocket.receive_json()
                 incoming_message = ClientMessage(**received_json)
                 logging.info(f"Received message: {incoming_message.to_json_dump()}")
 
                 outgoing_message = await handle_msg(incoming_message)
@@ -224,14 +229,18 @@
                         var ws = new WebSocket("ws://localhost:8000/agent");
                         ws.onmessage = function(event) {
                             var messages = document.getElementById('messages')
                             data = JSON.parse(event.data)
                             var content = document.createTextNode(data.content)
                             messages.appendChild(content)
                         };
+                        ws.onopen = function(event) {
+                            console.log("Sending acknowledge message...")
+                            ws.send("ack msg")
+                        }
                         function sendMessage(event) {
                             var input = document.getElementById("messageText")
                             var content = input.value
                             var config = { input: input.value }
                             var value = { content: content, config: config }
                             ws.send(JSON.stringify(value))
                             input.value = ''
```

### Comparing `dynamic-llm-0.0.5/dynamic/router/file_routes_builder.py` & `dynamic-llm-0.0.6/dynamic/router/file_routes_builder.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic/router/get_file_routes.py` & `dynamic-llm-0.0.6/dynamic/router/get_file_routes.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic/router/router.py` & `dynamic-llm-0.0.6/dynamic/router/router.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic/runners/callable.py` & `dynamic-llm-0.0.6/dynamic/runners/callable.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic/runners/langchain/agent.py` & `dynamic-llm-0.0.6/dynamic/runners/langchain/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from typing import Union, Dict, Optional
 
 from fastapi import WebSocket
 
 # dyanmic
 from dynamic.runners.runner import Runner
-from dynamic.classes.agent import DynamicAgent
+from dynamic.classes.dynamic_agent  import DynamicAgent
 from dynamic.runners.langchain.config import ChainRunnerConfig
 
 # langchain
 from langchain.agents import Agent, AgentExecutor, initialize_agent
 
 
 class AgentRunner(Runner):
```

### Comparing `dynamic-llm-0.0.5/dynamic/runners/langchain/chain.py` & `dynamic-llm-0.0.6/dynamic/runners/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic/runners/utils.py` & `dynamic-llm-0.0.6/dynamic/runners/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Tuple
 
 from dynamic.runners.runner import Runner, RunnerConfig
 from dynamic.runners.callable import CallableRunner, CallableRunnerConfig
 from dynamic.runners.langchain import AgentRunner, ChainRunner, ChainRunnerConfig
-from dynamic.classes.agent import DynamicAgent
+from dynamic.classes.dynamic_agent  import DynamicAgent
 
 from langchain.agents import Agent, AgentExecutor
 from langchain.chains.base import Chain
 
 
 def get_runner(handle: Any) -> Tuple[Runner, RunnerConfig]:
     if isinstance(handle, (Agent, AgentExecutor, DynamicAgent)):
```

### Comparing `dynamic-llm-0.0.5/dynamic/start_server.py` & `dynamic-llm-0.0.6/dynamic/start_server.py`

 * *Files identical despite different names*

### Comparing `dynamic-llm-0.0.5/dynamic_llm.egg-info/PKG-INFO` & `dynamic-llm-0.0.6/dynamic_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-llm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-llm-0.0.5/dynamic_llm.egg-info/SOURCES.txt` & `dynamic-llm-0.0.6/dynamic_llm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 README.md
 pyproject.toml
 setup.py
 dynamic/__init__.py
 dynamic/decorator.py
 dynamic/start_server.py
 dynamic/classes/__init__.py
-dynamic/classes/agent.py
-dynamic/classes/chain.py
+dynamic/classes/dynamic_agent.py
 dynamic/classes/logger.py
 dynamic/classes/message.py
 dynamic/protocols/__init__.py
 dynamic/protocols/server.py
 dynamic/protocols/ws.py
 dynamic/request/__init__.py
 dynamic/response/__init__.py
```

### Comparing `dynamic-llm-0.0.5/pyproject.toml` & `dynamic-llm-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamic-sh"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = [
     "Furqan Rydhan <furqan.rydhan@gmail.com>",
     "Aman Ibrahim <amanmibra@gmail.com>"
 ]
 readme = "README.md"
 keywords = ["llm", "langchain"]
```

### Comparing `dynamic-llm-0.0.5/setup.py` & `dynamic-llm-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 for name in ['dynamic-sh', 'dynamic-llm', 'dynamic-api']:
     setup(
         name=name,
-        version='0.0.5',
+        version='0.0.6',
         description='Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.',
         authors=['Furqan Rydhan <furqan@f.inc>', 'Aman Ibrahim <amanmibra@gmail.com>'],
         author_email='',
         packages=find_packages(),
         install_requires=[
             # List of package dependencies
         ],
```

