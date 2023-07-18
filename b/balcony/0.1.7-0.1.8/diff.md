# Comparing `tmp/balcony-0.1.7.tar.gz` & `tmp/balcony-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.7.tar", max compression
+gzip compressed data, was "balcony-0.1.8.tar", max compression
```

## Comparing `balcony-0.1.7.tar` & `balcony-0.1.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.7/LICENSE
--rw-r--r--   0        0        0     3621 2023-06-27 21:55:30.541972 balcony-0.1.7/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.7/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.7/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.7/balcony/aws.py
--rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.7/balcony/botocore_utils.py
--rw-r--r--   0        0        0    22612 2023-07-17 18:22:23.044112 balcony-0.1.7/balcony/cli.py
--rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.7/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.7/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.7/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.7/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.7/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.7/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.7/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.7/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.7/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.7/balcony/custom_tf_import_configs/_example_import_conf.yaml
--rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.7/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.7/balcony/custom_tf_import_configs/ecs.yaml
--rw-r--r--   0        0        0     1610 2023-07-17 18:20:28.021261 balcony-0.1.7/balcony/custom_tf_import_configs/iam.yaml
--rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.7/balcony/custom_tf_import_configs/rds.yaml
--rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.7/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.1.7/balcony/custom_tf_import_configs/vpc.yaml
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.7/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.7/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.7/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.7/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.7/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.7/balcony/errors.py
--rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.7/balcony/nodes.py
--rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.7/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.7/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.7/balcony/relations.py
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.7/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0    10693 2023-07-17 17:11:29.424367 balcony-0.1.7/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.1.7/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.1.7/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.7/balcony/terraform_import/wizard.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.7/balcony/test.py
--rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.7/balcony/utils.py
--rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.7/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.7/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-07-17 18:31:02.099122 balcony-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 balcony-0.1.7/setup.py
--rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 balcony-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3851 2023-07-17 18:52:57.338228 balcony-0.1.8/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.8/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.8/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.8/balcony/aws.py
+-rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.8/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    22612 2023-07-17 18:22:23.044112 balcony-0.1.8/balcony/cli.py
+-rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.8/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.8/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.8/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.8/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.8/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.8/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.8/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.8/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.8/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.8/balcony/custom_tf_import_configs/_example_import_conf.yaml
+-rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.8/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      935 2023-07-18 19:25:23.582721 balcony-0.1.8/balcony/custom_tf_import_configs/ecs.yaml
+-rw-r--r--   0        0        0     1610 2023-07-17 18:20:28.021261 balcony-0.1.8/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.8/balcony/custom_tf_import_configs/rds.yaml
+-rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.8/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.1.8/balcony/custom_tf_import_configs/vpc.yaml
+-rw-r--r--   0        0        0     3271 2023-07-18 18:28:06.436858 balcony-0.1.8/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.8/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0     2704 2023-07-18 19:10:24.404655 balcony-0.1.8/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.8/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.8/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.8/balcony/errors.py
+-rw-r--r--   0        0        0    49370 2023-07-18 18:50:11.229744 balcony-0.1.8/balcony/nodes.py
+-rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.8/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.8/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.8/balcony/relations.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.8/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0    10693 2023-07-17 17:11:29.424367 balcony-0.1.8/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.1.8/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.1.8/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.8/balcony/terraform_import/wizard.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.8/balcony/test.py
+-rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.8/balcony/utils.py
+-rw-r--r--   0        0        0     2344 2023-07-18 18:43:44.785613 balcony-0.1.8/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2124 2023-07-18 18:27:00.154209 balcony-0.1.8/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-07-18 19:26:08.878958 balcony-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 balcony-0.1.8/setup.py
+-rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 balcony-0.1.8/PKG-INFO
```

### Comparing `balcony-0.1.7/LICENSE` & `balcony-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/README.md` & `balcony-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,26 +36,32 @@
 
 # list available resources of ec2
 balcony aws ec2 
 
 # read a resource
 balcony aws s3 Buckets
 
+# show documentation
+balcony aws iam Policy --list
+
 # generate terraform import blocks for a resource
 balcony terraform-import s3 Buckets
 ```
 
 
 ## Features
 
 ### Read any AWS Resource
+
+`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.
+
 Related Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)
 
+![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)
 
-![](visuals/reading-a-resource-node.gif)
 
 ---
 
 ### Generate Terraform Import Blocks
 
 Terraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.
```

#### html2text {}

```diff
@@ -8,35 +8,37 @@
 Terraform Resource code balcony uses _read-only_ operations, it does not take
 any action on the used AWS account. ### [Visit the Documentation Website]
 (https://oguzhan-yilmaz.github.io/balcony/quickstart/)  ### Installation
 ```bash pip3 install balcony ``` Visit [**Installation & QuickStart Page**]
 (https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using
 _balcony_ ```bash title="Basic usage" # see options balcony # list available
 resources of ec2 balcony aws ec2 # read a resource balcony aws s3 Buckets #
-generate terraform import blocks for a resource balcony terraform-import s3
-Buckets ``` ## Features ### Read any AWS Resource Related Docs: [QuickStart]
-(https://oguzhan-yilmaz.github.io/balcony/quickstart/) ![](visuals/reading-a-
-resource-node.gif) --- ### Generate Terraform Import Blocks Terraform v1.5
-introduced [import blocks](https://developer.hashicorp.com/terraform/language/
-import) that allows users to define their imports as code. `balcony terraform-
-import  ` command generates these import blocks for you. `balcony terraform-
-import --list` to see the list of supported resources. Related Docs: [Generate
-Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-
-import/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/
-main/gifs/terraform-import-blocks-example.gif) --- ### Generate actual
-Terraform Resource Code If you have: - initialized terraform project -
-`import_blocks.tf` file that's generated with `balcony terraform-import`
-command you can run `terraform plan -generate-config-out=generated.tf` to
-generate actual `.tf` resource code. This feature is achieved with a Docker
-image. Related Docs: [Generate Terraform Code with Docker Image](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import-docker/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
-tf-code-ec2-insances-example.gif) --- ### Interactive Wizard to create balcony
-import configurations Balcony doesn't know how to create terraform `import
-blocks` for all of the AWS resources. It can be taught how to do it by creating
-`import-configurations` yaml files, but it's a manual process. This is where
-the interactive wizard comes in. Interactive Wizards asks you required
-questions to automatically create the `import-configurations` yaml files.
-Related Docs: [Terraform Import Configuration Wizard](https://oguzhan-
-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
+show documentation balcony aws iam Policy --list # generate terraform import
+blocks for a resource balcony terraform-import s3 Buckets ``` ## Features ###
+Read any AWS Resource `balcony aws   --paginate` command reads all resources of
+a given type in your AWS account. Related Docs: [QuickStart](https://oguzhan-
+yilmaz.github.io/balcony/quickstart/) ![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif) --- ### Generate
+Terraform Import Blocks Terraform v1.5 introduced [import blocks](https://
+developer.hashicorp.com/terraform/language/import) that allows users to define
+their imports as code. `balcony terraform-import  ` command generates these
+import blocks for you. `balcony terraform-import --list` to see the list of
+supported resources. Related Docs: [Generate Terraform Import Blocks](https://
+oguzhan-yilmaz.github.io/balcony/terraform-import/) ![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
+import-blocks-example.gif) --- ### Generate actual Terraform Resource Code If
+you have: - initialized terraform project - `import_blocks.tf` file that's
+generated with `balcony terraform-import` command you can run `terraform plan -
+generate-config-out=generated.tf` to generate actual `.tf` resource code. This
+feature is achieved with a Docker image. Related Docs: [Generate Terraform Code
+with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-
+docker/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/
+main/gifs/docker-gen-tf-code-ec2-insances-example.gif) --- ### Interactive
+Wizard to create balcony import configurations Balcony doesn't know how to
+create terraform `import blocks` for all of the AWS resources. It can be taught
+how to do it by creating `import-configurations` yaml files, but it's a manual
+process. This is where the interactive wizard comes in. Interactive Wizards
+asks you required questions to automatically create the `import-configurations`
+yaml files. Related Docs: [Terraform Import Configuration Wizard](https://
+oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 wizard-security-groups-example.gif)
```

### Comparing `balcony-0.1.7/balcony/__init__.py` & `balcony-0.1.8/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/aws.py` & `balcony-0.1.8/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/botocore_utils.py` & `balcony-0.1.8/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/cli.py` & `balcony-0.1.8/balcony/cli.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/config.py` & `balcony-0.1.8/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/codebuild.py` & `balcony-0.1.8/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/ecs.py` & `balcony-0.1.8/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/iam.py` & `balcony-0.1.8/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.8/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/s3.py` & `balcony-0.1.8/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/ses.py` & `balcony-0.1.8/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_nodes/ssm.py` & `balcony-0.1.8/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.1.8/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_tf_import_configs/iam.yaml` & `balcony-0.1.8/balcony/custom_tf_import_configs/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_tf_import_configs/rds.yaml` & `balcony-0.1.8/balcony/custom_tf_import_configs/rds.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_tf_import_configs/vpc.yaml` & `balcony-0.1.8/balcony/custom_tf_import_configs/vpc.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.8/balcony/custom_yamls/_example_service.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,18 @@
   operations:
     # Operation level customization must define a specific `operation_name` 
     - operation_name: <operation-name> 
       # Pagination token mapping customization
       pagination_token_mapping:
         output_key: NextContinuationToken # from output, get this key and
         parameter_name: ContinuationToken # pass it to this parameter
+      # override required-parameters of an operation
+      required_parameters:
+        - ParamName1
+        - ParamName2
       # This option overrides the `complement_api_parameters_list` function.
       complement_api_parameters:
         # This option will be evoked after api parameter generation is 
         # complete. You can use this feature to add key/value pairs, 
         - action: add
           data:
             any: data
```

### Comparing `balcony-0.1.7/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.8/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/custom_yamls/iam.yaml` & `balcony-0.1.8/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/nodes.py` & `balcony-0.1.8/balcony/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from utils import (
     camel_case_split,
     compare_nouns,
     icompare_two_token_lists,
     compare_two_camel_case_words,
     str_relations,
     is_word_in_a_list_of_words,
-    inform_about_develeoping_custom_resource_nodes
+    inform_about_develeoping_custom_resource_nodes,
 )
 from botocore_utils import (
     get_input_shape,
     annotate_shape_and_its_members_with_target_path,
     get_max_results_value_from_shape,
     find_key_in_dict_keys,
     generate_rich_tree_from_shape,
@@ -48,17 +48,14 @@
     "nexttoken",
     "continuationtoken",
     "marker",
     "nextcontinuationtoken",
 )
 
 
-
-
-
 class ResourceNode:
     def __init__(
         self, service_node: "ServiceNode", name: str, operation_names: List[str]
     ) -> None:
         self.service_node = service_node
         self.name = name
         self.operation_names = operation_names
@@ -489,28 +486,34 @@
 
         return api_parameters_list, None
 
     def print_operation(self, operation_name: str) -> None:
         operation_panel = self._rich_operation_details_panel(operation_name)
         console.print(operation_panel)
 
-    def _rich_operation_details_panel(self, operation_name: str, remove_input_shape=False, remove_documentation=False) -> Panel:
+    def _rich_operation_details_panel(
+        self, operation_name: str, remove_input_shape=False, remove_documentation=False
+    ) -> Panel:
 
         operation_model = self.get_operation_model(operation_name)
         input_shape = get_input_shape(operation_model)
         output_shape = operation_model.output_shape
-        input_shape_name = 'No Input Shape Found'
+        input_shape_name = "No Input Shape Found"
         input_shape_tree = Text("No Input Shape Found")
         if input_shape:
-            input_shape_tree = generate_rich_tree_from_shape(input_shape, remove_documentation=remove_documentation)
+            input_shape_tree = generate_rich_tree_from_shape(
+                input_shape, remove_documentation=remove_documentation
+            )
             input_shape_name = input_shape.name
-        output_shape_tree = generate_rich_tree_from_shape(output_shape, remove_documentation=remove_documentation)
+        output_shape_tree = generate_rich_tree_from_shape(
+            output_shape, remove_documentation=remove_documentation
+        )
 
         operation_docs = cleanhtml(operation_model.documentation)
-        
+
         panel_group = Group(
             Padding(f"[bold underline]Documentation:[/] {operation_docs}", (1, 2)),
             Panel(
                 input_shape_tree,
                 title=f"Input: [yellow]{input_shape_name}",
                 title_align="left",
                 padding=(1, 1),
@@ -518,15 +521,15 @@
             Panel(
                 output_shape_tree,
                 title=f"Output: [yellow]{output_shape.name}",
                 title_align="left",
                 padding=(1, 1),
             ),
         )
-        
+
         if remove_input_shape:
             panel_group = Group(
                 Padding(f"[bold underline]Documentation:[/] {operation_docs}", (1, 2)),
                 Panel(
                     output_shape_tree,
                     title=f"Output: [yellow]{output_shape.name}",
                     title_align="left",
@@ -815,14 +818,26 @@
                         Relation(**rel_model.__dict__)
                         for rel_model in operation.explicit_relations
                     ]
                     return explicit_relations, None
         # if no explicit relations are defined, then call the ResourceNode method and return it
         return super().get_operations_relations(operation_name)
 
+    def get_required_parameter_names_from_operation_name(
+        self, operation_name: str
+    ) -> List[str]:
+        operations = self.yaml_config.operations
+        for operation in operations:
+            if operation_name == operation.operation_name:
+                if operation.required_parameters:
+                    required_parameters = operation.required_parameters
+                    return required_parameters
+
+        return super().get_required_parameter_names_from_operation_name(operation_name)
+
     # NOTE: +overrideable
     def generate_jmespath_selector_from_relations(
         self, operation_name: str, relation_list: List[Dict]
     ) -> str:
         """Finds the `jmespath_selector` definition in the `yaml_config` for the selected Operation.
 
         Args:
```

### Comparing `balcony-0.1.7/balcony/reader.py` & `balcony-0.1.8/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/registries.py` & `balcony-0.1.8/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/relations.py` & `balcony-0.1.8/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/terraform_import/importer.py` & `balcony-0.1.8/balcony/terraform_import/importer.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/terraform_import/models.py` & `balcony-0.1.8/balcony/terraform_import/models.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/terraform_import/parsers.py` & `balcony-0.1.8/balcony/terraform_import/parsers.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/terraform_import/wizard.py` & `balcony-0.1.8/balcony/terraform_import/wizard.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/test.py` & `balcony-0.1.8/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/utils.py` & `balcony-0.1.8/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.7/balcony/yaml_config.py` & `balcony-0.1.8/balcony/yaml_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,33 +22,33 @@
         Exception or `None`: Exception if raised during parsing, or None if successful
     """
     try:
         with open(yaml_file_path, "r") as f:
             input_data = yaml.load(f, Loader=yaml.FullLoader)
         return YamlService(**input_data), None
     except Exception as e:
+        logger.debug(f"Failed to parse yaml file {yaml_file_path}. Error: {str(e)}")
         return False, e
 
 
-
-
 def find_and_parse_yaml_services() -> List[YamlService]:
     """Searches and finds the defined yaml files in the YAML_SERVICES_DIRECTORY directory that are not starting with '_'
 
     Returns:
         List[YamlService]: List of found YamlServices, created from yaml files
     """
     found_yaml_services = []
     yaml_files = find_all_yaml_files(YAML_SERVICES_DIRECTORY)
     logger.debug(
         f"Terraform Import Configuration Registry: Found {len(yaml_files)} yaml files in {YAML_SERVICES_DIRECTORY}. Starting to parse & validate them."
     )
     for yaml_file in yaml_files:
         yaml_service, error = parse_yaml_file_to_service(yaml_file)
         if error is None and yaml_service:
+            logger.debug(f"Succesfully parsed [bold]{yaml_file}[/] to Yaml ResourceNode")
             found_yaml_services.append(yaml_service)
         else:
             logger.debug(
                 f"Failed to parse [bold]{yaml_file}[/] to service. Error: {str(error)}. "
             )
 
     return found_yaml_services
```

### Comparing `balcony-0.1.7/balcony/yaml_validators.py` & `balcony-0.1.8/balcony/yaml_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 
 class YamlRelation(BaseModel):
     service_name: str
     resource_node_name: str
     operation_name: str
     required_shape_name: str
-    target_shape_name: str
-    target_shape_type: str
-    target_path: str
+    target_shape_name: Optional[str]
+    target_shape_type: Optional[str]
+    target_path: Optional[str]
 
 
 class YamlComplementApiParameterAction(BaseModel):
     """Defines the `add` and `remove` options for complement_api_parameters in YamlResourceNodeOperation"""
     _ACTION_TYPES = ("add", "remove")
 
     action: str
@@ -32,14 +32,15 @@
     """Defines the customizations for a specific operation in a Resource Node."""
     operation_name: str
     jmespath_selector: Optional[str]
     complement_api_parameters: Optional[List[YamlComplementApiParameterAction]]
     explicit_relations: Optional[List[YamlRelation]]
     override_api_parameters: Optional[List[Dict[str, Any]]]
     pagination_token_mapping: Optional[Dict[str, str]]
+    required_parameters: Optional[List[str]]
 
 
 class YamlServiceResourceNode(BaseModel):
     """Defines a Resource Node in a Service. It can have extra_relations and list of operations"""
     resource_node_name: str
     extra_relations: Optional[List[YamlRelation]]
     operations: Optional[List[YamlResourceNodeOperation]]
```

### Comparing `balcony-0.1.7/pyproject.toml` & `balcony-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.7"
+version = "0.1.8"
 description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
```

### Comparing `balcony-0.1.7/setup.py` & `balcony-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Read any resource in your AWS Account. You can generate terraform code for them, too.',
-    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n\n![](visuals/reading-a-resource-node.gif)\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with a Docker image.\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
+    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# show documentation\nbalcony aws iam Policy --list\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\n\n`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.\n\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with a Docker image.\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
     'author': 'Oguzhan Yilmaz',
     'author_email': 'oguzhanylmz271@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 ['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
 install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'PyYAML>=6.0,<7.0',
 'boto3>=1.24.80,<2.0.0', 'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0',
 'mkdocs-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0',
 'mkdocstrings[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0',
 'rich>=13.3.4,<14.0.0', 'typer>=0.7.0,<0.8.0'] entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']} setup_kwargs = { 'name':
-'balcony', 'version': '0.1.7', 'description': 'Read any resource in your AWS
+'balcony', 'version': '0.1.8', 'description': 'Read any resource in your AWS
 Account. You can generate terraform code for them, too.', 'long_description':
 '# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-
 fill the required parameters for AWS API calls \n- Read the JSON data of any
 AWS resource in your account\n- Generate [Terraform Import Blocks](https://
@@ -19,41 +19,44 @@
 Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not
 take any action on the used AWS account.\n\n\n### [Visit the Documentation
 Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n\n###
 Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation &
 QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get
 started using _balcony_\n\n```bash title="Basic usage"\n# see
 options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n#
-read a resource\nbalcony aws s3 Buckets\n\n# generate terraform import blocks
-for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n##
-Features\n\n### Read any AWS Resource\nRelated Docs: [QuickStart](https://
-oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n\n![](visuals/reading-a-
-resource-node.gif)\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform
-v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/
-language/import) that allows users to define their imports as code.\n\n`balcony
-terraform-import  ` command generates these import blocks for you.\n\n`balcony
-terraform-import --list` to see the list of supported resources.\n\nRelated
-Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/
-balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-
-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---
-\n\n### Generate actual Terraform Resource Code \n\nIf you have:\n\n-
-initialized terraform project\n- `import_blocks.tf` file that\'s generated with
-`balcony terraform-import` command\n\nyou can run `terraform plan -generate-
-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis
-feature is achieved with a Docker image.\n\nRelated Docs: [Generate Terraform
-Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-
-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/
-balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---
-\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony
-doesn\'t know how to create terraform `import blocks` for all of the AWS
-resources.\n\nIt can be taught how to do it by creating `import-configurations`
-yaml files, but it\'s a manual process. This is where the interactive wizard
-comes in.\n\nInteractive Wizards asks you required questions to automatically
-create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform
-Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/
-terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-
-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-
-example.gif)\n', 'author': 'Oguzhan Yilmaz', 'author_email':
-'oguzhanylmz271@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+read a resource\nbalcony aws s3 Buckets\n\n# show documentation\nbalcony aws
+iam Policy --list\n\n# generate terraform import blocks for a resource\nbalcony
+terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS
+Resource\n\n`balcony aws   --paginate` command reads all resources of a given
+type in your AWS account.\n\nRelated Docs: [QuickStart](https://oguzhan-
+yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n###
+Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks]
+(https://developer.hashicorp.com/terraform/language/import) that allows users
+to define their imports as code.\n\n`balcony terraform-import  ` command
+generates these import blocks for you.\n\n`balcony terraform-import --list` to
+see the list of supported resources.\n\nRelated Docs: [Generate Terraform
+Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n!
+[](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/
+terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform
+Resource Code \n\nIf you have:\n\n- initialized terraform project\n-
+`import_blocks.tf` file that\'s generated with `balcony terraform-import`
+command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to
+generate actual `.tf` resource code.\n\nThis feature is achieved with a Docker
+image.\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://
+oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
+tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create
+balcony import configurations \n\nBalcony doesn\'t know how to create terraform
+`import blocks` for all of the AWS resources.\n\nIt can be taught how to do it
+by creating `import-configurations` yaml files, but it\'s a manual process.
+This is where the interactive wizard comes in.\n\nInteractive Wizards asks you
+required questions to automatically create the `import-configurations` yaml
+files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://
+oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
+wizard-security-groups-example.gif)\n', 'author': 'Oguzhan Yilmaz',
+'author_email': 'oguzhanylmz271@gmail.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `balcony-0.1.7/PKG-INFO` & `balcony-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.7
+Version: 0.1.8
 Summary: Read any resource in your AWS Account. You can generate terraform code for them, too.
 License: GPL-3.0-or-later
 Author: Oguzhan Yilmaz
 Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -63,26 +63,32 @@
 
 # list available resources of ec2
 balcony aws ec2 
 
 # read a resource
 balcony aws s3 Buckets
 
+# show documentation
+balcony aws iam Policy --list
+
 # generate terraform import blocks for a resource
 balcony terraform-import s3 Buckets
 ```
 
 
 ## Features
 
 ### Read any AWS Resource
+
+`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.
+
 Related Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)
 
+![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)
 
-![](visuals/reading-a-resource-node.gif)
 
 ---
 
 ### Generate Terraform Import Blocks
 
 Terraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: balcony Version: 0.1.7 Summary: Read any resource
+Metadata-Version: 2.1 Name: balcony Version: 0.1.8 Summary: Read any resource
 in your AWS Account. You can generate terraform code for them, too. License:
 GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
@@ -22,35 +22,37 @@
 Terraform Resource code balcony uses _read-only_ operations, it does not take
 any action on the used AWS account. ### [Visit the Documentation Website]
 (https://oguzhan-yilmaz.github.io/balcony/quickstart/)  ### Installation
 ```bash pip3 install balcony ``` Visit [**Installation & QuickStart Page**]
 (https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using
 _balcony_ ```bash title="Basic usage" # see options balcony # list available
 resources of ec2 balcony aws ec2 # read a resource balcony aws s3 Buckets #
-generate terraform import blocks for a resource balcony terraform-import s3
-Buckets ``` ## Features ### Read any AWS Resource Related Docs: [QuickStart]
-(https://oguzhan-yilmaz.github.io/balcony/quickstart/) ![](visuals/reading-a-
-resource-node.gif) --- ### Generate Terraform Import Blocks Terraform v1.5
-introduced [import blocks](https://developer.hashicorp.com/terraform/language/
-import) that allows users to define their imports as code. `balcony terraform-
-import  ` command generates these import blocks for you. `balcony terraform-
-import --list` to see the list of supported resources. Related Docs: [Generate
-Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-
-import/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/
-main/gifs/terraform-import-blocks-example.gif) --- ### Generate actual
-Terraform Resource Code If you have: - initialized terraform project -
-`import_blocks.tf` file that's generated with `balcony terraform-import`
-command you can run `terraform plan -generate-config-out=generated.tf` to
-generate actual `.tf` resource code. This feature is achieved with a Docker
-image. Related Docs: [Generate Terraform Code with Docker Image](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import-docker/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
-tf-code-ec2-insances-example.gif) --- ### Interactive Wizard to create balcony
-import configurations Balcony doesn't know how to create terraform `import
-blocks` for all of the AWS resources. It can be taught how to do it by creating
-`import-configurations` yaml files, but it's a manual process. This is where
-the interactive wizard comes in. Interactive Wizards asks you required
-questions to automatically create the `import-configurations` yaml files.
-Related Docs: [Terraform Import Configuration Wizard](https://oguzhan-
-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
+show documentation balcony aws iam Policy --list # generate terraform import
+blocks for a resource balcony terraform-import s3 Buckets ``` ## Features ###
+Read any AWS Resource `balcony aws   --paginate` command reads all resources of
+a given type in your AWS account. Related Docs: [QuickStart](https://oguzhan-
+yilmaz.github.io/balcony/quickstart/) ![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif) --- ### Generate
+Terraform Import Blocks Terraform v1.5 introduced [import blocks](https://
+developer.hashicorp.com/terraform/language/import) that allows users to define
+their imports as code. `balcony terraform-import  ` command generates these
+import blocks for you. `balcony terraform-import --list` to see the list of
+supported resources. Related Docs: [Generate Terraform Import Blocks](https://
+oguzhan-yilmaz.github.io/balcony/terraform-import/) ![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
+import-blocks-example.gif) --- ### Generate actual Terraform Resource Code If
+you have: - initialized terraform project - `import_blocks.tf` file that's
+generated with `balcony terraform-import` command you can run `terraform plan -
+generate-config-out=generated.tf` to generate actual `.tf` resource code. This
+feature is achieved with a Docker image. Related Docs: [Generate Terraform Code
+with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-
+docker/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/
+main/gifs/docker-gen-tf-code-ec2-insances-example.gif) --- ### Interactive
+Wizard to create balcony import configurations Balcony doesn't know how to
+create terraform `import blocks` for all of the AWS resources. It can be taught
+how to do it by creating `import-configurations` yaml files, but it's a manual
+process. This is where the interactive wizard comes in. Interactive Wizards
+asks you required questions to automatically create the `import-configurations`
+yaml files. Related Docs: [Terraform Import Configuration Wizard](https://
+oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
 raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
 wizard-security-groups-example.gif)
```

