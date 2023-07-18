# Comparing `tmp/seqslab-cli-3.2.1.post0.tar.gz` & `tmp/seqslab-cli-3.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-cli-3.2.1.post0.tar", last modified: Mon Jun 12 02:43:09 2023, max compression
+gzip compressed data, was "seqslab-cli-3.2.2a0.tar", last modified: Tue Jul 18 06:57:32 2023, max compression
```

## Comparing `seqslab-cli-3.2.1.post0.tar` & `seqslab-cli-3.2.2a0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.857089 seqslab-cli-3.2.1.post0/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/auth/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/drs/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    38488 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/role/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/role/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/runsheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/runsheet/runsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/session_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/statusbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/usage_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/user/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.270305 seqslab-cli-3.2.2a0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.274305 seqslab-cli-3.2.2a0/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.274305 seqslab-cli-3.2.2a0/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/runsheet/runsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.278305 seqslab-cli-3.2.2a0/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/wes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.282305 seqslab-cli-3.2.2a0/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-18 06:57:32.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:57:31.000000 seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-18 06:57:32.286305 seqslab-cli-3.2.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 06:57:18.000000 seqslab-cli-3.2.2a0/setup.py
```

### Comparing `seqslab-cli-3.2.1.post0/LICENSE` & `seqslab-cli-3.2.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/__init__.py` & `seqslab-cli-3.2.2a0/python/seqslab/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 name = "seqslab"
 
 __all__ = [
 
 ]
 
 
-__version__ = "3.2.1.post0"
+__version__ = "3.2.2a0"
 
 LOGGING = {
     "DIR_PATH": "/var/log/seqslab"
 }
```

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/auth/azuread.py` & `seqslab-cli-3.2.2a0/python/seqslab/auth/azuread.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/auth/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/auth/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
             assertion = Auth.tokens["tokens"].get('access')
             credential = Auth.tokens["attrs"].get("scrt")
         else:
             # load from Keyring secret service
             assertion = keyring.get_password("net.seqslab.api.tokens.access", user)
             if not assertion:
                 cprint("Not signed in yet")
-                return errno.EAUTH
+                return errno.EPERM
             credential = Auth._decode(assertion).get("scrt")
 
         if not credential:
             cprint("Not signed in for daemon process")
             return errno.EINVAL
 
         try:
```

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/cli.py` & `seqslab-cli-3.2.2a0/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/context.py` & `seqslab-cli-3.2.2a0/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/api/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,51 +579,80 @@
                 "contents": drs_ids
             }]
 
         results = backend.create_drsobjects(drs_type='bundle', payloads=payloads)
 
         return results
 
-    @command(aliases=["clean"])
+    @command(aliases=["unregister"])
     @argument("ids",
               type=List[str],
               positional=False,
-              description="Specify the IDs of the DRS object that you want to delete "
+              description="Specify the IDs of the DRS objects that you want to delete "
                           "(optional).")
     @argument("names",
               type=List[str],
               positional=False,
-              description="Specify the names of the DRS object that you want to delete "
+              description="Specify the names of the DRS objects that you want to delete "
                           "(optional).")
     @argument("tags",
               type=List[str],
               positional=False,
-              description="Specify the labels of the DRS object that you want to delete "
+              description="Specify the labels of the DRS objects that you want to delete "
+                          "(optional).")
+    def unregister(
+            self,
+            ids: List[str] = [],
+            tags: List[str] = [],
+            names: List[str] = [],
+    ) -> int:
+        """
+        Unregister DRS objects by DRS ID, DRS name, or DRS tag.
+        """
+        if not ids and not names and not tags:
+            cprint("Must specify one of the IDs, names or tags to identify DRS objects for deletion", "red")
+            return errno.ENOENT
+
+        resps = asyncio.run(utils.drs_delete(ids, names, tags, query_opts=f"?backend_content=false"))
+        for r in resps:
+            print(r)
+
+        return 0
+
+    @command(aliases=["clean"])
+    @argument("ids",
+              type=List[str],
+              positional=False,
+              description="Specify the IDs of the DRS objects that you want to delete "
                           "(optional).")
-    @argument("backend_resource",
-              type=str,
+    @argument("names",
+              type=List[str],
               positional=False,
-              description="Specify whether or not you want to delete the associated computing resources (default = true, optional).",
-              aliases=["purge"],
-              choices=['true', 'false'])
+              description="Specify the names of the DRS objects that you want to delete "
+                          "(optional).")
+    @argument("tags",
+              type=List[str],
+              positional=False,
+              description="Specify the labels of the DRS objects that you want to delete "
+                          "(optional).")
     def delete(
             self,
             ids: List[str] = [],
             tags: List[str] = [],
             names: List[str] = [],
-            backend_resource: str = "true"
     ) -> int:
         """
-        Delete DRS objects by DRS id, by DRS name or by DRS tag.
+        Delete DRS objects and the associated files in cloud storage by DRS ID, DRS name, or DRS tag.
         """
         if not ids and not names and not tags:
-            cprint("Must specify one of the ids, names or tags to identify DRS objects for deletion", "red")
+            cprint("Must specify one of the IDs, names or tags to identify "
+                   "the associated files in cloud storage of DRS objects for deletion", "red")
             return errno.ENOENT
 
-        resps = asyncio.run(utils.drs_delete(ids, names, tags, query_opts=f"?backend_content={backend_resource}"))
+        resps = asyncio.run(utils.drs_delete(ids, names, tags, query_opts=f"?backend_content=true"))
         for r in resps:
             print(r)
 
         return 0
 
     @command
     @argument("names",
```

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/aiocopy.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/internal/aiocopy.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/utils.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/biomimetype.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/progressbar.py` & `seqslab-cli-3.2.2a0/python/seqslab/drs/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/exceptions.py` & `seqslab-cli-3.2.2a0/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/organization/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/plugin.py` & `seqslab-cli-3.2.2a0/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/role/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/role/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/role/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/role/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/runsheet/runsheet.py` & `seqslab-cli-3.2.2a0/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/settings.py` & `seqslab-cli-3.2.2a0/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/statusbar.py` & `seqslab-cli-3.2.2a0/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,39 +169,44 @@
     @argument("descriptor_type",
               type=str,
               description="Specify the descriptor type of the tool that you want "
                           "to register in this version (required).",
               choices=["WDL", "CWL", "NFL"])
     @argument("images",
               type=str,
-              description="Specify a JSON string describing a list of images you want to register in this version "
-                          "(required).", )
+              description="Specify a JSON string describing a list of images that you want "
+                          "to register in this version (required).", )
     @argument("author",
               type=List[str],
-              description="Specify the name of the author of the tool that you want "
+              description="Specify the author of the tool that you want "
                           "to register in this version (optional).", )
     @argument("verified",
               type=bool,
-              description="Specify whether or not this version of the tool that you want "
-                          "to register is verified (optional, default = false).", )
+              description="Specify whether or not the version of the tool that you want "
+                          "to register is verified (optional, default = false)."
+                          "For example, CLI mode: verified=True/False, "
+                          "Interactive mode: --verified or no value specified.", )
     @argument("verified_source",
               type=List[str],
               description="Specify the verified source of the tool that you want "
                           "to register in this version (optional).", )
     @argument("included_apps",
               type=List[str],
-              description="Specify the apps that you want to include with the tool that you want "
-                          "to register in this version (optional).", )
+              description="Specify the apps to be included with the tool that you want "
+                          "to register in this version (optional)."
+                          "For example, CLI mode: --included-apps app1 app2 app3, ..., " 
+                          "Interactive mode: included_apps=['app1', 'app2', ...]", )
     @argument("signed",
               type=bool,
               description="Specify whether or not this version of the tool that you want "
-                          "to register is signed (optional, default = false).", )
+                          "to register is signed (optional, default = false)."
+                          "For example, Interactive mode: signed=True/False, CLI mode: given --signed or not given.", )
     @argument("is_production",
               type=bool,
-              description="Specify whether or not this version of the tool that you want "
+              description="Specify whether or not the version of the tool that you want "
                           "to register is for production use (optional, default = false).", )
     def version(self, workspace: str, tool_id: str, id: str, descriptor_type: str, images: str,
                 name: str = "", **kwargs) -> int:
         """
             Register TRS version object.
         """
         if not workspace:
@@ -386,26 +391,54 @@
 
     @command
     @argument("output",
               type=str,
               positional=False,
               description="Specify the output format of the stdout file (optional, default = json).",
               choices=['json', 'table'])
-    def list(self, output='json') -> int:
+    @argument("page",
+              type=int,
+              positional=False,
+              description="Specify the page number in the set of paginated records (optional, default = 1).")
+    @argument("page_size",
+              type=int,
+              positional=False,
+              description="Specify the number of records to return in each page (optional, default = 10).")
+    @argument("tool_id",
+              type=str,
+              positional=False,
+              description="Specify the ID of each tool version (required).")
+    def list(self, tool_id: str = None, page: int = 1, page_size: int = 10, output='json') -> int:
         """
-            Display a list of existing tools.
+            If tool_id is specified, available versions of the tool are returned. If unspecified, a list of registered tools is returned.
         """
-        try:
-            backend = trs_register().load_resource()
-            r = backend.get_tool()
-            BaseTools._stdout(r['results'], output)
-            return 0
-        except Exception as error:
-            cprint(f"{error}", "red")
-            return errno.ESRCH
+        if tool_id:
+            if page or page_size:
+                cprint("WARNING: page and page_size do not affect the list version.", 'yellow')
+            r = self._list_version(tool_id)
+        else:
+            r = self._list_tool(page=page, page_size=page_size)
+
+        if isinstance(r, int):
+            return r
+
+        self._stdout(r['results'], output)
+        return 0
+
+    @staticmethod
+    @exception_handler
+    def _list_tool(page: int, page_size: int):
+        backend = trs_register().load_resource()
+        return backend.list_tool(page, page_size)
+
+    @staticmethod
+    @exception_handler
+    def _list_version(tool_id: str):
+        backend = trs_register().load_resource()
+        return backend.list_version(tool_id)
 
     @command
     @argument("tool_id",
               type=str,
               description="Specify a TRS ID (required).")
     @argument("version_id",
               type=str,
```

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/utils.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from seqslab.auth.commands import BaseAuth
 from seqslab.trs import __version__, API_HOSTNAME
 from abc import ABC
 from tenacity import retry, wait_fixed, stop_after_attempt
 from .template import get_template
 import os
 from nubia import context
-
+from yarl import URL
 
 class TRSregister(ABC):
     logger = logging.getLogger()
 
     TRS_TOOL_URL = f"https://{API_HOSTNAME}/trs/{__version__}/tools/?backend={{backend}}"
     TRS_TOOL_URL_SPEC = f"https://{API_HOSTNAME}/trs/{__version__}/tools/{{tool_id}}?backend={{backend}}"
     TRS_TOOLVERSION_URL = f"https://{API_HOSTNAME}/trs/{__version__}/tools/{{tool_id}}/versions/?backend={{backend}}"
@@ -130,23 +130,40 @@
     def register():
         try:
             return 0
         except Exception as error:
             raise error
 
     @staticmethod
-    def get_tool():
+    def list_tool(page:int, page_size:int):
+        try:
+            ctx = context.get_context()
+            backend = ctx.args.backend
+            token = BaseAuth.get_token().get("tokens").get("access")
+        except KeyError:
+            raise KeyError(f"No tokens, Please signin first!")
+        url = URL(TRSregister.TRS_TOOL_URL.format(backend=backend)).update_query({"page": page, "page_size": page_size})
+        with requests.get(url=str(url),
+                          headers={"Authorization": f"Bearer {token}"},
+                          stream=True
+                          ) as response:
+            if response.status_code not in [requests.codes.ok]:
+                raise requests.HTTPError(f"{response.status_code}: {repr(response.text)}")
+            return response.json()
+
+    @staticmethod
+    def list_version(tool_id: str):
         try:
             ctx = context.get_context()
             backend = ctx.args.backend
             token = BaseAuth.get_token().get("tokens").get("access")
         except KeyError:
             raise KeyError(f"No tokens, Please signin first!")
 
-        with requests.get(url=TRSregister.TRS_TOOL_URL.format(backend=backend),
+        with requests.get(url=TRSregister.TRS_TOOLVERSION_URL.format(tool_id=tool_id, backend=backend),
                           headers={"Authorization": f"Bearer {token}"},
                           stream=True
                           ) as response:
             if response.status_code not in [requests.codes.ok]:
                 raise requests.HTTPError(f"{response.status_code}: {repr(response.text)}")
             return response.json()
```

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/register/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/template/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/trs/template/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/usage_logger.py` & `seqslab-cli-3.2.2a0/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/user/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
+import errno
 import json
 import webbrowser
 from typing import List
 
 from nubia import argument
 from nubia import command
-from termcolor import cprint
 from seqslab.exceptions import exception_handler
+from termcolor import cprint
 
 from .internal.common import get_factory
 
 """
 Copyright (C) 2022, Atgenomix Incorporated.
 
 All Rights Reserved.
@@ -108,30 +109,30 @@
               type=str,
               positional=False,
               description="Specify the email account that is going to be added as a SeqsLab user account (required).")
     @argument("roles",
               type=List[str],
               positional=False,
               description="Specify the role the added user is going to be assigned to (required).")
-    @argument("active",
+    @argument("deactivate",
               type=bool,
               positional=False,
-              description="Specify whether or not to activate the registered user (optional, default = False).")
+              description="Specify whether or not to deactivate the created user (optional, default = False).")
     @argument("name",
               type=str,
               positional=False,
               description="Specify the user name that you want to use (optional).")
-    def add(self, email: str, roles: List[str] = [], active: bool = False, name: str = None) -> int:
+    def add(self, email: str, roles: List[str] = [], deactivate: bool = False, name: str = None) -> int:
         """
         Add a new user to the SeqsLab platform.
         """
         backend = get_factory().load_resource()
         ret = backend.add_user(email=email,
                                roles=roles,
-                               active=active,
+                               active=not deactivate,
                                name=name)
         if isinstance(ret, int):
             return ret
         cprint(json.dumps(ret, indent=4), 'yellow')
         return 0
 
     @command
@@ -143,39 +144,51 @@
               type=str,
               positional=False,
               description="The email account that is going to be added as a SeqsLab user account (optional).")
     @argument("roles",
               type=List[str],
               positional=False,
               description="Specify the role the user is going to be assigned to (optional).")
-    @argument("active",
+    @argument("activate",
               type=bool,
               positional=False,
               description="Specify whether or not to activate the registered user (optional).")
+    @argument("deactivate",
+              type=bool,
+              positional=False,
+              description="Specify whether or not to deactivate the registered user (optional).")
     @argument("name",
               type=str,
               positional=False,
               description="Specify the user name that you want to modify (optional).")
-    def update(self, id: str, email: str = None, roles: List[str] = [], active: bool = False,
-               name: str = None) -> int:
+    def update(self, id: str, email: str = None, roles: List[str] = [], activate: bool = False,
+               deactivate: bool = False, name: str = None) -> int:
         """
         Add a new user to the SeqsLab platform.
         """
         backend = get_factory().load_resource()
         payload = {}
         if email:
             payload['email'] = email
         if roles:
             payload['roles'] = roles
         if name:
             payload['name'] = name
-        if active:
+        if activate and not deactivate:
             payload['is_active'] = True
-        if not active:
+        elif deactivate and not activate:
             payload['is_active'] = False
+        elif activate and deactivate:
+            cprint("A user cannot be activated and deactivated at the same time", "red")
+            return errno.EINVAL
+
+        if not email and not roles and not activate and not deactivate and not name:
+            cprint("Specify at least one of the following parameters: email, roles, activate, deactivate, or name.",
+                   "red")
+            return errno.EINVAL
 
         ret = backend.patch_user(user_id=id,
                                  payload=payload)
         if isinstance(ret, int):
             return ret
         cprint(json.dumps(ret, indent=4), 'yellow')
         return 0
```

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/user/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/user/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/user/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/user/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/template/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/template/template.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/wes/utils.py` & `seqslab-cli-3.2.2a0/python/seqslab/wes/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/workspace/commands.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/common.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/azure.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/base.py` & `seqslab-cli-3.2.2a0/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/SOURCES.txt` & `seqslab-cli-3.2.2a0/python/seqslab_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1.post0/setup.py` & `seqslab-cli-3.2.2a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         'Programming Language :: Python :: 3.9',
         # https://pypi.org/pypi?%3Aaction=list_classifiers
     ],
     description="Atgenomix SeqsLab Command Line Tool",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/AnomeGAP/seqslab-cli",
-    license="MIT license",
+    license="Apache License, Version 2.0",
     packages=find_packages(where='python'),
     package_dir={'': 'python'},
 
     include_package_data=True,
     install_requires=get_requirement(),
     extras_require=extras_require,
     python_requires='>=3.8',
```

