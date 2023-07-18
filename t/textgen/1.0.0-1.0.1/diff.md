# Comparing `tmp/textgen-1.0.0.tar.gz` & `tmp/textgen-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-1.0.0.tar", last modified: Wed Jul  5 09:26:35 2023, max compression
+gzip compressed data, was "textgen-1.0.1.tar", last modified: Tue Jul 18 13:15:04 2023, max compression
```

## Comparing `textgen-1.0.0.tar` & `textgen-1.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.726122 textgen-1.0.0/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2023-05-09 12:23:08.000000 textgen-1.0.0/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    50754 2023-07-05 09:26:35.727118 textgen-1.0.0/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    44817 2023-07-04 04:37:00.000000 textgen-1.0.0/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-07-05 09:26:35.728308 textgen-1.0.0/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1394 2023-06-15 08:23:08.000000 textgen-1.0.0/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.630591 textgen-1.0.0/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1379 2023-06-16 09:50:52.000000 textgen-1.0.0/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.647338 textgen-1.0.0/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.653495 textgen-1.0.0/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       79 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    31716 2023-07-03 13:12:15.000000 textgen-1.0.0/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8514 2023-06-16 12:38:08.000000 textgen-1.0.0/textgen/chatglm/chatglm_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)     1265 2023-05-12 09:34:43.000000 textgen-1.0.0/textgen/chatglm/merge_peft_adapter.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.658100 textgen-1.0.0/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    15117 2023-07-03 13:03:20.000000 textgen-1.0.0/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.660239 textgen-1.0.0/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.667556 textgen-1.0.0/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    43533 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.675423 textgen-1.0.0/textgen/gpt/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/gpt/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    29197 2023-07-03 13:11:09.000000 textgen-1.0.0/textgen/gpt/gpt_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7407 2023-06-16 12:38:08.000000 textgen-1.0.0/textgen/gpt/gpt_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    13145 2023-06-19 08:05:18.000000 textgen-1.0.0/textgen/gpt/merge_peft_adapter.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.681933 textgen-1.0.0/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      231 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10113 2023-06-01 03:08:56.000000 textgen-1.0.0/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.689188 textgen-1.0.0/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56955 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65717 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.704430 textgen-1.0.0/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73253 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.718227 textgen-1.0.0/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50615 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50652 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.723766 textgen-1.0.0/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2023-05-09 12:23:08.000000 textgen-1.0.0/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-05 09:26:35.637750 textgen-1.0.0/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    50754 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1754 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      144 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-07-05 09:26:34.000000 textgen-1.0.0/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.436896 textgen-1.0.1/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2023-05-09 12:23:08.000000 textgen-1.0.1/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    50754 2023-07-18 13:15:04.438190 textgen-1.0.1/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    44817 2023-07-04 04:37:00.000000 textgen-1.0.1/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-07-18 13:15:04.439916 textgen-1.0.1/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1394 2023-07-18 13:14:11.000000 textgen-1.0.1/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.297604 textgen-1.0.1/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1379 2023-07-18 13:14:11.000000 textgen-1.0.1/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.315538 textgen-1.0.1/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.338231 textgen-1.0.1/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       79 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    31776 2023-07-18 07:20:45.000000 textgen-1.0.1/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8514 2023-06-16 12:38:08.000000 textgen-1.0.1/textgen/chatglm/chatglm_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1265 2023-05-12 09:34:43.000000 textgen-1.0.1/textgen/chatglm/merge_peft_adapter.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.346097 textgen-1.0.1/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15117 2023-07-03 13:03:20.000000 textgen-1.0.1/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.348211 textgen-1.0.1/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.359087 textgen-1.0.1/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    43533 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.371929 textgen-1.0.1/textgen/gpt/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/gpt/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    29257 2023-07-18 07:19:20.000000 textgen-1.0.1/textgen/gpt/gpt_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7407 2023-06-16 12:38:08.000000 textgen-1.0.1/textgen/gpt/gpt_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13145 2023-06-19 08:05:18.000000 textgen-1.0.1/textgen/gpt/merge_peft_adapter.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.375951 textgen-1.0.1/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      231 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10113 2023-06-01 03:08:56.000000 textgen-1.0.1/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.390531 textgen-1.0.1/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56955 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65717 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.409144 textgen-1.0.1/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73253 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.420105 textgen-1.0.1/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50615 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50652 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.426900 textgen-1.0.1/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2023-05-09 12:23:08.000000 textgen-1.0.1/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-18 13:15:04.303567 textgen-1.0.1/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    50754 2023-07-18 13:15:03.000000 textgen-1.0.1/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1754 2023-07-18 13:15:03.000000 textgen-1.0.1/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-18 13:15:03.000000 textgen-1.0.1/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      144 2023-07-18 13:15:03.000000 textgen-1.0.1/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-07-18 13:15:03.000000 textgen-1.0.1/textgen.egg-info/top_level.txt
```

### Comparing `textgen-1.0.0/LICENSE` & `textgen-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/PKG-INFO` & `textgen-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 1.0.0
+Version: 1.0.1
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [**🇨🇳中文**](https://github.com/shibing624/textgen/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/textgen/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: textgen Version: 1.0.0 Summary: Text Generation
+Metadata-Version: 2.1 Name: textgen Version: 1.0.1 Summary: Text Generation
 Model Home-page: https://github.com/shibing624/textgen Author: XuMing Author-
 email: xuming624@qq.com License: Apache 2.0 Description: [**ð¨ð³ä¸­æ**]
 (https://github.com/shibing624/textgen/blob/main/README.md) | [**ðEnglish**]
 (https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**ðææ¡£/
 Docs**](https://github.com/shibing624/textgen/wiki) | [**ð¤æ¨¡å/Models**]
 (https://huggingface.co/shibing624)
                                     [Logo]
```

### Comparing `textgen-1.0.0/README.md` & `textgen-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/setup.py` & `textgen-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='1.0.0',
+    version='1.0.1',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
```

### Comparing `textgen-1.0.0/textgen/__init__.py` & `textgen-1.0.1/textgen/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
```

### Comparing `textgen-1.0.0/textgen/augment/sentence_level_augment.py` & `textgen-1.0.1/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/augment/text_augment.py` & `textgen-1.0.1/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/augment/tokenizer.py` & `textgen-1.0.1/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/augment/translate_api.py` & `textgen-1.0.1/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/augment/word_level_augment.py` & `textgen-1.0.1/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/augment/word_vocab.py` & `textgen-1.0.1/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/chatglm/chatglm_model.py` & `textgen-1.0.1/textgen/chatglm/chatglm_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             self.device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
 
         self.results = {}
         model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
 
-        if torch.cuda.is_bf16_supported() and not self.args.bf16:
+        if torch.cuda.is_available() and torch.cuda.is_bf16_supported() and not self.args.bf16:
             logger.warning("GPU supports bf16, you can enable bf16.")
         self.torch_dtype = torch.bfloat16 if self.args.bf16 else (torch.float16 if self.args.fp16 else torch.float32)
         self.model = model_class.from_pretrained(
             model_name,
             load_in_8bit=self.args.int8,
             torch_dtype=self.torch_dtype,
             device_map=self.device_map,
@@ -395,15 +395,15 @@
         # Update model train config
         if self.args.gradient_checkpointing:
             self.model.gradient_checkpointing_enable()
             self.model.config.use_cache = False
         else:
             self.model.config.use_cache = True
         self.model.enable_input_require_grads()
-        if torch.cuda.device_count() > 1:
+        if torch.cuda.is_available() and torch.cuda.device_count() > 1:
             # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
             self.model.is_parallelizable = True
             self.model.model_parallel = True
         self.model.lm_head = CastOutputToFloat(self.model.lm_head)
 
         data_collator = DataCollatorForSeq2Seq(
             self.tokenizer,
```

### Comparing `textgen-1.0.0/textgen/chatglm/chatglm_utils.py` & `textgen-1.0.1/textgen/chatglm/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/chatglm/merge_peft_adapter.py` & `textgen-1.0.1/textgen/chatglm/merge_peft_adapter.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/config/global_args.py` & `textgen-1.0.1/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/config/model_args.py` & `textgen-1.0.1/textgen/config/model_args.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/custom_models/models.py` & `textgen-1.0.1/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/data/HowNetPOSWord.txt` & `textgen-1.0.1/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/data/stopwords.txt` & `textgen-1.0.1/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/gpt/gpt_model.py` & `textgen-1.0.1/textgen/gpt/gpt_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             self.device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
 
         self.results = {}
         model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
 
-        if torch.cuda.is_bf16_supported() and not self.args.bf16:
+        if torch.cuda.is_available() and torch.cuda.is_bf16_supported() and not self.args.bf16:
             logger.warning("GPU supports bf16, you can enable bf16.")
         self.torch_dtype = torch.bfloat16 if self.args.bf16 else (torch.float16 if self.args.fp16 else torch.float32)
         self.model = model_class.from_pretrained(
             model_name,
             load_in_8bit=self.args.int8,
             torch_dtype=self.torch_dtype,
             device_map=self.device_map,
@@ -404,15 +404,15 @@
         # Update model train config
         if self.args.gradient_checkpointing:
             self.model.gradient_checkpointing_enable()
             self.model.config.use_cache = False
         else:
             self.model.config.use_cache = True
         self.model.enable_input_require_grads()
-        if torch.cuda.device_count() > 1:
+        if torch.cuda.is_available() and torch.cuda.device_count() > 1:
             # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
             self.model.is_parallelizable = True
             self.model.model_parallel = True
 
         # Initialize our Trainer
         data_collator = DataCollatorForSeq2Seq(
             self.tokenizer,
```

### Comparing `textgen-1.0.0/textgen/gpt/gpt_utils.py` & `textgen-1.0.1/textgen/gpt/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/gpt/merge_peft_adapter.py` & `textgen-1.0.1/textgen/gpt/merge_peft_adapter.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/language_generation/language_generation_model.py` & `textgen-1.0.1/textgen/language_generation/language_generation_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/language_generation/language_generation_utils.py` & `textgen-1.0.1/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/language_modeling/language_modeling_model.py` & `textgen-1.0.1/textgen/language_modeling/language_modeling_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/language_modeling/language_modeling_utils.py` & `textgen-1.0.1/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/language_modeling/songnet_model.py` & `textgen-1.0.1/textgen/language_modeling/songnet_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/language_modeling/songnet_utils.py` & `textgen-1.0.1/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-1.0.1/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-1.0.1/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-1.0.1/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/seq2seq/data_reader.py` & `textgen-1.0.1/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/seq2seq/seq2seq_model.py` & `textgen-1.0.1/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/seq2seq/seq2seq_trainer.py` & `textgen-1.0.1/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/t5/copyt5_model.py` & `textgen-1.0.1/textgen/t5/copyt5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/t5/copyt5_utils.py` & `textgen-1.0.1/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/t5/t5_model.py` & `textgen-1.0.1/textgen/t5/t5_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/t5/t5_utils.py` & `textgen-1.0.1/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/unsup_generation/tgls_model.py` & `textgen-1.0.1/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen/unsup_generation/tgls_util.py` & `textgen-1.0.1/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-1.0.0/textgen.egg-info/PKG-INFO` & `textgen-1.0.1/textgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 1.0.0
+Version: 1.0.1
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [**🇨🇳中文**](https://github.com/shibing624/textgen/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/textgen/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: textgen Version: 1.0.0 Summary: Text Generation
+Metadata-Version: 2.1 Name: textgen Version: 1.0.1 Summary: Text Generation
 Model Home-page: https://github.com/shibing624/textgen Author: XuMing Author-
 email: xuming624@qq.com License: Apache 2.0 Description: [**ð¨ð³ä¸­æ**]
 (https://github.com/shibing624/textgen/blob/main/README.md) | [**ðEnglish**]
 (https://github.com/shibing624/textgen/blob/main/README_EN.md) | [**ðææ¡£/
 Docs**](https://github.com/shibing624/textgen/wiki) | [**ð¤æ¨¡å/Models**]
 (https://huggingface.co/shibing624)
                                     [Logo]
```

### Comparing `textgen-1.0.0/textgen.egg-info/SOURCES.txt` & `textgen-1.0.1/textgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

