# Comparing `tmp/goodai-ltm-0.2.0.tar.gz` & `tmp/goodai-ltm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.2.0.tar", last modified: Wed May 31 12:50:18 2023, max compression
+gzip compressed data, was "goodai-ltm-0.2.1.tar", last modified: Tue Jul 18 17:15:40 2023, max compression
```

## Comparing `goodai-ltm-0.2.0.tar` & `goodai-ltm-0.2.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.707733 goodai-ltm-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2008 2023-05-31 12:50:18.706732 goodai-ltm-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    15811 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.589092 goodai-ltm-0.2.0/goodai/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.604091 goodai-ltm-0.2.0/goodai/helpers/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/__init__.py
--rw-rw-rw-   0        0        0     3257 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/json_helper.py
--rw-rw-rw-   0        0        0     1473 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/helpers/sched_opt.py
--rw-rw-rw-   0        0        0     3911 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.607095 goodai-ltm-0.2.0/goodai/ltm/
--rw-rw-rw-   0        0        0       34 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.608092 goodai-ltm-0.2.0/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.612091 goodai-ltm-0.2.0/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     1996 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/names/__init__.py
--rw-rw-rw-   0        0        0   183119 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/names/wikidata-names.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.630514 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      485 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     3036 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      331 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    11554 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1857 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa_tok_entry.py
--rw-rw-rw-   0        0        0     8159 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/sharc.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.633132 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-05-08 20:37:32.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
--rw-rw-rw-   0        0        0     7168 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wiki.py
--rw-rw-rw-   0        0        0     7229 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wikianswers.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.647171 goodai-ltm-0.2.0/goodai/ltm/embeddings/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/__init__.py
--rw-rw-rw-   0        0        0     3212 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/auto.py
--rw-rw-rw-   0        0        0     1726 2023-05-03 22:03:18.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/base.py
--rw-rw-rw-   0        0        0     1554 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/contrast_classifier.py
--rw-rw-rw-   0        0        0     5994 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/default.py
--rw-rw-rw-   0        0        0     1515 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     3116 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/openai_emb.py
--rw-rw-rw-   0        0        0     2610 2023-05-03 22:03:18.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/st_emb.py
--rw-rw-rw-   0        0        0     5989 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/embeddings/trainable.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.661172 goodai-ltm-0.2.0/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0     1589 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/auto.py
--rw-rw-rw-   0        0        0     4796 2023-05-18 14:51:26.000000 goodai-ltm-0.2.0/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     2716 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/metrics.py
--rw-rw-rw-   0        0        0     2158 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/msmarco.py
--rw-rw-rw-   0        0        0     1708 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/qp_ds.py
--rw-rw-rw-   0        0        0     1901 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/qrecc.py
--rw-rw-rw-   0        0        0     2072 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/strategy_qa.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.662171 goodai-ltm-0.2.0/goodai/ltm/eval/tests/
--rw-rw-rw-   0        0        0     1420 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/eval/tests/test_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.676734 goodai-ltm-0.2.0/goodai/ltm/mem/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.0/goodai/ltm/mem/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/auto.py
--rw-rw-rw-   0        0        0     6012 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/base.py
--rw-rw-rw-   0        0        0     1678 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/chunk.py
--rw-rw-rw-   0        0        0    24198 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/chunk_queue.py
--rw-rw-rw-   0        0        0     4635 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/config.py
--rw-rw-rw-   0        0        0    10212 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/default.py
--rw-rw-rw-   0        0        0    17984 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/mem_foundation.py
--rw-rw-rw-   0        0        0    13064 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/mem/rewrite_model.py
--rw-rw-rw-   0        0        0     3465 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.679732 goodai-ltm-0.2.0/goodai/ltm/mem/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/mem/tests/__init__.py
--rw-rw-rw-   0        0        0    13906 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/tests/test_chunk_queue.py
--rw-rw-rw-   0        0        0    16882 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/mem/tests/test_mem.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.690733 goodai-ltm-0.2.0/goodai/ltm/reranking/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/auto.py
--rw-rw-rw-   0        0        0     1248 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/base.py
--rw-rw-rw-   0        0        0    10135 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/default.py
--rw-rw-rw-   0        0        0     2219 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/emb.py
--rw-rw-rw-   0        0        0      706 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/prob_model.py
--rw-rw-rw-   0        0        0      808 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/st_ce.py
--rw-rw-rw-   0        0        0     6952 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/reranking/stanford.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.691733 goodai-ltm-0.2.0/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.696732 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7420 2023-05-03 13:13:46.000000 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/em_trainer.py
--rw-rw-rw-   0        0        0     7635 2023-05-08 20:37:32.000000 goodai-ltm-0.2.0/goodai/ltm/training/query_passage/qppm_trainer.py
--rw-rw-rw-   0        0        0       23 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/ltm/version.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.698733 goodai-ltm-0.2.0/goodai/modules/
--rw-rw-rw-   0        0        0     1647 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/goodai/modules/loss.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.700732 goodai-ltm-0.2.0/goodai/text_gen/
--rw-rw-rw-   0        0        0      158 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/text_gen/base.py
--rw-rw-rw-   0        0        0     1860 2023-05-31 12:39:52.000000 goodai-ltm-0.2.0/goodai/text_gen/openai_tg.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:50:18.705732 goodai-ltm-0.2.0/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0     2008 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2573 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 12:50:18.000000 goodai-ltm-0.2.0/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 12:50:18.707733 goodai-ltm-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-05-11 14:39:36.000000 goodai-ltm-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.221484 goodai-ltm-0.2.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2008 2023-07-18 17:15:40.221484 goodai-ltm-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15811 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.098476 goodai-ltm-0.2.1/goodai/
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.114475 goodai-ltm-0.2.1/goodai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3257 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     1473 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/helpers/sched_opt.py
+-rw-rw-rw-   0        0        0     3911 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.116474 goodai-ltm-0.2.1/goodai/ltm/
+-rw-rw-rw-   0        0        0       34 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.119475 goodai-ltm-0.2.1/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.122474 goodai-ltm-0.2.1/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     1996 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/names/__init__.py
+-rw-rw-rw-   0        0        0   183119 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/names/wikidata-names.json
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.139474 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      485 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     3036 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      331 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    11554 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1857 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/qa_tok_entry.py
+-rw-rw-rw-   0        0        0     8159 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/sharc.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.142474 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     2632 2023-05-08 20:37:32.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
+-rw-rw-rw-   0        0        0     7168 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/wiki.py
+-rw-rw-rw-   0        0        0     7229 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/ltm/data/query_passage/wikianswers.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.157477 goodai-ltm-0.2.1/goodai/ltm/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     3212 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/auto.py
+-rw-rw-rw-   0        0        0     1726 2023-05-03 22:03:18.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/base.py
+-rw-rw-rw-   0        0        0     1554 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5994 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/default.py
+-rw-rw-rw-   0        0        0     1515 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     3116 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/openai_emb.py
+-rw-rw-rw-   0        0        0     2610 2023-05-03 22:03:18.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/st_emb.py
+-rw-rw-rw-   0        0        0     5989 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/embeddings/trainable.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.170490 goodai-ltm-0.2.1/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0     1589 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/auto.py
+-rw-rw-rw-   0        0        0     4796 2023-05-18 14:51:26.000000 goodai-ltm-0.2.1/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     2716 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/metrics.py
+-rw-rw-rw-   0        0        0     2158 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/msmarco.py
+-rw-rw-rw-   0        0        0     1708 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/qp_ds.py
+-rw-rw-rw-   0        0        0     1901 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/qrecc.py
+-rw-rw-rw-   0        0        0     2072 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/strategy_qa.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.172484 goodai-ltm-0.2.1/goodai/ltm/eval/tests/
+-rw-rw-rw-   0        0        0     1420 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/eval/tests/test_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.188485 goodai-ltm-0.2.1/goodai/ltm/mem/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:28.000000 goodai-ltm-0.2.1/goodai/ltm/mem/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/mem/auto.py
+-rw-rw-rw-   0        0        0     6334 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/base.py
+-rw-rw-rw-   0        0        0     1710 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/chunk.py
+-rw-rw-rw-   0        0        0    24637 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/chunk_queue.py
+-rw-rw-rw-   0        0        0     4769 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/config.py
+-rw-rw-rw-   0        0        0    10427 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/default.py
+-rw-rw-rw-   0        0        0    17986 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/mem_foundation.py
+-rw-rw-rw-   0        0        0    13064 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/ltm/mem/rewrite_model.py
+-rw-rw-rw-   0        0        0     3465 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/mem/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.191484 goodai-ltm-0.2.1/goodai/ltm/mem/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.1/goodai/ltm/mem/tests/__init__.py
+-rw-rw-rw-   0        0        0    14538 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/tests/test_chunk_queue.py
+-rw-rw-rw-   0        0        0    19855 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/mem/tests/test_mem.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.204484 goodai-ltm-0.2.1/goodai/ltm/reranking/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/auto.py
+-rw-rw-rw-   0        0        0     1248 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/base.py
+-rw-rw-rw-   0        0        0    10135 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/default.py
+-rw-rw-rw-   0        0        0     2219 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/emb.py
+-rw-rw-rw-   0        0        0      706 2023-05-02 15:31:29.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/prob_model.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/st_ce.py
+-rw-rw-rw-   0        0        0     6952 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/ltm/reranking/stanford.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.205484 goodai-ltm-0.2.1/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.1/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.210486 goodai-ltm-0.2.1/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-05-02 15:31:29.000000 goodai-ltm-0.2.1/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7420 2023-05-03 13:13:46.000000 goodai-ltm-0.2.1/goodai/ltm/training/query_passage/em_trainer.py
+-rw-rw-rw-   0        0        0     7635 2023-05-08 20:37:32.000000 goodai-ltm-0.2.1/goodai/ltm/training/query_passage/qppm_trainer.py
+-rw-rw-rw-   0        0        0       23 2023-07-18 17:15:19.000000 goodai-ltm-0.2.1/goodai/ltm/version.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.212484 goodai-ltm-0.2.1/goodai/modules/
+-rw-rw-rw-   0        0        0     1647 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/goodai/modules/loss.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.215484 goodai-ltm-0.2.1/goodai/text_gen/
+-rw-rw-rw-   0        0        0      158 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/text_gen/base.py
+-rw-rw-rw-   0        0        0     1860 2023-05-31 12:39:52.000000 goodai-ltm-0.2.1/goodai/text_gen/openai_tg.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:15:40.220483 goodai-ltm-0.2.1/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0     2008 2023-07-18 17:15:39.000000 goodai-ltm-0.2.1/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2573 2023-07-18 17:15:40.000000 goodai-ltm-0.2.1/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:15:39.000000 goodai-ltm-0.2.1/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-18 17:15:39.000000 goodai-ltm-0.2.1/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 17:15:40.000000 goodai-ltm-0.2.1/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:15:40.221484 goodai-ltm-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-05-11 14:39:36.000000 goodai-ltm-0.2.1/setup.py
```

### Comparing `goodai-ltm-0.2.0/LICENSE` & `goodai-ltm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/PKG-INFO` & `goodai-ltm-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodai-ltm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A text memory meant to be used with conversational language models.
 Home-page: https://github.com/GoodAI/goodai-ltm
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## GoodAI-LTM
```

### Comparing `goodai-ltm-0.2.0/README.md` & `goodai-ltm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/helpers/file_helper.py` & `goodai-ltm-0.2.1/goodai/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/helpers/sched_opt.py` & `goodai-ltm-0.2.1/goodai/helpers/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/helpers/tokenizer_helper.py` & `goodai-ltm-0.2.1/goodai/helpers/tokenizer_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/cloud.py` & `goodai-ltm-0.2.1/goodai/ltm/data/cloud.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.2.1/goodai/ltm/data/names/__init__.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/names/wikidata-names.json` & `goodai-ltm-0.2.1/goodai/ltm/data/names/wikidata-names.json`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/auto_data_source.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/auto_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/dataset.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/sharc.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/sharc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/wiki.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/data/query_passage/wikianswers.py` & `goodai-ltm-0.2.1/goodai/ltm/data/query_passage/wikianswers.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/auto.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/base.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/contrast_classifier.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/default.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/emb_qp_prob_model.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/emb_qp_prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/openai_emb.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/openai_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/st_emb.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/st_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/embeddings/trainable.py` & `goodai-ltm-0.2.1/goodai/ltm/embeddings/trainable.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/auto.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/mem.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/mem.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/msmarco.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/msmarco.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/qp_ds.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/qp_ds.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/qrecc.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/qrecc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/strategy_qa.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/strategy_qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/eval/tests/test_metrics.py` & `goodai-ltm-0.2.1/goodai/ltm/eval/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/auto.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/base.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,22 @@
         :param text_key: A key previously returned by the add_text() method.
         :param show_progress_bar: Whether a progress bar should be shown.
         :return: The text key.
         """
         pass
 
     @abstractmethod
+    def get_text(self, text_key: TextKeyType) -> Optional[str]:
+        """
+        :param text_key: A key previously returned by the add_text() method.
+        :return: The text associated with the provided key. If the key does not exist, the returned value is None.
+        """
+        pass
+
+    @abstractmethod
     def add_separator(self):
         """
         Adds a section separator. The last chunk in the memory queue will be filled with padding.
         Chunk expansion cannot go across section boundaries.
         """
         pass
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/chunk.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/chunk.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                  importance: Optional[float], timestamp: float):
         self.importance = importance
         self.metadata = metadata
         self.chunk_id = chunk_id
         self.capacity = capacity
         self.from_token_seq_id = from_token_seq_id
         self.to_token_seq_id = from_token_seq_id
-        self.indexed: bool = False
+        self.indexed_length: int = -1
         self.timestamp: float = timestamp
         self.associated_keys = []
 
     def __len__(self):
         return self.to_token_seq_id - self.from_token_seq_id
 
     def get_room(self):
@@ -37,14 +37,14 @@
         self.to_token_seq_id += num_tokens
 
     def shift(self, offset: int):
         self.from_token_seq_id += offset
         self.to_token_seq_id += offset
 
     def is_indexed(self) -> bool:
-        return self.indexed
+        return self.indexed_length == len(self)
 
-    def set_indexed(self, mode: bool):
-        self.indexed = mode
+    def update_indexed_state(self):
+        self.indexed_length = len(self)
 
     def add_key(self, text_key: TextKeyType):
         self.associated_keys.append(text_key)
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/chunk_queue.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/chunk_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         sep_ids = self.separator_seq_ids
         if len(sep_ids) > 0:
             last_sep_id = sep_ids[-1]
             if len(self.token_ids) + self.first_token_seq_id == last_sep_id:
                 return True
         return False
 
-    def add_separator(self, pad_token_id: int, timestamp: Optional[float] = None):
+    def add_separator(self):
         # self._pad_last_chunk(pad_token_id)
         # separator_seq_ids always assumed to be ordered
         self.separator_seq_ids.append(self.first_token_seq_id + len(self.token_ids))
 
     def add_sequence(self, new_token_ids: List[int], metadata: Optional[Any],
                      importance: Optional[float] = None, timestamp: Optional[float] = None,
                      _no_new_chunks: bool = False,
@@ -354,14 +354,24 @@
         # This call updates separator seq IDs according to the shift offset
         dc1 = self._resolve_discarded_chunks(discarded_chunks, text_key,
                                              seq_id_from, old_seq_id_to, new_seq_id_to,
                                              shift_offset)
         dc2 = self.check_overflow()
         return dc1 + dc2, text_key,
 
+    def get_sequence_token_ids(self, text_key: TextKeyType) -> Optional[List[int]]:
+        seq_bounds = self.sequence_map.get(text_key)
+        if seq_bounds is None:
+            logging.warning(f'Subsequence with key {text_key} not found.')
+            return None
+        seq_id_from, seq_id_to = seq_bounds
+        first_id = self.first_token_seq_id
+        index_from, index_to = seq_id_from - first_id, seq_id_to - first_id,
+        return self.token_ids[index_from:index_to]
+
     def get_chunks_for_indexing(self) -> Tuple[List[Chunk], List[List[int]]]:
         # TODO not super efficient
         token_id_matrix = []
         picked_buckets = []
         for i, chunk in enumerate(self.chunks):
             if not chunk.is_indexed():
                 token_ids = self.get_chunk_token_ids(chunk)
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/config.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     def for_paragraph(cls, max_extra_side_tokens: int = 192):
         return cls(max_extra_side_tokens=max_extra_side_tokens, limit_type=ChunkExpansionLimitType.PARAGRAPH)
 
     @classmethod
     def for_section(cls, max_extra_side_tokens: int = 1024):
         return cls(max_extra_side_tokens=max_extra_side_tokens, limit_type=ChunkExpansionLimitType.SECTION)
 
+    @classmethod
+    def for_chunk(cls):
+        return cls(max_extra_side_tokens=0, limit_type=ChunkExpansionLimitType.SECTION)
+
 
 class TextMemoryConfig:
     chunk_capacity: int
     """
     The capacity of a chunk, in tokens.
     """
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/default.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 
     def get_chunk(self, chunk_id: int) -> Chunk:
         return self.chunk_queue.get_chunk(chunk_id)
 
     def retrieve_chunk_sequences(self, chunks: List[Chunk]):
         return self.chunk_queue.retrieve_chunk_sequences_given_chunks(chunks)
 
+    def get_text(self, text_key: TextKeyType) -> Optional[str]:
+        token_ids = self.chunk_queue.get_sequence_token_ids(text_key)
+        if token_ids is None:
+            return None
+        return self.chunk_tokenizer.decode(token_ids, skip_special_tokens=True)
+
     def get_retrieval_key_for_text(self, queries: List[str], show_progress_bar: bool = False) -> torch.Tensor:
         return self.emb_model.encode_queries(queries, convert_to_tensor=True, show_progress_bar=show_progress_bar)
 
     def predict_match(self, sentences: List[Tuple[str, str]], show_progress_bar: bool = False,
                       batch_size: int = 32) -> List[float]:
         return self.matching_model.predict(sentences, show_progress_bar=show_progress_bar,
                                            batch_size=batch_size)
@@ -139,15 +145,15 @@
                                          rewrite_context=rewrite_context, show_progress_bar=show_progress_bar,
                                          timestamp=timestamp, text_key=text_key)
 
     def delete_text(self, text_key: TextKeyType, show_progress_bar: bool = False) -> TextKeyType:
         return self.replace_text(text_key, "", show_progress_bar=show_progress_bar)
 
     def add_separator(self):
-        self.chunk_queue.add_separator(self.pad_token_id)
+        self.chunk_queue.add_separator()
 
     def is_empty(self) -> bool:
         return len(self.chunk_queue.token_ids) == 0
 
     def retrieve_all_text(self) -> str:
         token_ids = self.chunk_queue.get_latest_token_ids(max_num_tokens=None)
         return self.chunk_tokenizer.decode(token_ids, skip_special_tokens=True)
@@ -180,16 +186,15 @@
         if len(sk_list) > 0:
             sk_all = torch.cat(sk_list)
             num_chunks, num_sk = sk_all.size(0), sk_all.size(1),
             sk_all = sk_all.view(num_chunks * num_sk, -1)
             sk_all_np = sk_all.cpu().numpy().astype(np.float32)
             b_indexes = []
             for chunk in picked_chunks:
-                if chunk.is_at_capacity():
-                    chunk.set_indexed(True)
+                chunk.update_indexed_state()
                 b_indexes.extend([chunk.chunk_id] * num_sk)
             b_indexes_np = np.array(b_indexes).astype(np.int64)
             self.vector_db.add_with_ids(sk_all_np, b_indexes_np)
 
     def clear(self):
         self.chunk_queue.flush()
         self.vector_db.reset()
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/mem_foundation.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/mem_foundation.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,15 @@
             for distance, chunk_id in zip(row_d, row_i):
                 if chunk_id in id_set or chunk_id < 0:
                     continue
                 id_set.add(chunk_id)
                 distinct_d_i.append((distance, chunk_id,))
             # Without duplicates, we only need at most expansion_top_k chunks at this point
             distinct_d_i = distinct_d_i[:expansion_top_k]
+
             # Retrieve chunk objects from queue
             row_chunks = [self.get_chunk(chunk_id) for _, chunk_id in distinct_d_i]
             row_passages = [self.get_complete_passage(chunk) for chunk in row_chunks]
             row_r_chunks = [RetrievedChunk(chunk, distance, passage)
                             for chunk, passage, (distance, _) in
                             zip(row_chunks, row_passages, distinct_d_i)]
             prelim_r_chunks.append(row_r_chunks)
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/rewrite_model.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/rewrite_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/simple_vector_db.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/simple_vector_db.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/tests/test_chunk_queue.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/tests/test_chunk_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,28 @@
-import math
 import unittest
-
 from goodai.ltm.mem.chunk_queue import ChunkQueue, ChunkExpansionOptions
 
 
 class TestChunkQueue(unittest.TestCase):
+    def test_simple_insertion(self):
+        seq_len = 8
+        queue_capacity = 10
+        num_seqs_in_chunk = 3
+        chunk_capacity = seq_len * num_seqs_in_chunk
+        chunk_index_at_overlap = chunk_capacity // 2
+        self.assertEqual(12, chunk_index_at_overlap)
+        sq = ChunkQueue(queue_capacity, chunk_capacity, chunk_index_at_overlap)
+        start = 0
+        token_ids = list(range(start, start + seq_len))
+        sq.add_sequence(token_ids, None)
+        token_ids = list(range(start + seq_len, start + seq_len + seq_len))
+        sq.add_sequence(token_ids, None)
+        self.assertEqual(2, len(sq.chunks))
+        self.assertEqual(16, len(sq.token_ids))
+
     def test_insertion(self):
         seq_len = 8
         queue_capacity = 10
         num_seqs_in_chunk = 3
         chunk_capacity = seq_len * num_seqs_in_chunk
         chunk_index_at_overlap = chunk_capacity // 2
         sq = ChunkQueue(queue_capacity, chunk_capacity, chunk_index_at_overlap)
@@ -139,24 +153,24 @@
 
     def test_separators(self):
         chunk_capacity = 5
         chunk_index_at_overlap = chunk_capacity // 2
         _chunk_queue = ChunkQueue(25, chunk_capacity, chunk_index_at_overlap, first_token_seq_id=75)
         _chunk_queue.add_sequence([1, 2, 3], None)
         _chunk_queue.add_sequence([4, 5, 6], None)
-        _chunk_queue.add_separator(0)
+        _chunk_queue.add_separator()
         _chunk_queue.add_sequence([7, 8, 9], None)
         _chunk_queue.add_sequence([10, 11, 12], None)
-        _chunk_queue.add_separator(0)
+        _chunk_queue.add_separator()
         _chunk_queue.add_sequence([10, 8, 12], None)
         _chunk_queue.add_sequence([14, 11, 12], None)
-        _chunk_queue.add_separator(0)
+        _chunk_queue.add_separator()
         _chunk_queue.add_sequence([3, 8, 21], None)
         _chunk_queue.add_sequence([13, 12, 9], None)
-        _chunk_queue.add_separator(0)
+        _chunk_queue.add_separator()
         _chunk_queue.add_sequence([3, 4, 28], None)
         _chunk_queue.add_sequence([12, 8, 25], None)
 
         punctuation_ids = {3, 8}
         ce_options = ChunkExpansionOptions.default(chunk_capacity, punctuation_ids)
 
         chunk_ids = [3, 6, 9]
@@ -170,28 +184,28 @@
     def test_overflow_with_separators(self):
         chunk_capacity = 5
         queue_capacity = 10
         chunk_index_at_overlap = chunk_capacity // 2
         _chunk_queue = ChunkQueue(queue_capacity, chunk_capacity, chunk_index_at_overlap, first_token_seq_id=75)
         for i in range(200):
             _chunk_queue.add_sequence([1, 2, 3], None)
-            _chunk_queue.add_separator(0)
+            _chunk_queue.add_separator()
         self.assertEqual(6, len(_chunk_queue.separator_seq_ids))
         self.assertTrue(_chunk_queue.separator_seq_ids[0] >= _chunk_queue.first_token_seq_id)
         self.assertTrue(_chunk_queue.separator_seq_ids[-1] <= _chunk_queue.first_token_seq_id +
                         len(_chunk_queue.token_ids))
 
     def test_flush(self):
         chunk_capacity = 5
         queue_capacity = 10
         chunk_index_at_overlap = chunk_capacity // 2
         _chunk_queue = ChunkQueue(queue_capacity, chunk_capacity, chunk_index_at_overlap, first_token_seq_id=220)
         for i in range(100):
             _chunk_queue.add_sequence([1, 2, 3], None)
-            _chunk_queue.add_separator(0)
+            _chunk_queue.add_separator()
         _chunk_queue.flush()
         self.assertTrue(len(_chunk_queue.separator_seq_ids) == 0)
         self.assertTrue(len(_chunk_queue.chunks) == 0)
         self.assertTrue(len(_chunk_queue.token_ids) == 0)
         self.assertTrue(len(_chunk_queue.chunk_map) == 0)
         self.assertTrue(_chunk_queue.first_token_seq_id == 0)
 
@@ -212,15 +226,15 @@
         expected_cs_2 = [[1, 2, 3, 8, 9], [3, 8, 9, 10, 9], [9, 10, 9], [9], [7, 8, 9], [9]]
         self.assertEqual(expected_cs_2, chunk_sequences)
 
     def test_replacement_2(self):
         chunk_capacity = 5
         chunk_index_at_overlap = chunk_capacity // 2
         _chunk_queue = ChunkQueue(25, chunk_capacity, chunk_index_at_overlap, first_token_seq_id=73)
-        _chunk_queue.add_separator(pad_token_id=0)
+        _chunk_queue.add_separator()
         _, k1 = _chunk_queue.add_sequence([1, 2, 3], None)
         _, k2 = _chunk_queue.add_sequence([4, 5, 6], None)
         _, k3 = _chunk_queue.add_sequence([7, 8, 9], None)
 
         chunk_sequences = _chunk_queue.get_chunk_sequences()
         expected_cs_1 = [[1, 2, 3, 4, 5], [3, 4, 5, 6, 7], [5, 6, 7, 8, 9], [7, 8, 9], [9]]
         self.assertEqual(expected_cs_1, chunk_sequences)
@@ -232,15 +246,15 @@
 
     def test_replacement_3(self):
         chunk_capacity = 5
         chunk_index_at_overlap = chunk_capacity // 2
         _chunk_queue = ChunkQueue(25, chunk_capacity, chunk_index_at_overlap, first_token_seq_id=43)
         _, k1 = _chunk_queue.add_sequence([1, 2, 3], None)
         _, k2 = _chunk_queue.add_sequence([4, 5, 6], None)
-        _chunk_queue.add_separator(pad_token_id=0)
+        _chunk_queue.add_separator()
         _, k3 = _chunk_queue.add_sequence([7, 8, 9], None)
 
         chunk_sequences = _chunk_queue.get_chunk_sequences()
         expected_cs_1 = [[1, 2, 3, 4, 5], [3, 4, 5, 6], [5, 6], [7, 8, 9], [9]]
         self.assertEqual(expected_cs_1, chunk_sequences)
 
         _chunk_queue.replace_sequence(k3, [11, 12, 11, 12, 11])
@@ -263,15 +277,15 @@
 
     def test_replacement_4(self):
         chunk_capacity = 5
         chunk_index_at_overlap = chunk_capacity // 2
         _chunk_queue = ChunkQueue(25, chunk_capacity, chunk_index_at_overlap, first_token_seq_id=43)
         _, k1 = _chunk_queue.add_sequence([1, 2, 3], None)
         _, k2 = _chunk_queue.add_sequence([4, 5, 6], None)
-        _chunk_queue.add_separator(pad_token_id=0)
+        _chunk_queue.add_separator()
         _, k3 = _chunk_queue.add_sequence([7, 8, 9], None)
 
         chunk_sequences = _chunk_queue.get_chunk_sequences()
         expected_cs_1 = [[1, 2, 3, 4, 5], [3, 4, 5, 6], [5, 6], [7, 8, 9], [9]]
         self.assertEqual(expected_cs_1, chunk_sequences)
 
         _chunk_queue.replace_sequence(k2, [11, 12, 13, 14, 15, 11, 12, 13, 14, 15])
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/mem/tests/test_mem.py` & `goodai-ltm-0.2.1/goodai/ltm/mem/tests/test_mem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import gc
 import unittest
-from typing import List, Tuple
+from typing import List, Tuple, cast
 
 from transformers import AutoTokenizer
 
 from goodai.ltm.embeddings.auto import AutoTextEmbeddingModel
 from goodai.ltm.eval.metrics import get_correctness_score
 from goodai.ltm.mem.auto import AutoTextMemory
 from goodai.ltm.mem.base import BaseReranker, RetrievedMemory, BaseTextMemory, BaseImportanceModel
 from goodai.ltm.mem.config import TextMemoryConfig, ChunkExpansionConfig, ChunkExpansionLimitType
+from goodai.ltm.mem.default import DefaultTextMemory
 from goodai.ltm.reranking.base import BaseTextMatchingModel
 
 
 class TestMem(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls._lr_emb_model = AutoTextEmbeddingModel.shared_pretrained('em-MiniLM-p1-01')
@@ -131,14 +132,36 @@
         qpm = _CustomQPM()
         mem = AutoTextMemory.create(matching_model=qpm, emb_model=self._lr_emb_model)
         mem.add_text(self._text)
         r_memories = mem.retrieve('Is water vapor widely present in the atmosphere?', k=5)
         assert 'UV-light' in r_memories[0].passage
         assert 'greenhouse' in r_memories[1].passage
 
+    def test_reranking_count_1(self):
+        s_counts = []
+
+        class _LocalReranker(BaseReranker):
+            def rerank(self, _r_memories: List[RetrievedMemory], _mem: BaseTextMemory) -> List[RetrievedMemory]:
+                nonlocal s_counts
+                s_counts.append(len(_r_memories))
+                result = list(_r_memories)
+                result.sort(key=lambda _m: _m.relevance)
+                return result
+
+        config = TextMemoryConfig()
+        config.reranking_k_factor = 7
+        config.chunk_capacity = 8
+        config.redundancy_overlap_threshold = 0.5
+        config.chunk_expansion_config = ChunkExpansionConfig.for_chunk()
+        mem = AutoTextMemory.create(emb_model=self._lr_emb_model, reranker=_LocalReranker(),
+                                    config=config)
+        mem.add_text(self._text)
+        mem.retrieve('Is water vapor widely present in the atmosphere?', k=3)
+        self.assertEqual([21], s_counts)
+
     def test_separators_and_replacement(self):
         facts = [
             'Cane toads have a life expectancy of 10 to 15 years in the wild.',
             'Kayaks are used to transport people in water.',
             'Darth Vader is portrayed as a man who always appears in black full-body armor and a mask.',
             'Tony Bennett had four children.'
         ]
@@ -161,14 +184,34 @@
             self.assertEqual(query.strip(), r_memories[0].passage.strip())
             self.assertAlmostEqual(i + 5, r_memories[0].timestamp)
             if is_replacement[i]:
                 self.assertTrue(r_memories[0].metadata['replacement'])
             else:
                 self.assertEqual(i, r_memories[0].metadata['index'])
 
+    def test_chunk_indexing_with_separators(self):
+        facts = [
+            "Higher education, also called post-secondary education, third-level or "
+            "tertiary education, is an optional final stage of formal learning that "
+            "occurs after completion of secondary education.",
+            'Cane toads have a life expectancy of 10 to 15 years in the wild.',
+            'Kayaks are used to transport people in water.',
+            'Darth Vader is portrayed as a man who always appears in black full-body armor and a mask.',
+            'Tony Bennett had four children.'
+        ]
+        config = TextMemoryConfig()
+        config.chunk_capacity = 8
+        mem = AutoTextMemory.create(emb_model=self._lr_emb_model, config=config)
+        for i, fact in enumerate(facts):
+            mem.add_text(fact)
+            mem.add_separator()
+        mem_default: DefaultTextMemory = cast(DefaultTextMemory, mem)
+        chunks, _ = mem_default.chunk_queue.get_chunks_for_indexing()
+        assert len(chunks) <= 3
+
     def test_delete_all(self):
         facts = [
             'Cane toads have a life expectancy of 10 to 15 years in the wild.',
             'Kayaks are used to transport people in water.',
             'Darth Vader is portrayed as a man who always appears in black full-body armor and a mask.',
             'Tony Bennett had four children.'
         ]
@@ -306,7 +349,30 @@
             p = m.passage.lower()
             if 'kayaks' in p:
                 self.assertAlmostEqual(m.importance, 0.25)
             elif 'vader' in p:
                 self.assertAlmostEqual(m.importance, 0.50)
             else:
                 self.assertAlmostEqual(m.importance, 0)
+
+    def test_get_text(self):
+        facts = [
+            'Cane toads have a life expectancy of 10 to 15 years in the wild.',
+            'Kayaks are used to transport people in water.',
+            'Darth Vader is portrayed as a man who always appears in black full-body armor and a mask.',
+            'Tony Bennett had four children.'
+        ]
+        config = TextMemoryConfig()
+        mem = AutoTextMemory.create(emb_model=self._lr_emb_model,
+                                    config=config)
+        text_keys = []
+        for i, fact in enumerate(facts):
+            tk = mem.add_text(fact, metadata={'index': i})
+            text_keys.append(tk)
+
+        for tk, fact in zip(text_keys, facts):
+            text = mem.get_text(tk)
+            self.assertEqual(fact, text)
+
+        text = mem.get_text(99999)
+        self.assertIsNone(text)
+
```

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/auto.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/base.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/base.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/default.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/emb.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/prob_model.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/st_ce.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/st_ce.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/reranking/stanford.py` & `goodai-ltm-0.2.1/goodai/ltm/reranking/stanford.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/training/query_passage/em_trainer.py` & `goodai-ltm-0.2.1/goodai/ltm/training/query_passage/em_trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/ltm/training/query_passage/qppm_trainer.py` & `goodai-ltm-0.2.1/goodai/ltm/training/query_passage/qppm_trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/modules/loss.py` & `goodai-ltm-0.2.1/goodai/modules/loss.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai/text_gen/openai_tg.py` & `goodai-ltm-0.2.1/goodai/text_gen/openai_tg.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/goodai_ltm.egg-info/PKG-INFO` & `goodai-ltm-0.2.1/goodai_ltm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodai-ltm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A text memory meant to be used with conversational language models.
 Home-page: https://github.com/GoodAI/goodai-ltm
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## GoodAI-LTM
```

### Comparing `goodai-ltm-0.2.0/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.2.1/goodai_ltm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.2.0/setup.py` & `goodai-ltm-0.2.1/setup.py`

 * *Files identical despite different names*

