# Comparing `tmp/llm-replicate-0.1.tar.gz` & `tmp/llm-replicate-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-replicate-0.1.tar", last modified: Tue Jul 18 04:08:29 2023, max compression
+gzip compressed data, was "llm-replicate-0.2.tar", last modified: Tue Jul 18 19:00:45 2023, max compression
```

## Comparing `llm-replicate-0.1.tar` & `llm-replicate-0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:28.998151 llm-replicate-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-18 04:08:28.998151 llm-replicate-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-18 04:08:14.000000 llm-replicate-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:28.998151 llm-replicate-0.1/llm_replicate/
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:28.998151 llm-replicate-0.1/llm_replicate/vendored_replicate/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-18 04:08:14.000000 llm-replicate-0.1/llm_replicate/vendored_replicate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:28.998151 llm-replicate-0.1/llm_replicate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-18 04:08:28.000000 llm-replicate-0.1/llm_replicate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-18 04:08:28.000000 llm-replicate-0.1/llm_replicate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:08:28.000000 llm-replicate-0.1/llm_replicate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 04:08:28.000000 llm-replicate-0.1/llm_replicate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:08:28.000000 llm-replicate-0.1/llm_replicate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 04:08:28.000000 llm-replicate-0.1/llm_replicate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-18 04:08:14.000000 llm-replicate-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:08:28.998151 llm-replicate-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:28.998151 llm-replicate-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-18 04:08:14.000000 llm-replicate-0.1/tests/test_replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.523337 llm-replicate-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-18 19:00:45.523337 llm-replicate-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-18 19:00:24.000000 llm-replicate-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.519337 llm-replicate-0.2/llm_replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.519337 llm-replicate-0.2/llm_replicate/vendored_replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.519337 llm-replicate-0.2/llm_replicate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-18 19:00:24.000000 llm-replicate-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:00:45.523337 llm-replicate-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.523337 llm-replicate-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-18 19:00:24.000000 llm-replicate-0.2/tests/test_replicate.py
```

### Comparing `llm-replicate-0.1/llm_replicate/__init__.py` & `llm-replicate-0.2/llm_replicate/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,24 +34,29 @@
         models = response.json()["models"]
         json_path = config_dir() / "fetch-models.json"
         with open(json_path, "w") as fp:
             json.dump(models, fp, indent=2)
 
     @replicate.command(name="add")
     @click.argument("model_id")
+    @click.option("--chat", is_flag=True, help="This is a chat model")
     @click.option("aliases", "--alias", multiple=True, help="Aliases for this model")
     @click.option("--version", help="Model version (defaults to latest)")
     @click.option("--key", "-k", help="Replicate API key")
-    def add_model(model_id, aliases, version, key):
+    def add_model(model_id, chat, aliases, version, key):
         """
         Register additional Replicate models with LLM
 
         Example usage:
 
             llm replicate add joehoover/falcon-40b-instruct
+
+        \b
+        Use --chat for "chat" models that should be prompted using
+        'User: ... \\nAssistant:' format.
         """
         if not version:
             # Fetch latest version from Replicate API
             token = llm.get_key(key, "replicate", env_var="REPLICATE_API_TOKEN")
             if not token:
                 raise click.ClickException(
                     "Pass --key, store a 'replicate' key or set the REPLICATE_API_TOKEN environment variable."
@@ -68,23 +73,25 @@
             version = model_details["latest_version"]["id"]
         # Add to models.json
         models_path = config_dir() / "models.json"
         if models_path.exists():
             models = json.loads(models_path.read_text())
         else:
             models = []
-        models.append(
-            {
-                "model": model_id,
-                "model_id": model_id.replace("/", "-"),
-                "version": version,
-                "aliases": aliases,
-            }
-        )
-        models_path.write_text(json.dumps(models, indent=2))
+        new_model = {
+            "model": model_id,
+            "model_id": model_id.replace("/", "-"),
+            "version": version,
+            "aliases": aliases,
+        }
+        if chat:
+            new_model["chat"] = True
+        updated_models = [model for model in models if model["model"] != model_id]
+        updated_models.append(new_model)
+        models_path.write_text(json.dumps(updated_models, indent=2))
 
     @replicate.command(name="edit-models")
     def edit_models():
         """
         Edit registered models using the default $EDITOR
         """
         models_path = config_dir() / "models.json"
@@ -101,59 +108,92 @@
         models = json.loads(fetch_models_path.read_text())
         for details in models:
             register(
                 ReplicateModel(
                     owner=details["owner"],
                     name=details["name"],
                     version_id=details["latest_version"]["id"],
+                    chat=False,
                 ),
             )
 
     models_path = config_dir() / "models.json"
     if models_path.exists():
         more_models = json.loads(models_path.read_text())
         for info in more_models:
             aliases = info.get("aliases", [])
             register(
                 ReplicateModel(
                     owner=info["model"].split("/")[0],
                     name=info["model"].split("/")[1],
                     version_id=info["version"],
+                    chat=info.get("chat", False),
                 ),
                 aliases=aliases,
             )
 
 
 class ReplicateModel(llm.Model):
     model_id = "replicate"
     needs_key = "replicate"
     key_env_var = "REPLICATE_API_TOKEN"
 
-    def __init__(self, owner, name, version_id):
+    def __init__(self, owner, name, version_id, chat):
         model_id = "replicate-{}-{}".format(owner, name)
         if model_id.startswith("replicate-replicate-"):
             model_id = model_id[len("replicate-") :]
         self.model_id = model_id
         self.version_id = version_id
         self.name = name
         self.owner = owner
+        self.chat = chat
+
+    def build_chat_prompt(self, prompt, conversation):
+        prompt_lines = []
+        if conversation is not None:
+            for prev_response in conversation.responses:
+                prompt_lines.extend(
+                    [
+                        f"User: {prev_response.prompt.prompt}\n",
+                        f"Assistant: {prev_response.text()}\n",
+                    ]
+                )
+
+        prompt_lines.extend(
+            [
+                f"User: {prompt.prompt}\n",
+                f"Assistant:",
+            ]
+        )
+        return prompt_lines
 
     def execute(self, prompt, stream, response, conversation):
         from . import vendored_replicate
 
+        if conversation and not self.chat:
+            raise llm.ModelError("Conversation mode is not supported")
+
+        lines = [prompt.prompt]
+        if self.chat:
+            lines = self.build_chat_prompt(prompt, conversation)
+
         client = vendored_replicate.Client(api_token=self.get_key())
         output = client.run(
             "{owner}/{name}:{version_id}".format(
                 owner=self.owner,
                 name=self.name,
                 version_id=self.version_id,
             ),
-            input={"prompt": prompt.prompt},
+            input={"prompt": "".join(lines)},
         )
+        response._prompt_json = {"lines": lines}
         yield from output
 
+    def __str__(self) -> str:
+        return "Replicate{}: {}".format(" (chat)" if self.chat else "", self.model_id)
+
 
 def config_dir():
     dir_path = llm.user_dir() / "replicate"
     if not dir_path.exists():
         dir_path.mkdir()
     return dir_path
```

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/base_model.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/base_model.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/client.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                 pass
             raise ReplicateError(f"HTTP error: {resp.status_code, resp.reason}")
         return resp
 
     def _headers(self) -> Dict[str, str]:
         return {
             "Authorization": f"Token {self._api_token()}",
-            "User-Agent": f"replicate-python/0.8.4",
+            "User-Agent": "replicate-python/0.8.4",
         }
 
     def _api_token(self) -> str:
         token = self.api_token
         # Evaluate lazily in case environment variable is set with dotenv, or something
         if token is None:
             token = os.environ.get("REPLICATE_API_TOKEN")
```

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/collection.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/collection.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/files.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/files.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/json.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/json.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/model.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/model.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/prediction.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/prediction.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/schema.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/schema.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/training.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/training.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate/vendored_replicate/version.py` & `llm-replicate-0.2/llm_replicate/vendored_replicate/version.py`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/llm_replicate.egg-info/SOURCES.txt` & `llm-replicate-0.2/llm_replicate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-replicate-0.1/pyproject.toml` & `llm-replicate-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "llm-replicate"
-version = "0.1"
+version = "0.2"
 description = "LLM plugin for models hosted on Replicate"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "llm",
+    "requests-mock",
     # vendored_replicate:
     "requests",
     "packaging"
 ]
 requires-python = ">3.7"
 
 [project.optional-dependencies]
@@ -21,8 +22,8 @@
 
 [project.urls]
 Homepage = "https://github.com/simonw/llm-replicate"
 Changelog = "https://github.com/simonw/llm-replicate/releases"
 Issues = "https://github.com/simonw/llm-replicate/issues"
 
 [project.entry-points.llm]
-replicate = "llm_replicate"
+replicate = "llm_replicate"
```

