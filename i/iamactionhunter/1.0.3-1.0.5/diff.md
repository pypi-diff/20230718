# Comparing `tmp/iamactionhunter-1.0.3.tar.gz` & `tmp/IAMActionHunter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamactionhunter-1.0.3.tar", max compression
+gzip compressed data, was "IAMActionHunter-1.0.5.tar", max compression
```

## Comparing `iamactionhunter-1.0.3.tar` & `IAMActionHunter-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11430 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/IAMActionHunter.py
--rw-r--r--   0        0        0        0 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/configs/__init.py__
--rw-r--r--   0        0        0     5970 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/configs/all.py
--rw-r--r--   0        0        0        0 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/__init__.py
--rw-r--r--   0        0        0     1973 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/create_csv.py
--rw-r--r--   0        0        0     6108 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/data_collection.py
--rw-r--r--   0        0        0     4141 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/statement_parser.py
--rw-r--r--   0        0        0      433 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/text_formatter.py
--rw-r--r--   0        0        0    11357 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/LICENSE
--rw-r--r--   0        0        0     4183 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/README.md
--rw-r--r--   0        0        0      882 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 iamactionhunter-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0    11695 2023-07-18 19:45:03.537957 IAMActionHunter-1.0.5/IAMActionHunter/IAMActionHunter.py
+-rwxr-xr-x   0        0        0        0 2023-06-22 20:28:53.511334 IAMActionHunter-1.0.5/IAMActionHunter/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-23 14:28:26.357544 IAMActionHunter-1.0.5/IAMActionHunter/configs/__init.py__
+-rwxr-xr-x   0        0        0     6163 2023-07-18 19:45:03.555098 IAMActionHunter-1.0.5/IAMActionHunter/configs/all.py
+-rwxr-xr-x   0        0        0        0 2023-06-23 14:28:26.379267 IAMActionHunter-1.0.5/IAMActionHunter/lib/__init__.py
+-rwxr-xr-x   0        0        0     1973 2023-06-23 14:28:26.401980 IAMActionHunter-1.0.5/IAMActionHunter/lib/create_csv.py
+-rwxr-xr-x   0        0        0     6108 2023-06-23 16:32:32.091620 IAMActionHunter-1.0.5/IAMActionHunter/lib/data_collection.py
+-rwxr-xr-x   0        0        0     4141 2023-07-18 19:45:03.571742 IAMActionHunter-1.0.5/IAMActionHunter/lib/statement_parser.py
+-rwxr-xr-x   0        0        0      433 2023-06-23 14:28:26.429848 IAMActionHunter-1.0.5/IAMActionHunter/lib/text_formatter.py
+-rwxr-xr-x   0        0        0    11357 2023-06-22 20:28:53.511334 IAMActionHunter-1.0.5/LICENSE
+-rwxr-xr-x   0        0        0     4272 2023-07-18 19:45:03.587377 IAMActionHunter-1.0.5/README.md
+-rwxr-xr-x   0        0        0      883 2023-07-18 20:23:33.902860 IAMActionHunter-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5419 1970-01-01 00:00:00.000000 IAMActionHunter-1.0.5/setup.py
+-rw-r--r--   0        0        0     4739 1970-01-01 00:00:00.000000 IAMActionHunter-1.0.5/PKG-INFO
```

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/IAMActionHunter.py` & `IAMActionHunter-1.0.5/IAMActionHunter/IAMActionHunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,28 +280,34 @@
 
         if not all_files:
             print("[-] No users or roles found for that query")
             sys.exit(1)
 
         if args.config:
             # Try to load config from builtin configs
-            if args.config in vars(configs):
-                query_config = vars(configs)[args.config]
+            builtin_configs = vars(configs)
+            if args.config in builtin_configs:
+                query_config = builtin_configs[args.config]
             else:
                 # Else try to load a config file
                 try:
-                    with open(f"configs/{args.config}.json", "r") as f:
+                    with open(f"{args.config}", "r") as f:
                         query_config = json.loads(f.read())
                 except FileNotFoundError:
-                    try:
-                        with open(args.config, "r") as f:
-                            query_config = json.loads(f.read())
-                    except FileNotFoundError:
-                        print(f"{args.config} does not exist. Please specify a valid config file or name")
-                        sys.exit(1)
+                    print(f"{args.config} does not exist. Please specify a valid config file or name. ")
+                    print("Builtin config options are:")
+                    print()
+                    for config in builtin_configs:
+                        if not config.startswith("__"):
+                            print(config)
+                    print()
+                    sys.exit(1)
+                except json.decoder.JSONDecodeError:
+                    print(f"{args.config} is not a valid config JSON file")
+                    sys.exit(1)
 
         # Iterate through all files and process them
         for permission_file in all_files:
             principal_type = permission_file.split("/")[-2][:-1]
             principal_name = permission_file.split("/")[-1].split(".json")[0]
 
             with open(permission_file, "r") as f:
```

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/configs/all.py` & `IAMActionHunter-1.0.5/IAMActionHunter/configs/all.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,8 +219,16 @@
         "Name": "PassExistingRoleToNewCodeStarProject",
         "ActionsNeeded": [
             "codestar:CreateProject",
             "iam:PassRole",
         ],
         "AllOrNone": True,
     },
+    {
+        "Description": "",
+        "Name": "ModifyEC2UserData",
+        "ActionsNeeded": [
+            "ec2:ModifyInstanceAttribute",
+        ],
+        "AllOrNone": True,
+    },
 ]
```

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/lib/create_csv.py` & `IAMActionHunter-1.0.5/IAMActionHunter/lib/create_csv.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/lib/data_collection.py` & `IAMActionHunter-1.0.5/IAMActionHunter/lib/data_collection.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/lib/statement_parser.py` & `IAMActionHunter-1.0.5/IAMActionHunter/lib/statement_parser.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/LICENSE` & `IAMActionHunter-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/README.md` & `IAMActionHunter-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Description
 IAMActionHunter is an IAM policy statement parser and query tool aims to simplify the process of collecting and understanding permission policy statements for users and roles in AWS Identity and Access Management (IAM). Although its functionality is straightforward, this tool was developed in response to the need for an efficient solution during day-to-day AWS penetration testing.
 
+### Blog Post
+https://rhinosecuritylabs.com/aws/iamactionhunter-aws-iam-permissions/
+
 ## Offensive Use
 The tool can be utilized to search for potential privilege escalation opportunities in AWS accounts by querying various AWS IAM actions that might be exploited. While other tools perform scans to identify privilege escalation risks, this tool enables a more manual approach, allowing users to investigate permissions and quickly review the roles, users, and resources they apply to for targeted analysis.
 
 ## Blue Team Use
 This tool also offers the ability to output and save query results in a CSV format, which is beneficial for security teams seeking a high-level overview of principal permissions and resources within an AWS account. For instance, you may want to identify users and roles with `iam:put*` permissions in an account. By executing a query and generating a CSV, you can easily review all users and roles with these permissions, along with the resources they have access to.
 
 # Installation
-Much of this functionality has also been implemented into https://github.com/RhinoSecurityLabs/pacu as a module, `iam__enum_action_query` if you prefer that.
 
 Suggested:
 ```
 pip3 install iamactionhunter
 ```
 
+Much of this functionality has also been implemented into https://github.com/RhinoSecurityLabs/pacu as a module, `iam__enum_action_query` if you prefer that.
 
 Clone and use Poetry:
 ```
 git clone https://github.com/RhinoSecurityLabs/IAMActionHunter.git
 cd IAMActionHunter
 poetry install
 iamactionhunter --help
```

### Comparing `iamactionhunter-1.0.3/pyproject.toml` & `IAMActionHunter-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "IAMActionHunter"
-version = "1.0.3"
+version = "1.0.5"
 description = "A query tool for AWS IAM policy statements."
 authors = ["Dave Yesland with Rhino Security Labs"]
 readme = "README.md"
 packages = [{include = "IAMActionHunter"},{include="lib", from="IAMActionHunter"},{include="configs", from="IAMActionHunter"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -28,8 +28,8 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 iamactionhunter = 'IAMActionHunter.IAMActionHunter:main'
 IAMActionHunter = 'IAMActionHunter.IAMActionHunter:main'
 
 [tool.black]
-line-length = 120
+line-length = 120
```

### Comparing `iamactionhunter-1.0.3/PKG-INFO` & `IAMActionHunter-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: iamactionhunter
-Version: 1.0.3
+Version: 1.0.5
 Summary: A query tool for AWS IAM policy statements.
 Author: Dave Yesland with Rhino Security Labs
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.87,<2.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: policyuniverse (>=1.5.0.20220613,<2.0.0.0)
 Description-Content-Type: text/markdown
 
 # Description
 IAMActionHunter is an IAM policy statement parser and query tool aims to simplify the process of collecting and understanding permission policy statements for users and roles in AWS Identity and Access Management (IAM). Although its functionality is straightforward, this tool was developed in response to the need for an efficient solution during day-to-day AWS penetration testing.
 
+### Blog Post
+https://rhinosecuritylabs.com/aws/iamactionhunter-aws-iam-permissions/
+
 ## Offensive Use
 The tool can be utilized to search for potential privilege escalation opportunities in AWS accounts by querying various AWS IAM actions that might be exploited. While other tools perform scans to identify privilege escalation risks, this tool enables a more manual approach, allowing users to investigate permissions and quickly review the roles, users, and resources they apply to for targeted analysis.
 
 ## Blue Team Use
 This tool also offers the ability to output and save query results in a CSV format, which is beneficial for security teams seeking a high-level overview of principal permissions and resources within an AWS account. For instance, you may want to identify users and roles with `iam:put*` permissions in an account. By executing a query and generating a CSV, you can easily review all users and roles with these permissions, along with the resources they have access to.
 
 # Installation
-Much of this functionality has also been implemented into https://github.com/RhinoSecurityLabs/pacu as a module, `iam__enum_action_query` if you prefer that.
 
 Suggested:
 ```
 pip3 install iamactionhunter
 ```
 
+Much of this functionality has also been implemented into https://github.com/RhinoSecurityLabs/pacu as a module, `iam__enum_action_query` if you prefer that.
 
 Clone and use Poetry:
 ```
 git clone https://github.com/RhinoSecurityLabs/IAMActionHunter.git
 cd IAMActionHunter
 poetry install
 iamactionhunter --help
```

