# Comparing `tmp/jupyter_on_golem-0.1.2.tar.gz` & `tmp/jupyter_on_golem-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_on_golem-0.1.2.tar", max compression
+gzip compressed data, was "jupyter_on_golem-0.1.3.tar", max compression
```

## Comparing `jupyter_on_golem-0.1.2.tar` & `jupyter_on_golem-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-14 12:00:18.341898 jupyter_on_golem-0.1.2/LICENSE
--rw-r--r--   0        0        0    13354 2023-07-14 12:00:18.341898 jupyter_on_golem-0.1.2/README.md
--rw-r--r--   0        0        0       73 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/__init__.py
--rw-r--r--   0        0        0     1283 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/__main__.py
--rw-r--r--   0        0        0    24507 2023-07-14 12:00:49.994194 jupyter_on_golem-0.1.2/jupyter_on_golem/golem.py
--rw-r--r--   0        0        0     2597 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/golem_kernel.py
--rw-r--r--   0        0        0      782 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/manifest.json
--rw-r--r--   0        0        0     3700 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/remote_python.py
--rw-r--r--   0        0        0      754 2023-07-14 12:00:40.830109 jupyter_on_golem-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14430 1970-01-01 00:00:00.000000 jupyter_on_golem-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-13 11:20:06.802724 jupyter_on_golem-0.1.3/LICENSE
+-rw-r--r--   0        0        0    13982 2023-07-18 18:48:18.449689 jupyter_on_golem-0.1.3/README.md
+-rw-r--r--   0        0        0       73 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.3/jupyter_on_golem/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.3/jupyter_on_golem/__main__.py
+-rw-r--r--   0        0        0    24507 2023-07-18 18:48:44.977606 jupyter_on_golem-0.1.3/jupyter_on_golem/golem.py
+-rw-r--r--   0        0        0     2597 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.3/jupyter_on_golem/golem_kernel.py
+-rw-r--r--   0        0        0      782 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.3/jupyter_on_golem/manifest.json
+-rw-r--r--   0        0        0     3700 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.3/jupyter_on_golem/remote_python.py
+-rw-r--r--   0        0        0      750 2023-07-18 18:49:13.857518 jupyter_on_golem-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    15054 1970-01-01 00:00:00.000000 jupyter_on_golem-0.1.3/PKG-INFO
```

### Comparing `jupyter_on_golem-0.1.2/LICENSE` & `jupyter_on_golem-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.2/README.md` & `jupyter_on_golem-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Jupyter on Golem - Python Kernel
 
 ## About
 
-Jupyter on Golem is a JupyterLab Python kernel (https://jupyterlab.readthedocs.io), which enables you to run your Python Notebooks using resources available on decentralized Golem Network (https://www.golem.network/). Providers of such resources are compensated for their work with GLM tokens.
+Jupyter on Golem is a Python kernel, which integrates with JupyterLab (https://jupyterlab.readthedocs.io) and enables it to run your Python Notebooks using resources available on decentralized Golem Network (https://www.golem.network/). Providers of such resources are compensated for their work with GLM tokens.
 
 JupyterLab is an open-source project that is widely used by data scientists, analysts, researchers and developers. It allows you to create and share Notebooks - documents that combine code, equations, visualisations and narrative text. JupyterLab is part of Project Jupyter, umbrella project born from IPython Project (https://ipython.org/) and centered around providing tools for interactive computing with computational notebooks. Find more about Jupyter Project: https://jupyter.org/
 
 **Simplified view on JupyterLab:**
 
 ![Simplified Diagram of a JupyterLab flow](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/jupyterlab.png)
 
@@ -225,13 +225,25 @@
 ## Feedback
 
 Did You try Jupyter on Golem? We would love to get to know your thoughts! Please give us your feedback [HERE](https://qkjx8blh5hm.typeform.com/JoGfeedback)
 
 ## Support
 
 If you experience problems with Jupyter on Golem, You can try to get some help in the following places:
-* **jupyter-on-golem** channel on our Golem Network [Discord Server](https://chat.golem.network/)
+* **jupyter-on-golem-discussion** channel on our Golem Network [Discord Server](https://chat.golem.network/)
 * [Github Repository](https://github.com/golemfactory/golem-kernel-python) of the project
 
+## Known Issues
+
+Below You will find list of known issues and potential solutions:
+
+### 1. Unsuccessful funding on Goerli Testnet:
+
+Sometimes after using `%fund goerli` command, You will get **"Funding failed"** output. It might happen due to delay between requesting tETH and tGLM by Jupyter on Golem. In most cases, it should be enough to just wait a few minutes. Afterwards, type `%status` command and You should be able to see that both tETH and tGLM have arrieved to Your wallet.
+
 ## Terms and Conditions
 
-By using Jupyter on Golem you agree to be bound by the terms described in Golem Network [Disclaimer](https://www.golem.network/disclaimer), [User Interaction Guidelines](https://www.golem.network/uig) and [Privacy Policy](https://www.golem.network/privacy).
+By using Jupyter on Golem you agree to be bound by the terms described in Golem Network [Disclaimer](https://www.golem.network/disclaimer), [User Interaction Guidelines](https://www.golem.network/uig) and [Privacy Policy](https://www.golem.network/privacy).
+
+## Legal Statements
+
+“Jupyter” and the Jupyter logos are trademarks or registered trademarks of NumFOCUS.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jupyter_on_golem-0.1.2/jupyter_on_golem/__main__.py` & `jupyter_on_golem-0.1.3/jupyter_on_golem/__main__.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.2/jupyter_on_golem/golem.py` & `jupyter_on_golem-0.1.3/jupyter_on_golem/golem.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 '''
 
 HELP_TEMPLATE = '''\
      _                   _                             ____       _                
     | |_   _ _ __  _   _| |_ ___ _ __    ___  _ __    / ___| ___ | | ___ _ __ ___  
  _  | | | | | '_ \| | | | __/ _ \ '__|  / _ \| '_ \  | |  _ / _ \| |/ _ \ '_ ` _ \ 
 | |_| | |_| | |_) | |_| | ||  __/ |    | (_) | | | | | |_| | (_) | |  __/ | | | | |
- \___/ \__,_| .__/ \__, |\__\___|_|     \___/|_| |_|  \____|\___/|_|\___|_| |_| |_| version: 0.1.2
+ \___/ \__,_| .__/ \__, |\__\___|_|     \___/|_| |_|  \____|\___/|_|\___|_| |_| |_| version: 0.1.3
             |_|    |___/                                                           
 
 Easy to use tool to run Your Jupyter Notebooks on the Golem Network!
 
 COMMANDS:    
     %status		Shows current status of Jupyter on Golem
     %fund		Requests for testnet funds, e.g. '%fund goerli'
```

### Comparing `jupyter_on_golem-0.1.2/jupyter_on_golem/golem_kernel.py` & `jupyter_on_golem-0.1.3/jupyter_on_golem/golem_kernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.2/jupyter_on_golem/manifest.json` & `jupyter_on_golem-0.1.3/jupyter_on_golem/manifest.json`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.2/jupyter_on_golem/remote_python.py` & `jupyter_on_golem-0.1.3/jupyter_on_golem/remote_python.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.2/pyproject.toml` & `jupyter_on_golem-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "jupyter-on-golem"
-version = "0.1.2"
+version = "0.1.3"
 description = "Jupyter Python kernel running on Golem network (https://www.golem.network/)"
 readme = "README.md"
-authors = ["GolemFactory <contact.jupyter@golem.network>"]
+authors = ["GolemFactory <contact.jog@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Distributed Computing"
 ]
```

### Comparing `jupyter_on_golem-0.1.2/PKG-INFO` & `jupyter_on_golem-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jupyter-on-golem
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jupyter Python kernel running on Golem network (https://www.golem.network/)
 License: LGPL-3.0-or-later
 Keywords: golem,jupyter,kernel,notebook
 Author: GolemFactory
-Author-email: contact.jupyter@golem.network
+Author-email: contact.jog@golem.network
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +24,15 @@
 Requires-Dist: websockets (==10.*)
 Description-Content-Type: text/markdown
 
 # Jupyter on Golem - Python Kernel
 
 ## About
 
-Jupyter on Golem is a JupyterLab Python kernel (https://jupyterlab.readthedocs.io), which enables you to run your Python Notebooks using resources available on decentralized Golem Network (https://www.golem.network/). Providers of such resources are compensated for their work with GLM tokens.
+Jupyter on Golem is a Python kernel, which integrates with JupyterLab (https://jupyterlab.readthedocs.io) and enables it to run your Python Notebooks using resources available on decentralized Golem Network (https://www.golem.network/). Providers of such resources are compensated for their work with GLM tokens.
 
 JupyterLab is an open-source project that is widely used by data scientists, analysts, researchers and developers. It allows you to create and share Notebooks - documents that combine code, equations, visualisations and narrative text. JupyterLab is part of Project Jupyter, umbrella project born from IPython Project (https://ipython.org/) and centered around providing tools for interactive computing with computational notebooks. Find more about Jupyter Project: https://jupyter.org/
 
 **Simplified view on JupyterLab:**
 
 ![Simplified Diagram of a JupyterLab flow](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/jupyterlab.png)
 
@@ -251,13 +251,26 @@
 ## Feedback
 
 Did You try Jupyter on Golem? We would love to get to know your thoughts! Please give us your feedback [HERE](https://qkjx8blh5hm.typeform.com/JoGfeedback)
 
 ## Support
 
 If you experience problems with Jupyter on Golem, You can try to get some help in the following places:
-* **jupyter-on-golem** channel on our Golem Network [Discord Server](https://chat.golem.network/)
+* **jupyter-on-golem-discussion** channel on our Golem Network [Discord Server](https://chat.golem.network/)
 * [Github Repository](https://github.com/golemfactory/golem-kernel-python) of the project
 
+## Known Issues
+
+Below You will find list of known issues and potential solutions:
+
+### 1. Unsuccessful funding on Goerli Testnet:
+
+Sometimes after using `%fund goerli` command, You will get **"Funding failed"** output. It might happen due to delay between requesting tETH and tGLM by Jupyter on Golem. In most cases, it should be enough to just wait a few minutes. Afterwards, type `%status` command and You should be able to see that both tETH and tGLM have arrieved to Your wallet.
+
 ## Terms and Conditions
 
 By using Jupyter on Golem you agree to be bound by the terms described in Golem Network [Disclaimer](https://www.golem.network/disclaimer), [User Interaction Guidelines](https://www.golem.network/uig) and [Privacy Policy](https://www.golem.network/privacy).
+
+## Legal Statements
+
+“Jupyter” and the Jupyter logos are trademarks or registered trademarks of NumFOCUS.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

