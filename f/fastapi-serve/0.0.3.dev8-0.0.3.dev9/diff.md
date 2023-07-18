# Comparing `tmp/fastapi-serve-0.0.3.dev8.tar.gz` & `tmp/fastapi-serve-0.0.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.3.dev8.tar", last modified: Tue Jul 18 05:28:59 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.3.dev9.tar", last modified: Tue Jul 18 05:55:59 2023, max compression
```

## Comparing `fastapi-serve-0.0.3.dev8.tar` & `fastapi-serve-0.0.3.dev9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.127293 fastapi-serve-0.0.3.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-18 05:28:59.127293 fastapi-serve-0.0.3.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.123293 fastapi-serve-0.0.3.dev8/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 05:28:58.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.123293 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.123293 fastapi-serve-0.0.3.dev8/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.123293 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.123293 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:28:59.123293 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 05:28:59.000000 fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:28:59.127293 fastapi-serve-0.0.3.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 05:28:55.000000 fastapi-serve-0.0.3.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/setup.py
```

### Comparing `fastapi-serve-0.0.3.dev8/LICENSE` & `fastapi-serve-0.0.3.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/PKG-INFO` & `fastapi-serve-0.0.3.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.3.dev8
+Version: 0.0.3.dev9
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -71,18 +71,19 @@
 
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
 We have a few examples to help you get acquainted with `fastapi-serve`:
 
-- 🚀 [Deploy a Simple FastAPI Application](examples/simple/)
-- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/)
-- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/authorization/)
-- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](examples/file_handling/)
+- 🚀 [Deploy a Simple FastAPI Application](docs/simple/)
+- 💹 Auto-scaling endpoints based on RPS, CPU, and Memory (Coming Soon!)
+- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
+- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
+- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
 - 🐳 Deployment with Custom Dockerfile (Coming Soon!)
 - 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
 
 
 ## 🖥️ `fastapi-serve` CLI 
 
 `fastapi-serve` comes with a simple CLI that allows you to deploy your FastAPI applications to the cloud with ease.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev8 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev9 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -39,34 +39,35 @@
 Hosting**: Export your app for self-hosting with ease, including docker-compose
 and Kubernetes yamls. ## ð¡ Getting Started First, install the `fastapi-
 serve` package using pip: ```bash pip install fastapi-serve ``` Then, simply
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
 deployed application along with the Swagger UI. ## ð Documentation We have a
 few examples to help you get acquainted with `fastapi-serve`: - ð [Deploy a
-Simple FastAPI Application](examples/simple/) - ðï¸ [Use Secrets for Redis-
-Powered Rate Limiting](examples/rate_limit/) - ð [Secure Your Endpoints with
-built-in OAuth2.0 Authorization](examples/authorization/) - ð [Handle File
-Uploads and Downloads with built-in Blob Storage](examples/file_handling/) -
-ð³ Deployment with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App
-for Self-Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸
-`fastapi-serve` CLI `fastapi-serve` comes with a simple CLI that allows you to
-deploy your FastAPI applications to the cloud with ease. | Description |
-Command | | --- | ---: | | Deploy your app locally | `fastapi-serve deploy
-local app:app` | | Deploy your app on JCloud | `fastapi-serve deploy jcloud
-app:app` | | Update existing app on JCloud | `fastapi-serve deploy jcloud app:
-app --app-id ` | | Get app status on JCloud | `fastapi-serve status ` | | List
-all apps on JCloud | `fastapi-serve list` | | Remove app on JCloud | `fastapi-
-serve remove ` | ## âï¸ð° Configuration and Pricing Read our
-[Configuration & Pricing Guide](examples/CONFIG.MD) to learn more about the
-various configuration options available to you and the pricing model for
-`fastapi-serve`. ## ðª Support If you encounter any problems or have
-questions, feel free to open an issue on the GitHub repository. You can also
-join our [Discord](https://discord.jina.ai/) to get help from our community
-members and the Jina team. ## Our Cloud Platform ð `cloud.jina.ai` is our
-robust and scalable cloud platform designed to run your FastAPI applications
-with minimum hassle and maximum efficiency. With features like auto-scaling,
-integrated observability, and automated containerization, it provides a
-seamless and worry-free deployment experience. --- `fastapi-serve` is more than
-just a deployment tool, it's a bridge that connects your local development
-environment with our powerful cloud infrastructure. Start using `fastapi-serve`
-today, and experience the joy of effortless deployments! ð
+Simple FastAPI Application](docs/simple/) - ð¹ Auto-scaling endpoints based
+on RPS, CPU, and Memory (Coming Soon!) - ðï¸ [Use Secrets for Redis-Powered
+Rate Limiting](docs/rate_limit/) - ð [Secure Your Endpoints with built-in
+OAuth2.0 Authorization](docs/authorization/) - ð [Handle File Uploads and
+Downloads with built-in Blob Storage](docs/file_handling/) - ð³ Deployment
+with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-
+Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸ `fastapi-
+serve` CLI `fastapi-serve` comes with a simple CLI that allows you to deploy
+your FastAPI applications to the cloud with ease. | Description | Command | | -
+-- | ---: | | Deploy your app locally | `fastapi-serve deploy local app:app` |
+| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` | | Update
+existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id ` | |
+Get app status on JCloud | `fastapi-serve status ` | | List all apps on JCloud
+| `fastapi-serve list` | | Remove app on JCloud | `fastapi-serve remove ` | ##
+âï¸ð° Configuration and Pricing Read our [Configuration & Pricing Guide]
+(examples/CONFIG.MD) to learn more about the various configuration options
+available to you and the pricing model for `fastapi-serve`. ## ðª Support If
+you encounter any problems or have questions, feel free to open an issue on the
+GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
+get help from our community members and the Jina team. ## Our Cloud Platform
+ð `cloud.jina.ai` is our robust and scalable cloud platform designed to run
+your FastAPI applications with minimum hassle and maximum efficiency. With
+features like auto-scaling, integrated observability, and automated
+containerization, it provides a seamless and worry-free deployment experience.
+--- `fastapi-serve` is more than just a deployment tool, it's a bridge that
+connects your local development environment with our powerful cloud
+infrastructure. Start using `fastapi-serve` today, and experience the joy of
+effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.3.dev8/README.md` & `fastapi-serve-0.0.3.dev9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
 We have a few examples to help you get acquainted with `fastapi-serve`:
 
-- 🚀 [Deploy a Simple FastAPI Application](examples/simple/)
-- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/)
-- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/authorization/)
-- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](examples/file_handling/)
+- 🚀 [Deploy a Simple FastAPI Application](docs/simple/)
+- 💹 Auto-scaling endpoints based on RPS, CPU, and Memory (Coming Soon!)
+- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
+- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
+- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
 - 🐳 Deployment with Custom Dockerfile (Coming Soon!)
 - 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
 
 
 ## 🖥️ `fastapi-serve` CLI 
 
 `fastapi-serve` comes with a simple CLI that allows you to deploy your FastAPI applications to the cloud with ease.
```

#### html2text {}

```diff
@@ -22,34 +22,35 @@
 Hosting**: Export your app for self-hosting with ease, including docker-compose
 and Kubernetes yamls. ## ð¡ Getting Started First, install the `fastapi-
 serve` package using pip: ```bash pip install fastapi-serve ``` Then, simply
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
 deployed application along with the Swagger UI. ## ð Documentation We have a
 few examples to help you get acquainted with `fastapi-serve`: - ð [Deploy a
-Simple FastAPI Application](examples/simple/) - ðï¸ [Use Secrets for Redis-
-Powered Rate Limiting](examples/rate_limit/) - ð [Secure Your Endpoints with
-built-in OAuth2.0 Authorization](examples/authorization/) - ð [Handle File
-Uploads and Downloads with built-in Blob Storage](examples/file_handling/) -
-ð³ Deployment with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App
-for Self-Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸
-`fastapi-serve` CLI `fastapi-serve` comes with a simple CLI that allows you to
-deploy your FastAPI applications to the cloud with ease. | Description |
-Command | | --- | ---: | | Deploy your app locally | `fastapi-serve deploy
-local app:app` | | Deploy your app on JCloud | `fastapi-serve deploy jcloud
-app:app` | | Update existing app on JCloud | `fastapi-serve deploy jcloud app:
-app --app-id ` | | Get app status on JCloud | `fastapi-serve status ` | | List
-all apps on JCloud | `fastapi-serve list` | | Remove app on JCloud | `fastapi-
-serve remove ` | ## âï¸ð° Configuration and Pricing Read our
-[Configuration & Pricing Guide](examples/CONFIG.MD) to learn more about the
-various configuration options available to you and the pricing model for
-`fastapi-serve`. ## ðª Support If you encounter any problems or have
-questions, feel free to open an issue on the GitHub repository. You can also
-join our [Discord](https://discord.jina.ai/) to get help from our community
-members and the Jina team. ## Our Cloud Platform ð `cloud.jina.ai` is our
-robust and scalable cloud platform designed to run your FastAPI applications
-with minimum hassle and maximum efficiency. With features like auto-scaling,
-integrated observability, and automated containerization, it provides a
-seamless and worry-free deployment experience. --- `fastapi-serve` is more than
-just a deployment tool, it's a bridge that connects your local development
-environment with our powerful cloud infrastructure. Start using `fastapi-serve`
-today, and experience the joy of effortless deployments! ð
+Simple FastAPI Application](docs/simple/) - ð¹ Auto-scaling endpoints based
+on RPS, CPU, and Memory (Coming Soon!) - ðï¸ [Use Secrets for Redis-Powered
+Rate Limiting](docs/rate_limit/) - ð [Secure Your Endpoints with built-in
+OAuth2.0 Authorization](docs/authorization/) - ð [Handle File Uploads and
+Downloads with built-in Blob Storage](docs/file_handling/) - ð³ Deployment
+with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-
+Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸ `fastapi-
+serve` CLI `fastapi-serve` comes with a simple CLI that allows you to deploy
+your FastAPI applications to the cloud with ease. | Description | Command | | -
+-- | ---: | | Deploy your app locally | `fastapi-serve deploy local app:app` |
+| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` | | Update
+existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id ` | |
+Get app status on JCloud | `fastapi-serve status ` | | List all apps on JCloud
+| `fastapi-serve list` | | Remove app on JCloud | `fastapi-serve remove ` | ##
+âï¸ð° Configuration and Pricing Read our [Configuration & Pricing Guide]
+(examples/CONFIG.MD) to learn more about the various configuration options
+available to you and the pricing model for `fastapi-serve`. ## ðª Support If
+you encounter any problems or have questions, feel free to open an issue on the
+GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
+get help from our community members and the Jina team. ## Our Cloud Platform
+ð `cloud.jina.ai` is our robust and scalable cloud platform designed to run
+your FastAPI applications with minimum hassle and maximum efficiency. With
+features like auto-scaling, integrated observability, and automated
+containerization, it provides a seamless and worry-free deployment experience.
+--- `fastapi-serve` is more than just a deployment tool, it's a bridge that
+connects your local development environment with our powerful cloud
+infrastructure. Start using `fastapi-serve` today, and experience the joy of
+effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/__main__.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/helper.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.3.dev9/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.3.dev8
+Version: 0.0.3.dev9
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -71,18 +71,19 @@
 
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
 We have a few examples to help you get acquainted with `fastapi-serve`:
 
-- 🚀 [Deploy a Simple FastAPI Application](examples/simple/)
-- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](examples/rate_limit/)
-- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](examples/authorization/)
-- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](examples/file_handling/)
+- 🚀 [Deploy a Simple FastAPI Application](docs/simple/)
+- 💹 Auto-scaling endpoints based on RPS, CPU, and Memory (Coming Soon!)
+- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
+- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
+- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
 - 🐳 Deployment with Custom Dockerfile (Coming Soon!)
 - 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
 
 
 ## 🖥️ `fastapi-serve` CLI 
 
 `fastapi-serve` comes with a simple CLI that allows you to deploy your FastAPI applications to the cloud with ease.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev8 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.3.dev9 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -39,34 +39,35 @@
 Hosting**: Export your app for self-hosting with ease, including docker-compose
 and Kubernetes yamls. ## ð¡ Getting Started First, install the `fastapi-
 serve` package using pip: ```bash pip install fastapi-serve ``` Then, simply
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
 deployed application along with the Swagger UI. ## ð Documentation We have a
 few examples to help you get acquainted with `fastapi-serve`: - ð [Deploy a
-Simple FastAPI Application](examples/simple/) - ðï¸ [Use Secrets for Redis-
-Powered Rate Limiting](examples/rate_limit/) - ð [Secure Your Endpoints with
-built-in OAuth2.0 Authorization](examples/authorization/) - ð [Handle File
-Uploads and Downloads with built-in Blob Storage](examples/file_handling/) -
-ð³ Deployment with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App
-for Self-Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸
-`fastapi-serve` CLI `fastapi-serve` comes with a simple CLI that allows you to
-deploy your FastAPI applications to the cloud with ease. | Description |
-Command | | --- | ---: | | Deploy your app locally | `fastapi-serve deploy
-local app:app` | | Deploy your app on JCloud | `fastapi-serve deploy jcloud
-app:app` | | Update existing app on JCloud | `fastapi-serve deploy jcloud app:
-app --app-id ` | | Get app status on JCloud | `fastapi-serve status ` | | List
-all apps on JCloud | `fastapi-serve list` | | Remove app on JCloud | `fastapi-
-serve remove ` | ## âï¸ð° Configuration and Pricing Read our
-[Configuration & Pricing Guide](examples/CONFIG.MD) to learn more about the
-various configuration options available to you and the pricing model for
-`fastapi-serve`. ## ðª Support If you encounter any problems or have
-questions, feel free to open an issue on the GitHub repository. You can also
-join our [Discord](https://discord.jina.ai/) to get help from our community
-members and the Jina team. ## Our Cloud Platform ð `cloud.jina.ai` is our
-robust and scalable cloud platform designed to run your FastAPI applications
-with minimum hassle and maximum efficiency. With features like auto-scaling,
-integrated observability, and automated containerization, it provides a
-seamless and worry-free deployment experience. --- `fastapi-serve` is more than
-just a deployment tool, it's a bridge that connects your local development
-environment with our powerful cloud infrastructure. Start using `fastapi-serve`
-today, and experience the joy of effortless deployments! ð
+Simple FastAPI Application](docs/simple/) - ð¹ Auto-scaling endpoints based
+on RPS, CPU, and Memory (Coming Soon!) - ðï¸ [Use Secrets for Redis-Powered
+Rate Limiting](docs/rate_limit/) - ð [Secure Your Endpoints with built-in
+OAuth2.0 Authorization](docs/authorization/) - ð [Handle File Uploads and
+Downloads with built-in Blob Storage](docs/file_handling/) - ð³ Deployment
+with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-
+Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸ `fastapi-
+serve` CLI `fastapi-serve` comes with a simple CLI that allows you to deploy
+your FastAPI applications to the cloud with ease. | Description | Command | | -
+-- | ---: | | Deploy your app locally | `fastapi-serve deploy local app:app` |
+| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` | | Update
+existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id ` | |
+Get app status on JCloud | `fastapi-serve status ` | | List all apps on JCloud
+| `fastapi-serve list` | | Remove app on JCloud | `fastapi-serve remove ` | ##
+âï¸ð° Configuration and Pricing Read our [Configuration & Pricing Guide]
+(examples/CONFIG.MD) to learn more about the various configuration options
+available to you and the pricing model for `fastapi-serve`. ## ðª Support If
+you encounter any problems or have questions, feel free to open an issue on the
+GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
+get help from our community members and the Jina team. ## Our Cloud Platform
+ð `cloud.jina.ai` is our robust and scalable cloud platform designed to run
+your FastAPI applications with minimum hassle and maximum efficiency. With
+features like auto-scaling, integrated observability, and automated
+containerization, it provides a seamless and worry-free deployment experience.
+--- `fastapi-serve` is more than just a deployment tool, it's a bridge that
+connects your local development environment with our powerful cloud
+infrastructure. Start using `fastapi-serve` today, and experience the joy of
+effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.3.dev8/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev8/setup.py` & `fastapi-serve-0.0.3.dev9/setup.py`

 * *Files identical despite different names*

