# Comparing `tmp/pke_zh-0.2.3.tar.gz` & `tmp/pke_zh-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pke_zh-0.2.3.tar", last modified: Wed Feb  1 13:30:37 2023, max compression
+gzip compressed data, was "pke_zh-0.2.5.tar", last modified: Tue Jul 18 12:59:01 2023, max compression
```

## Comparing `pke_zh-0.2.3.tar` & `pke_zh-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,41 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.940433 pke_zh-0.2.3/
--rw-r--r--   0 xuming     (501) staff       (20)    10256 2023-02-01 13:30:37.939667 pke_zh-0.2.3/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     7476 2023-02-01 13:27:46.000000 pke_zh-0.2.3/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.827169 pke_zh-0.2.3/pke_zh/
--rw-r--r--   0 xuming     (501) staff       (20)      290 2023-01-31 13:43:55.000000 pke_zh-0.2.3/pke_zh/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    17016 2023-02-01 07:01:17.000000 pke_zh-0.2.3/pke_zh/base.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.909555 pke_zh-0.2.3/pke_zh/data/
--rw-r--r--   0 xuming     (501) staff       (20)    14008 2023-01-31 08:16:43.000000 pke_zh-0.2.3/pke_zh/data/common_char_set.txt
--rw-r--r--   0 xuming     (501) staff       (20)  3989296 2023-02-01 10:06:03.000000 pke_zh-0.2.3/pke_zh/data/entropy_word_score.json
--rw-r--r--   0 xuming     (501) staff       (20)   163162 2023-01-31 08:16:43.000000 pke_zh-0.2.3/pke_zh/data/person_name.txt
--rw-r--r--   0 xuming     (501) staff       (20)   640666 2023-01-31 08:16:43.000000 pke_zh-0.2.3/pke_zh/data/place_name.txt
--rw-r--r--   0 xuming     (501) staff       (20) 12575598 2023-02-01 08:50:51.000000 pke_zh-0.2.3/pke_zh/data/pmi_word_score.json
--rw-r--r--   0 xuming     (501) staff       (20)     7472 2023-01-31 10:10:31.000000 pke_zh-0.2.3/pke_zh/data/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     3881 2023-01-31 09:29:16.000000 pke_zh-0.2.3/pke_zh/data_structures.py
--rw-r--r--   0 xuming     (501) staff       (20)     5069 2023-01-31 10:10:30.000000 pke_zh-0.2.3/pke_zh/readers.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.914983 pke_zh-0.2.3/pke_zh/supervised/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-01-31 08:16:43.000000 pke_zh-0.2.3/pke_zh/supervised/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    22950 2023-02-01 12:07:25.000000 pke_zh-0.2.3/pke_zh/supervised/wordrank.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.930309 pke_zh-0.2.3/pke_zh/unsupervised/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-01-31 10:10:31.000000 pke_zh-0.2.3/pke_zh/unsupervised/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    12755 2023-02-01 11:51:01.000000 pke_zh-0.2.3/pke_zh/unsupervised/keybert.py
--rw-r--r--   0 xuming     (501) staff       (20)     7648 2023-01-31 12:31:14.000000 pke_zh-0.2.3/pke_zh/unsupervised/multipartiterank.py
--rw-r--r--   0 xuming     (501) staff       (20)     6429 2023-01-31 10:10:30.000000 pke_zh-0.2.3/pke_zh/unsupervised/positionrank.py
--rw-r--r--   0 xuming     (501) staff       (20)     4224 2023-01-31 10:10:31.000000 pke_zh-0.2.3/pke_zh/unsupervised/singlerank.py
--rw-r--r--   0 xuming     (501) staff       (20)     6471 2023-02-01 13:23:01.000000 pke_zh-0.2.3/pke_zh/unsupervised/textrank.py
--rw-r--r--   0 xuming     (501) staff       (20)     2568 2023-01-31 12:31:14.000000 pke_zh-0.2.3/pke_zh/unsupervised/tfidf.py
--rw-r--r--   0 xuming     (501) staff       (20)     7767 2023-01-31 12:31:14.000000 pke_zh-0.2.3/pke_zh/unsupervised/topicrank.py
--rw-r--r--   0 xuming     (501) staff       (20)    16013 2023-02-01 07:47:42.000000 pke_zh-0.2.3/pke_zh/unsupervised/yake.py
--rw-r--r--   0 xuming     (501) staff       (20)     6184 2023-02-01 06:34:09.000000 pke_zh-0.2.3/pke_zh/unsupervised/yake_zh.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.936997 pke_zh-0.2.3/pke_zh/utils/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2023-01-31 08:16:43.000000 pke_zh-0.2.3/pke_zh/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    13624 2023-01-31 08:16:43.000000 pke_zh-0.2.3/pke_zh/utils/file_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     1077 2023-02-01 08:39:29.000000 pke_zh-0.2.3/pke_zh/utils/io_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     1760 2023-01-31 10:10:31.000000 pke_zh-0.2.3/pke_zh/utils/text_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     2247 2023-01-31 10:10:30.000000 pke_zh-0.2.3/pke_zh/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)      109 2023-02-01 13:29:45.000000 pke_zh-0.2.3/pke_zh/version.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-02-01 13:30:37.831752 pke_zh-0.2.3/pke_zh.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    10256 2023-02-01 13:30:37.000000 pke_zh-0.2.3/pke_zh.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      989 2023-02-01 13:30:37.000000 pke_zh-0.2.3/pke_zh.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-02-01 13:30:37.000000 pke_zh-0.2.3/pke_zh.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-02-01 12:17:32.000000 pke_zh-0.2.3/pke_zh.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       81 2023-02-01 13:30:37.000000 pke_zh-0.2.3/pke_zh.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        7 2023-02-01 13:30:37.000000 pke_zh-0.2.3/pke_zh.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)       38 2023-02-01 13:30:37.940643 pke_zh-0.2.3/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1935 2023-02-01 12:08:15.000000 pke_zh-0.2.3/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 12:59:01.874220 pke_zh-0.2.5/
+-rw-r--r--   0 xuming     (501) staff       (20)    12536 2023-07-18 12:59:01.873562 pke_zh-0.2.5/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     9799 2023-07-18 11:56:32.000000 pke_zh-0.2.5/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 12:59:01.712367 pke_zh-0.2.5/pke_zh/
+-rw-r--r--   0 xuming     (501) staff       (20)      500 2023-07-18 12:02:34.000000 pke_zh-0.2.5/pke_zh/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17246 2023-02-13 07:56:38.000000 pke_zh-0.2.5/pke_zh/base.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 12:59:01.867036 pke_zh-0.2.5/pke_zh/data/
+-rw-r--r--   0 xuming     (501) staff       (20)    14008 2023-01-31 08:16:43.000000 pke_zh-0.2.5/pke_zh/data/common_char_set.txt
+-rw-r--r--   0 xuming     (501) staff       (20)  3989296 2023-02-01 10:06:03.000000 pke_zh-0.2.5/pke_zh/data/entropy_word_score.json
+-rw-r--r--   0 xuming     (501) staff       (20)   163162 2023-01-31 08:16:43.000000 pke_zh-0.2.5/pke_zh/data/person_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20)   640666 2023-01-31 08:16:43.000000 pke_zh-0.2.5/pke_zh/data/place_name.txt
+-rw-r--r--   0 xuming     (501) staff       (20) 12575598 2023-02-01 08:50:51.000000 pke_zh-0.2.5/pke_zh/data/pmi_word_score.json
+-rw-r--r--   0 xuming     (501) staff       (20)     7472 2023-01-31 10:10:31.000000 pke_zh-0.2.5/pke_zh/data/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     3909 2023-02-13 07:27:59.000000 pke_zh-0.2.5/pke_zh/data_structures.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12867 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/keybert.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7787 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/multipartiterank.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6579 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/positionrank.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5345 2023-02-13 07:27:59.000000 pke_zh-0.2.5/pke_zh/readers.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4374 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/singlerank.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9772 2023-07-18 12:43:39.000000 pke_zh-0.2.5/pke_zh/textrank.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2721 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/tfidf.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7920 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/topicrank.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 12:59:01.871895 pke_zh-0.2.5/pke_zh/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2023-01-31 08:16:43.000000 pke_zh-0.2.5/pke_zh/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13624 2023-01-31 08:16:43.000000 pke_zh-0.2.5/pke_zh/utils/file_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1077 2023-02-01 08:39:29.000000 pke_zh-0.2.5/pke_zh/utils/io_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3377 2023-02-02 08:16:24.000000 pke_zh-0.2.5/pke_zh/utils/text_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2247 2023-01-31 10:10:30.000000 pke_zh-0.2.5/pke_zh/utils/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)      109 2023-07-18 11:55:57.000000 pke_zh-0.2.5/pke_zh/version.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23748 2023-07-18 12:34:04.000000 pke_zh-0.2.5/pke_zh/wordrank.py
+-rw-r--r--   0 xuming     (501) staff       (20)    16181 2023-07-18 12:37:47.000000 pke_zh-0.2.5/pke_zh/yake.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6351 2023-07-18 12:49:37.000000 pke_zh-0.2.5/pke_zh/yake_zh.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 12:59:01.716850 pke_zh-0.2.5/pke_zh.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    12536 2023-07-18 12:59:01.000000 pke_zh-0.2.5/pke_zh.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      799 2023-07-18 12:59:01.000000 pke_zh-0.2.5/pke_zh.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-18 12:59:01.000000 pke_zh-0.2.5/pke_zh.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-02-01 12:17:32.000000 pke_zh-0.2.5/pke_zh.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       81 2023-07-18 12:59:01.000000 pke_zh-0.2.5/pke_zh.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        7 2023-07-18 12:59:01.000000 pke_zh-0.2.5/pke_zh.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-07-18 12:59:01.874467 pke_zh-0.2.5/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1689 2023-07-18 11:55:57.000000 pke_zh-0.2.5/setup.py
```

### Comparing `pke_zh-0.2.3/PKG-INFO` & `pke_zh-0.2.5/pke_zh.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: pke_zh
-Version: 0.2.3
+Name: pke-zh
+Version: 0.2.5
 Summary: pke_zh, context-aware bag-of-words term weights for query and document.
 Home-page: https://github.com/shibing624/pke_zh
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: # pke_zh
         [![PyPI version](https://badge.fury.io/py/pke_zh.svg)](https://badge.fury.io/py/pke_zh)
-        [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
+        [![Downloads](https://pepy.tech/badge/pke_zh)](https://pepy.tech/project/pke_zh)
         [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
-        PKE_zh, Python Keyphrase Extraction for ZH(chinese).
+        PKE_zh, Python Keyphrase Extraction for zh(chinese).
         
-        **pke_zh**实现了多种中文关键词提取算法，包括有监督的WordRank、无监督的TextRank, TfIdf, KeyBert, PositionRank, TopicRank等，扩展性强，开箱即用。
+        **pke_zh**实现了多种中文关键词提取算法，包括有监督的WordRank，无监督的TextRank、TfIdf、KeyBert、PositionRank、TopicRank等，扩展性强，开箱即用。
         
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
@@ -29,84 +29,92 @@
         - [Reference](#reference)
         
         # Feature
         
         如何提取query或者文档的关键词？
         
         
-        ### 有监督方法
-        #### 特征工程的解决思路
-        1. 实现时采用模型打分方法，以搜索query为原始语料，人工标注句子中各词重要度
-        
-        > 重要度共分4级：
-        > * Super important：主要包括POI核心词，比如“方特、欢乐谷”
-        > * Required：包括行政区词、品类词等，比如“北京 温泉”中“北京”和“温泉”都很重要
-        > * Important：包括品类词、门票等，比如“顺景 温泉”中“温泉”相对没有那么重要，用户搜“顺景”大部分都是温泉的需求
-        > * Unimportant：包括语气词、代词、泛需求词、停用词等
+        ## 有监督方法
+        ### 特征工程的解决思路
+        把关键词提取任务转化为分类任务，对输入query句子分词并提取多种特征，再把特征喂给机器学习模型，模型区分出各词的重要性得分，这样挑出topK个词作为关键词。
         
-        上例中可见“温泉”在不同的query中重要度是不同的。
-        
-        **特征方法**
+        #### 特征工程
         
         * 文本特征：包括Query长度、Term长度，Term在Query中的偏移量，term词性、长度信息、term数目、位置信息、句法依存tag、是否数字、是否英文、是否停用词、是否专名实体、是否重要行业词、embedding模长、删词差异度、以及短语生成树得到term权重等
-        * 统计特征：包括PMI、IDF、textrank值、前后词互信息、左右邻熵、独立检索占比（term单独作为query的qv/所有包含term的query的qv和）、统计概率、idf变种iqf
+        * 统计特征：包括PMI、IDF、TextRank值、前后词互信息、左右邻熵、独立检索占比（term单独作为query的qv/所有包含term的query的qv和）、统计概率、idf变种iqf
         * 语言模型特征：整个query的语言模型概率 / 去掉该Term后的Query的语言模型概率
         
-        2. 模型方面采用树模型（XGBoost等）进行训练，得到权重分类模型后在线上预测
-        ![term-weighting](./docs/gbdt.png)
         
-        #### 深度模型的解决思路
-        * 利用深度学习模型来学习term重要性，比如通过训练基于BiLSTM+Attention的query意图分类模型
-        * 基于Seq2Seq/Transformer训练的query翻译改写模型得到的attention权重副产物再结合其他策略或作为上述分类回归模型的特征也可以用于衡量term的重要性
-        * 利用BERT模型训练端到端的词分级模型，类似序列标注模型，后接CRF判定词重要性权重输出
-        
-        
-        **深度模型**
-        
-        * BERT CLS + softmax 
-        * Seq2Seq 文本摘要模型
-        
-        ### 无监督方法
-        - [x] TextRank
-        - [x] TfIdf
-        - [x] SingleRank
-        - [x] PositionRank
-        - [x] TopicRank
-        - [x] MultipartiteRank
-        - [x] Yake
-        - [x] KeyBert
+        训练样本形如：
+        ```shell
+        邪御天娇 免费 阅读,3 1 1
+        ```
+        
+        **重要度label**共分4级：
+        - Super important：3级，主要包括POI核心词，比如“方特、欢乐谷”
+        - Required：2级，包括行政区词、品类词等，比如“北京 温泉”中“北京”和“温泉”都很重要
+        - Important：1级，包括品类词、门票等，比如“顺景 温泉”中“温泉”相对没有那么重要，用户搜“顺景”大部分都是温泉的需求
+        - Unimportant：0级，包括语气词、代词、泛需求词、停用词等
         
+        上例中可见“温泉”在不同的query中重要度是不同的。
+        
+        分类模型可以是GBDT、LR、SVM、Xgboost等，这里以GBDT为例，GBDT模型（WordRank）的输入是特征向量，输出是重要度label。
+        
+        ![term-weighting](./docs/gbdt.png)
+        
+        ### 深度模型的解决思路
+        - 思路一：本质依然是把关键词提取任务转化为词重要度分类任务，利用深度模型学习term重要度，取代人工提取特征，模型端到端预测词重要度label，按重要度排序后挑出topK个词作为关键词。深度模型有TextCNN、Fasttext、Transformer、BERT等，适用于分类任务的模型都行。分类任务实现参考：https://github.com/shibing624/pytextclassifier
+        - 思路二：用Seq2Seq生成模型，输入query，输出关键词或者摘要，生成模型可以是T5、Bart、Seq2Seq等，生成任务实现参考：https://github.com/shibing624/textgen
+        
+        ## 无监督方法
+        - 统计算法
+        - [x] TFIDF，是很强的baseline，有较强普适性，基本能应付大部分关键词抽取场景，简单有效，速度很快，效果一般
+        - [x] YAKE，人工总结规则的方法，不依赖外部语料，从单文档提取关键词，速度很快，效果差
+        - 图算法
+        - [x] TextRank，简单套用PageRank思想到关键词提取的方法，效果不比TFIDF强，而且涉及网络构建和随机游走迭代，速度慢，效果一般
+        - [x] SingleRank，类似TextRank，是PageRank的变体，可以提取出关键短语，速度快，效果一般
+        - [x] TopicRank，基于主题模型的关键词提取算法，考虑了文档中词语的语义关系，可以提取出与文档主题相关的关键词，速度慢，效果一般
+        - [x] MultipartiteRank，一种基于多元关系的关键词提取算法，在TopicRank的基础上，考虑了词语的语义关系和词语位置，速度慢，效果一般
+        - [x] PositionRank，是基于PageRank的图关系计算词权重，考虑了词位置和词频，速度一般，效果好
+        - 语义模型
+        - [x] KeyBERT，利用了预训练语言模型的能力来提取关键词，速度很慢，效果最好
+        
+        **模型选型**
+        - 要求速度快，选择TFIDF、YAKE、PositionRank
+        - 要求效果好，选择KeyBERT
         
+        无监督算法介绍见文章[中文关键词提取算法](http://t.csdn.cn/6NO24)
         
         # Install
         * From pip:
-        ```shell
-        pip3 install -U pke_zh
+        ```zsh
+        pip install -U pke_zh
         ```
+        
         * From source：
-        ```shell
+        ```zsh
         git clone https://github.com/shibing624/pke_zh.git
         cd pke_zh
-        python3 setup.py install
+        python setup.py install
         ```
         
         ### 依赖数据
-        * 千兆中文文本训练的语言模型[zh_giga.no_cna_cmn.prune01244.klm(2.8G)](https://deepspeech.bj.bcebos.com/zh_lm/zh_giga.no_cna_cmn.prune01244.klm)，模型由pycorrector库自动下载于：~/.pycorrector/datasets/zh_giga.no_cna_cmn.prune01244.klm 。
-        * 中文文本匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) ，模型由transformers库自动下载于：~/.cache/huggingface/transformers/ 下。
+        * 千兆中文文本训练的语言模型[zh_giga.no_cna_cmn.prune01244.klm(2.8G)](https://deepspeech.bj.bcebos.com/zh_lm/zh_giga.no_cna_cmn.prune01244.klm)，模型由pycorrector库自动下载于 `~/.pycorrector/datasets/zh_giga.no_cna_cmn.prune01244.klm` 。
+        * 中文文本匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) ，模型由transformers库自动下载于 `~/.cache/huggingface/transformers/` 下。
         
         # Usage
         
         ## 有监督关键词提取
         
-        直接调用训练好的WordRank模型，模型自动下载本地`~/.cache/pke_zh/wordrank_model.pkl`
+        直接调用训练好的WordRank模型，模型自动下载于 `~/.cache/pke_zh/wordrank_model.pkl` 。
         
         example: [examples/keyphrase_extraction_demo.py](examples/keyphrase_extraction_demo.py)
         
         ```python
-        from pke_zh.supervised.wordrank import WordRank
+        from pke_zh.wordrank import WordRank
         m = WordRank()
         print(m.extract("哪里下载电视剧周恩来？"))
         ```
         
         output:
         ```shell
         [('电视剧', 3), ('周恩来', 3), ('下载', 2), ('哪里', 1), ('？', 0)]
@@ -115,28 +123,28 @@
         
         ### 基于自有数据训练模型
         
         训练example: [examples/train_supervised_wordrank_demo.py](examples/train_supervised_wordrank_demo.py)
         
         
         ## 无监督关键词提取
-        支持TextRank、TfIdf、KeyBert等关键词提取算法。
+        支持TextRank、TfIdf、PositionRank、KeyBert等关键词提取算法。
         
         example: [examples/unsupervised_demo.py](examples/unsupervised_demo.py)
         
         
         ```python
-        from pke_zh.unsupervised.textrank import TextRank
-        from pke_zh.unsupervised.tfidf import TfIdf
-        from pke_zh.unsupervised.singlerank import SingleRank
-        from pke_zh.unsupervised.positionrank import PositionRank
-        from pke_zh.unsupervised.topicrank import TopicRank
-        from pke_zh.unsupervised.multipartiterank import MultipartiteRank
-        from pke_zh.unsupervised.yake import Yake
-        from pke_zh.unsupervised.keybert import KeyBert
+        from pke_zh.textrank import TextRank
+        from pke_zh.tfidf import TfIdf
+        from pke_zh.singlerank import SingleRank
+        from pke_zh.positionrank import PositionRank
+        from pke_zh.topicrank import TopicRank
+        from pke_zh.multipartiterank import MultipartiteRank
+        from pke_zh.yake import Yake
+        from pke_zh.keybert import KeyBert
         
         q = '哪里下载电视剧周恩来？'
         TextRank_m = TextRank()
         TfIdf_m = TfIdf()
         PositionRank_m = PositionRank()
         KeyBert_m = KeyBert()
         
@@ -157,14 +165,32 @@
         ```shell
         TextRank: [('电视剧', 1.00000002)]
         TfIdf: [('哪里下载', 1.328307500322222), ('下载电视剧', 1.328307500322222), ('电视剧周恩来', 1.328307500322222)]
         PositionRank_m: [('电视剧', 1.0)]
         KeyBert_m: [('电视剧', 0.47165293)]
         ```
         
+        ### 无监督关键句提取（自动摘要）
+        支持TextRank摘要提取算法。
+        
+        example: [examples/keysentences_extraction_demo.py](examples/keysentences_extraction_demo.py)
+        
+        
+        ```python
+        from pke_zh.textrank import TextRank
+        
+        m = TextRank()
+        r = m.extract_sentences("较早进入中国市场的星巴克，是不少小资钟情的品牌。相比 在美国的平民形象，星巴克在中国就显得“高端”得多。用料并无差别的一杯中杯美式咖啡，在美国仅约合人民币12元，国内要卖21元，相当于贵了75%。  第一财经日报")
+        print(r)
+        ```
+        
+        output:
+        ```shell
+        [('相比在美国的平民形象', 0.13208935993025409), ('在美国仅约合人民币12元', 0.1320761453200497), ('星巴克在中国就显得“高端”得多', 0.12497451534612379), ('国内要卖21元', 0.11929080110899569) ...]
+        ```
         
         # Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我：加我*微信号：xuming624*, 备注：*姓名-公司名-NLP* 进NLP交流群。
         
@@ -221,16 +247,11 @@
 Platform: Unix
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `pke_zh-0.2.3/README.md` & `pke_zh-0.2.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # pke_zh
 [![PyPI version](https://badge.fury.io/py/pke_zh.svg)](https://badge.fury.io/py/pke_zh)
-[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
+[![Downloads](https://pepy.tech/badge/pke_zh)](https://pepy.tech/project/pke_zh)
 [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
-PKE_zh, Python Keyphrase Extraction for ZH(chinese).
+PKE_zh, Python Keyphrase Extraction for zh(chinese).
 
-**pke_zh**实现了多种中文关键词提取算法，包括有监督的WordRank、无监督的TextRank, TfIdf, KeyBert, PositionRank, TopicRank等，扩展性强，开箱即用。
+**pke_zh**实现了多种中文关键词提取算法，包括有监督的WordRank，无监督的TextRank、TfIdf、KeyBert、PositionRank、TopicRank等，扩展性强，开箱即用。
 
 
 **Guide**
 
 - [Feature](#Feature)
 - [Install](#install)
 - [Usage](#usage)
@@ -21,84 +21,92 @@
 - [Reference](#reference)
 
 # Feature
 
 如何提取query或者文档的关键词？
 
 
-### 有监督方法
-#### 特征工程的解决思路
-1. 实现时采用模型打分方法，以搜索query为原始语料，人工标注句子中各词重要度
-
-> 重要度共分4级：
-> * Super important：主要包括POI核心词，比如“方特、欢乐谷”
-> * Required：包括行政区词、品类词等，比如“北京 温泉”中“北京”和“温泉”都很重要
-> * Important：包括品类词、门票等，比如“顺景 温泉”中“温泉”相对没有那么重要，用户搜“顺景”大部分都是温泉的需求
-> * Unimportant：包括语气词、代词、泛需求词、停用词等
+## 有监督方法
+### 特征工程的解决思路
+把关键词提取任务转化为分类任务，对输入query句子分词并提取多种特征，再把特征喂给机器学习模型，模型区分出各词的重要性得分，这样挑出topK个词作为关键词。
 
-上例中可见“温泉”在不同的query中重要度是不同的。
-
-**特征方法**
+#### 特征工程
 
 * 文本特征：包括Query长度、Term长度，Term在Query中的偏移量，term词性、长度信息、term数目、位置信息、句法依存tag、是否数字、是否英文、是否停用词、是否专名实体、是否重要行业词、embedding模长、删词差异度、以及短语生成树得到term权重等
-* 统计特征：包括PMI、IDF、textrank值、前后词互信息、左右邻熵、独立检索占比（term单独作为query的qv/所有包含term的query的qv和）、统计概率、idf变种iqf
+* 统计特征：包括PMI、IDF、TextRank值、前后词互信息、左右邻熵、独立检索占比（term单独作为query的qv/所有包含term的query的qv和）、统计概率、idf变种iqf
 * 语言模型特征：整个query的语言模型概率 / 去掉该Term后的Query的语言模型概率
 
-2. 模型方面采用树模型（XGBoost等）进行训练，得到权重分类模型后在线上预测
-![term-weighting](./docs/gbdt.png)
 
-#### 深度模型的解决思路
-* 利用深度学习模型来学习term重要性，比如通过训练基于BiLSTM+Attention的query意图分类模型
-* 基于Seq2Seq/Transformer训练的query翻译改写模型得到的attention权重副产物再结合其他策略或作为上述分类回归模型的特征也可以用于衡量term的重要性
-* 利用BERT模型训练端到端的词分级模型，类似序列标注模型，后接CRF判定词重要性权重输出
-
-
-**深度模型**
-
-* BERT CLS + softmax 
-* Seq2Seq 文本摘要模型
-
-### 无监督方法
-- [x] TextRank
-- [x] TfIdf
-- [x] SingleRank
-- [x] PositionRank
-- [x] TopicRank
-- [x] MultipartiteRank
-- [x] Yake
-- [x] KeyBert
+训练样本形如：
+```shell
+邪御天娇 免费 阅读,3 1 1
+```
+
+**重要度label**共分4级：
+- Super important：3级，主要包括POI核心词，比如“方特、欢乐谷”
+- Required：2级，包括行政区词、品类词等，比如“北京 温泉”中“北京”和“温泉”都很重要
+- Important：1级，包括品类词、门票等，比如“顺景 温泉”中“温泉”相对没有那么重要，用户搜“顺景”大部分都是温泉的需求
+- Unimportant：0级，包括语气词、代词、泛需求词、停用词等
 
+上例中可见“温泉”在不同的query中重要度是不同的。
+
+分类模型可以是GBDT、LR、SVM、Xgboost等，这里以GBDT为例，GBDT模型（WordRank）的输入是特征向量，输出是重要度label。
+
+![term-weighting](./docs/gbdt.png)
+
+### 深度模型的解决思路
+- 思路一：本质依然是把关键词提取任务转化为词重要度分类任务，利用深度模型学习term重要度，取代人工提取特征，模型端到端预测词重要度label，按重要度排序后挑出topK个词作为关键词。深度模型有TextCNN、Fasttext、Transformer、BERT等，适用于分类任务的模型都行。分类任务实现参考：https://github.com/shibing624/pytextclassifier
+- 思路二：用Seq2Seq生成模型，输入query，输出关键词或者摘要，生成模型可以是T5、Bart、Seq2Seq等，生成任务实现参考：https://github.com/shibing624/textgen
+
+## 无监督方法
+- 统计算法
+- [x] TFIDF，是很强的baseline，有较强普适性，基本能应付大部分关键词抽取场景，简单有效，速度很快，效果一般
+- [x] YAKE，人工总结规则的方法，不依赖外部语料，从单文档提取关键词，速度很快，效果差
+- 图算法
+- [x] TextRank，简单套用PageRank思想到关键词提取的方法，效果不比TFIDF强，而且涉及网络构建和随机游走迭代，速度慢，效果一般
+- [x] SingleRank，类似TextRank，是PageRank的变体，可以提取出关键短语，速度快，效果一般
+- [x] TopicRank，基于主题模型的关键词提取算法，考虑了文档中词语的语义关系，可以提取出与文档主题相关的关键词，速度慢，效果一般
+- [x] MultipartiteRank，一种基于多元关系的关键词提取算法，在TopicRank的基础上，考虑了词语的语义关系和词语位置，速度慢，效果一般
+- [x] PositionRank，是基于PageRank的图关系计算词权重，考虑了词位置和词频，速度一般，效果好
+- 语义模型
+- [x] KeyBERT，利用了预训练语言模型的能力来提取关键词，速度很慢，效果最好
+
+**模型选型**
+- 要求速度快，选择TFIDF、YAKE、PositionRank
+- 要求效果好，选择KeyBERT
 
+无监督算法介绍见文章[中文关键词提取算法](http://t.csdn.cn/6NO24)
 
 # Install
 * From pip:
-```shell
-pip3 install -U pke_zh
+```zsh
+pip install -U pke_zh
 ```
+
 * From source：
-```shell
+```zsh
 git clone https://github.com/shibing624/pke_zh.git
 cd pke_zh
-python3 setup.py install
+python setup.py install
 ```
 
 ### 依赖数据
-* 千兆中文文本训练的语言模型[zh_giga.no_cna_cmn.prune01244.klm(2.8G)](https://deepspeech.bj.bcebos.com/zh_lm/zh_giga.no_cna_cmn.prune01244.klm)，模型由pycorrector库自动下载于：~/.pycorrector/datasets/zh_giga.no_cna_cmn.prune01244.klm 。
-* 中文文本匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) ，模型由transformers库自动下载于：~/.cache/huggingface/transformers/ 下。
+* 千兆中文文本训练的语言模型[zh_giga.no_cna_cmn.prune01244.klm(2.8G)](https://deepspeech.bj.bcebos.com/zh_lm/zh_giga.no_cna_cmn.prune01244.klm)，模型由pycorrector库自动下载于 `~/.pycorrector/datasets/zh_giga.no_cna_cmn.prune01244.klm` 。
+* 中文文本匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) ，模型由transformers库自动下载于 `~/.cache/huggingface/transformers/` 下。
 
 # Usage
 
 ## 有监督关键词提取
 
-直接调用训练好的WordRank模型，模型自动下载本地`~/.cache/pke_zh/wordrank_model.pkl`
+直接调用训练好的WordRank模型，模型自动下载于 `~/.cache/pke_zh/wordrank_model.pkl` 。
 
 example: [examples/keyphrase_extraction_demo.py](examples/keyphrase_extraction_demo.py)
 
 ```python
-from pke_zh.supervised.wordrank import WordRank
+from pke_zh.wordrank import WordRank
 m = WordRank()
 print(m.extract("哪里下载电视剧周恩来？"))
 ```
 
 output:
 ```shell
 [('电视剧', 3), ('周恩来', 3), ('下载', 2), ('哪里', 1), ('？', 0)]
@@ -107,28 +115,28 @@
 
 ### 基于自有数据训练模型
 
 训练example: [examples/train_supervised_wordrank_demo.py](examples/train_supervised_wordrank_demo.py)
 
 
 ## 无监督关键词提取
-支持TextRank、TfIdf、KeyBert等关键词提取算法。
+支持TextRank、TfIdf、PositionRank、KeyBert等关键词提取算法。
 
 example: [examples/unsupervised_demo.py](examples/unsupervised_demo.py)
 
 
 ```python
-from pke_zh.unsupervised.textrank import TextRank
-from pke_zh.unsupervised.tfidf import TfIdf
-from pke_zh.unsupervised.singlerank import SingleRank
-from pke_zh.unsupervised.positionrank import PositionRank
-from pke_zh.unsupervised.topicrank import TopicRank
-from pke_zh.unsupervised.multipartiterank import MultipartiteRank
-from pke_zh.unsupervised.yake import Yake
-from pke_zh.unsupervised.keybert import KeyBert
+from pke_zh.textrank import TextRank
+from pke_zh.tfidf import TfIdf
+from pke_zh.singlerank import SingleRank
+from pke_zh.positionrank import PositionRank
+from pke_zh.topicrank import TopicRank
+from pke_zh.multipartiterank import MultipartiteRank
+from pke_zh.yake import Yake
+from pke_zh.keybert import KeyBert
 
 q = '哪里下载电视剧周恩来？'
 TextRank_m = TextRank()
 TfIdf_m = TfIdf()
 PositionRank_m = PositionRank()
 KeyBert_m = KeyBert()
 
@@ -149,14 +157,32 @@
 ```shell
 TextRank: [('电视剧', 1.00000002)]
 TfIdf: [('哪里下载', 1.328307500322222), ('下载电视剧', 1.328307500322222), ('电视剧周恩来', 1.328307500322222)]
 PositionRank_m: [('电视剧', 1.0)]
 KeyBert_m: [('电视剧', 0.47165293)]
 ```
 
+### 无监督关键句提取（自动摘要）
+支持TextRank摘要提取算法。
+
+example: [examples/keysentences_extraction_demo.py](examples/keysentences_extraction_demo.py)
+
+
+```python
+from pke_zh.textrank import TextRank
+
+m = TextRank()
+r = m.extract_sentences("较早进入中国市场的星巴克，是不少小资钟情的品牌。相比 在美国的平民形象，星巴克在中国就显得“高端”得多。用料并无差别的一杯中杯美式咖啡，在美国仅约合人民币12元，国内要卖21元，相当于贵了75%。  第一财经日报")
+print(r)
+```
+
+output:
+```shell
+[('相比在美国的平民形象', 0.13208935993025409), ('在美国仅约合人民币12元', 0.1320761453200497), ('星巴克在中国就显得“高端”得多', 0.12497451534612379), ('国内要卖21元', 0.11929080110899569) ...]
+```
 
 # Contact
 
 - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我：加我*微信号：xuming624*, 备注：*姓名-公司名-NLP* 进NLP交流群。
```

### Comparing `pke_zh-0.2.3/pke_zh/base.py` & `pke_zh-0.2.5/pke_zh/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,23 @@
 
         self.stoplist = list(load_stopwords(stopwords_path)) if stopwords_path and os.path.exists(stopwords_path) \
             else list(load_stopwords(default_stopwords_path))
         """List of stopwords."""
 
         self.valid_pos = {'n', 'a'} if valid_pos is None else valid_pos
 
-        punctuation_expand = ['/', ',', '$', '%', '^', '*', '(', '+', '"', "'", ']', '+', '|', '[', '+', '——', '！',
-                              '，', '、', '~', '@', '#', '￥', '%', '&', '*', '（', '）', '：', '；', '《', '）', '《',
-                              '》', '“', '”', '(', ')', '»', '〔', '〕', '-']
+        punctuation_expand = [
+            '/', ',', '$', '%', '^', '*', '(', '+', '"', "'", ']', '+', '|', '[', '+', '——', '！',
+            '，', '、', '~', '@', '#', '￥', '%', '&', '*', '（', '）', '：', '；', '《', '）', '《',
+            '》', '“', '”', '(', ')', '»', '〔', '〕', '-'
+        ]
         self.punctuations = list(punctuation) + punctuation_expand
 
+        self.sentence_delimiters = ['？', '?', '；', ';', '！', '!', '。', '……', '…', '\n', '，', ',']
+
         self.self_defined_keywords = []
         if self_defined_keyword_path is not None:
             words = open(self_defined_keyword_path, 'r', encoding='utf-8').readlines()
             words = [x.strip for x in words if x.strip()]
             words = sorted(words, key=lambda w: len(w), reverse=True)
             if len(words) > 10000:
                 logger.warning(
@@ -85,16 +89,16 @@
     def clear_cache(self):
         raise NotImplementedError
 
     def load_document(self, input, **kwargs):
         """Loads the content of a document/string/stream in a given language.
 
         :param input: str, input.
-        :param language: str, language of the input, defaults to 'en'.
-        :param encoding: str, encoding of the raw file.
+        :param language: str, language of the input, defaults to 'zh'.
+        :param encoding: str, encoding of the raw file, defaults to 'utf-8'.
         :param normalization: str, word normalization method, defaults to
             'stemming'. Other possible values are 'lemmatization' or 'None'
             for using word surface forms instead of stems/lemmas.
         """
         # get the language parameter
         language = kwargs.get('language', 'zh')
 
@@ -200,14 +204,15 @@
 
         :param n: int, the number of candidates, defaults to 10.
         :param redundancy_removal: bool, whether redundant keyphrases are
             filtered out from the n-best list, defaults to False.
         :param stemming: bool, whether to extract stems or surface forms
             (lowercased, first occurring form of candidate), default to
             False.
+        :return: list, the n-best candidates as (lexical form, weight) tuples.
         """
         # sort candidates by descending weight
         best = sorted(self.weights, key=self.weights.get, reverse=True)
 
         # remove redundant candidates
         if redundancy_removal:
             best = self.redundancy_removal_best(best, n)
@@ -408,15 +413,15 @@
                         list(self.candidates)])
         for k in list(self.candidates):
             if k in del_keys:
                 del self.candidates[k]
 
     def self_defined_keyword_matching(self):
         """
-
+        Match custom keywords
         :param docs: list of doc texts to be extracted
         :param keywords: self-defined keyword set
         :return:
         """
         result = []
         for w in self.self_defined_keywords:
             if w in self.raw_text:
```

### Comparing `pke_zh-0.2.3/pke_zh/data/common_char_set.txt` & `pke_zh-0.2.5/pke_zh/data/common_char_set.txt`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/data/entropy_word_score.json` & `pke_zh-0.2.5/pke_zh/data/entropy_word_score.json`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/data/person_name.txt` & `pke_zh-0.2.5/pke_zh/data/person_name.txt`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/data/place_name.txt` & `pke_zh-0.2.5/pke_zh/data/place_name.txt`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/data/pmi_word_score.json` & `pke_zh-0.2.5/pke_zh/data/pmi_word_score.json`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/data/stopwords.txt` & `pke_zh-0.2.5/pke_zh/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/data_structures.py` & `pke_zh-0.2.5/pke_zh/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         """ the Part-Of-Speech patterns of the candidate. """
 
         self.lexical_form = []
         """ the lexical form of the candidate. """
 
 
 def parse_sentence(sent_obj):
+    """Parse a sentence."""
     s = Sentence(words=sent_obj['words'])
 
     # add the POS
     s.pos = sent_obj['POS']
 
     # add the meta-information, for chinese, it's `char_offset`
     m_key = "char_offsets"
```

### Comparing `pke_zh-0.2.3/pke_zh/readers.py` & `pke_zh-0.2.5/pke_zh/readers.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,34 +45,43 @@
     """
     result = [t for tlist in tuple_list for t in tlist]
     return result
 
 
 def fetch_nested_list_elements(nested_list, idx):
     """
+    Fetch target elements from nested list
     :param nested_list: list of list, each list is a tuple
     :param idx: target index in a tuple
     :return: list of list, each list contains target elements
     """
     result = [[t[idx] for t in inner_list] for inner_list in nested_list]
     return result
 
 
 def reduce_charoffset(list_str):
+    """
+    Reduce char offset
+    :param list_str: list of string
+    """
     len_list = [len(x) for x in list_str]
     cur_sum = 0
     res = [0]
     for i in range(len(len_list) - 1):
         cur_sum += len_list[i]
         res.append(cur_sum)
     offset = [(x, x + len_list[i]) for i, x in enumerate(res)]
     return offset
 
 
 def cut_sent(para):
+    """
+    Split paragraph into sentences
+    :param para: paragraph
+    """
     para = re.sub('([。！？\?;；])([^”’])', r"\1\n\2", para)
     para = re.sub('(\.{6})([^”’])', r"\1\n\2", para)
     para = re.sub('(\…{2})([^”’])', r"\1\n\2", para)
     para = re.sub('([。！？；;\?][”’])([^，。！？\?])', r'\1\n\2', para)
     para = para.rstrip()
     paras = [p.strip() for p in para.split("\n") if p.strip()]
     return paras
@@ -108,20 +117,22 @@
                    'char_offsets': char_offsets[i],
                    'global_char_offsets': global_char_offsets,
                    'word_POS': pseg_results}
                   for i, ws in enumerate(words)]
         return result
 
     def sentence_pseg(self, sentences):
+        """Segment sentences into words and POS tags."""
         results = [[(s.word, s.flag) for s in pseg.cut(sent)] for sent in sentences]
         words = fetch_nested_list_elements(results, 0)
         postags = fetch_nested_list_elements(results, 1)
         return results, words, postags
 
     def clean(self, text):
+        """Clean text."""
         text = re.sub(r'img[_\d]+', '', text.strip())
         text = re.sub(r'_SEG_', '', text.strip())
         return text
 
 
 class Reader(object):
     def read(self, path):
@@ -136,15 +147,15 @@
 
         Args:
             language (str): language of text to process.
         """
 
         self.language = language
         if self.language != 'zh':
-            logger.warning('toolkit is created for zh language!')
+            logger.warning('toolkit is built for zh language')
         self.nlp = ChineseNLP()
 
     def read(self, text, **kwargs):
         """Read the input file and use spacy to pre-process.
 
         Args:
             text (str): raw text to pre-process.
```

### Comparing `pke_zh-0.2.3/pke_zh/supervised/wordrank.py` & `pke_zh-0.2.5/pke_zh/wordrank.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 from typing import Optional
 from copy import deepcopy
 import numpy as np
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.metrics import classification_report
 from sklearn.model_selection import train_test_split
 
-from pke_zh import USER_DATA_DIR
 from pke_zh.utils.io_utils import load_pkl, save_pkl, save_json, load_json
 from pke_zh.utils.text_utils import convert_to_unicode, is_number_string, is_alphabet_string, is_chinese_string
 from pke_zh.utils.tokenizer import word_segment
 from pke_zh.utils.file_utils import get_file
-from pke_zh.unsupervised.tfidf import TfIdf
-from pke_zh.unsupervised.textrank import TextRank
+from pke_zh.tfidf import TfIdf
+from pke_zh.textrank import TextRank
 
 pwd_path = os.path.abspath(os.path.dirname(__file__))
 
 # inner data file
-default_stopwords_path = os.path.join(pwd_path, '../data/stopwords.txt')
-person_name_path = os.path.join(pwd_path, '../data/person_name.txt')
-place_name_path = os.path.join(pwd_path, '../data/place_name.txt')
-common_char_path = os.path.join(pwd_path, '../data/common_char_set.txt')
-pmi_path = os.path.join(pwd_path, '../data/pmi_word_score.json')
-entropy_path = os.path.join(pwd_path, '../data/entropy_word_score.json')
-
+default_stopwords_path = os.path.join(pwd_path, 'data/stopwords.txt')
+person_name_path = os.path.join(pwd_path, 'data/person_name.txt')
+place_name_path = os.path.join(pwd_path, 'data/place_name.txt')
+common_char_path = os.path.join(pwd_path, 'data/common_char_set.txt')
+pmi_path = os.path.join(pwd_path, 'data/pmi_word_score.json')
+entropy_path = os.path.join(pwd_path, 'data/entropy_word_score.json')
+
+# user data dir used for supervised model
+USER_DATA_DIR = os.path.expanduser('~/.cache/pke_zh/')
+os.makedirs(USER_DATA_DIR, exist_ok=True)
 # word rank model path
 default_model_path = os.path.join(USER_DATA_DIR, 'wordrank_model.pkl')
 
 
 class AttrDict(dict):
     """Dict that can get attribute by dot"""
 
@@ -433,15 +435,16 @@
             place_name_path=place_name_path,
             common_char_path=common_char_path,
             segment_sep=' ',
             ngram=4,
             pmi_path=pmi_path,
             entropy_path=entropy_path,
     ):
-        """ init word rank model
+        """
+        Init word rank model
 
         Args:
             model_path (str): the path to load the model in pickle format,
                 default to "~/.cache/pke_zh/wordrank_model.pkl".
         """
         self.text_feature = TextFeature(
             stopwords_path=stopwords_path,
@@ -530,18 +533,24 @@
             ]
             feature = sent_feature + term_feature
             features.append(feature)
             terms.append(text.term)
         return features, terms
 
     def train(self, train_file, col_sep=',', is_word_segmented=True):
+        """
+        Train word rank model
+        :param train_file: train file path
+        :param col_sep: column separator
+        :param is_word_segmented: bool, is word segmented or not
+        """
         # 1.read train data
         contents, labels = self.data_reader(train_file, col_sep)
         logger.info('contents size:%s, labels size:%s' % (len(contents), len(labels)))
-
+        # 2.get feature
         features = []
         tags = []
         for content, label in zip(contents, labels):
             label_split = [int(i) for i in label.split(self.segment_sep)]
             content_split = content.split(self.segment_sep)
             if len(label_split) != len(content_split):
                 logger.warning('pass, content size not equal label size, %s %s' % (content, label))
@@ -565,14 +574,20 @@
         # 4.validation and evaluate
         logger.debug("evaluate model with validation data")
         self.evaluate(model, X_val, y_val)
         self.model = model
         return model
 
     def predict(self, query, is_word_segmented=False):
+        """
+        Predict query
+        :param query: input query
+        :param is_word_segmented: bool, is word segmented or not
+        :return: list, predict label
+        """
         logger.info('model predict')
         features, terms = self.get_feature(query, is_word_segmented=is_word_segmented)
         # predict classification model
         if self.model_path and os.path.exists(self.model_path):
             self.model = load_pkl(self.model_path)
             logger.debug('Loaded model: {}'.format(self.model_path))
         else:
@@ -581,14 +596,21 @@
         label_pred = self.model.predict(features)
         logger.info("words: %s" % terms)
         logger.info("predict label: %s" % label_pred)
         return label_pred
 
     @staticmethod
     def evaluate(model, test_data, test_label, pred_save_path=None):
+        """
+        Evaluate model
+        :param model: classification model
+        :param test_data: test data
+        :param test_label: test label
+        :param pred_save_path: predict result save path
+        """
         print('{0}, val mean acc:{1}'.format(model.__str__(), model.score(test_data, test_label)))
         # multi
         label_pred = model.predict(test_data)
         # precision_recall_curve: multiclass format is not supported
         print(classification_report(test_label, label_pred))
         if pred_save_path:
             with open(pred_save_path, 'w', encoding='utf-8') as f:
@@ -597,16 +619,19 @@
         return label_pred
 
     def extract(self, input_string, n_best=10):
         """
         Extract keywords from text
         :param input_string:
         :param n_best:
-        :return:
+        :return: list of keywords
         """
+        keyphrases = []
+        if not input_string:
+            return keyphrases
         term_weights = []
         text = convert_to_unicode(input_string)
         if len(text) == 1:
             term_scores = zip([text], [0.0])
         else:
             # get feature
             data_feature, terms = self.get_feature(text, is_word_segmented=False)
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/keybert.py` & `pke_zh-0.2.5/pke_zh/keybert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description:
 
 refer: https://maartengr.github.io/KeyBERT/guides/quickstart.html
 keybert关键词抽取，核心思想类似embedrank，
-    只是向量提取的度量方法使用keyBERT
+    只是句子向量提取的方法使用Sentence-BERT
 """
 
-from loguru import logger
 import itertools
+from typing import List
+
+import numpy as np
+from loguru import logger
 from sklearn.metrics.pairwise import cosine_similarity
 from text2vec import SentenceModel
-import numpy as np
-from typing import List
 
 from pke_zh.base import BaseKeywordExtractModel
 
 
-def max_sum_ranking(doc_embedding: np.ndarray,
-                    can_embeddings: np.ndarray,
-                    can_names: List[str],
-                    top_n: int,
-                    nr_candidates: int):
+def max_sum_ranking(
+        doc_embedding: np.ndarray,
+        can_embeddings: np.ndarray,
+        can_names: List[str],
+        top_n: int,
+        nr_candidates: int
+):
     """ Calculate Max Sum Distance for extraction of keywords
         We take the 2 x top_n most similar words/phrases to the document.
         Then, we take all top_n combinations from the 2 x top_n words and
         extract the combination that are the least similar to each other
         by cosine similarity.
         NOTE:
             This is O(n^2) and therefore not advised if you use a large top_n
@@ -36,25 +39,29 @@
             can_names: The selected candidate keywords/keyphrases
             top_n: 取top_n 个关键词
             nr_candidates: The number of candidates to consider, generaly set top_n *2
         Returns:
              List[Tuple[str, float]]: The selected keywords/keyphrases with their distances
         """
     # calculate distances and extract words
-    # print(doc_embedding)
+    if len(doc_embedding.shape) == 1:
+        doc_embedding = doc_embedding.reshape(1, -1)
+    if len(can_embeddings.shape) == 1:
+        can_embeddings = can_embeddings.reshape(1, -1)
+
     distances = cosine_similarity(doc_embedding, can_embeddings)
     distance_words = cosine_similarity(can_embeddings)
 
     # Get 2*top_n words as candidates based on cosine similarity
     can_idx = list(distances.argsort()[0][-nr_candidates:])
 
     can_name_filter = [can_names[i] for i in can_idx]
     cand_distance = distance_words[np.ix_(can_idx, can_idx)]
 
-    # Calculate the 候选词里的topn of words的组合， that are the least similar to each other
+    # Calculate the topn of words, that are the least similar to each other
     min_sim = 100000
     final_candidate = None
     # print(can_idx)
     for combination in itertools.combinations(range(len(can_idx)), top_n):
         sim = sum([cand_distance[i][j] for i in combination for j in combination if i != j])
         if sim < min_sim:
             final_candidate = combination
@@ -64,19 +71,21 @@
     if not final_candidate:
         final_candidate = can_idx
     for val in final_candidate:
         result.append((can_name_filter[val], distances[0][can_idx[val]]))
     return result
 
 
-def mmr_ranking(doc_embedding: np.ndarray,
-                can_embeddings: np.ndarray,
-                can_names: List[str],
-                top_n: int,
-                alpha: float = 0.5):
+def mmr_ranking(
+        doc_embedding: np.ndarray,
+        can_embeddings: np.ndarray,
+        can_names: List[str],
+        top_n: int,
+        alpha: float = 0.5
+):
     """ Calculate Maximal Marginal Relevance (MMR)
     between candidate keywords and the document.
     MMR considers the similarity of keywords/keyphrases with the
     document, along with the similarity of already selected
     keywords and keyphrases. This results in a selection of keywords
     that maximize their within diversity with respect to the document.
     Arguments:
@@ -114,19 +123,21 @@
     # return candia_name and score
     result = []
     for val in keywords_idx:
         result.append((can_names[val], doc_can_distances[val][0]))
     return result
 
 
-def mmr_norm_ranking(doc_embedding: np.ndarray,
-                     can_embeddings: np.ndarray,
-                     can_names: List[str],
-                     top_n: int,
-                     alpha: float = 0.5):
+def mmr_norm_ranking(
+        doc_embedding: np.ndarray,
+        can_embeddings: np.ndarray,
+        can_names: List[str],
+        top_n: int,
+        alpha: float = 0.5
+):
     """Rank candidates according to a query
 
     :param document: np.array, dense representation of document (query)
     :param candidates: np.array, dense representation of candidates
     :param l: float, ratio between distance to query or distance between
         chosen candidates
     Returns: a list of candidates rank
@@ -182,27 +193,27 @@
 
     return result
 
 
 class KeyBert(BaseKeywordExtractModel):
     def __init__(self, model='shibing624/text2vec-base-chinese'):
         """
-            原文支持若干种embedding 方法：SentenceModel、SentenceTransformers、Flair、Spacy、gensim
-            中文默认支持text2vec.SentenceModel model="shibing624/text2vec-base-chinese"模型，
-            英文可设置model="sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2"模型，
+        model:
+            支持若干种embedding 方法：SentenceModel、SentenceTransformers、Flair、Spacy、gensim
+            中文默认使用text2vec.SentenceModel model="shibing624/text2vec-base-chinese"模型，
+            英文可设置model="shibing624/text2vec-base-multilingual"模型，
             其他语言参考：sentence-transformers models:
                   * https://www.sbert.net/docs/pretrained_models.html
-            """
-        # param: model sentenceTransformers
+        """
         super(KeyBert, self).__init__()
         if isinstance(model, str):
             try:
                 self.model = SentenceModel(model)
             except Exception as e:
-                logger.error('wrong url for sentence model, change to default!')
+                logger.warning(f'wrong url for sentence model, change to default! {e}')
                 self.model = SentenceModel('shibing624/text2vec-base-chinese')
         elif isinstance(model, SentenceModel):
             self.model = model
         else:
             raise ValueError('model must be str or text2vec.SentenceModel')
         self.max_length = self.model.max_seq_length
 
@@ -268,15 +279,15 @@
         """
         # get doc's sentences
         doc_sents = self._doc_to_sent_list()
         doc_embed = self.model.encode(doc_sents)
         doc_embed = np.average(doc_embed, axis=0)  # 取平均
         doc_embed = np.expand_dims(doc_embed, axis=0)  # 增加一个维度
 
-        cand_name = list(self.candidates.keys())  # 记得是带空格的
+        cand_name = list(self.candidates.keys())
         cand_embed = self.model.encode(cand_name)
 
         if use_mmr:
             can_list = mmr_ranking(doc_embed, cand_embed, cand_name, top_n, alpha)
             self._weights_update(can_list)
         elif use_maxsum:
             can_list = max_sum_ranking(doc_embed, cand_embed, cand_name, top_n, nr_candidates)
@@ -294,15 +305,20 @@
         :param use_maxsum: 是否使用maxsum similarity for the selection of keywords
         :param use_mmr: Whether to use Maximal Marginal Relevance (MMR) for the selection of keywords/keyphrases
         :param alpha: mmr算法的超参数，if use_mmr is set True, default:0.5
         :param nr_candidates: The number of candidates to consider if use_maxsum is set to True
         :return: keywords list
         """
         # 1. load the content of the document.
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         self.load_document(input=input_file_or_string, language='zh', normalization=None)
         # 2. select sequences of nouns and adjectives as candidates.
         self.candidate_selection()
+        if not self.candidates:
+            return keyphrases
         # 3. weight the candidates using EmbedRank method
         self.candidate_weighting(use_maxsum, use_mmr, n_best, alpha, nr_candidates)
         # 4. get the 10-highest scored candidates as keyphrases
         keyphrases = self.get_n_best(n=n_best, redundancy_removal=True)
         return keyphrases
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/multipartiterank.py` & `pke_zh-0.2.5/pke_zh/multipartiterank.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from itertools import combinations
 
 import networkx as nx
 import numpy as np
 from scipy.cluster.hierarchy import linkage, fcluster
 from scipy.spatial.distance import pdist
 
-from pke_zh.unsupervised.topicrank import TopicRank
+from pke_zh.topicrank import TopicRank
 
 
 class MultipartiteRank(TopicRank):
     """Multipartite graph keyphrase extraction model."""
 
     def __init__(self, stopwords_path=None):
         """Redefining initializer for MultipartiteRank."""
@@ -192,25 +192,29 @@
             self.weight_adjustment(alpha)
 
         # compute the word scores using random walk
         self.weights = nx.pagerank_scipy(self.graph)
 
     def extract(self, input_file_or_string, n_best=10, pos=None, threshold=0.74):
         # 1. load document
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         self.load_document(input=input_file_or_string, language='zh')
 
         # 2. clear previous graph and topics if exists
         self.clear_cache()
 
         # 3. select the longest sequences of nouns and adjectives, that do
         # not contain punctuation marks or stopwords as candidates.
         if pos is None:
             pos = {'n', 'a'}
         self.candidate_selection(pos=pos)
-
+        if not self.candidates:
+            return keyphrases
         # 4. build the Multipartite graph and rank candidates using random walk,
         # alpha controls the weight adjustment mechanism, see TopicRank for
         # threshold/method parameters.
         self.candidate_weighting(alpha=1.1,
                                  threshold=threshold,
                                  method='average')
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/positionrank.py` & `pke_zh-0.2.5/pke_zh/positionrank.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   Documents.
   *In proceedings of ACL*, pages 1105-1115, 2017.
 """
 
 from collections import defaultdict
 import networkx as nx
 
-from pke_zh.unsupervised.singlerank import SingleRank
+from pke_zh.singlerank import SingleRank
 
 
 class PositionRank(SingleRank):
     """PositionRank keyphrase extraction model"""
 
     def __init__(self):
         """Redefining initializer for PositionRank."""
@@ -152,20 +152,25 @@
                         tol=0.0001,
                         personalization=self.positions,
                         weight='weight')
 
         # loop through the candidates
         self.candidate_weight_norm(w, normalized)
 
-    def extract(self, input_file_or_string, n_best=10, pos=None):
+    def extract(self, input_file_or_string, n_best=10, pos=None, **kwargs):
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         # 1. valid postags
         if pos is None:
             pos = {'n', 'a'}
         # 2. clear cache
         self.clear_cache()
         # 3. load the content of the document.
         self.load_document(input=input_file_or_string, language='zh', normalization=None)
         # 4. select the noun phrases up to 3 words as keyphrase candidates.
         self.candidate_selection(pos=pos, maximum_word_number=3)
+        if not self.candidates:
+            return keyphrases
         self.candidate_weighting(window=10, pos=pos)
         keyphrases = self.get_n_best(n=n_best)
         return keyphrases
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/singlerank.py` & `pke_zh-0.2.5/pke_zh/singlerank.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 * Xiaojun Wan and Jianguo Xiao.
   CollabRank: Towards a Collaborative Approach to Single-Document Keyphrase
   Extraction.
   *In proceedings of the COLING*, pages 969-976, 2008.
 """
 import networkx as nx
-from pke_zh.unsupervised.textrank import TextRank
+from pke_zh.textrank import TextRank
 
 
 class SingleRank(TextRank):
     """SingleRank keyphrase extraction model.
 
     This model is an extension of the TextRank model that uses the number of
     co-occurrences to weigh edges in the graph.
@@ -95,13 +95,18 @@
                               alpha=0.85,
                               tol=0.0001,
                               weight='weight')
 
         # loop through the candidates
         self.candidate_weight_calculate(w, normalized)
 
-    def extract(self, input_file_or_string, n_best=10, pos=None):
+    def extract(self, input_file_or_string, n_best=10, pos=None, **kwargs):
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         self.load_document(input=input_file_or_string, language='zh', normalization=None)
         self.candidate_selection(pos=pos)
+        if not self.candidates:
+            return keyphrases
         self.candidate_weighting(window=10, pos=pos)
         keyphrases = self.get_n_best(n=n_best)
         return keyphrases
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/tfidf.py` & `pke_zh-0.2.5/pke_zh/tfidf.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,12 +60,17 @@
         total = sum([len(v.surface_forms) for v in self.candidates.values()])
 
         for k, v in self.candidates.items():
             # add the idf score to the weights container
             self.weights[k] = len(v.surface_forms) / total * self.idf_freq.get(k, self.median_idf)
 
     def extract(self, input_file_or_string, n_best=10, pos=None):
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         self.load_document(input=input_file_or_string, language='zh')
         self.candidate_selection(n=3)
+        if not self.candidates:
+            return keyphrases
         self.candidate_weighting()
         keyphrases = self.get_n_best(n=n_best, redundancy_removal=True)
         return keyphrases
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/topicrank.py` & `pke_zh-0.2.5/pke_zh/topicrank.py`

 * *Files 6% similar despite different names*

```diff
@@ -202,16 +202,21 @@
                 self.weights[topic[most_frequent]] = w[i]
 
             else:
                 first = offsets.index(min(offsets))
                 self.weights[topic[first]] = w[i]
 
     def extract(self, input_file_or_string, n_best=10, pos=None):
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         if pos is None:
             pos = {'n', 'a'}
         self.load_document(input=input_file_or_string, language='zh')
         self.clear_cache()
         self.candidate_selection(pos=pos)
+        if not self.candidates:
+            return keyphrases
         self.candidate_weighting(threshold=0.74, method='average')
         # get the 10-highest scored candidates as keyphrases
         keyphrases = self.get_n_best(n=n_best)
         return keyphrases
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/yake.py` & `pke_zh-0.2.5/pke_zh/yake.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 modify from: https://pypi.org/project/iyake-cn/0.5.5/#files
 
 """
 
 import math
 from collections import defaultdict
 import numpy as np
+from pke_zh.utils.text_utils import edit_distance
 from pke_zh.base import BaseKeywordExtractModel
 
 
 class Yake(BaseKeywordExtractModel):
     """YAKE keyphrase extraction model."""
 
     def __init__(self):
@@ -308,17 +309,16 @@
             candidate (str): the lexical form of the candidate.
             prev (list): the list of already selected candidates.
             threshold (float): the threshold used when computing the
                     char sim score, defaults to 0.6.
         """
         # loop through the already selected candidates
         for prev_candidate in prev:
-            s1 = set(prev_candidate)
-            s2 = set(candidate)
-            sim_score = len(s1 & s2) / min(len(s1), len(s2))
+            dist = edit_distance(prev_candidate, candidate)
+            sim_score = 1.0 - dist
             if sim_score >= threshold:
                 return True
         return False
 
     def get_n_best(
             self,
             n=10,
@@ -359,20 +359,25 @@
 
         # get the list of best candidates as (lexical form, weight) tuples
         n_best = [(u.replace(' ', ''), self.weights[u]) for u in best[:min(n, len(best))]]
         # return the list of best candidates
         return n_best
 
     def extract(self, input_file_or_string, n_best=10, threshold=0.6, window=2):
+        keyphrases = []
+        if not input_file_or_string:
+            return keyphrases
         # load the content of the document.
         self.load_document(input=input_file_or_string, language='zh', normalization=None)
         self.clear_cache()
         # select {1-3}-grams not containing punctuation marks and not
         #    beginning/ending with a stop word as candidates.
         self.candidate_selection(n=3)
+        if not self.candidates:
+            return keyphrases
         # weight the candidates using YAKE weighting scheme, a window (in
         #    words) for computing left/right contexts can be specified.
         self.candidate_weighting(window=window)
         # Get the 10-highest scored candidates as keyphrases.
         #    redundant keyphrases are removed from the output using levenshtein
         #    distance and a threshold.
         keyphrases = self.get_n_best(n=n_best, threshold=threshold)
```

### Comparing `pke_zh-0.2.3/pke_zh/unsupervised/yake_zh.py` & `pke_zh-0.2.5/pke_zh/yake_zh.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re
 from math import log10, sqrt
 from jieba import lcut, posseg
 
 pwd_path = os.path.abspath(os.path.dirname(__file__))
 
 # inner data file
-default_stopwords_path = os.path.join(pwd_path, '../data/stopwords.txt')
+default_stopwords_path = os.path.join(pwd_path, 'data/stopwords.txt')
 jieba.setLogLevel('ERROR')
 
 
 def get_pos_lst(words_lst):
     # 分词的位置列表
     return list(zip(words_lst, range(1, len(words_lst) + 1)))
 
@@ -91,15 +91,16 @@
         clean_str = re.sub(r'[0-9]+', '', content)
 
     jb_lst = [w for w in lcut(clean_str) if len(w) > 1]  # 分词过滤单字
 
     if stop is not None:
         # 停用词
         jb_lst = [w for w in jb_lst if w not in stop]
-
+    if jb_lst is None or len(jb_lst) == 0:
+        return None
     uni_lst = list(set(jb_lst))
     uni_lst.sort(key=jb_lst.index)  # 固定顺序唯一词
     split_content = re.split(r'[，；。？！]', clean_str)  # 原文本按标点拆分句子列表
 
     # 位置 T_pos 得分表
     pos_lst = 0
     if pos_type == 'w':
@@ -161,15 +162,15 @@
 def get_key_words(df_scores, n_best=10, sort_col='s_t', ascend=True, p=None):
     # 获取关键词列表，默认前10个，升序
     if p is None:
         p = {'n', 'a'}
     p = list(p)
     df_scores = df_scores[df_scores['pseg'].isin(p)]
     df_items = df_scores.sort_values(sort_col, ascending=ascend)
-    print(df_items)
+    # print(df_items)
     word_scores = zip(df_items['word'].to_list(), df_items['s_t'].to_list())
     return list(word_scores)[:n_best]
 
 
 def get_stopwords(txt_file):
     return set([line.strip() for line in open(txt_file, 'r', encoding='utf-8').readlines()])
 
@@ -177,16 +178,20 @@
 class YakeZH:
     def __init__(self, stopwords_path=None):
         if stopwords_path is None:
             stopwords_path = default_stopwords_path
         self.stopwords = get_stopwords(stopwords_path)
 
     def extract(self, text, n_best=10):
+        keyphrases = []
+        if not text:
+            return keyphrases
         df = get_S_t(text, stop=self.stopwords)
-        keyphrases = get_key_words(df, n_best=n_best)
+        if df is not None:
+            keyphrases = get_key_words(df, n_best=n_best)
         return keyphrases
 
 
 if __name__ == '__main__':
     txt = '物流很快，服务也很好，还有售后回馈。外观很时尚并且超大视野'
     m = YakeZH()
     words = m.extract(txt)
```

### Comparing `pke_zh-0.2.3/pke_zh/utils/file_utils.py` & `pke_zh-0.2.5/pke_zh/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/utils/io_utils.py` & `pke_zh-0.2.5/pke_zh/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh/utils/tokenizer.py` & `pke_zh-0.2.5/pke_zh/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pke_zh-0.2.3/pke_zh.egg-info/PKG-INFO` & `pke_zh-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: pke-zh
-Version: 0.2.3
+Name: pke_zh
+Version: 0.2.5
 Summary: pke_zh, context-aware bag-of-words term weights for query and document.
 Home-page: https://github.com/shibing624/pke_zh
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: # pke_zh
         [![PyPI version](https://badge.fury.io/py/pke_zh.svg)](https://badge.fury.io/py/pke_zh)
-        [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
+        [![Downloads](https://pepy.tech/badge/pke_zh)](https://pepy.tech/project/pke_zh)
         [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
-        PKE_zh, Python Keyphrase Extraction for ZH(chinese).
+        PKE_zh, Python Keyphrase Extraction for zh(chinese).
         
-        **pke_zh**实现了多种中文关键词提取算法，包括有监督的WordRank、无监督的TextRank, TfIdf, KeyBert, PositionRank, TopicRank等，扩展性强，开箱即用。
+        **pke_zh**实现了多种中文关键词提取算法，包括有监督的WordRank，无监督的TextRank、TfIdf、KeyBert、PositionRank、TopicRank等，扩展性强，开箱即用。
         
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
@@ -29,84 +29,92 @@
         - [Reference](#reference)
         
         # Feature
         
         如何提取query或者文档的关键词？
         
         
-        ### 有监督方法
-        #### 特征工程的解决思路
-        1. 实现时采用模型打分方法，以搜索query为原始语料，人工标注句子中各词重要度
-        
-        > 重要度共分4级：
-        > * Super important：主要包括POI核心词，比如“方特、欢乐谷”
-        > * Required：包括行政区词、品类词等，比如“北京 温泉”中“北京”和“温泉”都很重要
-        > * Important：包括品类词、门票等，比如“顺景 温泉”中“温泉”相对没有那么重要，用户搜“顺景”大部分都是温泉的需求
-        > * Unimportant：包括语气词、代词、泛需求词、停用词等
+        ## 有监督方法
+        ### 特征工程的解决思路
+        把关键词提取任务转化为分类任务，对输入query句子分词并提取多种特征，再把特征喂给机器学习模型，模型区分出各词的重要性得分，这样挑出topK个词作为关键词。
         
-        上例中可见“温泉”在不同的query中重要度是不同的。
-        
-        **特征方法**
+        #### 特征工程
         
         * 文本特征：包括Query长度、Term长度，Term在Query中的偏移量，term词性、长度信息、term数目、位置信息、句法依存tag、是否数字、是否英文、是否停用词、是否专名实体、是否重要行业词、embedding模长、删词差异度、以及短语生成树得到term权重等
-        * 统计特征：包括PMI、IDF、textrank值、前后词互信息、左右邻熵、独立检索占比（term单独作为query的qv/所有包含term的query的qv和）、统计概率、idf变种iqf
+        * 统计特征：包括PMI、IDF、TextRank值、前后词互信息、左右邻熵、独立检索占比（term单独作为query的qv/所有包含term的query的qv和）、统计概率、idf变种iqf
         * 语言模型特征：整个query的语言模型概率 / 去掉该Term后的Query的语言模型概率
         
-        2. 模型方面采用树模型（XGBoost等）进行训练，得到权重分类模型后在线上预测
-        ![term-weighting](./docs/gbdt.png)
         
-        #### 深度模型的解决思路
-        * 利用深度学习模型来学习term重要性，比如通过训练基于BiLSTM+Attention的query意图分类模型
-        * 基于Seq2Seq/Transformer训练的query翻译改写模型得到的attention权重副产物再结合其他策略或作为上述分类回归模型的特征也可以用于衡量term的重要性
-        * 利用BERT模型训练端到端的词分级模型，类似序列标注模型，后接CRF判定词重要性权重输出
-        
-        
-        **深度模型**
-        
-        * BERT CLS + softmax 
-        * Seq2Seq 文本摘要模型
-        
-        ### 无监督方法
-        - [x] TextRank
-        - [x] TfIdf
-        - [x] SingleRank
-        - [x] PositionRank
-        - [x] TopicRank
-        - [x] MultipartiteRank
-        - [x] Yake
-        - [x] KeyBert
+        训练样本形如：
+        ```shell
+        邪御天娇 免费 阅读,3 1 1
+        ```
+        
+        **重要度label**共分4级：
+        - Super important：3级，主要包括POI核心词，比如“方特、欢乐谷”
+        - Required：2级，包括行政区词、品类词等，比如“北京 温泉”中“北京”和“温泉”都很重要
+        - Important：1级，包括品类词、门票等，比如“顺景 温泉”中“温泉”相对没有那么重要，用户搜“顺景”大部分都是温泉的需求
+        - Unimportant：0级，包括语气词、代词、泛需求词、停用词等
         
+        上例中可见“温泉”在不同的query中重要度是不同的。
+        
+        分类模型可以是GBDT、LR、SVM、Xgboost等，这里以GBDT为例，GBDT模型（WordRank）的输入是特征向量，输出是重要度label。
+        
+        ![term-weighting](./docs/gbdt.png)
+        
+        ### 深度模型的解决思路
+        - 思路一：本质依然是把关键词提取任务转化为词重要度分类任务，利用深度模型学习term重要度，取代人工提取特征，模型端到端预测词重要度label，按重要度排序后挑出topK个词作为关键词。深度模型有TextCNN、Fasttext、Transformer、BERT等，适用于分类任务的模型都行。分类任务实现参考：https://github.com/shibing624/pytextclassifier
+        - 思路二：用Seq2Seq生成模型，输入query，输出关键词或者摘要，生成模型可以是T5、Bart、Seq2Seq等，生成任务实现参考：https://github.com/shibing624/textgen
+        
+        ## 无监督方法
+        - 统计算法
+        - [x] TFIDF，是很强的baseline，有较强普适性，基本能应付大部分关键词抽取场景，简单有效，速度很快，效果一般
+        - [x] YAKE，人工总结规则的方法，不依赖外部语料，从单文档提取关键词，速度很快，效果差
+        - 图算法
+        - [x] TextRank，简单套用PageRank思想到关键词提取的方法，效果不比TFIDF强，而且涉及网络构建和随机游走迭代，速度慢，效果一般
+        - [x] SingleRank，类似TextRank，是PageRank的变体，可以提取出关键短语，速度快，效果一般
+        - [x] TopicRank，基于主题模型的关键词提取算法，考虑了文档中词语的语义关系，可以提取出与文档主题相关的关键词，速度慢，效果一般
+        - [x] MultipartiteRank，一种基于多元关系的关键词提取算法，在TopicRank的基础上，考虑了词语的语义关系和词语位置，速度慢，效果一般
+        - [x] PositionRank，是基于PageRank的图关系计算词权重，考虑了词位置和词频，速度一般，效果好
+        - 语义模型
+        - [x] KeyBERT，利用了预训练语言模型的能力来提取关键词，速度很慢，效果最好
+        
+        **模型选型**
+        - 要求速度快，选择TFIDF、YAKE、PositionRank
+        - 要求效果好，选择KeyBERT
         
+        无监督算法介绍见文章[中文关键词提取算法](http://t.csdn.cn/6NO24)
         
         # Install
         * From pip:
-        ```shell
-        pip3 install -U pke_zh
+        ```zsh
+        pip install -U pke_zh
         ```
+        
         * From source：
-        ```shell
+        ```zsh
         git clone https://github.com/shibing624/pke_zh.git
         cd pke_zh
-        python3 setup.py install
+        python setup.py install
         ```
         
         ### 依赖数据
-        * 千兆中文文本训练的语言模型[zh_giga.no_cna_cmn.prune01244.klm(2.8G)](https://deepspeech.bj.bcebos.com/zh_lm/zh_giga.no_cna_cmn.prune01244.klm)，模型由pycorrector库自动下载于：~/.pycorrector/datasets/zh_giga.no_cna_cmn.prune01244.klm 。
-        * 中文文本匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) ，模型由transformers库自动下载于：~/.cache/huggingface/transformers/ 下。
+        * 千兆中文文本训练的语言模型[zh_giga.no_cna_cmn.prune01244.klm(2.8G)](https://deepspeech.bj.bcebos.com/zh_lm/zh_giga.no_cna_cmn.prune01244.klm)，模型由pycorrector库自动下载于 `~/.pycorrector/datasets/zh_giga.no_cna_cmn.prune01244.klm` 。
+        * 中文文本匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese) ，模型由transformers库自动下载于 `~/.cache/huggingface/transformers/` 下。
         
         # Usage
         
         ## 有监督关键词提取
         
-        直接调用训练好的WordRank模型，模型自动下载本地`~/.cache/pke_zh/wordrank_model.pkl`
+        直接调用训练好的WordRank模型，模型自动下载于 `~/.cache/pke_zh/wordrank_model.pkl` 。
         
         example: [examples/keyphrase_extraction_demo.py](examples/keyphrase_extraction_demo.py)
         
         ```python
-        from pke_zh.supervised.wordrank import WordRank
+        from pke_zh.wordrank import WordRank
         m = WordRank()
         print(m.extract("哪里下载电视剧周恩来？"))
         ```
         
         output:
         ```shell
         [('电视剧', 3), ('周恩来', 3), ('下载', 2), ('哪里', 1), ('？', 0)]
@@ -115,28 +123,28 @@
         
         ### 基于自有数据训练模型
         
         训练example: [examples/train_supervised_wordrank_demo.py](examples/train_supervised_wordrank_demo.py)
         
         
         ## 无监督关键词提取
-        支持TextRank、TfIdf、KeyBert等关键词提取算法。
+        支持TextRank、TfIdf、PositionRank、KeyBert等关键词提取算法。
         
         example: [examples/unsupervised_demo.py](examples/unsupervised_demo.py)
         
         
         ```python
-        from pke_zh.unsupervised.textrank import TextRank
-        from pke_zh.unsupervised.tfidf import TfIdf
-        from pke_zh.unsupervised.singlerank import SingleRank
-        from pke_zh.unsupervised.positionrank import PositionRank
-        from pke_zh.unsupervised.topicrank import TopicRank
-        from pke_zh.unsupervised.multipartiterank import MultipartiteRank
-        from pke_zh.unsupervised.yake import Yake
-        from pke_zh.unsupervised.keybert import KeyBert
+        from pke_zh.textrank import TextRank
+        from pke_zh.tfidf import TfIdf
+        from pke_zh.singlerank import SingleRank
+        from pke_zh.positionrank import PositionRank
+        from pke_zh.topicrank import TopicRank
+        from pke_zh.multipartiterank import MultipartiteRank
+        from pke_zh.yake import Yake
+        from pke_zh.keybert import KeyBert
         
         q = '哪里下载电视剧周恩来？'
         TextRank_m = TextRank()
         TfIdf_m = TfIdf()
         PositionRank_m = PositionRank()
         KeyBert_m = KeyBert()
         
@@ -157,14 +165,32 @@
         ```shell
         TextRank: [('电视剧', 1.00000002)]
         TfIdf: [('哪里下载', 1.328307500322222), ('下载电视剧', 1.328307500322222), ('电视剧周恩来', 1.328307500322222)]
         PositionRank_m: [('电视剧', 1.0)]
         KeyBert_m: [('电视剧', 0.47165293)]
         ```
         
+        ### 无监督关键句提取（自动摘要）
+        支持TextRank摘要提取算法。
+        
+        example: [examples/keysentences_extraction_demo.py](examples/keysentences_extraction_demo.py)
+        
+        
+        ```python
+        from pke_zh.textrank import TextRank
+        
+        m = TextRank()
+        r = m.extract_sentences("较早进入中国市场的星巴克，是不少小资钟情的品牌。相比 在美国的平民形象，星巴克在中国就显得“高端”得多。用料并无差别的一杯中杯美式咖啡，在美国仅约合人民币12元，国内要卖21元，相当于贵了75%。  第一财经日报")
+        print(r)
+        ```
+        
+        output:
+        ```shell
+        [('相比在美国的平民形象', 0.13208935993025409), ('在美国仅约合人民币12元', 0.1320761453200497), ('星巴克在中国就显得“高端”得多', 0.12497451534612379), ('国内要卖21元', 0.11929080110899569) ...]
+        ```
         
         # Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pke_zh.svg)](https://github.com/shibing624/pke_zh/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我：加我*微信号：xuming624*, 备注：*姓名-公司名-NLP* 进NLP交流群。
         
@@ -221,16 +247,11 @@
 Platform: Unix
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `pke_zh-0.2.3/pke_zh.egg-info/SOURCES.txt` & `pke_zh-0.2.5/pke_zh.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 README.md
 setup.py
 pke_zh/__init__.py
 pke_zh/base.py
 pke_zh/data_structures.py
+pke_zh/keybert.py
+pke_zh/multipartiterank.py
+pke_zh/positionrank.py
 pke_zh/readers.py
+pke_zh/singlerank.py
+pke_zh/textrank.py
+pke_zh/tfidf.py
+pke_zh/topicrank.py
 pke_zh/version.py
+pke_zh/wordrank.py
+pke_zh/yake.py
+pke_zh/yake_zh.py
 pke_zh.egg-info/PKG-INFO
 pke_zh.egg-info/SOURCES.txt
 pke_zh.egg-info/dependency_links.txt
 pke_zh.egg-info/not-zip-safe
 pke_zh.egg-info/requires.txt
 pke_zh.egg-info/top_level.txt
 pke_zh/data/common_char_set.txt
 pke_zh/data/entropy_word_score.json
 pke_zh/data/person_name.txt
 pke_zh/data/place_name.txt
 pke_zh/data/pmi_word_score.json
 pke_zh/data/stopwords.txt
-pke_zh/supervised/__init__.py
-pke_zh/supervised/wordrank.py
-pke_zh/unsupervised/__init__.py
-pke_zh/unsupervised/keybert.py
-pke_zh/unsupervised/multipartiterank.py
-pke_zh/unsupervised/positionrank.py
-pke_zh/unsupervised/singlerank.py
-pke_zh/unsupervised/textrank.py
-pke_zh/unsupervised/tfidf.py
-pke_zh/unsupervised/topicrank.py
-pke_zh/unsupervised/yake.py
-pke_zh/unsupervised/yake_zh.py
 pke_zh/utils/__init__.py
 pke_zh/utils/file_utils.py
 pke_zh/utils/io_utils.py
 pke_zh/utils/text_utils.py
 pke_zh/utils/tokenizer.py
```

