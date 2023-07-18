# Comparing `tmp/lesscode_tag-0.0.6.tar.gz` & `tmp/lesscode_tag-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tag-0.0.6.tar", last modified: Wed Jul 12 06:14:23 2023, max compression
+gzip compressed data, was "dist/lesscode_tag-0.0.7.tar", last modified: Tue Jul 18 07:20:13 2023, max compression
```

## Comparing `lesscode_tag-0.0.6.tar` & `lesscode_tag-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/
--rw-r--r--   0 zhengy     (501) staff       (20)      379 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/PKG-INFO
--rw-r--r--   0 zhengy     (501) staff       (20)       52 2023-05-25 10:25:23.000000 lesscode_tag-0.0.6/README.md
-drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/lesscode_tag/
--rw-r--r--   0 zhengy     (501) staff       (20)        0 2023-05-25 10:25:23.000000 lesscode_tag-0.0.6/lesscode_tag/__init__.py
--rw-r--r--   0 zhengy     (501) staff       (20)     1807 2023-05-25 10:25:23.000000 lesscode_tag-0.0.6/lesscode_tag/aes.py
--rw-r--r--   0 zhengy     (501) staff       (20)     9164 2023-07-12 06:13:53.000000 lesscode_tag-0.0.6/lesscode_tag/business.py
--rw-r--r--   0 zhengy     (501) staff       (20)     9603 2023-05-25 10:25:23.000000 lesscode_tag-0.0.6/lesscode_tag/es_util.py
--rw-r--r--   0 zhengy     (501) staff       (20)       22 2023-07-12 06:13:53.000000 lesscode_tag-0.0.6/lesscode_tag/version.py
-drwxr-xr-x   0 zhengy     (501) staff       (20)        0 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/lesscode_tag.egg-info/
--rw-r--r--   0 zhengy     (501) staff       (20)      379 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/lesscode_tag.egg-info/PKG-INFO
--rw-r--r--   0 zhengy     (501) staff       (20)      280 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/lesscode_tag.egg-info/SOURCES.txt
--rw-r--r--   0 zhengy     (501) staff       (20)        1 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/lesscode_tag.egg-info/dependency_links.txt
--rw-r--r--   0 zhengy     (501) staff       (20)       13 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/lesscode_tag.egg-info/top_level.txt
--rw-r--r--   0 zhengy     (501) staff       (20)       38 2023-07-12 06:14:23.000000 lesscode_tag-0.0.6/setup.cfg
--rw-r--r--   0 zhengy     (501) staff       (20)     1273 2023-05-25 10:25:23.000000 lesscode_tag-0.0.6/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.7/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.7/lesscode_tag/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     9134 2023-07-18 07:14:17.000000 lesscode_tag-0.0.7/lesscode_tag/business.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-18 07:16:53.000000 lesscode_tag-0.0.7/lesscode_tag/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      271 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag.egg-info/requires.txt
+-rw-r--r--   0 baai       (501) staff       (20)       13 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/lesscode_tag.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-18 07:20:13.000000 lesscode_tag-0.0.7/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1299 2023-07-18 07:15:14.000000 lesscode_tag-0.0.7/setup.py
```

### Comparing `lesscode_tag-0.0.6/lesscode_tag/business.py` & `lesscode_tag-0.0.7/lesscode_tag/business.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lesscode_tag.es_util import es_condition_by_terms, es_condition_by_wildcard
+from lesscode_utils.es_utils import es_condition_by_terms, es_condition_by_wildcard
 
 
 def get_single_tag_condition(tag):
     should = []
     if tag == "省级专精特新":
         should.append({"bool": {"must": [{"terms": {"tags.diy_tag": ["省级专精特新企业"]}},
                                          {"bool": {
@@ -105,15 +105,14 @@
             if tag in ["独角兽"]:
                 es_condition_by_wildcard(bool_should_list, "tags.rank_tag.rank_name", tag)
             if tag in ["科技型中小企业"]:
                 es_condition_by_terms(bool_should_list, "tags.certification.certification_name", [tag])
             if tag in ["规上企业"]:
                 es_condition_by_terms(bool_should_list, "tags.nonpublic_tag", [tag])
     bool_should_more_list.append(bool_should_list)
-    return bool_should_more_list
 
 
 def parse_special_tag_new(tags, tags_param_list=None):
     """新版产业通 特色标签 解析，临时用等数据组将标签添加到diy_tag修改此方法"""
     result = []
     for tag in tags.get("market_tag", []):
         if tag.get("status", "") == "已上市" and tag.get("block", "") in ["主板上市", "科创板上市", "创业板上市", "北交所"]:
```

### Comparing `lesscode_tag-0.0.6/setup.py` & `lesscode_tag-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     platforms='python',
     install_requires=[
         # "pycryptodomex==3.17"
+        "lesscode_utils>=0.0.1"
     ]
 
 )
 
 """
 1、打包流程
 打包过程中也可以多增加一些额外的操作，减少上传中的错误
@@ -42,10 +43,10 @@
 twine check dist/*
 
 # 上传pypi
 twine upload dist/*
 twine upload dist/* -u yuyc -p yu230225
 twine upload dist/* --repository-url https://pypi.chanyeos.com/ -u admin -p shangqi
 # 安装最新的版本测试
-pip install -U lesscode_charts -i https://pypi.org/simple
-pip install -U lesscode_charts -i https://pypi.chanyeos.com/simple
+pip install -U lesscode_tag -i https://pypi.org/simple
+pip install -U lesscode_tag -i https://pypi.chanyeos.com/simple
 """
```

