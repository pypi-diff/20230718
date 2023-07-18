# Comparing `tmp/hityper-1.0.2.tar.gz` & `tmp/hityper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hityper-1.0.2.tar", last modified: Mon Mar 28 19:10:19 2022, max compression
+gzip compressed data, was "hityper-1.0.3.tar", last modified: Tue Jul 18 14:26:30 2023, max compression
```

## Comparing `hityper-1.0.2.tar` & `hityper-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwsr-x   0 ypeng     (4179) lyu_grp   (1018)        0 2022-03-28 19:10:19.598969 hityper-1.0.2/
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    11357 2022-03-25 10:31:27.000000 hityper-1.0.2/LICENSE
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    13938 2022-03-28 19:10:19.598969 hityper-1.0.2/PKG-INFO
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    13258 2022-03-28 05:27:01.000000 hityper-1.0.2/README.md
-drwxrwsr-x   0 ypeng     (4179) lyu_grp   (1018)        0 2022-03-28 19:10:19.598969 hityper-1.0.2/hityper/
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)      315 2022-03-28 19:10:03.000000 hityper-1.0.2/hityper/__init__.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    16518 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/__main__.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)     1000 2022-03-28 05:13:57.000000 hityper-1.0.2/hityper/config.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    14431 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/rej_typerule.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    25469 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/stdtypes.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)   102904 2022-03-28 19:07:46.000000 hityper-1.0.2/hityper/tdg.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)   123543 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/tdg_generator.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    23611 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/typeobject.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)   111314 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/typerule.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    22171 2022-03-28 05:11:07.000000 hityper-1.0.2/hityper/usertype_finder.py
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    20557 2022-03-28 19:05:42.000000 hityper-1.0.2/hityper/utils.py
-drwxrwsr-x   0 ypeng     (4179) lyu_grp   (1018)        0 2022-03-28 19:10:19.598969 hityper-1.0.2/hityper.egg-info/
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    13938 2022-03-28 19:10:19.000000 hityper-1.0.2/hityper.egg-info/PKG-INFO
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)      442 2022-03-28 19:10:19.000000 hityper-1.0.2/hityper.egg-info/SOURCES.txt
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)        1 2022-03-28 19:10:19.000000 hityper-1.0.2/hityper.egg-info/dependency_links.txt
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)       50 2022-03-28 19:10:19.000000 hityper-1.0.2/hityper.egg-info/entry_points.txt
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)      168 2022-03-28 19:10:19.000000 hityper-1.0.2/hityper.egg-info/requires.txt
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)        8 2022-03-28 19:10:19.000000 hityper-1.0.2/hityper.egg-info/top_level.txt
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)       38 2022-03-28 19:10:19.598969 hityper-1.0.2/setup.cfg
--rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)     1228 2022-03-25 10:31:27.000000 hityper-1.0.2/setup.py
+drwxrwsr-x   0 ypeng     (4179) lyu_grp   (1018)        0 2023-07-18 14:26:30.605558 hityper-1.0.3/
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    11357 2023-02-16 14:09:41.000000 hityper-1.0.3/LICENSE
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    15967 2023-07-18 14:26:30.605558 hityper-1.0.3/PKG-INFO
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    15287 2023-07-18 14:24:37.000000 hityper-1.0.3/README.md
+drwxrwsr-x   0 ypeng     (4179) lyu_grp   (1018)        0 2023-07-18 14:26:30.605558 hityper-1.0.3/hityper/
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)      313 2023-07-18 14:22:55.000000 hityper-1.0.3/hityper/__init__.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    19085 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/__main__.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)     1002 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/config.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    14389 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/rej_typerule.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    31571 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/stdtypes.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)   135663 2023-04-09 09:12:07.000000 hityper-1.0.3/hityper/tdg.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)   123701 2023-04-11 12:14:38.000000 hityper-1.0.3/hityper/tdg_generator.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    26270 2023-04-15 14:15:16.000000 hityper-1.0.3/hityper/typeobject.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)   116985 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/typerule.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    22177 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/usertype_finder.py
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    35709 2023-02-16 14:09:41.000000 hityper-1.0.3/hityper/utils.py
+drwxrwsr-x   0 ypeng     (4179) lyu_grp   (1018)        0 2023-07-18 14:26:30.605558 hityper-1.0.3/hityper.egg-info/
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)    15967 2023-07-18 14:26:29.000000 hityper-1.0.3/hityper.egg-info/PKG-INFO
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)      442 2023-07-18 14:26:30.000000 hityper-1.0.3/hityper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)        1 2023-07-18 14:26:29.000000 hityper-1.0.3/hityper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)       50 2023-07-18 14:26:29.000000 hityper-1.0.3/hityper.egg-info/entry_points.txt
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)      168 2023-07-18 14:26:29.000000 hityper-1.0.3/hityper.egg-info/requires.txt
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)        8 2023-07-18 14:26:30.000000 hityper-1.0.3/hityper.egg-info/top_level.txt
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)       38 2023-07-18 14:26:30.605558 hityper-1.0.3/setup.cfg
+-rw-rw-r--   0 ypeng     (4179) lyu_grp   (1018)     1228 2023-02-16 14:09:41.000000 hityper-1.0.3/setup.py
```

### Comparing `hityper-1.0.2/LICENSE` & `hityper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hityper-1.0.2/PKG-INFO` & `hityper-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hityper
-Version: 1.0.2
+Version: 1.0.3
 Summary: HiTyper: A hybrid type inference framework for Python
 Home-page: https://github.com/JohnnyPeng18/HiTyper
 Author: Yun Peng
 Author-email: research@yunpeng.work
 License: UNKNOWN
 Keywords: python,type inference,static analysis
 Platform: UNKNOWN
@@ -20,14 +20,22 @@
 # HiTyper
 ![](https://img.shields.io/badge/Version-1.0-blue)
 
 
 
 This is the tool released in the ICSE 2022 paper ["Static Inference Meets Deep Learning: A Hybrid Type InferenceApproach for Python"](https://arxiv.org/abs/2105.03595).
 
+## Updates
+
+**8 Aug, 2022:** 
+
+We add a new command `hityper preprocess` to transform the json files in ManyTypes4py datasets into the `groundtruth.json` and `detailed_groundtruth.json` files HiTyper needs under `hityper eval`. 
+
+We also add a new option `-g` in `hityper findusertype` to collect the `usertypes.json` HiTyper needs under `hityper eval` according to the groundtruth file `groundtruth.json`.
+
 ## Workflow
 
 HiTyper is a hybrid type inference tool built upon Type Dependency Graph (TDG), the typical workflow of it is as follows:
 
 ![](https://github.com/JohnnyPeng18/HiTyper/blob/main/imgs/workflow.png)
 
 For more details, please refer to the [paper](https://arxiv.org/abs/2105.03595).
@@ -40,25 +48,29 @@
 
 2) Deep learning models are feature-agnostic but they can hardly maintain the type correctness and are unable to predict unseen user-defined types
 
 The combination of static inference and deep learning shall complement each other and improve the coverage while maintaining the accuracy.
 
 ## Install
 
-To use HiTyper on your own computer, you can simply type:
+1. Install HiTyper from source
+
+To use HiTyper on your own computer, you can build from source: (If you need to modify the source code of HiTyper, please use this method and re-run the `pip install .` after modification each time)
 
 ```sh
-pip install hityper
+git clone https://github.com/JohnnyPeng18/HiTyper.git && cd HiTyper
+pip install .
 ```
 
-or build from source: (If you need to modify the source code of HiTyper, please use this method and re-run the `pip install .` after modification each time)
+2. Install HiTyper using `pip`
+
+You can install the latest version of HiTyper by using the following command:
 
 ```sh
-git clone https://github.com/JohnnyPeng18/HiTyper.git && cd HiTyper
-pip install .
+pip install hityper
 ```
 
 **Requirements:**
 
 - Python>=3.9
 - Linux
 
@@ -73,34 +85,57 @@
 ## Usage
 
 Currently HiTyper has the following command line options: (Some important settings are stored in file `config.py`, you may need to modify it before running HiTyper)
 
 ### findusertype
 
 ```sh
-hityper findusertype [-h] [-s SOURCE] -p REPO [-v] [-d OUTPUT_DIRECTORY]
+usage: hityper findusertype [-h] [-s SOURCE] [-p REPO] [-g GROUNDTRUTH] [-c CORE] [-v] [-d OUTPUT_DIRECTORY]
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
                         Path to a Python source file
   -p REPO, --repo REPO  Path to a Python project
+  -g GROUNDTRUTH, --groundtruth GROUNDTRUTH
+                        Path to a ground truth file
+  -c CORE, --core CORE  Number of cores to use when collecting user-defined types
   -v, --validate        Validate the imported user-defined types by finding their implementations
   -d OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
                         Path to the store the usertypes
 ```
 
-**Example:**
+**Example of collecting user-defined types in source files:**
 
 ```sh
 hityper findusertype -s python_project_repo/test.py -p python_project_repo -v -d outputs
 ```
 
 *This command generates the user-defined types collected by HiTyper and save them as `.json` files under `outputs/` folder.*
 
+`-p` option is required here, if you do not specify `-s`, the HiTyper will collect user-defined types in all files of repo specified by `-p`.
+
+**[Newly Added 6 Aug]**
+
+We add a option to automatically generate all user-defined type files that a ground truth dataset needs to evaluate HiTyper.
+
+**Example of collecting user-defined types in groundtruth datasets:**
+
+```sh
+hityper findusertype -g groundtruth.json -p repo_prefix -c 60 -d outputs
+```
+
+*This command generates the user-defined types in files indicates by `groundtruth.json` collected by HiTyper and save them as `.json` files under `outputs/` folder.*
+
+For the `groundtruth.json`, you need to use the same file in `hityper eval` command or generate it by using `hityper preprocess` command.
+
+`-p repo_prefix` is an optional argument here, if the filenames in `groundtruth.json` are the absolute paths then you do not need to specify `-p`, otherwise use `-p` to indicate which folder the source files are stored.
+
+The collection of all user-defined types for a large dataset is quite slow, try to specify a large number of cores used to make this process faster.
+
 ### gentdg
 
 ```sh
 hityper gentdg [-h] [-s SOURCE] -p REPO [-o] [-l LOCATION] [-a] [-c] [-d OUTPUT_DIRECTORY] [-f {json,pdf}]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -124,14 +159,16 @@
 hityper gentdg -s python_project_repo/test.py -p python_project_repo -d outputs -f json -o
 ```
 
 *This command generates the TDG for all functions in file `python_project_repo/test.py` and save them into `outputs` folder.* 
 
 Note that if you choose `json` format to save TDG, it will be only ONE `json` file that contains all TDGs in the source file. However, if you choose `pdf` format to save TDG, then there will be multiple `pdf` files and each one correspond to one function in the source file. This is because a pdf file can hardly contain a large TDG for every functions.
 
+For the location indicated by `-l`, use the format `funcname@classname` and use `global` as the classname if the function is a global function.
+
 HiTyper uses [PyCG](https://github.com/vitsalis/PyCG) to build call graphs in call analysis. Alias analysis and call analysis are temporarily built-in but HiTyper does not use them in inference. Further updates about them will be involved in HiTyper. 
 
 ### infer
 
 ```sh
 hityper infer [-h] [-s SOURCE] -p REPO [-l LOCATION] [-d OUTPUT_DIRECTORY] [-m RECOMMENDATIONS] [-t] [-n TOPN]
 
@@ -156,29 +193,33 @@
 hityper infer -s python_project_repo/test.py -p python_project_repo -d outputs -n 1 -t 
 ```
 
 *This command generates the inferred types for all variables, arguments and return values in the source file and save them into `output` folder.*
 
 If you do not specify `-m` or `-t` option, then HiTyper will only use the static inference part to infer types. Static inference generally takes several minutes.
 
+For the location indicated by `-l`, use the format `funcname@classname` and use `global` as the classname if the function is a global function.
+
 **Recommendation Model:**
 
 Note that HiTyper natively supports the recommendations from Type4Py and it invokes the following API provided by Type4Py to get recommendations if you use option `-t`:
 
 ```
 https://type4py.com/api/predict?tc=0
 ```
 
 **This will upload your file to the Type4Py server!** If you do not want to upload your file, you can use the [docker](https://github.com/saltudelft/type4py/wiki/Using-Type4Py-Rest-API) provided by Type4Py and changes the API in `config.py` into:
 
 ```
 http://localhost:PORT/api/predict?tc=0
 ```
 
-**HiTyper's performance deeply depends on the maximum performance of recommendation model (especially the performance to predict argument types)** 
+According to our experiments, the Type4Py model has much lower performance by quering the API above, you are suggested to train the model locally and generate the recommendation file which can be passed to `-m`.
+
+**Note: HiTyper's performance deeply depends on the maximum performance of recommendation model (especially the performance to predict argument types). Type inference of HiTyper can fail if the recommendation model cannot give a valid prediction while static inference does not work!** 
 
 If you want to use another more powerful model, you write code like `__main__.py` to adapt HiTyper to your DL model.
 
 ### eval
 
 ```sh
 hityper eval [-h] -g GROUNDTRUTH -c CLASSIFIED_GROUNDTRUTH -u USERTYPE [-m RECOMMENDATIONS] [-t] [-n TOPN]
@@ -205,14 +246,39 @@
 
 *This command evaluates the performance of HiTyper on a pre-defined groundtruth dataset. It will output similar results like stated in `Experiment Results` part.*
 
 Before evaluating Hityper using this command, please use `hityper findusertype` command to generate `usertypes.json`. This typically takes several hours, depending on the number of files.
 
 This option is designed only for future research evaluation.
 
+### Preprocess
+
+```sh
+usage: hityper preprocess [-h] -p JSON_REPO [-d OUTPUT_DIRECTORY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p JSON_REPO, --json_repo JSON_REPO
+                        Path to the repo of JSON files
+  -d OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
+                        Path to the transformed datasets
+```
+
+**Example:**
+
+```sh
+hityper preprocess -p ManyTypes4PyDataset/processed_projects_complete -d outputs
+```
+
+*This command transforms the json files in ManyTypes4Py datasets into the `groundtruth.json` and `detailed_groundtruth.json` files that required by the `hityper eval` command.*
+
+This command is to facilitate the researchers that use ManyTypes4Py dataset and want to evaluate HiTyper in it.
+
+If you want to run HiTyper in other datasets, please follow the same logic in `transformDataset` function of  `HiTyper/hityper/utils.py` to write a script.
+
 ## Experiment Results
 
 **Dataset:**
 
 The following results are evaluated using the [ManyTypes4Py](https://zenodo.org/record/4719447#.YjxcpBNBxb8) dataset. 
 
 Since the original dataset does not contain Python source files, to facilitate future research, we here also attached a [link](https://drive.google.com/file/d/1HdZyd3dKAUkiv2Nl0Zynp_YhrqU6HfMx/view?usp=sharing) for the Python source files HiTyper uses to infer types. Attached dataset is not identical with the original one because the original one contains some GitHub repos that do not allow open access or have been deleted.
@@ -236,55 +302,17 @@
 
 You can use the following command to reproduce the above results:
 
 ```sh
 hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json 
 ```
 
-**Using Type4Py's top 1 predictions as recommendations:**
-
-| Category           | Exact Match | Match to Parametric | Partial Match |
-| ------------------ | ----------- | ------------------- | ------------- |
-| Simple Types       | 67.20%      | 68.00%              | 69.80%        |
-| Generic Types      | 56.37%      | 71.05%              | 72.54%        |
-| User-defined Types | 40.42%      | 40.42%              | 43.82%        |
-| Arguments          | 22.36%      | 23.67%              | 27.56%        |
-| Return Values      | 59.11%      | 64.98%              | 69.30%        |
-| Local Variables    | 64.47%      | 68.78%              | 69.72%        |
-
-You can use the following command to reproduce the above results:
-
-```sh
-hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json -t -n 1
-```
-
-**Using Type4Py's top 10 predictions as recommendations:**
-
-| Category           | Exact Match | Match to Parametric | Partial Match |
-| ------------------ | ----------- | ------------------- | ------------- |
-| Simple Types       | 68.94%      | 69.64%              | 71.23%        |
-| Generic Types      | 57.29%      | 72.31%              | 73.68%        |
-| User-defined Types | 40.43%      | 40.43%              | 43.67%        |
-| Arguments          | 25.90%      | 27.30%              | 30.64%        |
-| Return Values      | 59.35%      | 65.25%              | 69.54%        |
-| Local Variables    | 65.21%      | 69.53%              | 70.37%        |
-
-You can use the following command to reproduce the above results:
-
-```sh
-hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json -t -n 10
-```
-
-The improvement brought by Type4Py currently is not very significant because:
-
-1) Type4Py cannot give recommendations for many hot types given by HiTyper
-
-2) Type4Py maintains low performance on predicting "rare types", which are mostly user-defined types
+We do not show the performance of HiTyper integrating different DL models here since there are many factors impacting the performance of DL models such as datasets, hyper-parameters, etc. Please align the performance by yourself before utilizing recommendations from DL models.
 
-We are currently working on building a DL model that's more suitable for HiTyper. Stay tuned!
+What's more, we are currently working on building a DL model that's more suitable for HiTyper. Stay tuned!
 
 **Other datasets:**
 
 If you want to evaluate HiTyper on other datasets, please generate files with the same format with `ManyTypes4Py_gts_test_verified.json`, `ManyTypes4Py_gts_test_verified_detailed.json`, or you can modify the code in `__main__.py`. To check a type's category, you can use `hityper.typeobject.TypeObject.checkType()`.
 
 In any case, you must also prepare the source files for static analysis.
 
@@ -300,21 +328,28 @@
 - Add supports for stub files
 
 ## Cite Us
 
 If you use HiTyper in your research, please cite us:
 
 ```latex
-@article{peng2022hityper,
-  author    = {Yun Peng and Cuiyun Gao and Zongjie Li and Bowei Gao and David Lo and Qirun Zhang and Michael R. Lyu},
-  title     = {Static Inference Meets Deep Learning: A Hybrid Type Inference Approach for Python},
-  journal   = {CoRR},
-  volume    = {abs/2105.03595},
-  year      = {2022},
-  url       = {https://arxiv.org/abs/2105.03595}
+@inproceedings{peng22hityper,
+author = {Peng, Yun and Gao, Cuiyun and Li, Zongjie and Gao, Bowei and Lo, David and Zhang, Qirun and Lyu, Michael},
+title = {Static Inference Meets Deep Learning: A Hybrid Type Inference Approach for Python},
+year = {2022},
+isbn = {9781450392211},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3510003.3510038},
+doi = {10.1145/3510003.3510038},
+booktitle = {Proceedings of the 44th International Conference on Software Engineering},
+pages = {2019–2030},
+numpages = {12},
+location = {Pittsburgh, Pennsylvania},
+series = {ICSE '22}
 }
 ```
 
 ## Contact
 
 We actively maintain this project and welcome contributions.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hityper-1.0.2/README.md` & `hityper-1.0.3/hityper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,41 @@
+Metadata-Version: 2.1
+Name: hityper
+Version: 1.0.3
+Summary: HiTyper: A hybrid type inference framework for Python
+Home-page: https://github.com/JohnnyPeng18/HiTyper
+Author: Yun Peng
+Author-email: research@yunpeng.work
+License: UNKNOWN
+Keywords: python,type inference,static analysis
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # HiTyper
 ![](https://img.shields.io/badge/Version-1.0-blue)
 
 
 
 This is the tool released in the ICSE 2022 paper ["Static Inference Meets Deep Learning: A Hybrid Type InferenceApproach for Python"](https://arxiv.org/abs/2105.03595).
 
+## Updates
+
+**8 Aug, 2022:** 
+
+We add a new command `hityper preprocess` to transform the json files in ManyTypes4py datasets into the `groundtruth.json` and `detailed_groundtruth.json` files HiTyper needs under `hityper eval`. 
+
+We also add a new option `-g` in `hityper findusertype` to collect the `usertypes.json` HiTyper needs under `hityper eval` according to the groundtruth file `groundtruth.json`.
+
 ## Workflow
 
 HiTyper is a hybrid type inference tool built upon Type Dependency Graph (TDG), the typical workflow of it is as follows:
 
 ![](https://github.com/JohnnyPeng18/HiTyper/blob/main/imgs/workflow.png)
 
 For more details, please refer to the [paper](https://arxiv.org/abs/2105.03595).
@@ -21,25 +48,29 @@
 
 2) Deep learning models are feature-agnostic but they can hardly maintain the type correctness and are unable to predict unseen user-defined types
 
 The combination of static inference and deep learning shall complement each other and improve the coverage while maintaining the accuracy.
 
 ## Install
 
-To use HiTyper on your own computer, you can simply type:
+1. Install HiTyper from source
+
+To use HiTyper on your own computer, you can build from source: (If you need to modify the source code of HiTyper, please use this method and re-run the `pip install .` after modification each time)
 
 ```sh
-pip install hityper
+git clone https://github.com/JohnnyPeng18/HiTyper.git && cd HiTyper
+pip install .
 ```
 
-or build from source: (If you need to modify the source code of HiTyper, please use this method and re-run the `pip install .` after modification each time)
+2. Install HiTyper using `pip`
+
+You can install the latest version of HiTyper by using the following command:
 
 ```sh
-git clone https://github.com/JohnnyPeng18/HiTyper.git && cd HiTyper
-pip install .
+pip install hityper
 ```
 
 **Requirements:**
 
 - Python>=3.9
 - Linux
 
@@ -54,34 +85,57 @@
 ## Usage
 
 Currently HiTyper has the following command line options: (Some important settings are stored in file `config.py`, you may need to modify it before running HiTyper)
 
 ### findusertype
 
 ```sh
-hityper findusertype [-h] [-s SOURCE] -p REPO [-v] [-d OUTPUT_DIRECTORY]
+usage: hityper findusertype [-h] [-s SOURCE] [-p REPO] [-g GROUNDTRUTH] [-c CORE] [-v] [-d OUTPUT_DIRECTORY]
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
                         Path to a Python source file
   -p REPO, --repo REPO  Path to a Python project
+  -g GROUNDTRUTH, --groundtruth GROUNDTRUTH
+                        Path to a ground truth file
+  -c CORE, --core CORE  Number of cores to use when collecting user-defined types
   -v, --validate        Validate the imported user-defined types by finding their implementations
   -d OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
                         Path to the store the usertypes
 ```
 
-**Example:**
+**Example of collecting user-defined types in source files:**
 
 ```sh
 hityper findusertype -s python_project_repo/test.py -p python_project_repo -v -d outputs
 ```
 
 *This command generates the user-defined types collected by HiTyper and save them as `.json` files under `outputs/` folder.*
 
+`-p` option is required here, if you do not specify `-s`, the HiTyper will collect user-defined types in all files of repo specified by `-p`.
+
+**[Newly Added 6 Aug]**
+
+We add a option to automatically generate all user-defined type files that a ground truth dataset needs to evaluate HiTyper.
+
+**Example of collecting user-defined types in groundtruth datasets:**
+
+```sh
+hityper findusertype -g groundtruth.json -p repo_prefix -c 60 -d outputs
+```
+
+*This command generates the user-defined types in files indicates by `groundtruth.json` collected by HiTyper and save them as `.json` files under `outputs/` folder.*
+
+For the `groundtruth.json`, you need to use the same file in `hityper eval` command or generate it by using `hityper preprocess` command.
+
+`-p repo_prefix` is an optional argument here, if the filenames in `groundtruth.json` are the absolute paths then you do not need to specify `-p`, otherwise use `-p` to indicate which folder the source files are stored.
+
+The collection of all user-defined types for a large dataset is quite slow, try to specify a large number of cores used to make this process faster.
+
 ### gentdg
 
 ```sh
 hityper gentdg [-h] [-s SOURCE] -p REPO [-o] [-l LOCATION] [-a] [-c] [-d OUTPUT_DIRECTORY] [-f {json,pdf}]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -105,14 +159,16 @@
 hityper gentdg -s python_project_repo/test.py -p python_project_repo -d outputs -f json -o
 ```
 
 *This command generates the TDG for all functions in file `python_project_repo/test.py` and save them into `outputs` folder.* 
 
 Note that if you choose `json` format to save TDG, it will be only ONE `json` file that contains all TDGs in the source file. However, if you choose `pdf` format to save TDG, then there will be multiple `pdf` files and each one correspond to one function in the source file. This is because a pdf file can hardly contain a large TDG for every functions.
 
+For the location indicated by `-l`, use the format `funcname@classname` and use `global` as the classname if the function is a global function.
+
 HiTyper uses [PyCG](https://github.com/vitsalis/PyCG) to build call graphs in call analysis. Alias analysis and call analysis are temporarily built-in but HiTyper does not use them in inference. Further updates about them will be involved in HiTyper. 
 
 ### infer
 
 ```sh
 hityper infer [-h] [-s SOURCE] -p REPO [-l LOCATION] [-d OUTPUT_DIRECTORY] [-m RECOMMENDATIONS] [-t] [-n TOPN]
 
@@ -137,29 +193,33 @@
 hityper infer -s python_project_repo/test.py -p python_project_repo -d outputs -n 1 -t 
 ```
 
 *This command generates the inferred types for all variables, arguments and return values in the source file and save them into `output` folder.*
 
 If you do not specify `-m` or `-t` option, then HiTyper will only use the static inference part to infer types. Static inference generally takes several minutes.
 
+For the location indicated by `-l`, use the format `funcname@classname` and use `global` as the classname if the function is a global function.
+
 **Recommendation Model:**
 
 Note that HiTyper natively supports the recommendations from Type4Py and it invokes the following API provided by Type4Py to get recommendations if you use option `-t`:
 
 ```
 https://type4py.com/api/predict?tc=0
 ```
 
 **This will upload your file to the Type4Py server!** If you do not want to upload your file, you can use the [docker](https://github.com/saltudelft/type4py/wiki/Using-Type4Py-Rest-API) provided by Type4Py and changes the API in `config.py` into:
 
 ```
 http://localhost:PORT/api/predict?tc=0
 ```
 
-**HiTyper's performance deeply depends on the maximum performance of recommendation model (especially the performance to predict argument types)** 
+According to our experiments, the Type4Py model has much lower performance by quering the API above, you are suggested to train the model locally and generate the recommendation file which can be passed to `-m`.
+
+**Note: HiTyper's performance deeply depends on the maximum performance of recommendation model (especially the performance to predict argument types). Type inference of HiTyper can fail if the recommendation model cannot give a valid prediction while static inference does not work!** 
 
 If you want to use another more powerful model, you write code like `__main__.py` to adapt HiTyper to your DL model.
 
 ### eval
 
 ```sh
 hityper eval [-h] -g GROUNDTRUTH -c CLASSIFIED_GROUNDTRUTH -u USERTYPE [-m RECOMMENDATIONS] [-t] [-n TOPN]
@@ -186,14 +246,39 @@
 
 *This command evaluates the performance of HiTyper on a pre-defined groundtruth dataset. It will output similar results like stated in `Experiment Results` part.*
 
 Before evaluating Hityper using this command, please use `hityper findusertype` command to generate `usertypes.json`. This typically takes several hours, depending on the number of files.
 
 This option is designed only for future research evaluation.
 
+### Preprocess
+
+```sh
+usage: hityper preprocess [-h] -p JSON_REPO [-d OUTPUT_DIRECTORY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p JSON_REPO, --json_repo JSON_REPO
+                        Path to the repo of JSON files
+  -d OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
+                        Path to the transformed datasets
+```
+
+**Example:**
+
+```sh
+hityper preprocess -p ManyTypes4PyDataset/processed_projects_complete -d outputs
+```
+
+*This command transforms the json files in ManyTypes4Py datasets into the `groundtruth.json` and `detailed_groundtruth.json` files that required by the `hityper eval` command.*
+
+This command is to facilitate the researchers that use ManyTypes4Py dataset and want to evaluate HiTyper in it.
+
+If you want to run HiTyper in other datasets, please follow the same logic in `transformDataset` function of  `HiTyper/hityper/utils.py` to write a script.
+
 ## Experiment Results
 
 **Dataset:**
 
 The following results are evaluated using the [ManyTypes4Py](https://zenodo.org/record/4719447#.YjxcpBNBxb8) dataset. 
 
 Since the original dataset does not contain Python source files, to facilitate future research, we here also attached a [link](https://drive.google.com/file/d/1HdZyd3dKAUkiv2Nl0Zynp_YhrqU6HfMx/view?usp=sharing) for the Python source files HiTyper uses to infer types. Attached dataset is not identical with the original one because the original one contains some GitHub repos that do not allow open access or have been deleted.
@@ -217,55 +302,17 @@
 
 You can use the following command to reproduce the above results:
 
 ```sh
 hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json 
 ```
 
-**Using Type4Py's top 1 predictions as recommendations:**
-
-| Category           | Exact Match | Match to Parametric | Partial Match |
-| ------------------ | ----------- | ------------------- | ------------- |
-| Simple Types       | 67.20%      | 68.00%              | 69.80%        |
-| Generic Types      | 56.37%      | 71.05%              | 72.54%        |
-| User-defined Types | 40.42%      | 40.42%              | 43.82%        |
-| Arguments          | 22.36%      | 23.67%              | 27.56%        |
-| Return Values      | 59.11%      | 64.98%              | 69.30%        |
-| Local Variables    | 64.47%      | 68.78%              | 69.72%        |
+We do not show the performance of HiTyper integrating different DL models here since there are many factors impacting the performance of DL models such as datasets, hyper-parameters, etc. Please align the performance by yourself before utilizing recommendations from DL models.
 
-You can use the following command to reproduce the above results:
-
-```sh
-hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json -t -n 1
-```
-
-**Using Type4Py's top 10 predictions as recommendations:**
-
-| Category           | Exact Match | Match to Parametric | Partial Match |
-| ------------------ | ----------- | ------------------- | ------------- |
-| Simple Types       | 68.94%      | 69.64%              | 71.23%        |
-| Generic Types      | 57.29%      | 72.31%              | 73.68%        |
-| User-defined Types | 40.43%      | 40.43%              | 43.67%        |
-| Arguments          | 25.90%      | 27.30%              | 30.64%        |
-| Return Values      | 59.35%      | 65.25%              | 69.54%        |
-| Local Variables    | 65.21%      | 69.53%              | 70.37%        |
-
-You can use the following command to reproduce the above results:
-
-```sh
-hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json -t -n 10
-```
-
-The improvement brought by Type4Py currently is not very significant because:
-
-1) Type4Py cannot give recommendations for many hot types given by HiTyper
-
-2) Type4Py maintains low performance on predicting "rare types", which are mostly user-defined types
-
-We are currently working on building a DL model that's more suitable for HiTyper. Stay tuned!
+What's more, we are currently working on building a DL model that's more suitable for HiTyper. Stay tuned!
 
 **Other datasets:**
 
 If you want to evaluate HiTyper on other datasets, please generate files with the same format with `ManyTypes4Py_gts_test_verified.json`, `ManyTypes4Py_gts_test_verified_detailed.json`, or you can modify the code in `__main__.py`. To check a type's category, you can use `hityper.typeobject.TypeObject.checkType()`.
 
 In any case, you must also prepare the source files for static analysis.
 
@@ -281,23 +328,32 @@
 - Add supports for stub files
 
 ## Cite Us
 
 If you use HiTyper in your research, please cite us:
 
 ```latex
-@article{peng2022hityper,
-  author    = {Yun Peng and Cuiyun Gao and Zongjie Li and Bowei Gao and David Lo and Qirun Zhang and Michael R. Lyu},
-  title     = {Static Inference Meets Deep Learning: A Hybrid Type Inference Approach for Python},
-  journal   = {CoRR},
-  volume    = {abs/2105.03595},
-  year      = {2022},
-  url       = {https://arxiv.org/abs/2105.03595}
+@inproceedings{peng22hityper,
+author = {Peng, Yun and Gao, Cuiyun and Li, Zongjie and Gao, Bowei and Lo, David and Zhang, Qirun and Lyu, Michael},
+title = {Static Inference Meets Deep Learning: A Hybrid Type Inference Approach for Python},
+year = {2022},
+isbn = {9781450392211},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3510003.3510038},
+doi = {10.1145/3510003.3510038},
+booktitle = {Proceedings of the 44th International Conference on Software Engineering},
+pages = {2019–2030},
+numpages = {12},
+location = {Pittsburgh, Pennsylvania},
+series = {ICSE '22}
 }
 ```
 
 ## Contact
 
 We actively maintain this project and welcome contributions. 
 
 If you have any question, please contact research@yunpeng.work.
 
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hityper-1.0.2/hityper/__main__.py` & `hityper-1.0.3/hityper/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 import ast
 import os
 import json
 import traceback
 from hityper.tdg_generator import TDGGenerator
 from hityper.usertype_finder import UsertypeFinder
-from hityper.utils import formatUserTypes, getRecommendations, test_multiplefile
+from hityper.utils import formatUserTypes, getRecommendations, test_multiplefile, transformDataset, collectUserTypeset
 from hityper.config import config
 from hityper import logger
 from hityper.utils import detectChange, SimModel
 import logging
 from tqdm import tqdm
 
 logger.name = __name__
@@ -22,17 +22,23 @@
     formatter = logging.Formatter('%(asctime)s[%(levelname)s][%(filename)s:%(lineno)d] %(message)s')
     fh.setFormatter(formatter)
     logger.addHandler(fh)
     
 
 
 def findusertype(args):
-    if args.repo:
-        outputrepo = args.output_directory if args.output_directory else "."
-        setuplogs(outputrepo)
+    outputrepo = args.output_directory if args.output_directory else "."
+    setuplogs(outputrepo)
+    if args.groundtruth:
+        if args.repo:
+            outfile = collectUserTypeset(args.groundtruth, filerepo = args.repo, cores = args.core, outputdir = outputrepo)
+        else:
+            outfile = collectUserTypeset(args.groundtruth, cores = args.core, outputdir = outputrepo)
+        logger.info("Saved collected user-defined types to {}.".format(outfile))
+    elif args.repo:
         if args.source:
             try:
                 source = open(args.source, "r", encoding = "utf-8").read()
                 root = ast.parse(source)
                 usertypefinder = UsertypeFinder(args.source, args.repo, args.validate)
                 usertypes, _ = usertypefinder.run(root)
                 with open(outputrepo + "/" + args.source.replace("/", "_").replace(".py", "_USERTYPES.json"), "w", encoding = "utf-8") as of:
@@ -73,15 +79,15 @@
             if not os.path.isfile(args.source):
                 logger.error("Cannot find source file {}".format(args.source))
             try:
                 source = open(args.source, "r", encoding = "utf-8").read()
                 root = ast.parse(source)
                 usertypefinder = UsertypeFinder(args.source, args.repo, True)
                 usertypes, _ = usertypefinder.run(root)
-                generator = TDGGenerator(args.source, args.optimize, args.location, usertypes, alias = 1 if args.alias_analysis else 0, repo = args.repo if args.call_analysis else None)
+                generator = TDGGenerator(args.source, args.optimize, [args.location], usertypes, alias = 1 if args.alias_analysis else 0, repo = args.repo if args.call_analysis else None)
                 global_tg = generator.run(root)
                 if args.output_format == "json":
                     with open(outputrepo + "/" + args.source.replace("/", "_").replace(".py", "_TDG.json"), "w", encoding = "utf-8") as of:
                         of.write(json.dumps(global_tg.dump(), sort_keys=True, indent=4, separators=(',', ': ')))
                         logger.info("Saved TDGs to {}".format(outputrepo + "/" + args.source.replace("/", "_").replace(".py", "_TDG.json")))
                 else:
                     for tg in global_tg.tgs:
@@ -96,15 +102,15 @@
             for f in tqdm(files):
                 if os.path.isfile(f):
                     try:
                         source = open(f, "r", encoding = "utf-8").read()
                         root = ast.parse(source)
                         usertypefinder = UsertypeFinder(f, args.repo, True)
                         usertypes, _ = usertypefinder.run(root)
-                        generator = TDGGenerator(f, args.optimize, args.location, usertypes, alias = 1 if args.alias_analysis else 0, repo = args.repo if args.call_analysis else None)
+                        generator = TDGGenerator(f, args.optimize, [args.location], usertypes, alias = 1 if args.alias_analysis else 0, repo = args.repo if args.call_analysis else None)
                         global_tg = generator.run(root)
                     except Exception as e:
                         traceback.print_exc()
                         logger.error("Failed to generate TDG for file {}, reason: {}".format(f, e))
                     if args.output_format == "json":
                         with open(outputrepo + "/" + f.replace("/", "_").replace(".py", "_TDG.json"), "w", encoding = "utf-8") as of:
                             of.write(json.dumps(global_tg.dump(), sort_keys=True, indent=4, separators=(',', ': ')))
@@ -137,23 +143,29 @@
             if not os.path.isfile(args.source):
                 logger.error("Cannot find source file {}".format(args.source))
             try:
                 source = open(args.source, "r", encoding = "utf-8").read()
                 root = ast.parse(source)
                 usertypefinder = UsertypeFinder(args.source, args.repo, True)
                 usertypes, _ = usertypefinder.run(root)
-                generator = TDGGenerator(args.source, True, args.location, usertypes, alias = 0, repo = None)
+                generator = TDGGenerator(args.source, True, [args.location], usertypes, alias = 0, repo = None)
                 global_tg = generator.run(root)
                 str_results = {}
-                global_tg.passTypes(debug = False)
-                str_results["global@global"] = global_tg.dumptypes()
                 if recommendations == None and args.type4py:
                     recommendations = getRecommendations(source)
-                elif isinstance(recommendations, dict) and f in recommendations:
-                            recommendations = recommendations[f]
+                elif isinstance(recommendations, dict) and args.source in recommendations:
+                    recommendations = recommendations[args.source]
+                if recommendations != None:
+                    global_tg.passTypes(debug = False)
+                    global_tg.recommendType(recommendations, formatUserTypes(usertypes), usertypes["module"], args.topn, simmodel = simmodel)
+                    global_tg.passTypes(debug = False)
+                else:
+                    global_tg.passTypes(debug = False)
+                global_tg.simplifyTypes()
+                str_results["global@global"] = global_tg.dumptypes()
                 for tg in global_tg.tgs:
                     if recommendations != None:
                         changed = True
                         iters = 0
                         while changed and iters < config["max_recommendation_iteration"]:
                             iters += 1
                             tg.passTypes(debug = False)
@@ -179,32 +191,33 @@
             for f in tqdm(files):
                 if os.path.isfile(f):
                     try:
                         source = open(f, "r", encoding = "utf-8").read()
                         root = ast.parse(source)
                         usertypefinder = UsertypeFinder(f, args.repo, True)
                         usertypes, _ = usertypefinder.run(root)
-                        generator = TDGGenerator(f, True, args.location, usertypes, alias = 0, repo = None)
+                        generator = TDGGenerator(f, True, None, usertypes, alias = 0, repo = None)
                         global_tg = generator.run(root)
                         str_results = {}
                         global_tg.passTypes(debug = False)
                         str_results["global@global"] = global_tg.dumptypes()
+                        single_recommendations = None
                         if recommendations == None and args.type4py:
-                            recommendations = getRecommendations(source)
+                            single_recommendations = getRecommendations(source)
                         elif isinstance(recommendations, dict) and f in recommendations:
-                            recommendations = recommendations[f]
+                            single_recommendations = recommendations[f]
                         for tg in global_tg.tgs:
-                            if recommendations != None:
+                            if single_recommendations != None:
                                 changed = True
                                 iters = 0
                                 while changed and iters < config["max_recommendation_iteration"]:
                                     iters += 1
                                     tg.passTypes(debug = False)
                                     types = tg.findHotTypes()
-                                    tg.recommendType(types, recommendations, formatUserTypes(usertypes), usertypes["module"], args.topn, simmodel = simmodel)
+                                    tg.recommendType(types, single_recommendations, formatUserTypes(usertypes), usertypes["module"], args.topn, simmodel = simmodel)
                                     tg.passTypes(debug = False)
                                     new_types = tg.findHotTypes()
                                     changed = detectChange(types, new_types)
                                     tg.simplifyTypes()
                             else:
                                 tg.passTypes(debug = False)
                                 tg.simplifyTypes()
@@ -215,27 +228,41 @@
                         logger.error("Type inference failed for file {}, reason: {}".format(f, e))
             with open(outputrepo + "/" + args.repo.replace("/", "_") + "_INFERREDTYPES.json", "w", encoding = "utf-8") as of:
                 of.write(json.dumps(results, sort_keys=True, indent=4, separators=(',', ': ')))
             logger.info("Saved results to {}".format(outputrepo + "/" + args.repo.replace("/", "_") + "_INFERREDTYPES.json"))
 
 
 def evaluate(args):
-    setuplogs(".")
-    test_multiplefile(args.groundtruth, args.classified_groundtruth, args.usertype, recfile = args.recommendations if args.recommendations else None, recmodel = args.type4py, topn = args.topn)
+    outputrepo = args.output_directory if args.output_directory else "."
+    setuplogs(outputrepo)
+    predictions = test_multiplefile(args.groundtruth, args.classified_groundtruth, args.usertype, recfile = args.recommendations if args.recommendations else None, recmodel = args.type4py, topn = args.topn, prefix = args.file_prefix, eval = True)
+    with open(outputrepo + "/" + args.groundtruth.replace("/", "_").replace(".json", "_INFERREDTYPES.json"), "w", encoding = "utf-8") as of:
+        of.write(json.dumps(predictions, sort_keys=True, indent=4, separators=(',', ': ')))
+    logger.info("Saved predictions to {}".format(outputrepo + "/" + args.groundtruth.replace("/", "_").replace(".json", "_INFERREDTYPES.json")))
+
+
+def preprocess(args):
+    outputrepo = args.output_directory if args.output_directory else "."
+    setuplogs(outputrepo)
+    outputfiles = transformDataset(args.json_repo, outputdir = outputrepo)
+    logger.info("Saved transformed datasets to {} and {}".format(outputfiles[0], outputfiles[1]))
+
 
 
 
 
 def main():
     arg_parser = argparse.ArgumentParser()
     sub_parsers = arg_parser.add_subparsers(dest='cmd')
 
     usertype_parser = sub_parsers.add_parser('findusertype')
     usertype_parser.add_argument('-s', '--source', required = False, type=str, help = "Path to a Python source file")
-    usertype_parser.add_argument('-p', '--repo', required = True, type=str, help = "Path to a Python project")
+    usertype_parser.add_argument('-p', '--repo', required = False, type=str, help = "Path to a Python project")
+    usertype_parser.add_argument('-g', '--groundtruth', required = False, type=str, help = "Path to a ground truth file")
+    usertype_parser.add_argument('-c', "--core", default = 8, type=int, help = "Number of cores to use when collecting user-defined types")
     usertype_parser.add_argument("-v", "--validate", default = True, action="store_true", help = "Validate the imported user-defined types by finding their implementations")
     usertype_parser.add_argument('-d', "--output_directory", required = False, type=str, help = "Path to the store the usertypes")
     usertype_parser.set_defaults(func = findusertype)
 
     tdg_parser = sub_parsers.add_parser('gentdg')
     tdg_parser.add_argument('-s', '--source', required = False, type=str, help = "Path to a Python source file")
     tdg_parser.add_argument('-p', '--repo', required = True, type=str, help = "Path to a Python project")
@@ -262,16 +289,24 @@
     eval_parser = sub_parsers.add_parser('eval')
     eval_parser.add_argument('-g', '--groundtruth', required = True, type=str, help = "Path to a ground truth dataset")
     eval_parser.add_argument('-c', '--classified_groundtruth', required = True, type=str, help = "Path to a classified ground truth dataset")
     eval_parser.add_argument('-u', '--usertype', required = True, type=str, help = "Path to a previously collected user-defined type set")
     eval_parser.add_argument('-m', "--recommendations", required = False, type=str, help = "Path to the recommendations generated by a DL model")
     eval_parser.add_argument('-t', "--type4py", default = False, action="store_true", help = "Use Type4Py as the recommendation model")
     eval_parser.add_argument('-n', "--topn", default = 1, type = int, help = "Indicate the top n predictions from DL models used by HiTyper")
+    eval_parser.add_argument('-d', "--output_directory", required = False, type=str, help = "Path to the inferred results")
+    eval_parser.add_argument('-p', "--file_prefix", required = False, type=str, help = "Path prefix to the files in ground truth dataset")
     eval_parser.set_defaults(func = evaluate)
 
+    preprocess_parser = sub_parsers.add_parser('preprocess')
+    preprocess_parser.add_argument("-p", '--json_repo', required = True, type = str, help = "Path to the repo of JSON files")
+    preprocess_parser.add_argument('-d', "--output_directory", required = False, type=str, help = "Path to the transformed datasets")
+    preprocess_parser.set_defaults(func = preprocess)
+
+
 
     args = arg_parser.parse_args()
     args.func(args)
 
 if __name__ == "__main__":
     main()
```

### Comparing `hityper-1.0.2/hityper/config.py` & `hityper-1.0.3/hityper/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 config = {
 
     #Indicate the web API that HiTyper should call to invoke the DL model
-    "type4py": "https://type4py.com/api/predict?tc=0",
+    "type4py": "http://localhost:5001/api/predict?tc=0",
 
     #Indicate the default DL model used in HiTyper
     "default_model": "type4py",
 
     #Indicate the maximum iterations that HiTyper iterates the whole TDG to conduct static inference
     "max_tdg_iteration": 100,
```

### Comparing `hityper-1.0.2/hityper/rej_typerule.py` & `hityper-1.0.3/hityper/rej_typerule.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,14 @@
         rej_list = [rej_ltypes]
         for n in range(1, len(operands)):
             rej_each = operands[n].rejtypes
             rej_list.append(rej_each)
         return rej_list
 
     def unknown_op(self,outs,operands,op):
-        print("Unknown Operation: " + op)
         rej_list = []
         for node in operands:
             rej_each = node.rejtypes
             rej_list.append(rej_each)
         return rej_list
 
     def rej_call(self, outs, operands, func, attr, usertypes):
```

### Comparing `hityper-1.0.2/hityper/stdtypes.py` & `hityper-1.0.3/hityper/stdtypes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,54 @@
 
 #The builtin types are collected from https://docs.python.org/zh-cn/3/library/stdtypes.html
 builtins = [
 "int", "float", "complex", "bool", "list", "tuple", "range", "str", "bytes", "bytearray", "memoryview", "set", "frozenset", "dict", "dict_keys", "dict_values", "dict_items", "None"
 ]
 
+ops = [
+"+", "-", "*", "/", "//", "%", "<<", ">>", "|", "^", "&", "@", "not", "~", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"
+]
+
+method2op = {
+    "__add__": "+",
+    "__sub__": "-",
+    "__mul__": "*",
+    "__truediv__": "/",
+    "__floordiv__": "//",
+    "__mod__": "%",
+    "__pow__": "**",
+    "__lshift__": "<<",
+    "__rshift__": ">>",
+    "__and__": "&",
+    "__or__": "|",
+    "__xor__": "^",
+    "__lt__": "<",
+    "__gt__": ">",
+    "__le__": "<=",
+    "__ge__": ">=",
+    "__eq__": "==",
+    "__ne__": "!=",
+    "__neg__": "-",
+    "__pos__": "+",
+    "__invert__": "~",
+    "__isub__": "-",
+    "__iadd__": "+",
+    "__imul__": "*",
+    "__idiv__": "/",
+    "__ifloordiv__": "//",
+    "__imod__": "%",
+    "__ipow__": "**",
+    "__ilshift__": "<<",
+    "__irshift__": ">>",
+    "__iand__": "&",
+    "__ior__": "|",
+    "__ixor__": "^",
+    "__iter__": "in"
+}
+
 
 #The following functions will not be automatcally inferred using the type templates in builtin_method, HiTyper has explicit rules to handle them in typerule.py
 builtin_method_properties = {
     #The following methods change the types of caller instead of return some new types
     "self-changable": {
         "list": ["append", "clear", "extend", "insert", "pop", "remove"],
         "set": ["update", "intersection_update", "difference_update", "symmetric_difference_update", "add", "remove", "discard", "pop", "clear"],
@@ -21,18 +62,18 @@
         "set": ["pop"],
         "dict": ["items", "keys", "values", "pop", "popitem", "get"],
         "overall": ["abs", "divmod", "enumerate", "frozenset", "list", "next", "round", "set", "sorted", "sum", "tuple", "type", "max", "min", "copy", "items", "keys", "values", "pop", "popitem", "get"]
     }
 }
 
 special_types = {
-    "@iterable@": ["list", "tuple", "range", "str", "bytes", "bytearray", "set", "frozenset", "dict"],
+    "@iterable@": ["list", "tuple", "range", "str", "bytes", "bytearray", "set", "frozenset", "dict", "Generator", "IO"],
     "@byte-like@": ["bytes", "bytearray"],
     "@set-like@": ["set", "frozenset"],
-    "@subscriptable@": ["list", "tuple", "str", "bytes", "bytearray"],
+    "@subscriptable@": ["list", "tuple", "str", "bytes", "bytearray", "dict"],
     "@number@": ["bool", "int", "float", "complex"],
     "@hashable@": [],
     "@sequence@": ["str", "bytes", "bytearray", "tuple", "list", "range"],
     "@collection@": ["set", "frozenset", "dict"],
     "@path-like@": ["str", "bytes"]
 }
 
@@ -90,14 +131,64 @@
     "abs": "__abs__",
     "hash": "__hash__",
     "next": "__next__",
     "repr": "__repr__",
     "str": "__str__"
 }
 
+
+builtin_op = {
+    "left": {
+        "int": ["+", "-", "*", "/", "//", "%", "<<", ">>", "|", "^", "&", "not", "~", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "float": ["+", "-", "*", "/", "//", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "complex": ["+", "-", "*", "/", "not", "and", "or", "==", "!=", "is", "is not", "in", "not in" ],
+        "bool": ["+", "-", "*", "/", "//", "%", "<<", ">>", "|", "^", "&", "not", "~", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "list": ["+", "*", "not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "tuple": ["+", "*", "not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "range": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "str": ["+", "*", "%", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "bytes": ["+", "*", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "bytearray": ["+", "*", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "memoryview": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "set": ["-", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "fronzeset": ["-", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "dict": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "dict_keys": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "dict_values": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "dict_items": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "None": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "Generator": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "Iterable": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "Callable": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"]
+    },
+    "right": {
+        "int": ["+", "-", "*", "/", "//", "%", "<<", ">>", "|", "^", "&", "not", "~", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not"],
+        "float": ["+", "-", "*", "/", "//", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not"],
+        "complex": ["+", "-", "*", "/", "not", "and", "or", "==", "!=", "is", "is not"],
+        "bool": ["+", "-", "*", "/", "//", "%", "<<", ">>", "|", "^", "&", "not", "~", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not"],
+        "list": ["+", "*", "not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "tuple": ["+", "*", "not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "range": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "str": ["+", "*", "%", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "bytes": ["+", "*", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "bytearray": ["+", "*", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "memoryview": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "set": ["-", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "fronzeset": ["-", "not", "and", "or", "==", "!=", "<", "<=", ">", ">=", "is", "is not", "in", "not in"],
+        "dict": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "dict_keys": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "dict_values": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "dict_items": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "None": ["not", "and", "or", "==", "!=", "is", "is not"],
+        "Generator": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "Iterable": ["not", "and", "or", "==", "!=", "is", "is not", "in", "not in"],
+        "Callable": ["not", "and", "or", "==", "!=", "is", "is not"]
+    }
+}
+
 #functions with dynamic features are not included
 builtin_method = {
     "standalone": {
         "abs": [[("x", "@number@")], "@originaltype@"],
         "all": [[("iterable", "@iterable@")], "bool"],
         "any": [[("iterable", "@iterable@")], "bool"],
         "ascii": [[("object", "Any")], "str"],
@@ -157,15 +248,15 @@
     },
     "list": {
         "index": [[("x", "@elementtype@"), ["i", "int"], ["j", "int"]], "int"],
         "count": [[("x", "@elementtype@")], "int"],
         "append": [[("x", "Any")], "None"],
         "clear": [[], "None"],
         "copy": [[], "@originaltype@"],
-        "extend": [[("t", "List")], "None"],
+        "extend": [[("t", "@iterable@")], "None"],
         "insert": [[("i", "int"), ("x", "Any")], "None"],
         "pop": [[["i", "int"]], "None"],
         "remove": [[("x", "@elementtype@")], "None"],
         "reverse": [[], "None"],
         "sort": [[["key", "Callable"], ["reverse", "bool"]], "None"]
     },
     "tuple": {
@@ -355,14 +446,31 @@
         "items": [[], "dict_items[List[Tuple[@keytype@, @valuetype@]]]"],
         "keys": [[], "dict_keys[List[@keytype@]]"],
         "pop": [[("key", "@keytype@")], "@valuetype@"],
         "popitem": [[], "Tuple[@keytype@, @valuetype@]"],
         "setdefault": [[("key", "Any")], "dict"],
         "update": [[("other", "dict")], [("other", "@iterable@")], "dict"],
         "values": [[], "dict_values[List[@valuetype@]]"]
+    },
+    "Generator": {
+        "__iter__": [],
+        "__next__": [],
+        "send": [],
+        "throw": [],
+        "close": []
+    },
+    "Iterable": {
+        "__iter__": []
+    },
+    "Callable": {
+        "__call__": []
+    },
+    "IO": {
+        "close": [],
+        "read": [[], "str"]
     }
 
 }
 
 
 
 
@@ -392,38 +500,41 @@
 #The types in collections module are extracted from https://docs.python.org/zh-cn/3/library/collections.abc.html
 collections_abc_module = [
 "Container", "Hashable", "Iterable", "Iterator", "Reversible", "Generator", "Sized", "Callable", "Collection", "Sequence", "MutableSequence",
 "ByteString", "Set", "MutableSet", "Mapping", "MutableMapping", "MappingView", "ItemsView", "KeysView", "ValuesView", "Awaitable", "Coroutine",
 "AsyncIterable", "AsyncIterator", "AsyncGenerator"
 ]
 
+
 #The standard errors are extracted from https://docs.python.org/zh-cn/3/library/exceptions.html
 errors = [
 "BaseException", "Exception", "ArithmeticError", "BufferError", "LookupError", "AssertionError", "AttributeError", "EOFError", "GeneratorExit", "ImportError",
 "ModuleNotFoundError", "IndexError", "KeyError", "KeyboardInterrupt", "MemoryError", "NameError", "NotImplementedError", "OSError", "OverflowError", "RecursionError",
 "ReferenceError", "RuntimeError", "StopIteration", "StopAsyncIteration", "SyntaxError", "IndentationError", "TabError", "SystemError", "SystemExit", "TypeError",
 "UnboundLocalError", "UnicodeError", "UnicodeEncodeError", "UnicodeTranslateError", "ValueError", "ZeroDivisionError", "EnvironmentError", "IOError", "WindowsError",
 "BlockingIOError", "ChildProcessError", "ConnectionError", "BrokenPipeError", "ConnectionAbortedError", "ConnectionRefusedError", "ConnectionResetError", 
 "FileExistsError", "FileNotFoundError", "InterruptedError", "IsADirectoryError", "NotADirectoryError", "PermissionError", "ProcessLookupError", "TimeoutError"
 ]
 
-#The standard errors are extracted from https://docs.python.org/zh-cn/3/library/exceptions.html
+#The standard warnings are extracted from https://docs.python.org/zh-cn/3/library/exceptions.html
 warnings = [
 "Warning", "DeprecationWarning", "PendingDeprecationWarning", "RuntimeWarning", "SyntaxWarning", "UserWarning", "FutureWarning", "ImportWarning", "UnicodeWarning",
 "BytesWarning", "EncodingWarning", "ResourceWarning"
 ]
 
 
 stdtypes = {
     "typing": typing_module,
     "collections": collections_module,
     "collections_abc": collections_abc_module,
     "builtins": builtins,
     "errors": errors,
     "warnings": warnings,
+    "generic": ["list", "tuple", "set", "frozenset", "dict", "Pattern", "Match", "Generator", "Callable", "Iterable"],
+    "simple": ["int", "float", "complex", "bool", "str", "bytes", "bytearray", "memoryview", "None", "Exception", "Warning", "Any"],
     "overall": typing_module + builtins + collections_module + collections_abc_module + errors + warnings
 }
 
 
 #This map converts the types stored in TypeObject to commonly used type names in source code
 exporttypemap = {}
 for i in stdtypes["builtins"]:
@@ -461,23 +572,29 @@
         for j in stdtypes["warnings"]:
             typestr = j
             if typestr.lower() not in inputtypemap:
                 inputtypemap[typestr.lower()] = j 
         for j in stdtypes["typing"]:
             typestr = "typing." + j
             if typestr.lower() not in inputtypemap:
-                inputtypemap[typestr.lower()] = j 
+                inputtypemap[typestr.lower()] = j
+            if  j.lower() not in inputtypemap:
+                inputtypemap[j.lower()] = j
         for j in stdtypes["collections"]:
             typestr = "collections." + j
             if typestr.lower() not in inputtypemap:
                 inputtypemap[typestr.lower()] = j 
+            if  j.lower() not in inputtypemap:
+                inputtypemap[j.lower()] = j
         for j in stdtypes["collections_abc"]:
             typestr = "collections_abc." + j
             if typestr.lower() not in inputtypemap:
                 inputtypemap[typestr.lower()] = j 
+            if  j.lower() not in inputtypemap:
+                inputtypemap[j.lower()] = j
 
 
 
 
 
 #This map provide the comparison between standard types as there may exist mutiple types name actually pointing one type.
 typeequalmap = {
```

### Comparing `hityper-1.0.2/hityper/tdg.py` & `hityper-1.0.3/hityper/tdg.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.name = name
         self.lineno = 0
         self.columnno = 0
         self.columnend = 0
         self.tg = None
         self.rejtypes = []
         self.nodeid = "Not Assigned"
+        self.tag = 0
 
         #visitlabel: 0 - this node is never visited
         #1 - state of input node of this node is not determined, move to queue and wait
         #2 - this node is finalized and can pass message to neighbors
         self.visitlabel = 0
 
     def setNodePos(self, lineno, columnno, columnend):
@@ -154,14 +155,18 @@
         #2 - add user defined type
         #3 - dynamically change types using flow algorithm
         #4 - add from DL model
         self.tag = 0
 
         #indicate whether the type set changes or not during last operation
         self.change = False
+    
+    def cleartypes(self):
+        self.types = []
+
 
     def addTypes(self, t, tag, independent_op = True):
         if independent_op:
             self.change = False
         if(type(t) == type([])):
             for i in t:
                 if (isinstance(i, TypeObject) and i not in self.types):
@@ -253,26 +258,31 @@
         self.nodetype = "TypeGen"
         self.op = operation
         #for Call AST nodes
         self.func = func
         #for Attribute AST nodes
         self.attr = attr
         self.types = []
-        self.splitindex = 0
+        self.splitindex = splitindex
         self.rejinputtypes = []
 
     def setFunc(self, func):
         self.func = func
 
     def checktypes(self):
         for n in self.ins:
             if len(n.types) == 0:
                 return False
         return True
 
+    def cleartypes(self):
+        self.rejinputtypes = []
+        self.types = []
+
+
     def performTypingRules(self, usertype = None, iterable=False):
         # if it's not about ierable or it's call -> format(which may cause more than 3 input nodes)
         #if not iterable and not(self.op == "call" and (self.func in call_overargu_funcs)):
         if not iterable and self.op != "call":
         # if not iterable and not (self.op=="call" and self.func=="format") and not (self.op=="call" and (self.func=="count" or self.func=="index" or self.func=="endswith")):
             # since it's possible that the length of ins is more than 3 when x if xx else xx is concerned, we don't check the len of ins
             # e.g state = (IOLoop.READ if readable else 0) | (IOLoop.WRITE if writable else 0)
@@ -302,15 +312,16 @@
                         raise ValueError("Incorrect number of rejected types " + "in " + self.op + " at Line: " + str(self.lineno) )
                 elif self.checktypes():
                     for i,n in enumerate(self.rejinputtypes):
                         if len(n) != 0:
                             norej = False
                         if i < len(self.ins):
                             for t in n:
-                                if t.added and t not in self.ins[i].rejtypes:
+                                if t not in self.ins[i].rejtypes and t.category != 2 and not isinstance(self.ins[i], TypeNode):
+                                    logger.info("Reject {} for node {} in op {}.".format(TypeObject.resolveTypeName(t), self.ins[i].name, self.op if self.op != "call" else self.func))
                                     self.ins[i].rejtypes.append(t)
             else:
                 raise ValueError("outputs should have at least 3 elements.")
         # if it's list_write or tuple_write
         else:
             if len(outputs) == 2:
                 self.rejinputtypes = outputs[0]
@@ -322,15 +333,16 @@
                     raise ValueError("Incorrect number of rejected types.")
                 else:
                     for i,n in enumerate(self.rejinputtypes):
                         if len(n) != 0:
                             norej = False
                         if i < len(self.ins):
                             for t in n:
-                                if t.added and t not in self.ins[i].rejtypes:
+                                if t not in self.ins[i].rejtypest not in self.ins[i].rejtypes and t.category != 2 and not isinstance(self.ins[i], TypeNode):
+                                    logger.info(f"Reject {TypeObject.resolveTypeName(t)} for node {self.ins[i].name} in op {self.op}.")
                                     self.ins[i].rejtypes.append(t)
         return norej
 
     def performRejTypingRule(self, usertype = None, iterable = False):
         rejtyperule = Rej_TypingRule()
         rejtypes = rejtyperule.act(self, self.ins, self.op, self.func, self.attr, usertype, iterable = iterable)
         if len(rejtypes) != len(self.ins):
@@ -460,14 +472,19 @@
         self.branchvar = var
         self.outtypes = []
         self.types = [[], []]
         self.rejtypes = [[], []]
     
     def addTypes(self, types):
         self.outtypes = types
+    
+    def cleartypes(self):
+        self.outtypes = []
+        self.types = [[], []]
+        self.rejtypes = [[], []]
 
     def splitTypes(self):
         if len(self.ins) != 1:
             logger.error("Branch node must have exactly one input node.")
             raise ValueError("Branch node must have exactly one input node.")
         elif len(self.outs) != 2:
             logger.error("Branch node must have exactly two output nodes.")
@@ -481,14 +498,17 @@
                         types.remove(removetype)
             self.types = []
             for t in self.outtypes:
                 if t != None:
                     self.types.append([t])
                 else:
                     self.types.append(TypeObject.removeInclusiveTypes(types))
+            if len(self.types) < 2:
+                for i in range(0, 2 - len(self.types)):
+                    self.types.append([])
     
     def dump(self):
         node = self._dump()
         node["nodetype"] = self.nodetype
         node["branchvar"] = self.branchvar
         node["outtypes"] = []
         for t in self.outtypes:
@@ -557,14 +577,17 @@
 class MergeNode(GraphBaseNode):
     def __init__(self, ins, outs, var):
         super(MergeNode, self).__init__(ins, outs, "merge")
         self.nodetype = "Merge"
         self.mergevar = var
         self.types = []
 
+    def cleartypes(self):
+        self.types = []
+
     def dump(self):
         node = self._dump()
         node["nodetype"] = self.nodetype
         node["mergevar"] = self.mergevar
         node["types"] = []
         for t in self.types:
             node["types"].append(t.dump())
@@ -791,24 +814,229 @@
         if len(self.returnvaluenodes) == 0:
             return [TypeObject("None",0)]
         for r in self.returnvaluenodes:
             returntype += r.types
         return returntype
 
 
+    def getDefPath(self, end, iteration, prev_nodes):
+        if len(end.ins) == 0:
+            return [[end]]
+        elif isinstance(end, TypeGenNode) and end.op == "call":
+            return [[end]]
+        elif iteration > config["max_tdg_iteration"]:
+            return []
+        else:
+            subpaths = []
+            for o in end.ins:
+                if o in prev_nodes:
+                    continue
+                if isinstance(o, SymbolNode) and o.scope != "local":
+                    continue
+                subpath = self.getDefPath(o, iteration + 1, prev_nodes + [end])
+                if len(subpath) != 0:
+                    subpaths += subpath
+            if len(subpaths) == 0:
+                return []
+            else:
+                paths = []
+                for p in subpaths:
+                    paths.append(p + [end])
+                return paths
+
+
+    def getDefPaths(self, node):
+        prevbranches = 0
+        nodeid = int(node.nodeid.split("@")[-1])
+        for n in self.branchnodes:
+            if int(n.nodeid.split("@")[-1]) < nodeid:
+                prevbranches += 1
+        for n in self.mergenodes:
+            if int(n.nodeid.split("@")[-1]) < nodeid:
+                prevbranches += 1
+        if prevbranches >= 15:
+            logger.warning("Too many branches before this variable, skipping to avoid path explosion...")
+            return []
+        paths = self.getDefPath(node, 0, [])
+        return paths
+
+
+    def getUsage(self, name):
+        if name not in self.symbolnodes:
+            return None, None
+        else:
+            ops = []
+            symbols = []
+            nodes = self.symbolnodes[name]
+            for n in nodes:
+                for on in n.outs:
+                    if isinstance(on, TypeGenNode) and on.op not in ops:
+                        if on.op == "call" and on.func != None:
+                            ops.append(on.op + "_" + on.func)
+                        else:
+                            ops.append(on.op)
+                            
+                    elif isinstance(on, SymbolNode) and on.symbol not in symbols:
+                        symbols.append(on.symbol)
+        return ops, symbols
+
+    def getNextEmptySymbolNodes(self, node):
+        queue = node.outs
+        visited = []
+        nodes = []
+        while(len(queue) != 0):
+            q = queue[0]
+            queue = queue[1:]
+            if isinstance(q, SymbolNode) and len(q.types) == 0:
+                nodes.append(q)
+            elif q not in visited:
+                queue += q.outs
+            visited.append(q)
+        
+        return nodes
 
+
+    def clearFlowTypes(self):
+        for n in self.nodes:
+            if n.tag == 3:
+                n.cleartypes()
+    
+    def clearAllTypes(self):
+        for n in self.nodes:
+            if not isinstance(n, TypeNode):
+                n.cleartypes()
         
 
 
 
+    def getTypeConlfictNum(self):
+        changed = True
+        iters = 0
+
+        inconsistences = []
+
+        while(changed and iters < config["max_tdg_iteration"]):
+
+            changed = False
+
+            queue = self.getNoInputNodes()
+
+            iters += 1
+            self.clearVisitLabel()
+            inneriter = 0
+            while(len(queue) != 0 and inneriter < 1000):
+                inneriter += 1
+                curnode = queue[0]
+                queue.pop(0)
+                curnode.visitlabel = 2
+
+                for n in curnode.ins:
+                    if n.visitlabel < 2:
+                        curnode.visitlabel = 1
+                        if curnode not in queue:
+                            queue.append(curnode)
+
+                if curnode.visitlabel == 2:
+                    if isinstance(curnode, SymbolNode):
+                        if len(curnode.ins) > 1:
+                            logger.error("[Static Inference] Symbol node should not have more than 1 input nodes.")
+                            raise ValueError("Symbol node should not have more than 1 input nodes.")
+                        else:
+                            for n in curnode.ins:
+                                if curnode.tag != 1 and curnode.tag != 4:
+                                    curnode.tag = 3
+                                    if not isinstance(n, BranchNode) and not TypeObject.isIdenticalSet(n.types, curnode.types):
+                                        changed = True
+                                        curnode.types = copy(n.types)
+                                    elif isinstance(n, BranchNode) and not TypeObject.isIdenticalSet(n.types[n.outs.index(curnode)], curnode.types):
+                                        changed = True
+                                        curnode.types = copy(n.types[n.outs.index(curnode)])
+                                elif not isinstance(n, BranchNode) and  not TypeObject.isSetIncluded(curnode.types, n.types) and len(n.types) != 0:
+                                    if [curnode, n] not in inconsistences:
+                                        inconsistences.append([curnode, n])
+                                    logger.info(f"inconsistence of {curnode.name}, {n.lineno}; previous node {n.name}, {n.lineno}: current - {TypeObject.resolveTypeNames(curnode.types)} previous node - {TypeObject.resolveTypeNames(n.types)}")
+                                    #logger.warning("[Static Inference] The types of " + curnode.name + " is statically added as: {" + TypeObject.resolveTypeNames(curnode.types) + "}" + "However, the types of input node are: {" +TypeObject.resolveTypeNames(n.types) + "}")
+                                elif isinstance(n, BranchNode) and not TypeObject.isSetIncluded(curnode.types, n.types[n.outs.index(curnode)]) and len(n.types[n.outs.index(curnode)]) != 0:
+                                    if [curnode, n] not in inconsistences:
+                                        inconsistences.append([curnode, n])
+                                    logger.info(f"inconsistence of {curnode.name}, {n.lineno}; previous node {n.name}, {n.lineno}: current - {TypeObject.resolveTypeNames(curnode.types)} previous node - {TypeObject.resolveTypeNames(n.types)}")
+                                    #logger.warning("[Static Inference] The types of " + curnode.name + " is statically added as: {" + TypeObject.resolveTypeNames(curnode.types) + "}" + "However, the types of input node are: {" +TypeObject.resolveTypeNames(n.types[n.outs.index(curnode)]) + "}")
+                    elif isinstance(curnode, TypeGenNode):
+                        curnode.tag = 3
+                        prev_types = deepcopy(curnode.types)
+                        if curnode.op == "call" and not curnode.performTypingRules(usertype = self.usertypes):
+                            logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                        elif curnode.op not in ["List_Read", "List_Write", "Set_Read", "Dict_Read", "Tuple_Read", "Tuple_Write", "JoinedStr"] and not curnode.performTypingRules(usertype = self.usertypes):
+                            logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                            #TODO:changed = True
+                        elif curnode.op in ["List_Read", "List_Write", "Set_Read", "Dict_Read", "Tuple_Read", "Tuple_Write", "JoinedStr"] and not curnode.performTypingRules(usertype = self.usertypes, iterable = True):
+                            logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                            #TODO:changed = True
+                        curnode.types = curnode.types
+                        if not TypeObject.isIdenticalSet(prev_types, curnode.types):
+                            #logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            #logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                            changed = True
+                    elif isinstance(curnode, TypeNode):
+                        pass
+                    elif isinstance(curnode, MergeNode):
+                        curnode.tag = 3
+                        prev_types = deepcopy(curnode.types)
+                        curnode.types = []
+                        for n in curnode.ins:
+                            if not isinstance(n, BranchNode):
+                                for t in n.types:
+                                    if not TypeObject.existSame(t, curnode.types):
+                                        curnode.types.append(t)
+                            else:
+                                for t in n.types[n.outs.index(curnode)]:
+                                    if not TypeObject.existSame(t, curnode.types):
+                                        curnode.types.append(t)
+                        curnode.types = curnode.types
+                        if not TypeObject.isIdenticalSet(prev_types, curnode.types):
+                            logger.debug("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "changed.")
+                            changed = True
+                    elif isinstance(curnode, BranchNode):
+                        curnode.tag = 3
+                        prev_types = deepcopy(curnode.types)
+                        curnode.splitTypes()
+                        if not TypeObject.isIdenticalSet(prev_types[0], curnode.types[0]) or not TypeObject.isIdenticalSet(prev_types[1], curnode.types[1]):
+                            logger.debug("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "changed.")
+                            changed = True
+
+                for n in curnode.outs:
+                    if n == "PlaceHolder":
+                        continue
+                    elif n.visitlabel == 0:
+                        n.visitlabel = 1
+                        queue.append(n)
+                        if isinstance(n, TypeGenNode) and n.name == "call":
+                            logger.debug("[Static Inference] Add node: " + n.name + n.func + " at Line: " + str(n.lineno))
+                        else:
+                            logger.debug("[Static Inference] Add node: " + n.name + " at Line: " + str(n.lineno))
+                    #this indicate a loop occurs
+                    elif n.visitlabel == 1:
+                        pass
+                    elif n.visitlabel == 2:
+                        if isinstance(n, TypeGenNode) and n.name == "call":
+                            logger.debug("[Static Inference] Node: " + n.name + n.func +  " at Line: " + str(n.lineno) +" has been finalized.")
+                        else:
+                            logger.debug("[Static Inference] Node: " + n.name +  " at Line: " + str(n.lineno) +" has been finalized.")
+
+        queue = self.getNodewithRejTypes()
+        return len(queue), len(inconsistences)
+
+
 
 
     def passTypes(self, debug = False):
 
-        #print message
         logger.info("[Static Inference] Start iterating TDG " + self.name)
 
 
         changed = True
         iters = 0
         while(changed and iters < config["max_tdg_iteration"]):
 
@@ -1036,15 +1264,15 @@
             if self.isSetDominate(nodes, n, 0):
                 removed.append(n)
         for n in removed:
             if n in queue:
                 queue.remove(n)
         
         for n in self.argnodes:
-            if len(n.types) == 1 and n.types[0].type == "None" and n not in queue:
+            if len(n.types) == 1 and n.types[0].type.lower() == "none" and n not in queue:
                 queue.append(n)
         
         removed = []
         for n in queue:
             if n.ctx == "Return" and len(n.ins) == 0:
                 removed.append(n)
 
@@ -1072,14 +1300,15 @@
             else:
                 n.types = TypeObject.removeInclusiveTypes(n.types)
 
 
 
     #This function defines how to map the explicitly wrong recommended types to a valid type
     def replaceType(self, usertypes, tt, nodename, simmodel = None):
+        return 0
         if tt.category != 0 and tt.type not in usertypes and len(tt.type) != 0:
             largest_score = 0
             largest_type = None
             typestr = tt.type
             for ut in usertypes:
                 if simmodel:
                     if typestr != "" and ut[0].split(".")[-1] != "":
@@ -1121,17 +1350,17 @@
                     tt.category = 2
                 elif ntype != None and largest_score <= nscore:
                     logger.info("[Type Correction]Recommended type {} has been corrected to {} for variable {}".format(typestr, ntype, nodename))
                     tt.type = ntype
                     tt.category = 2
             
 
-    def recommendType(self, typeslots, recommendations, usertypes, modules, topn, simmodel = None):
+    def recommendType(self, typeslots, recommendations, usertypes, modules, topn, simmodel = None, eval = False):
         classname = self.name.split("@")[-1]
-        funcname = "{}.{}".format(classname, self.name.split("@")[0])
+        funcname = "{}.{}".format(classname, self.name.split("@")[0]) if classname != "global" else self.name.split("@")[0]
         if "," in classname:
             classname = classname.split(",")[-1]
         if classname not in recommendations or funcname not in recommendations[classname]:
             logger.error("[Type Recommendation]Cannot find the entry in recommendations for current TDG {}".format(self.name))
             return None
         rec = recommendations[classname][funcname]
         for t in typeslots:
@@ -1151,33 +1380,84 @@
             if len(rectypes) == 0:
                 logger.warning("[Type Recommendation]Cannot get the recommended types for varibale {} or the recommended type set is empty.".format(name))
                 continue
             verifiedtypes = []
             for tt in rectypes:
                 if tt.category == 0:
                     for ett in tt.elementtype:
-                        if ett.category != 0 and ett.type.split(".")[0] not in modules:
+                        if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
                             self.replaceType(usertypes, ett, name, simmodel = simmodel)
                     for ett in tt.keytype:
-                        if ett.category != 0 and ett.type.split(".")[0] not in modules:
+                        if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
                             self.replaceType(usertypes, ett, name, simmodel = simmodel)
                     for ett in tt.valuetype:
-                        if ett.category != 0 and ett.type.split(".")[0] not in modules:
+                        if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
                             self.replaceType(usertypes, ett, name, simmodel = simmodel)
                     verifiedtypes.append(tt)
                 elif tt.category != 0 and tt.type.split(".")[0] not in modules:
                     self.replaceType(usertypes, tt, name, simmodel = simmodel)
-            logger.info("[Type Recommendation]Found recommendation for variable {}, recommended types: {}".format(name, TypeObject.DumpOriObjects(rectypes)))
-            for tt in rectypes:
+                    verifiedtypes.append(tt)
+                elif tt.category != 0 and (tt.type.split(".")[0] in modules or "." not in tt.type):
+                    verifiedtypes.append(tt)
+            logger.info("[Type Recommendation]Found recommendation for variable {}, recommended types: {}".format(name, TypeObject.DumpOriObjects(verifiedtypes)))
+            for tt in verifiedtypes:
                 tt.added = True
                 tt.startnodename = t.symbol
                 tt.startnodeorder = t.order
             verifiedtypes = TypeObject.removeRedundantTypes(verifiedtypes)
             t.types += verifiedtypes
             t.tag = 4
+        
+        if eval == True:
+            for a in rec["annotations"]:
+                nodes = []
+                if a["category"] == "return":
+                    for n in self.returnvaluenodes:
+                        if len(n.types) == 0 and len(n.ins) != 0:
+                            nodes.append(n)
+                elif a["category"] == "local":
+                    if a["name"] in self.symbolnodes:
+                        for n in self.symbolnodes[a["name"]]:
+                            if len(n.types) == 0:
+                                nodes.append(n)
+                if len(nodes) == 0:
+                    continue
+                rectypes = []
+                for i in range(0, topn):
+                    if i < len(a["type"]):
+                        rectypes += TypeObject.Str2Obj(a["type"][i])
+                if len(rectypes) == 0:
+                    continue
+                verifiedtypes = []
+                name = a["name"]
+                for tt in rectypes:
+                    if tt.category == 0:
+                        for ett in tt.elementtype:
+                            if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
+                                self.replaceType(usertypes, ett, name, simmodel = simmodel)
+                        for ett in tt.keytype:
+                            if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
+                                self.replaceType(usertypes, ett, name, simmodel = simmodel)
+                        for ett in tt.valuetype:
+                            if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
+                                self.replaceType(usertypes, ett, name, simmodel = simmodel)
+                        verifiedtypes.append(tt)
+                    elif tt.category != 0 and tt.type.split(".")[0] not in modules:
+                        self.replaceType(usertypes, tt, name, simmodel = simmodel)
+                        verifiedtypes.append(tt)
+                    elif tt.category != 0 and (tt.type.split(".")[0] in modules or "." not in tt.type):
+                        verifiedtypes.append(tt)
+                logger.info("[Type Recommendation]Found recommendation for variable {}, recommended types: {}".format(a["name"], TypeObject.DumpOriObjects(verifiedtypes)))
+                for tt in verifiedtypes:
+                    tt.added = True
+                verifiedtypes = TypeObject.removeRedundantTypes(verifiedtypes)
+                for n in nodes:
+                    n.types += verifiedtypes
+                    n.tag = 4
+                
 
     def storeAttributeTypes(self):
         if self.name == "__init__":
             for n in self.nodes:
                 if isinstance(n, SymbolNode) and n.scope == "attribute":
                     if n.classname not in self.globaltg.classtypes:
                         self.globaltg.classtypes[n.classname] = {}
@@ -1360,14 +1640,21 @@
                         typename = TypeObject.resolveTypeName(t)
                         if typename not in res["type"]:
                             res["type"].append(typename)
         for t in typemap:
             types.append(typemap[t])
         if explicitreturn == False:
             types.append({"category": "return", "name": self.name.split("@")[0], "type": ["None"]})
+        removed = []
+        for t in types:
+            if t["category"] == "local" and len(t["type"]) == 0:
+                removed.append(t)
+        for t in removed:
+            if t in types:
+                types.remove(t)
         return types
 
 
 
 
     def _dump(self, item):
         if isinstance(item, list):
@@ -1626,28 +1913,242 @@
 
     def getNoInputNodes(self):
         noinputnodes = []
         for n in self.globalnodes:
             if len(n.ins) == 0 and n not in noinputnodes:
                 noinputnodes.append(n)
         return noinputnodes
+    
+    def getEmptySymbols(self):
+        emptysymbols = []
+        for key in self.globalsymbols:
+            for n in self.globalsymbols[key]:
+                if len(n.types) == 0:
+                    emptysymbols.append(n)
+        return emptysymbols
 
     def clearVisitLabel(self):
         for n in self.globalnodes:
             n.visitlabel = 0
 
     def getNodewithRejTypes(self):
         nodes = []
         for n in self.globalnodes:
             if not isinstance(n, BranchNode) and len(n.rejtypes) != 0:
                 nodes.append(n)
             elif isinstance(n, BranchNode) and (len(n.rejtypes[0]) != 0 or len(n.rejtypes[1]) != 0):
                 nodes.append(n)
         return nodes
 
+    def getDefPath(self, end, iteration, prev_nodes):
+        if len(end.ins) == 0:
+            return [[end]]
+        elif iteration > config["max_tdg_iteration"]:
+            return []
+        else:
+            subpaths = []
+            for o in end.ins:
+                if o in prev_nodes:
+                    continue
+                subpath = self.getDefPath(o, iteration + 1, prev_nodes + [end])
+                if len(subpath) != 0:
+                    subpaths += subpath
+            if len(subpaths) == 0:
+                return []
+            else:
+                paths = []
+                for p in subpaths:
+                    paths.append(p + [end])
+                return paths
+
+
+    def getDefPaths(self, node):
+        paths = self.getDefPath(node, 0, [])
+        return paths
+
+
+    def getAliasUsage(self, name, scope):
+        node = self.aliasgraph.searchNode(name, scope)
+        if node != None:
+            attrs = []
+            for n in node.outs:
+                attrs.append(n.name)
+            for n in node.alias:
+                attrs.append(n.name)
+            return attrs
+        return None
+
+    def getUsage(self, name):
+        if name not in self.globalsymbols:
+            return None, None
+        else:
+            ops = []
+            symbols = []
+            nodes = self.globalsymbols[name]
+            for n in nodes:
+                for on in n.outs:
+                    if isinstance(on, TypeGenNode) and on.op not in ops:
+                        if on.op == "call" and on.func != None:
+                            ops.append(on.op + "_" + on.func)
+                        else:
+                            ops.append(on.op)
+                    elif isinstance(on, SymbolNode) and on.symbol not in symbols:
+                        symbols.append(on.symbol)
+        return ops, symbols
+
+    def getNextEmptySymbolNodes(self, node):
+        queue = node.outs
+        visited = []
+        nodes = []
+        while(len(queue) != 0):
+            q = queue[0]
+            queue = queue[1:]
+            if isinstance(q, SymbolNode) and len(q.types) == 0:
+                nodes.append(q)
+            elif q not in visited:
+                queue += q.outs
+            visited.append(q)
+        
+        return nodes
+
+    def clearFlowTypes(self):
+        for n in self.globalnodes:
+            if n.tag == 3:
+                n.cleartypes()
+
+    def clearAllTypes(self):
+        for n in self.globalnodes:
+            if not isinstance(n, TypeNode):
+                n.cleartypes()
+
+
+    
+    def getTypeConlfictNum(self):
+        changed = True
+        iters = 0
+
+        inconsistences = []
+
+        while(changed and iters < config["max_tdg_iteration"]):
+
+            changed = False
+
+            queue = self.getNoInputNodes()
+
+            iters += 1
+            self.clearVisitLabel()
+            inneriter = 0
+            while(len(queue) != 0 and inneriter < 1000):
+                inneriter += 1
+                curnode = queue[0]
+                queue.pop(0)
+                curnode.visitlabel = 2
+
+                for n in curnode.ins:
+                    if n.visitlabel < 2:
+                        curnode.visitlabel = 1
+                        if curnode not in queue:
+                            queue.append(curnode)
+
+                if curnode.visitlabel == 2:
+                    if isinstance(curnode, SymbolNode):
+                        if len(curnode.ins) > 1:
+                            logger.error("[Static Inference] Symbol node should not have more than 1 input nodes.")
+                            raise ValueError("Symbol node should not have more than 1 input nodes.")
+                        else:
+                            for n in curnode.ins:
+                                if curnode.tag != 1 and curnode.tag != 4:
+                                    curnode.tag = 3
+                                    if not isinstance(n, BranchNode) and not TypeObject.isIdenticalSet(n.types, curnode.types):
+                                        changed = True
+                                        curnode.types = copy(n.types)
+                                    elif isinstance(n, BranchNode) and not TypeObject.isIdenticalSet(n.types[n.outs.index(curnode)], curnode.types):
+                                        changed = True
+                                        curnode.types = copy(n.types[n.outs.index(curnode)])
+                                elif not isinstance(n, BranchNode) and  not TypeObject.isSetIncluded(curnode.types, n.types) and len(n.types) != 0:
+                                    if [curnode, n] not in inconsistences:
+                                        inconsistences.append([curnode, n])
+                                    logger.info(f"inconsistence of {curnode.name}, {n.lineno}; previous node {n.name}, {n.lineno}: current - {TypeObject.resolveTypeNames(curnode.types)} previous node - {TypeObject.resolveTypeNames(n.types)}")
+                                    #logger.warning("[Static Inference] The types of " + curnode.name + " is statically added as: {" + TypeObject.resolveTypeNames(curnode.types) + "}" + "However, the types of input node are: {" +TypeObject.resolveTypeNames(n.types) + "}")
+                                elif isinstance(n, BranchNode) and not TypeObject.isSetIncluded(curnode.types, n.types[n.outs.index(curnode)]) and len(n.types[n.outs.index(curnode)]) != 0:
+                                    if [curnode, n] not in inconsistences:
+                                        inconsistences.append([curnode, n])
+                                    logger.info(f"inconsistence of {curnode.name}, {n.lineno}; previous node {n.name}, {n.lineno}: current - {TypeObject.resolveTypeNames(curnode.types)} previous node - {TypeObject.resolveTypeNames(n.types)}")
+                                    #logger.warning("[Static Inference] The types of " + curnode.name + " is statically added as: {" + TypeObject.resolveTypeNames(curnode.types) + "}" + "However, the types of input node are: {" +TypeObject.resolveTypeNames(n.types[n.outs.index(curnode)]) + "}")
+                    elif isinstance(curnode, TypeGenNode):
+                        curnode.tag = 3
+                        prev_types = deepcopy(curnode.types)
+                        if curnode.op == "call" and not curnode.performTypingRules(usertype = self.usertypes):
+                            logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                        elif curnode.op not in ["List_Read", "List_Write", "Set_Read", "Dict_Read", "Tuple_Read", "Tuple_Write", "JoinedStr"] and not curnode.performTypingRules(usertype = self.usertypes):
+                            logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                            #TODO:changed = True
+                        elif curnode.op in ["List_Read", "List_Write", "Set_Read", "Dict_Read", "Tuple_Read", "Tuple_Write", "JoinedStr"] and not curnode.performTypingRules(usertype = self.usertypes, iterable = True):
+                            logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                            #TODO:changed = True
+                        curnode.types = curnode.types
+                        if not TypeObject.isIdenticalSet(prev_types, curnode.types):
+                            #logger.info("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "reject some types.")
+                            #logger.info("Current {} nodes have rejected types.".format(len(self.getNodewithRejTypes())))
+                            changed = True
+                    elif isinstance(curnode, TypeNode):
+                        pass
+                    elif isinstance(curnode, MergeNode):
+                        curnode.tag = 3
+                        prev_types = deepcopy(curnode.types)
+                        curnode.types = []
+                        for n in curnode.ins:
+                            if not isinstance(n, BranchNode):
+                                for t in n.types:
+                                    if not TypeObject.existSame(t, curnode.types):
+                                        curnode.types.append(t)
+                            else:
+                                for t in n.types[n.outs.index(curnode)]:
+                                    if not TypeObject.existSame(t, curnode.types):
+                                        curnode.types.append(t)
+                        curnode.types = curnode.types
+                        if not TypeObject.isIdenticalSet(prev_types, curnode.types):
+                            logger.debug("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "changed.")
+                            changed = True
+                    elif isinstance(curnode, BranchNode):
+                        curnode.tag = 3
+                        prev_types = deepcopy(curnode.types)
+                        curnode.splitTypes()
+                        if not TypeObject.isIdenticalSet(prev_types[0], curnode.types[0]) or not TypeObject.isIdenticalSet(prev_types[1], curnode.types[1]):
+                            logger.debug("[Static Inference] Node: " + curnode.name + " at Line: " + str(curnode.lineno) + "changed.")
+                            changed = True
+
+                for n in curnode.outs:
+                    if n == "PlaceHolder":
+                        continue
+                    elif n.visitlabel == 0:
+                        n.visitlabel = 1
+                        queue.append(n)
+                        if isinstance(n, TypeGenNode) and n.name == "call":
+                            logger.debug("[Static Inference] Add node: " + n.name + n.func + " at Line: " + str(n.lineno))
+                        else:
+                            logger.debug("[Static Inference] Add node: " + n.name + " at Line: " + str(n.lineno))
+                    #this indicate a loop occurs
+                    elif n.visitlabel == 1:
+                        pass
+                    elif n.visitlabel == 2:
+                        if isinstance(n, TypeGenNode) and n.name == "call":
+                            logger.debug("[Static Inference] Node: " + n.name + n.func +  " at Line: " + str(n.lineno) +" has been finalized.")
+                        else:
+                            logger.debug("[Static Inference] Node: " + n.name +  " at Line: " + str(n.lineno) +" has been finalized.")
+
+        queue = self.getNodewithRejTypes()
+        return len(queue), len(inconsistences)
+
+
+
+
     def passTypes(self, debug = False):
 
         #print message
         logger.info("[Static Inference] Start iterating Global TDG " + self.name)
 
 
         changed = True
@@ -1844,14 +2345,125 @@
                 queue = self.getNodewithRejTypes()
                 
                         
 
         #print message
         logger.info("[Static Inferece] Finished iterating TDG.")
 
+    def replaceType(self, usertypes, tt, nodename, simmodel = None):
+        return 0
+        if tt.category != 0 and tt.type not in usertypes and len(tt.type) != 0:
+            largest_score = 0
+            largest_type = None
+            typestr = tt.type
+            for ut in usertypes:
+                if simmodel:
+                    if typestr != "" and ut[0].split(".")[-1] != "":
+                        score = simmodel.get_similarity(typestr, ut[0].split(".")[-1])
+                    else:
+                        score = 0
+                else:
+                    score = Levenshtein.ratio(typestr, ut[0].split(".")[-1])
+                if score > largest_score:
+                    largest_score = score
+                    largest_type = ut[0]
+            nscore = 0
+            ntype = None
+            for ut in usertypes:
+                
+                if simmodel:
+                    if nodename != "" and ut[0].split(".")[-1] != "":
+                        score = simmodel.get_similarity(nodename, ut[0].split(".")[-1])
+                    else:
+                        score = 0
+                else:
+                    score = Levenshtein.ratio(nodename, ut[0].split(".")[-1])
+                if score > nscore:
+                    nscore = score
+                    ntype = ut[0]
+            if not simmodel:
+                if largest_type != None and largest_score + 0.1 >= nscore:
+                    logger.info("[Type Correction]Recommended type {} has been corrected to {} for variable {}".format(typestr, largest_type, nodename))
+                    tt.type = largest_type
+                    tt.category = 2
+                elif ntype != None and largest_score + 0.1 < nscore:
+                    logger.info("[Type Correction]Recommended type {} has been corrected to {} for variable {}".format(typestr, ntype, nodename))
+                    tt.type = ntype
+                    tt.category = 2
+            else:
+                if largest_type != None and largest_score > nscore:
+                    logger.info("[Type Correction]Recommended type {} has been corrected to {} for variable {}".format(typestr, largest_type, nodename))
+                    tt.type = largest_type
+                    tt.category = 2
+                elif ntype != None and largest_score <= nscore:
+                    logger.info("[Type Correction]Recommended type {} has been corrected to {} for variable {}".format(typestr, ntype, nodename))
+                    tt.type = ntype
+                    tt.category = 2
+
+
+    def recommendType(self, recommendations, usertypes, modules, topn, simmodel = None):
+        classname = "global"
+        funcname = "global"
+        if classname not in recommendations or funcname not in recommendations[classname]:
+            logger.error("[Type Recommendation]Cannot find the entry in recommendations for current TDG {}".format(self.name))
+            return None
+        rec = recommendations[classname][funcname]      
+        for a in rec["annotations"]:
+            nodes = []
+            if a["category"] == "local":
+                if a["name"] in self.globalsymbols:
+                    for n in self.globalsymbols[a["name"]]:
+                        if len(n.types) == 0:
+                            nodes.append(n)
+            if len(nodes) == 0:
+                continue
+            rectypes = []
+            for i in range(0, topn):
+                if i < len(a["type"]):
+                    rectypes += TypeObject.Str2Obj(a["type"][i])
+            if len(rectypes) == 0:
+                continue
+            verifiedtypes = []
+            name = a["name"]
+            for tt in rectypes:
+                if tt.category == 0:
+                    for ett in tt.elementtype:
+                        if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
+                            self.replaceType(usertypes, ett, name, simmodel = simmodel)
+                    for ett in tt.keytype:
+                        if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
+                            self.replaceType(usertypes, ett, name, simmodel = simmodel)
+                    for ett in tt.valuetype:
+                        if ett.category != 0 and "." in ett.type and ett.type.split(".")[0] not in modules:
+                            self.replaceType(usertypes, ett, name, simmodel = simmodel)
+                    verifiedtypes.append(tt)
+                elif tt.category != 0 and tt.type.split(".")[0] not in modules:
+                    self.replaceType(usertypes, tt, name, simmodel = simmodel)
+                    verifiedtypes.append(tt)
+                elif tt.category != 0 and (tt.type.split(".")[0] in modules or "." not in tt.type):
+                    verifiedtypes.append(tt)
+            logger.info("[Type Recommendation]Found recommendation for variable {}, recommended types: {}".format(a["name"], TypeObject.DumpOriObjects(verifiedtypes)))
+            for tt in verifiedtypes:
+                tt.added = True
+            verifiedtypes = TypeObject.removeRedundantTypes(verifiedtypes)
+            for n in nodes:
+                n.types += verifiedtypes
+                n.tag = 4
+
+
+    def simplifyTypes(self):
+        for n in self.globalnodes:
+            if isinstance(n, BranchNode):
+                types = []
+                types.append(TypeObject.removeInclusiveTypes(n.types[0]))
+                types.append(TypeObject.removeInclusiveTypes(n.types[1]))
+                n.types = types
+            else:
+                n.types = TypeObject.removeInclusiveTypes(n.types)
+
 
     def returntypes(self):
         types = []
         typemap = {}
         for s in self.globalsymbols:
             for n in self.globalsymbols[s]:
                 if "local@" + n.symbol.split("@")[0] not in typemap:
@@ -1880,21 +2492,28 @@
                     res = typemap["local@" + n.symbol.split("@")[0]]
                 for t in n.types:
                     typename = TypeObject.resolveTypeName(t)
                     if typename not in res["type"]:
                         res["type"].append(typename)
         for t in typemap:
             types.append(typemap[t])
+        removed = []
+        for t in types:
+            if t["category"] == "local" and len(t["type"]) == 0:
+                removed.append(t)
+        for t in removed:
+            if t in types:
+                types.remove(t)
         return types
 
     def draw(self, filerepo = None):
         if filerepo != None:
-            filename = filerepo + "/" + self.name.replace("/", "_")
+            filename = filerepo + "/" + self.name.replace("/", "_").replace(".py", "_GlobalTDG")
         else:
-            filename = self.name.replace("/", "_")
+            filename = self.name.replace("/", "_").replace(".py", "_GlobalTDG")
         f = Digraph("Type Graph", filename = filename)
 
         #draw symbol node
         f.attr("node", shape = "box")
         for key in self.globalsymbols:
             for n in self.globalsymbols[key]:
                 f.node(self.resolveName(n))
```

### Comparing `hityper-1.0.2/hityper/tdg_generator.py` & `hityper-1.0.3/hityper/tdg_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 AST2Op[ast.Eq] = "=="
 AST2Op[ast.NotEq] = "!="
 AST2Op[ast.Lt] = "<"
 AST2Op[ast.LtE] = "<="
 AST2Op[ast.Gt] = ">"
 AST2Op[ast.GtE] = ">="
 AST2Op[ast.Is] = "is"
-AST2Op[ast.IsNot] = "isnot"
+AST2Op[ast.IsNot] = "is not"
 AST2Op[ast.In] = "in"
 AST2Op[ast.NotIn] = "not in"
 
 
 
 
 
@@ -64,15 +64,15 @@
     elif isinstance(node.value, int):
         return TypeObject("int", 0)
     elif node.value == None:
         return TypeObject("None", 0)
     elif type(node.value) == type(Ellipsis):
         return None
     else:
-        raise TypeError("Currently we do not suupport constant of type: " + str(type(node.value)))
+        raise TypeError("Currently HiTyper does not support constant of type: " + str(type(node.value)))
 
 def Attribute2Str(node):
     if isinstance(node, ast.Attribute):
         return Attribute2Str(node.value) + "_@_" + node.attr
     elif isinstance(node, ast.Name):
         return node.id
     elif isinstance(node, ast.Constant):
@@ -245,15 +245,18 @@
         self.lastattribute = []
         
         #other info
         self.modules = []
         self.classnames = []
 
         if isinstance(locations, list):
-            self.locations = locations
+            if len(locations) == 1 and locations[0] == None:
+                self.locations = None
+            else:
+                self.locations = locations
         elif locations == None:
             self.locations = locations
         else:
             logger.error("Invalid locations for generating TDGs.")
             raise ValueError("Invalid locations for generating TDGs.")
         self.visitedfuncs = []
         self.withitemnames = []
@@ -352,15 +355,15 @@
             self.curop += 1
             self.visit(node.left)
             if type(node.comparators[0]) == ast.Constant:
                 typeobject = transformConstant(node.comparators[0])
             else:
                 typestr = Attribute2Str(node.comparators[0])
                 if typestr in stdtypes["overall"]:
-                    typeobject = TypeObject(inputtypemap[typestr], 0)
+                    typeobject = TypeObject(inputtypemap[typestr.lower()], 0)
                 else:
                     typeobject = TypeObject(typestr, 2)
             if type(node.ops[0]) == ast.IsNot:
                 inverse = inverse * -1
             if inverse == 1:
                 branchnode.addTypes([typeobject, None])
             else:
@@ -374,15 +377,15 @@
             and len(node.args) == 2 and type(node.args[1]) in [ast.Name, ast.Attribute]):
             branchnode = BranchNode([], [], None)
             self.opstack.append(branchnode)
             self.curop += 1
             self.visit(node.args[0])
             typestr = Attribute2Str(node.args[1])
             if typestr in stdtypes["overall"]:
-                typeobject = TypeObject(inputtypemap[typestr], 0)
+                typeobject = TypeObject(inputtypemap[typestr.lower()], 0)
             else:
                 typeobject = TypeObject(typestr, 2)
             if inverse == 1:
                 branchnode.addTypes([typeobject, None])
             else:
                 branchnode.addTypes([None, typeobject])
             self.opstack.pop(self.curop)
@@ -1941,15 +1944,15 @@
     def visit_AsyncFor(self, node):
         self.visit_For(node)
 
         
 
     def visit_For(self, node):
         if len(node.orelse) != 0:
-            raise ValueError("Currently we do not support for loops with else statements.")
+            raise ValueError("Currently HiTyper does not support for loops with else statements.")
 
         typegen = TypeGenNode("forin", [], [])
         typegen.setNodePos(node.lineno, node.col_offset, node.end_col_offset)
 
         
 
         self.opstack.append(typegen)
@@ -2026,15 +2029,15 @@
 
         self.addNode(typegen)
         
 
 
     def visit_While(self, node):
         if len(node.orelse) != 0:
-            raise ValueError("Currently we do not support for loops with else statements.")
+            raise ValueError("Currently HiTyper does not support for loops with else statements.")
 
         self.asifcond = True
         self.visit(node.test)
         self.asifcond = False
 
         attribute2id_ori = deepcopy(self.attribute2id)
         globalvar2id_ori = deepcopy(self.globalvar2id)
```

### Comparing `hityper-1.0.2/hityper/typeobject.py` & `hityper-1.0.3/hityper/typeobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,39 +90,46 @@
                 return True
         return False
 
 
     @staticmethod
     def existSame( l, listr):
         for r in listr:
-            if TypeObject.isIdentical(l,r):
+            if isinstance(r, str):
+                if r.startswith("<") and r.endswith(">"):
+                    continue
+                if TypeObject.isSimilar(l, TypeObject(r,0)):
+                    return True
+            elif TypeObject.isIdentical(l, r):
                 return True
         return False
 
     @staticmethod
     def existSimilar(l, listr):
         for r in listr:
             if TypeObject.isSimilar(l,r):
                 return True
         return False
 
     @staticmethod
     def findSame(l, listr):
         for r in listr:
-            if TypeObject.isIdentical(l,r):
+            if isinstance(r, str) and TypeObject.isSimilar(l, TypeObject(r,0)):
+                return r
+            elif isinstance(r, TypeObject) and TypeObject.isIdentical(l,r):
                 return r
         return None
 
     @staticmethod
     def isIdentical( l, r):
 
         if l.category != 0 and r.category != 0:
             if l.type == r.type:
                 return True
-            elif l.category == r.category and l.category == 2 and (l.type.split(".")[-1] == r.type.split(".")[-1]):
+            elif l.category == r.category and l.category == 2 and (l.type.split(".")[-1].lower() == r.type.split(".")[-1].lower()):
                 return True
             else:
                 return False
         if  l.category == 0 and r.category == 0:
             if typeequalmap[l.type.lower()] == typeequalmap[r.type.lower()]:
                 if l.type.lower() not in ["list", "tuple", "set", "iterable", "optional", "union", "sequence", "generator", "dict"]:
                     return True
@@ -135,27 +142,45 @@
                 return True
             elif (l.type.lower() == "iterable" and typeequalmap[r.type.lower()] <= 17 and typeequalmap[r.type.lower()] >= 11) or (r.type.lower() == "iterable" and typeequalmap[l.type.lower()] <= 17 and typeequalmap[l.type.lower()] >= 11):
                 return True
         if l.category == 0 and r.category == 2 and l.type.lower() == "type" and len(l.elementtype) == 1:
             return TypeObject.isIdentical(l.elementtype[0], r)
         if r.category == 0 and l.category == 2 and r.type.lower() == "type" and len(r.elementtype) == 1:
             return TypeObject.isIdentical(r.elementtype[0], l)
+        if (l.category == 2 or r.category == 2) and l.type.split(".")[-1].lower() == r.type.split(".")[-1].lower():
+            return True
         return False
     
     @staticmethod
     def isSimilar(l,r):
         if l.category == 0 and r.category == 0 and typeequalmap[l.type.lower()] == typeequalmap[r.type.lower()]:
             return True
         elif l.type.lower() == r.type.lower():
             return True
         else:
             return False
     
     @staticmethod
     def isIdenticalSet( llist, rlist):
+        
+        invalidtypes = []
+        for l in llist:
+            if not isinstance(l, TypeObject):
+                invalidtypes.append(l)
+        for r in rlist:
+            if not isinstance(r, TypeObject):
+                invalidtypes.append(r)
+        
+        for t in invalidtypes:
+            if t in llist:
+                llist.remove(t)
+        for t in invalidtypes:
+            if t in rlist:
+                rlist.remove(t)
+        
         for l in llist:
             if l.type.lower() == "any":
                 return True
             if not TypeObject.existSame(l, rlist) and l.type.lower() != "any":
                 return False
         for r in rlist:
             if r.type.lower() == "any":
@@ -271,24 +296,24 @@
 
 
 
     @staticmethod
     def simplifyGenericType(t):
         if not isinstance(t, TypeObject):
             return t
-        if t.type in ["Set", "Tuple", "List", "Awaitable", "Iterable", "Union"]:
+        if t.type.lower() in ["set", "frozenset", "tuple", "list", "awaitable", "iterable", "union", "generator"]:
             t.elementtype = TypeObject.removeInclusiveTypes(t.elementtype)
-        elif t.type == "Dict":
+        elif t.type.lower() == "dict":
             t.keytype = TypeObject.removeInclusiveTypes(t.keytype)
             t.valuetype = TypeObject.removeInclusiveTypes(t.valuetype)
-        elif t.type == "Optional":
+        elif t.type.lower() == "optional":
             t.elementtype = TypeObject.removeRedundantTypes(t.elementtype)
             rm = None
             for et in t.elementtype:
-                if et.type == "None":
+                if et.type.lower() == "none":
                     rm = et
                     break
             if rm != None and rm in t.elementtype:
                 t.elementtype.remove(rm)
 
         return t
 
@@ -316,28 +341,48 @@
                         removed = True
                         target = outs[i]
                         break
             if removed and target in outs:
                 outs.remove(target)
         return outs
 
+    @staticmethod
+    def removeInvalidTypes(t):
+        if isinstance(t, TypeObject):
+            elementtype = []
+            for tt in t.elementtype:
+                if isinstance(tt, TypeObject):
+                    elementtype.append(TypeObject.removeInvalidTypes(tt))
+            t.elementtype = elementtype
+            keytype = []
+            for tt in t.keytype:
+                if isinstance(tt, TypeObject):
+                    keytype.append(TypeObject.removeInvalidTypes(tt))
+            t.keytype = keytype
+            valuetype = []
+            for tt in t.valuetype:
+                if isinstance(tt, TypeObject):
+                    valuetype.append(TypeObject.removeInvalidTypes(tt))
+            return t
 
     def __str__(self):
         return TypeObject.resolveTypeName(self)
             
 
     @staticmethod
     def resolveTypeName(t):
         if isinstance(t, TypeObject):
+            t = TypeObject.removeInvalidTypes(t)
+            t = TypeObject.simplifyGenericType(t)
             if t.category != 0:
                 return t.type
             elif t.type.lower() not in exporttypemap:
                 raise TypeError("Unknown type: " + t.type)
             typestr = exporttypemap[t.type.lower()]
-            if t.type in ["Dict", "Callable"]:
+            if t.type.lower() in ["dict", "callable"] and len(t.keytype) + len(t.valuetype) > 0:
                 typestr = typestr + "["
                 if len(t.keytype) == 0:
                     typestr += ", "
                 elif len(t.keytype) == 1:
                     typestr = typestr + TypeObject.resolveTypeName(t.keytype[0]) + ", "
                 else:
                     typestr += "typing.Union["
@@ -352,15 +397,15 @@
                 else:
                     typestr += "typing.Union["
                     for n in t.valuetype:
                         typestr = typestr + TypeObject.resolveTypeName(n) + ","
                     typestr = typestr[:-1]
                     typestr += "]"
                 typestr += "]"
-            elif t.type in ["Set", "Tuple", "List", "Awaitable", "Iterable", "Sequence", "Generator"]:
+            elif t.type.lower() in ["set", "tuple", "list", "awaitable", "iterable", "sequence", "generator"] and len(t.elementtype) > 0:
                 typestr = typestr + "["
                 if len(t.elementtype) == 1:
                     typestr = typestr + TypeObject.resolveTypeName(t.elementtype[0])
                 elif len(t.elementtype) == 2 and (t.elementtype[0].type == "None" or t.elementtype[1].type == "None"):
                     typestr += "typing.Optional["
                     for i in t.elementtype:
                         if i.type != "None":
@@ -369,27 +414,27 @@
                 elif len(t.elementtype) >= 2:
                     typestr += "typing.Union["
                     for n in t.elementtype:
                         typestr = typestr + TypeObject.resolveTypeName(n) + ","
                     typestr = typestr[:-1]
                     typestr += "]"
                 typestr += "]"
-            elif t.type == "Optional":
+            elif t.type.lower() == "optional" and len(t.elementtype) > 0:
                 typestr += "["
                 if len(t.elementtype) > 1:
                     typestr += "typing.Union["
                     for n in t.elementtype:
                         typestr = typestr + TypeObject.resolveTypeName(n) + ","
                     typestr = typestr[:-1]
                     typestr += "]"
                 elif len(t.elementtype) == 1:
                     typestr = typestr + TypeObject.resolveTypeName(t.elementtype[0]) + "]"
                 else:
                     typestr += "]"
-            elif t.type == "Union":
+            elif t.type.lower() == "union" and len(t.elementtype) > 0:
                 typestr += "["
                 if len(t.elementtype) == 0:
                     typestr += "]"
                 if len(t.elementtype) == 1:
                     typestr = typestr + TypeObject.resolveTypeName(t.elementtype[0]) + "]"
                 elif len(t.elementtype) > 1:
                     for n in t.elementtype:
@@ -434,73 +479,73 @@
         elif typeobjs[0].category == 2:
             return "user-defined"
         else:
             return None
 
 
     @staticmethod
-    def Str2Obj(typestr):
+    def _Str2Obj(typestr):
         strobjs = []
         typestr = typestr.replace(" ", "")
         typestr = typestr.replace("builtins.", "")
         typestr = typestr.replace("typing_extensions.", "typing.")
         if len(typestr) > 2 and typestr[0] == "[" and typestr[-1] == "]":
             typestr = typestr[1:len(typestr) - 1]
         if typestr == None or typestr == "":
             return strobjs
         if len(typestr) > 500:
             #logger.warning("Type name is too long.")
             return strobjs
-        if typestr in ["Union", "typing.Union"] and "[" not in typestr:
+        if typestr.lower() in ["union", "typing.union"] and "[" not in typestr:
             return strobjs
         elif typestr.lower() in inputtypemap:
             strobjs.append(TypeObject(inputtypemap[typestr.lower()], 0))
             return strobjs
         elif "[" in typestr and "]" in typestr:
             typestr = typestr.replace("t.", "typing.")
             index1 = typestr.index("[")
             index2 = typestr.rfind("]")
             innerstr = typestr[index1 + 1:index2]
-            if "Union" in typestr[:index1]:
+            if "union" in typestr[:index1].lower():
                 strs = innerstr.split(",")
                 leftnum = 0
                 rightnum = 0
                 cur_str = ""
                 for s in strs:
                         cur_str += s
                         leftnum += s.count("[")
                         rightnum += s.count("]")
                         if leftnum == rightnum:
-                            strobjs += TypeObject.Str2Obj(cur_str)
+                            strobjs += TypeObject._Str2Obj(cur_str)
                             cur_str = ""
                         else:
                             cur_str += ","
                 return strobjs
-            elif "Optional" in typestr[:index1] or "typing.Optional" in typestr[:index1]:
-                strobjs += TypeObject.Str2Obj(innerstr)
+            elif "optional" in typestr[:index1].lower() or "typing.optional" in typestr[:index1].lower():
+                strobjs += TypeObject._Str2Obj(innerstr)
                 strobjs.append(TypeObject("None", 0))
                 return strobjs
             if typestr[:index1].lower() in inputtypemap:
                 typeobj = TypeObject(inputtypemap[typestr[:index1].lower()], 0)
-                if "Dict" in typestr[:index1] or "Mapping" in typestr[:index1] or "Callable" in typestr[:index1]:
+                if "dict" in typestr[:index1].lower() or "mapping" in typestr[:index1].lower() or "callable" in typestr[:index1].lower():
                     if "," in innerstr:
                         commaindex = innerstr.split(",")
                         leftnum = 0
                         rightnum = 0
                         cur_str = ""
                         count = 0
                         for s in commaindex:
                             cur_str += s
                             leftnum += s.count("[")
                             rightnum += s.count("]")
                             if leftnum == rightnum:
                                 if count == 0:
-                                    typeobj.keytype += TypeObject.Str2Obj(cur_str)
+                                    typeobj.keytype += TypeObject._Str2Obj(cur_str)
                                 else:
-                                    typeobj.valuetype += TypeObject.Str2Obj(cur_str)
+                                    typeobj.valuetype += TypeObject._Str2Obj(cur_str)
                                 count += 1
                                 cur_str = ""
                             else:
                                 cur_str += ","
                         strobjs.append(typeobj)
                         return strobjs
                     else:
@@ -511,43 +556,60 @@
                     rightnum = 0
                     cur_str = ""
                     for s in strs:
                         cur_str += s
                         leftnum += s.count("[")
                         rightnum += s.count("]")
                         if leftnum == rightnum:
-                            typeobj.elementtype += TypeObject.Str2Obj(cur_str)
+                            typeobj.elementtype += TypeObject._Str2Obj(cur_str)
                             cur_str = ""
                         else:
                             cur_str += ","
                     
                     '''
                     if "[" in innerstr and "]" in innerstr:
-                        typeobj.elementtype = TypeObject.Str2Obj(innerstr)
+                        typeobj.elementtype = TypeObject._Str2Obj(innerstr)
                     else:
                         strs = innerstr.split(",")
                         for s in strs:
-                            typeobj.elementtype += TypeObject.Str2Obj(s)
+                            typeobj.elementtype += TypeObject._Str2Obj(s)
                     '''
                     strobjs.append(typeobj)
                     return strobjs
             else:
-                typeobj = TypeObject(typestr.replace("[typing.Any]", ""), 2)
+                typeobj = TypeObject(typestr.replace("[typing.Any]", "").replace("[typing.any]", ""), 2)
                 strobjs.append(typeobj)
                 return strobjs
         elif typestr.startswith("typing") and "[" not in typestr and typestr.lower() in inputtypemap:
             typeobj = TypeObject(inputtypemap[typestr.lower()], 0)
             strobjs.append(typeobj)
             return strobjs
         else:
             typeobj = TypeObject(typestr, 2)
             strobjs.append(typeobj)
             return strobjs
 
     @staticmethod
+    def Str2Obj(typestr):
+        if typestr.count("[") != typestr.count("]"):
+            return []
+        else:
+            typeobjs = TypeObject._Str2Obj(typestr)
+            queue = typeobjs
+            while(len(queue) != 0):
+                obj = queue[0]
+                queue = queue[1:]
+                if obj.category == 2 and ("[" in obj.type or "]" in obj.type):
+                    return []
+                queue += obj.elementtype
+                queue += obj.keytype
+                queue += obj.valuetype
+            return typeobjs
+
+    @staticmethod
     def DumpObject(typeobj):
         print("Type: " + typeobj.type)
         print("Element Type:" + TypeObject.resolveTypeNames(typeobj.elementtype))
         print("Key Type:" + TypeObject.resolveTypeNames(typeobj.keytype))
         print("Value Type:" + TypeObject.resolveTypeNames(typeobj.valuetype))
 
     @staticmethod
```

### Comparing `hityper-1.0.2/hityper/typerule.py` & `hityper-1.0.3/hityper/typerule.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 raise ValueError("Operands must be a graph node")
         if (op in ["and", "or"]):
             return self.binop_and_or(left, right)
         elif (op == "not"):
             return self.unop_not(left, right)
         elif (op in ["<", "<=", ">", ">="]):
             return self.binop_compare_neq(left, right)
-        elif (op in ["==", "!=", "is", "isnot"]):
+        elif (op in ["==", "!=", "is", "is not"]):
             return self.binop_compare_eq(left, right)
         elif (op == "+" and right != None):
             return self.binop_add(operands)
         elif (op == "*"):
             return self.binop_mul(left, right)
         elif (op in ["-", "/", "//", "%", "**", "pow"] and right != None):
             return self.binop_num_op(left, right, op)
@@ -113,15 +113,15 @@
             return self.unknown_op(operands, op)
             #raise TypeError("Unknown Operation: " + op)
 
     def act(self, operands , op, func, attr, usertypes, iterable=False, curnode = None):
         #if not about iterable
         res = self.sub_act(operands , op, func, attr, usertypes, iterable=False, curnode = curnode)
         if res==None:
-            print("POSIIBLE NONE RETURN op is:", op)
+            logger.warning("POSIIBLE NONE RETURN op is:" + op if op != "call" else "POSIIBLE NONE RETURN op is:" + func)
         return res
 
     def unknown_op(self, operands, op):
         logger.warning("Unknown Operation: " + op)
         rej_types = []
         outs = []
         for i in operands:
@@ -156,18 +156,18 @@
         #out: bool(including user-defined)
         ltypes = left.types
         rtypes = right.types
         rej_ltypes = []
         rej_rtypes = []
         outs = TypeObject("bool", 0)
         for t in ltypes:
-            if (not TypeObject.existCompatible(t, rtypes)) or t.category != 0 or t.type in ["type", "Callable", "Dict", "None"]:
+            if (not TypeObject.existCompatible(t, rtypes)) or t.category != 0 or TypeObject.existSame(t, ["type", "Callable", "Dict", "None"]):
                 rej_ltypes.append(t)
         for t in rtypes:
-            if (not TypeObject.existCompatible(t, ltypes)) or t.category != 0 or t.type in ["type", "Callable", "Dict", "None"]:
+            if (not TypeObject.existCompatible(t, ltypes)) or t.category != 0 or TypeObject.existSame(t, ["type", "Callable", "Dict", "None"]):
                 rej_rtypes.append(t)
         return [rej_ltypes, rej_rtypes], outs
 
     def binop_compare_eq(self, left, right):
         #rule: left and right can have arbitary type
         #out: bool(including user-defined)
         rej_ltypes = []
@@ -185,30 +185,30 @@
         rej_ltypes = []
         rej_rtypes = []
         outs = []
         # if ltypes or rtypes are None, add rej
         # if len(ltypes)==0:
         #     rej_ltypes.append()
         for t in ltypes:
-            if t.type in ["Tuple", "List"]:
+            if TypeObject.existSame(t, ["Tuple", "List"]):
                 temp = TypeObject(t.type, 0)
                 temp.elementtype += t.elementtype
                 rexist = False
                 for rt in rtypes:
                     if rt.type == t.type:
                         temp.elementtype += rt.elementtype
                         rexist = True
                 if rexist:
                     outs.append(temp)          
-            elif ((not TypeObject.existSame(t, rtypes)) and (not TypeObject.existCompatible(t, rtypes))) or t.category != 0 or t.type in ["type", "Callable", "Set", "Dict", "None"]:
+            elif ((not TypeObject.existSame(t, rtypes)) and (not TypeObject.existCompatible(t, rtypes))) or t.category != 0 or TypeObject.existSame(t, ["type", "Callable", "Set", "Dict", "None"]):
                 rej_ltypes.append(t)
             elif (not TypeObject.existSame(t, outs)):
                 outs.append(t)
         for t in rtypes:
-            if ((not TypeObject.existSame(t, ltypes)) and (not TypeObject.existCompatible(t, ltypes))) or t.category != 0 or t.type in ["type", "Callable", "Set", "Dict", "None"]:
+            if ((not TypeObject.existSame(t, ltypes)) and (not TypeObject.existCompatible(t, ltypes))) or t.category != 0 or TypeObject.existSame(t, ["type", "Callable", "Set", "Dict", "None"]):
                 rej_rtypes.append(t)
             elif not TypeObject.existSame(t, outs):
                 outs.append(t)
         if len(operands)==2:
             return [rej_ltypes, rej_rtypes], outs
         elif len(operands)>2:
             rej = []
@@ -225,31 +225,31 @@
         rtypes = right.types
         rej_ltypes = []
         rej_rtypes = []
         outs = []
         
         if not TypeObject.existType("int", ltypes) and not TypeObject.existType("bool", ltypes):
             for t in rtypes:
-                if t.type not in ["bool", "float", "int"]:
+                if not TypeObject.existSame(t, ["bool", "float", "int"]):
                     rej_rtypes.append(t)
         if not TypeObject.existType("int", rtypes) and not TypeObject.existType("bool", rtypes):
             for t in ltypes:
-                if t.type not in ["bool", "float", "int"]:
+                if not TypeObject.existSame(t, ["bool", "float", "int"]):
                     rej_ltypes.append(t)
 
         for t in ltypes:
-            if t.type in ["type", "Callable", "None", "Set", "Dict"]:
+            if TypeObject.existSame(t, ["type", "Callable", "None", "Set", "Dict"]):
                 rej_ltypes.append(t)
 
         for t in rtypes:
-            if t.type in ["type", "Callable", "None", "Set", "Dict"]:
+            if TypeObject.existSame(t, ["type", "Callable", "None", "Set", "Dict"]):
                 rej_rtypes.append(t)
 
-        self.check_failed(ltypes, rej_ltypes)
-        self.check_failed(rtypes, rej_rtypes)
+        #self.check_failed(ltypes, rej_ltypes)
+        #self.check_failed(rtypes, rej_rtypes)
 
         if TypeObject.existType("float", ltypes) or TypeObject.existType("float", rtypes):
             outs.append(TypeObject("float", 0))
         if (TypeObject.existType("int", ltypes) or TypeObject.existType("bool", ltypes)) and (TypeObject.existType("int", rtypes) or TypeObject.existType("bool", rtypes)):
             outs.append(TypeObject("int", 0))
         if TypeObject.existType("int", ltypes) or TypeObject.existType("bool", ltypes):
             for t in rtypes:
@@ -274,41 +274,41 @@
         level = 0
         # for joinedstr
         strtemp = TypeObject("Text",0)
         if op=='%' and TypeObject.existSame(strtemp,ltypes):
             outs = [TypeObject("Text", 0)]
             # left can only be Text
             for idx in range(len(ltypes)):
-                if ltypes[idx].type!="Text":
+                if not TypeObject.existSame(ltypes[idx], ["str"]):
                     rej_ltypes.append(ltypes[idx])
             return [rej_ltypes, rej_rtypes], outs
 
         for idx in range(len(rtypes)):
             if rtypes[idx].type=="bool":
                 rtypes[idx] = TypeObject("int", 0) # raise the type
-            elif rtypes[idx].type not in ["bool", "int", "float", "complex"]:
+            elif not TypeObject.existSame(rtypes[idx], special_types["@number@"]):
                 rej_rtypes.append(rtypes[idx])
-            elif ["bool", "int", "float", "complex"].index(rtypes[idx].type) > level:
-                level = ["bool", "int", "float", "complex"].index(rtypes[idx].type)
+            elif special_types["@number@"].index(rtypes[idx].type.lower()) > level:
+                level = special_types["@number@"].index(rtypes[idx].type.lower())
 
         for idx in range(len(ltypes)):
             if ltypes[idx].type=="bool":
                 ltypes[idx] = TypeObject("int", 0) # raise the type
 
         for t in ltypes:
-            if t.type not in ["bool", "int", "float", "complex"]:
+            if not TypeObject.existSame(t, special_types["@number@"]):
                 rej_ltypes.append(t)
-            elif t.type in ["int", "float", "complex"] and TypeObject.existSame(t, rtypes) and not TypeObject.existSame(t, outs):
+            elif TypeObject.existSame(t, ["int", "float", "complex"]) and TypeObject.existSame(t, rtypes) and not TypeObject.existSame(t, outs):
                 outs.append(t)
-            elif t.type in ["int", "float", "complex"] and not TypeObject.existSame(t, rtypes) and ["bool", "int", "float", "complex"].index(t.type) > level and not TypeObject.existSame(t, outs):
+            elif TypeObject.existSame(t, ["int", "float", "complex"]) and not TypeObject.existSame(t, rtypes) and special_types["@number@"].index(t.type.lower()) > level and not TypeObject.existSame(t, outs):
                 outs.append(t)
 
         
         for t in rtypes:
-            if t.type in ["int", "float", "complex"] and ["bool", "int", "float", "complex"].index(t.type) == level and not TypeObject.existSame(t, outs):
+            if TypeObject.existSame(t, ["int", "float", "complex"]) and special_types["@number@"].index(t.type.lower()) == level and not TypeObject.existSame(t, outs):
                 outs.append(t)
 
         if op == "/" and len(ltypes) > len(rej_ltypes) and len(rtypes) > len(rej_rtypes):
             outs = [TypeObject("float", 0)]
 
         return [rej_ltypes, rej_rtypes], outs
 
@@ -317,37 +317,37 @@
         #out: the original number type
         #not surport user-define
         ltypes = left.types
         rej_ltypes = []
         rej_rtypes = []
         outs = []
         for t in ltypes:
-            if t.type not in ["bool", "int", "float", "complex"]:
+            if not TypeObject.existSame(t, special_types["@number@"]):
                 rej_ltypes.append(t)
             elif not TypeObject.existSame(t, outs):
                 outs.append(t)
         return [rej_ltypes, rej_rtypes], outs
 
     def unop_int(self, left, right):
         # NO MORE USED
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("int", 0)
         for t in ltypes:
-            if t.type not in ["int", "float", "complex", "bytes", "Text", "bool"]:
+            if not TypeObject.existSame(t, ["int", "float", "complex", "bytes", "Text", "bool"]):
                 rej_ltypes.append(t)
         return [rej_ltypes], outs
 
     def unop_float(self, left, right):
         #NO MORE USED
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("float", 0)
         for t in ltypes:
-            if t.type not in ["int", "float", "complex", "bytes", "Text", "bool"]:
+            if not TypeObject.existSame(t, ["int", "float", "complex", "bytes", "Text", "bool"]):
                 rej_ltypes.append(t)
         return [rej_ltypes], outs
 
     def binop_divmod(self, left, right):
         # NO MORE USED
         #rule: just the combination of / and % in numbers
         #out: numbers
@@ -357,18 +357,18 @@
         # if one is float =>math.floor(a / b), a % b float/float
         ltypes = left.types
         rtypes = right.types
         basic_type = TypeObject("int", 0)
         llevel = rlevel = 1
         for lt in ltypes:
             if TypeObject.isCompatible(lt, basic_type):
-                llevel = max(llevel, ["bool", "int", "float", "complex"].index(lt.type))
+                llevel = max(llevel, special_types["@number@"].index(lt.type.lower()))
         for rt in rtypes:
             if TypeObject.isCompatible(rt,basic_type):
-                rlevel = max(rlevel, ["bool", "int", "float", "complex"].index(rt.type))
+                rlevel = max(rlevel, special_types["@number@"].index(rt.type.lower()))
         if llevel<2 and rlevel<2:
             rej_ltypes, rej_rtypes, outs = self.binop_num_op(left, right,"%")
         else:
             rej_ltypes, rej_rtypes, outs = self.binop_num_op(left, right,"/")
         finalouts = TypeObject("Tuple", 0)
         finalouts.buildTuple(outs)
         return [rej_ltypes, rej_rtypes], finalouts
@@ -384,19 +384,19 @@
             rtypes = right.types
             rej_ltypes = []
             rej_rtypes = []
             outs = []
             temp1 = TypeObject("int", 0)
             temp2 = TypeObject("bool", 0)
             for t in ltypes:
-                if t.type not in ["int", "bool","Any", "Set"] and t.category==0:
+                if not TypeObject.existSame(t, ["int", "bool","Any", "Set"]) and t.category==0:
                     rej_ltypes.append(t)
 
             for t in rtypes:
-                if t.type not in ["int", "bool","Any", "Set"] and t.category==0:
+                if not TypeObject.existSame(t, ["int", "bool","Any", "Set"]) and t.category==0:
                     rej_rtypes.append(t)
 
             if TypeObject.existSame(TypeObject("Set", 0), ltypes) and TypeObject.existSame(TypeObject("Set", 0), rtypes):
                 outs.append(TypeObject.findSame(TypeObject("Set", 0), ltypes))
                 outs.append(TypeObject.findSame(TypeObject("Set", 0), rtypes))
         
             outs += [temp1,temp2]
@@ -408,63 +408,63 @@
             temp1 = TypeObject("int", 0)
             temp2 = TypeObject("bool", 0)
             rej = []
             for inode in operands:
                 itypes = inode.types
                 rej_types = []
                 for t in itypes:
-                    if t.type not in ["int", "bool", "Any"] and t.category == 0:
+                    if not TypeObject.existSame(t, ["int", "bool","Any"]) and t.category == 0:
                         rej_types.append(t)
                 rej.append(rej_types)
             return rej,[temp1,temp2]
 
 
     def unop_int_op(self, left, right):
         #rule: can accept int and bool
         #out: int
         #not support user-define
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("int", 0)
         for t in ltypes:
-            if t.type not in ["int", "bool"]:
+            if not TypeObject.existSame(t, ["int", "bool"]):
                 rej_ltypes.append(t)
         return [rej_ltypes], outs
 
     def unop_bytes(self, left, right):
         # No more use here
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("bytes", 0)
         for t in ltypes:
-            if t.type in ["List", "Tuple", "Set"]:
+            if TypeObject.existSame(t, ["List", "Tuple", "Set"]):
                 rej_elementtypes = []
                 if isinstance(t.elementtype, list):
                     for it in t.elementtype:
-                        if it.type not in ["int", "bool"]:
+                        if not TypeObject.existSame(it, ["int", "bool"]):
                             rej_elementtypes.append(it)
-                elif t.elementtype.type not in ["int", "bool"]:
+                elif not TypeObject.existSame(t.elementtype, ["int", "bool"]):
                     rej_elementtypes.append(t.elementtype)
                 rej_type = TypeObject(t.type, 0)
                 rej_type.elementtype = rej_elementtypes
                 rej_ltypes.append(rej_type)
             elif t.type == "Dict":
                 rej_keytypes = []
                 if isinstance(t.keytype, list):
                     for it in t.keytype:
-                        if it.type not in ["int", "bool"]:
+                        if not TypeObject.existSame(it, ["int", "bool"]):
                             rej_keytypes.append(it)
                 elif t.keytype not in ["int", "bool"]:
                     rej_keytypes.append(t.keytype)
                 rej_valuetypes = []
                 rej_type = TypeObject("Dict", 0)
                 rej_type.keytype = rej_keytypes
                 rej_type.valuetype = rej_valuetypes
                 rej_ltypes.append(rej_type)
-            elif t.type not in ["int", "bool"]:
+            elif not TypeObject.existSame(t, ["int", "bool"]):
                 rej_ltypes.append(t)
         return [rej_ltypes], outs
 
     def unop_str(self, left, right):
         #rule: can accept any type
         #out: string(including user-define)
         rej_ltypes = []
@@ -475,22 +475,22 @@
         #rule: can accept iterable types
         #out: tuple
         # not support user-define
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("Tuple", 0)
         for t in ltypes:
-            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+            if not TypeObject.existSame(t, special_types["@iterable@"]):
                 rej_ltypes.append(t)
-            elif t.type == "Dict":
+            elif TypeObject.existSame(t, ["Dict"]):
                 if isinstance(t.keytype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
-            elif t.type == "Text":
+            elif TypeObject.existSame(t, ["Text"]):
                 outs.elementtype.append(TypeObject("Text", 0))
             else:
 
                 if isinstance(t.elementtype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
@@ -500,22 +500,22 @@
         #rule: can accept iterable types
         #out: list
         # not support user-define
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("List", 0)
         for t in ltypes:
-            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+            if not TypeObject.existSame(t, special_types["@iterable@"]):
                 rej_ltypes.append(t)
-            elif t.type == "List":
+            elif TypeObject.existSame(t, ["List"]):
                 if isinstance(t.keytype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
-            elif t.type == "Text":
+            elif TypeObject.existSame(t, ["Text"]):
                 outs.elementtype.append(TypeObject("Text", 0))
             else:
 
                 if isinstance(t.elementtype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
@@ -525,22 +525,22 @@
         #rule: can accept iterable types
         #out: set
         # not support user-define
         ltypes = left.types
         rej_ltypes = []
         outs = TypeObject("Set", 0)
         for t in ltypes:
-            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+            if not TypeObject.existSame(t, special_types["@iterable@"]):
                 rej_ltypes.append(t)
-            elif t.type == "Set":
+            elif TypeObject.existSame(t, ["Set"]):
                 if isinstance(t.keytype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
-            elif t.type == "Text":
+            elif TypeObject.existSame(t, ["Text"]):
                 outs.elementtype.append(TypeObject("Text", 0))
             else:
 
                 if isinstance(t.elementtype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
@@ -578,34 +578,36 @@
         #out: bool
         # not support user-define
         rtypes = right.types
         rej_ltypes = []
         rej_rtypes = []
         outs = TypeObject("bool", 0)
         for t in rtypes:
-            if t.type not in ["Tuple", "Dict", "List", "Set", "Text"]:
+            if not TypeObject.existSame(t, special_types["@iterable@"]):
                 rej_rtypes.append(t)
         return [rej_ltypes, rej_rtypes], outs
 
     def unop_forin(self, left, right):
         #rule: left must be tuple, dict, list, set and string
         #out: element type of left
         ltypes = left.types
         rej_ltypes = []
         outs = []
         for t in ltypes:
-            if t.type not in ["Tuple", "Dict", "List", "Set", "Text"]:
+            if not TypeObject.existSame(t, special_types["@iterable@"]):
                 rej_ltypes.append(t)
-            elif t.type == "Text":
+            elif TypeObject.existSame(t, ["Text"]):
                 outs.append(TypeObject("Text", 0))
-            elif t.type == "Dict":
+            elif TypeObject.existSame(t, ["Dict"]):
                 if isinstance(t.keytype, list):
                     outs += t.keytype
                 else:
                     outs.append(t.keytype)
+            elif TypeObject.existSame(t, ["IO"]):
+                outs.append(TypeObject("Text", 0))
             else:
                 if isinstance(t.elementtype, list):
                     outs += t.elementtype
                 else:
                     outs.append(t.elementtype)
         return [rej_ltypes], outs    
 
@@ -614,15 +616,15 @@
         #out: list
         ltypes = left.types
         rtypes = right.types
         rej_ltypes = []
         rej_rtypes = []
         outs = TypeObject("List", 0)
         for t in ltypes:
-            if t.type != "List":
+            if not TypeObject.existSame(t, ["List"]):
                 rej_ltypes.append(t)
             else:
                 if isinstance(t.elementtype, list):
                     outs.elementtype += t.elementtype
                 else:
                     outs.elementtype.append(t.elementtype)
         
@@ -648,24 +650,24 @@
 
             rej_ttypes = []
             rej_itypes = []
 
             outs = []
             if TypeObject.existType("List", ttypes):
                 for it in itypes:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes.append(it)
 
             for t in ttypes:
-                if t.type not in ["Dict", "List"]:
+                if not TypeObject.existSame(t, ["Dict", "List"]):
                     rej_ttypes.append(t)
-                elif t.type == "List":
+                elif TypeObject.existSame(t, ["List"]):
                     otype = TypeObject("List", 0)
                     outs.append(otype)
-                elif t.type == "Dict":
+                elif TypeObject.existSame(t, ["Dict"]):
                     otype = TypeObject("Dict", 0)
                     outs.append(otype)
 
             return [rej_ttypes, rej_itypes], outs
         elif len(operands)>2:
             target = operands[0]
             index = operands[1]
@@ -676,31 +678,31 @@
             vtypes = value.types
             rej_ttypes = []
             rej_itypes = []
             rej_vtypes = []
             outs = []
             if TypeObject.existType("List", ttypes):
                 for it in itypes:
-                        if it.type not in ["int", "bool"]:
+                        if not TypeObject.existSame(it, ["int", "bool"]):
                             rej_itypes.append(it)
 
             for t in ttypes:
                 if t.type not in ["Dict", "List"] and t.category != 2:
                     rej_ttypes.append(t)
-                elif t.type == "List":
+                elif TypeObject.existSame(t, ["List"]):
                     otype = TypeObject("List", 0)
                     if isinstance(t.elementtype, list):
                         otype.elementtype += t.elementtype
                     else:
                         otype.elementtype.append(t.elementtype)
                     for vt in vtypes:
                         if not TypeObject.existSame(vt, otype.elementtype):
                             otype.elementtype.append(vt)
                     outs.append(otype)
-                elif t.type == "Dict":
+                elif TypeObject.existSame(t, ["Dict"]):
                     otype = TypeObject("Dict", 0)
                     if isinstance(t.keytype, list):
                         otype.keytype += t.keytype
                     else:
                         otype.keytype.append(t.keytype)
                     if isinstance(t.valuetype, list):
                         otype.valuetype += t.valuetype
@@ -733,19 +735,19 @@
             ttypes = target.types
 
             rej_ttypes = []
 
             outs = []
 
             for t in ttypes:
-                if t.type not in ["Dict", "List", "Tuple", "Text", "bytes"]:
+                if not TypeObject.existSame(t, special_types["@subscriptable@"]):
                     rej_ttypes.append(t)
-                elif t.type in ["Text", "bytes"]:
+                elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
                     outs.append(t)
-                elif t.type == "Dict":
+                elif TypeObject.existSame(t, ["Dict"]):
                     if isinstance(t.valuetype, list):
                         outs += t.valuetype
                     else:
                         outs.append(t.valuetype)
                 else:
                     if isinstance(t.elementtype, list):
                         outs += t.elementtype
@@ -767,23 +769,23 @@
             # if target is dict, just add [] to rej.
             if TypeObject.existType("Dict", ttypes):
                 rej_itypes = []
             elif TypeObject.existType("List", ttypes) or TypeObject.existType("Tuple", ttypes) or TypeObject.existType(
                     "Text", ttypes):
                 # to check the rest 1 or 2
                 for it in itypes:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes.append(it)
 
             for t in ttypes:
-                if t.type not in ["Dict", "List", "Tuple", "Text", "bytes"]:
+                if not TypeObject.existSame(t, special_types["@subscriptable@"]):
                     rej_ttypes.append(t)
-                elif t.type in ["Text", "bytes"]:
+                elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
                     outs.append(t)
-                elif t.type == "Dict":
+                elif TypeObject.existSame(t, ["Dict"]):
                     if isinstance(t.valuetype, list):
                         outs += t.valuetype
                     else:
                         outs.append(t.valuetype)
                 else:
                     if isinstance(t.elementtype, list):
                         outs += t.elementtype
@@ -808,26 +810,26 @@
             if TypeObject.existType("Dict", ttypes):
                 rej_itypes = []
                 rej_itypes2 = []
             elif TypeObject.existType("List", ttypes) or TypeObject.existType("Tuple", ttypes) or TypeObject.existType(
                     "Text", ttypes):
                 # to check the rest 1 or 2
                 for it in itypes:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes.append(it)
                 for it in itypes2:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes2.append(it)
 
             for t in ttypes:
-                if t.type not in ["Dict", "List", "Tuple", "Text", "bytes"]:
+                if not TypeObject.existSame(t, special_types["@subscriptable@"]):
                     rej_ttypes.append(t)
-                elif t.type in ["Text", "bytes"]:
+                elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
                     outs.append(t)
-                elif t.type == "Dict":
+                elif TypeObject.existSame(t, ["Dict"]):
                     if isinstance(t.valuetype, list):
                         outs += t.valuetype
                     else:
                         outs.append(t.valuetype)
                 else:
                     if isinstance(t.elementtype, list):
                         outs += t.elementtype
@@ -857,29 +859,29 @@
                 rej_itypes = []
                 rej_itypes2 = []
                 rej_itypes3 = []
             elif TypeObject.existType("List", ttypes) or TypeObject.existType("Tuple", ttypes) or TypeObject.existType(
                     "Text", ttypes):
                 # to check the rest 1 or 2
                 for it in itypes:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes.append(it)
                 for it in itypes2:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes2.append(it)
                 for it in itypes3:
-                    if it.type not in ["int", "bool"]:
+                    if not TypeObject.existSame(it, ["int", "bool"]):
                         rej_itypes3.append(it)
 
             for t in ttypes:
-                if t.type not in ["Dict", "List", "Tuple", "Text"]:
+                if not TypeObject.existSame(t, special_types["@subscriptable@"]):
                     rej_ttypes.append(t)
-                elif t.type == "Text":
+                elif TypeObject.existSame(t, ["Text"]):
                     outs.append(TypeObject("Text", 0))
-                elif t.type == "Dict":
+                elif TypeObject.existSame(t, ["Dict"]):
                     if isinstance(t.valuetype, list):
                         outs += t.valuetype
                     else:
                         outs.append(t.valuetype)
                 else:
                     if isinstance(t.elementtype, list):
                         outs += t.elementtype
@@ -944,21 +946,28 @@
                     rej_arg_types = []
                     outs = []
                     accpetable_targettypes = []
                     returntypes = []
                     for i in range(1, len(operands)):
                         rej_arg_types.append([])
                     for k in builtin_method:
-                        if func in builtin_method[k]:
+                        if func in builtin_method[k] and k != "standalone":
                             accpetable_targettypes.append(k)
                     for t in target.types:
-                        if t.type.lower() in accpetable_targettypes:
-                            rule = builtin_method[t.type.lower()][func]
+                        if TypeObject.existSame(t, accpetable_targettypes):
+                            rule = builtin_method[TypeObject.findSame(t, accpetable_targettypes)][func]
                             if len(rule) == 2:
-                                if len(rule[0]) < len(operands) - 1:
+                                if len(rule[0]) == 0:
+                                    for o in operands:
+                                        rej_types.append([])
+                                    if "@" not in rule[1]:
+                                        returntypes = TypeObject.Str2Obj(rule[1])
+                                    else:
+                                        logger.warning("Unhandled return value for built-in function {}".format(func))
+                                elif len(rule[0]) < len(operands) - 1:
                                     rej_target_types.append(t)
                                     continue
                                 else:
                                     for index in range(1, len(operands)):
                                         if rule[0][index - 1][1] == "Any" or isinstance(rule[0][index - 1], list):
                                             rej_types.append([])
                                             continue
@@ -1035,15 +1044,15 @@
                                                     if not TypeObject.existType(ot, validtypes):
                                                         rej_arg_types[index - 1].append(ot)
                                             if "@" not in rule[-1]:
                                                 returntypes = TypeObject.Str2Obj(rule[-1])
                                             else:
                                                 logger.warning("Unhandled return value for built-in function {}".format(func))
 
-                        else:
+                        elif len(accpetable_targettypes) != 0:
                             rej_target_types.append(t)
                     rej_types = [rej_target_types] + rej_arg_types
                     outs = returntypes
                     return rej_types, outs
                 #standalone functions
                 else:
                     if func in builtin_method["standalone"]:
@@ -1074,34 +1083,36 @@
                                         rej_types[i].append(ot)
                             if "@" not in rule[-1]:
                                 returntypes = TypeObject.Str2Obj(rule[-1])
                             else:
                                 logger.warning("Unhandled return value for built-in function {}".format(func))
                         elif len(rule) > 2:
                             found = False
+                            validtypes = [[] for i in operands]
                             for r in rule:
                                 if isinstance(r, list) and len(r) == len(operands):
                                     found = True
                                     for i in range(0, len(operands)):
                                         if r[i][1] == "Any" or isinstance(r[i], list):
                                             rej_types.append([])
                                             continue
                                         elif r[i][1].startswith("@") and r[i][1] in special_types:
-                                            validtypes = []
+                                            #validtypes = []
                                             for t in special_types[r[i][1]]:
-                                                validtypes += TypeObject.Str2Obj(t)
+                                                validtypes[i] += TypeObject.Str2Obj(t)
                                         else:
-                                            validtypes = TypeObject.Str2Obj(r[i][1])
-                                        for ot in operands[i].types:
-                                            if not TypeObject.existType(ot, validtypes):
-                                                rej_types[i].append(ot)
-                                if "@" not in rule[-1]:
-                                    returntypes = TypeObject.Str2Obj(rule[-1])
-                                else:
-                                    logger.warning("Unhandled return value for built-in function {}".format(func))
+                                            validtypes[i] += TypeObject.Str2Obj(r[i][1])
+                            if "@" not in rule[-1]:
+                                returntypes = TypeObject.Str2Obj(rule[-1])
+                            else:
+                                logger.warning("Unhandled return value for built-in function {}".format(func))
+                            for i in range(0, len(operands)):
+                                for ot in operands[i].types:
+                                    if not TypeObject.existType(ot, validtypes[i]) and len(validtypes[i]) != 0:
+                                        rej_types[i].append(ot)
                             if found == False:
                                 for r in rule:
                                     if isinstance(r, list) and len(r) > len(operands) - 1:
                                         found = True
                                         for i in range(0, len(operands)):
                                             if r[i][1] == "Any" or isinstance(r[i], list):
                                                 rej_types.append([])
@@ -1138,17 +1149,17 @@
                     failed = False
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     temp = TypeObject("List", 0)
                     outs = []
                     for t in target.types:
-                        if t.type != "List":
+                        if not TypeObject.existSame(t, ["List"]):
                             rej_target_types.append(t)
-                        elif t.type == "List":
+                        elif TypeObject.existSame(t, ["List"]):
                             for types_t in t.elementtype:
                                 temp.elementtype.append(types_t)
                     if len(rej_target_types) == len(target.types):
                         outs += target.types
                         failed = True
                     rej_types.append(rej_target_types)
 
@@ -1174,15 +1185,15 @@
                     # mention that it will remove all the existing types!!!!!
                     #TODO how to deal with this situation?
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type not in ["List","Dict","set"]:
+                        if not TypeObject.existSame(t, ["List","Dict","set"]):
                             rej_target_types.append(t)
                         else:
                             temp = TypeObject(t.type, 0)
                             outs.append(temp)
                     rej_types.append(rej_target_types)
                     for i in range(1, len(operands)):
                         rej_types.append([])
@@ -1200,29 +1211,40 @@
                 if attr!=None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     temp = TypeObject("List", 0)
                     outs = []
                     for t in target.types:
-                        if t.type != "List":
+                        if not TypeObject.existSame(t, ["List"]):
                             rej_target_types.append(t)
-                        elif t.type =="List":
+                        elif TypeObject.existSame(t, ["List"]):
                             for types_t in t.elementtype:
                                 temp.elementtype.append(types_t)
                     rej_types.append(rej_target_types)
 
                     rej_target_types = []
                     for i in range(1, len(operands)):
                         for t in operands[i].types:
-                            if t.type!= "List":
+                            if not TypeObject.existSame(t, ["List", "Tuple", "str", "bytes", "bytearray", "Set", "frozenset", "Dict", "Generator", "IO"]):
                                 rej_target_types.append(t)
-                            for types_t in t.elementtype:
-                                if not TypeObject.existType(types_t, temp.elementtype):
-                                    temp.elementtype.append(types_t)
+                            if TypeObject.existSame(t, ["list", "tuple", "set", "frozenset", "Generator"]):
+                                for types_t in t.elementtype:
+                                    if not TypeObject.existType(types_t, temp.elementtype):
+                                        temp.elementtype.append(types_t)
+                            elif TypeObject.existSame(t, ["str", "IO"]):
+                                if not TypeObject.existType("str", temp.elementtype):
+                                    temp.elementtype.append(TypeObject("str", 0))
+                            elif TypeObject.existSame(t, ["bytes", "bytearray"]):
+                                if not TypeObject.existType("bytes", temp.elementtype):
+                                    temp.elementtype.append(TypeObject("bytes", 0))
+                            elif TypeObject.existSame(t, ["Dict"]):
+                                for types_t in t.keytype:
+                                    if not TypeObject.existType(types_t, temp.elementtype):
+                                        temp.elementtype.append(types_t)
                         rej_types.append(rej_target_types)
                     outs.append(temp)
                     return rej_types, outs
                 else:
                     rej_ltypes = []
                     for i in range(0, len(operands)):
                         rej_ltypes.append([])
@@ -1235,27 +1257,27 @@
                 if attr != None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     temp = TypeObject("List", 0)
                     outs = []
                     for t in target.types:
-                        if t.type != "List":
+                        if not TypeObject.existSame(t, ["List"]):
                             rej_target_types.append(t)
-                        elif t.type == "List":
+                        elif TypeObject.existSame(t, ["List"]):
                             for types_t in t.elementtype:
                                 temp.elementtype.append(types_t)
                     rej_types.append(rej_target_types)
 
                     # second one is int
                     if len(operands) > 1:
                         rej_target_types = []
                         sub_temp = operands[1]
                         for t in sub_temp.types:
-                            if t.type not in ["int","bool"]:
+                            if not TypeObject.existSame(t, ["int","bool"]):
                                 rej_target_types.append(t)
                         rej_types.append(rej_target_types)
 
                     rej_target_types = []
                     for i in range(1, len(operands)):
                         for t in operands[i].types:
                             if not TypeObject.existType(t, temp.elementtype):
@@ -1276,15 +1298,15 @@
                 # pop(key[,default])
                 if attr!=None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type not in  ["List","Dict", "Set"]:
+                        if not TypeObject.existSame(t, ["List","Dict", "Set"]):
                             rej_target_types.append(t)
                         else:
                             # here we don't change the possible types in it because it's hard to say
                             outs.append(t)
                     rej_types.append(rej_target_types)
                     # the second one has to be int(for list),if there is
                     for i in range(1, len(operands)):
@@ -1304,15 +1326,15 @@
                     #aList.remove('xyz');
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     temp = None
                     for t in target.types:
-                        if t.type not in ["List", "Set"]:
+                        if not TypeObject.existSame(t, ["List", "Set"]):
                             rej_target_types.append(t)
                         else:
                             # here we don't change the possible types in it because it's hard to say
                             temp  =deepcopy(t)
                             outs.append(temp)
                     rej_types.append(rej_target_types)
                     # the second one has to be int(for list),if there is
@@ -1336,33 +1358,42 @@
                 # dict.update(dict2)
                 # it is also possible that it's a user-defined function
                     if len(operands)>0:
                         rej_types = []
                         target = operands[0]
                         rej_target_types = []
                         outs = []
-                        temp = TypeObject("Dict",0)
+                        temp = None
                         for t in target.types:
-                            if t.type not in ["Dict"]:
+                            if not TypeObject.existSame(t, ["Dict", "Set"]):
                                 rej_target_types.append(t)
                             else:
                                 temp = deepcopy(t)
 
                         rej_types.append(rej_target_types)
                         # the second one has to be int(for list),if there is
                         if len(operands) > 1:
                             target = operands[1]
                             rej_target_types = []
-                            for t in target.types:
-                                if t.type not in ["Dict"]:
-                                    rej_target_types.append(t)
-                                else:
-                                    temp.keytype += t.keytype
-                                    temp.valuetype += t.valuetype
-                                    temp.elementtype = temp.keytype
+                            if temp != None:
+                                for t in target.types:
+                                    if not TypeObject.existSame(t, ["List", "Tuple", "range", "str", "bytes", "bytearray", "Set", "frozenset", "Dict", "IO"]):
+                                        rej_target_types.append(t)
+                                    elif TypeObject.existSame(t, ["str", "IO"]):
+                                        if not TypeObject.existType("str", temp.elementtype):
+                                            temp.elementtype.append(TypeObject("str", 0))
+                                    elif TypeObject.existSame(t, ["bytes", "bytearray"]):
+                                        if not TypeObject.existType("bytes", temp.elementtype):
+                                            temp.elementtype.append(TypeObject("bytes", 0))
+                                    elif TypeObject.existSame(temp, ["Dict"]):
+                                        temp.keytype += t.keytype
+                                        temp.valuetype += t.valuetype
+                                        temp.elementtype = temp.keytype
+                                    else:
+                                        temp.elementtype += t.elementtype
 
                             rej_types.append(rej_target_types)
                         if len(operands)>2:
                             for i in range(2, len(operands)):
                                 rej_types.append([])
 
                         if temp!= None:
@@ -1392,28 +1423,28 @@
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
 
                     temp = None
                     outs = []
                     for t in target.types:
-                        if t.type not in ["Set"]:
+                        if not TypeObject.existSame(t, ["Set"]):
                             rej_target_types.append(t)
-                        elif t.type == "Set":
+                        elif TypeObject.existSame(t, ["Set"]):
                             temp = deepcopy(t)
                     rej_types.append(rej_target_types)
 
                     if func!="union":
                         # TODO! maybe we can infer a more specific one? but too consuming now.
                         if len(operands) > 1:
                             for i in range(1, len(operands)):
                                 target = operands[i]
                                 rej_target_types = []
                                 for t in target.types:
-                                    if t.type not in ["Set"]:
+                                    if not TypeObject.existSame(t, ["Set"]):
                                         rej_target_types.append(t)
                                 rej_types.append(rej_target_types)
 
                         if temp != None:
                             outs.append(temp)
                         else:
                             outs = []
@@ -1421,15 +1452,15 @@
 
                     else:
                         if len(operands) > 1:
                             for i in range(1, len(operands)):
                                 target = operands[i]
                                 rej_target_types = []
                                 for t in target.types:
-                                    if t.type not in ["Set"]:
+                                    if not TypeObject.existSame(t, ["Set"]):
                                         rej_target_types.append(t)
                                     else:
                                         for eletype in t.elementtype:
                                             if not TypeObject.existType(eletype.type, temp.elementtype):
                                                 temp.elementtype.append(eletype)
 
                                 rej_types.append(rej_target_types)
@@ -1455,24 +1486,24 @@
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
 
                     temp = None
                     outs = []
                     for t in target.types:
-                        if t.type not in ["Set"]:
+                        if not TypeObject.existSame(t, ["Set"]):
                             rej_target_types.append(t)
-                        elif t.type == "Set":
+                        elif TypeObject.existSame(t, ["Set"]):
                             temp = deepcopy(t)
                     rej_types.append(rej_target_types)
 
                     target = operands[1]
                     rej_target_types = []
                     for t in target.types:
-                        if t.type not in ["Set"]:
+                        if not TypeObject.existSame(t, ["Set"]):
                             rej_target_types.append(t)
                     rej_types.append(rej_target_types)
 
                     if len(operands)>2:
                         for i in range(2,len(operands)):
                             rej_types.append([])
 
@@ -1496,17 +1527,17 @@
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
 
                     temp = None
                     outs = []
                     for t in target.types:
-                        if t.type not in ["Set"]:
+                        if not TypeObject.existSame(t, ["Set"]):
                             rej_target_types.append(t)
-                        elif t.type=="Set":
+                        elif TypeObject.existSame(t, ["Set"]):
                             temp = deepcopy(t)
                     rej_types.append(rej_target_types)
 
                     for i in range(1, len(operands)):
                         rej_types.append([])
                         target = operands[i]
                         # add the possible types in it
@@ -1534,24 +1565,24 @@
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
 
                     temp = None
                     outs = []
                     for t in target.types:
-                        if t.type not in ["Set"]:
+                        if not TypeObject.existSame(t, ["Set"]):
                             rej_target_types.append(t)
-                        elif t.type == "Set":
+                        elif TypeObject.existSame(t, ["Set"]):
                             temp = deepcopy(t)
                     rej_types.append(rej_target_types)
 
                     target = operands[1]
                     rej_target_types = []
                     for t in target.types:
-                        if t.type not in ["Set"]:
+                        if not TypeObject.existSame(t, ["Set"]):
                             rej_target_types.append(t)
                         else:
                             for eletype in t.elementtype:
                                 if not TypeObject.existType(eletype.type,temp.elementtype):
                                     temp.elementtype.append(eletype)
                     rej_types.append(rej_target_types)
 
@@ -1578,15 +1609,15 @@
                 if attr!=None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     temp = TypeObject("Tuple",0)
                     for t in target.types:
-                        if t.type not in ["Dict"]:
+                        if not TypeObject.existSame(t, ["Dict"]):
                             rej_target_types.append(t)
                         else:
                             temp.elementtype += t.keytype
                             temp.elementtype += t.valuetype
                     rej_types.append(rej_target_types)
                     # the second one has to be int(for list),if there is
                     for i in range(1, len(operands)):
@@ -1605,15 +1636,15 @@
                 # a.setdefault('Sex', "Never")
                 if attr!=None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type not in ["Dict"]:
+                        if not TypeObject.existSame(t, ["Dict"]):
                             rej_target_types.append(t)
                         else:
                             for item in t.valuetype:
                                 if item!=None:
                                     outs.append(item)
                     rej_types.append(rej_target_types)
                     # the second one has to be int(for list),if there is
@@ -1624,15 +1655,14 @@
                         rej_types.append([])
                         for itypes in operands[2].types:
                             if not TypeObject.existSame(itypes,outs):
                                 outs.append(itypes)
                     else:
                         for i in range(1, len(operands)):
                             rej_types.append([])
-                    print(len(outs))
                     return rej_types, outs
                 else:
                     rej_ltypes = []
                     for i in range(0, len(operands)):
                         rej_ltypes.append([])
                     outs = []
                     return rej_ltypes, outs
@@ -1644,17 +1674,17 @@
             elif func=="copy":
                 if attr!=None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type not in ["List", "Dict", "set"]:
+                        if not TypeObject.existSame(t, ["List", "Dict", "Set"]):
                             rej_target_types.append(t)
-                        elif t.type in ["List", "Dict", "set"]:
+                        elif TypeObject.existSame(t, ["List", "Dict", "Set"]):
                             outs.append(t)
                     rej_types.append(rej_target_types)
                     for i in range(1, len(operands)):
                         rej_types.append([])
                     return rej_types, outs
                 else:
                     rej_ltypes = []
@@ -1666,15 +1696,15 @@
             elif func == "items":
                 if attr != None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type != "Dict":
+                        if not TypeObject.existSame(t, ["Dict"]):
                             rej_target_types.append(t)
                         else:
                             temp = TypeObject("set", 0)
                             innerlist = TypeObject("List", 0)
                             for k in t.keytype:
                                 for v in t.valuetype:
                                     innertuple = TypeObject("Tuple", 0)
@@ -1683,67 +1713,85 @@
                                     innerlist.elementtype.append(innertuple)
                             temp.elementtype.append(innerlist)
                             outs.append(temp)
                     rej_types.append(rej_target_types)
                     for i in range(1, len(operands)):
                         rej_types.append([])
                     return rej_types, outs
+                else:
+                    rej_ltypes = []
+                    for i in range(0, len(operands)):
+                        rej_ltypes.append([])
+                    outs = []
+                    return rej_ltypes, outs
             
             elif func == "keys":
                 if attr != None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type != "Dict":
+                        if not TypeObject.existSame(t, ["Dict"]):
                             rej_target_types.append(t)
                         else:
                             temp = TypeObject("set", 0)
                             innerlist = TypeObject("List", 0)
                             for k in t.keytype:
                                 innerlist.elementtype.append(k)
                             temp.elementtype.append(innerlist)
                             outs.append(temp)
                     rej_types.append(rej_target_types)
                     for i in range(1, len(operands)):
                         rej_types.append([])
                     return rej_types, outs
+                else:
+                    rej_ltypes = []
+                    for i in range(0, len(operands)):
+                        rej_ltypes.append([])
+                    outs = []
+                    return rej_ltypes, outs
 
             elif func == "values":
                 if attr != None:
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type != "Dict":
+                        if not TypeObject.existSame(t, ["Dict"]):
                             rej_target_types.append(t)
                         else:
                             temp = TypeObject("set", 0)
                             innerlist = TypeObject("List", 0)
                             for k in t.valuetype:
                                 innerlist.elementtype.append(k)
                             temp.elementtype.append(innerlist)
                             outs.append(temp)
                     rej_types.append(rej_target_types)
                     for i in range(1, len(operands)):
                         rej_types.append([])
                     return rej_types, outs
+                else:
+                    rej_ltypes = []
+                    for i in range(0, len(operands)):
+                        rej_ltypes.append([])
+                    outs = []
+                    return rej_ltypes, outs
 
             elif func == "abs":
                 # as for NOTAttribute function, we have to make sure self.attr==None
                 if attr == None:
                     ltypes = operands[0].types
                     rej_target_types = []
                     rej_ltypes = []
 
                     outs = []
                     for t in ltypes:
-                        if t.type not in ["bool", "int", "float", "complex"]:
+                        if not TypeObject.existSame(t, special_types["@number@"]):
                             rej_target_types.append(t)
                         elif not TypeObject.existSame(t, outs):
                             if t !=None:
                                 outs.append(t)
                     rej_ltypes.append(rej_target_types)
                     for i in range(1, len(operands)):
                         rej_ltypes.append([])
@@ -1762,18 +1810,18 @@
                     right = operands[1]
                     ltypes = left.types
                     rtypes = right.types
                     basic_type = TypeObject("int", 0)
                     llevel = rlevel = 1
                     for lt in ltypes:
                         if TypeObject.isCompatible(lt, basic_type):
-                            llevel = max(llevel, ["bool", "int", "float", "complex"].index(lt.type))
+                            llevel = max(llevel, special_types["@number@"].index(lt.type))
                     for rt in rtypes:
                         if TypeObject.isCompatible(rt, basic_type):
-                            rlevel = max(rlevel, ["bool", "int", "float", "complex"].index(rt.type))
+                            rlevel = max(rlevel, special_types["@number@"].index(rt.type))
                     if llevel < 2 and rlevel < 2:
                         [rej_ltypes, rej_rtypes], outs = self.binop_num_op(left, right, "%")
                     else:
                         [rej_ltypes, rej_rtypes], outs = self.binop_num_op(left, right, "/")
                     finalouts = TypeObject("Tuple", 0)
                     finalouts.buildTuple(outs)
                     return [rej_ltypes, rej_rtypes], finalouts
@@ -1789,21 +1837,25 @@
                 if len(operands) <= 2 and len(operands) >= 1:
                     rej_types = []
                     outs = []
                     elementtype = []
                     for i in operands:
                         rej_types.append([])
                     for t in operands[0].types:
-                        if t.type not in special_types["@iterable@"]:
+                        if not TypeObject.existSame(t, special_types["@iterable@"]):
                             rej_types[0].append(t)
+                        elif TypeObject.existSame(t, ["Dict"]):
+                            elementtype += t.keytype
+                        elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                            elementtype.append(t)
                         else:
                             elementtype += t.elementtype
                     if len(operands) == 2:
                         for t in operands[1].types:
-                            if t.type != "int":
+                            if not TypeObject.existSame(t, ["bool", "int"]):
                                 rej_types[1].append(t)
                     temp = TypeObject("Generator", 0)
                     for e in elementtype:
                         innertuple = TypeObject("Tuple", 0)
                         innertuple.elementtype = [TypeObject("int", 0), e]
                         temp.elementtype.append(innertuple)
                     outs.append(temp)
@@ -1822,15 +1874,15 @@
                     if len(operands)==1:
                         ltypes = operands[0].types
                         rej_target_types = []
                         rej_ltypes = []
                         temp = TypeObject("int", 0)
                         outs = []
                         for t in ltypes:
-                            if t.type not in ["bool", "int", "float", "complex"]:
+                            if not TypeObject.existSame(t, special_types["@number@"]):
                                 rej_target_types.append(t)
 
                         rej_ltypes.append(rej_target_types)
 
                         for i in range(1, len(operands)):
                             rej_ltypes.append([])
                         outs.append(temp)
@@ -1841,20 +1893,20 @@
                         rtypes = operands[1].types
                         rej_target_types =  rej_rtarget_types=[]
                         rej_ltypes = []
 
                         temp = TypeObject("float", 0)
                         outs = []
                         for t in ltypes:
-                            if t.type not in ["bool", "int", "float", "complex"]:
+                            if not TypeObject.existSame(t, special_types["@number@"]):
                                 rej_target_types.append(t)
                         rej_ltypes.append(rej_target_types)
 
                         for t in rtypes:
-                            if t.type not in ["bool", "int"]:
+                            if not TypeObject.existSame(t, ["bool", "int"]):
                                 rej_rtarget_types.append(t)
                         rej_ltypes.append(rej_rtarget_types)
                         outs.append(temp)
                         return rej_ltypes, outs
                 else:
                     rej_ltypes = []
                     for i in range(0, len(operands)):
@@ -1868,16 +1920,20 @@
                 if attr == None:
                     first = operands[0].types
                     rej_target_types = []
                     rej_ltypes = []
                     temp = TypeObject("List", 0)
                     outs = []
                     for t in first:
-                        if t.type not in ["List", "Tuple", "Set", "Dict", "Iterable", "Text"]:
+                        if not TypeObject.existSame(t, special_types["@iterable@"]):
                             rej_target_types.append(t)
+                        elif TypeObject.existSame(t, ["Dict"]):
+                            temp.elementtype += t.keytype
+                        elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                            temp.elementtype.append(t)
                         else:
                             if isinstance(t.elementtype, list):
                                 temp.elementtype += t.elementtype
                             else:
                                 temp.elementtype.append(t.elementtype)
 
                     rej_ltypes.append(rej_target_types)
@@ -1900,31 +1956,31 @@
                     first = operands[0].types
                     rej_target_types = []
                     rej_ltypes = []
                     isinitial = True
                     outs = []
                     simplelevel_up = 0
                     for t in first:
-                        if t.type not in ["List", "Tuple", "Set", "Dict", "Iterable", "Text"]:
+                        if not TypeObject.existSame(t, special_types["@iterable@"]):
                             rej_target_types.append(t)
                         for elet in t.elementtype:
                             if isinitial:
                                 isinitial = False
-                                if elet.type in ["bool", "int", "float", "complex"]:
-                                    simplelevel_up = ["bool", "int", "float", "complex"].index(elet.type)
+                                if TypeObject.existSame(elet, special_types["@number@"]):
+                                    simplelevel_up = special_types["@number@"].index(elet.type)
                                 else:
                                     simplelevel_up = 0
                             else:
-                                if elet.type in ["bool", "int", "float", "complex"]:
+                                if TypeObject.existSame(elet, special_types["@number@"]):
 
-                                    simplelevel_up = max(["bool", "int", "float", "complex"].index(elet.type), simplelevel_up)
+                                    simplelevel_up = max(special_types["@number@"].index(elet.type), simplelevel_up)
                                 else:
                                     simplelevel_up = max(1,simplelevel_up)
 
-                    temp = TypeObject(["bool", "int", "float", "complex"][simplelevel_up],"0")
+                    temp = TypeObject(special_types["@number@"][simplelevel_up], 0)
 
                     rej_ltypes.append(rej_target_types)
 
                     for i in range(1, len(operands)):
                         rej_ltypes.append([])
                     outs.append(temp)
                     return rej_ltypes, outs
@@ -1943,20 +1999,20 @@
                         outs = TypeObject("Tuple", 0)
                         return [], [outs]
                     else:
                         ltypes = operands[0].types
                         rej_ltypes = []
                         outs = TypeObject("Tuple", 0)
                         for t in ltypes:
-                            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+                            if not TypeObject.existSame(t, special_types["@iterable@"]):
                                 rej_ltypes.append(t)
-                            elif t.type == "Dict":
+                            elif TypeObject.existSame(t, ["Dict"]):
                                 outs.elementtype = t.keytype
-                            elif t.type == "Text":
-                                outs.elementtype.append(TypeObject("Text", 0))
+                            elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                                outs.elementtype.append(t)
                             else:
                                 outs.elementtype = t.elementtype
                         return [rej_ltypes], outs
                 else:
                     rej_ltypes = []
                     for i in range(0, len(operands)):
                         rej_ltypes.append([])
@@ -1971,20 +2027,20 @@
                         outs = TypeObject("List", 0)
                         return [], [outs]
                     elif len(operands) == 1:
                         ltypes = operands[0].types
                         rej_ltypes = []
                         outs = TypeObject("List", 0)
                         for t in ltypes:
-                            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+                            if not TypeObject.existSame(t, special_types["@iterable@"]):
                                 rej_ltypes.append(t)
-                            elif t.type == "Dict":
+                            elif TypeObject.existSame(t, ["Dict"]):
                                 outs.elementtype = t.keytype
-                            elif t.type == "Text":
-                                outs.elementtype.append(TypeObject("Text", 0))
+                            elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                                outs.elementtype.append(t)
                             else:
                                 outs.elementtype = t.elementtype
                         return [rej_ltypes], outs
                     else:
                         rej_ltypes = []
                         for i in range(0, len(operands)):
                             rej_ltypes.append([])
@@ -2005,20 +2061,20 @@
 
                         outs = TypeObject("Set", 0)
                         return [], [outs]
                     elif len(operands)==1:
                         ltypes = operands[0].types
                         outs = TypeObject("Set", 0)
                         for t in ltypes:
-                            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+                            if not TypeObject.existSame(t, special_types["@iterable@"]):
                                 rej_ltypes.append(t)
-                            elif t.type == "Dict":
+                            elif TypeObject.existSame(t, ["Dict"]):
                                 outs.elementtype = t.keytype
-                            elif t.type == "Text":
-                                outs.elementtype.append(TypeObject("Text", 0))
+                            elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                                outs.elementtype.append(t)
                             else:
                                 outs.elementtype = t.elementtype
                         return [rej_ltypes], [outs]
                     else:
                         for i in range(0, len(operands)):
                             rej_ltypes.append([])
                         outs = []
@@ -2037,20 +2093,20 @@
 
                         outs = TypeObject("frozenset", 0)
                         return [], [outs]
                     else:
                         ltypes = operands[0].types
                         outs = TypeObject("Set", 0)
                         for t in ltypes:
-                            if t.type not in ["Tuple", "List", "Set", "Dict", "Text"]:
+                            if not TypeObject.existSame(t, special_types["@iterable@"]):
                                 rej_ltypes.append(t)
-                            elif t.type == "Dict":
+                            elif TypeObject.existSame(t, ["Dict"]):
                                 outs.elementtype = t.keytype
-                            elif t.type == "Text":
-                                outs.elementtype.append(TypeObject("Text", 0))
+                            elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                                outs.elementtype.append(t)
                             else:
                                 outs.elementtype = t.elementtype
                         return [rej_ltypes], [outs]
                 else:
                     for i in range(0, len(operands)):
                         rej_ltypes.append([])
                     outs = []
@@ -2066,21 +2122,21 @@
                         temp.elementtype = operands[0].types
                         outs.append(temp)
                         return rej_types, outs
                     elif len(operands) == 3:
                         rej_types = [[], [], []]
                         outs = []
                         for t in operands[0].types:
-                            if not TypeObject.equal2type(t, "str"):
+                            if not TypeObject.existSame(t, ["str"]):
                                 rej_types[0].append(t)
                         for t in operands[1].types:
-                            if not TypeObject.equal2type(t, "tuple"):
+                            if not TypeObject.existSame(t, ["tuple"]):
                                 rej_types[1].append(t)
                         for t in operands[2].types:
-                            if not TypeObject.equal2type(t, "dict"):
+                            if not TypeObject.existSame(t, ["dict"]):
                                 rej_types[2].append(t)
                         temp = TypeObject("type", 0)
                         outs.append(temp)
                         return rej_types, outs
                     else:
                         rej_types = []
                         outs = []
@@ -2099,15 +2155,15 @@
                     if len(operands) == 1:
                         rej_types = []
                         outs = []
                         elementtype = []
                         for i in range(0, len(operands)):
                             rej_types.append([])
                         for t in operands[0].types:
-                            if t.type != "Generator":
+                            if not TypeObject.existSame(t, ["Generator"]):
                                 rej_types[0].append(t)
                             else:
                                 elementtype = t.elementtype
                         outs += elementtype
                         return rej_types, outs
                     else:
                         rej_ltypes = []
@@ -2129,21 +2185,23 @@
                     ltypes = operands[0].types
                     rej_target_types = []
                     rej_ltypes = []
                     outs = []
                     if len(operands)==1:
                         temp = []
                         for t in ltypes:
-                            if t.type not in ["List", "Tuple", "Set", "Dict", "Iterable", "Text"]:
+                            if not TypeObject.existSame(t, special_types["@iterable@"]):
                                 rej_target_types.append(t)
-                            elif t.type == "Dict":
-                                if isinstance(t.elementtype, list):
-                                    outs += t.elementtype
+                            elif  TypeObject.existSame(t, ["Dict"]):
+                                if isinstance(t.keytype, list):
+                                    outs += t.keytype
                                 else:
-                                    outs.append(t.elementtype)
+                                    outs.append(t.keytype)
+                            elif TypeObject.existSame(t, ["Text", "bytes", "bytearray"]):
+                                outs.append(t)
                             else:
                                 if t.elementtype!=[]:
                                     if t.elementtype[0]!= None:
                                         outs.append(t.elementtype[0]) # for list/dict is also okay as it returns keytype
                         rej_ltypes.append(rej_target_types)
                         for i in range(1, len(operands)):
                             rej_ltypes.append([])
@@ -2153,44 +2211,44 @@
                     else:
                         ifsimple = False
                         first = operands[0]
                         simplelevel_up =simplelevel_down =  0
                         isinitial = True
                         for indexop in operands:
                             for ftypes in indexop.types:
-                                if ftypes.type not in ["List", "Tuple", "Set", "Dict", "Iterable", "Text"]:
+                                if not TypeObject.existSame(ftypes, special_types["@iterable@"]):
                                     ifsimple = True
                                     if isinitial:
                                         isinitial = False
-                                        if ftypes.type in ["bool", "int", "float", "complex"]:
-                                            simplelevel_up = simplelevel_down = ["bool", "int", "float", "complex"].index(ftypes.type)
+                                        if TypeObject.existSame(ftypes, special_types["@number@"]):
+                                            simplelevel_up = simplelevel_down = special_types["@number@"].index(ftypes.type)
                                         else:
                                             simplelevel_up = simplelevel_down = 1
                                     else:
-                                        if ftypes.type in ["bool", "int", "float", "complex"]:
-                                            simplelevel_up = max(["bool", "int", "float", "complex"].index(ftypes.type),simplelevel_up)
-                                            simplelevel_down = min(["bool", "int", "float", "complex"].index(ftypes.type), simplelevel_down)
+                                        if TypeObject.existSame(ftypes, special_types["@number@"]):
+                                            simplelevel_up = max(special_types["@number@"].index(ftypes.type),simplelevel_up)
+                                            simplelevel_down = min(special_types["@number@"].index(ftypes.type), simplelevel_down)
                                         else:
                                             simplelevel_up = max(1,simplelevel_up)
                                             simplelevel_down = max(1,simplelevel_down)
                                 # if it's like b = max([1,2],[0,4])
-                                elif ftypes.type == "Dict":
+                                elif TypeObject.existSame(ftypes, ["Dict"]):
                                     outs += ftypes.keytype
                                     for i in range(0, len(operands)):
                                         rej_ltypes.append([])
                                     return rej_ltypes, outs
                                 else:
                                     if len(outs)==0:
                                         outs.append(ftypes)
                                     elif not TypeObject.existSame(ftypes,outs):
                                         outs.append(ftypes)
                         # add all the possible types
                         if ifsimple:
                             for i in range(simplelevel_down,simplelevel_up+1):
-                                temp = TypeObject(["bool", "int", "float", "complex"][i],"0")
+                                temp = TypeObject(special_types["@number@"][i],"0")
                                 outs.append(temp)
 
                         for i in range(0, len(operands)):
                             rej_ltypes.append([])
                         return rej_ltypes, outs
                 else:
                     rej_ltypes = []
@@ -2203,15 +2261,15 @@
                 if attr!=None:
                     # a.get('Sex', "Never")
                     rej_types = []
                     target = operands[0]
                     rej_target_types = []
                     outs = []
                     for t in target.types:
-                        if t.type not in ["Dict"]:
+                        if not TypeObject.existSame(t, ["Dict"]):
                             rej_target_types.append(t)
                         else:
                             for item in t.valuetype:
                                 if item!=None:
                                     outs.append(item)
                     rej_types.append(rej_target_types)
                     # the second one has to be int(for list),if there is
@@ -2391,15 +2449,15 @@
     def Dict_Read(self,operands):
         # similiar to List Read,but add keytype and valuetype
         rej_types = []
         outs = []
         temp = TypeObject("Dict", 0)
         # according to the rules, the first half are keytypes and the left half are valuetypes
         if(len(operands)%2!=0):
-            print('len(operands) is odd. case a: lambda case b: {**kw}' )
+            logger.warning('len(operands) is odd. case a: lambda case b: {**kw}' )
         for i in range(int(len(operands)/2)):
             if isinstance(operands[i].types, list):
                 temp.elementtype += operands[i].types
             else:
                 temp.elementtype.append(operands[i].types)
         temp.keytype = temp.elementtype
         for i in range(int(len(operands)/2),len(operands)):
```

### Comparing `hityper-1.0.2/hityper/usertype_finder.py` & `hityper-1.0.3/hityper/usertype_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 
     def parse_initfiles(self, path, repopaths):
         if not os.path.isfile(path):
             return None
         else:
             source = open(path, "r").read()
             root = ast.parse(source)
-            a = analyzer(path, "/".join(repopaths), self.validate)
+            a = UsertypeFinder(path, "/".join(repopaths), self.validate)
             types, _ = a.run(root)
             return types
             
     def scan_file(self, filepath, name, repopaths):
         if filepath.endswith(".py"):
             filepath = filepath.replace(".py", "")
         if(os.path.isdir(filepath) and filepath not in scaned_files):
```

### Comparing `hityper-1.0.2/hityper.egg-info/PKG-INFO` & `hityper-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-Metadata-Version: 2.1
-Name: hityper
-Version: 1.0.2
-Summary: HiTyper: A hybrid type inference framework for Python
-Home-page: https://github.com/JohnnyPeng18/HiTyper
-Author: Yun Peng
-Author-email: research@yunpeng.work
-License: UNKNOWN
-Keywords: python,type inference,static analysis
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HiTyper
 ![](https://img.shields.io/badge/Version-1.0-blue)
 
 
 
 This is the tool released in the ICSE 2022 paper ["Static Inference Meets Deep Learning: A Hybrid Type InferenceApproach for Python"](https://arxiv.org/abs/2105.03595).
 
+## Updates
+
+**8 Aug, 2022:** 
+
+We add a new command `hityper preprocess` to transform the json files in ManyTypes4py datasets into the `groundtruth.json` and `detailed_groundtruth.json` files HiTyper needs under `hityper eval`. 
+
+We also add a new option `-g` in `hityper findusertype` to collect the `usertypes.json` HiTyper needs under `hityper eval` according to the groundtruth file `groundtruth.json`.
+
 ## Workflow
 
 HiTyper is a hybrid type inference tool built upon Type Dependency Graph (TDG), the typical workflow of it is as follows:
 
 ![](https://github.com/JohnnyPeng18/HiTyper/blob/main/imgs/workflow.png)
 
 For more details, please refer to the [paper](https://arxiv.org/abs/2105.03595).
@@ -40,25 +29,29 @@
 
 2) Deep learning models are feature-agnostic but they can hardly maintain the type correctness and are unable to predict unseen user-defined types
 
 The combination of static inference and deep learning shall complement each other and improve the coverage while maintaining the accuracy.
 
 ## Install
 
-To use HiTyper on your own computer, you can simply type:
+1. Install HiTyper from source
+
+To use HiTyper on your own computer, you can build from source: (If you need to modify the source code of HiTyper, please use this method and re-run the `pip install .` after modification each time)
 
 ```sh
-pip install hityper
+git clone https://github.com/JohnnyPeng18/HiTyper.git && cd HiTyper
+pip install .
 ```
 
-or build from source: (If you need to modify the source code of HiTyper, please use this method and re-run the `pip install .` after modification each time)
+2. Install HiTyper using `pip`
+
+You can install the latest version of HiTyper by using the following command:
 
 ```sh
-git clone https://github.com/JohnnyPeng18/HiTyper.git && cd HiTyper
-pip install .
+pip install hityper
 ```
 
 **Requirements:**
 
 - Python>=3.9
 - Linux
 
@@ -73,34 +66,57 @@
 ## Usage
 
 Currently HiTyper has the following command line options: (Some important settings are stored in file `config.py`, you may need to modify it before running HiTyper)
 
 ### findusertype
 
 ```sh
-hityper findusertype [-h] [-s SOURCE] -p REPO [-v] [-d OUTPUT_DIRECTORY]
+usage: hityper findusertype [-h] [-s SOURCE] [-p REPO] [-g GROUNDTRUTH] [-c CORE] [-v] [-d OUTPUT_DIRECTORY]
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SOURCE, --source SOURCE
                         Path to a Python source file
   -p REPO, --repo REPO  Path to a Python project
+  -g GROUNDTRUTH, --groundtruth GROUNDTRUTH
+                        Path to a ground truth file
+  -c CORE, --core CORE  Number of cores to use when collecting user-defined types
   -v, --validate        Validate the imported user-defined types by finding their implementations
   -d OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
                         Path to the store the usertypes
 ```
 
-**Example:**
+**Example of collecting user-defined types in source files:**
 
 ```sh
 hityper findusertype -s python_project_repo/test.py -p python_project_repo -v -d outputs
 ```
 
 *This command generates the user-defined types collected by HiTyper and save them as `.json` files under `outputs/` folder.*
 
+`-p` option is required here, if you do not specify `-s`, the HiTyper will collect user-defined types in all files of repo specified by `-p`.
+
+**[Newly Added 6 Aug]**
+
+We add a option to automatically generate all user-defined type files that a ground truth dataset needs to evaluate HiTyper.
+
+**Example of collecting user-defined types in groundtruth datasets:**
+
+```sh
+hityper findusertype -g groundtruth.json -p repo_prefix -c 60 -d outputs
+```
+
+*This command generates the user-defined types in files indicates by `groundtruth.json` collected by HiTyper and save them as `.json` files under `outputs/` folder.*
+
+For the `groundtruth.json`, you need to use the same file in `hityper eval` command or generate it by using `hityper preprocess` command.
+
+`-p repo_prefix` is an optional argument here, if the filenames in `groundtruth.json` are the absolute paths then you do not need to specify `-p`, otherwise use `-p` to indicate which folder the source files are stored.
+
+The collection of all user-defined types for a large dataset is quite slow, try to specify a large number of cores used to make this process faster.
+
 ### gentdg
 
 ```sh
 hityper gentdg [-h] [-s SOURCE] -p REPO [-o] [-l LOCATION] [-a] [-c] [-d OUTPUT_DIRECTORY] [-f {json,pdf}]
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -124,14 +140,16 @@
 hityper gentdg -s python_project_repo/test.py -p python_project_repo -d outputs -f json -o
 ```
 
 *This command generates the TDG for all functions in file `python_project_repo/test.py` and save them into `outputs` folder.* 
 
 Note that if you choose `json` format to save TDG, it will be only ONE `json` file that contains all TDGs in the source file. However, if you choose `pdf` format to save TDG, then there will be multiple `pdf` files and each one correspond to one function in the source file. This is because a pdf file can hardly contain a large TDG for every functions.
 
+For the location indicated by `-l`, use the format `funcname@classname` and use `global` as the classname if the function is a global function.
+
 HiTyper uses [PyCG](https://github.com/vitsalis/PyCG) to build call graphs in call analysis. Alias analysis and call analysis are temporarily built-in but HiTyper does not use them in inference. Further updates about them will be involved in HiTyper. 
 
 ### infer
 
 ```sh
 hityper infer [-h] [-s SOURCE] -p REPO [-l LOCATION] [-d OUTPUT_DIRECTORY] [-m RECOMMENDATIONS] [-t] [-n TOPN]
 
@@ -156,29 +174,33 @@
 hityper infer -s python_project_repo/test.py -p python_project_repo -d outputs -n 1 -t 
 ```
 
 *This command generates the inferred types for all variables, arguments and return values in the source file and save them into `output` folder.*
 
 If you do not specify `-m` or `-t` option, then HiTyper will only use the static inference part to infer types. Static inference generally takes several minutes.
 
+For the location indicated by `-l`, use the format `funcname@classname` and use `global` as the classname if the function is a global function.
+
 **Recommendation Model:**
 
 Note that HiTyper natively supports the recommendations from Type4Py and it invokes the following API provided by Type4Py to get recommendations if you use option `-t`:
 
 ```
 https://type4py.com/api/predict?tc=0
 ```
 
 **This will upload your file to the Type4Py server!** If you do not want to upload your file, you can use the [docker](https://github.com/saltudelft/type4py/wiki/Using-Type4Py-Rest-API) provided by Type4Py and changes the API in `config.py` into:
 
 ```
 http://localhost:PORT/api/predict?tc=0
 ```
 
-**HiTyper's performance deeply depends on the maximum performance of recommendation model (especially the performance to predict argument types)** 
+According to our experiments, the Type4Py model has much lower performance by quering the API above, you are suggested to train the model locally and generate the recommendation file which can be passed to `-m`.
+
+**Note: HiTyper's performance deeply depends on the maximum performance of recommendation model (especially the performance to predict argument types). Type inference of HiTyper can fail if the recommendation model cannot give a valid prediction while static inference does not work!** 
 
 If you want to use another more powerful model, you write code like `__main__.py` to adapt HiTyper to your DL model.
 
 ### eval
 
 ```sh
 hityper eval [-h] -g GROUNDTRUTH -c CLASSIFIED_GROUNDTRUTH -u USERTYPE [-m RECOMMENDATIONS] [-t] [-n TOPN]
@@ -205,14 +227,39 @@
 
 *This command evaluates the performance of HiTyper on a pre-defined groundtruth dataset. It will output similar results like stated in `Experiment Results` part.*
 
 Before evaluating Hityper using this command, please use `hityper findusertype` command to generate `usertypes.json`. This typically takes several hours, depending on the number of files.
 
 This option is designed only for future research evaluation.
 
+### Preprocess
+
+```sh
+usage: hityper preprocess [-h] -p JSON_REPO [-d OUTPUT_DIRECTORY]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p JSON_REPO, --json_repo JSON_REPO
+                        Path to the repo of JSON files
+  -d OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
+                        Path to the transformed datasets
+```
+
+**Example:**
+
+```sh
+hityper preprocess -p ManyTypes4PyDataset/processed_projects_complete -d outputs
+```
+
+*This command transforms the json files in ManyTypes4Py datasets into the `groundtruth.json` and `detailed_groundtruth.json` files that required by the `hityper eval` command.*
+
+This command is to facilitate the researchers that use ManyTypes4Py dataset and want to evaluate HiTyper in it.
+
+If you want to run HiTyper in other datasets, please follow the same logic in `transformDataset` function of  `HiTyper/hityper/utils.py` to write a script.
+
 ## Experiment Results
 
 **Dataset:**
 
 The following results are evaluated using the [ManyTypes4Py](https://zenodo.org/record/4719447#.YjxcpBNBxb8) dataset. 
 
 Since the original dataset does not contain Python source files, to facilitate future research, we here also attached a [link](https://drive.google.com/file/d/1HdZyd3dKAUkiv2Nl0Zynp_YhrqU6HfMx/view?usp=sharing) for the Python source files HiTyper uses to infer types. Attached dataset is not identical with the original one because the original one contains some GitHub repos that do not allow open access or have been deleted.
@@ -236,55 +283,17 @@
 
 You can use the following command to reproduce the above results:
 
 ```sh
 hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json 
 ```
 
-**Using Type4Py's top 1 predictions as recommendations:**
-
-| Category           | Exact Match | Match to Parametric | Partial Match |
-| ------------------ | ----------- | ------------------- | ------------- |
-| Simple Types       | 67.20%      | 68.00%              | 69.80%        |
-| Generic Types      | 56.37%      | 71.05%              | 72.54%        |
-| User-defined Types | 40.42%      | 40.42%              | 43.82%        |
-| Arguments          | 22.36%      | 23.67%              | 27.56%        |
-| Return Values      | 59.11%      | 64.98%              | 69.30%        |
-| Local Variables    | 64.47%      | 68.78%              | 69.72%        |
+We do not show the performance of HiTyper integrating different DL models here since there are many factors impacting the performance of DL models such as datasets, hyper-parameters, etc. Please align the performance by yourself before utilizing recommendations from DL models.
 
-You can use the following command to reproduce the above results:
-
-```sh
-hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json -t -n 1
-```
-
-**Using Type4Py's top 10 predictions as recommendations:**
-
-| Category           | Exact Match | Match to Parametric | Partial Match |
-| ------------------ | ----------- | ------------------- | ------------- |
-| Simple Types       | 68.94%      | 69.64%              | 71.23%        |
-| Generic Types      | 57.29%      | 72.31%              | 73.68%        |
-| User-defined Types | 40.43%      | 40.43%              | 43.67%        |
-| Arguments          | 25.90%      | 27.30%              | 30.64%        |
-| Return Values      | 59.35%      | 65.25%              | 69.54%        |
-| Local Variables    | 65.21%      | 69.53%              | 70.37%        |
-
-You can use the following command to reproduce the above results:
-
-```sh
-hityper eval -g ManyTypes4Py_gts_test_verified.json -c ManyTypes4Py_gts_test_verified_detailed.json -u ManyTypes4Py_test_usertypes.json -t -n 10
-```
-
-The improvement brought by Type4Py currently is not very significant because:
-
-1) Type4Py cannot give recommendations for many hot types given by HiTyper
-
-2) Type4Py maintains low performance on predicting "rare types", which are mostly user-defined types
-
-We are currently working on building a DL model that's more suitable for HiTyper. Stay tuned!
+What's more, we are currently working on building a DL model that's more suitable for HiTyper. Stay tuned!
 
 **Other datasets:**
 
 If you want to evaluate HiTyper on other datasets, please generate files with the same format with `ManyTypes4Py_gts_test_verified.json`, `ManyTypes4Py_gts_test_verified_detailed.json`, or you can modify the code in `__main__.py`. To check a type's category, you can use `hityper.typeobject.TypeObject.checkType()`.
 
 In any case, you must also prepare the source files for static analysis.
 
@@ -300,25 +309,30 @@
 - Add supports for stub files
 
 ## Cite Us
 
 If you use HiTyper in your research, please cite us:
 
 ```latex
-@article{peng2022hityper,
-  author    = {Yun Peng and Cuiyun Gao and Zongjie Li and Bowei Gao and David Lo and Qirun Zhang and Michael R. Lyu},
-  title     = {Static Inference Meets Deep Learning: A Hybrid Type Inference Approach for Python},
-  journal   = {CoRR},
-  volume    = {abs/2105.03595},
-  year      = {2022},
-  url       = {https://arxiv.org/abs/2105.03595}
+@inproceedings{peng22hityper,
+author = {Peng, Yun and Gao, Cuiyun and Li, Zongjie and Gao, Bowei and Lo, David and Zhang, Qirun and Lyu, Michael},
+title = {Static Inference Meets Deep Learning: A Hybrid Type Inference Approach for Python},
+year = {2022},
+isbn = {9781450392211},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3510003.3510038},
+doi = {10.1145/3510003.3510038},
+booktitle = {Proceedings of the 44th International Conference on Software Engineering},
+pages = {2019–2030},
+numpages = {12},
+location = {Pittsburgh, Pennsylvania},
+series = {ICSE '22}
 }
 ```
 
 ## Contact
 
 We actively maintain this project and welcome contributions. 
 
 If you have any question, please contact research@yunpeng.work.
 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hityper-1.0.2/setup.py` & `hityper-1.0.3/setup.py`

 * *Files identical despite different names*

