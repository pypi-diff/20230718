# Comparing `tmp/prompttools-0.0.8.tar.gz` & `tmp/prompttools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompttools-0.0.8.tar", last modified: Sun Jul  9 02:49:38 2023, max compression
+gzip compressed data, was "prompttools-0.0.9.tar", last modified: Sun Jul  9 02:51:38 2023, max compression
```

## Comparing `prompttools-0.0.8.tar` & `prompttools-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.955250 prompttools-0.0.8/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.8/LICENSE
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5757 2023-07-09 02:49:38.954822 prompttools-0.0.8/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5156 2023-07-08 17:32:41.000000 prompttools-0.0.8/README.md
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.934516 prompttools-0.0.8/prompttools/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:50:24.000000 prompttools-0.0.8/prompttools/__init__.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.940358 prompttools-0.0.8/prompttools/experiment/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.8/prompttools/experiment/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      315 2023-07-08 00:40:21.000000 prompttools-0.0.8/prompttools/experiment/error.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)    12162 2023-07-08 00:38:48.000000 prompttools-0.0.8/prompttools/experiment/experiment.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2614 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/experiment/openai_chat_experiment.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2977 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/experiment/openai_completion_experiment.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:17.000000 prompttools-0.0.8/prompttools/experiment/openai_function_experiment.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:43.000000 prompttools-0.0.8/prompttools/experiment/vector_database_experiment.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.942351 prompttools-0.0.8/prompttools/experiment/widgets/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:20.000000 prompttools-0.0.8/prompttools/experiment/widgets/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2540 2023-07-05 19:53:43.000000 prompttools-0.0.8/prompttools/experiment/widgets/comparison.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2773 2023-07-05 18:58:31.000000 prompttools-0.0.8/prompttools/experiment/widgets/feedback.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      227 2023-07-05 19:13:42.000000 prompttools-0.0.8/prompttools/experiment/widgets/utility.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.946402 prompttools-0.0.8/prompttools/harness/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.8/prompttools/harness/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2205 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/harness/chat_history_harness.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2684 2023-07-05 23:52:26.000000 prompttools-0.0.8/prompttools/harness/chat_model_comparison_harness.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:46.000000 prompttools-0.0.8/prompttools/harness/document_retrieval_harness.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      185 2023-07-05 16:26:17.000000 prompttools-0.0.8/prompttools/harness/function_call_harness.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2314 2023-07-05 22:40:03.000000 prompttools-0.0.8/prompttools/harness/harness.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3105 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/harness/prompt_template_harness.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3175 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/harness/system_prompt_harness.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.947009 prompttools-0.0.8/prompttools/mock/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:14.000000 prompttools-0.0.8/prompttools/mock/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1246 2023-07-05 22:19:30.000000 prompttools-0.0.8/prompttools/mock/mock.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.948366 prompttools-0.0.8/prompttools/requests/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.8/prompttools/requests/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2591 2023-07-05 19:53:59.000000 prompttools-0.0.8/prompttools/requests/request_queue.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1624 2023-07-05 22:40:03.000000 prompttools-0.0.8/prompttools/requests/retries.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.949683 prompttools-0.0.8/prompttools/testing/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:08.000000 prompttools-0.0.8/prompttools/testing/__init__.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.950387 prompttools-0.0.8/prompttools/testing/error/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:11.000000 prompttools-0.0.8/prompttools/testing/error/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      840 2023-07-05 19:53:59.000000 prompttools-0.0.8/prompttools/testing/error/failure.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3788 2023-07-08 00:33:36.000000 prompttools-0.0.8/prompttools/testing/prompttest.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.952762 prompttools-0.0.8/prompttools/testing/runner/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:10.000000 prompttools-0.0.8/prompttools/testing/runner/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4261 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/testing/runner/prompt_template_runner.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1638 2023-07-05 22:40:03.000000 prompttools-0.0.8/prompttools/testing/runner/runner.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4199 2023-07-08 00:35:30.000000 prompttools-0.0.8/prompttools/testing/runner/system_prompt_runner.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      177 2023-07-05 19:53:59.000000 prompttools-0.0.8/prompttools/testing/threshold_type.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.953929 prompttools-0.0.8/prompttools/utils/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 04:30:21.000000 prompttools-0.0.8/prompttools/utils/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1600 2023-07-05 19:53:59.000000 prompttools-0.0.8/prompttools/utils/similarity.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       89 2023-07-09 02:49:29.000000 prompttools-0.0.8/prompttools/version.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:49:38.936498 prompttools-0.0.8/prompttools.egg-info/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5757 2023-07-09 02:49:38.000000 prompttools-0.0.8/prompttools.egg-info/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1737 2023-07-09 02:49:38.000000 prompttools-0.0.8/prompttools.egg-info/SOURCES.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-09 02:49:38.000000 prompttools-0.0.8/prompttools.egg-info/dependency_links.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.8/prompttools.egg-info/not-zip-safe
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-09 02:49:38.000000 prompttools-0.0.8/prompttools.egg-info/requires.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       12 2023-07-09 02:49:38.000000 prompttools-0.0.8/prompttools.egg-info/top_level.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-09 02:49:15.000000 prompttools-0.0.8/pyproject.toml
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.8/requirements.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-09 02:49:38.955364 prompttools-0.0.8/setup.cfg
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3737 2023-07-09 02:49:32.000000 prompttools-0.0.8/setup.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-09 02:49:20.000000 prompttools-0.0.8/version.txt
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.454267 prompttools-0.0.9/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.9/LICENSE
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5828 2023-07-09 02:51:38.453803 prompttools-0.0.9/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5227 2023-07-09 02:50:48.000000 prompttools-0.0.9/README.md
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.423022 prompttools-0.0.9/prompttools/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:50:24.000000 prompttools-0.0.9/prompttools/__init__.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.430974 prompttools-0.0.9/prompttools/experiment/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      390 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/experiment/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      315 2023-07-08 00:40:21.000000 prompttools-0.0.9/prompttools/experiment/error.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)    12162 2023-07-08 00:38:48.000000 prompttools-0.0.9/prompttools/experiment/experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2603 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/experiment/openai_chat_experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2966 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/experiment/openai_completion_experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:17.000000 prompttools-0.0.9/prompttools/experiment/openai_function_experiment.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:43.000000 prompttools-0.0.9/prompttools/experiment/vector_database_experiment.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.434224 prompttools-0.0.9/prompttools/experiment/widgets/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:20.000000 prompttools-0.0.9/prompttools/experiment/widgets/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2540 2023-07-05 19:53:43.000000 prompttools-0.0.9/prompttools/experiment/widgets/comparison.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2773 2023-07-05 18:58:31.000000 prompttools-0.0.9/prompttools/experiment/widgets/feedback.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      227 2023-07-05 19:13:42.000000 prompttools-0.0.9/prompttools/experiment/widgets/utility.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.440783 prompttools-0.0.9/prompttools/harness/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      693 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/harness/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2174 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/harness/chat_history_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2653 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/harness/chat_model_comparison_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      184 2023-07-05 16:26:46.000000 prompttools-0.0.9/prompttools/harness/document_retrieval_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      185 2023-07-05 16:26:17.000000 prompttools-0.0.9/prompttools/harness/function_call_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2303 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/harness/harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3059 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/harness/prompt_template_harness.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3144 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/harness/system_prompt_harness.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.442037 prompttools-0.0.9/prompttools/mock/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:14.000000 prompttools-0.0.9/prompttools/mock/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1246 2023-07-05 22:19:30.000000 prompttools-0.0.9/prompttools/mock/mock.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.444216 prompttools-0.0.9/prompttools/requests/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-04 19:36:44.000000 prompttools-0.0.9/prompttools/requests/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2591 2023-07-05 19:53:59.000000 prompttools-0.0.9/prompttools/requests/request_queue.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1624 2023-07-05 22:40:03.000000 prompttools-0.0.9/prompttools/requests/retries.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.446650 prompttools-0.0.9/prompttools/testing/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:08.000000 prompttools-0.0.9/prompttools/testing/__init__.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.447871 prompttools-0.0.9/prompttools/testing/error/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:11.000000 prompttools-0.0.9/prompttools/testing/error/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      840 2023-07-05 19:53:59.000000 prompttools-0.0.9/prompttools/testing/error/failure.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3788 2023-07-08 00:33:36.000000 prompttools-0.0.9/prompttools/testing/prompttest.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.451393 prompttools-0.0.9/prompttools/testing/runner/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 00:53:10.000000 prompttools-0.0.9/prompttools/testing/runner/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4228 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/testing/runner/prompt_template_runner.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1638 2023-07-05 22:40:03.000000 prompttools-0.0.9/prompttools/testing/runner/runner.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4177 2023-07-09 02:50:48.000000 prompttools-0.0.9/prompttools/testing/runner/system_prompt_runner.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      177 2023-07-05 19:53:59.000000 prompttools-0.0.9/prompttools/testing/threshold_type.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.452774 prompttools-0.0.9/prompttools/utils/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-08 04:30:21.000000 prompttools-0.0.9/prompttools/utils/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1600 2023-07-05 19:53:59.000000 prompttools-0.0.9/prompttools/utils/similarity.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       89 2023-07-09 02:51:23.000000 prompttools-0.0.9/prompttools/version.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-09 02:51:38.425883 prompttools-0.0.9/prompttools.egg-info/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5828 2023-07-09 02:51:38.000000 prompttools-0.0.9/prompttools.egg-info/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1737 2023-07-09 02:51:38.000000 prompttools-0.0.9/prompttools.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-09 02:51:38.000000 prompttools-0.0.9/prompttools.egg-info/dependency_links.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.9/prompttools.egg-info/not-zip-safe
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-09 02:51:38.000000 prompttools-0.0.9/prompttools.egg-info/requires.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       12 2023-07-09 02:51:38.000000 prompttools-0.0.9/prompttools.egg-info/top_level.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-09 02:51:16.000000 prompttools-0.0.9/pyproject.toml
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.9/requirements.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-09 02:51:38.454411 prompttools-0.0.9/setup.cfg
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3737 2023-07-09 02:51:29.000000 prompttools-0.0.9/setup.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-09 02:51:13.000000 prompttools-0.0.9/version.txt
```

### Comparing `prompttools-0.0.8/LICENSE` & `prompttools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/PKG-INFO` & `prompttools-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompttools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for LLM prompt testing and experimentation
 Home-page: https://github.com/hegelai/prompttools
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/prompttools
 Project-URL: Bug Tracker, https://github.com/hegelai/prompttools
@@ -55,14 +55,17 @@
 ### Notebooks
 
 There are a few different ways to run an experiment in a notebook. 
 
 The simplest way is to define an experimentation harness and an evaluation function:
 
 ```python
+from prompttools.harness import PromptTemplateExperimentationHarness
+
+
 def eval_fn(prompt: str, results: Dict, metadata: Dict) -> float:
     # Your logic here, or use a built-in one such as `prompttools.utils.similarity`.
     pass
 
 prompt_templates = [
     "Answer the following question: {{input}}", 
     "Respond the following query: {{input}}"
```

### Comparing `prompttools-0.0.8/README.md` & `prompttools-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 ### Notebooks
 
 There are a few different ways to run an experiment in a notebook. 
 
 The simplest way is to define an experimentation harness and an evaluation function:
 
 ```python
+from prompttools.harness import PromptTemplateExperimentationHarness
+
+
 def eval_fn(prompt: str, results: Dict, metadata: Dict) -> float:
     # Your logic here, or use a built-in one such as `prompttools.utils.similarity`.
     pass
 
 prompt_templates = [
     "Answer the following question: {{input}}", 
     "Respond the following query: {{input}}"
```

### Comparing `prompttools-0.0.8/prompttools/experiment/experiment.py` & `prompttools-0.0.9/prompttools/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/experiment/openai_chat_experiment.py` & `prompttools-0.0.9/prompttools/experiment/openai_chat_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 from typing import Dict, List, Optional
 import openai
 
 import logging
 
 from prompttools.mock.mock import mock_chat_completion_fn
-from prompttools.experiment.experiment import Experiment
+from prompttools.experiment import Experiment
 
 
 class OpenAIChatExperiment(Experiment):
     r"""
     This class defines an experiment for OpenAI's chat completion API.
     It accepts lists for each argument passed into OpenAI's API, then creates
     a cartesian product of those arguments, and gets results for each.
```

### Comparing `prompttools-0.0.8/prompttools/experiment/openai_completion_experiment.py` & `prompttools-0.0.9/prompttools/experiment/openai_completion_experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 from typing import Dict, List, Optional
 import openai
 import logging
 
 from prompttools.mock.mock import mock_completion_fn
-from prompttools.experiment.experiment import Experiment
+from prompttools.experiment import Experiment
 
 
 class OpenAICompletionExperiment(Experiment):
     r"""
     This class defines an experiment for OpenAI's chat completion API.
     It accepts lists for each argument passed into OpenAI's API, then creates
     a cartesian product of those arguments, and gets results for each.
```

### Comparing `prompttools-0.0.8/prompttools/experiment/widgets/comparison.py` & `prompttools-0.0.9/prompttools/experiment/widgets/comparison.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/experiment/widgets/feedback.py` & `prompttools-0.0.9/prompttools/experiment/widgets/feedback.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/harness/chat_history_harness.py` & `prompttools-0.0.9/prompttools/harness/chat_history_harness.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) Hegel AI, Inc.
 # All rights reserved.
 #
 # This source code's license can be found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, List, Optional
-from prompttools.harness.harness import ExperimentationHarness
-from prompttools.experiment.openai_chat_experiment import OpenAIChatExperiment
+from prompttools.harness import ExperimentationHarness
+from prompttools.experiment import OpenAIChatExperiment
 
 
 class ChatHistoryExperimentationHarness(ExperimentationHarness):
     r"""
     An experimentation harness used for compare multiple chat histories.
 
     Args:
```

### Comparing `prompttools-0.0.8/prompttools/harness/chat_model_comparison_harness.py` & `prompttools-0.0.9/prompttools/harness/chat_model_comparison_harness.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) Hegel AI, Inc.
 # All rights reserved.
 #
 # This source code's license can be found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, List, Optional
-from prompttools.harness.harness import ExperimentationHarness
-from prompttools.experiment.openai_chat_experiment import OpenAIChatExperiment
+from prompttools.harness import ExperimentationHarness
+from prompttools.experiment import OpenAIChatExperiment
 
 
 class ChatModelComparisonHarness(ExperimentationHarness):
     r"""
     An experimentation harness used for comparing chat models.
     Multi-model version of ``ChatHistoryExperimentationHarness``.
```

### Comparing `prompttools-0.0.8/prompttools/harness/harness.py` & `prompttools-0.0.9/prompttools/harness/harness.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Hegel AI, Inc.
 # All rights reserved.
 #
 # This source code's license can be found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Callable, Dict, List
-from prompttools.experiment.experiment import Experiment
+from prompttools.experiment import Experiment
 
 
 class ExperimentationHarness:
     r"""
     Base class for experimentation harnesses. This should not be used directly, please use the subclasses instead.
     """
```

### Comparing `prompttools-0.0.8/prompttools/harness/prompt_template_harness.py` & `prompttools-0.0.9/prompttools/harness/prompt_template_harness.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 # All rights reserved.
 #
 # This source code's license can be found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, List, Optional
 import jinja2
-from prompttools.harness.harness import ExperimentationHarness
-from prompttools.experiment.openai_completion_experiment import (
-    OpenAICompletionExperiment,
-)
+from prompttools.harness import ExperimentationHarness
+from prompttools.experiment import OpenAICompletionExperiment
 
 
 class PromptTemplateExperimentationHarness(ExperimentationHarness):
     r"""
     An experimentation harness used to test various prompt templates.
     We use `jinja` templates, e.g. "Answer the following question: {{input}}".
```

### Comparing `prompttools-0.0.8/prompttools/harness/system_prompt_harness.py` & `prompttools-0.0.9/prompttools/harness/system_prompt_harness.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) Hegel AI, Inc.
 # All rights reserved.
 #
 # This source code's license can be found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, List, Optional
-from prompttools.harness.harness import ExperimentationHarness
-from prompttools.experiment.openai_chat_experiment import OpenAIChatExperiment
+from prompttools.harness import ExperimentationHarness
+from prompttools.experiment import OpenAIChatExperiment
 
 
 class SystemPromptExperimentationHarness(ExperimentationHarness):
     r"""
     An experimentation harness used to test various system prompts.
 
     Args:
```

### Comparing `prompttools-0.0.8/prompttools/mock/mock.py` & `prompttools-0.0.9/prompttools/mock/mock.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/requests/request_queue.py` & `prompttools-0.0.9/prompttools/requests/request_queue.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/requests/retries.py` & `prompttools-0.0.9/prompttools/requests/retries.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/testing/error/failure.py` & `prompttools-0.0.9/prompttools/testing/error/failure.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/testing/prompttest.py` & `prompttools-0.0.9/prompttools/testing/prompttest.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/testing/runner/prompt_template_runner.py` & `prompttools-0.0.9/prompttools/testing/runner/prompt_template_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Callable, Dict, List, Tuple
 import csv
 import logging
 
 from prompttools.testing.threshold_type import ThresholdType
 from prompttools.testing.error.failure import log_failure
-from prompttools.harness.prompt_template_harness import (
-    PromptTemplateExperimentationHarness,
-)
+from prompttools.harness import PromptTemplateExperimentationHarness
 from prompttools.testing.runner.runner import PromptTestRunner
 from prompttools.testing.error.failure import PromptTestSetupException
 
 
 class PromptTemplateTestRunner(PromptTestRunner):
     r"""
     A prompt test runner for tests based on prompt templates.
```

### Comparing `prompttools-0.0.8/prompttools/testing/runner/runner.py` & `prompttools-0.0.9/prompttools/testing/runner/runner.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools/testing/runner/system_prompt_runner.py` & `prompttools-0.0.9/prompttools/testing/runner/system_prompt_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Dict, List, Tuple
 import csv
 import logging
 
 from prompttools.testing.threshold_type import ThresholdType
 from prompttools.testing.error.failure import log_failure
-from prompttools.harness.system_prompt_harness import SystemPromptExperimentationHarness
+from prompttools.harness import SystemPromptExperimentationHarness
 from prompttools.testing.runner.runner import PromptTestRunner
 from prompttools.testing.error.failure import PromptTestSetupException
 
 
 class SystemPromptTestRunner(PromptTestRunner):
     r"""
     A prompt test runner for tests based on system prompts.
```

### Comparing `prompttools-0.0.8/prompttools/utils/similarity.py` & `prompttools-0.0.9/prompttools/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/prompttools.egg-info/PKG-INFO` & `prompttools-0.0.9/prompttools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompttools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for LLM prompt testing and experimentation
 Home-page: https://github.com/hegelai/prompttools
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/prompttools
 Project-URL: Bug Tracker, https://github.com/hegelai/prompttools
@@ -55,14 +55,17 @@
 ### Notebooks
 
 There are a few different ways to run an experiment in a notebook. 
 
 The simplest way is to define an experimentation harness and an evaluation function:
 
 ```python
+from prompttools.harness import PromptTemplateExperimentationHarness
+
+
 def eval_fn(prompt: str, results: Dict, metadata: Dict) -> float:
     # Your logic here, or use a built-in one such as `prompttools.utils.similarity`.
     pass
 
 prompt_templates = [
     "Answer the following question: {{input}}", 
     "Respond the following query: {{input}}"
```

### Comparing `prompttools-0.0.8/prompttools.egg-info/SOURCES.txt` & `prompttools-0.0.9/prompttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.8/pyproject.toml` & `prompttools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prompttools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Hegel AI", email="team@hegel-ai.com" },
 ]
 description = "Tools for LLM prompt testing and experimentation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `prompttools-0.0.8/setup.py` & `prompttools-0.0.9/setup.py`

 * *Files identical despite different names*

