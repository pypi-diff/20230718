# Comparing `tmp/nope_py-1.7.8rc3.tar.gz` & `tmp/nope_py-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nope_py-1.7.8rc3.tar", last modified: Fri Jul 14 22:27:18 2023, max compression
+gzip compressed data, was "nope_py-1.7.9.tar", last modified: Tue Jul 18 08:25:01 2023, max compression
```

## Comparing `nope_py-1.7.8rc3.tar` & `nope_py-1.7.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/
--rw-r--r--   0 martin    (1000) martin    (1001)     1062 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1001)     8141 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1001)     7557 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/
--rw-r--r--   0 martin    (1000) martin    (1001)      525 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/cli/
--rw-r--r--   0 martin    (1000) martin    (1001)      458 2023-07-14 16:52:13.000000 nope_py-1.7.8rc3/nope/cli/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      121 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/cli/__main__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2309 2023-07-14 17:45:33.000000 nope_py-1.7.8rc3/nope/cli/logo.py
--rw-r--r--   0 martin    (1000) martin    (1001)      729 2023-07-14 16:54:17.000000 nope_py-1.7.8rc3/nope/cli/main.py
--rw-r--r--   0 martin    (1000) martin    (1001)     9578 2023-07-14 22:06:47.000000 nope_py-1.7.8rc3/nope/cli/run.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4669 2023-07-14 22:26:41.000000 nope_py-1.7.8rc3/nope/cli/scan.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/communication/
--rw-r--r--   0 martin    (1000) martin    (1001)      158 2023-07-14 21:32:17.000000 nope_py-1.7.8rc3/nope/communication/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1111 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/abstractBridgePlugin.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1633 2023-07-14 21:36:02.000000 nope_py-1.7.8rc3/nope/communication/addLayer.py
--rw-r--r--   0 martin    (1000) martin    (1001)     5498 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/bridge.py
--rw-r--r--   0 martin    (1000) martin    (1001)      450 2023-07-14 21:36:59.000000 nope_py-1.7.8rc3/nope/communication/getLayer.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/communication/layers/
--rw-r--r--   0 martin    (1000) martin    (1001)     2522 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/EventCommunicationInterface.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2896 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/IoSocketClientLayer.py
--rw-r--r--   0 martin    (1000) martin    (1001)      196 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      872 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/abstractLayer.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6122 2023-07-14 17:51:17.000000 nope_py-1.7.8rc3/nope/communication/layers/mqttLayer.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/decorators/
--rw-r--r--   0 martin    (1000) martin    (1001)       82 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/decorators/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1285 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/decorators/classes.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/demo/
--rw-r--r--   0 martin    (1000) martin    (1001)       93 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/demo/instances/
--rw-r--r--   0 martin    (1000) martin    (1001)     1474 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/instances/DecoratedHelloWorld.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1461 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/instances/HelloWorld.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1212 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/instances/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/demo/plugins/
--rw-r--r--   0 martin    (1000) martin    (1001)      936 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/00-load-hello.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2514 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/01-dynamic.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2933 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/02-multiple.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3176 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/03-different-items.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1224 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/04-fix.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/
--rw-r--r--   0 martin    (1000) martin    (1001)      355 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/baseServices/
--rw-r--r--   0 martin    (1000) martin    (1001)      909 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/baseServices/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2676 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/baseServices/connectivy.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/
--rw-r--r--   0 martin    (1000) martin    (1001)       57 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    12628 2023-07-14 16:31:06.000000 nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/connectivityManager.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/core/
--rw-r--r--   0 martin    (1000) martin    (1001)      110 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/core/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4897 2023-07-14 17:45:31.000000 nope_py-1.7.8rc3/nope/dispatcher/core/nopeCore.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2103 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/getDispatcher.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/
--rw-r--r--   0 martin    (1000) martin    (1001)      106 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      896 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/assignmentChecker.py
--rw-r--r--   0 martin    (1000) martin    (1001)    38653 2023-07-14 21:08:55.000000 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/instanceManager.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4289 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/nopeDispatcher.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/
--rw-r--r--   0 martin    (1000) martin    (1001)       79 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    23952 2023-07-14 17:45:32.000000 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/rpcManager.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3200 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/selectors.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/eventEmitter/
--rw-r--r--   0 martin    (1000) martin    (1001)       79 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/eventEmitter/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6492 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/eventEmitter/nopeEventEmitter.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/helpers/
--rw-r--r--   0 martin    (1000) martin    (1001)     2457 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    15786 2023-07-14 18:38:50.000000 nope_py-1.7.8rc3/nope/helpers/asyncHelpers.py
--rw-r--r--   0 martin    (1000) martin    (1001)    12082 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/dictMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)      695 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/dispatcherPathes.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4025 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/dottedDict.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4035 2023-07-14 17:45:29.000000 nope_py-1.7.8rc3/nope/helpers/emitter.py
--rw-r--r--   0 martin    (1000) martin    (1001)      805 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/files.py
--rw-r--r--   0 martin    (1000) martin    (1001)    11974 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/hashable.py
--rw-r--r--   0 martin    (1000) martin    (1001)      767 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/idMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)      591 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/importing.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2732 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/jsonMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2316 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/listMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)    14217 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/objectMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     5206 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/path.py
--rw-r--r--   0 martin    (1000) martin    (1001)    10488 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/pathMatchingMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)      610 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/prints.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1459 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/runtime.py
--rw-r--r--   0 martin    (1000) martin    (1001)      748 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/setMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4807 2023-07-14 17:45:30.000000 nope_py-1.7.8rc3/nope/helpers/stringMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1894 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/timers.py
--rw-r--r--   0 martin    (1000) martin    (1001)      119 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/timestamp.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/loader/
--rw-r--r--   0 martin    (1000) martin    (1001)      234 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/loader/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      748 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/loader/getPackageLoader.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2709 2023-07-14 21:44:22.000000 nope_py-1.7.8rc3/nope/loader/loadPackages.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6379 2023-07-14 16:41:06.000000 nope_py-1.7.8rc3/nope/loader/nopePackkageLoader.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/logger/
--rw-r--r--   0 martin    (1000) martin    (1001)       99 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/logger/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2436 2023-07-14 16:46:17.000000 nope_py-1.7.8rc3/nope/logger/logger.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/merging/
--rw-r--r--   0 martin    (1000) martin    (1001)       53 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/merging/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2293 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/merging/mergeData.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/modules/
--rw-r--r--   0 martin    (1000) martin    (1001)      206 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/modules/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    17745 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/modules/baseModule.py
--rw-r--r--   0 martin    (1000) martin    (1001)     7614 2023-07-14 17:59:08.000000 nope_py-1.7.8rc3/nope/modules/genericModule.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/observable/
--rw-r--r--   0 martin    (1000) martin    (1001)      151 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/observable/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3003 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/observable/nopeObservable.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/plugins/
--rw-r--r--   0 martin    (1000) martin    (1001)      125 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6051 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/ack_messages.py
--rw-r--r--   0 martin    (1000) martin    (1001)      919 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/hello.py
--rw-r--r--   0 martin    (1000) martin    (1001)    21800 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/plugin.py
--rw-r--r--   0 martin    (1000) martin    (1001)    16129 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/rpc_with_callbacks.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/pubSub/
--rw-r--r--   0 martin    (1000) martin    (1001)       94 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/pubSub/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3718 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/pubSub/nopeDataPubSubSystem.py
--rw-r--r--   0 martin    (1000) martin    (1001)    25149 2023-07-14 18:38:53.000000 nope_py-1.7.8rc3/nope/pubSub/nopePubSubSystem.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/types/
--rw-r--r--   0 martin    (1000) martin    (1001)     3358 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/types/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope_py.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1001)     8141 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1001)     3118 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1001)        1 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1001)       46 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/entry_points.txt
--rw-r--r--   0 martin    (1000) martin    (1001)       49 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1001)        5 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1001)      103 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1001)     2520 2023-07-14 22:27:13.000000 nope_py-1.7.8rc3/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/test/
--rw-r--r--   0 martin    (1000) martin    (1001)     1427 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2053 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_communicator.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2960 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_plugin.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1545 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_plugin_bridge.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1396 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_plugin_rpc_callbacks.py
--rw-r--r--   0 martin    (1000) martin    (1001)      644 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_pub_sub.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3128 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_rpc_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:01.110916 nope_py-1.7.9/
+-rw-rw-rw-   0        0        0     1083 2023-07-18 08:01:38.000000 nope_py-1.7.9/LICENSE
+-rw-rw-rw-   0        0        0     8428 2023-07-18 08:25:01.111838 nope_py-1.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7791 2023-07-18 08:01:38.000000 nope_py-1.7.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.431364 nope_py-1.7.9/nope/
+-rw-rw-rw-   0        0        0      525 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.462306 nope_py-1.7.9/nope/cli/
+-rw-rw-rw-   0        0        0      469 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/cli/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/cli/__main__.py
+-rw-rw-rw-   0        0        0     2336 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/cli/logo.py
+-rw-rw-rw-   0        0        0      763 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/cli/main.py
+-rw-rw-rw-   0        0        0     9860 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/cli/run.py
+-rw-rw-rw-   0        0        0     3816 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/cli/scan.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.498324 nope_py-1.7.9/nope/communication/
+-rw-rw-rw-   0        0        0      162 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/__init__.py
+-rw-rw-rw-   0        0        0     1154 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/abstractBridgePlugin.py
+-rw-rw-rw-   0        0        0     1671 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/addLayer.py
+-rw-rw-rw-   0        0        0     5691 2023-07-18 08:05:06.000000 nope_py-1.7.9/nope/communication/bridge.py
+-rw-rw-rw-   0        0        0      466 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/getLayer.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.526304 nope_py-1.7.9/nope/communication/layers/
+-rw-rw-rw-   0        0        0     2522 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/layers/EventCommunicationInterface.py
+-rw-rw-rw-   0        0        0     2896 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/layers/IoSocketClientLayer.py
+-rw-rw-rw-   0        0        0      200 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/layers/__init__.py
+-rw-rw-rw-   0        0        0      903 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/layers/abstractLayer.py
+-rw-rw-rw-   0        0        0     6122 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/communication/layers/mqttLayer.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.535598 nope_py-1.7.9/nope/decorators/
+-rw-rw-rw-   0        0        0       83 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/decorators/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/decorators/classes.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.543300 nope_py-1.7.9/nope/demo/
+-rw-rw-rw-   0        0        0       95 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.561303 nope_py-1.7.9/nope/demo/instances/
+-rw-rw-rw-   0        0        0     1524 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/instances/DecoratedHelloWorld.py
+-rw-rw-rw-   0        0        0     1510 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/instances/HelloWorld.py
+-rw-rw-rw-   0        0        0     1243 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/instances/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.597689 nope_py-1.7.9/nope/demo/plugins/
+-rw-rw-rw-   0        0        0      977 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/plugins/00-load-hello.py
+-rw-rw-rw-   0        0        0     2597 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/plugins/01-dynamic.py
+-rw-rw-rw-   0        0        0     3031 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/plugins/02-multiple.py
+-rw-rw-rw-   0        0        0     3284 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/plugins/03-different-items.py
+-rw-rw-rw-   0        0        0     1264 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/demo/plugins/04-fix.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.611307 nope_py-1.7.9/nope/dispatcher/
+-rw-rw-rw-   0        0        0      362 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.622310 nope_py-1.7.9/nope/dispatcher/baseServices/
+-rw-rw-rw-   0        0        0      943 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/baseServices/__init__.py
+-rw-rw-rw-   0        0        0     2772 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/baseServices/connectivy.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.635311 nope_py-1.7.9/nope/dispatcher/connectivityManager/
+-rw-rw-rw-   0        0        0       58 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/connectivityManager/__init__.py
+-rw-rw-rw-   0        0        0    13002 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/connectivityManager/connectivityManager.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.653501 nope_py-1.7.9/nope/dispatcher/core/
+-rw-rw-rw-   0        0        0      115 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/core/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/core/nopeCore.py
+-rw-rw-rw-   0        0        0     2175 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/getDispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.675613 nope_py-1.7.9/nope/dispatcher/instanceManager/
+-rw-rw-rw-   0        0        0      108 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/instanceManager/__init__.py
+-rw-rw-rw-   0        0        0      929 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/instanceManager/assignmentChecker.py
+-rw-rw-rw-   0        0        0    39609 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/instanceManager/instanceManager.py
+-rw-rw-rw-   0        0        0     4399 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/nopeDispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.692303 nope_py-1.7.9/nope/dispatcher/rpcManager/
+-rw-rw-rw-   0        0        0       81 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/rpcManager/__init__.py
+-rw-rw-rw-   0        0        0    24614 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/rpcManager/rpcManager.py
+-rw-rw-rw-   0        0        0     3309 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/dispatcher/rpcManager/selectors.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.706304 nope_py-1.7.9/nope/eventEmitter/
+-rw-rw-rw-   0        0        0       82 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/eventEmitter/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/eventEmitter/nopeEventEmitter.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.870304 nope_py-1.7.9/nope/helpers/
+-rw-rw-rw-   0        0        0     2457 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/__init__.py
+-rw-rw-rw-   0        0        0    16265 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/asyncHelpers.py
+-rw-rw-rw-   0        0        0    12446 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/dictMethods.py
+-rw-rw-rw-   0        0        0      720 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/dispatcherPathes.py
+-rw-rw-rw-   0        0        0     4166 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/dottedDict.py
+-rw-rw-rw-   0        0        0     4035 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/emitter.py
+-rw-rw-rw-   0        0        0      836 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/files.py
+-rw-rw-rw-   0        0        0    12428 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/hashable.py
+-rw-rw-rw-   0        0        0      793 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/idMethods.py
+-rw-rw-rw-   0        0        0      617 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/importing.py
+-rw-rw-rw-   0        0        0     2821 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/jsonMethods.py
+-rw-rw-rw-   0        0        0     2411 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/listMethods.py
+-rw-rw-rw-   0        0        0    14752 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/objectMethods.py
+-rw-rw-rw-   0        0        0     5206 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/path.py
+-rw-rw-rw-   0        0        0    10739 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/pathMatchingMethods.py
+-rw-rw-rw-   0        0        0      610 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/prints.py
+-rw-rw-rw-   0        0        0     1459 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/runtime.py
+-rw-rw-rw-   0        0        0      778 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/setMethods.py
+-rw-rw-rw-   0        0        0     4999 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/stringMethods.py
+-rw-rw-rw-   0        0        0     1894 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/timers.py
+-rw-rw-rw-   0        0        0      119 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/helpers/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.892552 nope_py-1.7.9/nope/loader/
+-rw-rw-rw-   0        0        0      241 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/loader/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/loader/getPackageLoader.py
+-rw-rw-rw-   0        0        0     2797 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/loader/loadPackages.py
+-rw-rw-rw-   0        0        0     6539 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/loader/nopePackkageLoader.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.902371 nope_py-1.7.9/nope/logger/
+-rw-rw-rw-   0        0        0      100 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/logger/__init__.py
+-rw-rw-rw-   0        0        0     2526 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.913355 nope_py-1.7.9/nope/merging/
+-rw-rw-rw-   0        0        0       54 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/merging/__init__.py
+-rw-rw-rw-   0        0        0     2359 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/merging/mergeData.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.932303 nope_py-1.7.9/nope/modules/
+-rw-rw-rw-   0        0        0      214 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/modules/__init__.py
+-rw-rw-rw-   0        0        0    18241 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/modules/baseModule.py
+-rw-rw-rw-   0        0        0     7829 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/modules/genericModule.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.946304 nope_py-1.7.9/nope/observable/
+-rw-rw-rw-   0        0        0      157 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/observable/__init__.py
+-rw-rw-rw-   0        0        0     3097 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/observable/nopeObservable.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:00.979301 nope_py-1.7.9/nope/plugins/
+-rw-rw-rw-   0        0        0      129 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/plugins/__init__.py
+-rw-rw-rw-   0        0        0     6213 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/plugins/ack_messages.py
+-rw-rw-rw-   0        0        0      946 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/plugins/hello.py
+-rw-rw-rw-   0        0        0    22410 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/plugins/plugin.py
+-rw-rw-rw-   0        0        0    16526 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/plugins/rpc_with_callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:01.009103 nope_py-1.7.9/nope/pubSub/
+-rw-rw-rw-   0        0        0       96 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/pubSub/__init__.py
+-rw-rw-rw-   0        0        0     3810 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/pubSub/nopeDataPubSubSystem.py
+-rw-rw-rw-   0        0        0    25800 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/pubSub/nopePubSubSystem.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:01.015844 nope_py-1.7.9/nope/types/
+-rw-rw-rw-   0        0        0     3468 2023-07-18 08:01:38.000000 nope_py-1.7.9/nope/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:01.058849 nope_py-1.7.9/nope_py.egg-info/
+-rw-rw-rw-   0        0        0     8428 2023-07-18 08:25:00.000000 nope_py-1.7.9/nope_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3118 2023-07-18 08:25:00.000000 nope_py-1.7.9/nope_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:25:00.000000 nope_py-1.7.9/nope_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-18 08:25:00.000000 nope_py-1.7.9/nope_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-07-18 08:25:00.000000 nope_py-1.7.9/nope_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-18 08:25:00.000000 nope_py-1.7.9/nope_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-07-18 08:25:01.114839 nope_py-1.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     2517 2023-07-18 08:06:19.000000 nope_py-1.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:25:01.105838 nope_py-1.7.9/test/
+-rw-rw-rw-   0        0        0     1427 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test.py
+-rw-rw-rw-   0        0        0     2144 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test_communicator.py
+-rw-rw-rw-   0        0        0     3047 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test_plugin.py
+-rw-rw-rw-   0        0        0     1606 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test_plugin_bridge.py
+-rw-rw-rw-   0        0        0     1454 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test_plugin_rpc_callbacks.py
+-rw-rw-rw-   0        0        0      682 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test_pub_sub.py
+-rw-rw-rw-   0        0        0     3254 2023-07-18 08:01:38.000000 nope_py-1.7.9/test/test_rpc_manager.py
```

### Comparing `nope_py-1.7.8rc3/LICENSE` & `nope_py-1.7.9/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) ZeMA gGmbH
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) ZeMA gGmbH
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nope_py-1.7.8rc3/PKG-INFO` & `nope_py-1.7.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,251 +1,235 @@
-Metadata-Version: 2.1
-Name: nope_py
-Version: 1.7.8rc3
-Summary: NOPE-Lib represents the No Programming Environment Library for python.
-Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
-Author: Martin Karkowski
-Author-email: m.karkowski@zema.de
-Maintainer: Martin Karkowski
-Maintainer-email: m.karkowski@zema.de
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NoPE 
-
-## A Python wrapper for the Library
-
-Please visit our [Docu](https://zema-ggmbh.github.io/NoPE-Docs/)
-
-## Show me `NoPE` in 5 Minutes! 
-
-### 1. Create a `Nodejs` Project
-
-Get started by **creating a new project** distributed using `NoPE`.
-
-For our **PYTHON** project we will use the nope-js-node cli tools to create a Project.
-
-1. Installation using  npm:
-  ```bash
-  npm install -g nope-js-node
-  ```
-2. Start your first Project:
-  ```bash
-  nope-js project create
-  ```
-  This should open a `cli`.
-
-3. Answer the requried questions to complete create the directory.
-  - Name the project `HelloWorld`
-  - Give it a short summary. This summary will used during distributing your project.
-  - make shure you select `python` as project type    
-
-4. navigate to the create folder ( e.g. `cd ./HelloWorld` ) 
-
-  This creates a project structure.
-
-5. Open your IDE (e.g. vscode)
-
-By using the project-tool the following features are added to the project:
-- Debugging of the application using VS code (launch-file)
-- Creation of a doc file (see doc/make)
-- Helpers to build a browser related version
-- Use of a changelog
-- Deployment as a package
-- Simple extension using project-tool
-
-## 2. Add a Service in `Python`
-
-Our goal is to define a greeting service
-> The service creates a greeting message for a person. 
-
-### Why a Service
-
-> This service is independent of how many times it has been called.
-> Our functionality is stateless, this allows us to use a service.
-
-### Using the `CLI` to generate the Service
-
-1. To create the Service: 
-  use the `project-tool` to create the service 
-
-  ```bash
-  nope-js project edit
-  ```
-
-2. Perfom the following selection inside of the tool.
-  1. Selection `add`, to add a new element
-  2. Select `service`, because we want to create a service
-  3. Enter the name of the service, in our case `HelloWorld`
-  
-  Creation of the corresponding files and imports is done automatically
-
-  This will update our project folder.
-
-Now `NoPE` defined a new service file (`HelloWorldFunctions.py`) for us:
-
-```python
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from nope import getNopeLogger
-
-LOGGER = getNopeLogger("HelloWorldService")
-
-# Please provide the schema for the Function.
-# See the Example below.
-SCHEMA = {
-    "type": "function",
-        
-    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
-    # It contains a list of all required inputs.
-    "inputs": [
-    ],
-    # To describe the return of a function we added the field "outputs". It contains a 
-    # JSON-Schema Object.
-    "outputs":{
-    }
-}
-
-async def HelloWorld(greetings: str):
-    # Please overwrite me!
-    LOGGER.debug("calling service 'HelloWorld' with the following parameters:" + str(greetings))
-    return "Hello " + greetings + "!"
-```
-
-In that file, you will find a template for the service we want to implement. By default, the newly created service implements the hello-world behavior. This must changed. In our case it matches the desired behavior.
-
-
-> All services **must** be implemented `async` manner. This is necessary so that the runtime is not blocked.
-
-
-### Adding a Service interface
-
-We now want to describe our service, that it can be used correctly at different Runtimes. Therefore we will define the `schema` to the `SCHEMA` variable. This Schema follows the definition of a `JSON-Schema`:
-
-```python
-SCHEMA = {
-    "type": "function",
-        
-    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
-    # It contains a list of all required inputs.
-    "inputs": [
-        {
-            # The Description of the Parameter
-            "description": "The name which should receive a Greeting",
-            # Its used name in the function (see the arguments of the function)
-            "name": "greetings",
-            # The Schema follows a default JSON-Schema
-            "schema": {
-                "type": "string"
-            }
-        }
-    ],
-    # To describe the return of a function we added the field "outputs". It contains a 
-    # JSON-Schema Object.
-    "outputs":{
-        "type": "string",
-
-        # We provide some extra Info for the other users.
-        "description": "The greeting Message!"
-    }
-}
-```
-
-Because the python implementation is lacking some typings please checkout the docs
-
-## 3. Running the Service:
-
-To run the `service` and distribute to different `NoPE`-Runtimes we have to determine a configuration:
-
-```bash
-nope-py scan
-```
-The `cli` will find all defined `services` or `modules` exposed in a so called `NoPE-Package` (This has been created automatically during the initalization of the project). The tool will store its results in the following configuration (located at `./config/config.json`):
-
-```json
-[
-    {
-        "nameOfPackage": "HelloWorld",
-        "autostart": {},
-        "defaultInstances": [],
-        "providedServices": [
-            {
-                "options": {
-                    "schema": {
-                        ...
-                    },
-                    "resultSink": null,
-                    "timeout": -1,
-                    "id": "HelloWorld",
-                    "ui": {
-                        "file": false,
-                        "autoGenBySchema": false,
-                        "requiredProvidersForRendering": []
-                    },
-                    "isDynamic": false
-                }
-            }
-        ],
-        "providedClasses": [],
-        "requiredPackages": [],
-        "path": "C:\\Users\\m.karkowski\\Documents\\00-Repos\\TEST\\HelloWorld\\HelloWorld\\__init__.py"
-    }
-]
-```
-
-Finally we are ready to distribute our service by using the command:
-
-```bash
-nope-py run
-```
-
-This will start a runtime providing our service.
-
-## 4. Interact with the Runtime
-
-Currently our service is only run internally (nope is not connected and runs without an external connection layer). To check and play with the distribution, we kill our old process (`ctrl+c`) create a separate process (e.g. a bash) and provide a serve:
-
-```bash
-nope-js run -c io-server
-```
-
-This will spool up a `socket-io` server on our localhost. 
-
-Afterwards we will restart our Runtime hosting the created service using `io-sockets` as connection layer:
-
-```bash
-nope-py run -c io-client
-```
-
-Now we are able to start our `interact-tool` to manually execute our process:
-
-```bash
-nope-js interact -c io-client -s
-```
-
-To use the `interact`-**tool** follow the questions:
-
-1. What do you want to do?
-    - We want to inspect our distributed system -> `inspect`
-2. What do you want to inspect?
-    - We want to check if our service is present -> `service`
-    - We should be albe to see our `HelloWorld`-Service (see 1)
-3. Now we want to execute this service. Therefore we navigate `back` to the main menu
-4. Now we select `execute` and afterwards `service` because we want to execute our service
-5. Now the Tool renders the available services and we select `HelloWorld` (see 2) and it will render the previously defined Schema.
-6. Now we have to enter the inputs required by the Service:
-    - It is important that the parameters are entered as list (because there might be more the 1 Parameter)
-    - Enter the parameters as valid `JSON` Data.
-    - Press `enter`
-
-    > Executing services with the interact tool will perfom function immedialty. If you integrated Hardware be aware of that.
-
-7. The Tool shows the result (see 4)
-
-
-> You are now running a distributed System using **remote procedure calls** in ***python***
+# NoPE 
+
+## A Python wrapper for the Library
+
+Please visit our [Docu](https://zema-ggmbh.github.io/NoPE-Docs/)
+
+## Show me `NoPE` in 5 Minutes! 
+
+### 1. Create a `Nodejs` Project
+
+Get started by **creating a new project** distributed using `NoPE`.
+
+For our **PYTHON** project we will use the nope-js-node cli tools to create a Project.
+
+1. Installation using  npm:
+  ```bash
+  npm install -g nope-js-node
+  ```
+2. Start your first Project:
+  ```bash
+  nope-js project create
+  ```
+  This should open a `cli`.
+
+3. Answer the requried questions to complete create the directory.
+  - Name the project `HelloWorld`
+  - Give it a short summary. This summary will used during distributing your project.
+  - make shure you select `python` as project type    
+
+4. navigate to the create folder ( e.g. `cd ./HelloWorld` ) 
+
+  This creates a project structure.
+
+5. Open your IDE (e.g. vscode)
+
+By using the project-tool the following features are added to the project:
+- Debugging of the application using VS code (launch-file)
+- Creation of a doc file (see doc/make)
+- Helpers to build a browser related version
+- Use of a changelog
+- Deployment as a package
+- Simple extension using project-tool
+
+## 2. Add a Service in `Python`
+
+Our goal is to define a greeting service
+> The service creates a greeting message for a person. 
+
+### Why a Service
+
+> This service is independent of how many times it has been called.
+> Our functionality is stateless, this allows us to use a service.
+
+### Using the `CLI` to generate the Service
+
+1. To create the Service: 
+  use the `project-tool` to create the service 
+
+  ```bash
+  nope-js project edit
+  ```
+
+2. Perfom the following selection inside of the tool.
+  1. Selection `add`, to add a new element
+  2. Select `service`, because we want to create a service
+  3. Enter the name of the service, in our case `HelloWorld`
+  
+  Creation of the corresponding files and imports is done automatically
+
+  This will update our project folder.
+
+Now `NoPE` defined a new service file (`HelloWorldFunctions.py`) for us:
+
+```python
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from nope import getNopeLogger
+
+LOGGER = getNopeLogger("HelloWorldService")
+
+# Please provide the schema for the Function.
+# See the Example below.
+SCHEMA = {
+    "type": "function",
+        
+    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
+    # It contains a list of all required inputs.
+    "inputs": [
+    ],
+    # To describe the return of a function we added the field "outputs". It contains a 
+    # JSON-Schema Object.
+    "outputs":{
+    }
+}
+
+async def HelloWorld(greetings: str):
+    # Please overwrite me!
+    LOGGER.debug("calling service 'HelloWorld' with the following parameters:" + str(greetings))
+    return "Hello " + greetings + "!"
+```
+
+In that file, you will find a template for the service we want to implement. By default, the newly created service implements the hello-world behavior. This must changed. In our case it matches the desired behavior.
+
+
+> All services **must** be implemented `async` manner. This is necessary so that the runtime is not blocked.
+
+
+### Adding a Service interface
+
+We now want to describe our service, that it can be used correctly at different Runtimes. Therefore we will define the `schema` to the `SCHEMA` variable. This Schema follows the definition of a `JSON-Schema`:
+
+```python
+SCHEMA = {
+    "type": "function",
+        
+    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
+    # It contains a list of all required inputs.
+    "inputs": [
+        {
+            # The Description of the Parameter
+            "description": "The name which should receive a Greeting",
+            # Its used name in the function (see the arguments of the function)
+            "name": "greetings",
+            # The Schema follows a default JSON-Schema
+            "schema": {
+                "type": "string"
+            }
+        }
+    ],
+    # To describe the return of a function we added the field "outputs". It contains a 
+    # JSON-Schema Object.
+    "outputs":{
+        "type": "string",
+
+        # We provide some extra Info for the other users.
+        "description": "The greeting Message!"
+    }
+}
+```
+
+Because the python implementation is lacking some typings please checkout the docs
+
+## 3. Running the Service:
+
+To run the `service` and distribute to different `NoPE`-Runtimes we have to determine a configuration:
+
+```bash
+nope-py scan
+```
+The `cli` will find all defined `services` or `modules` exposed in a so called `NoPE-Package` (This has been created automatically during the initalization of the project). The tool will store its results in the following configuration (located at `./config/config.json`):
+
+```json
+[
+    {
+        "nameOfPackage": "HelloWorld",
+        "autostart": {},
+        "defaultInstances": [],
+        "providedServices": [
+            {
+                "options": {
+                    "schema": {
+                        ...
+                    },
+                    "resultSink": null,
+                    "timeout": -1,
+                    "id": "HelloWorld",
+                    "ui": {
+                        "file": false,
+                        "autoGenBySchema": false,
+                        "requiredProvidersForRendering": []
+                    },
+                    "isDynamic": false
+                }
+            }
+        ],
+        "providedClasses": [],
+        "requiredPackages": [],
+        "path": "C:\\Users\\m.karkowski\\Documents\\00-Repos\\TEST\\HelloWorld\\HelloWorld\\__init__.py"
+    }
+]
+```
+
+Finally we are ready to distribute our service by using the command:
+
+```bash
+nope-py run
+```
+
+This will start a runtime providing our service.
+
+## 4. Interact with the Runtime
+
+Currently our service is only run internally (nope is not connected and runs without an external connection layer). To check and play with the distribution, we kill our old process (`ctrl+c`) create a separate process (e.g. a bash) and provide a serve:
+
+```bash
+nope-js run -c io-server
+```
+
+This will spool up a `socket-io` server on our localhost. 
+
+Afterwards we will restart our Runtime hosting the created service using `io-sockets` as connection layer:
+
+```bash
+nope-py run -c io-client
+```
+
+Now we are able to start our `interact-tool` to manually execute our process:
+
+```bash
+nope-js interact -c io-client -s
+```
+
+To use the `interact`-**tool** follow the questions:
+
+1. What do you want to do?
+    - We want to inspect our distributed system -> `inspect`
+2. What do you want to inspect?
+    - We want to check if our service is present -> `service`
+    - We should be albe to see our `HelloWorld`-Service (see 1)
+3. Now we want to execute this service. Therefore we navigate `back` to the main menu
+4. Now we select `execute` and afterwards `service` because we want to execute our service
+5. Now the Tool renders the available services and we select `HelloWorld` (see 2) and it will render the previously defined Schema.
+6. Now we have to enter the inputs required by the Service:
+    - It is important that the parameters are entered as list (because there might be more the 1 Parameter)
+    - Enter the parameters as valid `JSON` Data.
+    - Press `enter`
+
+    > Executing services with the interact tool will perfom function immedialty. If you integrated Hardware be aware of that.
+
+7. The Tool shows the result (see 4)
+
+
+> You are now running a distributed System using **remote procedure calls** in ***python***
```

### Comparing `nope_py-1.7.8rc3/README.md` & `nope_py-1.7.9/nope_py.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,235 +1,254 @@
-# NoPE 
-
-## A Python wrapper for the Library
-
-Please visit our [Docu](https://zema-ggmbh.github.io/NoPE-Docs/)
-
-## Show me `NoPE` in 5 Minutes! 
-
-### 1. Create a `Nodejs` Project
-
-Get started by **creating a new project** distributed using `NoPE`.
-
-For our **PYTHON** project we will use the nope-js-node cli tools to create a Project.
-
-1. Installation using  npm:
-  ```bash
-  npm install -g nope-js-node
-  ```
-2. Start your first Project:
-  ```bash
-  nope-js project create
-  ```
-  This should open a `cli`.
-
-3. Answer the requried questions to complete create the directory.
-  - Name the project `HelloWorld`
-  - Give it a short summary. This summary will used during distributing your project.
-  - make shure you select `python` as project type    
-
-4. navigate to the create folder ( e.g. `cd ./HelloWorld` ) 
-
-  This creates a project structure.
-
-5. Open your IDE (e.g. vscode)
-
-By using the project-tool the following features are added to the project:
-- Debugging of the application using VS code (launch-file)
-- Creation of a doc file (see doc/make)
-- Helpers to build a browser related version
-- Use of a changelog
-- Deployment as a package
-- Simple extension using project-tool
-
-## 2. Add a Service in `Python`
-
-Our goal is to define a greeting service
-> The service creates a greeting message for a person. 
-
-### Why a Service
-
-> This service is independent of how many times it has been called.
-> Our functionality is stateless, this allows us to use a service.
-
-### Using the `CLI` to generate the Service
-
-1. To create the Service: 
-  use the `project-tool` to create the service 
-
-  ```bash
-  nope-js project edit
-  ```
-
-2. Perfom the following selection inside of the tool.
-  1. Selection `add`, to add a new element
-  2. Select `service`, because we want to create a service
-  3. Enter the name of the service, in our case `HelloWorld`
-  
-  Creation of the corresponding files and imports is done automatically
-
-  This will update our project folder.
-
-Now `NoPE` defined a new service file (`HelloWorldFunctions.py`) for us:
-
-```python
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from nope import getNopeLogger
-
-LOGGER = getNopeLogger("HelloWorldService")
-
-# Please provide the schema for the Function.
-# See the Example below.
-SCHEMA = {
-    "type": "function",
-        
-    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
-    # It contains a list of all required inputs.
-    "inputs": [
-    ],
-    # To describe the return of a function we added the field "outputs". It contains a 
-    # JSON-Schema Object.
-    "outputs":{
-    }
-}
-
-async def HelloWorld(greetings: str):
-    # Please overwrite me!
-    LOGGER.debug("calling service 'HelloWorld' with the following parameters:" + str(greetings))
-    return "Hello " + greetings + "!"
-```
-
-In that file, you will find a template for the service we want to implement. By default, the newly created service implements the hello-world behavior. This must changed. In our case it matches the desired behavior.
-
-
-> All services **must** be implemented `async` manner. This is necessary so that the runtime is not blocked.
-
-
-### Adding a Service interface
-
-We now want to describe our service, that it can be used correctly at different Runtimes. Therefore we will define the `schema` to the `SCHEMA` variable. This Schema follows the definition of a `JSON-Schema`:
-
-```python
-SCHEMA = {
-    "type": "function",
-        
-    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
-    # It contains a list of all required inputs.
-    "inputs": [
-        {
-            # The Description of the Parameter
-            "description": "The name which should receive a Greeting",
-            # Its used name in the function (see the arguments of the function)
-            "name": "greetings",
-            # The Schema follows a default JSON-Schema
-            "schema": {
-                "type": "string"
-            }
-        }
-    ],
-    # To describe the return of a function we added the field "outputs". It contains a 
-    # JSON-Schema Object.
-    "outputs":{
-        "type": "string",
-
-        # We provide some extra Info for the other users.
-        "description": "The greeting Message!"
-    }
-}
-```
-
-Because the python implementation is lacking some typings please checkout the docs
-
-## 3. Running the Service:
-
-To run the `service` and distribute to different `NoPE`-Runtimes we have to determine a configuration:
-
-```bash
-nope-py scan
-```
-The `cli` will find all defined `services` or `modules` exposed in a so called `NoPE-Package` (This has been created automatically during the initalization of the project). The tool will store its results in the following configuration (located at `./config/config.json`):
-
-```json
-[
-    {
-        "nameOfPackage": "HelloWorld",
-        "autostart": {},
-        "defaultInstances": [],
-        "providedServices": [
-            {
-                "options": {
-                    "schema": {
-                        ...
-                    },
-                    "resultSink": null,
-                    "timeout": -1,
-                    "id": "HelloWorld",
-                    "ui": {
-                        "file": false,
-                        "autoGenBySchema": false,
-                        "requiredProvidersForRendering": []
-                    },
-                    "isDynamic": false
-                }
-            }
-        ],
-        "providedClasses": [],
-        "requiredPackages": [],
-        "path": "C:\\Users\\m.karkowski\\Documents\\00-Repos\\TEST\\HelloWorld\\HelloWorld\\__init__.py"
-    }
-]
-```
-
-Finally we are ready to distribute our service by using the command:
-
-```bash
-nope-py run
-```
-
-This will start a runtime providing our service.
-
-## 4. Interact with the Runtime
-
-Currently our service is only run internally (nope is not connected and runs without an external connection layer). To check and play with the distribution, we kill our old process (`ctrl+c`) create a separate process (e.g. a bash) and provide a serve:
-
-```bash
-nope-js run -c io-server
-```
-
-This will spool up a `socket-io` server on our localhost. 
-
-Afterwards we will restart our Runtime hosting the created service using `io-sockets` as connection layer:
-
-```bash
-nope-py run -c io-client
-```
-
-Now we are able to start our `interact-tool` to manually execute our process:
-
-```bash
-nope-js interact -c io-client -s
-```
-
-To use the `interact`-**tool** follow the questions:
-
-1. What do you want to do?
-    - We want to inspect our distributed system -> `inspect`
-2. What do you want to inspect?
-    - We want to check if our service is present -> `service`
-    - We should be albe to see our `HelloWorld`-Service (see 1)
-3. Now we want to execute this service. Therefore we navigate `back` to the main menu
-4. Now we select `execute` and afterwards `service` because we want to execute our service
-5. Now the Tool renders the available services and we select `HelloWorld` (see 2) and it will render the previously defined Schema.
-6. Now we have to enter the inputs required by the Service:
-    - It is important that the parameters are entered as list (because there might be more the 1 Parameter)
-    - Enter the parameters as valid `JSON` Data.
-    - Press `enter`
-
-    > Executing services with the interact tool will perfom function immedialty. If you integrated Hardware be aware of that.
-
-7. The Tool shows the result (see 4)
-
-
-> You are now running a distributed System using **remote procedure calls** in ***python***
+Metadata-Version: 2.1
+Name: nope-py
+Version: 1.7.9
+Summary: NOPE-Lib represents the No Programming Environment Library for python.
+Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
+Author: Martin Karkowski
+Author-email: m.karkowski@zema.de
+Maintainer: Martin Karkowski
+Maintainer-email: m.karkowski@zema.de
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NoPE 
+
+## A Python wrapper for the Library
+
+Please visit our [Docu](https://zema-ggmbh.github.io/NoPE-Docs/)
+
+## Show me `NoPE` in 5 Minutes! 
+
+### 1. Create a `Nodejs` Project
+
+Get started by **creating a new project** distributed using `NoPE`.
+
+For our **PYTHON** project we will use the nope-js-node cli tools to create a Project.
+
+1. Installation using  npm:
+  ```bash
+  npm install -g nope-js-node
+  ```
+2. Start your first Project:
+  ```bash
+  nope-js project create
+  ```
+  This should open a `cli`.
+
+3. Answer the requried questions to complete create the directory.
+  - Name the project `HelloWorld`
+  - Give it a short summary. This summary will used during distributing your project.
+  - make shure you select `python` as project type    
+
+4. navigate to the create folder ( e.g. `cd ./HelloWorld` ) 
+
+  This creates a project structure.
+
+5. Open your IDE (e.g. vscode)
+
+By using the project-tool the following features are added to the project:
+- Debugging of the application using VS code (launch-file)
+- Creation of a doc file (see doc/make)
+- Helpers to build a browser related version
+- Use of a changelog
+- Deployment as a package
+- Simple extension using project-tool
+
+## 2. Add a Service in `Python`
+
+Our goal is to define a greeting service
+> The service creates a greeting message for a person. 
+
+### Why a Service
+
+> This service is independent of how many times it has been called.
+> Our functionality is stateless, this allows us to use a service.
+
+### Using the `CLI` to generate the Service
+
+1. To create the Service: 
+  use the `project-tool` to create the service 
+
+  ```bash
+  nope-js project edit
+  ```
+
+2. Perfom the following selection inside of the tool.
+  1. Selection `add`, to add a new element
+  2. Select `service`, because we want to create a service
+  3. Enter the name of the service, in our case `HelloWorld`
+  
+  Creation of the corresponding files and imports is done automatically
+
+  This will update our project folder.
+
+Now `NoPE` defined a new service file (`HelloWorldFunctions.py`) for us:
+
+```python
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from nope import getNopeLogger
+
+LOGGER = getNopeLogger("HelloWorldService")
+
+# Please provide the schema for the Function.
+# See the Example below.
+SCHEMA = {
+    "type": "function",
+        
+    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
+    # It contains a list of all required inputs.
+    "inputs": [
+    ],
+    # To describe the return of a function we added the field "outputs". It contains a 
+    # JSON-Schema Object.
+    "outputs":{
+    }
+}
+
+async def HelloWorld(greetings: str):
+    # Please overwrite me!
+    LOGGER.debug("calling service 'HelloWorld' with the following parameters:" + str(greetings))
+    return "Hello " + greetings + "!"
+```
+
+In that file, you will find a template for the service we want to implement. By default, the newly created service implements the hello-world behavior. This must changed. In our case it matches the desired behavior.
+
+
+> All services **must** be implemented `async` manner. This is necessary so that the runtime is not blocked.
+
+
+### Adding a Service interface
+
+We now want to describe our service, that it can be used correctly at different Runtimes. Therefore we will define the `schema` to the `SCHEMA` variable. This Schema follows the definition of a `JSON-Schema`:
+
+```python
+SCHEMA = {
+    "type": "function",
+        
+    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
+    # It contains a list of all required inputs.
+    "inputs": [
+        {
+            # The Description of the Parameter
+            "description": "The name which should receive a Greeting",
+            # Its used name in the function (see the arguments of the function)
+            "name": "greetings",
+            # The Schema follows a default JSON-Schema
+            "schema": {
+                "type": "string"
+            }
+        }
+    ],
+    # To describe the return of a function we added the field "outputs". It contains a 
+    # JSON-Schema Object.
+    "outputs":{
+        "type": "string",
+
+        # We provide some extra Info for the other users.
+        "description": "The greeting Message!"
+    }
+}
+```
+
+Because the python implementation is lacking some typings please checkout the docs
+
+## 3. Running the Service:
+
+To run the `service` and distribute to different `NoPE`-Runtimes we have to determine a configuration:
+
+```bash
+nope-py scan
+```
+The `cli` will find all defined `services` or `modules` exposed in a so called `NoPE-Package` (This has been created automatically during the initalization of the project). The tool will store its results in the following configuration (located at `./config/config.json`):
+
+```json
+[
+    {
+        "nameOfPackage": "HelloWorld",
+        "autostart": {},
+        "defaultInstances": [],
+        "providedServices": [
+            {
+                "options": {
+                    "schema": {
+                        ...
+                    },
+                    "resultSink": null,
+                    "timeout": -1,
+                    "id": "HelloWorld",
+                    "ui": {
+                        "file": false,
+                        "autoGenBySchema": false,
+                        "requiredProvidersForRendering": []
+                    },
+                    "isDynamic": false
+                }
+            }
+        ],
+        "providedClasses": [],
+        "requiredPackages": [],
+        "path": "C:\\Users\\m.karkowski\\Documents\\00-Repos\\TEST\\HelloWorld\\HelloWorld\\__init__.py"
+    }
+]
+```
+
+Finally we are ready to distribute our service by using the command:
+
+```bash
+nope-py run
+```
+
+This will start a runtime providing our service.
+
+## 4. Interact with the Runtime
+
+Currently our service is only run internally (nope is not connected and runs without an external connection layer). To check and play with the distribution, we kill our old process (`ctrl+c`) create a separate process (e.g. a bash) and provide a serve:
+
+```bash
+nope-js run -c io-server
+```
+
+This will spool up a `socket-io` server on our localhost. 
+
+Afterwards we will restart our Runtime hosting the created service using `io-sockets` as connection layer:
+
+```bash
+nope-py run -c io-client
+```
+
+Now we are able to start our `interact-tool` to manually execute our process:
+
+```bash
+nope-js interact -c io-client -s
+```
+
+To use the `interact`-**tool** follow the questions:
+
+1. What do you want to do?
+    - We want to inspect our distributed system -> `inspect`
+2. What do you want to inspect?
+    - We want to check if our service is present -> `service`
+    - We should be albe to see our `HelloWorld`-Service (see 1)
+3. Now we want to execute this service. Therefore we navigate `back` to the main menu
+4. Now we select `execute` and afterwards `service` because we want to execute our service
+5. Now the Tool renders the available services and we select `HelloWorld` (see 2) and it will render the previously defined Schema.
+6. Now we have to enter the inputs required by the Service:
+    - It is important that the parameters are entered as list (because there might be more the 1 Parameter)
+    - Enter the parameters as valid `JSON` Data.
+    - Press `enter`
+
+    > Executing services with the interact tool will perfom function immedialty. If you integrated Hardware be aware of that.
+
+7. The Tool shows the result (see 4)
+
+
+> You are now running a distributed System using **remote procedure calls** in ***python***
+
```

### Comparing `nope_py-1.7.8rc3/nope/__init__.py` & `nope_py-1.7.9/nope/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/cli/logo.py` & `nope_py-1.7.9/nope/cli/logo.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-NOPELOGO = '''
- -----              .---.                                        ..----******--.            -------------------.
-.Peeeen.            =eeeP*                                     .oPeeeeeeeeeeeeePo|-.  ....-*oeeeeeeeeeeeeeeeeePP*.........-*||-
-.PeeeePo-           =eeee*                                     -eeeePn=======oPPPPPn- ....-*oeeeePPPPPPPPPPPPPPP-          -**.
-.PeeeeeeP*          =eeee*               ------                -eeeeo.         *oeeeP-      oeeee-
-.PeeePPPPP|         neeee*        .     -******.    .          -eeeeo.          *eeeP=    .-oeeee-                          ..
-.PeeeP|oeeP|        neeee*      .****-.-********..-***-.       -eeeeo.          .eeePo-...-*oeeeP*-------------------------|++-
-.Peeee..nPePn.      neeee*     *************************-      -eeeeo.           eeeeP-  ..-oeeee-                          -.
-.Peeee.  =PPPn.     neeee*      -********||**||********.       -eeeeo.          .eeePn      oeeee-
-.Peeee.   +PPPn.    neeee*      .*****|||*-..-*||******        -eeeeo.          +eeeP|  ...-oeeeen=+++++++++++*            .--
-.PeeeP-    |PPPo-   neeee*  *********||-        *|*********-   -eeeeP**--..--*|oPePP|.....-*oeeeeeeeeeeeeeeeePn------------*+|-
-.Peeee-.....|PPPo.  neeee*  *********|*         .+|********-   -eeeeePeeeeeeeeePPP=-       -oeeee|-------------             .
-.Peeee*    ..|PePn. neeee*  *********||.        -||********-   -eeeeP==nnnoonn=|*.          oeeee-
-.Peeee*    ...*oPPo|oeeee*..-.  .*****||*-....-*|******.       -eeeeo.                ....-*oeeee*                        .-**.
-.oeeee*....... *PePPPeeee=****- .*******||||||||*******.       -eeeeo.                ....-*oeeeP*........................-*||-
-.oeeee-    .****|Peeeeeee=***- -************************-      -eeeeo.                     .oeeee-
-.oeeee.    .*****+Peeeeee=****---****---********--*****-       -eeeeo.                     .oPeee*..............
-.oPeee.       -***+PPeeee=******  -.    -******.   .-.         -eeeeo.                ....-*oeeeePeeeeeeeeeeeeeP=..........*||-
- nPPPP.      -*****+PPPPP=**-..         .******                .oPPPo.                ....--oPPPPPPPPPPPPPPPPPPP=..........-**.
-             .**--**********-
-                  -***- .-*-.
-                   ...
-'''
-
-
-def renderLogo():
-    print("\n" + NOPELOGO + "\n")
+NOPELOGO = '''
+ -----              .---.                                        ..----******--.            -------------------.
+.Peeeen.            =eeeP*                                     .oPeeeeeeeeeeeeePo|-.  ....-*oeeeeeeeeeeeeeeeeePP*.........-*||-
+.PeeeePo-           =eeee*                                     -eeeePn=======oPPPPPn- ....-*oeeeePPPPPPPPPPPPPPP-          -**.
+.PeeeeeeP*          =eeee*               ------                -eeeeo.         *oeeeP-      oeeee-
+.PeeePPPPP|         neeee*        .     -******.    .          -eeeeo.          *eeeP=    .-oeeee-                          ..
+.PeeeP|oeeP|        neeee*      .****-.-********..-***-.       -eeeeo.          .eeePo-...-*oeeeP*-------------------------|++-
+.Peeee..nPePn.      neeee*     *************************-      -eeeeo.           eeeeP-  ..-oeeee-                          -.
+.Peeee.  =PPPn.     neeee*      -********||**||********.       -eeeeo.          .eeePn      oeeee-
+.Peeee.   +PPPn.    neeee*      .*****|||*-..-*||******        -eeeeo.          +eeeP|  ...-oeeeen=+++++++++++*            .--
+.PeeeP-    |PPPo-   neeee*  *********||-        *|*********-   -eeeeP**--..--*|oPePP|.....-*oeeeeeeeeeeeeeeeePn------------*+|-
+.Peeee-.....|PPPo.  neeee*  *********|*         .+|********-   -eeeeePeeeeeeeeePPP=-       -oeeee|-------------             .
+.Peeee*    ..|PePn. neeee*  *********||.        -||********-   -eeeeP==nnnoonn=|*.          oeeee-
+.Peeee*    ...*oPPo|oeeee*..-.  .*****||*-....-*|******.       -eeeeo.                ....-*oeeee*                        .-**.
+.oeeee*....... *PePPPeeee=****- .*******||||||||*******.       -eeeeo.                ....-*oeeeP*........................-*||-
+.oeeee-    .****|Peeeeeee=***- -************************-      -eeeeo.                     .oeeee-
+.oeeee.    .*****+Peeeeee=****---****---********--*****-       -eeeeo.                     .oPeee*..............
+.oPeee.       -***+PPeeee=******  -.    -******.   .-.         -eeeeo.                ....-*oeeeePeeeeeeeeeeeeeP=..........*||-
+ nPPPP.      -*****+PPPPP=**-..         .******                .oPPPo.                ....--oPPPPPPPPPPPPPPPPPPP=..........-**.
+             .**--**********-
+                  -***- .-*-.
+                   ...
+'''
+
+
+def renderLogo():
+    print("\n" + NOPELOGO + "\n")
```

### Comparing `nope_py-1.7.8rc3/nope/cli/run.py` & `nope_py-1.7.9/nope/cli/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-
-import argparse
-import asyncio
-import json
-import logging
-import sys
-
-from nope.loader import getPackageLoader, loadConfig, loadDesiredPackages
-from nope.communication import getLayer, LAYER_DEFAULT_PARAMETERS, VALID_LAYERS
-from nope.dispatcher.rpcManager.selectors import ValidDefaultSelectors
-from nope.helpers import ensureDottedAccess, generateId, EXECUTOR, generateId
-
-
-def getDefaultParameters():
-    return {
-        "file": "./config/settings.json",
-        "channel": "event",
-        "skipLoadingConfig": False,
-        "channelParams": "not-provided",
-        "log": "info",
-        "dispatcherLogLevel": "info",
-        "communicationLogLevel": "info",
-        "delay": 2,
-        "timings": {},
-        "defaultSelector": "first",
-        "forceUsingSelectors": False,
-        "preventVarifiedNames": False,
-        # "logToFile": False,
-        "id": generateId(),
-        "profile": False,
-        "useBaseServices": True,
-    }
-
-
-def getArgs(add_mode=True, parser=None, default_args=None):
-    """ Helper Function to extract the Arguments
-    """
-
-    if default_args is None:
-        default_args = dict()
-
-    if parser is None:
-        parser = argparse.ArgumentParser(
-            description='cli-tool to run the backend')
-    if add_mode:
-        parser.add_argument('mode', type=str, default="run",
-                            help='option, used to run the code')
-    parser.add_argument('--file', type=str, default="config/settings.json", dest='file',
-                        help='configuration file to use. This File contains the defined packages.')
-    parser.add_argument('-c', type=str, default=default_args.get("channel", "event"), dest='channel',
-                        help='name of the communication layer to use. Possible values are: ' + ', '.join(
-                            [key for key in LAYER_DEFAULT_PARAMETERS.keys()]))
-    parser.add_argument('-p', '--channelParams', type=str, default=default_args.get("channelParams", "not-provided"), dest='channelParams',
-                        help='name of the communication layer to use. Possible values are: ' + ', '.join(
-                            [key for key in LAYER_DEFAULT_PARAMETERS.keys()]))
-    parser.add_argument('-s', '--skip-loading-config', dest='skipLoadingConfig', action='store_true',
-                        help='Skips the Configuration File.')
-
-    parser.add_argument("--default-selector", default=default_args.get("defaultSelector", "first"), dest="defaultSelector",
-                        help="The default-selector to select the service providers. Possible Values are: " +
-                        ", ".join(ValidDefaultSelectors)
-                        )
-
-    parser.add_argument("--log-to-file", help="Log will be stored in a logfile.",
-                        action="store_true", dest='logToFile')
-
-    parser.add_argument('-l', '--log', type=str, default=default_args.get("log", "debug"), dest='log',
-                        help='Level of the Logger. Valid values are "debug", "info"')
-
-    parser.add_argument('--id', type=str, default=default_args.get("id", generateId(use_as_var=True, pre_string="_dispatcher")), dest='id',
-                        help="Define a custom id to the Dispatcher",)
-
-    parser.add_argument('--dispatcher-log', type=str, default=default_args.get("dispatcherLogLevel", "info"), dest='dispatcherLogLevel',
-                        help='Specify the Logger Level of the Dispatcher. Defaults to "info"')
-
-    parser.add_argument('--communication-log', type=str, default=default_args.get("communicationLogLevel", "info"), dest='communicationLogLevel',
-                        help='Specify the Logger Level of the Communication. Defaults to "info"')
-
-    parser.add_argument('--noBaseServices', default=False, dest='useBaseServices', action='store_true',
-                        help='Flag to enable prevent the base Services to be loaded')
-
-    args = parser.parse_args()
-
-    if args.channel in [key for key in VALID_LAYERS.keys()]:
-        pass
-    else:
-        print("invalid communication-layer has been selected")
-        raise Exception("invalid communication-layer has been selected")
-
-    if args.channelParams == "not-provided":
-        args.channelParams = None
-
-    if args.channelParams is not None:
-        try:
-            try:
-                args.params = json.loads(args.params)
-                print(args.params)
-            except Exception as E:
-                "".startswith
-                if not (args.params.startswith(
-                        "{") or args.params.startswith("[")):
-                    args.params = json.loads('"' + args.params + '"')
-                else:
-                    print(E)
-                    raise Exception("Please provide valid JSON")
-        except BaseException:
-            print("Please provide valid JSON")
-            sys.exit()
-
-    args.useBaseServices = not args.useBaseServices or default_args.get(
-        "useBaseServices", False)
-    args.skipLoadingConfig = args.skipLoadingConfig or default_args.get(
-        "skipLoadingConfig", False)
-    args.logToFile = args.logToFile or default_args.get("logToFile", False)
-
-    ret = getDefaultParameters()
-    ret.update(args.__dict__)
-    return ensureDottedAccess(ret)
-
-
-async def generateNopeBackend(_args: dict, run=False):
-    """ Helper Function, which will create a Nope Instance.
-    """
-    args = getDefaultParameters()
-    args.update(_args if isinstance(_args, dict) else _args.__dict__)
-
-    # Test if we need to parse the Data.
-    if isinstance(args, dict):
-        args = ensureDottedAccess(args)
-
-    if getattr(args, "channel", "event") in VALID_LAYERS:
-        pass
-    else:
-        print("invalid communication-layer has been selected")
-        return
-
-    # Get a Communicator
-    communicator = await getLayer(
-        args["channel"],
-        args.get("params", None),
-        args["communicationLogLevel"]
-    )
-
-    # Get the Loader
-    loader = getPackageLoader(
-        communicator=communicator,
-        **args
-    )
-
-    await loader.dispatcher.ready.waitFor()
-    if args.delay:
-        await asyncio.sleep(args.delay)
-
-    def __run():
-
-        try:
-            if not getattr(args, "skip_loading_config", False):
-                # Load all Packages
-                EXECUTOR.callParallel(
-                    loadDesiredPackages,
-                    loader,
-                    loadConfig(args.file),
-                    delay=args.delay
-                )
-
-        except FileNotFoundError:
-            print("Configuration-File not Found!")
-
-        def stop():
-            print("Calling Stop")
-            # Now we have to run our loop,
-            # until the bridge has been disposed.
-            EXECUTOR.loop.run_until_complete(
-                loader.dispatcher.dispose()
-            )
-
-        EXECUTOR.run(before=stop)
-
-    if run:
-        try:
-            if not getattr(args, "skip_loading_config", False):
-                # Load all Packages
-                await loadDesiredPackages(
-                    loader,
-                    loadConfig(args.file).get("packages",[]),
-                    delay=args.delay
-                )                
-
-        except FileNotFoundError:
-            print("Configuration-File not Found!")
-
-        connections = []
-
-        with open(args.file, 'r') as file:
-            raw_data = file.read()
-            config = json.loads(raw_data)
-            connections = config.get("connections",[])
-
-        for item in connections:
-            if item["name"] == "io-client" or item["name"] == "mqtt":          
-                addLayer(
-                    loader.dispatcher.communicator,
-                    item["name"],
-                    item["url"],
-                    item["log"],
-                    item["considerConnection"],
-                    item["forwardData"]
-                )
-
-            elif "event":
-                pass
-            else:
-                raise Exception("Using unkown Connection :(")
-
-        try:
-            await loader.dispatcher.runEndless()
-        except asyncio.CancelledError:
-            EXECUTOR.callParallel(loader.dispatcher.dispose)
-            # await loader.dispatcher.dispose()
-
-    return loader, loader.dispatcher, communicator, __run
-
-
-async def run(add_mode, run=False):
-    args = getArgs(add_mode)
-
-    try:
-        file_name = args.file
-
-        with open(file_name, 'r') as file:
-            raw_data = file.read()
-            config = json.loads(raw_data)
-
-            args = getArgs(add_mode, default_args=config["config"])
-            args.file = file_name
-
-    except BaseException as E:
-        print(E)
-        pass
-
-    _, __, ___, run = await generateNopeBackend(args, run=True)
-
-
-def run_cli(add_mode=True):
-    args = getArgs(add_mode)
-
-    try:
-        with open(args.file, 'r') as file:
-            raw_data = file.read()
-            config = json.loads(raw_data)
-
-            args = getArgs(add_mode, default_args=config["config"])
-
-    except BaseException as E:
-        print(E)
-        pass
-
-    task = asyncio.ensure_future(generateNopeBackend(args, run=True))
-    try:
-        EXECUTOR.start(task)
-    except KeyboardInterrupt:
-        print()
-        # IF we detect a cancel, we dispose every thing
-        task.cancel()
-        EXECUTOR.stop()
-        EXECUTOR.dispose()
-
-
-if __name__ == "__main__":
-    import sys
-    import os
-    import io
-
-    SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-    sys.path.append(os.path.dirname(SCRIPT_DIR))
-
-    run_cli(False)
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+
+import argparse
+import asyncio
+import json
+import logging
+import sys
+
+from nope.loader import getPackageLoader, loadConfig, loadDesiredPackages
+from nope.communication import getLayer, LAYER_DEFAULT_PARAMETERS, VALID_LAYERS
+from nope.dispatcher.rpcManager.selectors import ValidDefaultSelectors
+from nope.helpers import ensureDottedAccess, generateId, EXECUTOR, generateId
+
+
+def getDefaultParameters():
+    return {
+        "file": "./config/settings.json",
+        "channel": "event",
+        "skipLoadingConfig": False,
+        "channelParams": "not-provided",
+        "log": "debug",
+        "dispatcherLogLevel": "info",
+        "communicationLogLevel": "info",
+        "delay": 2,
+        "timings": {},
+        "defaultSelector": "first",
+        "forceUsingSelectors": False,
+        "preventVarifiedNames": False,
+        # "logToFile": False,
+        "id": generateId(),
+        "profile": False,
+        "useBaseServices": True,
+    }
+
+
+def getArgs(add_mode=True, parser=None, default_args=None):
+    """ Helper Function to extract the Arguments
+    """
+
+    if default_args is None:
+        default_args = dict()
+
+    if parser is None:
+        parser = argparse.ArgumentParser(
+            description='cli-tool to run the backend')
+    if add_mode:
+        parser.add_argument('mode', type=str, default="run",
+                            help='option, used to run the code')
+    parser.add_argument('--file', type=str, default="config/settings.json", dest='file',
+                        help='configuration file to use. This File contains the defined packages.')
+    parser.add_argument('-c', type=str, default=default_args.get("channel", "event"), dest='channel',
+                        help='name of the communication layer to use. Possible values are: ' + ', '.join(
+                            [key for key in LAYER_DEFAULT_PARAMETERS.keys()]))
+    parser.add_argument('-p', '--channelParams', type=str, default=default_args.get("channelParams", "not-provided"), dest='channelParams',
+                        help='name of the communication layer to use. Possible values are: ' + ', '.join(
+                            [key for key in LAYER_DEFAULT_PARAMETERS.keys()]))
+    parser.add_argument('-s', '--skip-loading-config', dest='skipLoadingConfig', action='store_true',
+                        help='Skips the Configuration File.')
+
+    parser.add_argument("--default-selector", default=default_args.get("defaultSelector", "first"), dest="defaultSelector",
+                        help="The default-selector to select the service providers. Possible Values are: " +
+                        ", ".join(ValidDefaultSelectors)
+                        )
+
+    parser.add_argument("--log-to-file", help="Log will be stored in a logfile.",
+                        action="store_true", dest='logToFile')
+
+    parser.add_argument('-l', '--log', type=str, default=default_args.get("log", "debug"), dest='log',
+                        help='Level of the Logger. Valid values are "debug", "info"')
+
+    parser.add_argument('--id', type=str, default=default_args.get("id", generateId(use_as_var=True, pre_string="_dispatcher")), dest='id',
+                        help="Define a custom id to the Dispatcher",)
+
+    parser.add_argument('--dispatcher-log', type=str, default=default_args.get("dispatcherLogLevel", "info"), dest='dispatcherLogLevel',
+                        help='Specify the Logger Level of the Dispatcher. Defaults to "info"')
+
+    parser.add_argument('--communication-log', type=str, default=default_args.get("communicationLogLevel", "info"), dest='communicationLogLevel',
+                        help='Specify the Logger Level of the Communication. Defaults to "info"')
+
+    parser.add_argument('--noBaseServices', default=False, dest='useBaseServices', action='store_true',
+                        help='Flag to enable prevent the base Services to be loaded')
+
+    args = parser.parse_args()
+
+    if args.channel in [key for key in VALID_LAYERS.keys()]:
+        pass
+    else:
+        print("invalid communication-layer has been selected")
+        raise Exception("invalid communication-layer has been selected")
+
+    if args.channelParams == "not-provided":
+        args.channelParams = None
+
+    if args.channelParams is not None:
+        try:
+            try:
+                args.params = json.loads(args.params)
+                print(args.params)
+            except Exception as E:
+                "".startswith
+                if not (args.params.startswith(
+                        "{") or args.params.startswith("[")):
+                    args.params = json.loads('"' + args.params + '"')
+                else:
+                    print(E)
+                    raise Exception("Please provide valid JSON")
+        except BaseException:
+            print("Please provide valid JSON")
+            sys.exit()
+
+    args.useBaseServices = not args.useBaseServices or default_args.get(
+        "useBaseServices", False)
+    args.skipLoadingConfig = args.skipLoadingConfig or default_args.get(
+        "skipLoadingConfig", False)
+    args.logToFile = args.logToFile or default_args.get("logToFile", False)
+
+    ret = getDefaultParameters()
+    ret.update(args.__dict__)
+    return ensureDottedAccess(ret)
+
+
+async def generateNopeBackend(_args: dict, run=False):
+    """ Helper Function, which will create a Nope Instance.
+    """
+    args = getDefaultParameters()
+    args.update(_args if isinstance(_args, dict) else _args.__dict__)
+
+    # Test if we need to parse the Data.
+    if isinstance(args, dict):
+        args = ensureDottedAccess(args)
+
+    if getattr(args, "channel", "event") in VALID_LAYERS:
+        pass
+    else:
+        print("invalid communication-layer has been selected")
+        return
+
+    # Get a Communicator
+    communicator = await getLayer(
+        args["channel"],
+        args.get("params", None),
+        args["communicationLogLevel"]
+    )
+
+    # Get the Loader
+    loader = getPackageLoader(
+        communicator=communicator,
+        **args
+    )
+
+    await loader.dispatcher.ready.waitFor()
+    if args.delay:
+        await asyncio.sleep(args.delay)
+
+    def __run():
+
+        try:
+            if not getattr(args, "skip_loading_config", False):
+                # Load all Packages
+                EXECUTOR.callParallel(
+                    loadDesiredPackages,
+                    loader,
+                    loadConfig(args.file),
+                    delay=args.delay
+                )
+
+        except FileNotFoundError:
+            print("Configuration-File not Found!")
+
+        def stop():
+            print("Calling Stop")
+            # Now we have to run our loop,
+            # until the bridge has been disposed.
+            EXECUTOR.loop.run_until_complete(
+                loader.dispatcher.dispose()
+            )
+
+        EXECUTOR.run(before=stop)
+
+    if run:
+        try:
+            if not getattr(args, "skip_loading_config", False):
+                # Load all Packages
+                await loadDesiredPackages(
+                    loader,
+                    loadConfig(args.file).get("packages",[]),
+                    delay=args.delay
+                )                
+
+        except FileNotFoundError:
+            print("Configuration-File not Found!")
+
+        connections = []
+
+        with open(args.file, 'r') as file:
+            raw_data = file.read()
+            config = json.loads(raw_data)
+            connections = config.get("connections",[])
+
+        for item in connections:
+            if item["name"] == "io-client" or item["name"] == "mqtt":          
+                addLayer(
+                    loader.dispatcher.communicator,
+                    item["name"],
+                    item["url"],
+                    item["log"],
+                    item["considerConnection"],
+                    item["forwardData"]
+                )
+
+            elif "event":
+                pass
+            else:
+                raise Exception("Using unkown Connection :(")
+
+        try:
+            await loader.dispatcher.runEndless()
+        except asyncio.CancelledError:
+            EXECUTOR.callParallel(loader.dispatcher.dispose)
+            # await loader.dispatcher.dispose()
+
+    return loader, loader.dispatcher, communicator, __run
+
+
+async def run(add_mode, run=False):
+    args = getArgs(add_mode)
+
+    try:
+        file_name = args.file
+
+        with open(file_name, 'r') as file:
+            raw_data = file.read()
+            config = json.loads(raw_data)
+
+            args = getArgs(add_mode, default_args=config["config"])
+            args.file = file_name
+
+    except BaseException as E:
+        print(E)
+        pass
+
+    _, __, ___, run = await generateNopeBackend(args, run=True)
+
+
+def run_cli(add_mode=True):
+    args = getArgs(add_mode)
+
+    try:
+        with open(args.file, 'r') as file:
+            raw_data = file.read()
+            config = json.loads(raw_data)
+
+            args = getArgs(add_mode, default_args=config["config"])
+
+    except BaseException as E:
+        print(E)
+        pass
+
+    task = asyncio.ensure_future(generateNopeBackend(args, run=True))
+    try:
+        EXECUTOR.start(task)
+    except KeyboardInterrupt:
+        print()
+        # IF we detect a cancel, we dispose every thing
+        task.cancel()
+        EXECUTOR.stop()
+        EXECUTOR.dispose()
+
+
+if __name__ == "__main__":
+    import sys
+    import os
+    import io
+
+    SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
+    sys.path.append(os.path.dirname(SCRIPT_DIR))
+
+    run_cli(False)
```

### Comparing `nope_py-1.7.8rc3/nope/communication/abstractBridgePlugin.py` & `nope_py-1.7.9/nope/communication/abstractBridgePlugin.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# This is a reference Implementation for a Plugin:
-class AbstractBridgePlugin:
-
-    def __init__(self):
-        self.options = ensureDottedAccess(dict(), False)
-        self._id = generateId()
-
-        # Must contain an obervalbe with the flag ready.
-        self.ready = NopeObservable()
-        self.ready.setContent(False)
-
-    @property
-    def id(self) -> str:
-        return self._id
-
-    async def transformData(self, eventName: str, data):
-        # Must return the following data:
-        # 1. eventName: str
-        # 2. data: any
-        # 3.
-
-        # Example 1:
-        #   return eventName, data, None
-
-        # Example 2:
-        #   return eventName, data, None
-        raise Exception("Not Implemented")
-
-    async def init(self) -> None:
-        # Expected after calling init, the ready flag will be
-        # called.
-
-        # Example:
-        #   self.ready.setContent(True)
-
-        raise Exception("Not Implemented")
-
-    def reset(self) -> None:
-        # No return type is being used.
-        raise Exception("Not Implemented")
-
-    async def dispose(self, quiet=False):
-        pass
+# This is a reference Implementation for a Plugin:
+class AbstractBridgePlugin:
+
+    def __init__(self):
+        self.options = ensureDottedAccess(dict(), False)
+        self._id = generateId()
+
+        # Must contain an obervalbe with the flag ready.
+        self.ready = NopeObservable()
+        self.ready.setContent(False)
+
+    @property
+    def id(self) -> str:
+        return self._id
+
+    async def transformData(self, eventName: str, data):
+        # Must return the following data:
+        # 1. eventName: str
+        # 2. data: any
+        # 3.
+
+        # Example 1:
+        #   return eventName, data, None
+
+        # Example 2:
+        #   return eventName, data, None
+        raise Exception("Not Implemented")
+
+    async def init(self) -> None:
+        # Expected after calling init, the ready flag will be
+        # called.
+
+        # Example:
+        #   self.ready.setContent(True)
+
+        raise Exception("Not Implemented")
+
+    def reset(self) -> None:
+        # No return type is being used.
+        raise Exception("Not Implemented")
+
+    async def dispose(self, quiet=False):
+        pass
```

### Comparing `nope_py-1.7.8rc3/nope/communication/addLayer.py` & `nope_py-1.7.9/nope/communication/addLayer.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from nope.communication.bridge import Bridge
-from nope.communication.layers import MQTTLayer, IoSocketClientLayer
-from nope.helpers import generateId, DottedDict
-
-VALID_LAYERS = DottedDict({
-    'event': Bridge,
-    'io-client': IoSocketClientLayer,
-    'mqtt': MQTTLayer
-})
-
-LAYER_DEFAULT_PARAMETERS = DottedDict({
-    'io-client': 'http://127.0.0.1:7000',
-    'mqtt': 'mqtt://localhost:1883'
-})
-
-
-async def addLayer(bridge: Bridge, layer: str, parameter=None, logger=False, considerConnection = False, forwardData = False):
-    """ Adds a Layer to the Bridge.
-
-    Args:
-        bridge (Bridge): The Bridge used to add the layer to
-        layer (str): Name of the Layer. Must match the VALID_LAYERS elements
-        parameter (Any, optional): The Parameter used for the Layer. Defaults to None.
-        logger (bool, optional): A Definition for a Logger for the Layer. Defaults to False.
-        considerConnection (bool, optional): Flag to consinder that connection for the connected flag. Defaults to False.
-        forwardData (bool, optional): Enables or Disables the forwarding of the data. Defaults to False.
-    """
-    params = parameter if parameter is not None else LAYER_DEFAULT_PARAMETERS.get(layer, False)
-    
-    if layer == 'event':
-        pass
-    elif layer == 'io-client':
-        await bridge.addCommunicationLayer(IoSocketClientLayer(params, logger), forwardData, considerConnection)
-    elif layer == 'mqtt':
-        await bridge.addCommunicationLayer(MQTTLayer(params, logger), forwardData, considerConnection)
-    else:
-        raise Exception("Wrong Layer provided!")
-
+from nope.communication.bridge import Bridge
+from nope.communication.layers import MQTTLayer, IoSocketClientLayer
+from nope.helpers import generateId, DottedDict
+
+VALID_LAYERS = DottedDict({
+    'event': Bridge,
+    'io-client': IoSocketClientLayer,
+    'mqtt': MQTTLayer
+})
+
+LAYER_DEFAULT_PARAMETERS = DottedDict({
+    'io-client': 'http://127.0.0.1:7000',
+    'mqtt': 'mqtt://localhost:1883'
+})
+
+
+async def addLayer(bridge: Bridge, layer: str, parameter=None, logger=False, considerConnection = False, forwardData = False):
+    """ Adds a Layer to the Bridge.
+
+    Args:
+        bridge (Bridge): The Bridge used to add the layer to
+        layer (str): Name of the Layer. Must match the VALID_LAYERS elements
+        parameter (Any, optional): The Parameter used for the Layer. Defaults to None.
+        logger (bool, optional): A Definition for a Logger for the Layer. Defaults to False.
+        considerConnection (bool, optional): Flag to consinder that connection for the connected flag. Defaults to False.
+        forwardData (bool, optional): Enables or Disables the forwarding of the data. Defaults to False.
+    """
+    params = parameter if parameter is not None else LAYER_DEFAULT_PARAMETERS.get(layer, False)
+    
+    if layer == 'event':
+        pass
+    elif layer == 'io-client':
+        await bridge.addCommunicationLayer(IoSocketClientLayer(params, logger), forwardData, considerConnection)
+    elif layer == 'mqtt':
+        await bridge.addCommunicationLayer(MQTTLayer(params, logger), forwardData, considerConnection)
+    else:
+        raise Exception("Wrong Layer provided!")
+
     bridge.connected.forcePublish()
```

### Comparing `nope_py-1.7.8rc3/nope/communication/bridge.py` & `nope_py-1.7.9/nope/communication/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,43 +67,48 @@
         if forwardData:
             await layer.on(event, lambda data: EXECUTOR.callParallel(self._emit, event, layer, data))
         else:
             await layer.on(event, lambda data: self._internalEmitter.emit(event, data))
 
     async def _on(self, event, cb):
 
-        # if required we will add a logger for the events.
-        if self._logger and event != 'StatusChanged':
-            def debug_callback(data):
-                if self._logger:
-                    self._logger.debug(f'received "{event}", data={data}')
-                    self._logger.debug(f'subscribe to "{event}"')
-
-            self._internalEmitter.on(event, debug_callback)
-
-        self._internalEmitter.on(event, cb)
-
         # We now store the callback.
         if event not in self._callbacks:
             self._callbacks[event] = [cb]
+
+             # if required we will add a logger for the events.
+             # but this will happen only for new items.
+            if self._logger and event != 'StatusChanged':
+                def debug_callback(data):
+                    if self._logger:
+                        self._logger.debug(f'received "{event}", data={data}')
+                        self._logger.debug(f'subscribe to "{event}"')
+
+                self._internalEmitter.on(event, debug_callback)
+
+            self._internalEmitter.on(event, cb)
+
+            promises = []
+
+            # Now we try to add the callback to the connected layers.
+            for data in self._layers.values():
+                if data.layer.connected.getContent():
+                    promises.append(
+                        self._subscribeToCallback(
+                            data.layer, event, data.forwardData))
+
+            # Now wait for every Layer.
+            if promises:
+                await asyncio.gather(*promises)
         else:
-            self._callbacks[event].append(cb)
+            self._internalEmitter.on(event, cb)
 
-        promises = []
+            self._callbacks[event].append(cb)
 
-        # Now we try to add the callback to the connected layers.
-        for data in self._layers.values():
-            if data.layer.connected.getContent():
-                promises.append(
-                    self._subscribeToCallback(
-                        data.layer, event, data.forwardData))
-
-        # Now wait for every Layer.
-        if promises:
-            await asyncio.gather(*promises)
+        
 
     async def _emit(self, event, toExclude, dataToSend=None, force=False):
         if self._logger and event != 'StatusChanged':
             self._logger.debug(f'emitting {str(event)} {str(dataToSend)}')
         if self._useInternalEmitter or force:
             self._internalEmitter.emit(event, dataToSend)
```

### Comparing `nope_py-1.7.8rc3/nope/communication/layers/EventCommunicationInterface.py` & `nope_py-1.7.9/nope/communication/layers/EventCommunicationInterface.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/communication/layers/IoSocketClientLayer.py` & `nope_py-1.7.9/nope/communication/layers/IoSocketClientLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/communication/layers/abstractLayer.py` & `nope_py-1.7.9/nope/communication/layers/abstractLayer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from nope.helpers import generateId
-from nope.logger import defineNopeLogger
-from nope.observable import NopeObservable
-
-
-class AbstractLayer:
-
-    def __init__(self, uri: str, logger='info'):
-        # Define the URI
-        self.id = generateId()
-        self.receivesOwnMessages = False
-
-        self._logger = defineNopeLogger(logger, "core.mirror.io")
-
-        self.connected = NopeObservable()
-        self.connected.setContent(False)
-
-    async def on(self, eventName: str, cb):
-        raise Exception("Not implemented")
-
-    async def off(self, eventName: str, cb):
-        raise Exception("Not implemented")
-
-    async def emit(self, eventName: str, data):
-        raise Exception("Not implemented")
-
-    async def dispose(self):
-        raise Exception("Not implemented")
-
-    def detailListeners(self, t, listeners):
-        raise Exception("Not implemented")
+from nope.helpers import generateId
+from nope.logger import defineNopeLogger
+from nope.observable import NopeObservable
+
+
+class AbstractLayer:
+
+    def __init__(self, uri: str, logger='info'):
+        # Define the URI
+        self.id = generateId()
+        self.receivesOwnMessages = False
+
+        self._logger = defineNopeLogger(logger, "core.mirror.io")
+
+        self.connected = NopeObservable()
+        self.connected.setContent(False)
+
+    async def on(self, eventName: str, cb):
+        raise Exception("Not implemented")
+
+    async def off(self, eventName: str, cb):
+        raise Exception("Not implemented")
+
+    async def emit(self, eventName: str, data):
+        raise Exception("Not implemented")
+
+    async def dispose(self):
+        raise Exception("Not implemented")
+
+    def detailListeners(self, t, listeners):
+        raise Exception("Not implemented")
```

### Comparing `nope_py-1.7.8rc3/nope/communication/layers/mqttLayer.py` & `nope_py-1.7.9/nope/communication/layers/mqttLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/decorators/classes.py` & `nope_py-1.7.9/nope/decorators/classes.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from nope.helpers import ensureDottedAccess
-
-
-def _class_decorator_factory(storing_type: str):
-    def func(options):
-        options = ensureDottedAccess(options)
-
-        class class_decorator:
-            """ A Simple Decorator for classes
-                This will store the decorated element in an list
-                named "decoratedItems"
-
-                You can provide options etc.
-            """
-
-            def __init__(self, item):
-                nonlocal storing_type
-                self._type = storing_type
-
-            def __set_name__(self, owner, name):
-                # We want to store the item.
-                if not hasattr(owner, "decoratedItems"):
-                    setattr(owner, "decoratedItems", [])
-
-                # Store item
-                owner.decoratedItems.append(
-                    ensureDottedAccess({
-                        "accessor": name,
-                        "options": options,
-                        "type": self._type,
-                        "owner": owner
-                    })
-                )
-
-        return class_decorator
-
-    return func
-
-
-exportAsNopeService = _class_decorator_factory("method")
-exportAsNopeProperty = _class_decorator_factory("property")
-exportAsNopeEvent = _class_decorator_factory("event")
+from nope.helpers import ensureDottedAccess
+
+
+def _class_decorator_factory(storing_type: str):
+    def func(options):
+        options = ensureDottedAccess(options)
+
+        class class_decorator:
+            """ A Simple Decorator for classes
+                This will store the decorated element in an list
+                named "decoratedItems"
+
+                You can provide options etc.
+            """
+
+            def __init__(self, item):
+                nonlocal storing_type
+                self._type = storing_type
+
+            def __set_name__(self, owner, name):
+                # We want to store the item.
+                if not hasattr(owner, "decoratedItems"):
+                    setattr(owner, "decoratedItems", [])
+
+                # Store item
+                owner.decoratedItems.append(
+                    ensureDottedAccess({
+                        "accessor": name,
+                        "options": options,
+                        "type": self._type,
+                        "owner": owner
+                    })
+                )
+
+        return class_decorator
+
+    return func
+
+
+exportAsNopeService = _class_decorator_factory("method")
+exportAsNopeProperty = _class_decorator_factory("property")
+exportAsNopeEvent = _class_decorator_factory("event")
```

### Comparing `nope_py-1.7.8rc3/nope/demo/instances/DecoratedHelloWorld.py` & `nope_py-1.7.9/nope/demo/instances/DecoratedHelloWorld.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from ...decorators.classes import exportAsNopeService
-from ...modules import BaseModule
-from ...observable import NopeObservable
-
-
-class DecoratedHelloWorldModule(BaseModule):
-
-    def __init__(self, core):
-        super().__init__(core)
-
-        # Define the Description:
-        self.setAuthor("martin", "karkowski", "m.karkowski@zema.de")
-        self.setVersion("1.0", "01.11.2022")
-        self.description = "A Simple Hello World Module. It contains a Property and a Function."
-
-        # Generate the Observable
-        self.prop = NopeObservable()
-
-    async def init(self):
-        await super().init()
-
-        await self.registerProperty('prop', self.prop, {
-            'topic': 'prop',
-            'mode': ['publish', 'subscribe']
-        })
-
-        def _callback(data, sender, *args):
-            if (sender != self.prop.id):
-                self._logger.warn("External-Update. Data= " + str(data))
-
-        self.prop.subscribe(_callback)
-
-    @exportAsNopeService({
-        "schema": {
-            "type": "string",
-            "name": "greetings_to",
-            "description": "The person how receives the greeting"
-        }
-    })
-    async def hello(self, greetings_to: str):
-        return 'hello ' + greetings_to + ' from ' + self.identifier
-
-    async def dispose(self):
-        await super().dispose()
-
-        print(self.identifier, "as helloworld is getting removed")
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from ...decorators.classes import exportAsNopeService
+from ...modules import BaseModule
+from ...observable import NopeObservable
+
+
+class DecoratedHelloWorldModule(BaseModule):
+
+    def __init__(self, core):
+        super().__init__(core)
+
+        # Define the Description:
+        self.setAuthor("martin", "karkowski", "m.karkowski@zema.de")
+        self.setVersion("1.0", "01.11.2022")
+        self.description = "A Simple Hello World Module. It contains a Property and a Function."
+
+        # Generate the Observable
+        self.prop = NopeObservable()
+
+    async def init(self):
+        await super().init()
+
+        await self.registerProperty('prop', self.prop, {
+            'topic': 'prop',
+            'mode': ['publish', 'subscribe']
+        })
+
+        def _callback(data, sender, *args):
+            if (sender != self.prop.id):
+                self._logger.warn("External-Update. Data= " + str(data))
+
+        self.prop.subscribe(_callback)
+
+    @exportAsNopeService({
+        "schema": {
+            "type": "string",
+            "name": "greetings_to",
+            "description": "The person how receives the greeting"
+        }
+    })
+    async def hello(self, greetings_to: str):
+        return 'hello ' + greetings_to + ' from ' + self.identifier
+
+    async def dispose(self):
+        await super().dispose()
+
+        print(self.identifier, "as helloworld is getting removed")
```

### Comparing `nope_py-1.7.8rc3/nope/demo/plugins/01-dynamic.py` & `nope_py-1.7.9/nope/demo/plugins/01-dynamic.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from asyncio import sleep
-
-import nope
-from nope import getLayer, EXECUTOR, getDispatcher
-from nope.plugins import install, plugin
-
-"""
-This is an Example how to extend the behavior of any class inside of Nope.
-
-Therefore we define a function (extend) which receives one Parameter, the
-module which is located under the given path. This module must contain
-the loaded class or function. We have to decorate the function with the
-’plugin' decorator (which receives the path as parameter).
-
-Inside of the function we are able to access the original class using the
-`module.*ACCESSOR*`. In the example below we create an extra function
-"hello_dynamic" which will just give us a simple hello world response.
-
-Additional you are able to "store" functions into the module (see our
-extend function).
-
-If you want to manipulate specific vars --> please use a dict. for the
-key use the name of the variable you want to edit.
-"""
-
-
-@plugin("nope.dispatcher.rpcManager")
-def extend_1(module):
-    "Extends `module` - rpcManager"
-
-    class NopeRpcManager(module.NopeRpcManager):
-        async def performCall(self, *args, **kwargs):
-            """ Extend the original behavior """
-            print("calling perform call - extend 1")
-            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
-
-        def hello_dynamic(self):
-            "Ask the plugin to say hello"
-            print("Hello from the Dynamic Plugin")
-
-    def hello_dynamic():
-        "Ask the plugin to say hello"
-        print("Hello from the Dynamic Plugin")
-
-    hello_dynamic_vars = {"hello": "Hello from the Dynamic Plugin"}
-    return NopeRpcManager, hello_dynamic, hello_dynamic_vars
-
-
-# Now install our plugin
-install(nope, extend_1)
-
-
-# The following main is just for clearification
-
-
-async def main():
-    # Create our dispatcher
-    dispatcher = getDispatcher({
-        "communicator": await getLayer("event"),
-        "logger": False,
-    })
-
-    manager = dispatcher.rpcManager
-
-    async def hello_srv(greetings):
-        print("Hello", greetings, "!")
-
-    await dispatcher.ready.waitFor()
-    await dispatcher.rpcManager.registerService(hello_srv, {"id": "hello_srv"})
-
-    await sleep(0.1)
-
-    manager.hello_dynamic()
-    await manager.performCall("hello_srv", ["reader"])
-
-    # Now we are able to access our variable
-    print(nope.dispatcher.rpcManager.hello)
-
-    # and our new function, we injected into the module.
-    nope.dispatcher.rpcManager.hello_dynamic()
-
-
-EXECUTOR.loop.run_until_complete(main())
+from asyncio import sleep
+
+import nope
+from nope import getLayer, EXECUTOR, getDispatcher
+from nope.plugins import install, plugin
+
+"""
+This is an Example how to extend the behavior of any class inside of Nope.
+
+Therefore we define a function (extend) which receives one Parameter, the
+module which is located under the given path. This module must contain
+the loaded class or function. We have to decorate the function with the
+’plugin' decorator (which receives the path as parameter).
+
+Inside of the function we are able to access the original class using the
+`module.*ACCESSOR*`. In the example below we create an extra function
+"hello_dynamic" which will just give us a simple hello world response.
+
+Additional you are able to "store" functions into the module (see our
+extend function).
+
+If you want to manipulate specific vars --> please use a dict. for the
+key use the name of the variable you want to edit.
+"""
+
+
+@plugin("nope.dispatcher.rpcManager")
+def extend_1(module):
+    "Extends `module` - rpcManager"
+
+    class NopeRpcManager(module.NopeRpcManager):
+        async def performCall(self, *args, **kwargs):
+            """ Extend the original behavior """
+            print("calling perform call - extend 1")
+            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
+
+        def hello_dynamic(self):
+            "Ask the plugin to say hello"
+            print("Hello from the Dynamic Plugin")
+
+    def hello_dynamic():
+        "Ask the plugin to say hello"
+        print("Hello from the Dynamic Plugin")
+
+    hello_dynamic_vars = {"hello": "Hello from the Dynamic Plugin"}
+    return NopeRpcManager, hello_dynamic, hello_dynamic_vars
+
+
+# Now install our plugin
+install(nope, extend_1)
+
+
+# The following main is just for clearification
+
+
+async def main():
+    # Create our dispatcher
+    dispatcher = getDispatcher({
+        "communicator": await getLayer("event"),
+        "logger": False,
+    })
+
+    manager = dispatcher.rpcManager
+
+    async def hello_srv(greetings):
+        print("Hello", greetings, "!")
+
+    await dispatcher.ready.waitFor()
+    await dispatcher.rpcManager.registerService(hello_srv, {"id": "hello_srv"})
+
+    await sleep(0.1)
+
+    manager.hello_dynamic()
+    await manager.performCall("hello_srv", ["reader"])
+
+    # Now we are able to access our variable
+    print(nope.dispatcher.rpcManager.hello)
+
+    # and our new function, we injected into the module.
+    nope.dispatcher.rpcManager.hello_dynamic()
+
+
+EXECUTOR.loop.run_until_complete(main())
```

### Comparing `nope_py-1.7.8rc3/nope/demo/plugins/02-multiple.py` & `nope_py-1.7.9/nope/demo/plugins/02-multiple.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import nope
-from nope import getLayer, EXECUTOR, getDispatcher
-from nope.plugins import install, plugin
-
-"""
-You can although combine different plugins for 1 element.
-
-Therefore the install method will receive instead of a plugin
-a list of plugins. The tool will apply the installation using
-the provided order.
-
-"""
-
-
-@plugin("nope.dispatcher.rpcManager")
-def extend_1(module):
-    "Extends `module` - rpcManager"
-
-    class NopeRpcManager(module.NopeRpcManager):
-        async def performCall(self, *args, **kwargs):
-            """ Extend the original behavior """
-            print("calling perform call - extend 1")
-            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
-
-        def hello_dynamic(self):
-            "Ask the plugin to say hello"
-            print("Hello from the Dynamic Plugin")
-
-    def hello_dynamic():
-        "Ask the plugin to say hello"
-        print("Hello from the Dynamic Plugin")
-
-    hello_dynamic_vars = {"hello": "Hello from the Dynamic Plugin"}
-    return NopeRpcManager, hello_dynamic, hello_dynamic_vars
-
-
-@plugin("nope.dispatcher.rpcManager")
-def extend_2(module):
-    "Extends `module` - rpcManager"
-
-    class NopeRpcManager(module.NopeRpcManager):
-        async def performCall(self, *args, **kwargs):
-            """ Extend the original behavior """
-            print("calling perform call - extend 2")
-            try:
-                return await module.NopeRpcManager.performCall(self, *args, **kwargs)
-            except BaseException:
-                print("Failed but we got the error")
-
-    return NopeRpcManager
-
-
-"""
-In our case the plugin 1 is loaded first and then the second (extend_2)
-In the method 'performCall' of the 'NopeRpcManager' this results in loading
-the latest plugin first (extend_2) accessing the 'module.NopeRpcManager' inside
-of 'extend_2' returns you the already modified 'NopeRpcManager' with plugin 1
-(extend 1)
-
-If we call the method
->>> await manager.performCall("hello_srv", ["reader"])
-calling perform call - extend 2
-calling perform call - extend 1
-Failed but we got the error
-"""
-
-install(nope, [extend_1, extend_2])
-
-
-# The following main is just for clearification
-
-
-async def main():
-    # Create our dispatcher
-    dispatcher = getDispatcher({
-        "communicator": await getLayer("event"),
-        "logger": False,
-    })
-
-    manager = dispatcher.rpcManager
-    await dispatcher.ready.waitFor()
-
-    manager.hello_dynamic()
-    await manager.performCall("hello_srv", ["reader"])
-    # If we call the method
-    # >>> await manager.performCall("hello_srv", ["reader"])
-    # calling perform call - extend 2
-    # calling perform call - extend 1
-    # Failed but we got the error
-
-    # Now we are able to access our variable
-    print(nope.dispatcher.rpcManager.hello)
-
-    # and our new function, we injected into the module.
-    nope.dispatcher.rpcManager.hello_dynamic()
-
-
-EXECUTOR.loop.run_until_complete(main())
+import nope
+from nope import getLayer, EXECUTOR, getDispatcher
+from nope.plugins import install, plugin
+
+"""
+You can although combine different plugins for 1 element.
+
+Therefore the install method will receive instead of a plugin
+a list of plugins. The tool will apply the installation using
+the provided order.
+
+"""
+
+
+@plugin("nope.dispatcher.rpcManager")
+def extend_1(module):
+    "Extends `module` - rpcManager"
+
+    class NopeRpcManager(module.NopeRpcManager):
+        async def performCall(self, *args, **kwargs):
+            """ Extend the original behavior """
+            print("calling perform call - extend 1")
+            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
+
+        def hello_dynamic(self):
+            "Ask the plugin to say hello"
+            print("Hello from the Dynamic Plugin")
+
+    def hello_dynamic():
+        "Ask the plugin to say hello"
+        print("Hello from the Dynamic Plugin")
+
+    hello_dynamic_vars = {"hello": "Hello from the Dynamic Plugin"}
+    return NopeRpcManager, hello_dynamic, hello_dynamic_vars
+
+
+@plugin("nope.dispatcher.rpcManager")
+def extend_2(module):
+    "Extends `module` - rpcManager"
+
+    class NopeRpcManager(module.NopeRpcManager):
+        async def performCall(self, *args, **kwargs):
+            """ Extend the original behavior """
+            print("calling perform call - extend 2")
+            try:
+                return await module.NopeRpcManager.performCall(self, *args, **kwargs)
+            except BaseException:
+                print("Failed but we got the error")
+
+    return NopeRpcManager
+
+
+"""
+In our case the plugin 1 is loaded first and then the second (extend_2)
+In the method 'performCall' of the 'NopeRpcManager' this results in loading
+the latest plugin first (extend_2) accessing the 'module.NopeRpcManager' inside
+of 'extend_2' returns you the already modified 'NopeRpcManager' with plugin 1
+(extend 1)
+
+If we call the method
+>>> await manager.performCall("hello_srv", ["reader"])
+calling perform call - extend 2
+calling perform call - extend 1
+Failed but we got the error
+"""
+
+install(nope, [extend_1, extend_2])
+
+
+# The following main is just for clearification
+
+
+async def main():
+    # Create our dispatcher
+    dispatcher = getDispatcher({
+        "communicator": await getLayer("event"),
+        "logger": False,
+    })
+
+    manager = dispatcher.rpcManager
+    await dispatcher.ready.waitFor()
+
+    manager.hello_dynamic()
+    await manager.performCall("hello_srv", ["reader"])
+    # If we call the method
+    # >>> await manager.performCall("hello_srv", ["reader"])
+    # calling perform call - extend 2
+    # calling perform call - extend 1
+    # Failed but we got the error
+
+    # Now we are able to access our variable
+    print(nope.dispatcher.rpcManager.hello)
+
+    # and our new function, we injected into the module.
+    nope.dispatcher.rpcManager.hello_dynamic()
+
+
+EXECUTOR.loop.run_until_complete(main())
```

### Comparing `nope_py-1.7.8rc3/nope/demo/plugins/03-different-items.py` & `nope_py-1.7.9/nope/demo/plugins/03-different-items.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from asyncio import sleep
-
-import nope
-from nope.plugins import install, plugin
-
-"""
-You can although combine different plugins for 1 element.
-
-Therefore the install method will receive instead of a plugin
-a list of plugins. The tool will apply the installation using
-the provided order.
-
-"""
-
-
-@plugin("nope.dispatcher.rpcManager")
-def extend_1(module):
-    "Extends `module` - rpcManager"
-
-    class NopeRpcManager(module.NopeRpcManager):
-        async def performCall(self, *args, **kwargs):
-            """ Extend the original behavior """
-            print("calling perform call - extend 1")
-            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
-
-        def hello_dynamic(self):
-            "Ask the plugin to say hello"
-            print("Hello from the Dynamic Plugin")
-
-    def hello_dynamic():
-        "Ask the plugin to say hello"
-        print("Hello from the Dynamic Plugin")
-
-    hello_dynamic_vars = {"hello": "Hello from the Dynamic Plugin"}
-    return NopeRpcManager, hello_dynamic, hello_dynamic_vars
-
-
-@plugin("nope.dispatcher.nopeDispatcher")
-def extend_2(module):
-    "Extends `module` - NopeDispatcher"
-
-    class NopeDispatcher(module.NopeDispatcher):
-        async def performCall(self, *args, **kwargs):
-            """ Extend the original behavior """
-            print("calling perform call - from ")
-            try:
-                return await self.rpcManager.performCall(self, *args, **kwargs)
-            except BaseException:
-                print("Failed but we got the error")
-
-    return NopeDispatcher
-
-
-"""
-In our case the plugin 1 is loaded first and then the second (extend_2)
-In the method 'performCall' of the 'NopeRpcManager' this results in loading
-the latest plugin first (extend_2) accessing the 'module.NopeRpcManager' inside
-of 'extend_2' returns you the already modified 'NopeRpcManager' with plugin 1
-(extend 1)
-
-If we call the method
->>> await manager.performCall("hello_srv", ["reader"])
-calling perform call - extend 1
-Failed but we got the error
-"""
-
-nope, updated, skipped = install(nope, extend_1)
-nope, updated, skipped = install(nope, extend_2)
-
-print(updated, skipped)
-
-
-# The following main is just for clearification
-
-
-async def main():
-    # Create our dispatcher
-    dispatcher = nope.getDispatcher({
-        "communicator": await nope.getLayer("event"),
-        "logger": False,
-    })
-
-    manager = dispatcher.rpcManager
-
-    async def hello_srv(greetings):
-        print("Hello", greetings, "!")
-
-    await dispatcher.ready.waitFor()
-    await dispatcher.rpcManager.registerService(hello_srv, {"id": "hello_srv"})
-
-    await sleep(0.1)
-
-    # manager.hello_dynamic()
-    await manager.performCall("hello_srv", ["reader"])
-    await dispatcher.performCall("hello_srv", ["reader"])
-    # If we call the method
-    # >>> await dispatcher.performCall("hello_srv", ["reader"])
-    # calling perform call - extend 2
-    # calling perform call - extend 1
-    # Failed but we got the error
-
-    # Now we are able to access our variable
-
-    # and our new function, we injected into the module.
-    nope.dispatcher.rpcManager.hello_dynamic()
-
-
-nope.EXECUTOR.loop.run_until_complete(main())
+from asyncio import sleep
+
+import nope
+from nope.plugins import install, plugin
+
+"""
+You can although combine different plugins for 1 element.
+
+Therefore the install method will receive instead of a plugin
+a list of plugins. The tool will apply the installation using
+the provided order.
+
+"""
+
+
+@plugin("nope.dispatcher.rpcManager")
+def extend_1(module):
+    "Extends `module` - rpcManager"
+
+    class NopeRpcManager(module.NopeRpcManager):
+        async def performCall(self, *args, **kwargs):
+            """ Extend the original behavior """
+            print("calling perform call - extend 1")
+            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
+
+        def hello_dynamic(self):
+            "Ask the plugin to say hello"
+            print("Hello from the Dynamic Plugin")
+
+    def hello_dynamic():
+        "Ask the plugin to say hello"
+        print("Hello from the Dynamic Plugin")
+
+    hello_dynamic_vars = {"hello": "Hello from the Dynamic Plugin"}
+    return NopeRpcManager, hello_dynamic, hello_dynamic_vars
+
+
+@plugin("nope.dispatcher.nopeDispatcher")
+def extend_2(module):
+    "Extends `module` - NopeDispatcher"
+
+    class NopeDispatcher(module.NopeDispatcher):
+        async def performCall(self, *args, **kwargs):
+            """ Extend the original behavior """
+            print("calling perform call - from ")
+            try:
+                return await self.rpcManager.performCall(self, *args, **kwargs)
+            except BaseException:
+                print("Failed but we got the error")
+
+    return NopeDispatcher
+
+
+"""
+In our case the plugin 1 is loaded first and then the second (extend_2)
+In the method 'performCall' of the 'NopeRpcManager' this results in loading
+the latest plugin first (extend_2) accessing the 'module.NopeRpcManager' inside
+of 'extend_2' returns you the already modified 'NopeRpcManager' with plugin 1
+(extend 1)
+
+If we call the method
+>>> await manager.performCall("hello_srv", ["reader"])
+calling perform call - extend 1
+Failed but we got the error
+"""
+
+nope, updated, skipped = install(nope, extend_1)
+nope, updated, skipped = install(nope, extend_2)
+
+print(updated, skipped)
+
+
+# The following main is just for clearification
+
+
+async def main():
+    # Create our dispatcher
+    dispatcher = nope.getDispatcher({
+        "communicator": await nope.getLayer("event"),
+        "logger": False,
+    })
+
+    manager = dispatcher.rpcManager
+
+    async def hello_srv(greetings):
+        print("Hello", greetings, "!")
+
+    await dispatcher.ready.waitFor()
+    await dispatcher.rpcManager.registerService(hello_srv, {"id": "hello_srv"})
+
+    await sleep(0.1)
+
+    # manager.hello_dynamic()
+    await manager.performCall("hello_srv", ["reader"])
+    await dispatcher.performCall("hello_srv", ["reader"])
+    # If we call the method
+    # >>> await dispatcher.performCall("hello_srv", ["reader"])
+    # calling perform call - extend 2
+    # calling perform call - extend 1
+    # Failed but we got the error
+
+    # Now we are able to access our variable
+
+    # and our new function, we injected into the module.
+    nope.dispatcher.rpcManager.hello_dynamic()
+
+
+nope.EXECUTOR.loop.run_until_complete(main())
```

### Comparing `nope_py-1.7.8rc3/nope/demo/plugins/04-fix.py` & `nope_py-1.7.9/nope/demo/plugins/04-fix.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import nope
-from nope.plugins import install, plugin
-
-"""
-This is an Example how to extend the behavior of any class inside of Nope.
-
-Therefore we define a function (extend) which receives one Parameter, the
-module which is located under the given path. This module must contain
-the loaded class or function. We have to decorate the function with the
-’plugin' decorator (which receives the path as parameter).
-
-Inside of the function we are able to access the original class using the
-`module.*ACCESSOR*`. In the example below we create an extra function
-"hello_dynamic" which will just give us a simple hello world response.
-
-Additional you are able to "store" functions into the module (see our
-extend function).
-
-If you want to manipulate specific vars --> please use a dict. for the
-key use the name of the variable you want to edit.
-"""
-
-
-@plugin("nope.helpers.timestamp")
-def extend(module):
-    "Extends `module` - rpcManager"
-
-    def getTimestamp(options=None) -> str:
-        return module.getTimestamp() + 500
-
-    return getTimestamp
-
-
-# Now install our plugin
-nope, _, __ = install(nope, extend)
-
-# The following main is just for clearification
-print("ready")
-print(nope.helpers.getTimestamp())
-print("done")
+import nope
+from nope.plugins import install, plugin
+
+"""
+This is an Example how to extend the behavior of any class inside of Nope.
+
+Therefore we define a function (extend) which receives one Parameter, the
+module which is located under the given path. This module must contain
+the loaded class or function. We have to decorate the function with the
+’plugin' decorator (which receives the path as parameter).
+
+Inside of the function we are able to access the original class using the
+`module.*ACCESSOR*`. In the example below we create an extra function
+"hello_dynamic" which will just give us a simple hello world response.
+
+Additional you are able to "store" functions into the module (see our
+extend function).
+
+If you want to manipulate specific vars --> please use a dict. for the
+key use the name of the variable you want to edit.
+"""
+
+
+@plugin("nope.helpers.timestamp")
+def extend(module):
+    "Extends `module` - rpcManager"
+
+    def getTimestamp(options=None) -> str:
+        return module.getTimestamp() + 500
+
+    return getTimestamp
+
+
+# Now install our plugin
+nope, _, __ = install(nope, extend)
+
+# The following main is just for clearification
+print("ready")
+print(nope.helpers.getTimestamp())
+print("done")
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/baseServices/__init__.py` & `nope_py-1.7.9/nope/dispatcher/baseServices/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from .connectivy import generatePingServices
-from ...helpers import ensureDottedAccess
-
-SERVICES_NAME = {
-    # "defineMaster": generateDefineMaster,
-    "pingService": generatePingServices,
-    # "timeSyncingService": enableTimeSyncing,
-    # "syncingDataService": enablingSyncingData,
-}
-
-
-async def addAllBaseServices(dispatcher, opts=None):
-    """ Adds Bases Services to the Dispatcher.
-
-    Args:
-        dispatcher (Nope): _description_
-        opts (_type_, optional): _description_. Defaults to None.
-
-    Returns:
-        _type_: _description_
-    """
-
-    await dispatcher.ready.waitFor()
-    services = ensureDottedAccess(None)
-
-    if (opts and opts.services):
-        for name in opts.services:
-            services.update(await SERVICES_NAME[name](dispatcher))
-
-    else:
-        for name in SERVICES_NAME:
-            services.update(await SERVICES_NAME[name](dispatcher))
-
-    return services
+from .connectivy import generatePingServices
+from ...helpers import ensureDottedAccess
+
+SERVICES_NAME = {
+    # "defineMaster": generateDefineMaster,
+    "pingService": generatePingServices,
+    # "timeSyncingService": enableTimeSyncing,
+    # "syncingDataService": enablingSyncingData,
+}
+
+
+async def addAllBaseServices(dispatcher, opts=None):
+    """ Adds Bases Services to the Dispatcher.
+
+    Args:
+        dispatcher (Nope): _description_
+        opts (_type_, optional): _description_. Defaults to None.
+
+    Returns:
+        _type_: _description_
+    """
+
+    await dispatcher.ready.waitFor()
+    services = ensureDottedAccess(None)
+
+    if (opts and opts.services):
+        for name in opts.services:
+            services.update(await SERVICES_NAME[name](dispatcher))
+
+    else:
+        for name in SERVICES_NAME:
+            services.update(await SERVICES_NAME[name](dispatcher))
+
+    return services
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/baseServices/connectivy.py` & `nope_py-1.7.9/nope/dispatcher/baseServices/connectivy.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import asyncio
-import logging
-
-from nope.helpers import avgOfArray, ensureDottedAccess, maxOfArray, minOfArray
-from nope.logger import getNopeLogger
-
-logger = getNopeLogger('baseService', level=logging.INFO)
-
-
-async def generatePingServices(dispatcher):
-    async def ping():
-        return ensureDottedAccess({
-            'dispatcherId': dispatcher.id,
-            'timestamp': dispatcher.connectivityManager.now
-        })
-
-    serviceName = 'nope/baseService/ping'
-
-    await dispatcher.rpcManager.registerService(
-        ping,
-        ensureDottedAccess({
-            'id': serviceName,
-            'schema': {
-                'inputs': [],
-                'outputs': {
-                    'type': 'object',
-                    'properties': {
-                        'dispatcherId': {
-                            'type': 'string',
-                            'description': 'Id of the responding Dispatcher'
-                        },
-                        'timestamp': {
-                            'type': 'number',
-                            'description': 'UTC-Timestamp of the system which is responding'
-                        }
-                    }
-                }
-            },
-            'type': 'function',
-            'description': 'Ping'
-        })
-    )
-
-    logger.info("adding 'ping' service!")
-
-    return await generatePingAccessors(dispatcher)
-
-
-async def generatePingAccessors(dispatcher):
-    serviceName = 'nope/baseService/ping'
-
-    # Function to determine the ping in the services.
-    async def determinePing(target: str):
-        # Call the Pings
-        start = dispatcher.connectivityManager.now
-        result = await dispatcher.rpcManager.performCall(serviceName, [], {target})
-        delay = dispatcher.connectivityManager.now
-
-        ping = delay - start
-
-        return ensureDottedAccess({
-            "ping": ping,
-            **result,
-        })
-
-    # Function to Ping all Services
-
-    async def pingAll():
-        dispatchers = list(
-            dispatcher.rpcManager.services.keyMappingReverse.get(
-                serviceName
-            )
-        )
-
-        promises = []
-        for target in dispatchers:
-            promises.append(determinePing(target))
-
-        if promises:
-            pings = await asyncio.gather(*promises)
-
-        _avg = avgOfArray(pings, "ping")
-        _max = maxOfArray(pings, "ping")
-        _min = minOfArray(pings, "ping")
-
-        return ensureDottedAccess({
-            "pings": pings,
-            "avg": _avg,
-            "max": _max,
-            "min": _min,
-        })
-
-    return ensureDottedAccess({
-        "determinePing": determinePing,
-        "pingAll": pingAll
-    })
+import asyncio
+import logging
+
+from nope.helpers import avgOfArray, ensureDottedAccess, maxOfArray, minOfArray
+from nope.logger import getNopeLogger
+
+logger = getNopeLogger('baseService', level=logging.INFO)
+
+
+async def generatePingServices(dispatcher):
+    async def ping():
+        return ensureDottedAccess({
+            'dispatcherId': dispatcher.id,
+            'timestamp': dispatcher.connectivityManager.now
+        })
+
+    serviceName = 'nope/baseService/ping'
+
+    await dispatcher.rpcManager.registerService(
+        ping,
+        ensureDottedAccess({
+            'id': serviceName,
+            'schema': {
+                'inputs': [],
+                'outputs': {
+                    'type': 'object',
+                    'properties': {
+                        'dispatcherId': {
+                            'type': 'string',
+                            'description': 'Id of the responding Dispatcher'
+                        },
+                        'timestamp': {
+                            'type': 'number',
+                            'description': 'UTC-Timestamp of the system which is responding'
+                        }
+                    }
+                }
+            },
+            'type': 'function',
+            'description': 'Ping'
+        })
+    )
+
+    logger.info("adding 'ping' service!")
+
+    return await generatePingAccessors(dispatcher)
+
+
+async def generatePingAccessors(dispatcher):
+    serviceName = 'nope/baseService/ping'
+
+    # Function to determine the ping in the services.
+    async def determinePing(target: str):
+        # Call the Pings
+        start = dispatcher.connectivityManager.now
+        result = await dispatcher.rpcManager.performCall(serviceName, [], {target})
+        delay = dispatcher.connectivityManager.now
+
+        ping = delay - start
+
+        return ensureDottedAccess({
+            "ping": ping,
+            **result,
+        })
+
+    # Function to Ping all Services
+
+    async def pingAll():
+        dispatchers = list(
+            dispatcher.rpcManager.services.keyMappingReverse.get(
+                serviceName
+            )
+        )
+
+        promises = []
+        for target in dispatchers:
+            promises.append(determinePing(target))
+
+        if promises:
+            pings = await asyncio.gather(*promises)
+
+        _avg = avgOfArray(pings, "ping")
+        _max = maxOfArray(pings, "ping")
+        _min = minOfArray(pings, "ping")
+
+        return ensureDottedAccess({
+            "pings": pings,
+            "avg": _avg,
+            "max": _max,
+            "min": _min,
+        })
+
+    return ensureDottedAccess({
+        "determinePing": determinePing,
+        "pingAll": pingAll
+    })
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/core/nopeCore.py` & `nope_py-1.7.9/nope/dispatcher/core/nopeCore.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from nope.dispatcher.connectivityManager import NopeConnectivityManager
-from nope.dispatcher.instanceManager import NopeInstanceManager
-from nope.dispatcher.rpcManager import generateSelector, NopeRpcManager
-from nope.helpers import ensureDottedAccess, generateId, EXECUTOR, Promise
-from nope.logger import defineNopeLogger
-from nope.observable import NopeObservable
-from nope.pubSub import DataPubSubSystem, PubSubSystem
-
-
-class NopeCore:
-
-    def __init__(self, _options, id=None):
-
-        _options = ensureDottedAccess(_options)
-
-        def forwardEvent(item, rest):
-            if item.sender != rcvExternally:
-                EXECUTOR.callParallel(
-                    self.communicator.emit,
-                    'event',
-                    ensureDottedAccess({
-                        **item,
-                        'sender': self._id
-                    })
-                )
-
-        def forwardData(item, rest):
-            if item.sender != rcvExternally:
-                EXECUTOR.callParallel(
-                    self.communicator.emit,
-                    'dataChanged',
-                    ensureDottedAccess({
-                        **item,
-                        'sender': self._id
-                    })
-                )
-
-        def isReady(_):
-            return self.connectivityManager.ready.getContent() \
-                and self.rpcManager.ready.getContent() \
-                and self.instanceManager.ready.getContent()
-
-        def onEvent(msg):
-            msg = ensureDottedAccess(msg)
-            if msg.sender != self._id:
-                data = msg.get("data")
-                path = msg.get("path")
-                msg.sender = rcvExternally
-                self.eventDistributor.emit(path, data, msg)
-
-        def onData(msg):
-            msg = ensureDottedAccess(msg)
-            if msg.sender != self._id:
-                data = msg.get("data")
-                name = msg.get("path")
-                msg.sender = rcvExternally
-                self.dataDistributor.pushData(name, data, msg)
-
-        self._options = _options
-        self._id = id
-        self._disposed = EXECUTOR.generatePromise()
-
-        self.communicator = _options.communicator
-
-        if self._id is None:
-            if _options.id:
-                self._id = _options.id
-            else:
-                self._id = generateId()
-
-        self.logger = defineNopeLogger(_options.logger, 'core')
-        if self.logger:
-            self.logger.info('setting up sub-systems.')
-
-        self.eventDistributor = PubSubSystem()
-        self.eventDistributor.id = self._id
-        self.dataDistributor = DataPubSubSystem()
-        self.dataDistributor.id = self._id
-
-        defaultSelector = generateSelector(
-            _options.get("defaultSelector", "first"), self)
-
-        self.connectivityManager = NopeConnectivityManager(
-            _options,
-            self._id
-        )
-        self.rpcManager = NopeRpcManager(
-            _options,
-            defaultSelector,
-            self._id,
-            self.connectivityManager
-        )
-        self.instanceManager = NopeInstanceManager(
-            _options,
-            defaultSelector,
-            self._id,
-            self.connectivityManager,
-            self.rpcManager,
-            self
-        )
-
-        self.ready = NopeObservable()
-
-        self.ready.getter = isReady
-        rcvExternally = generateId()
-
-        EXECUTOR.callParallel(
-            self.communicator.on,
-            'event',
-            onEvent
-        )
-
-        self.eventDistributor.onIncrementalDataChange.subscribe(
-            forwardEvent)
-
-        EXECUTOR.callParallel(
-            self.communicator.on,
-            'dataChanged',
-            onData
-        )
-
-        self.dataDistributor.onIncrementalDataChange.subscribe(
-            forwardData)
-
-        # Forward the Ready items.
-        self.connectivityManager.ready.subscribe(
-            lambda *args: self.ready.forcePublish())
-        self.rpcManager.ready.subscribe(
-            lambda *args: self.ready.forcePublish())
-        self.instanceManager.ready.subscribe(
-            lambda *args: self.ready.forcePublish())
-
-        self.disposing = False
-
-    @property
-    def id(self):
-        return self._id
-
-    async def dispose(self):
-        self.disposing = True
-        self.ready.dispose()
-
-        if self.logger:
-            self.logger.warn('Removing Dispatcher. Shutting down.')
-
-        await self.eventDistributor.dispose()
-        await self.dataDistributor.dispose()
-        await self.connectivityManager.dispose()
-        await self.rpcManager.dispose()
-        await self.instanceManager.dispose()
-
-        if not self._disposed.cancelled() and not self._disposed.done():
-            self._disposed.set_result(True)
-
-    async def runEndless(self):
-        await self._disposed
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from nope.dispatcher.connectivityManager import NopeConnectivityManager
+from nope.dispatcher.instanceManager import NopeInstanceManager
+from nope.dispatcher.rpcManager import generateSelector, NopeRpcManager
+from nope.helpers import ensureDottedAccess, generateId, EXECUTOR, Promise
+from nope.logger import defineNopeLogger
+from nope.observable import NopeObservable
+from nope.pubSub import DataPubSubSystem, PubSubSystem
+
+
+class NopeCore:
+
+    def __init__(self, _options, id=None):
+
+        _options = ensureDottedAccess(_options)
+
+        def forwardEvent(item, rest):
+            if item.sender != rcvExternally:
+                EXECUTOR.callParallel(
+                    self.communicator.emit,
+                    'event',
+                    ensureDottedAccess({
+                        **item,
+                        'sender': self._id
+                    })
+                )
+
+        def forwardData(item, rest):
+            if item.sender != rcvExternally:
+                EXECUTOR.callParallel(
+                    self.communicator.emit,
+                    'dataChanged',
+                    ensureDottedAccess({
+                        **item,
+                        'sender': self._id
+                    })
+                )
+
+        def isReady(_):
+            return self.connectivityManager.ready.getContent() \
+                and self.rpcManager.ready.getContent() \
+                and self.instanceManager.ready.getContent()
+
+        def onEvent(msg):
+            msg = ensureDottedAccess(msg)
+            if msg.sender != self._id:
+                data = msg.get("data")
+                path = msg.get("path")
+                msg.sender = rcvExternally
+                self.eventDistributor.emit(path, data, msg)
+
+        def onData(msg):
+            msg = ensureDottedAccess(msg)
+            if msg.sender != self._id:
+                data = msg.get("data")
+                name = msg.get("path")
+                msg.sender = rcvExternally
+                self.dataDistributor.pushData(name, data, msg)
+
+        self._options = _options
+        self._id = id
+        self._disposed = EXECUTOR.generatePromise()
+
+        self.communicator = _options.communicator
+
+        if self._id is None:
+            if _options.id:
+                self._id = _options.id
+            else:
+                self._id = generateId()
+
+        self.logger = defineNopeLogger(_options.logger, 'core')
+        if self.logger:
+            self.logger.info('setting up sub-systems.')
+
+        self.eventDistributor = PubSubSystem()
+        self.eventDistributor.id = self._id
+        self.dataDistributor = DataPubSubSystem()
+        self.dataDistributor.id = self._id
+
+        defaultSelector = generateSelector(
+            _options.get("defaultSelector", "first"), self)
+
+        self.connectivityManager = NopeConnectivityManager(
+            _options,
+            self._id
+        )
+        self.rpcManager = NopeRpcManager(
+            _options,
+            defaultSelector,
+            self._id,
+            self.connectivityManager
+        )
+        self.instanceManager = NopeInstanceManager(
+            _options,
+            defaultSelector,
+            self._id,
+            self.connectivityManager,
+            self.rpcManager,
+            self
+        )
+
+        self.ready = NopeObservable()
+
+        self.ready.getter = isReady
+        rcvExternally = generateId()
+
+        EXECUTOR.callParallel(
+            self.communicator.on,
+            'event',
+            onEvent
+        )
+
+        self.eventDistributor.onIncrementalDataChange.subscribe(
+            forwardEvent)
+
+        EXECUTOR.callParallel(
+            self.communicator.on,
+            'dataChanged',
+            onData
+        )
+
+        self.dataDistributor.onIncrementalDataChange.subscribe(
+            forwardData)
+
+        # Forward the Ready items.
+        self.connectivityManager.ready.subscribe(
+            lambda *args: self.ready.forcePublish())
+        self.rpcManager.ready.subscribe(
+            lambda *args: self.ready.forcePublish())
+        self.instanceManager.ready.subscribe(
+            lambda *args: self.ready.forcePublish())
+
+        self.disposing = False
+
+    @property
+    def id(self):
+        return self._id
+
+    async def dispose(self):
+        self.disposing = True
+        self.ready.dispose()
+
+        if self.logger:
+            self.logger.warn('Removing Dispatcher. Shutting down.')
+
+        await self.eventDistributor.dispose()
+        await self.dataDistributor.dispose()
+        await self.connectivityManager.dispose()
+        await self.rpcManager.dispose()
+        await self.instanceManager.dispose()
+
+        if not self._disposed.cancelled() and not self._disposed.done():
+            self._disposed.set_result(True)
+
+    async def runEndless(self):
+        await self._disposed
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/instanceManager/assignmentChecker.py` & `nope_py-1.7.9/nope/dispatcher/instanceManager/assignmentChecker.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-
-def generateAssignmentChecker(selector, core):
-    # Generate a function which will return true.
-    async def generate_true():
-        return True
-
-    if selector == 'first':
-        return generate_true
-    elif selector == 'cpu-usage':
-        return generate_true
-    elif selector == 'free-ram':
-        return generate_true
-
-    elif selector == 'dispatcher':
-        async def dispatcher_matching(_module, used_dispatcher):
-            return used_dispatcher.id == core.id
-
-        return dispatcher_matching
-
-    elif selector == 'host':
-        host = core.connectivityManager.info.host.name
-
-        async def host_matching(_module, used_dispatcher):
-            return used_dispatcher.host.name == host
-
-        return host_matching
-
-    else:
-        raise Exception('Please provide an valid selector')
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+
+def generateAssignmentChecker(selector, core):
+    # Generate a function which will return true.
+    async def generate_true():
+        return True
+
+    if selector == 'first':
+        return generate_true
+    elif selector == 'cpu-usage':
+        return generate_true
+    elif selector == 'free-ram':
+        return generate_true
+
+    elif selector == 'dispatcher':
+        async def dispatcher_matching(_module, used_dispatcher):
+            return used_dispatcher.id == core.id
+
+        return dispatcher_matching
+
+    elif selector == 'host':
+        host = core.connectivityManager.info.host.name
+
+        async def host_matching(_module, used_dispatcher):
+            return used_dispatcher.host.name == host
+
+        return host_matching
+
+    else:
+        raise Exception('Please provide an valid selector')
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/instanceManager/instanceManager.py` & `nope_py-1.7.9/nope/dispatcher/instanceManager/instanceManager.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,956 +1,956 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-import asyncio
-import json
-
-from nope.communication.bridge import Bridge
-from nope.dispatcher.connectivityManager import NopeConnectivityManager
-from nope.dispatcher.rpcManager import NopeRpcManager
-from nope.helpers import SPLITCHAR, ensureDottedAccess, generateId, isIterable, EXECUTOR, waitFor, varifyPath, formatException
-from nope.logger import defineNopeLogger
-from nope.merging import DictBasedMergeData
-from nope.modules import NopeGenericModule
-from nope.observable import NopeObservable
-
-
-class NopeInstanceManager:
-
-    def __init__(self, options, _defaultSelector, _id=None,
-                 _connectivityManager=None, _rpcManager=None, _core=None):
-
-        self.options = options
-        self._defaultSelector = _defaultSelector
-        self._id = _id
-        self._connectivityManager = _connectivityManager
-        self._rpcManager = _rpcManager
-        self._core = _core
-        self._communicator: Bridge = options.communicator
-        self.__disposed = False
-
-        if _id is None:
-            self._id = generateId()
-        if _connectivityManager is None:
-            self._connectivityManager = NopeConnectivityManager(
-                options, id=self._id)
-        if _rpcManager is None:
-            self._rpcManager = NopeRpcManager(
-                options,
-                self._defaultSelector,
-                id=self._id,
-                connectivityManager=self._connectivityManager
-            )
-
-        self._logger = defineNopeLogger(
-            options.logger, 'core.instance-manager')
-
-        # Flag to indicate, that the system is ready.
-        self.ready = NopeObservable()
-        self.ready.setContent(False)
-
-        self._mappingOfRemoteDispatchersAndGenerators = dict()
-        # Overview of the available Constructors in the network.
-        self.constructors = DictBasedMergeData(
-            self._mappingOfRemoteDispatchersAndGenerators, '+', '+')
-        self._mappingOfRemoteDispatchersAndInstances = dict()
-
-        # Overview of the available instances in the network.
-        #   - OriginalKey = DispatcherID (string);
-        #   - OriginalValue = Available Instance Messages (IAvailableInstancesMsg);
-        #   - ExtractedKey = The name of the Instance (string);
-        #   - ExtractedValue = instance-description (INopeModuleDescription);
-        self.instances = DictBasedMergeData(
-            self._mappingOfRemoteDispatchersAndInstances, 'instances/+', 'instances/+/identifier')
-
-        self._internalWrapperGenerators = dict()
-        self._registeredConstructors = dict()
-        self._instances = dict()
-        self._externalInstances = dict()
-        self._internalInstances = set()
-        self._initializingInstance = dict()
-        self._externalInstancesNames = set()
-
-        # Contains the identifiers of the instances, which are hosted in the
-        # provided dispatcher.
-        self.internalInstances = NopeObservable()
-        self.internalInstances.setContent([])
-
-        self.constructorServices = NopeObservable()
-        self.constructorServices.setContent([])
-
-        _ctorStart = f'nope{SPLITCHAR}core{SPLITCHAR}constructor{SPLITCHAR}'
-
-        def _extractGenerators(*args):
-
-            constructorServices = set()
-
-            self._mappingOfRemoteDispatchersAndGenerators.clear()
-            for dispatcher, services in self._rpcManager.services.originalData.items():
-                def _filterMatchingServices(svc):
-                    if "id" in svc and svc.id.startswith(_ctorStart):
-                        constructorServices.add(svc["id"])
-                        return True
-                    return False
-
-                generators = list(
-                    map(
-                        lambda item: item.id[len(_ctorStart):],
-                        filter(
-                            _filterMatchingServices,
-                            services.services
-                        )
-                    )
-                )
-
-                if len(generators):
-                    self._mappingOfRemoteDispatchersAndGenerators[dispatcher] = generators
-
-            self.constructorServices.setContent(list(constructorServices))
-            self.constructors.update()
-
-        # Subscribe to changes.
-        self._rpcManager.services.data.subscribe(_extractGenerators)
-
-        if self._logger:
-            self._logger.info('core.instance-manager online')
-
-        self.reset()
-        EXECUTOR.callParallel(self._init)
-
-    async def _sendAvailableInstances(self):
-        # Update the Instances provided by this module.
-        await self._communicator.emit(
-            "instancesChanged",
-            {
-                "dispatcher": self._id,
-                # We will send the descriptions.
-                # Generate the Module Description for every identifier:
-                "instances": list(
-                    map(lambda item: self._instances[item]["instance"].toDescription(), self._internalInstances))
-            }
-        )
-
-        # Update the Instances
-        self.internalInstances.setContent(list(self._internalInstances))
-
-    async def _init(self):
-
-        await self._communicator.connected.waitFor()
-        await self._connectivityManager.ready.waitFor()
-        await self._rpcManager.ready.waitFor()
-
-        async def _generateWrapper(dispather, description):
-            mod = NopeGenericModule(
-                dispather,
-                # self._generateEmitter,
-                # self._generateObservable
-            )
-            await mod.fromDescription(description, "overwrite")
-            return mod
-
-        self.registerInternalWrapperGenerator(
-            "*",
-            _generateWrapper
-        )
-
-        def _onDispatchersChanged(changes, *args):
-            """ Callback which will handle new and offline Dispatchers.
-            """
-
-            if len(changes.added):
-                # If there are dispatchers online,
-                # We will emit our available services.
-                EXECUTOR.callParallel(self._sendAvailableInstances)
-
-            if len(changes.removed):
-                # Remove the dispatchers.
-                for removedId in changes.removed:
-                    self.removeDispatcher(removedId)
-
-        # We will use our status-manager to listen to changes.
-        self._connectivityManager.dispatchers.onChange.subscribe(
-            _onDispatchersChanged)
-
-        # Make shure we are emitting the instances provided.
-        await self._communicator.on("bonjour", lambda *args: EXECUTOR.callParallel(self._sendAvailableInstances))
-
-        def _onInstancesChanged(message, *args):
-            """ Callback which will be called if the commincator receives a Message
-                that some instances has been changed.
-
-            Args:
-                message: The Message from the System.
-            """
-            # Store the instance.
-            self._mappingOfRemoteDispatchersAndInstances[message.dispatcher] = message
-
-            # Update the Mapping
-            self.instances.update()
-
-            if self._logger:
-                self._logger.debug(
-                    'Remote Dispatcher "' + str(message.dispatcher) + '" updated its available instances')
-
-        # Listen to the Changes.
-        await self._communicator.on("instancesChanged", _onInstancesChanged)
-
-        if self._logger:
-            self._logger.debug("core.instance-manager " +
-                               str(self._id) + " initialized")
-
-        self.ready.setContent(True)
-
-    def getServiceName(self, name: str, type: str) -> str:
-        """ Helper to get the corresponding Service name
-
-        Args:
-            name (str): Name of the Service
-            _type (str): The desired type of the requested service name. Could be "dispose" or "constructor"
-
-        Returns:
-            str: The Adapted Name
-        """
-        if type == "constructor":
-            return f"nope{SPLITCHAR}core{SPLITCHAR}constructor{SPLITCHAR}{name}"
-        elif type == "dispose":
-            return f"nope{SPLITCHAR}core{SPLITCHAR}destructor{SPLITCHAR}{name}"
-        else:
-            raise Exception("The given type is not correct.")
-
-    def _getInstanceInfo(self, identifier: str):
-        """ Function, that will extract the information of the instance and the providing dispatcher.
-
-        Args:
-            identifier (str): The identifier of instance
-        """
-        # First check if the instance exists.
-        if not self.instanceExists(identifier, False):
-            return None
-
-        ret = ensureDottedAccess({})
-
-        # First we check if we are taking care of an internal instance, if so
-        # we will use this instance to enrich the description, otherwise, we
-        # will look in the external instances.
-        if identifier in self._instances:
-            ret.description = self._instances[identifier].instance.toDescription(
-            )
-        else:
-            for item in self._mappingOfRemoteDispatchersAndInstances.values():
-                instances = item.instances
-
-                for instance in instances:
-                    if instance.identifier == identifier:
-                        ret.description = instance
-                        break
-
-        ret.dispatcher = self.getManagerOfInstance(identifier)
-
-        return ret
-
-    def removeDispatcher(self, dispatcher: str):
-        """  Helper to remove a dispatcher.
-
-        Args:
-            dispatcher (str): The Id of the Dispatcher
-        """
-        if self._mappingOfRemoteDispatchersAndInstances.pop(dispatcher, False):
-            self.instances.update()
-
-    async def registerConstructor(self, identifier: str, cb):
-        """ Registers a Constructor, that enables other NopeInstanceManagers to create an instance of the given type. Therefore a callback "cb" is registered with the given "typeIdentifier"
-
-        Args:
-            identifier (str): The identifier for the Constructor (Like a service)
-            cb (function): The callback used, to create an instance. The Callback receives the following parameters (NopeCore, identifier:str)
-        """
-
-        if self._logger:
-            self._logger.debug(
-                'Adding instance generator for "' + (identifier +
-                                                     '" to external Generators. Other Elements can now create instances of self type.'
-                                                     ))
-
-        async def createInstance(data):
-
-            # Check if an instance exists or not.
-            # if not => create an instance an store it.
-
-            if data.identifier not in self._instances:
-                hashableData = [data.identifier, data.params, data.type]
-                try:
-                    hashed = hash(hashableData)
-                except BaseException as E:
-                    hashed = json.dumps(hashableData)
-
-                # It might happen, that an instance is requested multiple times.
-                # therefore we have to make shure, we wont create them multiple times:
-                # We will test it by using the "_internalInstances" set
-
-                if data.identifier not in self._initializingInstance:
-
-                    try:
-
-                        # Mark the Instance as available.
-                        self._initializingInstance[data.identifier] = hashed
-
-                        # Create the Instance
-                        _instance = await cb(self._core, data.identifier)
-                        _instance.identifier = data.identifier
-
-                        # Make shure the Data is expressed as Array.
-                        if not isIterable(data.params):
-                            data.params = [data.params]
-
-                        # Initialize the instance with the parameters.
-                        await _instance.init(*data.params)
-
-                        async def disposeInstance(_data):
-                            """ A Function is registered, taking care of removing
-                                an instances, if it isnt needed any more.
-
-                            Args:
-                                _data (msg): The message containing the dispatcher id.
-                            """
-
-                            _data = ensureDottedAccess(_data)
-
-                            if self._instances.get(data.identifier).usedBy:
-                                try:
-
-                                    if _data.dispatcherId in self._instances.get(
-                                            data.identifier).usedBy:
-                                        # Pop the dispatcher if it is present:
-                                        idx = self._instances.get(
-                                            data.identifier).usedBy.index(
-                                            _data.dispatcherId)
-                                        self._instances.get(
-                                            data.identifier).usedBy.pop(idx)
-
-                                    if len(self._instances.get(
-                                            data.identifier).usedBy) == 0:
-                                        # Unmark as internal instance
-                                        self._internalInstances.remove(
-                                            data.identifier)
-                                        # Remove the Instance.
-                                        await _instance.dispose()
-                                        # Removes the instances
-                                        self._instances.pop(data.identifier)
-                                        # Remove the Function itself
-                                        await self._rpcManager.unregisterService(self.getServiceName(data.identifier, 'dispose'))
-                                        # Emit the instances again
-                                        await self._sendAvailableInstances()
-
-                                except ValueError:
-                                    pass
-
-                        # A Function is registered, taking care of removing
-                        # an instances, if it isnt needed any more.
-                        await self._rpcManager.registerService(
-                            disposeInstance,
-                            ensureDottedAccess({
-                                'id': self.getServiceName(data.identifier, 'dispose'),
-                                'schema': ensureDottedAccess({
-                                    'description': f'Service, which will destructor for the instance "{data.identifier}". This function will be called internal only.',
-                                    'type': 'function'})
-                            })
-                        )
-
-                        # Store the Instance.
-                        self._instances[data.identifier] = ensureDottedAccess({
-                            'instance': _instance,
-                            'usedBy': [data.dispatcherId]
-                        })
-
-                        self._internalInstances.add(data.identifier)
-
-                        # Update the available instances:
-                        await self._sendAvailableInstances()
-
-                        # Make shure, we remove this instance.hash
-                        self._initializingInstance.pop(data.identifier)
-
-                    except BaseException as E:
-                        # Make shure, we remove this instance.hash
-                        self._initializingInstance.pop(data.identifier)
-
-                        raise E
-
-                elif self._initializingInstance.get(data.identifier) != hashed:
-                    raise Exception(
-                        'Providing different Parameters for the same Identifier'
-                    )
-                else:
-                    # Check if the Instance is ready.
-                    firstHint = True
-
-                    def checker():
-                        nonlocal firstHint
-                        if firstHint:
-                            self._logger.warn(
-                                f'Parallel request for the same Instance "{data.identifier}" => Waiting until the Instance has been initialized')
-                            firstHint = False
-                        return data.identifier in self._instances
-
-                    await waitFor(
-                        checker,
-                        ensureDottedAccess({
-                            'testFirst': True,
-                            'delay': 100
-                        })
-                    )
-            else:
-                # If an Element exists => Add the Element.
-                self._instances.get(data.identifier).usedBy.append(
-                    data.dispatcherId)
-
-            # Define the Response.
-            response = ensureDottedAccess({
-                'description': self._instances.get(data.identifier).instance.toDescription(),
-                'type': data.type
-            })
-
-            # Send the Response
-            return response
-
-        _cb = await self._rpcManager.registerService(
-            createInstance,
-            ensureDottedAccess({
-                # We will add the Name to our service.
-                'id': self.getServiceName(identifier, 'constructor'),
-                # We dont want to have a Prefix for construcors
-                'addNopeServiceIdPrefix': False,
-                'schema': ensureDottedAccess({
-                    'description': f'Service, which will create an construtor for the type "{identifier}".',
-                    'type': 'function'
-                })
-            })
-        )
-
-        # Store a generator
-        self._registeredConstructors[identifier] = _cb
-
-    async def unregisterConstructor(self, identifier: str):
-        """ Unregisters a present Constructor. After this, created instances are still valid, the user isnt able to create new ones.
-
-        Args:
-            identifier (str): The identifier for the Constructor (Like a service)
-        """
-        if identifier in self._registeredConstructors:
-            if self._logger:
-                self._logger.debug('Removing instance generator for "' + identifier +
-                                   '" from external Generators. Other Elements cant create instances of self type anymore.')
-
-            # We will just unregister the service from our
-            # system. Therefore we just use the rpcManager
-
-            await self._rpcManager.unregisterService(self._registeredConstructors.get(identifier))
-            self._registeredConstructors.pop(identifier)
-
-    def registerInternalWrapperGenerator(self, identifier: str, cb):
-        """ Defaultly a generic wrapper will be returned, when an instance is created. you
-            can specifiy specific wrapper type for different "typeIdentifier" with this method.
-
-        Args:
-            identifier (str): The identifier for the Constructor (Like a service)
-            cb (function): The Callback which creates the specific wrapper.
-        """
-        if self._logger:
-            self._logger.debug('Adding instance generator for "' + identifier +
-                               '" as internal Generator. This Generator wont be used externally.')
-
-        self._internalWrapperGenerators[identifier] = cb
-
-    def unregisterInternalWrapperGenerator(self, identifier: str):
-        """ Removes a specific generator for for a wrapper.
-
-        Args:
-            identifier (str): The identifier for the Constructor (Like a service)
-        """
-        if self._logger:
-            self._logger.debug('Rmoving instance generator for "' + identifier +
-                               '" from internal Generator. The sytem cant create elements of self type any more.')
-
-        self._internalWrapperGenerators.pop(identifier)
-
-    def instanceExists(self, identifier: str, externalOnly=True) -> bool:
-        """  Helper, to test if an instance with the given identifier exists or not.
-
-        Args:
-            identifier (str):  identifier of the instance.
-            externalOnly (bool, optional): If set to true we will only look for external instances in the external dispatchers. Defaults to True.
-
-        Returns:
-            bool: The Testresult
-        """
-        if identifier not in self.instances.simplified:
-            return False
-
-        if externalOnly:
-            manager = self.getManagerOfInstance(identifier)
-            return manager["id"] != self._id
-
-        return True
-
-    def getManagerOfInstance(self, identifier: str):
-        """ Returns the hosting dispatcher for the given instance.
-
-        Args:
-            identifier (str): The identifier for instance (its name)
-
-        Returns:
-            INopeStatusInfo | False: The Status or false if not present.
-        """
-        # First we will check if the instance is available internally
-        if identifier in self._internalInstances:
-            return self._connectivityManager.info
-
-        # If that isnt the case, we will check all dispatchers and search the
-        # instance.
-        for iter_item in self._mappingOfRemoteDispatchersAndInstances.items():
-            dispatcher = iter_item[0]
-            msg = iter_item[1]
-            for instance in msg.instances:
-                if instance.identifier == identifier:
-                    return self._connectivityManager.getStatus(dispatcher)
-
-        return None
-
-    def getInstanceDescription(self, instanceIdentifier: str):
-        """ Returns the instance Description for a specific instance. It is just a simplified wrapper
-            for the "instances"-property.
-
-        Args:
-            instanceIdentifier (str): The identifier for instance (its name)
-
-        Returns:
-            INopeModuleDescription | False: The Description or False if not found.
-        """
-        if instanceIdentifier in self._instances:
-            return self._instances.get(
-                instanceIdentifier).instance.toDescription()
-
-        for data in self._mappingOfRemoteDispatchersAndInstances.values():
-            instances = data.get("instances", [])
-            for instance in instances:
-                if instance["identifier"] == instanceIdentifier:
-                    return instance
-
-        return False
-
-    def constructorExists(self, typeIdentifier: str) -> bool:
-        """ Helper to test if a constructor linkt to the provided "typeIdentifier" exists or not.
-
-        Args:
-            typeIdentifier (str): The identifier for the Constructor (Like a service)
-
-        Returns:
-            bool: _description_
-        """
-        return typeIdentifier in self.constructors.data.getContent()
-
-    async def createInstance(self, description, options=None):
-        """ Allows to create an instance. This might be the case on remote dispatchers or
-            on the same element. Only a wrapper is returned, which communicates with a
-            dispatcher, because we dont know where the element is provided. You can use the
-            method "getDispatcherForInstance" to determine the dispatcher running the instance.
-
-            The returned wrapper acts like a normal "internal" class.
-
-        Args:
-            description (dict-like): Description of the instance to be created
-            options (dict-like, optional): Options used during creating the instance.. Defaults to None.
-
-
-        Returns:
-            NopeGenericModule | Registered Wrapper: An Generic Nope Module as Wrapper or a custom wrapper for the class.
-        """
-
-        # Define the Default Description
-        # which will lead to an error.
-
-        options = ensureDottedAccess(options)
-        description = ensureDottedAccess(description)
-
-        # Assign the provided Description
-        _description = ensureDottedAccess({
-            'dispatcherId': self._id,
-            'identifier': 'error',
-            'params': [],
-            'type': 'unkown'
-        })
-        _description.update(description)
-        _description.update({'dispatcherId': self._id})
-
-        # Check if the Description is complete
-        if (_description.type == 'unkown' or _description.identifier) == 'error':
-            raise Exception(
-                'Please Provide at least a "type" and "identifier" in the paremeters')
-
-        # Use the varified Name (removes the invalid chars.)
-        _description.identifier = varifyPath(
-            _description.identifier) if self.options.forceUsingValidVarNames else _description.identifier
-        if self._logger:
-            self._logger.debug('Requesting an Instance of type: "' + _description.type +
-                               '" with the identifier: "' + str(_description.identifier) + '"')
-
-        try:
-            _type = _description.type
-            if _type not in self._internalWrapperGenerators:
-                _type = '*'
-
-            if not self.constructorExists(_description.type):
-                # No default type is present for a remote
-                # => assing the default type which is "*""
-                raise Exception('Generator "' + _description.type +
-                                '" isnt present in the network!')
-            if _type in self._internalWrapperGenerators:
-                if self._logger:
-                    self._logger.debug('No instance with the identifiert: "' + str(_description.identifier) +
-                                       '" found, but an internal generator is available. Using the internal one for creating the instance and requesting the "real" instance externally')
-
-                # Now test if there is allready an instance with this name and type.
-                # If so, we check if we have the correct type etc. Additionally we
-                # try to extract its dispatcher-id and will use that as selector
-                # to allow the function be called.
-
-                _instanceDetails = self._getInstanceInfo(
-                    _description.identifier)
-
-                usedDispatcher = None
-
-                if _instanceDetails is not None and _instanceDetails.description.type != _description.type:
-                    raise Exception(
-                        "There exists an Instance named: '" + str(_description.identifier) + "' but it uses a different type. Requested type: '" +
-                        _description.type + "', given type: '" + str(_instanceDetails.description.type) + "'")
-
-                elif _instanceDetails is not None:
-                    usedDispatcher = _instanceDetails.dispatcher.id
-
-                if usedDispatcher and options.assignmentValid:
-
-                    # If we have an dispatcher, which was been used to create the instance,
-                    # we have to check, the selected Dispatcher Matches our
-                    # criteria.
-
-                    if not await options.assignmentValid(_instanceDetails.description, _instanceDetails.dispatcher):
-                        raise Exception('Assignment is invalid.')
-
-                definedInstance = await self._rpcManager.performCall(
-                    self.getServiceName(_description.type, 'constructor'),
-                    [
-                        _description
-                    ],
-                    options
-                )
-
-                if self._logger:
-                    self._logger.debug(
-                        f'Received a description for the instance "{definedInstance.description.identifier}"')
-
-                # Create the Wrapper for our instance.
-                wrapper = await self._internalWrapperGenerators.get(_type)(self._core, definedInstance.description)
-                if self._logger:
-                    self._logger.debug(
-                        f'Created a Wrapper for the instance "{definedInstance.description.identifier}"')
-
-                originalDispose = wrapper.dispose
-
-                async def dispose():
-                    await self.deleteInstance(wrapper.identifier)
-
-                    await originalDispose()
-
-                setattr(wrapper, "dispose", dispose)
-
-                self._instances[_description.identifier] = ensureDottedAccess({
-                    'instance': wrapper,
-                    'usedBy': [
-                        _description.dispatcherId
-                    ]
-                }
-                )
-
-                return wrapper
-
-            raise Exception('No internal generator Available!')
-
-        except Exception as e:
-
-            if self._logger:
-                self._logger.error(
-                    'During creating an Instance, the following error Occurd')
-                self._logger.error(formatException(e))
-
-            raise e
-
-    async def generateWrapper(self, description):
-        # Define the Default Description
-        # which will lead to an error.
-        description = ensureDottedAccess(description)
-
-        # Assign the provided Description
-        _description = ensureDottedAccess({
-            'dispatcherId': self._id,
-            'identifier': 'error',
-            'params': [],
-            'type': 'unkown'
-        })
-        _description.update(description)
-        _description.update({'dispatcherId': self._id})
-
-        # Check if the Description is complete
-        if (_description.type == 'unkown' or _description.identifier) == 'error':
-            raise Exception(
-                'Please Provide at least a "type" and "identifier" in the paremeters')
-
-        # Use the varified Name (removes the invalid chars.)
-        _description.identifier = varifyPath(
-            _description.identifier) if self.options.forceUsingValidVarNames else _description.identifier
-        if self._logger:
-            self._logger.debug('Requesting an Instance of type: "' + _description.type +
-                               '" with the identifier: "' + str(_description.identifier) + '"')
-
-        try:
-            _type = _description.type
-            if _type not in self._internalWrapperGenerators:
-                _type = '*'
-
-            if not self.constructorExists(_description.type):
-                # No default type is present for a remote
-                # => assing the default type which is "*""
-                raise Exception('Generator "' + _description.type +
-                                '" isnt present in the network!')
-            if _type in self._internalWrapperGenerators:
-                if self._logger:
-                    self._logger.debug('No instance with the identifiert: "' + str(_description.identifier) +
-                                       '" found, but an internal generator is available. Using the internal one for creating the instance and requesting the "real" instance externally')
-
-                # Now test if there is allready an instance with this name and type.
-                # If so, we check if we have the correct type etc. Additionally we
-                # try to extract its dispatcher-id and will use that as selector
-                # to allow the function be called.
-
-                _instanceDetails = self._getInstanceInfo(
-                    _description.identifier)
-
-                if _instanceDetails is not None and _instanceDetails.description.type != _description.type:
-                    raise Exception(
-                        "There exists an Instance named: '" + str(_description.identifier) + "' but it uses a different type. Requested type: '" +
-                        _description.type + "', given type: '" + str(_instanceDetails.description.type) + "'")
-
-                elif _instanceDetails is None:
-                    raise Exception(
-                        'No instance known with the idenfitier "' + str(_description.identifier) + '" !')
-
-                definedInstance = _instanceDetails.description
-
-                # Create the Wrapper for our instance.
-                wrapper = await self._internalWrapperGenerators.get(_type)(self._core, definedInstance.description)
-                if self._logger:
-                    self._logger.debug(
-                        f'Created a Wrapper for the instance "{definedInstance.description.identifier}"')
-
-                originalDispose = wrapper.dispose
-
-                async def dispose():
-                    await self.deleteInstance(wrapper.indentifier)
-
-                    await originalDispose()
-
-                setattr(wrapper, "dispose", dispose)
-
-                self._instances[_description.identifier] = ensureDottedAccess({
-                    'instance': wrapper,
-                    'usedBy': [
-                        _description.dispatcherId
-                    ]
-                }
-                )
-
-                return wrapper
-
-            raise Exception('No internal generator Available!')
-
-        except Exception as e:
-
-            if self._logger:
-                self._logger.error(
-                    'During creating an Instance, the following error Occurd')
-                self._logger.error(formatException(e))
-
-            raise e
-
-    async def registerInstance(self, instance):
-        """ Option, to statically register an instance, without using an specific generator etc.
-            This instance is just present in the network.
-
-        Args:
-            instance (INopeInstance): The Instnce to register
-
-        Returns:
-            INopeInstance: The instance.
-        """
-        self._instances[instance.identifier] = ensureDottedAccess({
-            'instance': instance,
-            'usedBy': [],
-            'manual': True
-        }
-        )
-
-        self._internalInstances.add(instance.identifier)
-
-        await self._sendAvailableInstances()
-
-        return instance
-
-    async def deleteInstance(self, instance, preventSendingUpdate=False) -> bool:
-        """ Disposes an instance and removes it. Thereby the Instance wont be available for other
-            InstanceManagers in the system.
-
-        Args:
-            instance (any): The Instance to consider
-            preventSendingUpdate (bool, optional): If set to True the other systems wont be notified. This is for internal purpose only. Defaults to False.
-
-        Returns:
-            bool: The success
-        """
-        # Block to find the instance.
-        # Based on the property (string or instance)
-        # the corresponding instance object has to be select.
-
-        _instance = None
-        _identifier = None
-
-        if isinstance(instance, str):
-            _instance = self._instances.get(instance)
-            _identifier = instance
-        else:
-            for data in self._instances.values():
-                if instance == data.instance:
-                    _instance = data
-                    _identifier = data.instance.identifier
-                    break
-        try:
-            params = ensureDottedAccess({
-                'dispatcherId': self._id,
-                'identifier': _identifier
-            })
-
-            # Call the corresponding Dispose Function for the "real" instance
-            # All other elements are just accessors.
-            await self._rpcManager.performCall(
-                self.getServiceName(_identifier, "dispose"),
-                [
-                    params
-                ]
-            )
-        except BaseException as E:
-            # Only if it is an internal
-            # Instance, we do not want to
-            # throw that error, otherwise
-            # we want that error to be
-            # present.
-            if _instance:
-                pass
-            else:
-                raise E
-
-        # if the instance has been found => delete the instance.
-        if _instance:
-            _instance.usedBy.pop()
-            if len(_instance.usedBy) == 0:
-
-                # Delete the Identifier
-                self._instances.pop(_instance.instance.identifier)
-
-                # Check if an update should be emitted or not.
-                if not preventSendingUpdate:
-                    # Update the Instances provided by this module.
-                    await self._sendAvailableInstances()
-
-            return True
-        return False
-
-    async def getInstancesOfType(self, typeToGet: str):
-        """ Creates Wrappers for the Type of the given element.
-
-        Args:
-            typeToGet (str): Type of the instances to get the wrappers for.
-
-        Returns:
-            list: List containing all kown Elements of the given type.
-        """
-
-        indentifier = map(lambda item: item.identifier, filter(
-            lambda item: item.type == typeToGet, self.instances.data.getContent()))
-
-        promises = []
-
-        for identifier in indentifier:
-            promises.append(
-                self.createInstance(
-                    ensureDottedAccess({
-                        'identifier': identifier,
-                        'type': typeToGet,
-                        'params': []
-                    })
-                )
-            )
-
-        # Wait to generate all Instances.
-        if promises:
-            result = await asyncio.gather(*promises)
-        return result
-
-    def reset(self):
-        self._mappingOfRemoteDispatchersAndGenerators.clear()
-        self._mappingOfRemoteDispatchersAndInstances.clear()
-        self.constructors.update()
-        self.instances.update()
-        self._internalWrapperGenerators = dict()
-        self._registeredConstructors = dict()
-
-        # If Instances Exists => Delete them.
-        if self._instances:
-
-            promises = []
-
-            # Dispose all Instances.
-            for name, instance in self._instances.items():
-
-                def onDone(p):
-                    if p.exception() and self._logger:
-                        self._logger.error(
-                            'Failed Removing Instance "' + name + '"')
-                        self._logger.error(formatException(e))
-
-                promise: asyncio.Future = self.deleteInstance(name, True)
-                promise.add_done_callback(onDone)
-
-                if self._logger:
-                    self._logger.warn('Disposing instance "' + name + '"')
-
-                promises.append(promise)
-
-            EXECUTOR.callParallel(asyncio.gather, *promises)
-
-        self._instances = dict()
-        self._externalInstances = dict()
-        self._internalInstances = set()
-        self._initializingInstance = dict()
-        self._externalInstancesNames = set()
-        self.internalInstances.setContent([])
-
-        if self._communicator.connected.getContent():
-            EXECUTOR.callParallel(self._sendAvailableInstances)
-
-    async def dispose(self):
-        self.reset()
-        self.instances.dispose()
-        self.__disposed = True
-
-    def __del__(self):
-        if not self.__disposed:
-            EXECUTOR.callParallel(self.dispose)
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+import asyncio
+import json
+
+from nope.communication.bridge import Bridge
+from nope.dispatcher.connectivityManager import NopeConnectivityManager
+from nope.dispatcher.rpcManager import NopeRpcManager
+from nope.helpers import SPLITCHAR, ensureDottedAccess, generateId, isIterable, EXECUTOR, waitFor, varifyPath, formatException
+from nope.logger import defineNopeLogger
+from nope.merging import DictBasedMergeData
+from nope.modules import NopeGenericModule
+from nope.observable import NopeObservable
+
+
+class NopeInstanceManager:
+
+    def __init__(self, options, _defaultSelector, _id=None,
+                 _connectivityManager=None, _rpcManager=None, _core=None):
+
+        self.options = options
+        self._defaultSelector = _defaultSelector
+        self._id = _id
+        self._connectivityManager = _connectivityManager
+        self._rpcManager = _rpcManager
+        self._core = _core
+        self._communicator: Bridge = options.communicator
+        self.__disposed = False
+
+        if _id is None:
+            self._id = generateId()
+        if _connectivityManager is None:
+            self._connectivityManager = NopeConnectivityManager(
+                options, id=self._id)
+        if _rpcManager is None:
+            self._rpcManager = NopeRpcManager(
+                options,
+                self._defaultSelector,
+                id=self._id,
+                connectivityManager=self._connectivityManager
+            )
+
+        self._logger = defineNopeLogger(
+            options.logger, 'core.instance-manager')
+
+        # Flag to indicate, that the system is ready.
+        self.ready = NopeObservable()
+        self.ready.setContent(False)
+
+        self._mappingOfRemoteDispatchersAndGenerators = dict()
+        # Overview of the available Constructors in the network.
+        self.constructors = DictBasedMergeData(
+            self._mappingOfRemoteDispatchersAndGenerators, '+', '+')
+        self._mappingOfRemoteDispatchersAndInstances = dict()
+
+        # Overview of the available instances in the network.
+        #   - OriginalKey = DispatcherID (string);
+        #   - OriginalValue = Available Instance Messages (IAvailableInstancesMsg);
+        #   - ExtractedKey = The name of the Instance (string);
+        #   - ExtractedValue = instance-description (INopeModuleDescription);
+        self.instances = DictBasedMergeData(
+            self._mappingOfRemoteDispatchersAndInstances, 'instances/+', 'instances/+/identifier')
+
+        self._internalWrapperGenerators = dict()
+        self._registeredConstructors = dict()
+        self._instances = dict()
+        self._externalInstances = dict()
+        self._internalInstances = set()
+        self._initializingInstance = dict()
+        self._externalInstancesNames = set()
+
+        # Contains the identifiers of the instances, which are hosted in the
+        # provided dispatcher.
+        self.internalInstances = NopeObservable()
+        self.internalInstances.setContent([])
+
+        self.constructorServices = NopeObservable()
+        self.constructorServices.setContent([])
+
+        _ctorStart = f'nope{SPLITCHAR}core{SPLITCHAR}constructor{SPLITCHAR}'
+
+        def _extractGenerators(*args):
+
+            constructorServices = set()
+
+            self._mappingOfRemoteDispatchersAndGenerators.clear()
+            for dispatcher, services in self._rpcManager.services.originalData.items():
+                def _filterMatchingServices(svc):
+                    if "id" in svc and svc.id.startswith(_ctorStart):
+                        constructorServices.add(svc["id"])
+                        return True
+                    return False
+
+                generators = list(
+                    map(
+                        lambda item: item.id[len(_ctorStart):],
+                        filter(
+                            _filterMatchingServices,
+                            services.services
+                        )
+                    )
+                )
+
+                if len(generators):
+                    self._mappingOfRemoteDispatchersAndGenerators[dispatcher] = generators
+
+            self.constructorServices.setContent(list(constructorServices))
+            self.constructors.update()
+
+        # Subscribe to changes.
+        self._rpcManager.services.data.subscribe(_extractGenerators)
+
+        if self._logger:
+            self._logger.info('core.instance-manager online')
+
+        self.reset()
+        EXECUTOR.callParallel(self._init)
+
+    async def _sendAvailableInstances(self):
+        # Update the Instances provided by this module.
+        await self._communicator.emit(
+            "instancesChanged",
+            {
+                "dispatcher": self._id,
+                # We will send the descriptions.
+                # Generate the Module Description for every identifier:
+                "instances": list(
+                    map(lambda item: self._instances[item]["instance"].toDescription(), self._internalInstances))
+            }
+        )
+
+        # Update the Instances
+        self.internalInstances.setContent(list(self._internalInstances))
+
+    async def _init(self):
+
+        await self._communicator.connected.waitFor()
+        await self._connectivityManager.ready.waitFor()
+        await self._rpcManager.ready.waitFor()
+
+        async def _generateWrapper(dispather, description):
+            mod = NopeGenericModule(
+                dispather,
+                # self._generateEmitter,
+                # self._generateObservable
+            )
+            await mod.fromDescription(description, "overwrite")
+            return mod
+
+        self.registerInternalWrapperGenerator(
+            "*",
+            _generateWrapper
+        )
+
+        def _onDispatchersChanged(changes, *args):
+            """ Callback which will handle new and offline Dispatchers.
+            """
+
+            if len(changes.added):
+                # If there are dispatchers online,
+                # We will emit our available services.
+                EXECUTOR.callParallel(self._sendAvailableInstances)
+
+            if len(changes.removed):
+                # Remove the dispatchers.
+                for removedId in changes.removed:
+                    self.removeDispatcher(removedId)
+
+        # We will use our status-manager to listen to changes.
+        self._connectivityManager.dispatchers.onChange.subscribe(
+            _onDispatchersChanged)
+
+        # Make shure we are emitting the instances provided.
+        await self._communicator.on("bonjour", lambda *args: EXECUTOR.callParallel(self._sendAvailableInstances))
+
+        def _onInstancesChanged(message, *args):
+            """ Callback which will be called if the commincator receives a Message
+                that some instances has been changed.
+
+            Args:
+                message: The Message from the System.
+            """
+            # Store the instance.
+            self._mappingOfRemoteDispatchersAndInstances[message.dispatcher] = message
+
+            # Update the Mapping
+            self.instances.update()
+
+            if self._logger:
+                self._logger.debug(
+                    'Remote Dispatcher "' + str(message.dispatcher) + '" updated its available instances')
+
+        # Listen to the Changes.
+        await self._communicator.on("instancesChanged", _onInstancesChanged)
+
+        if self._logger:
+            self._logger.debug("core.instance-manager " +
+                               str(self._id) + " initialized")
+
+        self.ready.setContent(True)
+
+    def getServiceName(self, name: str, type: str) -> str:
+        """ Helper to get the corresponding Service name
+
+        Args:
+            name (str): Name of the Service
+            _type (str): The desired type of the requested service name. Could be "dispose" or "constructor"
+
+        Returns:
+            str: The Adapted Name
+        """
+        if type == "constructor":
+            return f"nope{SPLITCHAR}core{SPLITCHAR}constructor{SPLITCHAR}{name}"
+        elif type == "dispose":
+            return f"nope{SPLITCHAR}core{SPLITCHAR}destructor{SPLITCHAR}{name}"
+        else:
+            raise Exception("The given type is not correct.")
+
+    def _getInstanceInfo(self, identifier: str):
+        """ Function, that will extract the information of the instance and the providing dispatcher.
+
+        Args:
+            identifier (str): The identifier of instance
+        """
+        # First check if the instance exists.
+        if not self.instanceExists(identifier, False):
+            return None
+
+        ret = ensureDottedAccess({})
+
+        # First we check if we are taking care of an internal instance, if so
+        # we will use this instance to enrich the description, otherwise, we
+        # will look in the external instances.
+        if identifier in self._instances:
+            ret.description = self._instances[identifier].instance.toDescription(
+            )
+        else:
+            for item in self._mappingOfRemoteDispatchersAndInstances.values():
+                instances = item.instances
+
+                for instance in instances:
+                    if instance.identifier == identifier:
+                        ret.description = instance
+                        break
+
+        ret.dispatcher = self.getManagerOfInstance(identifier)
+
+        return ret
+
+    def removeDispatcher(self, dispatcher: str):
+        """  Helper to remove a dispatcher.
+
+        Args:
+            dispatcher (str): The Id of the Dispatcher
+        """
+        if self._mappingOfRemoteDispatchersAndInstances.pop(dispatcher, False):
+            self.instances.update()
+
+    async def registerConstructor(self, identifier: str, cb):
+        """ Registers a Constructor, that enables other NopeInstanceManagers to create an instance of the given type. Therefore a callback "cb" is registered with the given "typeIdentifier"
+
+        Args:
+            identifier (str): The identifier for the Constructor (Like a service)
+            cb (function): The callback used, to create an instance. The Callback receives the following parameters (NopeCore, identifier:str)
+        """
+
+        if self._logger:
+            self._logger.debug(
+                'Adding instance generator for "' + (identifier +
+                                                     '" to external Generators. Other Elements can now create instances of self type.'
+                                                     ))
+
+        async def createInstance(data):
+
+            # Check if an instance exists or not.
+            # if not => create an instance an store it.
+
+            if data.identifier not in self._instances:
+                hashableData = [data.identifier, data.params, data.type]
+                try:
+                    hashed = hash(hashableData)
+                except BaseException as E:
+                    hashed = json.dumps(hashableData)
+
+                # It might happen, that an instance is requested multiple times.
+                # therefore we have to make shure, we wont create them multiple times:
+                # We will test it by using the "_internalInstances" set
+
+                if data.identifier not in self._initializingInstance:
+
+                    try:
+
+                        # Mark the Instance as available.
+                        self._initializingInstance[data.identifier] = hashed
+
+                        # Create the Instance
+                        _instance = await cb(self._core, data.identifier)
+                        _instance.identifier = data.identifier
+
+                        # Make shure the Data is expressed as Array.
+                        if not isIterable(data.params):
+                            data.params = [data.params]
+
+                        # Initialize the instance with the parameters.
+                        await _instance.init(*data.params)
+
+                        async def disposeInstance(_data):
+                            """ A Function is registered, taking care of removing
+                                an instances, if it isnt needed any more.
+
+                            Args:
+                                _data (msg): The message containing the dispatcher id.
+                            """
+
+                            _data = ensureDottedAccess(_data)
+
+                            if self._instances.get(data.identifier).usedBy:
+                                try:
+
+                                    if _data.dispatcherId in self._instances.get(
+                                            data.identifier).usedBy:
+                                        # Pop the dispatcher if it is present:
+                                        idx = self._instances.get(
+                                            data.identifier).usedBy.index(
+                                            _data.dispatcherId)
+                                        self._instances.get(
+                                            data.identifier).usedBy.pop(idx)
+
+                                    if len(self._instances.get(
+                                            data.identifier).usedBy) == 0:
+                                        # Unmark as internal instance
+                                        self._internalInstances.remove(
+                                            data.identifier)
+                                        # Remove the Instance.
+                                        await _instance.dispose()
+                                        # Removes the instances
+                                        self._instances.pop(data.identifier)
+                                        # Remove the Function itself
+                                        await self._rpcManager.unregisterService(self.getServiceName(data.identifier, 'dispose'))
+                                        # Emit the instances again
+                                        await self._sendAvailableInstances()
+
+                                except ValueError:
+                                    pass
+
+                        # A Function is registered, taking care of removing
+                        # an instances, if it isnt needed any more.
+                        await self._rpcManager.registerService(
+                            disposeInstance,
+                            ensureDottedAccess({
+                                'id': self.getServiceName(data.identifier, 'dispose'),
+                                'schema': ensureDottedAccess({
+                                    'description': f'Service, which will destructor for the instance "{data.identifier}". This function will be called internal only.',
+                                    'type': 'function'})
+                            })
+                        )
+
+                        # Store the Instance.
+                        self._instances[data.identifier] = ensureDottedAccess({
+                            'instance': _instance,
+                            'usedBy': [data.dispatcherId]
+                        })
+
+                        self._internalInstances.add(data.identifier)
+
+                        # Update the available instances:
+                        await self._sendAvailableInstances()
+
+                        # Make shure, we remove this instance.hash
+                        self._initializingInstance.pop(data.identifier)
+
+                    except BaseException as E:
+                        # Make shure, we remove this instance.hash
+                        self._initializingInstance.pop(data.identifier)
+
+                        raise E
+
+                elif self._initializingInstance.get(data.identifier) != hashed:
+                    raise Exception(
+                        'Providing different Parameters for the same Identifier'
+                    )
+                else:
+                    # Check if the Instance is ready.
+                    firstHint = True
+
+                    def checker():
+                        nonlocal firstHint
+                        if firstHint:
+                            self._logger.warn(
+                                f'Parallel request for the same Instance "{data.identifier}" => Waiting until the Instance has been initialized')
+                            firstHint = False
+                        return data.identifier in self._instances
+
+                    await waitFor(
+                        checker,
+                        ensureDottedAccess({
+                            'testFirst': True,
+                            'delay': 100
+                        })
+                    )
+            else:
+                # If an Element exists => Add the Element.
+                self._instances.get(data.identifier).usedBy.append(
+                    data.dispatcherId)
+
+            # Define the Response.
+            response = ensureDottedAccess({
+                'description': self._instances.get(data.identifier).instance.toDescription(),
+                'type': data.type
+            })
+
+            # Send the Response
+            return response
+
+        _cb = await self._rpcManager.registerService(
+            createInstance,
+            ensureDottedAccess({
+                # We will add the Name to our service.
+                'id': self.getServiceName(identifier, 'constructor'),
+                # We dont want to have a Prefix for construcors
+                'addNopeServiceIdPrefix': False,
+                'schema': ensureDottedAccess({
+                    'description': f'Service, which will create an construtor for the type "{identifier}".',
+                    'type': 'function'
+                })
+            })
+        )
+
+        # Store a generator
+        self._registeredConstructors[identifier] = _cb
+
+    async def unregisterConstructor(self, identifier: str):
+        """ Unregisters a present Constructor. After this, created instances are still valid, the user isnt able to create new ones.
+
+        Args:
+            identifier (str): The identifier for the Constructor (Like a service)
+        """
+        if identifier in self._registeredConstructors:
+            if self._logger:
+                self._logger.debug('Removing instance generator for "' + identifier +
+                                   '" from external Generators. Other Elements cant create instances of self type anymore.')
+
+            # We will just unregister the service from our
+            # system. Therefore we just use the rpcManager
+
+            await self._rpcManager.unregisterService(self._registeredConstructors.get(identifier))
+            self._registeredConstructors.pop(identifier)
+
+    def registerInternalWrapperGenerator(self, identifier: str, cb):
+        """ Defaultly a generic wrapper will be returned, when an instance is created. you
+            can specifiy specific wrapper type for different "typeIdentifier" with this method.
+
+        Args:
+            identifier (str): The identifier for the Constructor (Like a service)
+            cb (function): The Callback which creates the specific wrapper.
+        """
+        if self._logger:
+            self._logger.debug('Adding instance generator for "' + identifier +
+                               '" as internal Generator. This Generator wont be used externally.')
+
+        self._internalWrapperGenerators[identifier] = cb
+
+    def unregisterInternalWrapperGenerator(self, identifier: str):
+        """ Removes a specific generator for for a wrapper.
+
+        Args:
+            identifier (str): The identifier for the Constructor (Like a service)
+        """
+        if self._logger:
+            self._logger.debug('Rmoving instance generator for "' + identifier +
+                               '" from internal Generator. The sytem cant create elements of self type any more.')
+
+        self._internalWrapperGenerators.pop(identifier)
+
+    def instanceExists(self, identifier: str, externalOnly=True) -> bool:
+        """  Helper, to test if an instance with the given identifier exists or not.
+
+        Args:
+            identifier (str):  identifier of the instance.
+            externalOnly (bool, optional): If set to true we will only look for external instances in the external dispatchers. Defaults to True.
+
+        Returns:
+            bool: The Testresult
+        """
+        if identifier not in self.instances.simplified:
+            return False
+
+        if externalOnly:
+            manager = self.getManagerOfInstance(identifier)
+            return manager["id"] != self._id
+
+        return True
+
+    def getManagerOfInstance(self, identifier: str):
+        """ Returns the hosting dispatcher for the given instance.
+
+        Args:
+            identifier (str): The identifier for instance (its name)
+
+        Returns:
+            INopeStatusInfo | False: The Status or false if not present.
+        """
+        # First we will check if the instance is available internally
+        if identifier in self._internalInstances:
+            return self._connectivityManager.info
+
+        # If that isnt the case, we will check all dispatchers and search the
+        # instance.
+        for iter_item in self._mappingOfRemoteDispatchersAndInstances.items():
+            dispatcher = iter_item[0]
+            msg = iter_item[1]
+            for instance in msg.instances:
+                if instance.identifier == identifier:
+                    return self._connectivityManager.getStatus(dispatcher)
+
+        return None
+
+    def getInstanceDescription(self, instanceIdentifier: str):
+        """ Returns the instance Description for a specific instance. It is just a simplified wrapper
+            for the "instances"-property.
+
+        Args:
+            instanceIdentifier (str): The identifier for instance (its name)
+
+        Returns:
+            INopeModuleDescription | False: The Description or False if not found.
+        """
+        if instanceIdentifier in self._instances:
+            return self._instances.get(
+                instanceIdentifier).instance.toDescription()
+
+        for data in self._mappingOfRemoteDispatchersAndInstances.values():
+            instances = data.get("instances", [])
+            for instance in instances:
+                if instance["identifier"] == instanceIdentifier:
+                    return instance
+
+        return False
+
+    def constructorExists(self, typeIdentifier: str) -> bool:
+        """ Helper to test if a constructor linkt to the provided "typeIdentifier" exists or not.
+
+        Args:
+            typeIdentifier (str): The identifier for the Constructor (Like a service)
+
+        Returns:
+            bool: _description_
+        """
+        return typeIdentifier in self.constructors.data.getContent()
+
+    async def createInstance(self, description, options=None):
+        """ Allows to create an instance. This might be the case on remote dispatchers or
+            on the same element. Only a wrapper is returned, which communicates with a
+            dispatcher, because we dont know where the element is provided. You can use the
+            method "getDispatcherForInstance" to determine the dispatcher running the instance.
+
+            The returned wrapper acts like a normal "internal" class.
+
+        Args:
+            description (dict-like): Description of the instance to be created
+            options (dict-like, optional): Options used during creating the instance.. Defaults to None.
+
+
+        Returns:
+            NopeGenericModule | Registered Wrapper: An Generic Nope Module as Wrapper or a custom wrapper for the class.
+        """
+
+        # Define the Default Description
+        # which will lead to an error.
+
+        options = ensureDottedAccess(options)
+        description = ensureDottedAccess(description)
+
+        # Assign the provided Description
+        _description = ensureDottedAccess({
+            'dispatcherId': self._id,
+            'identifier': 'error',
+            'params': [],
+            'type': 'unkown'
+        })
+        _description.update(description)
+        _description.update({'dispatcherId': self._id})
+
+        # Check if the Description is complete
+        if (_description.type == 'unkown' or _description.identifier) == 'error':
+            raise Exception(
+                'Please Provide at least a "type" and "identifier" in the paremeters')
+
+        # Use the varified Name (removes the invalid chars.)
+        _description.identifier = varifyPath(
+            _description.identifier) if self.options.forceUsingValidVarNames else _description.identifier
+        if self._logger:
+            self._logger.debug('Requesting an Instance of type: "' + _description.type +
+                               '" with the identifier: "' + str(_description.identifier) + '"')
+
+        try:
+            _type = _description.type
+            if _type not in self._internalWrapperGenerators:
+                _type = '*'
+
+            if not self.constructorExists(_description.type):
+                # No default type is present for a remote
+                # => assing the default type which is "*""
+                raise Exception('Generator "' + _description.type +
+                                '" isnt present in the network!')
+            if _type in self._internalWrapperGenerators:
+                if self._logger:
+                    self._logger.debug('No instance with the identifiert: "' + str(_description.identifier) +
+                                       '" found, but an internal generator is available. Using the internal one for creating the instance and requesting the "real" instance externally')
+
+                # Now test if there is allready an instance with this name and type.
+                # If so, we check if we have the correct type etc. Additionally we
+                # try to extract its dispatcher-id and will use that as selector
+                # to allow the function be called.
+
+                _instanceDetails = self._getInstanceInfo(
+                    _description.identifier)
+
+                usedDispatcher = None
+
+                if _instanceDetails is not None and _instanceDetails.description.type != _description.type:
+                    raise Exception(
+                        "There exists an Instance named: '" + str(_description.identifier) + "' but it uses a different type. Requested type: '" +
+                        _description.type + "', given type: '" + str(_instanceDetails.description.type) + "'")
+
+                elif _instanceDetails is not None:
+                    usedDispatcher = _instanceDetails.dispatcher.id
+
+                if usedDispatcher and options.assignmentValid:
+
+                    # If we have an dispatcher, which was been used to create the instance,
+                    # we have to check, the selected Dispatcher Matches our
+                    # criteria.
+
+                    if not await options.assignmentValid(_instanceDetails.description, _instanceDetails.dispatcher):
+                        raise Exception('Assignment is invalid.')
+
+                definedInstance = await self._rpcManager.performCall(
+                    self.getServiceName(_description.type, 'constructor'),
+                    [
+                        _description
+                    ],
+                    options
+                )
+
+                if self._logger:
+                    self._logger.debug(
+                        f'Received a description for the instance "{definedInstance.description.identifier}"')
+
+                # Create the Wrapper for our instance.
+                wrapper = await self._internalWrapperGenerators.get(_type)(self._core, definedInstance.description)
+                if self._logger:
+                    self._logger.debug(
+                        f'Created a Wrapper for the instance "{definedInstance.description.identifier}"')
+
+                originalDispose = wrapper.dispose
+
+                async def dispose():
+                    await self.deleteInstance(wrapper.identifier)
+
+                    await originalDispose()
+
+                setattr(wrapper, "dispose", dispose)
+
+                self._instances[_description.identifier] = ensureDottedAccess({
+                    'instance': wrapper,
+                    'usedBy': [
+                        _description.dispatcherId
+                    ]
+                }
+                )
+
+                return wrapper
+
+            raise Exception('No internal generator Available!')
+
+        except Exception as e:
+
+            if self._logger:
+                self._logger.error(
+                    'During creating an Instance, the following error Occurd')
+                self._logger.error(formatException(e))
+
+            raise e
+
+    async def generateWrapper(self, description):
+        # Define the Default Description
+        # which will lead to an error.
+        description = ensureDottedAccess(description)
+
+        # Assign the provided Description
+        _description = ensureDottedAccess({
+            'dispatcherId': self._id,
+            'identifier': 'error',
+            'params': [],
+            'type': 'unkown'
+        })
+        _description.update(description)
+        _description.update({'dispatcherId': self._id})
+
+        # Check if the Description is complete
+        if (_description.type == 'unkown' or _description.identifier) == 'error':
+            raise Exception(
+                'Please Provide at least a "type" and "identifier" in the paremeters')
+
+        # Use the varified Name (removes the invalid chars.)
+        _description.identifier = varifyPath(
+            _description.identifier) if self.options.forceUsingValidVarNames else _description.identifier
+        if self._logger:
+            self._logger.debug('Requesting an Instance of type: "' + _description.type +
+                               '" with the identifier: "' + str(_description.identifier) + '"')
+
+        try:
+            _type = _description.type
+            if _type not in self._internalWrapperGenerators:
+                _type = '*'
+
+            if not self.constructorExists(_description.type):
+                # No default type is present for a remote
+                # => assing the default type which is "*""
+                raise Exception('Generator "' + _description.type +
+                                '" isnt present in the network!')
+            if _type in self._internalWrapperGenerators:
+                if self._logger:
+                    self._logger.debug('No instance with the identifiert: "' + str(_description.identifier) +
+                                       '" found, but an internal generator is available. Using the internal one for creating the instance and requesting the "real" instance externally')
+
+                # Now test if there is allready an instance with this name and type.
+                # If so, we check if we have the correct type etc. Additionally we
+                # try to extract its dispatcher-id and will use that as selector
+                # to allow the function be called.
+
+                _instanceDetails = self._getInstanceInfo(
+                    _description.identifier)
+
+                if _instanceDetails is not None and _instanceDetails.description.type != _description.type:
+                    raise Exception(
+                        "There exists an Instance named: '" + str(_description.identifier) + "' but it uses a different type. Requested type: '" +
+                        _description.type + "', given type: '" + str(_instanceDetails.description.type) + "'")
+
+                elif _instanceDetails is None:
+                    raise Exception(
+                        'No instance known with the idenfitier "' + str(_description.identifier) + '" !')
+
+                definedInstance = _instanceDetails.description
+
+                # Create the Wrapper for our instance.
+                wrapper = await self._internalWrapperGenerators.get(_type)(self._core, definedInstance.description)
+                if self._logger:
+                    self._logger.debug(
+                        f'Created a Wrapper for the instance "{definedInstance.description.identifier}"')
+
+                originalDispose = wrapper.dispose
+
+                async def dispose():
+                    await self.deleteInstance(wrapper.indentifier)
+
+                    await originalDispose()
+
+                setattr(wrapper, "dispose", dispose)
+
+                self._instances[_description.identifier] = ensureDottedAccess({
+                    'instance': wrapper,
+                    'usedBy': [
+                        _description.dispatcherId
+                    ]
+                }
+                )
+
+                return wrapper
+
+            raise Exception('No internal generator Available!')
+
+        except Exception as e:
+
+            if self._logger:
+                self._logger.error(
+                    'During creating an Instance, the following error Occurd')
+                self._logger.error(formatException(e))
+
+            raise e
+
+    async def registerInstance(self, instance):
+        """ Option, to statically register an instance, without using an specific generator etc.
+            This instance is just present in the network.
+
+        Args:
+            instance (INopeInstance): The Instnce to register
+
+        Returns:
+            INopeInstance: The instance.
+        """
+        self._instances[instance.identifier] = ensureDottedAccess({
+            'instance': instance,
+            'usedBy': [],
+            'manual': True
+        }
+        )
+
+        self._internalInstances.add(instance.identifier)
+
+        await self._sendAvailableInstances()
+
+        return instance
+
+    async def deleteInstance(self, instance, preventSendingUpdate=False) -> bool:
+        """ Disposes an instance and removes it. Thereby the Instance wont be available for other
+            InstanceManagers in the system.
+
+        Args:
+            instance (any): The Instance to consider
+            preventSendingUpdate (bool, optional): If set to True the other systems wont be notified. This is for internal purpose only. Defaults to False.
+
+        Returns:
+            bool: The success
+        """
+        # Block to find the instance.
+        # Based on the property (string or instance)
+        # the corresponding instance object has to be select.
+
+        _instance = None
+        _identifier = None
+
+        if isinstance(instance, str):
+            _instance = self._instances.get(instance)
+            _identifier = instance
+        else:
+            for data in self._instances.values():
+                if instance == data.instance:
+                    _instance = data
+                    _identifier = data.instance.identifier
+                    break
+        try:
+            params = ensureDottedAccess({
+                'dispatcherId': self._id,
+                'identifier': _identifier
+            })
+
+            # Call the corresponding Dispose Function for the "real" instance
+            # All other elements are just accessors.
+            await self._rpcManager.performCall(
+                self.getServiceName(_identifier, "dispose"),
+                [
+                    params
+                ]
+            )
+        except BaseException as E:
+            # Only if it is an internal
+            # Instance, we do not want to
+            # throw that error, otherwise
+            # we want that error to be
+            # present.
+            if _instance:
+                pass
+            else:
+                raise E
+
+        # if the instance has been found => delete the instance.
+        if _instance:
+            _instance.usedBy.pop()
+            if len(_instance.usedBy) == 0:
+
+                # Delete the Identifier
+                self._instances.pop(_instance.instance.identifier)
+
+                # Check if an update should be emitted or not.
+                if not preventSendingUpdate:
+                    # Update the Instances provided by this module.
+                    await self._sendAvailableInstances()
+
+            return True
+        return False
+
+    async def getInstancesOfType(self, typeToGet: str):
+        """ Creates Wrappers for the Type of the given element.
+
+        Args:
+            typeToGet (str): Type of the instances to get the wrappers for.
+
+        Returns:
+            list: List containing all kown Elements of the given type.
+        """
+
+        indentifier = map(lambda item: item.identifier, filter(
+            lambda item: item.type == typeToGet, self.instances.data.getContent()))
+
+        promises = []
+
+        for identifier in indentifier:
+            promises.append(
+                self.createInstance(
+                    ensureDottedAccess({
+                        'identifier': identifier,
+                        'type': typeToGet,
+                        'params': []
+                    })
+                )
+            )
+
+        # Wait to generate all Instances.
+        if promises:
+            result = await asyncio.gather(*promises)
+        return result
+
+    def reset(self):
+        self._mappingOfRemoteDispatchersAndGenerators.clear()
+        self._mappingOfRemoteDispatchersAndInstances.clear()
+        self.constructors.update()
+        self.instances.update()
+        self._internalWrapperGenerators = dict()
+        self._registeredConstructors = dict()
+
+        # If Instances Exists => Delete them.
+        if self._instances:
+
+            promises = []
+
+            # Dispose all Instances.
+            for name, instance in self._instances.items():
+
+                def onDone(p):
+                    if p.exception() and self._logger:
+                        self._logger.error(
+                            'Failed Removing Instance "' + name + '"')
+                        self._logger.error(formatException(e))
+
+                promise: asyncio.Future = self.deleteInstance(name, True)
+                promise.add_done_callback(onDone)
+
+                if self._logger:
+                    self._logger.warn('Disposing instance "' + name + '"')
+
+                promises.append(promise)
+
+            EXECUTOR.callParallel(asyncio.gather, *promises)
+
+        self._instances = dict()
+        self._externalInstances = dict()
+        self._internalInstances = set()
+        self._initializingInstance = dict()
+        self._externalInstancesNames = set()
+        self.internalInstances.setContent([])
+
+        if self._communicator.connected.getContent():
+            EXECUTOR.callParallel(self._sendAvailableInstances)
+
+    async def dispose(self):
+        self.reset()
+        self.instances.dispose()
+        self.__disposed = True
+
+    def __del__(self):
+        if not self.__disposed:
+            EXECUTOR.callParallel(self.dispose)
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/nopeDispatcher.py` & `nope_py-1.7.9/nope/dispatcher/nopeDispatcher.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from nope.dispatcher.core import NopeCore
-from nope.helpers.pathMatchingMethods import comparePatternAndPath, ensureDottedAccess
-
-
-class NopeDispatcher(NopeCore):
-    """  A Dispatcher to perform a function on a Remote Dispatcher. Therefore a Task is created and forwarded to the remote.
-    """
-
-    @property
-    def masterExists(self):
-        return self.connectivityManager.master.isMasterForced
-
-    def pushData(self, path: str, content, options=None) -> None:
-        """ Pushs the desired data into the system.
-        Args:
-            path (str): The path to the Data.
-            content (any): The Content to Push
-            options (dict-like, optional): The Options during pushing. Defaults to None.
-        """
-        options = ensureDottedAccess(options)
-        return self.dataDistributor.pushData(path, content, options)
-
-    def pullData(self, path: str, _default=None):
-        """ Helper to pull some data from the system.
-
-        Args:
-            path (str): The path to the Data.
-            _default (any, optional): The value to use if no data has been found. If not provided an error is thrown. Defaults to None.
-
-        Returns:
-            any: The data or default type (if set)
-        """
-        return self.dataDistributor.pullData(path, _default)
-
-    def subscribeToEvent(self, event: str, callback):
-        """ Helper to subscribe to specific events.
-
-        Args:
-            event (str): Name of the event to listen to.
-            callback (callable): the Callback to use. Must receive *args.
-
-        Returns:
-            Observer: Observer for the Subcription. contains the methods "pause", "unpause" and "unsubscribe"
-        """
-        return self.eventDistributor.registerSubscription(event, callback)
-
-    def emitEvent(self, eventName, data, options=None):
-        """ Emits an event with the given name. All event-subscriber, where the topic matches will receive this notification.
-
-        Args:
-            event (str): Name of the event to emii.
-            data (any): The data to emit.
-            options (dict-like): will be added to the event (for instance timestamp, sender, etc.)
-        """
-        options = ensureDottedAccess(options)
-        self.eventDistributor.emit(eventName, data, options)
-
-    def query(self, pattern: str, type: str) -> list:
-        """ Receive the "instances" | "services" | "properties" | "events"
-            which matches with the given pattern. Therefore the user provides
-            the pattern and type.
-            @return {string[]} List of the matching items.
-
-        Args:
-            pattern (str): pattern Pattern to query the provided type.
-            type (str): type which should be querried. Allowed values are: "instances" | "services" | "properties" | "events"
-        """
-
-        items = []
-
-        if type == 'instances':
-
-            def callback_0(item):
-                return item.identifier
-
-            items = map(callback_0, self.instanceManager.
-                        instances.data.getContent())
-        elif type == 'services':
-            items = list(self.rpcManager.services.simplified.keys())
-        elif type == 'properties':
-            items = self.dataDistributor.publishers.data.getContent()
-        elif type == 'events':
-            items = self.eventDistributor.publishers.data.getContent()
-        else:
-            raise Exception('Invalid Type-Parameter')
-
-        return list(filter(lambda item: comparePatternAndPath(
-            pattern, item).affected, items))
-
-    def getAllHosts(self):
-        hosts = set()
-        for info in self.connectivityManager.dispatchers.originalData.values():
-            hosts.add(info.host.name)
-        return list(hosts)
-
-    def toDescription(self):
-
-        ret = self.connectivityManager.info.copy()
-        ret.update(
-            ensureDottedAccess({
-                'isMaster': self.connectivityManager.isMaster,
-                'instances': self.instanceManager.instances.data.getContent(),
-                'services': self.rpcManager.services.data.getContent(),
-                'events': self.eventDistributor.emitters,
-                'properties': self.dataDistributor.emitters,
-                'data': self.dataDistributor.pullData('', dict())
-            })
-        )
-
-        return ret
+from nope.dispatcher.core import NopeCore
+from nope.helpers.pathMatchingMethods import comparePatternAndPath, ensureDottedAccess
+
+
+class NopeDispatcher(NopeCore):
+    """  A Dispatcher to perform a function on a Remote Dispatcher. Therefore a Task is created and forwarded to the remote.
+    """
+
+    @property
+    def masterExists(self):
+        return self.connectivityManager.master.isMasterForced
+
+    def pushData(self, path: str, content, options=None) -> None:
+        """ Pushs the desired data into the system.
+        Args:
+            path (str): The path to the Data.
+            content (any): The Content to Push
+            options (dict-like, optional): The Options during pushing. Defaults to None.
+        """
+        options = ensureDottedAccess(options)
+        return self.dataDistributor.pushData(path, content, options)
+
+    def pullData(self, path: str, _default=None):
+        """ Helper to pull some data from the system.
+
+        Args:
+            path (str): The path to the Data.
+            _default (any, optional): The value to use if no data has been found. If not provided an error is thrown. Defaults to None.
+
+        Returns:
+            any: The data or default type (if set)
+        """
+        return self.dataDistributor.pullData(path, _default)
+
+    def subscribeToEvent(self, event: str, callback):
+        """ Helper to subscribe to specific events.
+
+        Args:
+            event (str): Name of the event to listen to.
+            callback (callable): the Callback to use. Must receive *args.
+
+        Returns:
+            Observer: Observer for the Subcription. contains the methods "pause", "unpause" and "unsubscribe"
+        """
+        return self.eventDistributor.registerSubscription(event, callback)
+
+    def emitEvent(self, eventName, data, options=None):
+        """ Emits an event with the given name. All event-subscriber, where the topic matches will receive this notification.
+
+        Args:
+            event (str): Name of the event to emii.
+            data (any): The data to emit.
+            options (dict-like): will be added to the event (for instance timestamp, sender, etc.)
+        """
+        options = ensureDottedAccess(options)
+        self.eventDistributor.emit(eventName, data, options)
+
+    def query(self, pattern: str, type: str) -> list:
+        """ Receive the "instances" | "services" | "properties" | "events"
+            which matches with the given pattern. Therefore the user provides
+            the pattern and type.
+            @return {string[]} List of the matching items.
+
+        Args:
+            pattern (str): pattern Pattern to query the provided type.
+            type (str): type which should be querried. Allowed values are: "instances" | "services" | "properties" | "events"
+        """
+
+        items = []
+
+        if type == 'instances':
+
+            def callback_0(item):
+                return item.identifier
+
+            items = map(callback_0, self.instanceManager.
+                        instances.data.getContent())
+        elif type == 'services':
+            items = list(self.rpcManager.services.simplified.keys())
+        elif type == 'properties':
+            items = self.dataDistributor.publishers.data.getContent()
+        elif type == 'events':
+            items = self.eventDistributor.publishers.data.getContent()
+        else:
+            raise Exception('Invalid Type-Parameter')
+
+        return list(filter(lambda item: comparePatternAndPath(
+            pattern, item).affected, items))
+
+    def getAllHosts(self):
+        hosts = set()
+        for info in self.connectivityManager.dispatchers.originalData.values():
+            hosts.add(info.host.name)
+        return list(hosts)
+
+    def toDescription(self):
+
+        ret = self.connectivityManager.info.copy()
+        ret.update(
+            ensureDottedAccess({
+                'isMaster': self.connectivityManager.isMaster,
+                'instances': self.instanceManager.instances.data.getContent(),
+                'services': self.rpcManager.services.data.getContent(),
+                'events': self.eventDistributor.emitters,
+                'properties': self.dataDistributor.emitters,
+                'data': self.dataDistributor.pullData('', dict())
+            })
+        )
+
+        return ret
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/rpcManager/rpcManager.py` & `nope_py-1.7.9/nope/dispatcher/rpcManager/rpcManager.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,662 +1,662 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-import asyncio
-
-from nope.communication.bridge import Bridge
-from nope.dispatcher.connectivityManager import NopeConnectivityManager
-from nope.eventEmitter import NopeEventEmitter
-from nope.helpers import generateId, ensureDottedAccess, isAsyncFunction, \
-    formatException, DottedDict, SPLITCHAR, isIterable, isList, EXECUTOR
-from nope.logger import defineNopeLogger
-from nope.merging import DictBasedMergeData
-from nope.observable import NopeObservable
-
-_DEFAULT_RESULT = object()
-
-
-class WrappedFunction:
-
-    def __init__(self, func, _id, unregister):
-        self._func = func
-        self._unregister = unregister
-        self.id = _id
-        self.isAsync = isAsyncFunction(func)
-
-    def __call__(self, *args, **kwarg):
-        return EXECUTOR.callParallel(self._func, *args, **kwarg)
-
-
-class NopeRpcManager:
-
-    def __init__(self, options, defaultSelector, id=None,
-                 connectivityManager=None):
-
-        options = ensureDottedAccess(options)
-
-        self.options = options
-        self._defaultSelector = defaultSelector
-        self._id = id
-        self._communicator: Bridge = options.communicator
-        self._connectivityManager: NopeConnectivityManager = connectivityManager
-
-        self._runningInternalRequestedTasks = dict()
-        self._registeredServices = dict()
-
-        if self._id is None:
-            self._id = generateId()
-
-        if self._connectivityManager is None:
-            self._connectivityManager = NopeConnectivityManager(
-                options, self.id)
-
-        self._logger = defineNopeLogger(options.logger, 'core.rpc-manager')
-        self.ready = NopeObservable()
-        self.ready.setContent(False)
-
-        self.__warned = False
-
-        self._mappingOfDispatchersAndServices = dict()
-        self.services = DictBasedMergeData(
-            self._mappingOfDispatchersAndServices, 'services/+', 'services/+/id')
-        self.onCancelTask = NopeEventEmitter()
-
-        if self._logger:
-            self._logger.info(f'manager created id={self.id}')
-
-        self._runningExternalRequestedTasks = dict()
-
-        self.reset()
-        EXECUTOR.callParallel(self._init)
-
-    @property
-    def id(self):
-        return self._id
-
-    def updateDispatcher(self, msg):
-        self._mappingOfDispatchersAndServices[msg.dispatcher] = msg
-        self.services.update()
-
-    async def _handleExternalRequest(self, data, func: WrappedFunction | None = None):
-        try:
-            if not callable(func):
-                if data.functionId not in self._registeredServices:
-                    return
-                func = self._registeredServices[data.functionId].get(
-                    "func", None)
-
-            if self._logger:
-                self._logger.debug(
-                    f'Dispatcher "{self.id}" received request: "{data.functionId}" -> task: "{data.taskId}"')
-
-            if callable(func):
-                # Now we check, if we have to perform test, whether
-                # we are allowed to execute the task:
-                if data.get("target", self.id) != self.id:
-                    return
-
-                # Define a list containing callbacks:
-                cbs = []
-
-                observer = None
-
-                def on_cancel(reason, *args):
-                    nonlocal observer
-                    if reason.taskId == data.taskId:
-
-                        for cb in cbs:
-                            cb(reason)
-
-                        observer.unsubscribe()
-                        observer = None
-
-                observer = self.onCancelTask.subscribe(on_cancel)
-
-                # extract the arguments etc.
-                # create an empty list and fill it afterwards
-                args = [None] * len(data.params)
-                for item in data.params:
-                    args[item.idx] = item.data
-
-                _result = _DEFAULT_RESULT
-
-                if not func.isAsync and not self.__warned:
-                    if self._logger:
-                        self._logger.warn(
-                            "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                        self._logger.warn(
-                            "Offloading function to a separate thread.")
-                    else:
-                        print(
-                            "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                        print("Offloading function to a separate thread.")
-                    # We only want to warn the user once.
-                    self.__warned = True
-
-                resultPromise = func(*args)
-
-                try:
-                    if resultPromise is not None and getattr(
-                            resultPromise, 'cancelCallback', False):
-                        def _cancel_main(reason):
-                            resultPromise.cancelCallback(reason)
-
-                        cbs.append(_cancel_main)
-
-                except Exception as error:
-                    # The Cancel Function isn't available in
-                    # the provided promise.
-                    pass
-
-                self._runningExternalRequestedTasks[data.taskId] = data.requestedBy
-
-                # Wait for the Result to finish.
-                _result = await resultPromise
-
-                # Define the Result message
-                result = {
-                    'result': _result if _result is not _DEFAULT_RESULT else None,
-                    'taskId': data.taskId,
-                    'type': 'response'
-                }
-
-                if self._logger:
-                    self._logger.debug(
-                        'Internally executed requested Function for Task: ' + str(data['taskId']) + " - Function \"" +
-                        data['functionId'] + '\". Sending result on ' + str(data['resultSink']))
-
-                # Use the communicator to publish the result.
-                await self._communicator.emit("rpcResponse", result)
-
-        except Exception as error:
-
-            if self._logger:
-                self._logger.error(
-                    f'Dispatcher "{self.id}" failed with request: "{data.taskId}"')
-                self._logger.error(formatException(error))
-            else:
-                print(formatException(error))
-
-            self._runningExternalRequestedTasks.pop(data.requestedBy, None)
-
-            result = {
-                'error': {
-                    'error': str(error),
-                    'msg': str(error)
-                },
-                'taskId': data.taskId,
-                'type': 'response'
-            }
-
-            # Use the communicator to publish the result.
-            await self._communicator.emit("rpcResponse", result)
-
-    async def _handle_external_response(self, data):
-        try:
-            # Extract the Task
-            task: DottedDict = self._runningInternalRequestedTasks.get(
-                data.taskId, None)
-
-            if task:
-
-                # Based on the Result of the Remote => proceed.
-                # Either throw an error or forward the result
-                self._runningInternalRequestedTasks.pop(data.taskId)
-
-                if data.error:
-                    if self._logger:
-                        self._logger.error(
-                            "Failed with task " + str(data['taskId']))
-                        self._logger.error(
-                            "Reason: " + str(data['error']['msg']))
-                        self._logger.exception(data['error'])
-
-                    # Reject the Error:
-                    task.future.set_exception(Exception(data['error']))
-
-                    if "timeout" in task and task.timeout is not None:
-                        # Assume, that the timeout has been
-                        # defined with setTimeout
-                        task.timeout.cancel()
-
-                    return True
-
-                else:
-                    if self._logger:
-                        self._logger.debug('Got sucessfull result for Task: "' + str(
-                            data['taskId']) + '". Forwarding Result to Future.')
-
-                    task.future.set_result(data.result)
-
-                    if self._logger:
-                        self._logger.debug("Forwarded result to future")
-
-                    if "timeout" in task and task.timeout is not None:
-                        task.timeout.cancel()
-
-                    return True
-
-        except Exception as error:
-            if self._logger:
-                self._logger.error(
-                    "Error during handling an external response")
-                self._logger.error(formatException(error))
-            else:
-                print(formatException(error))
-
-        return False
-
-    async def _sendAvailableServices(self):
-        """ Function used to update the Available Services.
-        """
-
-        message = ensureDottedAccess({
-            "dispatcher": self.id,
-            "services": list(map(lambda item: item.options, self._registeredServices.values()))
-        })
-
-        if self._logger:
-            self._logger.debug("sending available services")
-
-        await self._communicator.emit("servicesChanged", message)
-
-    async def _init(self):
-        self.ready.setContent(False)
-
-        await self._communicator.connected.waitFor()
-        await self._connectivityManager.ready.waitFor()
-
-        def onServicesChanged(msg):
-            try:
-                self.updateDispatcher(msg)
-            except Exception as error:
-                if self._logger:
-                    self._logger.error("Failed to add the new services")
-                    self._logger.error(formatException(error))
-                else:
-                    print(formatException(error))
-
-        await self._communicator.on("servicesChanged", onServicesChanged)
-        await self._communicator.on("rpcRequest", lambda data: EXECUTOR.callParallel(self._handleExternalRequest, data))
-        await self._communicator.on("rpcResponse",
-                                    lambda data: EXECUTOR.callParallel(self._handle_external_response, data))
-
-        def on_cancelation(msg):
-            if msg.dispatcher == self._id:
-                self.onCancelTask.emit(msg)
-
-        await self._communicator.on("taskCancelation", on_cancelation)
-
-        def on_unregister(msg):
-            if msg.identifier in self._registeredServices:
-                self.unregisterService(msg.identifier)
-
-        await self._communicator.on("rpcUnregister", on_unregister)
-
-        # We are now listening on these changes!
-        await self._communicator.on("bonjour", lambda *args: EXECUTOR.callParallel(self._sendAvailableServices))
-
-        def onDispatchersChanged(changes, *args):
-            if len(changes.added):
-                # If there are dispatchers online,
-                # We will emit our available services.
-                EXECUTOR.callParallel(self._sendAvailableServices)
-            if len(changes.removed):
-                for rm in changes.removed:
-                    self.removeDispatcher(rm)
-
-        self._connectivityManager.dispatchers.onChange.subscribe(
-            onDispatchersChanged)
-
-        if self._logger:
-            self._logger.info(f"core.rpc-manager {self._id} initialized!")
-
-        self.ready.setContent(True)
-
-    def removeDispatcher(self, dispatcherId: str):
-        res = self._mappingOfDispatchersAndServices.pop(dispatcherId, False)
-        if (res):
-            self.services.update()
-
-            # Now we need to cancel every Task of the dispatcher,
-            # which isnt present any more.
-            EXECUTOR.callParallel(self.cancelRunningTasksOfDispatcher, dispatcherId, Exception(
-                "Dispatcher has been removed! Tasks cannot be executed any more."))
-            # Stop executing the requested Tasks.
-            EXECUTOR.callParallel(self.cancelRequestedTasksOfDispatcher, dispatcherId, Exception(
-                "Dispatcher has been removed! Tasks are not required any more."))
-
-    async def cancelTask(self, taskId: str, reason, quiet=False):
-        if taskId in self._runningInternalRequestedTasks:
-            task = self._runningInternalRequestedTasks[taskId]
-
-            # Delete the task
-            self._runningInternalRequestedTasks.pop(taskId)
-
-            # Propagate the Cancellation (internally):
-            task.future.set_exception(reason)
-
-            # Propagate the Cancellation externally.
-            # Therefore use the desired Mode.
-            await self._communicator.emit("taskCancelation", ensureDottedAccess({
-                "dispatcher": self._id,
-                "reason": str(reason),
-                "taskId": taskId,
-                "quiet": quiet
-            }))
-
-            return True
-        # Task hasnt been found => Cancel the Task.
-        return False
-
-    async def _cancelHelper(self, tasksToCancel: set, reason):
-        """ Helper Function, used to close all tasks with a specific service.
-        """
-        if len(tasksToCancel) > 0:
-            for taskId in tasksToCancel:
-                await self.cancelTask(taskId, reason)
-
-    async def cancelRunningTasksOfService(self, serviceName: str, reason):
-        """ Helper Function, used to close all tasks with a specific service.
-        """
-        # Set containing all Tasks, that has to be canceled
-        toCancel = set()
-
-        # Filter all Tasks that should be canceled.
-        for taskId, task in self._runningInternalRequestedTasks.items():
-            if task.serviceName == serviceName:
-                toCancel.add(taskId)
-
-        return await self._cancelHelper(toCancel, reason)
-
-    async def cancelRequestedTasksOfDispatcher(self, dispatcher: str, reason):
-        """ Helper to cancel all Tasks which have been requested by a Dispatcher.
-        """
-        # Set containing all Tasks, that has to be canceled
-        toCancel = set()
-
-        for taskId, requestedBy in self._runningExternalRequestedTasks.items():
-            if requestedBy == dispatcher:
-                toCancel.add(taskId)
-
-        return await self._cancelHelper(toCancel, reason)
-
-    async def cancelRunningTasksOfDispatcher(self, dispatcher: str, reason):
-        """ Cancels all Tasks of the given Dispatcher
-        """
-        toCancel = set()
-        for taskId, target in self._runningExternalRequestedTasks.items():
-            if target == dispatcher:
-                toCancel.add(taskId)
-
-        return await self._cancelHelper(toCancel, reason)
-
-    def serviceExists(self, serviceName: str):
-        """ Function to test if a specific Service exists.
-        """
-        return serviceName in self.services.amountOf and self.services.amountOf[
-            serviceName] > 0
-
-    def _getServiceName(self, _id: str, _type: str):
-        if _type in ("request", "response"):
-            return _id if _id.startswith(f"{_type}/") else f"{_type}/{_id}"
-        raise Exception(
-            "For the parameter 'type' the values: 'request' and 'response' are allowed!")
-
-    async def unregisterService(self, func):
-        idOfFunc: str = ""
-        if isinstance(func, str):
-            if self.options.forceUsingValidVarNames:
-                idOfFunc = varifyPath(func)
-            else:
-                idOfFunc = func
-        else:
-            idOfFunc = func.id
-
-        promise = self._sendAvailableServices()
-
-        if self._logger:
-            self._logger.debug(
-                f'Dispatcher "{self._id}" unregistered: "{idOfFunc}"')
-
-        ret = self._registeredServices.pop(idOfFunc, False)
-
-        await promise
-
-        return ret != False
-
-    def _adaptServiceId(self, serviceName: str):
-        if serviceName.startswith(f'nope{SPLITCHAR}service{SPLITCHAR}'):
-            return serviceName
-        return f'nope{SPLITCHAR}service{SPLITCHAR}{serviceName}'
-
-    async def registerService(self, func, options):
-        options = ensureDottedAccess(options)
-
-        # Define / Use the ID of the Function.
-        idOfFunc: str = options.id
-
-        if idOfFunc is None:
-            idOfFunc = generateId()
-
-        if self.options.addNopeServiceIdPrefix:
-            idOfFunc = self._adaptServiceId(idOfFunc)
-        if self.options.forceUsingValidVarNames:
-            idOfFunc = varifyPath(idOfFunc)
-
-        options.id = idOfFunc
-
-        if not self.__warned and not isAsyncFunction(func):
-            if self._logger:
-                self._logger.warn(
-                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                self._logger.warn(
-                    f'The service "{idOfFunc}" is synchronous!')
-            else:
-                print(
-                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                print(f'The service "{idOfFunc}" is synchronous!')
-            # We only want to warn the user once.
-            self.__warned = True
-
-        # Unregister the Function:
-        def unregister():
-            self.unregisterService(idOfFunc)
-
-        # Create a Wrapper
-        wrapped = WrappedFunction(func, idOfFunc, unregister)
-
-        self._registeredServices[idOfFunc] = ensureDottedAccess({
-            "options": options,
-            "func": wrapped
-        })
-
-        await self._sendAvailableServices()
-
-        if self._logger:
-            self._logger.debug(
-                f'Dispatcher "{self._id}" registered: "{idOfFunc}"')
-
-        return wrapped
-
-    async def _performCall(self, serviceName, params, options=None):
-        optionsToUse = ensureDottedAccess({
-            "resultSink": self._getServiceName(serviceName, "response"),
-            "waitForResult": True
-        })
-        optionsToUse.update(ensureDottedAccess(options))
-
-        taskId = generateId()
-
-        # Create a Future of the Loop.
-        future = EXECUTOR.generatePromise(taskId=taskId)
-
-        def clear():
-            if taskId in self._runningInternalRequestedTasks:
-                task = self._runningInternalRequestedTasks[taskId]
-
-                if task.timeout is not None:
-                    task.timeout.cancel()
-
-                self._runningInternalRequestedTasks.pop(taskId)
-
-            if self._logger:
-                self._logger.debug('Clearing Callbacks from ' + str(taskId))
-
-        try:
-            tastRequest = ensureDottedAccess({
-                "future": future,
-                "clear": clear,
-                'serviceName': serviceName,
-                'timeout': None,
-            })
-
-            # Store the Future as Task.
-            self._runningInternalRequestedTasks[taskId] = tastRequest
-
-            # Define the packet to send:
-            packet = {
-                'functionId': serviceName,
-                'params': [],
-                'taskId': taskId,
-                'resultSink': optionsToUse['resultSink'],
-                'requestedBy': self._id,
-                'target': None
-            }
-
-            # Iterate over all Parameters and
-            # Determin Callbacks. Based on the Parameter-
-            # Type assign it either to packet.params (
-            # for parsable Parameters) and packet.callbacks
-            # (for callback Parameters)
-            for idx, param in enumerate(params):
-                packet['params'].append({
-                    'idx': idx,
-                    'data': param
-                })
-
-            if not self.serviceExists(serviceName):
-                error = Exception(
-                    f'No Service Provider known for "{serviceName}"')
-                if self._logger:
-                    self._logger.error(
-                        f'No Service Provider known for "{serviceName}"')
-                    self._logger.error(formatException(error))
-
-                raise error
-
-            if self.options.forceUsingSelectors or self.services.amountOf.get(
-                    serviceName, 0) > 1:
-
-                optionsForSelector = ensureDottedAccess({
-                    "rpcManager": self,
-                    "serviceName": serviceName
-                })
-
-                if isinstance(optionsToUse.target, str):
-                    tastRequest.target = optionsToUse.target
-                elif callable(optionsToUse.selector):
-                    tastRequest.target = await options.selector(optionsForSelector)
-                elif isinstance(optionsToUse.selector, str):
-                    tastRequest.target = await self._defaultSelector(optionsForSelector)
-
-            else:
-                tastRequest.target = list(
-                    self.services.keyMappingreverse[serviceName])[0]
-
-            packet["target"] = tastRequest.target
-
-            await self._communicator.emit("rpcRequest", packet)
-
-            if self._logger:
-                self._logger.debug(
-                    f'Dispatcher "{self._id}" putting task "{taskId}" on: "{self._getServiceName(tastRequest.serviceName, "request")}"')
-
-            if optionsToUse.get("timeout", 0) > 0:
-                async def onTimeout():
-                    await self.cancelTask(
-                        taskId,
-                        TimeoutError(
-                            f"TIMEOUT. The Service allowed execution time of {optionsToUse.timeout} [ms] has been excided")
-                    )
-
-                # Create our timeout and store it.
-                tastRequest.timeout = EXECUTOR.setTimeout(
-                    onTimeout, optionsToUse.timeout)
-
-        except Exception as err:
-            if self._logger:
-                self._logger.error('Something went wrong on calling')
-                self._logger.exception(formatException(err))
-            else:
-                print(formatException(err))
-
-            # Call the Clear Function
-            clear()
-
-            # Throw an error.
-            future.set_exception(err)
-
-        # Define a Function, which could be used for cancelation.
-        def _cancelTask(reason):
-            EXECUTOR.callParallel(self.cancelTask, taskId, reason)
-
-        future.cancelCallback = _cancelTask
-
-        if not optionsToUse.waitForResult:
-            EXECUTOR.loop.create_task(future)
-            return future
-
-        return await future
-
-    async def performCall(self, serviceName, params, options=None):
-        if isList(serviceName):
-            if isList(options) and len(serviceName) != len(options):
-                raise Exception(
-                    "The length of the provided services and options does not match")
-
-            optionsToUse = [options] * \
-                len(serviceName) if not isIterable(options) else options
-
-            futures = []
-
-            for idx, srv in enumerate(serviceName):
-                futures.append(
-                    self._performCall(
-                        srv,
-                        params,
-                        optionsToUse[idx]
-                    )
-                )
-
-            return await asyncio.gather(*futures)
-
-        else:
-            if isList(options):
-                raise Exception(
-                    "The length of the provided services and options does not match")
-
-            return await self._performCall(serviceName, params, options)
-
-    def clearTasks(self):
-        self._runningInternalRequestedTasks.clear()
-
-    def unregisterAll(self, log=False):
-        toUnregister = list(self._registeredServices.keys())
-        for srv in toUnregister:
-            EXECUTOR.callParallel(self.unregisterService, srv)
-            # Log the removing of the service.
-            if log and self._logger:
-                self._logger.warn('removing service "' + srv + '"')
-        self._registeredServices.clear()
-
-    def reset(self):
-        self.clearTasks()
-        self.unregisterAll()
-        EXECUTOR.callParallel(self._sendAvailableServices)
-
-    async def dispose(self):
-        self.clearTasks()
-        self.ready.dispose()
-        self.unregisterAll(log=True)
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+import asyncio
+
+from nope.communication.bridge import Bridge
+from nope.dispatcher.connectivityManager import NopeConnectivityManager
+from nope.eventEmitter import NopeEventEmitter
+from nope.helpers import generateId, ensureDottedAccess, isAsyncFunction, \
+    formatException, DottedDict, SPLITCHAR, isIterable, isList, EXECUTOR
+from nope.logger import defineNopeLogger
+from nope.merging import DictBasedMergeData
+from nope.observable import NopeObservable
+
+_DEFAULT_RESULT = object()
+
+
+class WrappedFunction:
+
+    def __init__(self, func, _id, unregister):
+        self._func = func
+        self._unregister = unregister
+        self.id = _id
+        self.isAsync = isAsyncFunction(func)
+
+    def __call__(self, *args, **kwarg):
+        return EXECUTOR.callParallel(self._func, *args, **kwarg)
+
+
+class NopeRpcManager:
+
+    def __init__(self, options, defaultSelector, id=None,
+                 connectivityManager=None):
+
+        options = ensureDottedAccess(options)
+
+        self.options = options
+        self._defaultSelector = defaultSelector
+        self._id = id
+        self._communicator: Bridge = options.communicator
+        self._connectivityManager: NopeConnectivityManager = connectivityManager
+
+        self._runningInternalRequestedTasks = dict()
+        self._registeredServices = dict()
+
+        if self._id is None:
+            self._id = generateId()
+
+        if self._connectivityManager is None:
+            self._connectivityManager = NopeConnectivityManager(
+                options, self.id)
+
+        self._logger = defineNopeLogger(options.logger, 'core.rpc-manager')
+        self.ready = NopeObservable()
+        self.ready.setContent(False)
+
+        self.__warned = False
+
+        self._mappingOfDispatchersAndServices = dict()
+        self.services = DictBasedMergeData(
+            self._mappingOfDispatchersAndServices, 'services/+', 'services/+/id')
+        self.onCancelTask = NopeEventEmitter()
+
+        if self._logger:
+            self._logger.info(f'manager created id={self.id}')
+
+        self._runningExternalRequestedTasks = dict()
+
+        self.reset()
+        EXECUTOR.callParallel(self._init)
+
+    @property
+    def id(self):
+        return self._id
+
+    def updateDispatcher(self, msg):
+        self._mappingOfDispatchersAndServices[msg.dispatcher] = msg
+        self.services.update()
+
+    async def _handleExternalRequest(self, data, func: WrappedFunction | None = None):
+        try:
+            if not callable(func):
+                if data.functionId not in self._registeredServices:
+                    return
+                func = self._registeredServices[data.functionId].get(
+                    "func", None)
+
+            if self._logger:
+                self._logger.debug(
+                    f'Dispatcher "{self.id}" received request: "{data.functionId}" -> task: "{data.taskId}"')
+
+            if callable(func):
+                # Now we check, if we have to perform test, whether
+                # we are allowed to execute the task:
+                if data.get("target", self.id) != self.id:
+                    return
+
+                # Define a list containing callbacks:
+                cbs = []
+
+                observer = None
+
+                def on_cancel(reason, *args):
+                    nonlocal observer
+                    if reason.taskId == data.taskId:
+
+                        for cb in cbs:
+                            cb(reason)
+
+                        observer.unsubscribe()
+                        observer = None
+
+                observer = self.onCancelTask.subscribe(on_cancel)
+
+                # extract the arguments etc.
+                # create an empty list and fill it afterwards
+                args = [None] * len(data.params)
+                for item in data.params:
+                    args[item.idx] = item.data
+
+                _result = _DEFAULT_RESULT
+
+                if not func.isAsync and not self.__warned:
+                    if self._logger:
+                        self._logger.warn(
+                            "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                        self._logger.warn(
+                            "Offloading function to a separate thread.")
+                    else:
+                        print(
+                            "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                        print("Offloading function to a separate thread.")
+                    # We only want to warn the user once.
+                    self.__warned = True
+
+                resultPromise = func(*args)
+
+                try:
+                    if resultPromise is not None and getattr(
+                            resultPromise, 'cancelCallback', False):
+                        def _cancel_main(reason):
+                            resultPromise.cancelCallback(reason)
+
+                        cbs.append(_cancel_main)
+
+                except Exception as error:
+                    # The Cancel Function isn't available in
+                    # the provided promise.
+                    pass
+
+                self._runningExternalRequestedTasks[data.taskId] = data.requestedBy
+
+                # Wait for the Result to finish.
+                _result = await resultPromise
+
+                # Define the Result message
+                result = {
+                    'result': _result if _result is not _DEFAULT_RESULT else None,
+                    'taskId': data.taskId,
+                    'type': 'response'
+                }
+
+                if self._logger:
+                    self._logger.debug(
+                        'Internally executed requested Function for Task: ' + str(data['taskId']) + " - Function \"" +
+                        data['functionId'] + '\". Sending result on ' + str(data['resultSink']))
+
+                # Use the communicator to publish the result.
+                await self._communicator.emit("rpcResponse", result)
+
+        except Exception as error:
+
+            if self._logger:
+                self._logger.error(
+                    f'Dispatcher "{self.id}" failed with request: "{data.taskId}"')
+                self._logger.error(formatException(error))
+            else:
+                print(formatException(error))
+
+            self._runningExternalRequestedTasks.pop(data.requestedBy, None)
+
+            result = {
+                'error': {
+                    'error': str(error),
+                    'msg': str(error)
+                },
+                'taskId': data.taskId,
+                'type': 'response'
+            }
+
+            # Use the communicator to publish the result.
+            await self._communicator.emit("rpcResponse", result)
+
+    async def _handle_external_response(self, data):
+        try:
+            # Extract the Task
+            task: DottedDict = self._runningInternalRequestedTasks.get(
+                data.taskId, None)
+
+            if task:
+
+                # Based on the Result of the Remote => proceed.
+                # Either throw an error or forward the result
+                self._runningInternalRequestedTasks.pop(data.taskId)
+
+                if data.error:
+                    if self._logger:
+                        self._logger.error(
+                            "Failed with task " + str(data['taskId']))
+                        self._logger.error(
+                            "Reason: " + str(data['error']['msg']))
+                        self._logger.exception(data['error'])
+
+                    # Reject the Error:
+                    task.future.set_exception(Exception(data['error']))
+
+                    if "timeout" in task and task.timeout is not None:
+                        # Assume, that the timeout has been
+                        # defined with setTimeout
+                        task.timeout.cancel()
+
+                    return True
+
+                else:
+                    if self._logger:
+                        self._logger.debug('Got sucessfull result for Task: "' + str(
+                            data['taskId']) + '". Forwarding Result to Future.')
+
+                    task.future.set_result(data.result)
+
+                    if self._logger:
+                        self._logger.debug("Forwarded result to future")
+
+                    if "timeout" in task and task.timeout is not None:
+                        task.timeout.cancel()
+
+                    return True
+
+        except Exception as error:
+            if self._logger:
+                self._logger.error(
+                    "Error during handling an external response")
+                self._logger.error(formatException(error))
+            else:
+                print(formatException(error))
+
+        return False
+
+    async def _sendAvailableServices(self):
+        """ Function used to update the Available Services.
+        """
+
+        message = ensureDottedAccess({
+            "dispatcher": self.id,
+            "services": list(map(lambda item: item.options, self._registeredServices.values()))
+        })
+
+        if self._logger:
+            self._logger.debug("sending available services")
+
+        await self._communicator.emit("servicesChanged", message)
+
+    async def _init(self):
+        self.ready.setContent(False)
+
+        await self._communicator.connected.waitFor()
+        await self._connectivityManager.ready.waitFor()
+
+        def onServicesChanged(msg):
+            try:
+                self.updateDispatcher(msg)
+            except Exception as error:
+                if self._logger:
+                    self._logger.error("Failed to add the new services")
+                    self._logger.error(formatException(error))
+                else:
+                    print(formatException(error))
+
+        await self._communicator.on("servicesChanged", onServicesChanged)
+        await self._communicator.on("rpcRequest", lambda data: EXECUTOR.callParallel(self._handleExternalRequest, data))
+        await self._communicator.on("rpcResponse",
+                                    lambda data: EXECUTOR.callParallel(self._handle_external_response, data))
+
+        def on_cancelation(msg):
+            if msg.dispatcher == self._id:
+                self.onCancelTask.emit(msg)
+
+        await self._communicator.on("taskCancelation", on_cancelation)
+
+        def on_unregister(msg):
+            if msg.identifier in self._registeredServices:
+                self.unregisterService(msg.identifier)
+
+        await self._communicator.on("rpcUnregister", on_unregister)
+
+        # We are now listening on these changes!
+        await self._communicator.on("bonjour", lambda *args: EXECUTOR.callParallel(self._sendAvailableServices))
+
+        def onDispatchersChanged(changes, *args):
+            if len(changes.added):
+                # If there are dispatchers online,
+                # We will emit our available services.
+                EXECUTOR.callParallel(self._sendAvailableServices)
+            if len(changes.removed):
+                for rm in changes.removed:
+                    self.removeDispatcher(rm)
+
+        self._connectivityManager.dispatchers.onChange.subscribe(
+            onDispatchersChanged)
+
+        if self._logger:
+            self._logger.info(f"core.rpc-manager {self._id} initialized!")
+
+        self.ready.setContent(True)
+
+    def removeDispatcher(self, dispatcherId: str):
+        res = self._mappingOfDispatchersAndServices.pop(dispatcherId, False)
+        if (res):
+            self.services.update()
+
+            # Now we need to cancel every Task of the dispatcher,
+            # which isnt present any more.
+            EXECUTOR.callParallel(self.cancelRunningTasksOfDispatcher, dispatcherId, Exception(
+                "Dispatcher has been removed! Tasks cannot be executed any more."))
+            # Stop executing the requested Tasks.
+            EXECUTOR.callParallel(self.cancelRequestedTasksOfDispatcher, dispatcherId, Exception(
+                "Dispatcher has been removed! Tasks are not required any more."))
+
+    async def cancelTask(self, taskId: str, reason, quiet=False):
+        if taskId in self._runningInternalRequestedTasks:
+            task = self._runningInternalRequestedTasks[taskId]
+
+            # Delete the task
+            self._runningInternalRequestedTasks.pop(taskId)
+
+            # Propagate the Cancellation (internally):
+            task.future.set_exception(reason)
+
+            # Propagate the Cancellation externally.
+            # Therefore use the desired Mode.
+            await self._communicator.emit("taskCancelation", ensureDottedAccess({
+                "dispatcher": self._id,
+                "reason": str(reason),
+                "taskId": taskId,
+                "quiet": quiet
+            }))
+
+            return True
+        # Task hasnt been found => Cancel the Task.
+        return False
+
+    async def _cancelHelper(self, tasksToCancel: set, reason):
+        """ Helper Function, used to close all tasks with a specific service.
+        """
+        if len(tasksToCancel) > 0:
+            for taskId in tasksToCancel:
+                await self.cancelTask(taskId, reason)
+
+    async def cancelRunningTasksOfService(self, serviceName: str, reason):
+        """ Helper Function, used to close all tasks with a specific service.
+        """
+        # Set containing all Tasks, that has to be canceled
+        toCancel = set()
+
+        # Filter all Tasks that should be canceled.
+        for taskId, task in self._runningInternalRequestedTasks.items():
+            if task.serviceName == serviceName:
+                toCancel.add(taskId)
+
+        return await self._cancelHelper(toCancel, reason)
+
+    async def cancelRequestedTasksOfDispatcher(self, dispatcher: str, reason):
+        """ Helper to cancel all Tasks which have been requested by a Dispatcher.
+        """
+        # Set containing all Tasks, that has to be canceled
+        toCancel = set()
+
+        for taskId, requestedBy in self._runningExternalRequestedTasks.items():
+            if requestedBy == dispatcher:
+                toCancel.add(taskId)
+
+        return await self._cancelHelper(toCancel, reason)
+
+    async def cancelRunningTasksOfDispatcher(self, dispatcher: str, reason):
+        """ Cancels all Tasks of the given Dispatcher
+        """
+        toCancel = set()
+        for taskId, target in self._runningExternalRequestedTasks.items():
+            if target == dispatcher:
+                toCancel.add(taskId)
+
+        return await self._cancelHelper(toCancel, reason)
+
+    def serviceExists(self, serviceName: str):
+        """ Function to test if a specific Service exists.
+        """
+        return serviceName in self.services.amountOf and self.services.amountOf[
+            serviceName] > 0
+
+    def _getServiceName(self, _id: str, _type: str):
+        if _type in ("request", "response"):
+            return _id if _id.startswith(f"{_type}/") else f"{_type}/{_id}"
+        raise Exception(
+            "For the parameter 'type' the values: 'request' and 'response' are allowed!")
+
+    async def unregisterService(self, func):
+        idOfFunc: str = ""
+        if isinstance(func, str):
+            if self.options.forceUsingValidVarNames:
+                idOfFunc = varifyPath(func)
+            else:
+                idOfFunc = func
+        else:
+            idOfFunc = func.id
+
+        promise = self._sendAvailableServices()
+
+        if self._logger:
+            self._logger.debug(
+                f'Dispatcher "{self._id}" unregistered: "{idOfFunc}"')
+
+        ret = self._registeredServices.pop(idOfFunc, False)
+
+        await promise
+
+        return ret != False
+
+    def _adaptServiceId(self, serviceName: str):
+        if serviceName.startswith(f'nope{SPLITCHAR}service{SPLITCHAR}'):
+            return serviceName
+        return f'nope{SPLITCHAR}service{SPLITCHAR}{serviceName}'
+
+    async def registerService(self, func, options):
+        options = ensureDottedAccess(options)
+
+        # Define / Use the ID of the Function.
+        idOfFunc: str = options.id
+
+        if idOfFunc is None:
+            idOfFunc = generateId()
+
+        if self.options.addNopeServiceIdPrefix:
+            idOfFunc = self._adaptServiceId(idOfFunc)
+        if self.options.forceUsingValidVarNames:
+            idOfFunc = varifyPath(idOfFunc)
+
+        options.id = idOfFunc
+
+        if not self.__warned and not isAsyncFunction(func):
+            if self._logger:
+                self._logger.warn(
+                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                self._logger.warn(
+                    f'The service "{idOfFunc}" is synchronous!')
+            else:
+                print(
+                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                print(f'The service "{idOfFunc}" is synchronous!')
+            # We only want to warn the user once.
+            self.__warned = True
+
+        # Unregister the Function:
+        def unregister():
+            self.unregisterService(idOfFunc)
+
+        # Create a Wrapper
+        wrapped = WrappedFunction(func, idOfFunc, unregister)
+
+        self._registeredServices[idOfFunc] = ensureDottedAccess({
+            "options": options,
+            "func": wrapped
+        })
+
+        await self._sendAvailableServices()
+
+        if self._logger:
+            self._logger.debug(
+                f'Dispatcher "{self._id}" registered: "{idOfFunc}"')
+
+        return wrapped
+
+    async def _performCall(self, serviceName, params, options=None):
+        optionsToUse = ensureDottedAccess({
+            "resultSink": self._getServiceName(serviceName, "response"),
+            "waitForResult": True
+        })
+        optionsToUse.update(ensureDottedAccess(options))
+
+        taskId = generateId()
+
+        # Create a Future of the Loop.
+        future = EXECUTOR.generatePromise(taskId=taskId)
+
+        def clear():
+            if taskId in self._runningInternalRequestedTasks:
+                task = self._runningInternalRequestedTasks[taskId]
+
+                if task.timeout is not None:
+                    task.timeout.cancel()
+
+                self._runningInternalRequestedTasks.pop(taskId)
+
+            if self._logger:
+                self._logger.debug('Clearing Callbacks from ' + str(taskId))
+
+        try:
+            tastRequest = ensureDottedAccess({
+                "future": future,
+                "clear": clear,
+                'serviceName': serviceName,
+                'timeout': None,
+            })
+
+            # Store the Future as Task.
+            self._runningInternalRequestedTasks[taskId] = tastRequest
+
+            # Define the packet to send:
+            packet = {
+                'functionId': serviceName,
+                'params': [],
+                'taskId': taskId,
+                'resultSink': optionsToUse['resultSink'],
+                'requestedBy': self._id,
+                'target': None
+            }
+
+            # Iterate over all Parameters and
+            # Determin Callbacks. Based on the Parameter-
+            # Type assign it either to packet.params (
+            # for parsable Parameters) and packet.callbacks
+            # (for callback Parameters)
+            for idx, param in enumerate(params):
+                packet['params'].append({
+                    'idx': idx,
+                    'data': param
+                })
+
+            if not self.serviceExists(serviceName):
+                error = Exception(
+                    f'No Service Provider known for "{serviceName}"')
+                if self._logger:
+                    self._logger.error(
+                        f'No Service Provider known for "{serviceName}"')
+                    self._logger.error(formatException(error))
+
+                raise error
+
+            if self.options.forceUsingSelectors or self.services.amountOf.get(
+                    serviceName, 0) > 1:
+
+                optionsForSelector = ensureDottedAccess({
+                    "rpcManager": self,
+                    "serviceName": serviceName
+                })
+
+                if isinstance(optionsToUse.target, str):
+                    tastRequest.target = optionsToUse.target
+                elif callable(optionsToUse.selector):
+                    tastRequest.target = await options.selector(optionsForSelector)
+                elif isinstance(optionsToUse.selector, str):
+                    tastRequest.target = await self._defaultSelector(optionsForSelector)
+
+            else:
+                tastRequest.target = list(
+                    self.services.keyMappingreverse[serviceName])[0]
+
+            packet["target"] = tastRequest.target
+
+            await self._communicator.emit("rpcRequest", packet)
+
+            if self._logger:
+                self._logger.debug(
+                    f'Dispatcher "{self._id}" putting task "{taskId}" on: "{self._getServiceName(tastRequest.serviceName, "request")}"')
+
+            if optionsToUse.get("timeout", 0) > 0:
+                async def onTimeout():
+                    await self.cancelTask(
+                        taskId,
+                        TimeoutError(
+                            f"TIMEOUT. The Service allowed execution time of {optionsToUse.timeout} [ms] has been excided")
+                    )
+
+                # Create our timeout and store it.
+                tastRequest.timeout = EXECUTOR.setTimeout(
+                    onTimeout, optionsToUse.timeout)
+
+        except Exception as err:
+            if self._logger:
+                self._logger.error('Something went wrong on calling')
+                self._logger.exception(formatException(err))
+            else:
+                print(formatException(err))
+
+            # Call the Clear Function
+            clear()
+
+            # Throw an error.
+            future.set_exception(err)
+
+        # Define a Function, which could be used for cancelation.
+        def _cancelTask(reason):
+            EXECUTOR.callParallel(self.cancelTask, taskId, reason)
+
+        future.cancelCallback = _cancelTask
+
+        if not optionsToUse.waitForResult:
+            EXECUTOR.loop.create_task(future)
+            return future
+
+        return await future
+
+    async def performCall(self, serviceName, params, options=None):
+        if isList(serviceName):
+            if isList(options) and len(serviceName) != len(options):
+                raise Exception(
+                    "The length of the provided services and options does not match")
+
+            optionsToUse = [options] * \
+                len(serviceName) if not isIterable(options) else options
+
+            futures = []
+
+            for idx, srv in enumerate(serviceName):
+                futures.append(
+                    self._performCall(
+                        srv,
+                        params,
+                        optionsToUse[idx]
+                    )
+                )
+
+            return await asyncio.gather(*futures)
+
+        else:
+            if isList(options):
+                raise Exception(
+                    "The length of the provided services and options does not match")
+
+            return await self._performCall(serviceName, params, options)
+
+    def clearTasks(self):
+        self._runningInternalRequestedTasks.clear()
+
+    def unregisterAll(self, log=False):
+        toUnregister = list(self._registeredServices.keys())
+        for srv in toUnregister:
+            EXECUTOR.callParallel(self.unregisterService, srv)
+            # Log the removing of the service.
+            if log and self._logger:
+                self._logger.warn('removing service "' + srv + '"')
+        self._registeredServices.clear()
+
+    def reset(self):
+        self.clearTasks()
+        self.unregisterAll()
+        EXECUTOR.callParallel(self._sendAvailableServices)
+
+    async def dispose(self):
+        self.clearTasks()
+        self.ready.dispose()
+        self.unregisterAll(log=True)
```

### Comparing `nope_py-1.7.8rc3/nope/dispatcher/rpcManager/selectors.py` & `nope_py-1.7.9/nope/dispatcher/rpcManager/selectors.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from nope.helpers import maxOfArray, minOfArray
-
-
-ValidDefaultSelectors = [
-    "master",
-    "first",
-    "dispatcher",
-    "host",
-    "free-ram",
-    "cpu-usage",
-]
-
-
-def generateSelector(selector, core):
-    """ A Helper Function, to generate the Basic selector Functions.
-
-    params:
-        selector (master|first|dispatcher|host|cpu-usage)
-
-    """
-
-    if selector == 'master':
-
-        # Define a function, which will select the same master.
-        async def masterSelector(opts):
-            masterId = core.connectivityManager.master.id
-            data = core.rpcManager.services.keyMappingreverse
-            if opts.serviceName in data:
-                arr = list(data[opts.serviceName])
-                if masterId in arr:
-                    return masterId
-            raise Exception('No matching dispatcher present.')
-
-        return masterSelector
-
-    elif selector == 'first':
-
-        async def firstFound(opts):
-            data = core.rpcManager.services.keyMappingreverse
-            if opts.serviceName in data:
-                arr = list(data[opts.serviceName])
-                if len(arr) > 0:
-                    return arr[0]
-            raise Exception('No matching dispatcher present.')
-
-        return firstFound
-
-    elif selector == 'dispatcher':
-
-        async def ownDispatcher(opts):
-            ids = core.connectivityManager.dispatchers.data.getContent()
-            if core.id in ids:
-                return core.id
-            raise Exception('No matching dispatcher present.')
-
-        return ownDispatcher
-
-    elif selector == 'host':
-
-        host = core.connectivityManager.info.host.name
-
-        async def sameHost(opts):
-            data = core.rpcManager.services.keyMappingreverse
-            if opts.serviceName in data:
-                items = list(data[opts.serviceName])
-                hosts = list(
-                    map(
-                        lambda item: core.connectivityManager.dispatchers.originalData[
-                            item].host.name,
-                        items
-                    )
-                )
-
-                if host in hosts:
-                    return items[hosts.index(host)]
-
-            raise Exception('No matching dispatcher present.')
-
-        return sameHost
-
-    elif selector == 'cpu-usage':
-
-        async def cpuUsage():
-            dispatchers = core.connectivityManager.dispatchers.data.getContent()
-            best_option = minOfArray(dispatchers, 'host.cpu.usage')
-            if best_option.index >= 0:
-                return dispatchers[best_option.index]
-            raise Exception('No matching dispatcher present.')
-
-        return cpuUsage
-
-    elif selector == 'free-ram':
-
-        async def ramUsage():
-            dispatchers = core.connectivityManager.dispatchers.data.getContent()
-            best_option = maxOfArray(dispatchers, 'host.ram.free')
-            if best_option.index >= 0:
-                return dispatchers[best_option.index]
-
-            raise Exception('No matching dispatcher present.')
-
-        return ramUsage
-
-    else:
-        raise Exception('Please use a valid selector')
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from nope.helpers import maxOfArray, minOfArray
+
+
+ValidDefaultSelectors = [
+    "master",
+    "first",
+    "dispatcher",
+    "host",
+    "free-ram",
+    "cpu-usage",
+]
+
+
+def generateSelector(selector, core):
+    """ A Helper Function, to generate the Basic selector Functions.
+
+    params:
+        selector (master|first|dispatcher|host|cpu-usage)
+
+    """
+
+    if selector == 'master':
+
+        # Define a function, which will select the same master.
+        async def masterSelector(opts):
+            masterId = core.connectivityManager.master.id
+            data = core.rpcManager.services.keyMappingreverse
+            if opts.serviceName in data:
+                arr = list(data[opts.serviceName])
+                if masterId in arr:
+                    return masterId
+            raise Exception('No matching dispatcher present.')
+
+        return masterSelector
+
+    elif selector == 'first':
+
+        async def firstFound(opts):
+            data = core.rpcManager.services.keyMappingreverse
+            if opts.serviceName in data:
+                arr = list(data[opts.serviceName])
+                if len(arr) > 0:
+                    return arr[0]
+            raise Exception('No matching dispatcher present.')
+
+        return firstFound
+
+    elif selector == 'dispatcher':
+
+        async def ownDispatcher(opts):
+            ids = core.connectivityManager.dispatchers.data.getContent()
+            if core.id in ids:
+                return core.id
+            raise Exception('No matching dispatcher present.')
+
+        return ownDispatcher
+
+    elif selector == 'host':
+
+        host = core.connectivityManager.info.host.name
+
+        async def sameHost(opts):
+            data = core.rpcManager.services.keyMappingreverse
+            if opts.serviceName in data:
+                items = list(data[opts.serviceName])
+                hosts = list(
+                    map(
+                        lambda item: core.connectivityManager.dispatchers.originalData[
+                            item].host.name,
+                        items
+                    )
+                )
+
+                if host in hosts:
+                    return items[hosts.index(host)]
+
+            raise Exception('No matching dispatcher present.')
+
+        return sameHost
+
+    elif selector == 'cpu-usage':
+
+        async def cpuUsage():
+            dispatchers = core.connectivityManager.dispatchers.data.getContent()
+            best_option = minOfArray(dispatchers, 'host.cpu.usage')
+            if best_option.index >= 0:
+                return dispatchers[best_option.index]
+            raise Exception('No matching dispatcher present.')
+
+        return cpuUsage
+
+    elif selector == 'free-ram':
+
+        async def ramUsage():
+            dispatchers = core.connectivityManager.dispatchers.data.getContent()
+            best_option = maxOfArray(dispatchers, 'host.ram.free')
+            if best_option.index >= 0:
+                return dispatchers[best_option.index]
+
+            raise Exception('No matching dispatcher present.')
+
+        return ramUsage
+
+    else:
+        raise Exception('Please use a valid selector')
```

### Comparing `nope_py-1.7.8rc3/nope/eventEmitter/nopeEventEmitter.py` & `nope_py-1.7.9/nope/eventEmitter/nopeEventEmitter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from asyncio import Future
-
-from ..helpers import generateId, DottedDict, Emitter, ensureDottedAccess, isAsyncFunction, getTimestamp, Promise, \
-    EXECUTOR
-
-
-# from ..logger.getLogger import getNopeLogger
-# logger = getNopeLogger('obervable')
-
-
-class NopeEventEmitter:
-
-    def __init__(self, options=None):
-        self.id = generateId()
-        self.options = ensureDottedAccess({'generateTimestamp': True})
-        self.options.update(ensureDottedAccess(options))
-        self.setter = None
-        self.getter = None
-        self._subscriptions = set()
-        self.disablePublishing = False
-        self._emitter = Emitter()
-
-    def emit(self, value, options=None):
-        return self._emit(value, ensureDottedAccess(options))
-
-    def _emit(self, value, options=None):
-
-        options = ensureDottedAccess(options)
-
-        _value = value
-        if self.setter is not None:
-            adapted = ensureDottedAccess(self.setter(value, options))
-            if not adapted.valid:
-                return False
-            _value = adapted.data
-        # Assign the Value (either use it directly or use the getter)
-        _value = self.getter(_value) if self.getter is not None else _value
-        if options.forced or (self.disablePublishing == False):
-            options = self._updateSenderAndTimestamp(options)
-            self._emitter.emit(data=ensureDottedAccess(
-                {'value': _value, **options}))
-            return self.hasSubscriptions
-        return False
-
-    def _updateSenderAndTimestamp(self, options: DottedDict):
-        if not options.sender:
-            options.sender = self.id
-        if self.options.generateTimestamp:
-            options.timestamp = options.get("timestamp", getTimestamp())
-        return options
-
-    def dispose(self):
-        for _unsubscribe in self._subscriptions:
-            _unsubscribe()
-        self._subscriptions.clear()
-        self._emitter.close()
-
-    def subscribe(self, callback,
-                  options: dict | DottedDict = DottedDict({'type': 'sync', 'mode': ['direct', 'sub', 'super']})):
-        options = ensureDottedAccess(options)
-        options.skipCurrent = self.options.showCurrent and not self.options.playHistory
-        return self._subscribe(self._adaptCallback(callback, options))
-
-    def _adaptCallback(self, callback, options):
-        first = True
-
-        def adaptedCallback(_data: DottedDict):
-            nonlocal first
-
-            data = _data.copy()
-
-            if first and options.skipCurrent:
-                first = False
-                return
-
-            first = False
-
-            if data is not None:
-                # Pop the value
-                value = data.pop("value")
-                # Now we call value, ... rest
-                callback(value, data)
-
-        return adaptedCallback
-
-    def _subscribe(self, callback):
-
-        return self._emitter.on(callback=callback)
-
-    def once(self, callback, options=None):
-        ret = None
-
-        def adaptedCallback(data, rest):
-            ret.unsubscribe()
-            callback(data, rest)
-
-        ret = self.subscribe(adaptedCallback, options)
-        return ret
-
-    def waitFor(self, testCallback=None, options=None):
-
-        # Convert our Options.
-
-        _options = ensureDottedAccess({
-            'testCurrent': True,
-            "timeout": 0
-        })
-        _options.update(ensureDottedAccess(options))
-
-        if testCallback is None:
-            # Define a Test Callback
-            def test(value, *args):
-                return value == True
-
-            testCallback = test
-
-        subscription = None
-        timeout = None
-
-        def callback(resolve, reject):
-            nonlocal subscription
-            nonlocal timeout
-
-            first = True
-            resolved = False
-
-            def finish(err, sucessfull, data, timedout):
-                nonlocal first
-                nonlocal resolved
-                nonlocal subscription
-                nonlocal timeout
-
-                if err:
-                    reject(err)
-
-                    if subscription:
-                        subscription.unsubscribe()
-                        subscription = None
-
-                    if timeout and not timedout:
-                        timeout.cancel()
-                elif sucessfull:
-                    if subscription:
-                        subscription.unsubscribe()
-                        subscription = None
-                    if not resolved:
-                        resolved = True
-                        resolve(data)
-
-                    if timeout and not timedout:
-                        timeout.cancel()
-
-            def check_data(value, rest):
-                nonlocal first
-                nonlocal resolved
-                nonlocal subscription
-
-                if (first and _options.testCurrent) or not first:
-                    if isAsyncFunction(testCallback):
-                        # Try to offload the Function
-                        prom: Future = Promise.cast(testCallback(value, rest))
-
-                        def done(p: Future):
-                            nonlocal first
-                            first = False
-
-                            if p.done():
-                                finish(False, True, p.result(), False)
-                            if p.exception():
-                                finish(p.exception(), False, False, False)
-
-                        prom.add_done_callback(done)
-                    else:
-                        result = testCallback(value, rest)
-                        finish(False, result, value, False)
-
-                        first = False
-
-            try:
-                if _options.timeout > 0:
-                    timeout = EXECUTOR.setTimeout(
-                        finish, _options.timeout, TimeoutError("Time elapsed"), False, False, True)
-
-                subscription = self.subscribe(check_data)
-            except BaseException:
-                reject(Exception("Failed to subscribe"))
-
-        return Promise(callback)
-
-    def waitForUpdate(self, options=DottedDict({'testCurrent': True})):
-        # Define a Callback
-        def callback(resolve, reject):
-            def cb(value, rest):
-                resolve(value)
-
-            self.once(cb, options)
-
-        return Promise(callback)
-
-    @property
-    def hasSubscriptions(self):
-        return self._emitter.hasSubscriptions()
-
-    @property
-    def observerLength(self):
-        return self._emitter.amountOfSubscriptions()
+from asyncio import Future
+
+from ..helpers import generateId, DottedDict, Emitter, ensureDottedAccess, isAsyncFunction, getTimestamp, Promise, \
+    EXECUTOR
+
+
+# from ..logger.getLogger import getNopeLogger
+# logger = getNopeLogger('obervable')
+
+
+class NopeEventEmitter:
+
+    def __init__(self, options=None):
+        self.id = generateId()
+        self.options = ensureDottedAccess({'generateTimestamp': True})
+        self.options.update(ensureDottedAccess(options))
+        self.setter = None
+        self.getter = None
+        self._subscriptions = set()
+        self.disablePublishing = False
+        self._emitter = Emitter()
+
+    def emit(self, value, options=None):
+        return self._emit(value, ensureDottedAccess(options))
+
+    def _emit(self, value, options=None):
+
+        options = ensureDottedAccess(options)
+
+        _value = value
+        if self.setter is not None:
+            adapted = ensureDottedAccess(self.setter(value, options))
+            if not adapted.valid:
+                return False
+            _value = adapted.data
+        # Assign the Value (either use it directly or use the getter)
+        _value = self.getter(_value) if self.getter is not None else _value
+        if options.forced or (self.disablePublishing == False):
+            options = self._updateSenderAndTimestamp(options)
+            self._emitter.emit(data=ensureDottedAccess(
+                {'value': _value, **options}))
+            return self.hasSubscriptions
+        return False
+
+    def _updateSenderAndTimestamp(self, options: DottedDict):
+        if not options.sender:
+            options.sender = self.id
+        if self.options.generateTimestamp:
+            options.timestamp = options.get("timestamp", getTimestamp())
+        return options
+
+    def dispose(self):
+        for _unsubscribe in self._subscriptions:
+            _unsubscribe()
+        self._subscriptions.clear()
+        self._emitter.close()
+
+    def subscribe(self, callback,
+                  options: dict | DottedDict = DottedDict({'type': 'sync', 'mode': ['direct', 'sub', 'super']})):
+        options = ensureDottedAccess(options)
+        options.skipCurrent = self.options.showCurrent and not self.options.playHistory
+        return self._subscribe(self._adaptCallback(callback, options))
+
+    def _adaptCallback(self, callback, options):
+        first = True
+
+        def adaptedCallback(_data: DottedDict):
+            nonlocal first
+
+            data = _data.copy()
+
+            if first and options.skipCurrent:
+                first = False
+                return
+
+            first = False
+
+            if data is not None:
+                # Pop the value
+                value = data.pop("value")
+                # Now we call value, ... rest
+                callback(value, data)
+
+        return adaptedCallback
+
+    def _subscribe(self, callback):
+
+        return self._emitter.on(callback=callback)
+
+    def once(self, callback, options=None):
+        ret = None
+
+        def adaptedCallback(data, rest):
+            ret.unsubscribe()
+            callback(data, rest)
+
+        ret = self.subscribe(adaptedCallback, options)
+        return ret
+
+    def waitFor(self, testCallback=None, options=None):
+
+        # Convert our Options.
+
+        _options = ensureDottedAccess({
+            'testCurrent': True,
+            "timeout": 0
+        })
+        _options.update(ensureDottedAccess(options))
+
+        if testCallback is None:
+            # Define a Test Callback
+            def test(value, *args):
+                return value == True
+
+            testCallback = test
+
+        subscription = None
+        timeout = None
+
+        def callback(resolve, reject):
+            nonlocal subscription
+            nonlocal timeout
+
+            first = True
+            resolved = False
+
+            def finish(err, sucessfull, data, timedout):
+                nonlocal first
+                nonlocal resolved
+                nonlocal subscription
+                nonlocal timeout
+
+                if err:
+                    reject(err)
+
+                    if subscription:
+                        subscription.unsubscribe()
+                        subscription = None
+
+                    if timeout and not timedout:
+                        timeout.cancel()
+                elif sucessfull:
+                    if subscription:
+                        subscription.unsubscribe()
+                        subscription = None
+                    if not resolved:
+                        resolved = True
+                        resolve(data)
+
+                    if timeout and not timedout:
+                        timeout.cancel()
+
+            def check_data(value, rest):
+                nonlocal first
+                nonlocal resolved
+                nonlocal subscription
+
+                if (first and _options.testCurrent) or not first:
+                    if isAsyncFunction(testCallback):
+                        # Try to offload the Function
+                        prom: Future = Promise.cast(testCallback(value, rest))
+
+                        def done(p: Future):
+                            nonlocal first
+                            first = False
+
+                            if p.done():
+                                finish(False, True, p.result(), False)
+                            if p.exception():
+                                finish(p.exception(), False, False, False)
+
+                        prom.add_done_callback(done)
+                    else:
+                        result = testCallback(value, rest)
+                        finish(False, result, value, False)
+
+                        first = False
+
+            try:
+                if _options.timeout > 0:
+                    timeout = EXECUTOR.setTimeout(
+                        finish, _options.timeout, TimeoutError("Time elapsed"), False, False, True)
+
+                subscription = self.subscribe(check_data)
+            except BaseException:
+                reject(Exception("Failed to subscribe"))
+
+        return Promise(callback)
+
+    def waitForUpdate(self, options=DottedDict({'testCurrent': True})):
+        # Define a Callback
+        def callback(resolve, reject):
+            def cb(value, rest):
+                resolve(value)
+
+            self.once(cb, options)
+
+        return Promise(callback)
+
+    @property
+    def hasSubscriptions(self):
+        return self._emitter.hasSubscriptions()
+
+    @property
+    def observerLength(self):
+        return self._emitter.amountOfSubscriptions()
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/__init__.py` & `nope_py-1.7.9/nope/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/helpers/asyncHelpers.py` & `nope_py-1.7.9/nope/helpers/asyncHelpers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,479 +1,479 @@
-import asyncio
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
-from functools import partial
-
-from .prints import formatException
-
-
-def isAsyncFunction(func) -> bool:
-    """ Test whether the function is defined async or not.
-
-    Args:
-        func (_type_): _description_
-
-    Returns:
-        bool: _description_
-    """
-    return asyncio.iscoroutinefunction(func)
-
-
-def getOrCreateEventloop():
-    """ Creates or gets the default Eventloop.
-
-    Returns:
-        EventLoop: The determine Eventloop
-    """
-    try:
-        return asyncio.get_event_loop()
-    except RuntimeError as ex:
-        if "There is no current event loop in thread" in str(ex):
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-            return asyncio.get_event_loop()
-        else:
-            raise ex
-
-
-class NopeExecutor:
-    """ Helper for async execution. The executor helps you to run sync functions in extra threads
-        in a compatible manner to NoPE.
-    """
-
-    def __init__(self, loop: asyncio.AbstractEventLoop | None = None,
-                 executor: ThreadPoolExecutor | ProcessPoolExecutor | None = None):
-        self._loop: asyncio.AbstractEventLoop = loop
-        self._executor: ThreadPoolExecutor | ProcessPoolExecutor = executor
-        if self._loop is None:
-            self._loop = getOrCreateEventloop()
-
-        self.logger = None
-        self._todos = set()
-        self._running = False
-
-    def assignLoop(self, loop, forceDefaultToBeDefaultLoop=False):
-        """ Helper to assign a event loop.
-
-        Args:
-            loop (_type_): _description_
-            forceDefaultToBeDefaultLoop (bool, optional): _description_. Defaults to False.
-        """
-        self._loop = loop
-
-        if self.logger:
-            self.logger.warn("Use this function with care!")
-
-        if forceDefaultToBeDefaultLoop:
-            asyncio.set_event_loop(self._loop)
-
-    @property
-    def loop(self) -> asyncio.AbstractEventLoop:
-        """ Returns the used loop
-
-        Returns:
-            asyncio.AbstractEventLoop: The internally used loop
-        """
-        return self._loop
-
-    def useThreadPool(self, max_workers=None):
-        self._executor = ThreadPoolExecutor(max_workers=max_workers)
-
-    def useMultiProcessPool(self, max_workers=None):
-        self._executor = ProcessPoolExecutor(max_workers=max_workers)
-
-    def stop(self, max_iterations=1024):
-        # Determine all open tasks
-        pending = asyncio.all_tasks(loop=self.loop)
-        pending = [t for t in pending if not (t.done() or t.cancelled())]
-        iteration = 0
-
-        while pending:
-            # Create a pending task for all open tasks.
-            group = asyncio.gather(*pending)
-            self.loop.run_until_complete(group)
-
-            if iteration < max_iterations:
-                iteration += 1
-            else:
-                raise Exception("Max Recursion reached.")
-
-            pending = [
-                t for t in asyncio.all_tasks(
-                    loop=self.loop) if not (
-                    t.done() or t.cancelled())]
-
-    def dispose(self, wait=True, cancel_futures=False,
-                finish_open_tasks=False):
-        """ Disposes the Executor """
-
-        if finish_open_tasks:
-            tasks = list(self._todos)
-
-            for t in [t for t in tasks if not (t.done() or t.cancelled())]:
-                # give canceled tasks the last chance to run
-                self.loop.run_until_complete(t)
-
-        self.loop.stop()
-
-        if self._executor:
-            self._executor.shutdown(wait=wait, cancel_futures=cancel_futures)
-
-        self.loop.close()
-
-    def start(self, future, run_tasks=False):
-        if not isinstance(future, (asyncio.Task, asyncio.Future)):
-            raise Exception("Please provide a Future or Task!")
-
-        self._running = True
-        self.loop.run_until_complete(future)
-
-        if run_tasks:
-            tasks = list(self._todos)
-
-            for t in [t for t in tasks if not (t.done() or t.cancelled())]:
-                # give canceled tasks the last chance to run
-                self.loop.run_until_complete(t)
-
-    def run(self, before=None, after=None):
-        """ Starts the eventloop and runs it forever """
-        try:
-            if not self._running:
-                self._running = True
-                self.loop.run_forever()
-
-            else:
-                # tasks = list(self._todos)
-
-                # for t in [t for t in tasks if not (t.done() or t.cancelled())]:
-                #     # give canceled tasks the last chance to run
-                #     self.loop.run_until_complete(t)
-                pass
-
-        except KeyboardInterrupt:
-            print("KeyboardInterrupt detected")
-
-            if callable(before):
-                before()
-
-            tasks = list(self._todos)
-            for t in [t for t in tasks if not (t.done() or t.cancelled())]:
-                # give canceled tasks the last chance to run
-                self.loop.run_until_complete(t)
-
-            if callable(after):
-                after()
-
-            self.dispose()
-
-    def generatePromise(self, **kwargs):
-        """ Helper to create an Future.
-
-            The keys and values of the future are df
-
-        Returns:
-            asyncio.Future: A Future
-        """
-
-        future = self.loop.create_future()
-
-        def _cancel():
-            pass
-
-        setattr(future, 'cancelCallback', _cancel)
-
-        for k, v in kwargs.items():
-            if not hasattr(future, k):
-                setattr(future, k, v)
-            else:
-                raise Exception(
-                    f"You cant use the name {k}. It is predefined by the original Future.")
-
-        return self.ensureExecution(future)
-
-    def ensureExecution(self, todo):
-        """ Make shure, the future / task is being executed. The user do not need to store the
-            item to prevent the garbage collector to remove it.
-
-        Args:
-            todo (Future | Task): The item to take care of
-
-        Returns:
-            Future | Task: The item.
-        """
-        if isinstance(todo, (asyncio.Task, asyncio.Future)):
-            self._todos.add(todo)
-
-            def remove(*args, **kwargs):
-                self._todos.remove(todo)
-
-            todo.add_done_callback(remove)
-
-        return todo
-
-    def setTimeout(self, func, timeout_ms: int, *args, **kwargs):
-        """ Function to call the function after the delay.
-
-        Args:
-            func (function): The function to call.
-            timeout_ms (int): Delay in ms.
-
-        Returns:
-            asyncio.Task: The task, executing the timeout.
-        """
-        function_to_use = self.wrapFuncIfRequired(func)
-
-        async def timeout():
-            promise = None
-            try:
-                await asyncio.sleep(timeout_ms / 1000.0)
-                promise = function_to_use(*args, **kwargs)
-                await promise
-            except asyncio.CancelledError:
-                if self.logger:
-                    self.logger.warn("Loop closed!")
-            except Exception as error:
-                if promise:
-                    if self.logger:
-                        self.logger.error(
-                            "Exception raised during executing 'setTimeout'")
-                        self.logger.error(formatException(error))
-                    else:
-                        print(formatException(error))
-
-        task = self.loop.create_task(timeout())
-
-        return self.ensureExecution(task)
-
-    def setInterval(self, func, interval_ms: int, *args,
-                    **kwargs) -> asyncio.Task:
-        """ Creates an interval which will be called
-
-        Args:
-            func (function): The function to call.
-            interval_ms (int): Interval in ms.
-
-        Returns:
-            asyncio.Task: The task, executing the interval.
-        """
-        function_to_use = self.wrapFuncIfRequired(func)
-
-        async def interval():
-            try:
-                promise = None
-                while True:
-                    await asyncio.sleep(interval_ms / 1000.0)
-                    promise = function_to_use(*args, **kwargs)
-                    await promise
-            except asyncio.CancelledError:
-                if self.logger:
-                    self.logger.warn("Loop closed!")
-            except Exception as error:
-                if self.logger:
-                    self.logger.error(
-                        "Exception raised during executing 'interval'")
-                    self.logger.error(formatException(error))
-                else:
-                    print(formatException(error))
-
-        task = self.loop.create_task(interval())
-
-        return self.ensureExecution(task)
-
-    def callParallel(self, func, *args, done_callback=None, **
-                     kwargs) -> asyncio.Task | asyncio.Future:
-        """ Helper, which will call the function in the Background.
-
-
-        Args:
-            func (function): The function, which should be called in parallel
-
-        Returns:
-            asyncio.Task | asyncio.Future: The Task for the Function.
-        """
-        function_to_use = self.wrapFuncIfRequired(func)
-        task = self.loop.create_task(function_to_use(*args, **kwargs))
-
-        def on_done(future: asyncio.Task):
-            err = future.exception()
-            if err:
-                if self.logger:
-                    self.logger.error(err)
-                    self.logger.error(formatException(err))
-                else:
-                    print(err)
-                    print(formatException(err))
-
-            elif done_callback:
-                done_callback(future)
-
-        # if done_callback:
-        #     task.add_done_callback(done_callback)
-        # else:
-        task.add_done_callback(on_done)
-
-        return self.ensureExecution(task)
-
-    def wrapFuncIfRequired(self, func):
-        """ Helper to asyncify a the provided function if requried. If it is already a coroutine,
-            we will return this, otherwise the function will be wrapped into an async function.
-
-        Args:
-            func (function): The function, which must be will be wrapped
-
-        Returns:
-            corutine: The function as async function
-        """
-        if not callable(func):
-            raise TypeError("The parameter 'func' is not callable")
-
-        if not asyncio.iscoroutinefunction(func):
-            async def run(*args, **kwargs):
-                pfunc = partial(func, *args, **kwargs)
-                try:
-                    return await self.loop.run_in_executor(self._executor, pfunc)
-                except asyncio.CancelledError:
-                    if self.logger:
-                        self.logger.warn("Loop closed!")
-                except Exception as error:
-                    if self.logger:
-                        self.logger.error(
-                            "Exception raised during executing a wrapped sync method '_wrapFuncIfRequired'")
-                        self.logger.error(formatException(error))
-                    else:
-                        print(formatException(error))
-
-            return run
-        else:
-            return func
-
-
-EXECUTOR = NopeExecutor()
-EXECUTOR.useThreadPool()
-
-
-def Promise(callback):
-    """ Creates a NodeJS like Promise
-
-    Args:
-        callback (function or coroutine): The function receiving resolve and reject. Best to be sync.
-
-    Returns:
-        Future: The awaitable Future.
-    """
-    future = EXECUTOR.generatePromise()
-
-    def reject(error):
-        if future.done():
-            print(formatException(Exception("Called 'reject' multiple times")))
-            return
-        future.set_exception(error)
-
-    def resolve(value):
-        if future.done():
-            print(formatException(Exception("Called 'resolve' multiple times")))
-            return
-        future.set_result(value)
-
-    # Now we want call the callback in an extra thread.
-    callback(resolve, reject)
-
-    return future
-
-
-async def waitFor(callback, initalWaitInMs: int | None = None, testFirst: bool = True, maxRetries: int = float("inf"),
-                  delay: int = 50, maxTimeout: int | None = None, additionalDelay: int | None = None):
-    """ Function which will wait for the callback to return true
-
-    Args:
-        callback (function): The Callback which will be checkt with the given delay. The Function must return a boolean value. It can be a coroutine.
-        initalWaitInMs (int, optional): First amount of time to wait. Defaults to None.
-        testFirst (bool, optional): Flag to enable Testing directly (after the intial wait time). Defaults to True.
-        maxRetries (int, optional): Number of allowed retries. Defaults to float("inf").
-        delay (int, optional): The delay in *ms* after which the elements are tested again. Defaults to 50 [ms].
-        maxTimeout (int, optional): The max Time to wait. Throws an error if reached. Defaults to None.
-        additionalDelay (int, optional): _description_. Defaults to None.
-
-    Returns:
-        Promise: A Promise which can be awaited.
-    """
-
-    # Ensure our callback is async.
-    asyncCallback = EXECUTOR.wrapFuncIfRequired(callback)
-
-    # Define our callback, that we will hand over to our Promise.
-
-    async def cb(resolve, reject):
-
-        if initalWaitInMs:
-            # We will wait
-            await asyncio.sleep(initalWaitInMs / 1000.0)
-
-        try:
-            if testFirst and await asyncCallback():
-                if additionalDelay:
-                    await asyncio.sleep(additionalDelay / 1000.0)
-
-                resolve(True)
-                return
-            else:
-                retryCounter = 0
-
-                timeout: asyncio.Task = None
-                interval: asyncio.Task = None
-
-                # If there is a Timeout, define a Timeout Function, which will
-                # Throw an Error on Timeout.
-
-                if maxTimeout:
-                    def onTimeout():
-                        if interval:
-                            interval.cancel()
-
-                        reject(TimeoutError("Timed out!"))
-
-                    timeout = EXECUTOR.setTimeout(onTimeout, maxTimeout)
-
-                # Define a Testfunction, which will periodically test whether the condition is
-                # fullfield or not. Internally it counts the number of retries, if the max allowed
-                # number of retries has been reached => Throw an Error
-
-                async def inInterval():
-                    try:
-                        nonlocal retryCounter
-                        if maxRetries and maxRetries > retryCounter:
-                            # Stop the interval
-                            interval.cancel()
-
-                            if timeout:
-                                timeout.cancel()
-
-                            reject(Exception("Max Retries has been reached!"))
-                        elif await asyncCallback():
-                            # Stop the interval
-                            interval.cancel()
-
-                            if timeout:
-                                timeout.cancel()
-
-                            if additionalDelay:
-                                await asyncio.sleep(additionalDelay / 1000.0)
-
-                            resolve(True)
-
-                        retryCounter += 1
-
-                    except Exception as e:
-                        # Stop the interval
-                        interval.cancel()
-
-                        if timeout:
-                            timeout.cancel()
-
-                        # Forward the Error.
-                        reject(e)
-
-                interval = EXECUTOR.setInterval(inInterval, delay)
-
-        except Exception as e:
-            reject(e)
-
-    return Promise(cb)
+import asyncio
+from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from functools import partial
+
+from .prints import formatException
+
+
+def isAsyncFunction(func) -> bool:
+    """ Test whether the function is defined async or not.
+
+    Args:
+        func (_type_): _description_
+
+    Returns:
+        bool: _description_
+    """
+    return asyncio.iscoroutinefunction(func)
+
+
+def getOrCreateEventloop():
+    """ Creates or gets the default Eventloop.
+
+    Returns:
+        EventLoop: The determine Eventloop
+    """
+    try:
+        return asyncio.get_event_loop()
+    except RuntimeError as ex:
+        if "There is no current event loop in thread" in str(ex):
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            return asyncio.get_event_loop()
+        else:
+            raise ex
+
+
+class NopeExecutor:
+    """ Helper for async execution. The executor helps you to run sync functions in extra threads
+        in a compatible manner to NoPE.
+    """
+
+    def __init__(self, loop: asyncio.AbstractEventLoop | None = None,
+                 executor: ThreadPoolExecutor | ProcessPoolExecutor | None = None):
+        self._loop: asyncio.AbstractEventLoop = loop
+        self._executor: ThreadPoolExecutor | ProcessPoolExecutor = executor
+        if self._loop is None:
+            self._loop = getOrCreateEventloop()
+
+        self.logger = None
+        self._todos = set()
+        self._running = False
+
+    def assignLoop(self, loop, forceDefaultToBeDefaultLoop=False):
+        """ Helper to assign a event loop.
+
+        Args:
+            loop (_type_): _description_
+            forceDefaultToBeDefaultLoop (bool, optional): _description_. Defaults to False.
+        """
+        self._loop = loop
+
+        if self.logger:
+            self.logger.warn("Use this function with care!")
+
+        if forceDefaultToBeDefaultLoop:
+            asyncio.set_event_loop(self._loop)
+
+    @property
+    def loop(self) -> asyncio.AbstractEventLoop:
+        """ Returns the used loop
+
+        Returns:
+            asyncio.AbstractEventLoop: The internally used loop
+        """
+        return self._loop
+
+    def useThreadPool(self, max_workers=None):
+        self._executor = ThreadPoolExecutor(max_workers=max_workers)
+
+    def useMultiProcessPool(self, max_workers=None):
+        self._executor = ProcessPoolExecutor(max_workers=max_workers)
+
+    def stop(self, max_iterations=1024):
+        # Determine all open tasks
+        pending = asyncio.all_tasks(loop=self.loop)
+        pending = [t for t in pending if not (t.done() or t.cancelled())]
+        iteration = 0
+
+        while pending:
+            # Create a pending task for all open tasks.
+            group = asyncio.gather(*pending)
+            self.loop.run_until_complete(group)
+
+            if iteration < max_iterations:
+                iteration += 1
+            else:
+                raise Exception("Max Recursion reached.")
+
+            pending = [
+                t for t in asyncio.all_tasks(
+                    loop=self.loop) if not (
+                    t.done() or t.cancelled())]
+
+    def dispose(self, wait=True, cancel_futures=False,
+                finish_open_tasks=False):
+        """ Disposes the Executor """
+
+        if finish_open_tasks:
+            tasks = list(self._todos)
+
+            for t in [t for t in tasks if not (t.done() or t.cancelled())]:
+                # give canceled tasks the last chance to run
+                self.loop.run_until_complete(t)
+
+        self.loop.stop()
+
+        if self._executor:
+            self._executor.shutdown(wait=wait, cancel_futures=cancel_futures)
+
+        self.loop.close()
+
+    def start(self, future, run_tasks=False):
+        if not isinstance(future, (asyncio.Task, asyncio.Future)):
+            raise Exception("Please provide a Future or Task!")
+
+        self._running = True
+        self.loop.run_until_complete(future)
+
+        if run_tasks:
+            tasks = list(self._todos)
+
+            for t in [t for t in tasks if not (t.done() or t.cancelled())]:
+                # give canceled tasks the last chance to run
+                self.loop.run_until_complete(t)
+
+    def run(self, before=None, after=None):
+        """ Starts the eventloop and runs it forever """
+        try:
+            if not self._running:
+                self._running = True
+                self.loop.run_forever()
+
+            else:
+                # tasks = list(self._todos)
+
+                # for t in [t for t in tasks if not (t.done() or t.cancelled())]:
+                #     # give canceled tasks the last chance to run
+                #     self.loop.run_until_complete(t)
+                pass
+
+        except KeyboardInterrupt:
+            print("KeyboardInterrupt detected")
+
+            if callable(before):
+                before()
+
+            tasks = list(self._todos)
+            for t in [t for t in tasks if not (t.done() or t.cancelled())]:
+                # give canceled tasks the last chance to run
+                self.loop.run_until_complete(t)
+
+            if callable(after):
+                after()
+
+            self.dispose()
+
+    def generatePromise(self, **kwargs):
+        """ Helper to create an Future.
+
+            The keys and values of the future are df
+
+        Returns:
+            asyncio.Future: A Future
+        """
+
+        future = self.loop.create_future()
+
+        def _cancel():
+            pass
+
+        setattr(future, 'cancelCallback', _cancel)
+
+        for k, v in kwargs.items():
+            if not hasattr(future, k):
+                setattr(future, k, v)
+            else:
+                raise Exception(
+                    f"You cant use the name {k}. It is predefined by the original Future.")
+
+        return self.ensureExecution(future)
+
+    def ensureExecution(self, todo):
+        """ Make shure, the future / task is being executed. The user do not need to store the
+            item to prevent the garbage collector to remove it.
+
+        Args:
+            todo (Future | Task): The item to take care of
+
+        Returns:
+            Future | Task: The item.
+        """
+        if isinstance(todo, (asyncio.Task, asyncio.Future)):
+            self._todos.add(todo)
+
+            def remove(*args, **kwargs):
+                self._todos.remove(todo)
+
+            todo.add_done_callback(remove)
+
+        return todo
+
+    def setTimeout(self, func, timeout_ms: int, *args, **kwargs):
+        """ Function to call the function after the delay.
+
+        Args:
+            func (function): The function to call.
+            timeout_ms (int): Delay in ms.
+
+        Returns:
+            asyncio.Task: The task, executing the timeout.
+        """
+        function_to_use = self.wrapFuncIfRequired(func)
+
+        async def timeout():
+            promise = None
+            try:
+                await asyncio.sleep(timeout_ms / 1000.0)
+                promise = function_to_use(*args, **kwargs)
+                await promise
+            except asyncio.CancelledError:
+                if self.logger:
+                    self.logger.warn("Loop closed!")
+            except Exception as error:
+                if promise:
+                    if self.logger:
+                        self.logger.error(
+                            "Exception raised during executing 'setTimeout'")
+                        self.logger.error(formatException(error))
+                    else:
+                        print(formatException(error))
+
+        task = self.loop.create_task(timeout())
+
+        return self.ensureExecution(task)
+
+    def setInterval(self, func, interval_ms: int, *args,
+                    **kwargs) -> asyncio.Task:
+        """ Creates an interval which will be called
+
+        Args:
+            func (function): The function to call.
+            interval_ms (int): Interval in ms.
+
+        Returns:
+            asyncio.Task: The task, executing the interval.
+        """
+        function_to_use = self.wrapFuncIfRequired(func)
+
+        async def interval():
+            try:
+                promise = None
+                while True:
+                    await asyncio.sleep(interval_ms / 1000.0)
+                    promise = function_to_use(*args, **kwargs)
+                    await promise
+            except asyncio.CancelledError:
+                if self.logger:
+                    self.logger.warn("Loop closed!")
+            except Exception as error:
+                if self.logger:
+                    self.logger.error(
+                        "Exception raised during executing 'interval'")
+                    self.logger.error(formatException(error))
+                else:
+                    print(formatException(error))
+
+        task = self.loop.create_task(interval())
+
+        return self.ensureExecution(task)
+
+    def callParallel(self, func, *args, done_callback=None, **
+                     kwargs) -> asyncio.Task | asyncio.Future:
+        """ Helper, which will call the function in the Background.
+
+
+        Args:
+            func (function): The function, which should be called in parallel
+
+        Returns:
+            asyncio.Task | asyncio.Future: The Task for the Function.
+        """
+        function_to_use = self.wrapFuncIfRequired(func)
+        task = self.loop.create_task(function_to_use(*args, **kwargs))
+
+        def on_done(future: asyncio.Task):
+            err = future.exception()
+            if err:
+                if self.logger:
+                    self.logger.error(err)
+                    self.logger.error(formatException(err))
+                else:
+                    print(err)
+                    print(formatException(err))
+
+            elif done_callback:
+                done_callback(future)
+
+        # if done_callback:
+        #     task.add_done_callback(done_callback)
+        # else:
+        task.add_done_callback(on_done)
+
+        return self.ensureExecution(task)
+
+    def wrapFuncIfRequired(self, func):
+        """ Helper to asyncify a the provided function if requried. If it is already a coroutine,
+            we will return this, otherwise the function will be wrapped into an async function.
+
+        Args:
+            func (function): The function, which must be will be wrapped
+
+        Returns:
+            corutine: The function as async function
+        """
+        if not callable(func):
+            raise TypeError("The parameter 'func' is not callable")
+
+        if not asyncio.iscoroutinefunction(func):
+            async def run(*args, **kwargs):
+                pfunc = partial(func, *args, **kwargs)
+                try:
+                    return await self.loop.run_in_executor(self._executor, pfunc)
+                except asyncio.CancelledError:
+                    if self.logger:
+                        self.logger.warn("Loop closed!")
+                except Exception as error:
+                    if self.logger:
+                        self.logger.error(
+                            "Exception raised during executing a wrapped sync method '_wrapFuncIfRequired'")
+                        self.logger.error(formatException(error))
+                    else:
+                        print(formatException(error))
+
+            return run
+        else:
+            return func
+
+
+EXECUTOR = NopeExecutor()
+EXECUTOR.useThreadPool()
+
+
+def Promise(callback):
+    """ Creates a NodeJS like Promise
+
+    Args:
+        callback (function or coroutine): The function receiving resolve and reject. Best to be sync.
+
+    Returns:
+        Future: The awaitable Future.
+    """
+    future = EXECUTOR.generatePromise()
+
+    def reject(error):
+        if future.done():
+            print(formatException(Exception("Called 'reject' multiple times")))
+            return
+        future.set_exception(error)
+
+    def resolve(value):
+        if future.done():
+            print(formatException(Exception("Called 'resolve' multiple times")))
+            return
+        future.set_result(value)
+
+    # Now we want call the callback in an extra thread.
+    callback(resolve, reject)
+
+    return future
+
+
+async def waitFor(callback, initalWaitInMs: int | None = None, testFirst: bool = True, maxRetries: int = float("inf"),
+                  delay: int = 50, maxTimeout: int | None = None, additionalDelay: int | None = None):
+    """ Function which will wait for the callback to return true
+
+    Args:
+        callback (function): The Callback which will be checkt with the given delay. The Function must return a boolean value. It can be a coroutine.
+        initalWaitInMs (int, optional): First amount of time to wait. Defaults to None.
+        testFirst (bool, optional): Flag to enable Testing directly (after the intial wait time). Defaults to True.
+        maxRetries (int, optional): Number of allowed retries. Defaults to float("inf").
+        delay (int, optional): The delay in *ms* after which the elements are tested again. Defaults to 50 [ms].
+        maxTimeout (int, optional): The max Time to wait. Throws an error if reached. Defaults to None.
+        additionalDelay (int, optional): _description_. Defaults to None.
+
+    Returns:
+        Promise: A Promise which can be awaited.
+    """
+
+    # Ensure our callback is async.
+    asyncCallback = EXECUTOR.wrapFuncIfRequired(callback)
+
+    # Define our callback, that we will hand over to our Promise.
+
+    async def cb(resolve, reject):
+
+        if initalWaitInMs:
+            # We will wait
+            await asyncio.sleep(initalWaitInMs / 1000.0)
+
+        try:
+            if testFirst and await asyncCallback():
+                if additionalDelay:
+                    await asyncio.sleep(additionalDelay / 1000.0)
+
+                resolve(True)
+                return
+            else:
+                retryCounter = 0
+
+                timeout: asyncio.Task = None
+                interval: asyncio.Task = None
+
+                # If there is a Timeout, define a Timeout Function, which will
+                # Throw an Error on Timeout.
+
+                if maxTimeout:
+                    def onTimeout():
+                        if interval:
+                            interval.cancel()
+
+                        reject(TimeoutError("Timed out!"))
+
+                    timeout = EXECUTOR.setTimeout(onTimeout, maxTimeout)
+
+                # Define a Testfunction, which will periodically test whether the condition is
+                # fullfield or not. Internally it counts the number of retries, if the max allowed
+                # number of retries has been reached => Throw an Error
+
+                async def inInterval():
+                    try:
+                        nonlocal retryCounter
+                        if maxRetries and maxRetries > retryCounter:
+                            # Stop the interval
+                            interval.cancel()
+
+                            if timeout:
+                                timeout.cancel()
+
+                            reject(Exception("Max Retries has been reached!"))
+                        elif await asyncCallback():
+                            # Stop the interval
+                            interval.cancel()
+
+                            if timeout:
+                                timeout.cancel()
+
+                            if additionalDelay:
+                                await asyncio.sleep(additionalDelay / 1000.0)
+
+                            resolve(True)
+
+                        retryCounter += 1
+
+                    except Exception as e:
+                        # Stop the interval
+                        interval.cancel()
+
+                        if timeout:
+                            timeout.cancel()
+
+                        # Forward the Error.
+                        reject(e)
+
+                interval = EXECUTOR.setInterval(inInterval, delay)
+
+        except Exception as e:
+            reject(e)
+
+    return Promise(cb)
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/dictMethods.py` & `nope_py-1.7.9/nope/helpers/dictMethods.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-from collections.abc import Iterable
-
-from .dottedDict import DottedDict, ensureDottedAccess
-from .objectMethods import convertData, rgetattr, rqueryAttr, flattenObject, rsetattr
-from .path import SPLITCHAR, getLeastCommonPathSegment, pathToCamelCase, pathToSnakeCase
-from .prints import formatException
-from .stringMethods import camelToSnake, snakeToCamel
-
-__SENTINENTAL = object()
-
-
-def keysToSnake(d: dict, adaptStrValues=False):
-    """ helperfunction, which will change the keys to
-        snake case.
-    """
-    ret = {}
-    for key, value in d.items():
-        if adaptStrValues and isinstance(value, str):
-            ret[camelToSnake(key)] = camelToSnake(value)
-        else:
-            ret[camelToSnake(key)] = value
-
-    return ret
-
-
-def keysToSnakeNested(d: dict, adaptStrValues=False):
-    """ helper function, which will change the keys to
-        snake case. this will work with nested dicts as well
-    """
-
-    flatten = flattenObject(d, onlyPathToBaseValue=True)
-
-    ret = ensureDottedAccess({})
-
-    for k, v in flatten.items():
-        if adaptStrValues and isinstance(v, str):
-            rsetattr(ret, pathToSnakeCase(k), camelToSnake(v))
-        else:
-            rsetattr(ret, pathToSnakeCase(k), v)
-
-    return ret
-
-
-def keysToCamel(d: dict, adaptStrValues=False):
-    """ helperfunction, which will change the options to
-        camel case.
-    """
-    ret = {}
-    for key, value in d.items():
-        if adaptStrValues and isinstance(value, str):
-            ret[snakeToCamel(key)] = snakeToCamel(value)
-        else:
-            ret[snakeToCamel(key)] = value
-
-    return ret
-
-
-def keysToCamelNested(d: dict, adaptStrValues=False):
-    """ helperfunction, which will change the options to
-        camel case. this will work with nested dicts as well
-        (expecting every key contains a dict again.)
-    """
-    flatten = flattenObject(d, onlyPathToBaseValue=True)
-
-    ret = ensureDottedAccess({})
-
-    for k, v in flatten.items():
-        if adaptStrValues and isinstance(v, str):
-            rsetattr(ret, pathToCamelCase(k), snakeToCamel(v))
-        else:
-            rsetattr(ret, pathToCamelCase(k), v)
-
-    return ret
-
-
-def extractUniqueValues(d, path='', pathKey: str = None):
-    """ Extracts the unique values of an map.
-
-    Args:
-        d (dict-like): The dict-like object that should be transformed.
-        path (str, optional): The path of the attribute of that should be extracted of the value. Defaults to ''.
-        pathKey (str, optional):   The Path of the unique key. If set to `None` -> The Item is selected directly.
-                                    Defaults to None.
-
-    Returns:
-        set: A set containing the unique values.
-    """
-    if pathKey is None:
-        pathKey = path
-    if path != pathKey:
-        _commonSegment = getLeastCommonPathSegment([path, pathKey], DottedDict(
-            {'considerSingleLevel': False, 'considerMultiLevel': False}))
-
-        # Assign the Value
-        _commonSegment = _commonSegment if _commonSegment is not False else ""
-
-        # Determine the Length of the common segment, to determine the relative
-        # pathes
-        _commonSegmentLength = len(_commonSegment.split(
-            SPLITCHAR)) if _commonSegment != "" else 0
-
-        _relPathContent = SPLITCHAR.join(
-            path.split(SPLITCHAR)[_commonSegmentLength:])
-        _relPathKey = SPLITCHAR.join(pathKey.split(SPLITCHAR)[
-                                     _commonSegmentLength:])
-        _items = extractValues(d, _commonSegment)
-        _keysToUse = set()
-        ret = []
-        for item in _items:
-            # Extract key and data:
-            key = rgetattr(item, _relPathKey) if _relPathKey else item
-            data = rgetattr(item, _relPathContent) if _relPathContent else item
-            if key not in _keysToUse:
-                # Only if the Key has not been used we are allowed to add
-                # the data.
-                _keysToUse.add(key)
-                if data not in ret:
-                    ret.append(data)
-        return ret
-    return extractValues(d, path, unique=True)
-
-
-def extractValues(d, path='', unique=False):
-    """ Helper to extract values of the map. Therefore the path must be provided.
-
-    Example:
-        >> d = {1:{"a": 0}, 2:{"a": 1}}
-        >> r = extractValues(d,"a")
-
-        r = [0,1]
-
-    Args:
-        d (dict-like): The dict-like object that should be transformed.
-        path (str, optional): The path of the attribute of that should be extracted of the value. Defaults to ''.
-        unique (bool, optional): Performs a check to extract only unique values.
-
-    Returns:
-        list: containing the element.
-    """
-    s = list()
-    for v in d.values():
-        if path:
-            for item in rqueryAttr(v, path):
-                if not unique or (unique and (item.data not in s)):
-                    s.append(item.data)
-        elif not unique or (unique and (v not in s)):
-            s.append(v)
-    return s
-
-
-def transformDict(d, pathExtractedValue: str,
-                  pathExtractedKey: str, logger=None):
-    """_summary_
-
-    Args:
-        d (_type_): _description_
-        pathExtractedValue (str): _description_
-        pathExtractedKey (str): _description_
-
-    Returns:
-        _type_: _description_
-    """
-
-    # Initialize all values:
-    keyMapping = dict()
-    reverseKeyMapping = dict()
-    conflicts = dict()
-    extractedDict = dict()
-    orgKeyToExtractedValue = dict()
-    amountOf = dict()
-    props = []
-    onlyValidProps = True
-
-    if isinstance(pathExtractedKey, str):
-        props.append(DottedDict({'key': 'key', 'query': pathExtractedKey}))
-        onlyValidProps = onlyValidProps and (len(pathExtractedKey) > 0)
-    else:
-        onlyValidProps = False
-
-    if isinstance(pathExtractedValue, str):
-        props.append(DottedDict(
-            {'key': 'value', 'query': pathExtractedValue}))
-        onlyValidProps = onlyValidProps and (len(pathExtractedValue) > 0)
-    else:
-        onlyValidProps = False
-
-    keyIsHashable = True
-    valueIsHashable = True
-
-    __warned = False
-
-    # Iterate over the items of the dict,
-    # then we will extract the data stored in the Value.
-    for k, v in d.items():
-        extracted = []
-
-        if onlyValidProps:
-            extracted = convertData(v, props)
-
-            for element in extracted:
-                # Try to convert the data:
-                try:
-                    hash(element.key)
-                    element.keyIsHashable = True
-                except BaseException:
-                    element.keyIsHashable = False
-                    keyIsHashable = False
-
-                # Try to convert the data:
-                try:
-                    hash(element.value)
-                    element.valueIsHashable = True
-                except BaseException:
-                    element.valueIsHashable = False
-                    valueIsHashable = False
-
-        else:
-
-            keys = []
-            values = []
-
-            # We migt adapt the key and the Value. Therefore we will use
-            # the next if statements
-
-            if isinstance(pathExtractedKey, str):
-                if len(pathExtractedKey) > 0:
-                    keys = rqueryAttr(v, pathExtractedKey)
-                else:
-                    keys = [v]
-            else:
-                keys = [k]
-
-            if isinstance(pathExtractedValue, str):
-                if len(pathExtractedValue) > 0:
-                    values = rqueryAttr(v, pathExtractedValue)
-                else:
-                    values = [v]
-            else:
-                values = [v]
-
-            for key in keys:
-                for value in values:
-                    data = DottedDict({
-                        'key': key,
-                        'value': value,
-                        'keyIsHashable': True,
-                        'valueIsHashable': True
-                    })
-
-                    # Try to convert the data:
-                    try:
-                        hash(data.key)
-                    except BaseException:
-                        data.keyIsHashable = False
-                        keyIsHashable = False
-
-                    # Try to convert the data:
-                    try:
-                        hash(data.value)
-                    except BaseException:
-                        data.valueIsHashable = False
-                        valueIsHashable = False
-
-                    extracted.append(data)
-
-        # Create the entries for the following dicts.
-        keyMapping[k] = set()
-        orgKeyToExtractedValue[k] = set() if valueIsHashable else list()
-
-        for item in extracted:
-
-            if not item.keyIsHashable:
-                error = Exception(
-                    f"Can not hash the new key='{item.key}' (type={type(item.key)}) from path='{pathExtractedKey}'")
-
-                if logger:
-                    logger.error(error)
-                else:
-                    print(formatException(error))
-
-                raise error
-
-            if item.key in extractedDict:
-                # If the extracted new key has already been defined,
-                # we have to determine whether the stored item matches
-                # the allready provided definition.
-                if not (extractedDict.get(item.key) == item.value):
-                    # Conflict detected -> Store it
-
-                    if item.key not in conflicts:
-                        conflicts[item.key] = set(
-                        ) if valueIsHashable else list()
-
-                    getattr(conflicts.get(item.key),
-                            "add" if valueIsHashable else "append")(item.value)
-                    getattr(conflicts.get(item.key), "add" if valueIsHashable else "append")(
-                        extractedDict.get(item.key))
-                else:
-                    # No conflict -> just store the amount
-                    amountOf[item.key] = amountOf.get(item.key, 0) + 1
-            else:
-                # Store the item and amount
-                extractedDict[item.key] = item.value
-                amountOf[item.key] = amountOf.get(item.key, 0) + 1
-
-            #  If the reverse haven't been set ==> create it.
-            if not (item.key in reverseKeyMapping):
-                reverseKeyMapping[item.key] = set()
-
-            # Store the mapping of new-key --> org-key.
-            reverseKeyMapping[item.key].add(k)
-
-            # Store the mapping of org-key --> new-key.
-            keyMapping[k].add(item.key)
-
-            # Now store the item.
-            getattr(orgKeyToExtractedValue[k], "add" if valueIsHashable else "append")(
-                item.value)
-
-    return DottedDict({
-        'extracted_map': extractedDict,
-        'keyMapping': keyMapping,
-        'conflicts': conflicts,
-        'keyMappingreverse': reverseKeyMapping,
-        'orgKeyToExtractedValue': orgKeyToExtractedValue,
-        'amountOf': amountOf
-    })
-
-
-def reverse(d, path='', pathKey: str = None):
-    """ Reverses the given map.
-
-        If the path is provided, the Data is extracted based on the given path.
-        If the `pathKey`, a different Key is used.
-
-    Args:
-        d (dict): The dict used as source.
-        path (str, optional): The path for the attributes in the value. Defaults to ''.
-        pathKey (str, optional): The path of the key, which will be provided in the `value`. Defaults to None.
-
-    Returns:
-        dict: The reversed Dict.
-    """
-    ret = dict()
-    if pathKey is None:
-        pathKey = path
-    for k, v in d.items():
-        keyToUse = k
-
-        if pathKey:
-            keyToUse = rgetattr(v, pathKey, __SENTINENTAL)
-        valueToUse = v
-        if path:
-            valueToUse = rgetattr(v, path, __SENTINENTAL)
-        if isinstance(valueToUse, Iterable):
-            for _v in valueToUse:
-                if _v not in ret:
-                    ret[_v] = set()
-                ret.get(_v).add(keyToUse)
-        else:
-            if valueToUse not in ret:
-                ret[valueToUse] = set()
-            ret.get(valueToUse).add(keyToUse)
-    return ret
+from collections.abc import Iterable
+
+from .dottedDict import DottedDict, ensureDottedAccess
+from .objectMethods import convertData, rgetattr, rqueryAttr, flattenObject, rsetattr
+from .path import SPLITCHAR, getLeastCommonPathSegment, pathToCamelCase, pathToSnakeCase
+from .prints import formatException
+from .stringMethods import camelToSnake, snakeToCamel
+
+__SENTINENTAL = object()
+
+
+def keysToSnake(d: dict, adaptStrValues=False):
+    """ helperfunction, which will change the keys to
+        snake case.
+    """
+    ret = {}
+    for key, value in d.items():
+        if adaptStrValues and isinstance(value, str):
+            ret[camelToSnake(key)] = camelToSnake(value)
+        else:
+            ret[camelToSnake(key)] = value
+
+    return ret
+
+
+def keysToSnakeNested(d: dict, adaptStrValues=False):
+    """ helper function, which will change the keys to
+        snake case. this will work with nested dicts as well
+    """
+
+    flatten = flattenObject(d, onlyPathToBaseValue=True)
+
+    ret = ensureDottedAccess({})
+
+    for k, v in flatten.items():
+        if adaptStrValues and isinstance(v, str):
+            rsetattr(ret, pathToSnakeCase(k), camelToSnake(v))
+        else:
+            rsetattr(ret, pathToSnakeCase(k), v)
+
+    return ret
+
+
+def keysToCamel(d: dict, adaptStrValues=False):
+    """ helperfunction, which will change the options to
+        camel case.
+    """
+    ret = {}
+    for key, value in d.items():
+        if adaptStrValues and isinstance(value, str):
+            ret[snakeToCamel(key)] = snakeToCamel(value)
+        else:
+            ret[snakeToCamel(key)] = value
+
+    return ret
+
+
+def keysToCamelNested(d: dict, adaptStrValues=False):
+    """ helperfunction, which will change the options to
+        camel case. this will work with nested dicts as well
+        (expecting every key contains a dict again.)
+    """
+    flatten = flattenObject(d, onlyPathToBaseValue=True)
+
+    ret = ensureDottedAccess({})
+
+    for k, v in flatten.items():
+        if adaptStrValues and isinstance(v, str):
+            rsetattr(ret, pathToCamelCase(k), snakeToCamel(v))
+        else:
+            rsetattr(ret, pathToCamelCase(k), v)
+
+    return ret
+
+
+def extractUniqueValues(d, path='', pathKey: str = None):
+    """ Extracts the unique values of an map.
+
+    Args:
+        d (dict-like): The dict-like object that should be transformed.
+        path (str, optional): The path of the attribute of that should be extracted of the value. Defaults to ''.
+        pathKey (str, optional):   The Path of the unique key. If set to `None` -> The Item is selected directly.
+                                    Defaults to None.
+
+    Returns:
+        set: A set containing the unique values.
+    """
+    if pathKey is None:
+        pathKey = path
+    if path != pathKey:
+        _commonSegment = getLeastCommonPathSegment([path, pathKey], DottedDict(
+            {'considerSingleLevel': False, 'considerMultiLevel': False}))
+
+        # Assign the Value
+        _commonSegment = _commonSegment if _commonSegment is not False else ""
+
+        # Determine the Length of the common segment, to determine the relative
+        # pathes
+        _commonSegmentLength = len(_commonSegment.split(
+            SPLITCHAR)) if _commonSegment != "" else 0
+
+        _relPathContent = SPLITCHAR.join(
+            path.split(SPLITCHAR)[_commonSegmentLength:])
+        _relPathKey = SPLITCHAR.join(pathKey.split(SPLITCHAR)[
+                                     _commonSegmentLength:])
+        _items = extractValues(d, _commonSegment)
+        _keysToUse = set()
+        ret = []
+        for item in _items:
+            # Extract key and data:
+            key = rgetattr(item, _relPathKey) if _relPathKey else item
+            data = rgetattr(item, _relPathContent) if _relPathContent else item
+            if key not in _keysToUse:
+                # Only if the Key has not been used we are allowed to add
+                # the data.
+                _keysToUse.add(key)
+                if data not in ret:
+                    ret.append(data)
+        return ret
+    return extractValues(d, path, unique=True)
+
+
+def extractValues(d, path='', unique=False):
+    """ Helper to extract values of the map. Therefore the path must be provided.
+
+    Example:
+        >> d = {1:{"a": 0}, 2:{"a": 1}}
+        >> r = extractValues(d,"a")
+
+        r = [0,1]
+
+    Args:
+        d (dict-like): The dict-like object that should be transformed.
+        path (str, optional): The path of the attribute of that should be extracted of the value. Defaults to ''.
+        unique (bool, optional): Performs a check to extract only unique values.
+
+    Returns:
+        list: containing the element.
+    """
+    s = list()
+    for v in d.values():
+        if path:
+            for item in rqueryAttr(v, path):
+                if not unique or (unique and (item.data not in s)):
+                    s.append(item.data)
+        elif not unique or (unique and (v not in s)):
+            s.append(v)
+    return s
+
+
+def transformDict(d, pathExtractedValue: str,
+                  pathExtractedKey: str, logger=None):
+    """_summary_
+
+    Args:
+        d (_type_): _description_
+        pathExtractedValue (str): _description_
+        pathExtractedKey (str): _description_
+
+    Returns:
+        _type_: _description_
+    """
+
+    # Initialize all values:
+    keyMapping = dict()
+    reverseKeyMapping = dict()
+    conflicts = dict()
+    extractedDict = dict()
+    orgKeyToExtractedValue = dict()
+    amountOf = dict()
+    props = []
+    onlyValidProps = True
+
+    if isinstance(pathExtractedKey, str):
+        props.append(DottedDict({'key': 'key', 'query': pathExtractedKey}))
+        onlyValidProps = onlyValidProps and (len(pathExtractedKey) > 0)
+    else:
+        onlyValidProps = False
+
+    if isinstance(pathExtractedValue, str):
+        props.append(DottedDict(
+            {'key': 'value', 'query': pathExtractedValue}))
+        onlyValidProps = onlyValidProps and (len(pathExtractedValue) > 0)
+    else:
+        onlyValidProps = False
+
+    keyIsHashable = True
+    valueIsHashable = True
+
+    __warned = False
+
+    # Iterate over the items of the dict,
+    # then we will extract the data stored in the Value.
+    for k, v in d.items():
+        extracted = []
+
+        if onlyValidProps:
+            extracted = convertData(v, props)
+
+            for element in extracted:
+                # Try to convert the data:
+                try:
+                    hash(element.key)
+                    element.keyIsHashable = True
+                except BaseException:
+                    element.keyIsHashable = False
+                    keyIsHashable = False
+
+                # Try to convert the data:
+                try:
+                    hash(element.value)
+                    element.valueIsHashable = True
+                except BaseException:
+                    element.valueIsHashable = False
+                    valueIsHashable = False
+
+        else:
+
+            keys = []
+            values = []
+
+            # We migt adapt the key and the Value. Therefore we will use
+            # the next if statements
+
+            if isinstance(pathExtractedKey, str):
+                if len(pathExtractedKey) > 0:
+                    keys = rqueryAttr(v, pathExtractedKey)
+                else:
+                    keys = [v]
+            else:
+                keys = [k]
+
+            if isinstance(pathExtractedValue, str):
+                if len(pathExtractedValue) > 0:
+                    values = rqueryAttr(v, pathExtractedValue)
+                else:
+                    values = [v]
+            else:
+                values = [v]
+
+            for key in keys:
+                for value in values:
+                    data = DottedDict({
+                        'key': key,
+                        'value': value,
+                        'keyIsHashable': True,
+                        'valueIsHashable': True
+                    })
+
+                    # Try to convert the data:
+                    try:
+                        hash(data.key)
+                    except BaseException:
+                        data.keyIsHashable = False
+                        keyIsHashable = False
+
+                    # Try to convert the data:
+                    try:
+                        hash(data.value)
+                    except BaseException:
+                        data.valueIsHashable = False
+                        valueIsHashable = False
+
+                    extracted.append(data)
+
+        # Create the entries for the following dicts.
+        keyMapping[k] = set()
+        orgKeyToExtractedValue[k] = set() if valueIsHashable else list()
+
+        for item in extracted:
+
+            if not item.keyIsHashable:
+                error = Exception(
+                    f"Can not hash the new key='{item.key}' (type={type(item.key)}) from path='{pathExtractedKey}'")
+
+                if logger:
+                    logger.error(error)
+                else:
+                    print(formatException(error))
+
+                raise error
+
+            if item.key in extractedDict:
+                # If the extracted new key has already been defined,
+                # we have to determine whether the stored item matches
+                # the allready provided definition.
+                if not (extractedDict.get(item.key) == item.value):
+                    # Conflict detected -> Store it
+
+                    if item.key not in conflicts:
+                        conflicts[item.key] = set(
+                        ) if valueIsHashable else list()
+
+                    getattr(conflicts.get(item.key),
+                            "add" if valueIsHashable else "append")(item.value)
+                    getattr(conflicts.get(item.key), "add" if valueIsHashable else "append")(
+                        extractedDict.get(item.key))
+                else:
+                    # No conflict -> just store the amount
+                    amountOf[item.key] = amountOf.get(item.key, 0) + 1
+            else:
+                # Store the item and amount
+                extractedDict[item.key] = item.value
+                amountOf[item.key] = amountOf.get(item.key, 0) + 1
+
+            #  If the reverse haven't been set ==> create it.
+            if not (item.key in reverseKeyMapping):
+                reverseKeyMapping[item.key] = set()
+
+            # Store the mapping of new-key --> org-key.
+            reverseKeyMapping[item.key].add(k)
+
+            # Store the mapping of org-key --> new-key.
+            keyMapping[k].add(item.key)
+
+            # Now store the item.
+            getattr(orgKeyToExtractedValue[k], "add" if valueIsHashable else "append")(
+                item.value)
+
+    return DottedDict({
+        'extracted_map': extractedDict,
+        'keyMapping': keyMapping,
+        'conflicts': conflicts,
+        'keyMappingreverse': reverseKeyMapping,
+        'orgKeyToExtractedValue': orgKeyToExtractedValue,
+        'amountOf': amountOf
+    })
+
+
+def reverse(d, path='', pathKey: str = None):
+    """ Reverses the given map.
+
+        If the path is provided, the Data is extracted based on the given path.
+        If the `pathKey`, a different Key is used.
+
+    Args:
+        d (dict): The dict used as source.
+        path (str, optional): The path for the attributes in the value. Defaults to ''.
+        pathKey (str, optional): The path of the key, which will be provided in the `value`. Defaults to None.
+
+    Returns:
+        dict: The reversed Dict.
+    """
+    ret = dict()
+    if pathKey is None:
+        pathKey = path
+    for k, v in d.items():
+        keyToUse = k
+
+        if pathKey:
+            keyToUse = rgetattr(v, pathKey, __SENTINENTAL)
+        valueToUse = v
+        if path:
+            valueToUse = rgetattr(v, path, __SENTINENTAL)
+        if isinstance(valueToUse, Iterable):
+            for _v in valueToUse:
+                if _v not in ret:
+                    ret[_v] = set()
+                ret.get(_v).add(keyToUse)
+        else:
+            if valueToUse not in ret:
+                ret[valueToUse] = set()
+            ret.get(valueToUse).add(keyToUse)
+    return ret
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/dispatcherPathes.py` & `nope_py-1.7.9/nope/helpers/dispatcherPathes.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .path import SPLITCHAR
-
-
-def getPropertyPath(identifier, name):
-    return f'{identifier}{SPLITCHAR}properties{SPLITCHAR}{name}'
-
-
-def isPropertyPathCorrect(identifier, path):
-    return path.startswith(f'{identifier}{SPLITCHAR}properties{SPLITCHAR}')
-
-
-def getMethodPath(identifier, name):
-    return f'{identifier}{SPLITCHAR}methods{SPLITCHAR}{name}'
-
-
-def isMethodPathCorrect(identifier, path):
-    return path.startswith(f'{identifier}{SPLITCHAR}methods{SPLITCHAR}')
-
-
-def getEmitterPath(identifier, name):
-    return f'{identifier}{SPLITCHAR}events{SPLITCHAR}{name}'
-
-
-def isEmitterPathCorrect(identifier, path):
-    return path.startswith(f'{identifier}{SPLITCHAR}events{SPLITCHAR}')
+from .path import SPLITCHAR
+
+
+def getPropertyPath(identifier, name):
+    return f'{identifier}{SPLITCHAR}properties{SPLITCHAR}{name}'
+
+
+def isPropertyPathCorrect(identifier, path):
+    return path.startswith(f'{identifier}{SPLITCHAR}properties{SPLITCHAR}')
+
+
+def getMethodPath(identifier, name):
+    return f'{identifier}{SPLITCHAR}methods{SPLITCHAR}{name}'
+
+
+def isMethodPathCorrect(identifier, path):
+    return path.startswith(f'{identifier}{SPLITCHAR}methods{SPLITCHAR}')
+
+
+def getEmitterPath(identifier, name):
+    return f'{identifier}{SPLITCHAR}events{SPLITCHAR}{name}'
+
+
+def isEmitterPathCorrect(identifier, path):
+    return path.startswith(f'{identifier}{SPLITCHAR}events{SPLITCHAR}')
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/emitter.py` & `nope_py-1.7.9/nope/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/helpers/files.py` & `nope_py-1.7.9/nope/helpers/files.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import os
-import pathlib
-
-
-def createFile(path: str, with_file=True):
-    """ Helper to create a path to a file.
-
-    Args:
-        path (str): The Path with or without a file.
-        with_file (bool, optional): If the file is contained the Flag must be set to true. Defaults to True.
-    """
-
-    sep = os.sep
-    abs_path = pathlib.Path(path).absolute()
-    if not abs_path.exists():
-
-        if with_file:
-            abs_path_as_str = str(abs_path)
-            path_segments = abs_path_as_str.split(sep)
-
-            if len(path_segments) > 0:
-                pathlib.Path(
-                    sep.join(path_segments[:-1])).mkdir(parents=True, exist_ok=True)
-
-            abs_path.touch(exist_ok=True)
-
-        else:
-
-            abs_path.mkdir(parents=True, exist_ok=True)
-
-    return str(abs_path)
+import os
+import pathlib
+
+
+def createFile(path: str, with_file=True):
+    """ Helper to create a path to a file.
+
+    Args:
+        path (str): The Path with or without a file.
+        with_file (bool, optional): If the file is contained the Flag must be set to true. Defaults to True.
+    """
+
+    sep = os.sep
+    abs_path = pathlib.Path(path).absolute()
+    if not abs_path.exists():
+
+        if with_file:
+            abs_path_as_str = str(abs_path)
+            path_segments = abs_path_as_str.split(sep)
+
+            if len(path_segments) > 0:
+                pathlib.Path(
+                    sep.join(path_segments[:-1])).mkdir(parents=True, exist_ok=True)
+
+            abs_path.touch(exist_ok=True)
+
+        else:
+
+            abs_path.mkdir(parents=True, exist_ok=True)
+
+    return str(abs_path)
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/hashable.py` & `nope_py-1.7.9/nope/helpers/hashable.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,454 +1,454 @@
-"""This module proposes hashable version of the mutable containers
-`list`, `dict` and `set`, called respectively `hlist`, `hdict` and
-`hset`.
-After one object has been hashed, it becomes not mutable and raises a
-`ValueError` if a method which changes the object (let call a
-_mutation_ such a method) is invoqued. The object can be then
-un-hashed by calling `unhash` on it so that it becomes mutable again.
-Notice that this may cause troubles if the object is stored in a set
-or dict which uses its hashcode to locate it. Notice also that
-hashable containers cannot be hashed if they contain non hashable
-objects.
->>> l = hlist(range(5))
->>> l
-hlist([0, 1, 2, 3, 4])
->>> _ = hash(l)
->>> l.append(5)
-Traceback (most recent call last):
-...
-ValueError: hashed 'hlist' object is not mutable
->>> unhash(l)
->>> l.append(5)
->>> l
-hlist([0, 1, 2, 3, 4, 5])
-Testing if a `hlist` is in a `set`, `dict`, `hset` or `hdict` causes
-its hashing. If this is not desirable, you should either compensate
-with a call to `unhash`, or test if a copy is in the set:
->>> s = set()
->>> s.add(list(range(4)))
-Traceback (most recent call last):
-...
-TypeError: ...
->>> s.add(hlist(range(4)))
->>> l = hlist(range(3))
->>> l in s
-False
->>> l.append(3)
-Traceback (most recent call last):
-...
-ValueError: hashed 'hlist' object is not mutable
->>> unhash(l)
->>> l.append(3)
->>> l[:] in s
-True
->>> l.append(4)
-"""
-
-import inspect
-from functools import reduce
-from operator import xor
-
-
-def unhash(obj):
-    """Make the object mutable again. This should be used with
-    caution, especially if the object is stored in a dict or a set.
-    >>> l = hlist(range(3))
-    >>> _ = hash(l)
-    >>> l.append(3)
-    Traceback (most recent call last):
-    ...
-    ValueError: hashed 'hlist' object is not mutable
-    >>> unhash(l)
-    >>> l.append(3)
-    @param obj: any object
-    @type obj: `object`
-    """
-    try:
-        del obj._hash
-    except BaseException:
-        pass
-
-
-# apidoc skip
-def hashable(cls):
-    """Wrap methods in a class in order to make it hashable.
-    """
-    classname, bases, classdict = cls.__name__, cls.__bases__, cls.__dict__
-    for name, attr in classdict.items():
-        try:
-            doc = inspect.getdoc(attr)
-            if doc is None:
-                attr.__doc__ = getattr(bases[0], name).__doc__
-            else:
-                attr.__doc__ = "\n".join([inspect.getdoc(getattr(bases[0],
-                                                                 name)),
-                                          doc])
-        except BaseException:
-            pass
-
-    def __hash__(self):
-        if not hasattr(self, "__hash") or self.__hash is None:
-            self.__hash = self.__hash__.HASH(self)
-        return self.__hash
-
-    __hash__.HASH = classdict["__hash__"]
-    __hash__.__doc__ = classdict["__hash__"].__doc__
-    cls.__hash__ = __hash__
-
-    def __mutable__(self):
-        "Raise `ValueError` if the %s has been hashed."
-        if self.hashed():
-            raise ValueError("hashed '%s' object is not mutable" % classname)
-
-    try:
-        __mutable__.__doc__ = __mutable__.__doc__ % classname
-    except BaseException:
-        pass
-    cls.__mutable__ = __mutable__
-
-    def hashed(self):
-        "Return 'True' if the %s has been hashed, 'False' otherwise."
-        return hasattr(self, "__hash") and self.__hash is not None
-
-    try:
-        hashed.__doc__ = hashed.__doc__ % classname
-    except BaseException:
-        pass
-    cls.hashed = hashed
-
-    def mutable(self):
-        "Return 'True' if the %s is not hashed, 'False' otherwise."
-        return not self.hashed()
-
-    try:
-        mutable.__doc__ = mutable.__doc__ % classname
-    except BaseException:
-        pass
-    cls.mutable = mutable
-    return cls
-
-
-class hlist(list):
-    """Hashable lists. They support all standard methods from `list`.
-    >>> l = hlist(range(5))
-    >>> l
-    hlist([0, 1, 2, 3, 4])
-    >>> l.append(5)
-    >>> l
-    hlist([0, 1, 2, 3, 4, 5])
-    >>> _ = hash(l)
-    >>> l.append(6)
-    Traceback (most recent call last):
-    ...
-    ValueError: hashed 'hlist' object is not mutable
-    >>> unhash(l)
-    >>> l.append(6)
-    """
-
-    # apidoc stop
-    def __add__(self, other):
-        return self.__class__(list.__add__(self, other))
-
-    def __delitem__(self, item):
-        self.__mutable__()
-        list.__delitem__(self, item)
-
-    def __delslice__(self, *l, **d):
-        self.__mutable__()
-        list.__delslice__(self, *l, **d)
-
-    def __getslice__(self, first, last):
-        return self.__class__(list.__getslice__(self, first, last))
-
-    def __getitem__(self, item):
-        ret = list.__getitem__(self, item)
-        if ret.__class__ is list:
-            return self.__class__(ret)
-        return ret
-
-    def __hash__(self):
-        return hash(tuple(self))
-
-    def __iadd__(self, other):
-        return self.__class__(list.__iadd__(self, other))
-
-    def __imul__(self, n):
-        return self.__class__(list.__imul__(self, n))
-
-    def __mul__(self, n):
-        return self.__class__(list.__mul__(self, n))
-
-    def __repr__(self):
-        """
-        >>> repr(hlist(range(3)))
-        'hlist([0, 1, 2])'
-        """
-        return "%s(%s)" % (self.__class__.__name__, list.__repr__(self))
-
-    def __rmul__(self, n):
-        return self._class__(list.__rmul__(self, n))
-
-    def __setitem__(self, index, item):
-        self.__mutable__()
-        list.__setitem__(self, index, item)
-
-    def __setslice__(self, first, last, item):
-        self.__mutable__()
-        list.__setslice__(self, first, last, item)
-
-    def append(self, item):
-        self.__mutable__()
-        list.append(self, item)
-
-    def extend(self, iterable):
-        self.__mutable__()
-        list.extend(self, iterable)
-
-    def insert(self, index, item):
-        self.__mutable__()
-        list.insert(self, index, item)
-
-    def pop(self, index=-1):
-        self.__mutable__()
-        return list.pop(self, index)
-
-    def remove(self, item):
-        self.__mutable__()
-        list.remove(self, item)
-
-    def reverse(self):
-        self.__mutable__()
-        list.reverse(self)
-
-    def sort(self, cmp=None, key=None, reverse=False):
-        self.__mutable__()
-        list.sort(self, cmp, key, reverse)
-
-
-hlist = hashable(hlist)
-
-
-class hdict(dict):
-    """Hashable dictionnaries. They support all standard methods from
-    `dict`.
-    >>> l = hlist(range(5))
-    >>> d = hdict([(l, 0)])
-    >>> d
-    hdict({hlist([0, 1, 2, 3, 4]): 0})
-    >>> l in d
-    True
-    >>> [0, 1, 2, 3, 4] in d
-    Traceback (most recent call last):
-    ...
-    TypeError: ...
-    >>> hlist([0, 1, 2, 3, 4]) in d
-    True
-    >>> d[hlist([0, 1, 2, 3, 4])]
-    0
-    >>> l.append(5)
-    Traceback (most recent call last):
-    ...
-    ValueError: hashed 'hlist' object is not mutable
-    >>> _ = hash(d)
-    >>> d.pop(l)  # any mutation would produce the same error
-    Traceback (most recent call last):
-    ...
-    ValueError: hashed 'hdict' object is not mutable
-    >>> unhash(d)
-    >>> d.pop(l)
-    0
-    """
-
-    # apidoc stop
-    def __delitem__(self, key):
-        self.__mutable__()
-        dict.__delitem__(self, key)
-
-    def __hash__(self):
-        """
-        >>> _ = hash(hdict(a=1, b=2))
-        """
-        # 252756382 = hash("snakes.hashables.hlist")
-        return reduce(xor, (hash(i) for i in self.items()), 252756382)
-
-    def __repr__(self):
-        """
-        >>> repr(hdict(a=1))
-        "hdict({'a': 1})"
-        """
-        return "%s(%s)" % (self.__class__.__name__, dict.__repr__(self))
-
-    def __setitem__(self, key, item):
-        self.__mutable__()
-        dict.__setitem__(self, key, item)
-
-    def clear(self):
-        self.__mutable__()
-        dict.clear(self)
-
-    def copy(self):
-        return self.__class__(dict.copy(self))
-
-    @classmethod
-    def fromkeys(_class, *args):
-        return _class(dict.fromkeys(*args))
-
-    def pop(self, *args):
-        self.__mutable__()
-        return dict.pop(self, *args)
-
-    def popitem(self):
-        self.__mutable__()
-        return dict.popitem(self)
-
-    def setdefault(self, key, item=None):
-        self.__mutable__()
-        return dict.setdefault(self, key, item)
-
-    def update(self, other, **more):
-        self.__mutable__()
-        return dict.update(self, other, **more)
-
-
-hdict = hashable(hdict)
-
-
-class hset(set):
-    """Hashable sets. They support all standard methods from `set`.
-    >>> s = hset()
-    >>> l = hlist(range(5))
-    >>> s.add(l)
-    >>> s
-    hset([hlist([0, 1, 2, 3, 4])])
-    >>> l in s
-    True
-    >>> [0, 1, 2, 3, 4] in s
-    Traceback (most recent call last):
-    ...
-    TypeError: ...
-    >>> hlist([0, 1, 2, 3, 4]) in s
-    True
-    >>> l.append(5)
-    Traceback (most recent call last):
-    ...
-    ValueError: hashed 'hlist' object is not mutable
-    >>> _ = hash(s)
-    >>> s.discard(l)  # any mutation would produce the same error
-    Traceback (most recent call last):
-    ...
-    ValueError: hashed 'hset' object is not mutable
-    >>> unhash(s)
-    >>> s.discard(l)
-    """
-
-    # apidoc stop
-    def __and__(self, other):
-        return self.__class__(set.__and__(self, other))
-
-    def __hash__(self):
-        """
-        >>> _ = hash(hset([1, 2, 3]))
-        >>> _ = hash(hset(range(5)) - set([0, 4]))
-        """
-        # 196496309 = hash("snakes.hashables.hset")
-        return reduce(xor, (hash(x) for x in self), 196496309)
-
-    def __iand__(self, other):
-        return self.__class__(set.__iand__(self, other))
-
-    def __ior__(self, other):
-        return self.__class__(set.__ior__(self, other))
-
-    def __isub__(self, other):
-        return self.__class__(set.__isub__(self, other))
-
-    def __ixor__(self, other):
-        return self.__class__(set.__ixor__(self, other))
-
-    def __or__(self, other):
-        return self.__class__(set.__or__(self, other))
-
-    def __rand__(self, other):
-        return self.__class__(set.__rand__(self, other))
-
-    def __repr__(self):
-        """
-        >>> repr(hset([1]))
-        'hset([1])'
-        """
-        return "%s([%s])" % (self.__class__.__name__,
-                             set.__repr__(self)[6:-2])
-
-    def __ror__(self, other):
-        return self.__class__(set.__ror__(self, other))
-
-    def __rsub__(self, other):
-        return self.__class__(set.__rsub__(self, other))
-
-    def __rxor__(self, other):
-        return self.__class__(set.__rxor__(self, other))
-
-    def __str__(self):
-        return self.__class__.__name__ + \
-            "(" + set.__str__(self).split("(", 1)[1]
-
-    def __sub__(self, other):
-        return self.__class__(set.__sub__(self, other))
-
-    def __xor__(self, other):
-        return self.__class__(set.__xor__(self, other))
-
-    def add(self, item):
-        self.__mutable__()
-        set.add(self, item)
-
-    def clear(self):
-        self.__mutable__()
-        set.clear(self)
-
-    def copy(self):
-        return self.__class__(set.copy(self))
-
-    def difference(self, other):
-        return self.__class__(set.difference(self, other))
-
-    def difference_update(self, other):
-        self.__mutable__()
-        set.difference_update(self, other)
-
-    def discard(self, item):
-        self.__mutable__()
-        set.discard(self, item)
-
-    def intersection(self, other):
-        return self._class__(set.intersection(self, other))
-
-    def intersection_update(self, other):
-        self.__mutable__()
-        set.intersection_update(self, other)
-
-    def pop(self):
-        self.__mutable__()
-        return set.pop(self)
-
-    def remove(self, item):
-        self.__mutable__()
-        set.remove(self, item)
-
-    def symmetric_difference(self, other):
-        self.__mutable__()
-        set.symmetric_difference(self, other)
-
-    def symmetric_difference_update(self, other):
-        self.__mutable__()
-        set.symmetric_difference_update(self, other)
-
-    def union(self, other):
-        return self.__class__(set.union(self, other))
-
-    def update(self, other):
-        self.__mutable__()
-        set.update(self, other)
-
-
-hset = hashable(hset)
+"""This module proposes hashable version of the mutable containers
+`list`, `dict` and `set`, called respectively `hlist`, `hdict` and
+`hset`.
+After one object has been hashed, it becomes not mutable and raises a
+`ValueError` if a method which changes the object (let call a
+_mutation_ such a method) is invoqued. The object can be then
+un-hashed by calling `unhash` on it so that it becomes mutable again.
+Notice that this may cause troubles if the object is stored in a set
+or dict which uses its hashcode to locate it. Notice also that
+hashable containers cannot be hashed if they contain non hashable
+objects.
+>>> l = hlist(range(5))
+>>> l
+hlist([0, 1, 2, 3, 4])
+>>> _ = hash(l)
+>>> l.append(5)
+Traceback (most recent call last):
+...
+ValueError: hashed 'hlist' object is not mutable
+>>> unhash(l)
+>>> l.append(5)
+>>> l
+hlist([0, 1, 2, 3, 4, 5])
+Testing if a `hlist` is in a `set`, `dict`, `hset` or `hdict` causes
+its hashing. If this is not desirable, you should either compensate
+with a call to `unhash`, or test if a copy is in the set:
+>>> s = set()
+>>> s.add(list(range(4)))
+Traceback (most recent call last):
+...
+TypeError: ...
+>>> s.add(hlist(range(4)))
+>>> l = hlist(range(3))
+>>> l in s
+False
+>>> l.append(3)
+Traceback (most recent call last):
+...
+ValueError: hashed 'hlist' object is not mutable
+>>> unhash(l)
+>>> l.append(3)
+>>> l[:] in s
+True
+>>> l.append(4)
+"""
+
+import inspect
+from functools import reduce
+from operator import xor
+
+
+def unhash(obj):
+    """Make the object mutable again. This should be used with
+    caution, especially if the object is stored in a dict or a set.
+    >>> l = hlist(range(3))
+    >>> _ = hash(l)
+    >>> l.append(3)
+    Traceback (most recent call last):
+    ...
+    ValueError: hashed 'hlist' object is not mutable
+    >>> unhash(l)
+    >>> l.append(3)
+    @param obj: any object
+    @type obj: `object`
+    """
+    try:
+        del obj._hash
+    except BaseException:
+        pass
+
+
+# apidoc skip
+def hashable(cls):
+    """Wrap methods in a class in order to make it hashable.
+    """
+    classname, bases, classdict = cls.__name__, cls.__bases__, cls.__dict__
+    for name, attr in classdict.items():
+        try:
+            doc = inspect.getdoc(attr)
+            if doc is None:
+                attr.__doc__ = getattr(bases[0], name).__doc__
+            else:
+                attr.__doc__ = "\n".join([inspect.getdoc(getattr(bases[0],
+                                                                 name)),
+                                          doc])
+        except BaseException:
+            pass
+
+    def __hash__(self):
+        if not hasattr(self, "__hash") or self.__hash is None:
+            self.__hash = self.__hash__.HASH(self)
+        return self.__hash
+
+    __hash__.HASH = classdict["__hash__"]
+    __hash__.__doc__ = classdict["__hash__"].__doc__
+    cls.__hash__ = __hash__
+
+    def __mutable__(self):
+        "Raise `ValueError` if the %s has been hashed."
+        if self.hashed():
+            raise ValueError("hashed '%s' object is not mutable" % classname)
+
+    try:
+        __mutable__.__doc__ = __mutable__.__doc__ % classname
+    except BaseException:
+        pass
+    cls.__mutable__ = __mutable__
+
+    def hashed(self):
+        "Return 'True' if the %s has been hashed, 'False' otherwise."
+        return hasattr(self, "__hash") and self.__hash is not None
+
+    try:
+        hashed.__doc__ = hashed.__doc__ % classname
+    except BaseException:
+        pass
+    cls.hashed = hashed
+
+    def mutable(self):
+        "Return 'True' if the %s is not hashed, 'False' otherwise."
+        return not self.hashed()
+
+    try:
+        mutable.__doc__ = mutable.__doc__ % classname
+    except BaseException:
+        pass
+    cls.mutable = mutable
+    return cls
+
+
+class hlist(list):
+    """Hashable lists. They support all standard methods from `list`.
+    >>> l = hlist(range(5))
+    >>> l
+    hlist([0, 1, 2, 3, 4])
+    >>> l.append(5)
+    >>> l
+    hlist([0, 1, 2, 3, 4, 5])
+    >>> _ = hash(l)
+    >>> l.append(6)
+    Traceback (most recent call last):
+    ...
+    ValueError: hashed 'hlist' object is not mutable
+    >>> unhash(l)
+    >>> l.append(6)
+    """
+
+    # apidoc stop
+    def __add__(self, other):
+        return self.__class__(list.__add__(self, other))
+
+    def __delitem__(self, item):
+        self.__mutable__()
+        list.__delitem__(self, item)
+
+    def __delslice__(self, *l, **d):
+        self.__mutable__()
+        list.__delslice__(self, *l, **d)
+
+    def __getslice__(self, first, last):
+        return self.__class__(list.__getslice__(self, first, last))
+
+    def __getitem__(self, item):
+        ret = list.__getitem__(self, item)
+        if ret.__class__ is list:
+            return self.__class__(ret)
+        return ret
+
+    def __hash__(self):
+        return hash(tuple(self))
+
+    def __iadd__(self, other):
+        return self.__class__(list.__iadd__(self, other))
+
+    def __imul__(self, n):
+        return self.__class__(list.__imul__(self, n))
+
+    def __mul__(self, n):
+        return self.__class__(list.__mul__(self, n))
+
+    def __repr__(self):
+        """
+        >>> repr(hlist(range(3)))
+        'hlist([0, 1, 2])'
+        """
+        return "%s(%s)" % (self.__class__.__name__, list.__repr__(self))
+
+    def __rmul__(self, n):
+        return self._class__(list.__rmul__(self, n))
+
+    def __setitem__(self, index, item):
+        self.__mutable__()
+        list.__setitem__(self, index, item)
+
+    def __setslice__(self, first, last, item):
+        self.__mutable__()
+        list.__setslice__(self, first, last, item)
+
+    def append(self, item):
+        self.__mutable__()
+        list.append(self, item)
+
+    def extend(self, iterable):
+        self.__mutable__()
+        list.extend(self, iterable)
+
+    def insert(self, index, item):
+        self.__mutable__()
+        list.insert(self, index, item)
+
+    def pop(self, index=-1):
+        self.__mutable__()
+        return list.pop(self, index)
+
+    def remove(self, item):
+        self.__mutable__()
+        list.remove(self, item)
+
+    def reverse(self):
+        self.__mutable__()
+        list.reverse(self)
+
+    def sort(self, cmp=None, key=None, reverse=False):
+        self.__mutable__()
+        list.sort(self, cmp, key, reverse)
+
+
+hlist = hashable(hlist)
+
+
+class hdict(dict):
+    """Hashable dictionnaries. They support all standard methods from
+    `dict`.
+    >>> l = hlist(range(5))
+    >>> d = hdict([(l, 0)])
+    >>> d
+    hdict({hlist([0, 1, 2, 3, 4]): 0})
+    >>> l in d
+    True
+    >>> [0, 1, 2, 3, 4] in d
+    Traceback (most recent call last):
+    ...
+    TypeError: ...
+    >>> hlist([0, 1, 2, 3, 4]) in d
+    True
+    >>> d[hlist([0, 1, 2, 3, 4])]
+    0
+    >>> l.append(5)
+    Traceback (most recent call last):
+    ...
+    ValueError: hashed 'hlist' object is not mutable
+    >>> _ = hash(d)
+    >>> d.pop(l)  # any mutation would produce the same error
+    Traceback (most recent call last):
+    ...
+    ValueError: hashed 'hdict' object is not mutable
+    >>> unhash(d)
+    >>> d.pop(l)
+    0
+    """
+
+    # apidoc stop
+    def __delitem__(self, key):
+        self.__mutable__()
+        dict.__delitem__(self, key)
+
+    def __hash__(self):
+        """
+        >>> _ = hash(hdict(a=1, b=2))
+        """
+        # 252756382 = hash("snakes.hashables.hlist")
+        return reduce(xor, (hash(i) for i in self.items()), 252756382)
+
+    def __repr__(self):
+        """
+        >>> repr(hdict(a=1))
+        "hdict({'a': 1})"
+        """
+        return "%s(%s)" % (self.__class__.__name__, dict.__repr__(self))
+
+    def __setitem__(self, key, item):
+        self.__mutable__()
+        dict.__setitem__(self, key, item)
+
+    def clear(self):
+        self.__mutable__()
+        dict.clear(self)
+
+    def copy(self):
+        return self.__class__(dict.copy(self))
+
+    @classmethod
+    def fromkeys(_class, *args):
+        return _class(dict.fromkeys(*args))
+
+    def pop(self, *args):
+        self.__mutable__()
+        return dict.pop(self, *args)
+
+    def popitem(self):
+        self.__mutable__()
+        return dict.popitem(self)
+
+    def setdefault(self, key, item=None):
+        self.__mutable__()
+        return dict.setdefault(self, key, item)
+
+    def update(self, other, **more):
+        self.__mutable__()
+        return dict.update(self, other, **more)
+
+
+hdict = hashable(hdict)
+
+
+class hset(set):
+    """Hashable sets. They support all standard methods from `set`.
+    >>> s = hset()
+    >>> l = hlist(range(5))
+    >>> s.add(l)
+    >>> s
+    hset([hlist([0, 1, 2, 3, 4])])
+    >>> l in s
+    True
+    >>> [0, 1, 2, 3, 4] in s
+    Traceback (most recent call last):
+    ...
+    TypeError: ...
+    >>> hlist([0, 1, 2, 3, 4]) in s
+    True
+    >>> l.append(5)
+    Traceback (most recent call last):
+    ...
+    ValueError: hashed 'hlist' object is not mutable
+    >>> _ = hash(s)
+    >>> s.discard(l)  # any mutation would produce the same error
+    Traceback (most recent call last):
+    ...
+    ValueError: hashed 'hset' object is not mutable
+    >>> unhash(s)
+    >>> s.discard(l)
+    """
+
+    # apidoc stop
+    def __and__(self, other):
+        return self.__class__(set.__and__(self, other))
+
+    def __hash__(self):
+        """
+        >>> _ = hash(hset([1, 2, 3]))
+        >>> _ = hash(hset(range(5)) - set([0, 4]))
+        """
+        # 196496309 = hash("snakes.hashables.hset")
+        return reduce(xor, (hash(x) for x in self), 196496309)
+
+    def __iand__(self, other):
+        return self.__class__(set.__iand__(self, other))
+
+    def __ior__(self, other):
+        return self.__class__(set.__ior__(self, other))
+
+    def __isub__(self, other):
+        return self.__class__(set.__isub__(self, other))
+
+    def __ixor__(self, other):
+        return self.__class__(set.__ixor__(self, other))
+
+    def __or__(self, other):
+        return self.__class__(set.__or__(self, other))
+
+    def __rand__(self, other):
+        return self.__class__(set.__rand__(self, other))
+
+    def __repr__(self):
+        """
+        >>> repr(hset([1]))
+        'hset([1])'
+        """
+        return "%s([%s])" % (self.__class__.__name__,
+                             set.__repr__(self)[6:-2])
+
+    def __ror__(self, other):
+        return self.__class__(set.__ror__(self, other))
+
+    def __rsub__(self, other):
+        return self.__class__(set.__rsub__(self, other))
+
+    def __rxor__(self, other):
+        return self.__class__(set.__rxor__(self, other))
+
+    def __str__(self):
+        return self.__class__.__name__ + \
+            "(" + set.__str__(self).split("(", 1)[1]
+
+    def __sub__(self, other):
+        return self.__class__(set.__sub__(self, other))
+
+    def __xor__(self, other):
+        return self.__class__(set.__xor__(self, other))
+
+    def add(self, item):
+        self.__mutable__()
+        set.add(self, item)
+
+    def clear(self):
+        self.__mutable__()
+        set.clear(self)
+
+    def copy(self):
+        return self.__class__(set.copy(self))
+
+    def difference(self, other):
+        return self.__class__(set.difference(self, other))
+
+    def difference_update(self, other):
+        self.__mutable__()
+        set.difference_update(self, other)
+
+    def discard(self, item):
+        self.__mutable__()
+        set.discard(self, item)
+
+    def intersection(self, other):
+        return self._class__(set.intersection(self, other))
+
+    def intersection_update(self, other):
+        self.__mutable__()
+        set.intersection_update(self, other)
+
+    def pop(self):
+        self.__mutable__()
+        return set.pop(self)
+
+    def remove(self, item):
+        self.__mutable__()
+        set.remove(self, item)
+
+    def symmetric_difference(self, other):
+        self.__mutable__()
+        set.symmetric_difference(self, other)
+
+    def symmetric_difference_update(self, other):
+        self.__mutable__()
+        set.symmetric_difference_update(self, other)
+
+    def union(self, other):
+        return self.__class__(set.union(self, other))
+
+    def update(self, other):
+        self.__mutable__()
+        set.update(self, other)
+
+
+hset = hashable(hset)
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/idMethods.py` & `nope_py-1.7.9/nope/helpers/idMethods.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from uuid import uuid4
-
-from .stringMethods import replaceAll
-
-
-def generateId(use_as_var: bool = False, pre_string: str = None) -> str:
-    """ Helper to generate an id.
-        if "use_as_var" is provided in the Options => the id is converted to an id
-        if "pre_string" is provided, this string will be added in front of the id.
-
-
-    Args:
-        options (dotted_dict, optional):    The options. May cotains "use_as_var" and "pre_string".
-                                            Defaults to dotted_dict({}).
-
-    Returns:
-        str: The id.
-    """
-
-    _id = str(uuid4())
-    if use_as_var:
-        _id = replaceAll(_id, '-', '')
-        pre_string = pre_string if pre_string else '_'
-    if pre_string:
-        _id = pre_string + _id
-    return _id
+from uuid import uuid4
+
+from .stringMethods import replaceAll
+
+
+def generateId(use_as_var: bool = False, pre_string: str = None) -> str:
+    """ Helper to generate an id.
+        if "use_as_var" is provided in the Options => the id is converted to an id
+        if "pre_string" is provided, this string will be added in front of the id.
+
+
+    Args:
+        options (dotted_dict, optional):    The options. May cotains "use_as_var" and "pre_string".
+                                            Defaults to dotted_dict({}).
+
+    Returns:
+        str: The id.
+    """
+
+    _id = str(uuid4())
+    if use_as_var:
+        _id = replaceAll(_id, '-', '')
+        pre_string = pre_string if pre_string else '_'
+    if pre_string:
+        _id = pre_string + _id
+    return _id
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/jsonMethods.py` & `nope_py-1.7.9/nope/helpers/jsonMethods.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from dataclasses import is_dataclass, asdict
-from inspect import isfunction, getsource
-from json import dumps as _dumps, loads as _loads, JSONEncoder, JSONDecoder
-from typing import Any
-
-FUNC_BEGIN = "__FUNCTION_BEGIN__"
-FUNC_END = "__FUNCTION_END__"
-
-
-class EnhancedJSONEncoder(JSONEncoder):
-    def default(self, o):
-        if is_dataclass(o):
-            return asdict(o)
-        if isfunction(o):
-            code = getsource(o)
-
-            if code.startswith("def"):
-
-                code = code.replace("\n", "\\n")
-
-                return f"{FUNC_BEGIN}{code}{FUNC_END}{o.__name__}"
-
-            elif "lambda" in code:
-                idx = code.index("lambda")
-                return f"{FUNC_BEGIN}{code[idx:]}{FUNC_END}"
-        return super().default(o)
-
-
-class SimpleJSONEncoder(JSONEncoder):
-    def default(self, o):
-        if is_dataclass(o):
-            return asdict(o)
-        elif isfunction(o):
-            return None
-        return super().default(o)
-
-
-class EnhancedJSONDecoder(JSONDecoder):
-    def __init__(self, *args, **kwargs):
-        JSONDecoder.__init__(
-            self,
-            object_hook=self.object_hook,
-            *args,
-            **kwargs)
-
-    def object_hook(self, o):
-        if isinstance(o, dict):
-
-            to_adapt = dict()
-
-            for key, value in o.items():
-                if isinstance(value, str):
-                    if value.startswith(FUNC_BEGIN) and FUNC_END in value:
-                        code = value[len(FUNC_BEGIN):value.index(FUNC_END)]
-                        if code.startswith("def"):
-                            exec(code)
-                            name = value[value.index(
-                                FUNC_END) + len(FUNC_END):]
-                            o[key] = eval(name)
-                        else:
-                            o[key] = eval(code)
-                        continue
-        return o
-
-
-def dumps(o: Any, indent: int = 4, parse_functions=True, **kwargs) -> str:
-    """ Helper function, to dump data to JSON and serialize
-        python functions.
-
-
-    Args:
-        o (Any): The Object to start
-        indent (int, optional): The indent. Defaults to 4.
-        parse_functions (bool, optional): Flag to enable storing Python Functions. Defaults to True.
-
-    Returns:
-        str: The parsed object.
-    """
-    if parse_functions:
-        kwargs.pop("cls", None)
-        return _dumps(o, indent=indent, cls=EnhancedJSONEncoder, **kwargs)
-    return _dumps(o, indent=indent, cls=SimpleJSONEncoder, **kwargs)
-
-
-def loads(s: str, parse_functions=True, **kwargs) -> Any:
-    if parse_functions:
-        kwargs.pop("cls", None)
-        return _loads(s, cls=EnhancedJSONDecoder, **kwargs)
-    return _loads(s, **kwargs)
+from dataclasses import is_dataclass, asdict
+from inspect import isfunction, getsource
+from json import dumps as _dumps, loads as _loads, JSONEncoder, JSONDecoder
+from typing import Any
+
+FUNC_BEGIN = "__FUNCTION_BEGIN__"
+FUNC_END = "__FUNCTION_END__"
+
+
+class EnhancedJSONEncoder(JSONEncoder):
+    def default(self, o):
+        if is_dataclass(o):
+            return asdict(o)
+        if isfunction(o):
+            code = getsource(o)
+
+            if code.startswith("def"):
+
+                code = code.replace("\n", "\\n")
+
+                return f"{FUNC_BEGIN}{code}{FUNC_END}{o.__name__}"
+
+            elif "lambda" in code:
+                idx = code.index("lambda")
+                return f"{FUNC_BEGIN}{code[idx:]}{FUNC_END}"
+        return super().default(o)
+
+
+class SimpleJSONEncoder(JSONEncoder):
+    def default(self, o):
+        if is_dataclass(o):
+            return asdict(o)
+        elif isfunction(o):
+            return None
+        return super().default(o)
+
+
+class EnhancedJSONDecoder(JSONDecoder):
+    def __init__(self, *args, **kwargs):
+        JSONDecoder.__init__(
+            self,
+            object_hook=self.object_hook,
+            *args,
+            **kwargs)
+
+    def object_hook(self, o):
+        if isinstance(o, dict):
+
+            to_adapt = dict()
+
+            for key, value in o.items():
+                if isinstance(value, str):
+                    if value.startswith(FUNC_BEGIN) and FUNC_END in value:
+                        code = value[len(FUNC_BEGIN):value.index(FUNC_END)]
+                        if code.startswith("def"):
+                            exec(code)
+                            name = value[value.index(
+                                FUNC_END) + len(FUNC_END):]
+                            o[key] = eval(name)
+                        else:
+                            o[key] = eval(code)
+                        continue
+        return o
+
+
+def dumps(o: Any, indent: int = 4, parse_functions=True, **kwargs) -> str:
+    """ Helper function, to dump data to JSON and serialize
+        python functions.
+
+
+    Args:
+        o (Any): The Object to start
+        indent (int, optional): The indent. Defaults to 4.
+        parse_functions (bool, optional): Flag to enable storing Python Functions. Defaults to True.
+
+    Returns:
+        str: The parsed object.
+    """
+    if parse_functions:
+        kwargs.pop("cls", None)
+        return _dumps(o, indent=indent, cls=EnhancedJSONEncoder, **kwargs)
+    return _dumps(o, indent=indent, cls=SimpleJSONEncoder, **kwargs)
+
+
+def loads(s: str, parse_functions=True, **kwargs) -> Any:
+    if parse_functions:
+        kwargs.pop("cls", None)
+        return _loads(s, cls=EnhancedJSONDecoder, **kwargs)
+    return _loads(s, **kwargs)
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/listMethods.py` & `nope_py-1.7.9/nope/helpers/listMethods.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-
-from collections.abc import Iterable
-from functools import reduce
-
-from .dottedDict import DottedDict
-from .objectMethods import rgetattr
-
-
-def extractListElements(_list, _path: str):
-    def extract(_prop):
-        ret = rgetattr(_prop, _path)
-        if ret:
-            return ret
-
-    return map(extract, _list)
-
-
-def getElement(_list, operand, _path=''):
-    for element in _list:
-        if operand == rgetattr(element, _path):
-            return element
-    return None
-
-
-def avgOfArray(_list, _path: str, defaultValue=0):
-    if len(_list) == 0:
-        return defaultValue
-
-    values = map(lambda item: rgetattr(item, _path, defaultValue), _list)
-    value = reduce(lambda prev, curr: prev + curr, values)
-    return value / len(_list)
-
-
-def minOfArray(_list, _path, defaultValue=float("inf")):
-    if len(_list) == 0:
-        return DottedDict({'min': defaultValue, 'index': None})
-
-    values = list(map(lambda item: rgetattr(item, _path, defaultValue), _list))
-    minValue = min(values)
-    return DottedDict({'min': minValue, 'index': values.index(minValue)})
-
-
-def maxOfArray(_list, _path, defaultValue=-float("inf")):
-    if len(_list) == 0:
-        return DottedDict({'max': defaultValue, 'index': None})
-
-    values = list(map(lambda item: rgetattr(item, _path, defaultValue), _list))
-    maxValue = max(values)
-    return DottedDict({'max': maxValue, 'index': values.index(maxValue)})
-
-
-def isIterable(obj):
-    """ Helper to test if an objec is iterable.
-    """
-
-    if isinstance(obj, str):
-        return False
-    return isinstance(obj, Iterable)
-
-
-def isList(obj) -> bool:
-    """ Helper to check if the item is a list.
-
-    Args:
-        obj (any): The item to check
-
-    Returns:
-        bool: Result. If `True` => List
-    """
-    return type(obj) in (list,)
-
-
-def flattenDeep(l: list) -> list:
-    """ Helper to flatten a list of elements:
-
-    Example:
-        >>> l = [1, [2,3,[4,5]]]
-        >>> flatten_deep(l)
-        [1,2,3,4,5]
-
-    Args:
-        l (list): A nested list.
-
-    Returns:
-        list: A flattend list. (1 Dimension)
-    """
-    if len(l) == 0:
-        return l
-    if isinstance(l[0], list):
-        return flattenDeep(l[0]) + flattenDeep(l[1:])
-    return l[:1] + flattenDeep(l[1:])
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+
+from collections.abc import Iterable
+from functools import reduce
+
+from .dottedDict import DottedDict
+from .objectMethods import rgetattr
+
+
+def extractListElements(_list, _path: str):
+    def extract(_prop):
+        ret = rgetattr(_prop, _path)
+        if ret:
+            return ret
+
+    return map(extract, _list)
+
+
+def getElement(_list, operand, _path=''):
+    for element in _list:
+        if operand == rgetattr(element, _path):
+            return element
+    return None
+
+
+def avgOfArray(_list, _path: str, defaultValue=0):
+    if len(_list) == 0:
+        return defaultValue
+
+    values = map(lambda item: rgetattr(item, _path, defaultValue), _list)
+    value = reduce(lambda prev, curr: prev + curr, values)
+    return value / len(_list)
+
+
+def minOfArray(_list, _path, defaultValue=float("inf")):
+    if len(_list) == 0:
+        return DottedDict({'min': defaultValue, 'index': None})
+
+    values = list(map(lambda item: rgetattr(item, _path, defaultValue), _list))
+    minValue = min(values)
+    return DottedDict({'min': minValue, 'index': values.index(minValue)})
+
+
+def maxOfArray(_list, _path, defaultValue=-float("inf")):
+    if len(_list) == 0:
+        return DottedDict({'max': defaultValue, 'index': None})
+
+    values = list(map(lambda item: rgetattr(item, _path, defaultValue), _list))
+    maxValue = max(values)
+    return DottedDict({'max': maxValue, 'index': values.index(maxValue)})
+
+
+def isIterable(obj):
+    """ Helper to test if an objec is iterable.
+    """
+
+    if isinstance(obj, str):
+        return False
+    return isinstance(obj, Iterable)
+
+
+def isList(obj) -> bool:
+    """ Helper to check if the item is a list.
+
+    Args:
+        obj (any): The item to check
+
+    Returns:
+        bool: Result. If `True` => List
+    """
+    return type(obj) in (list,)
+
+
+def flattenDeep(l: list) -> list:
+    """ Helper to flatten a list of elements:
+
+    Example:
+        >>> l = [1, [2,3,[4,5]]]
+        >>> flatten_deep(l)
+        [1,2,3,4,5]
+
+    Args:
+        l (list): A nested list.
+
+    Returns:
+        list: A flattend list. (1 Dimension)
+    """
+    if len(l) == 0:
+        return l
+    if isinstance(l[0], list):
+        return flattenDeep(l[0]) + flattenDeep(l[1:])
+    return l[:1] + flattenDeep(l[1:])
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/objectMethods.py` & `nope_py-1.7.9/nope/helpers/objectMethods.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from copy import deepcopy
-
-from .dottedDict import DottedDict, ensureDottedAccess
-from .path import (MULTI_LEVEL_WILDCARD, SPLITCHAR, containsWildcards,
-                   getLeastCommonPathSegment)
-from .pathMatchingMethods import comparePatternAndPath
-
-SENTINEL_1 = object()
-SENTINEL_2 = object()
-
-
-def rgetattr(data, path, default=SENTINEL_1, splitchar=SPLITCHAR):
-    """ Helper to recursively get an value.
-
-    Args:
-        data (any): The data to extract the value from
-        path (str): The path to extract the data from.
-        default (any, optional): The Default value which will be return if no value has been found. If not provided None is returned
-        splitchar (str, optional): _description_. Defaults to SPLITCHAR.
-
-    Returns:
-        any: The found data.
-    """
-    obj = data
-    if len(path) > 0:
-        if splitchar in path:
-            for attr in path.split(splitchar):
-                if type(obj) in (dict, DottedDict):
-                    obj = obj.get(attr)
-                else:
-                    try:
-                        obj = obj[attr]
-                    except BaseException:
-                        if default == SENTINEL_1:
-                            return None
-                        return default
-        else:
-            try:
-                data = obj[path]
-                return data
-            except KeyError:
-                if default == SENTINEL_1:
-                    return None
-                return default
-
-    return obj
-
-
-def rqueryAttr(data, query):
-    if not containsWildcards(query):
-        extractedData = rgetattr(data, query, SENTINEL_2)
-        if extractedData == SENTINEL_2:
-            return []
-
-        return [
-            DottedDict({
-                'path': query,
-                'data': extractedData
-            })
-        ]
-
-    ret = []
-    multi_level = MULTI_LEVEL_WILDCARD in query
-    # Determine the max depth
-    max_depth = None if multi_level else len(query.split(SPLITCHAR))
-
-    # get the flatten object
-    _dict = flattenObject(
-        data,
-        max_depth=max_depth,
-        onlyPathToBaseValue=False
-    )
-
-    # Iterate over the items and use our path matcher to extract the matching
-    # items.
-    for iter_item in _dict.items():
-        path = iter_item[0]
-        value = iter_item[1]
-        r = comparePatternAndPath(query, path)
-
-        if r.affectedOnSameLevel or (multi_level and r.affectedByChild):
-            ret.append(
-                DottedDict({
-                    'path': path,
-                    'data': value
-                })
-            )
-
-    return ret
-
-
-def convertData(data, props):
-    """ Helper to query data from an object.
-
-        props is defined as followed:
-        ```typescript
-        props: {
-            key: string;
-            query: string;
-        }[]
-        ```
-
-        Example 1:
-
-        data = { "deep": { "nested": "test" } }
-        result = convertData(data, [
-            {
-                "key": "result",
-                "query": "deep/nested",
-            },
-        ])
-
-        ==> result = [{"result": "test"}]
-
-        Example 2:
-
-        data = {
-            "array": [
-            {
-                "data1": 0,
-                "data2": "a",
-            },
-            {
-                "data1": 1,
-                "data2": "a",
-            },
-            ],
-            "not": { "nested": "hello" }
-        }
-
-        result = convertData(data, [
-            {
-                "key": "a",
-                "query": "array/+/data1",
-            },
-            {
-                "key": "b",
-                "query": "array/+/data2",
-            },
-        ])
-
-        ==> result = [{"a": 0, "b": "a"}, {"a": 1, "b": "a"}]
-
-    Args:
-        data (any): The data
-        props (dotted_dict[]): The query to use.
-    """
-
-    ret = DottedDict({})
-
-    commonPattern = getLeastCommonPathSegment(
-        list(
-            map(
-                lambda _item: _item.get("query"),
-                props
-            )
-        )
-    )
-
-    for prop in props:
-        ret[prop.get("key")] = rqueryAttr(data, prop.get("query"))
-
-    helper = DottedDict({})
-
-    for prop in props:
-        items = ret[prop.get("key")]
-
-        for idx, item in enumerate(items):
-
-            if isinstance(commonPattern, str):
-                result = comparePatternAndPath(commonPattern, item["path"])
-                if result.pathToExtractData:
-                    if not (result.pathToExtractData in helper):
-                        helper[result.pathToExtractData] = DottedDict()
-                    helper[result.pathToExtractData][prop.get(
-                        "key")] = item.data
-            else:
-                if idx not in helper:
-                    helper[idx] = DottedDict()
-
-                helper[idx][prop.get("key")] = item.data
-
-    return list(helper.values())
-
-
-def _set(obj, accessor: str, value):
-    try:
-        obj[accessor] = value
-    except BaseException as E:
-        try:
-            setattr(obj, accessor, value)
-        except BaseException as E:
-            raise E
-
-
-def _get(obj, accessor, return_none=False):
-    try:
-        return obj[accessor]
-    except BaseException as E:
-        try:
-            return getattr(obj, accessor)
-        except BaseException as E:
-            if return_none:
-                return None
-            raise E
-
-
-def rsetattr(data, path: str, value, splitchar: str = SPLITCHAR):
-    """ unction to Set recursely a Attribute of an Object
-
-    Args:
-        data (any):  The Object, where the data should be stored
-        path (str): The Path of the Attribute. All are seprated by a the splitchar. (Defaults to'.' => For Instance 'a/b/0/a/c')
-        value (any): The Value which should be Stored in the Attribute.
-        splitchar (str, optional): The Splitchar to use. Defaults to "/". Defaults to SPLITCHAR.
-    """
-
-    obj = data
-
-    ptrs = path.split(splitchar)
-
-    for idx, attr in enumerate(ptrs[0:-1]):
-        # Adapt the Object by going through a loop
-
-        accessor = int(attr) if isInt(attr) else attr
-
-        sub = _get(obj, accessor, return_none=True)
-
-        if isinstance(obj, list):
-            length = len(obj)
-            while length <= accessor:
-                obj.append(None)
-                length = len(obj)
-
-        if sub is None:
-            # _obj is an Array and it doesnt contain the index
-            # Extract the Next Element:
-            nextAccessor = ptrs[idx + 1]
-
-            nextIsInt = isInt(nextAccessor)
-
-            if nextIsInt:
-                _set(obj, accessor, [None] * (int(nextAccessor) + 1))
-            else:
-                _set(obj, accessor, DottedDict({}))
-
-            sub = _get(obj, accessor)
-
-        obj = sub
-
-    try:
-        obj[ptrs[len(ptrs) - 1]] = value
-    except BaseException as E:
-        try:
-            sub = setattr(obj, ptrs[len(ptrs) - 1], value)
-        except BaseException as E:
-            raise E
-
-
-def isInt(value) -> bool:
-    """ Checks whether the Value is an Integer
-
-    Args:
-        value: Value to be checked
-    """
-    if isinstance(value, int):
-        return True
-
-    try:
-        int(value)
-        return True
-    except BaseException:
-        return False
-
-
-def isFloat(value) -> bool:
-    """ Checks whether the Value is a Float
-
-    Args:
-        value: Value to be checked
-    """
-    if isinstance(value, float):
-        return True
-
-    try:
-        float(value)
-        return True
-    except BaseException:
-        return False
-
-
-def isNumber(value) -> bool:
-    return isFloat(value) or isInt(value)
-
-
-def objectToDict(obj):
-    """ Function Converts a Object to a dict.
-
-    Args:
-        obj: The Object which should be converted.
-    """
-
-    ret = dict
-    # Iterate through all properties of the Object
-    for prop in obj:
-        if not callable(obj):
-            ret[prop] = obj[prop]
-
-    return ret
-
-
-def isDictLike(obj) -> bool:
-    """ Check if the object is dict-like.
-
-    Args:
-        obj (any): The object to check
-
-    Returns:
-        bool:  Whether `obj` has dict-like properties.
-
-    Examples:
-        >>> isDictLike({1: 2})
-        True
-        >>> isDictLike([1, 2, 3])
-        False
-        >>> isDictLike(dict)
-        False
-        >>> isDictLike(dict())
-        True
-    """
-    attributes_to_check = ("__getitem__")
-
-    for attr in attributes_to_check:
-        if not hasattr(obj, attr):
-            return False
-
-    # Prevent returning Classes:
-    return not isinstance(obj, type)
-
-
-def allowsSubscripton(obj):
-    return hasattr(obj, "__getitem__")
-
-
-def flattenObject(data, prefix="", splitchar=SPLITCHAR,
-                  onlyPathToBaseValue=False, max_depth=None):
-    ret = DottedDict()
-
-    # Check if we are ae to access the items using an subscription.
-    if allowsSubscripton(data):
-        def callback(path, data, *args):
-            ret[path] = data
-
-        recursiveForEach(
-            data,
-            callback,
-            prefix,
-            splitchar,
-            onlyPathToBaseValue,
-            max_depth
-        )
-
-    return ret
-
-
-def deflattenObject(flattenObject, options=None):
-    _options = ensureDottedAccess({'prefix': '', 'splitchar': SPLITCHAR})
-    _options.update(ensureDottedAccess(options))
-
-    ret = ensureDottedAccess({})
-
-    for key, val in flattenObject.items():
-        if _options.prefix != '':
-            key = key[len(_options.prefix):]
-        rsetattr(ret, key, val, _options.splitchar)
-
-    return ret
-
-
-def getKeys(obj):
-    """ Helper, to get keys of an array, dict etc.
-
-    Args:
-        obj: The considered Object.
-
-    Returns:
-        list: List of Keys
-    """
-    keys = list()
-    t_obj = type(obj)
-    if not (t_obj is str) and not (callable(obj)):
-        if t_obj in (list, set):
-            # For list, we will use the index
-            keys = range(0, len(obj))
-        elif hasattr(obj, "keys"):
-            # We are working with a dict.
-            keys = list(obj.keys())
-        else:
-            try:
-                # For all other items, we will use the vars as key.
-                keys = list(vars(obj))
-            except BaseException:
-                pass
-
-    return keys
-
-
-def deepAssign(target, source):
-    """ Deeply assigns the items given in the dict, whereas the
-        keys of the source will be used as path, its value as value
-        to assign.
-
-    Args:
-        target (any): original object.
-        source (dict | dict-like): Todo
-
-    Returns:
-        any: the manipulated target
-    """
-    flattend = flattenObject(source)
-    for iter_item in flattend.entries():
-        path = iter_item[0]
-        value = iter_item[1]
-        rsetattr(target, path, value)
-    return target
-
-
-def recursiveForEach(obj, callback=None, prefix="", splitchar=SPLITCHAR, callOnlyOnBaseValues=True,
-                     max_depth=None, parent='', level=0):
-    """ Function, that will iterate over an object.
-
-    Args:
-        obj: The Object to iterate
-        prefix (_type_): A prefix for the Path.
-        callback (callable, optional): Callback, that will be called.. Defaults to None.
-        splitchar (_type_, optional): The Splitchar to use, to generate the path. Defaults to SPLITCHAR.
-        callOnlyOnBaseValues (bool, optional): A Flag, to call the Function only on Values. Defaults to True.
-        max_depth (_type_, optional): Determine the max Depth, after which the Iteration will be stopped.. Defaults to None.
-        parent (str, optional): For Recursive call only. Defaults to ''.
-        level (int, optional): For Recursive call only. Defaults to 0.
-    """
-    if isInt(max_depth) and level > max_depth:
-        # Break the Loop
-        return
-
-    # No try to extrac the Keys.
-    keys = getKeys(obj)
-
-    called = False
-    if not callOnlyOnBaseValues and callable(callback):
-        callback(prefix, obj, parent, level)
-        called = True
-
-    # If there exits some keys:
-    if len(keys) > 0:
-        # We will iterate over the and
-        for key in keys:
-            # Define the variable, containing the path
-            path = str(key) if '' == prefix else prefix + splitchar + str(key)
-
-            if obj[key] is not None:
-                if hasattr(obj[key], "to_json") and callable(obj[key].to_json):
-                    data = obj[key].to_json()
-                    recursiveForEach(
-                        data,
-                        callback,
-                        path,
-                        splitchar,
-                        callOnlyOnBaseValues,
-                        max_depth,
-                        prefix,
-                        level + 1
-                    )
-
-                else:
-
-                    recursiveForEach(
-                        obj[key],
-                        callback,
-                        path,
-                        splitchar,
-                        callOnlyOnBaseValues,
-                        max_depth,
-                        prefix,
-                        level + 1
-                    )
-    elif not called:
-        callback(prefix, obj, prefix, level)
-
-
-def keepProperties(obj, properties):
-    if allowsSubscripton(obj):
-        ret = DottedDict({})
-        default_obj = DottedDict({'error': True})
-
-        for key in getKeys(obj):
-            value = rgetattr(obj, key, default_obj)
-            valueToAssign = value
-            if value != default_obj:
-                valueToAssign = copy(value)
-            else:
-                valueToAssign = properties[key]()
-            rsetattr(ret, key, valueToAssign)
-
-        return ret
-    raise Exception('Function can only create Objects')
-
-
-WARNED = False
-
-
-def copy(obj):
-    """ A Helper, which can be used to receive a copy.
-
-    Args:
-        obj (any): The Object to copy
-
-    Returns:
-        bool, any: A flag, to show whether it succeeded or failed; the copy (or if failed the object) itself.
-    """
-    try:
-        return deepcopy(obj)
-    except BaseException:
-        try:
-            return obj.copy()
-        except BaseException:
-            global WARNED
-            if not WARNED:
-                WARNED = True
-                print("Failed to create a copy using orignal value.")
-            return obj
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from copy import deepcopy
+
+from .dottedDict import DottedDict, ensureDottedAccess
+from .path import (MULTI_LEVEL_WILDCARD, SPLITCHAR, containsWildcards,
+                   getLeastCommonPathSegment)
+from .pathMatchingMethods import comparePatternAndPath
+
+SENTINEL_1 = object()
+SENTINEL_2 = object()
+
+
+def rgetattr(data, path, default=SENTINEL_1, splitchar=SPLITCHAR):
+    """ Helper to recursively get an value.
+
+    Args:
+        data (any): The data to extract the value from
+        path (str): The path to extract the data from.
+        default (any, optional): The Default value which will be return if no value has been found. If not provided None is returned
+        splitchar (str, optional): _description_. Defaults to SPLITCHAR.
+
+    Returns:
+        any: The found data.
+    """
+    obj = data
+    if len(path) > 0:
+        if splitchar in path:
+            for attr in path.split(splitchar):
+                if type(obj) in (dict, DottedDict):
+                    obj = obj.get(attr)
+                else:
+                    try:
+                        obj = obj[attr]
+                    except BaseException:
+                        if default == SENTINEL_1:
+                            return None
+                        return default
+        else:
+            try:
+                data = obj[path]
+                return data
+            except KeyError:
+                if default == SENTINEL_1:
+                    return None
+                return default
+
+    return obj
+
+
+def rqueryAttr(data, query):
+    if not containsWildcards(query):
+        extractedData = rgetattr(data, query, SENTINEL_2)
+        if extractedData == SENTINEL_2:
+            return []
+
+        return [
+            DottedDict({
+                'path': query,
+                'data': extractedData
+            })
+        ]
+
+    ret = []
+    multi_level = MULTI_LEVEL_WILDCARD in query
+    # Determine the max depth
+    max_depth = None if multi_level else len(query.split(SPLITCHAR))
+
+    # get the flatten object
+    _dict = flattenObject(
+        data,
+        max_depth=max_depth,
+        onlyPathToBaseValue=False
+    )
+
+    # Iterate over the items and use our path matcher to extract the matching
+    # items.
+    for iter_item in _dict.items():
+        path = iter_item[0]
+        value = iter_item[1]
+        r = comparePatternAndPath(query, path)
+
+        if r.affectedOnSameLevel or (multi_level and r.affectedByChild):
+            ret.append(
+                DottedDict({
+                    'path': path,
+                    'data': value
+                })
+            )
+
+    return ret
+
+
+def convertData(data, props):
+    """ Helper to query data from an object.
+
+        props is defined as followed:
+        ```typescript
+        props: {
+            key: string;
+            query: string;
+        }[]
+        ```
+
+        Example 1:
+
+        data = { "deep": { "nested": "test" } }
+        result = convertData(data, [
+            {
+                "key": "result",
+                "query": "deep/nested",
+            },
+        ])
+
+        ==> result = [{"result": "test"}]
+
+        Example 2:
+
+        data = {
+            "array": [
+            {
+                "data1": 0,
+                "data2": "a",
+            },
+            {
+                "data1": 1,
+                "data2": "a",
+            },
+            ],
+            "not": { "nested": "hello" }
+        }
+
+        result = convertData(data, [
+            {
+                "key": "a",
+                "query": "array/+/data1",
+            },
+            {
+                "key": "b",
+                "query": "array/+/data2",
+            },
+        ])
+
+        ==> result = [{"a": 0, "b": "a"}, {"a": 1, "b": "a"}]
+
+    Args:
+        data (any): The data
+        props (dotted_dict[]): The query to use.
+    """
+
+    ret = DottedDict({})
+
+    commonPattern = getLeastCommonPathSegment(
+        list(
+            map(
+                lambda _item: _item.get("query"),
+                props
+            )
+        )
+    )
+
+    for prop in props:
+        ret[prop.get("key")] = rqueryAttr(data, prop.get("query"))
+
+    helper = DottedDict({})
+
+    for prop in props:
+        items = ret[prop.get("key")]
+
+        for idx, item in enumerate(items):
+
+            if isinstance(commonPattern, str):
+                result = comparePatternAndPath(commonPattern, item["path"])
+                if result.pathToExtractData:
+                    if not (result.pathToExtractData in helper):
+                        helper[result.pathToExtractData] = DottedDict()
+                    helper[result.pathToExtractData][prop.get(
+                        "key")] = item.data
+            else:
+                if idx not in helper:
+                    helper[idx] = DottedDict()
+
+                helper[idx][prop.get("key")] = item.data
+
+    return list(helper.values())
+
+
+def _set(obj, accessor: str, value):
+    try:
+        obj[accessor] = value
+    except BaseException as E:
+        try:
+            setattr(obj, accessor, value)
+        except BaseException as E:
+            raise E
+
+
+def _get(obj, accessor, return_none=False):
+    try:
+        return obj[accessor]
+    except BaseException as E:
+        try:
+            return getattr(obj, accessor)
+        except BaseException as E:
+            if return_none:
+                return None
+            raise E
+
+
+def rsetattr(data, path: str, value, splitchar: str = SPLITCHAR):
+    """ unction to Set recursely a Attribute of an Object
+
+    Args:
+        data (any):  The Object, where the data should be stored
+        path (str): The Path of the Attribute. All are seprated by a the splitchar. (Defaults to'.' => For Instance 'a/b/0/a/c')
+        value (any): The Value which should be Stored in the Attribute.
+        splitchar (str, optional): The Splitchar to use. Defaults to "/". Defaults to SPLITCHAR.
+    """
+
+    obj = data
+
+    ptrs = path.split(splitchar)
+
+    for idx, attr in enumerate(ptrs[0:-1]):
+        # Adapt the Object by going through a loop
+
+        accessor = int(attr) if isInt(attr) else attr
+
+        sub = _get(obj, accessor, return_none=True)
+
+        if isinstance(obj, list):
+            length = len(obj)
+            while length <= accessor:
+                obj.append(None)
+                length = len(obj)
+
+        if sub is None:
+            # _obj is an Array and it doesnt contain the index
+            # Extract the Next Element:
+            nextAccessor = ptrs[idx + 1]
+
+            nextIsInt = isInt(nextAccessor)
+
+            if nextIsInt:
+                _set(obj, accessor, [None] * (int(nextAccessor) + 1))
+            else:
+                _set(obj, accessor, DottedDict({}))
+
+            sub = _get(obj, accessor)
+
+        obj = sub
+
+    try:
+        obj[ptrs[len(ptrs) - 1]] = value
+    except BaseException as E:
+        try:
+            sub = setattr(obj, ptrs[len(ptrs) - 1], value)
+        except BaseException as E:
+            raise E
+
+
+def isInt(value) -> bool:
+    """ Checks whether the Value is an Integer
+
+    Args:
+        value: Value to be checked
+    """
+    if isinstance(value, int):
+        return True
+
+    try:
+        int(value)
+        return True
+    except BaseException:
+        return False
+
+
+def isFloat(value) -> bool:
+    """ Checks whether the Value is a Float
+
+    Args:
+        value: Value to be checked
+    """
+    if isinstance(value, float):
+        return True
+
+    try:
+        float(value)
+        return True
+    except BaseException:
+        return False
+
+
+def isNumber(value) -> bool:
+    return isFloat(value) or isInt(value)
+
+
+def objectToDict(obj):
+    """ Function Converts a Object to a dict.
+
+    Args:
+        obj: The Object which should be converted.
+    """
+
+    ret = dict
+    # Iterate through all properties of the Object
+    for prop in obj:
+        if not callable(obj):
+            ret[prop] = obj[prop]
+
+    return ret
+
+
+def isDictLike(obj) -> bool:
+    """ Check if the object is dict-like.
+
+    Args:
+        obj (any): The object to check
+
+    Returns:
+        bool:  Whether `obj` has dict-like properties.
+
+    Examples:
+        >>> isDictLike({1: 2})
+        True
+        >>> isDictLike([1, 2, 3])
+        False
+        >>> isDictLike(dict)
+        False
+        >>> isDictLike(dict())
+        True
+    """
+    attributes_to_check = ("__getitem__")
+
+    for attr in attributes_to_check:
+        if not hasattr(obj, attr):
+            return False
+
+    # Prevent returning Classes:
+    return not isinstance(obj, type)
+
+
+def allowsSubscripton(obj):
+    return hasattr(obj, "__getitem__")
+
+
+def flattenObject(data, prefix="", splitchar=SPLITCHAR,
+                  onlyPathToBaseValue=False, max_depth=None):
+    ret = DottedDict()
+
+    # Check if we are ae to access the items using an subscription.
+    if allowsSubscripton(data):
+        def callback(path, data, *args):
+            ret[path] = data
+
+        recursiveForEach(
+            data,
+            callback,
+            prefix,
+            splitchar,
+            onlyPathToBaseValue,
+            max_depth
+        )
+
+    return ret
+
+
+def deflattenObject(flattenObject, options=None):
+    _options = ensureDottedAccess({'prefix': '', 'splitchar': SPLITCHAR})
+    _options.update(ensureDottedAccess(options))
+
+    ret = ensureDottedAccess({})
+
+    for key, val in flattenObject.items():
+        if _options.prefix != '':
+            key = key[len(_options.prefix):]
+        rsetattr(ret, key, val, _options.splitchar)
+
+    return ret
+
+
+def getKeys(obj):
+    """ Helper, to get keys of an array, dict etc.
+
+    Args:
+        obj: The considered Object.
+
+    Returns:
+        list: List of Keys
+    """
+    keys = list()
+    t_obj = type(obj)
+    if not (t_obj is str) and not (callable(obj)):
+        if t_obj in (list, set):
+            # For list, we will use the index
+            keys = range(0, len(obj))
+        elif hasattr(obj, "keys"):
+            # We are working with a dict.
+            keys = list(obj.keys())
+        else:
+            try:
+                # For all other items, we will use the vars as key.
+                keys = list(vars(obj))
+            except BaseException:
+                pass
+
+    return keys
+
+
+def deepAssign(target, source):
+    """ Deeply assigns the items given in the dict, whereas the
+        keys of the source will be used as path, its value as value
+        to assign.
+
+    Args:
+        target (any): original object.
+        source (dict | dict-like): Todo
+
+    Returns:
+        any: the manipulated target
+    """
+    flattend = flattenObject(source)
+    for iter_item in flattend.entries():
+        path = iter_item[0]
+        value = iter_item[1]
+        rsetattr(target, path, value)
+    return target
+
+
+def recursiveForEach(obj, callback=None, prefix="", splitchar=SPLITCHAR, callOnlyOnBaseValues=True,
+                     max_depth=None, parent='', level=0):
+    """ Function, that will iterate over an object.
+
+    Args:
+        obj: The Object to iterate
+        prefix (_type_): A prefix for the Path.
+        callback (callable, optional): Callback, that will be called.. Defaults to None.
+        splitchar (_type_, optional): The Splitchar to use, to generate the path. Defaults to SPLITCHAR.
+        callOnlyOnBaseValues (bool, optional): A Flag, to call the Function only on Values. Defaults to True.
+        max_depth (_type_, optional): Determine the max Depth, after which the Iteration will be stopped.. Defaults to None.
+        parent (str, optional): For Recursive call only. Defaults to ''.
+        level (int, optional): For Recursive call only. Defaults to 0.
+    """
+    if isInt(max_depth) and level > max_depth:
+        # Break the Loop
+        return
+
+    # No try to extrac the Keys.
+    keys = getKeys(obj)
+
+    called = False
+    if not callOnlyOnBaseValues and callable(callback):
+        callback(prefix, obj, parent, level)
+        called = True
+
+    # If there exits some keys:
+    if len(keys) > 0:
+        # We will iterate over the and
+        for key in keys:
+            # Define the variable, containing the path
+            path = str(key) if '' == prefix else prefix + splitchar + str(key)
+
+            if obj[key] is not None:
+                if hasattr(obj[key], "to_json") and callable(obj[key].to_json):
+                    data = obj[key].to_json()
+                    recursiveForEach(
+                        data,
+                        callback,
+                        path,
+                        splitchar,
+                        callOnlyOnBaseValues,
+                        max_depth,
+                        prefix,
+                        level + 1
+                    )
+
+                else:
+
+                    recursiveForEach(
+                        obj[key],
+                        callback,
+                        path,
+                        splitchar,
+                        callOnlyOnBaseValues,
+                        max_depth,
+                        prefix,
+                        level + 1
+                    )
+    elif not called:
+        callback(prefix, obj, prefix, level)
+
+
+def keepProperties(obj, properties):
+    if allowsSubscripton(obj):
+        ret = DottedDict({})
+        default_obj = DottedDict({'error': True})
+
+        for key in getKeys(obj):
+            value = rgetattr(obj, key, default_obj)
+            valueToAssign = value
+            if value != default_obj:
+                valueToAssign = copy(value)
+            else:
+                valueToAssign = properties[key]()
+            rsetattr(ret, key, valueToAssign)
+
+        return ret
+    raise Exception('Function can only create Objects')
+
+
+WARNED = False
+
+
+def copy(obj):
+    """ A Helper, which can be used to receive a copy.
+
+    Args:
+        obj (any): The Object to copy
+
+    Returns:
+        bool, any: A flag, to show whether it succeeded or failed; the copy (or if failed the object) itself.
+    """
+    try:
+        return deepcopy(obj)
+    except BaseException:
+        try:
+            return obj.copy()
+        except BaseException:
+            global WARNED
+            if not WARNED:
+                WARNED = True
+                print("Failed to create a copy using orignal value.")
+            return obj
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/path.py` & `nope_py-1.7.9/nope/helpers/path.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/helpers/pathMatchingMethods.py` & `nope_py-1.7.9/nope/helpers/pathMatchingMethods.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-from .dottedDict import ensureDottedAccess, DottedDict
-from .path import (MULTI_LEVEL_WILDCARD, SINGLE_LEVEL_WILDCARD, SPLITCHAR,
-                   containsWildcards, patternIsValid)
-
-
-def generateResult(res=DottedDict({})):
-    """ internal helper to generate the defined result.
-
-    Args:
-        res (dotted_dict, optional): The Result. Defaults to dotted_dict({}).
-
-    Returns:
-        dotted_dict: The Result
-    """
-    defaultResult = DottedDict({
-        'affected': False,
-        'affectedByChild': False,
-        'affectedByParent': False,
-        'affectedOnSameLevel': False,
-        'containsWildcards': False,
-        'patternToExtractData': False,
-        'patternLengthComparedToPathLength': '=',
-        'pathToExtractData': False
-    })
-
-    defaultResult.update(res)
-    defaultResult.affected = defaultResult.affectedByChild or defaultResult.affectedByParent or defaultResult.affectedOnSameLevel
-
-    return defaultResult
-
-
-def comparePatternAndPath(pathPattern: str, contentPath: str, _options=None):
-    """ Matches the given path, with the pattern and determines, if the path might affect the given pattern.
-
-        example: path = "a/b/c"; pattern = "a/#"; => totalPath = "a/b/c"; diffPath = "b/c"
-
-    Args:
-        pathPattern (str): The pattern to test
-        contentPath (str): The path to use as basis
-        options (dotted_dict, optional): _description_. Defaults to dotted_dict({'matchTopicsWithoutWildcards': False}).
-
-    Returns:
-        dotted_dict: The Result
-    """
-    options = ensureDottedAccess({'matchTopicsWithoutWildcards': False})
-    options.update(ensureDottedAccess(_options))
-
-    if containsWildcards(contentPath):
-        raise Exception(
-            "The Path is invalid. The path should not contain pattern-related chars '#' or '+'.")
-    if not patternIsValid(pathPattern):
-        raise Exception('The Pattern is invalid.')
-    if not patternIsValid(contentPath):
-        raise Exception('The Path is invalid.')
-
-    _containsWildcards = containsWildcards(pathPattern)
-    _patternSegments = pathPattern.split(SPLITCHAR)
-    _contentPathSegments = contentPath.split(SPLITCHAR)
-    _patternLength = len(_patternSegments)
-    _contentPathLength = len(_contentPathSegments)
-
-    # Define the Char for the comparer
-    patternLengthComparedToPathLength = '='
-    if _patternLength > _contentPathLength:
-        patternLengthComparedToPathLength = '>'
-    elif _patternLength < _contentPathLength:
-        patternLengthComparedToPathLength = '<'
-
-    # If both, the pattern and the path are equal => return the result.
-    if pathPattern == contentPath:
-        return generateResult(
-            DottedDict(
-                {
-                    'affectedOnSameLevel': True,
-                    'pathToExtractData': contentPath,
-                    'patternLengthComparedToPathLength': patternLengthComparedToPathLength
-                }
-            )
-        )
-
-    # If the Path is not realy defined.
-    if contentPath == '':
-        return generateResult(
-            DottedDict({
-                'affectedByParent': True,
-                'patternToExtractData': pathPattern if _containsWildcards else False,
-                'pathToExtractData': False if _containsWildcards else pathPattern,
-                'patternLengthComparedToPathLength': '>',
-                'containsWildcards': _containsWildcards
-            })
-        )
-    if pathPattern == '':
-        return generateResult(
-            DottedDict({
-                'affectedByChild': True,
-                'pathToExtractData': '',
-                'patternLengthComparedToPathLength': '<'
-            })
-        )
-    if options.matchTopicsWithoutWildcards:
-        if contentPath.startswith(pathPattern):
-            # Path is longer then the Pattern;
-            # => A Change is performed by "Child",
-            if _containsWildcards:
-                return generateResult(
-                    DottedDict({
-                        'affectedByChild': True,
-                        'pathToExtractData': contentPath,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    })
-                )
-            else:
-                return generateResult(
-                    DottedDict({
-                        'affectedByChild': True,
-                        'pathToExtractData': pathPattern,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    })
-                )
-        elif pathPattern.startswith(contentPath):
-            # Pattern is longer then the path;
-            # => A Change might be initated by
-            # the super element
-
-            # The PathToExtractData is allways false, if the path is smaller then the
-            # pattern
-
-            if _containsWildcards:
-                return generateResult(
-                    DottedDict({
-                        'affectedByParent': True,
-                        'patternToExtractData': pathPattern,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    })
-                )
-            else:
-                return generateResult(
-                    DottedDict({
-                        'affectedByParent': True,
-                        'pathToExtractData': pathPattern,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    })
-                )
-
-    partialPath = ''
-    i = 0
-
-    # Iterate over the Segments.
-    while i < _patternLength:
-        # Store the current Pattern Segment
-        currentPattern = _patternSegments[i]
-
-        # We need to know, if there is SINGLE_LEVEL_WILDCARD or MULTI_LEVEL_WILDCARD
-        # there fore we will extract the Wildlevels.
-        patternChar = currentPattern[0]
-        currentPath = _contentPathSegments[i] if i < _contentPathLength else None
-        i = i + 1
-        if currentPath is None:
-            # Our Pattern is larger then our contentPath.
-            # So we dont know, whether we will get some
-            # data. Therefore we have to perform a query
-            # later ==> Set The Path / Pattern.
-
-            if _containsWildcards:
-                # But we contain Patterns.
-                # So we are not allowed to build a
-                # diff object.
-                return generateResult(
-                    DottedDict({
-                        'affectedByParent': True,
-                        'patternToExtractData': pathPattern,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    })
-                )
-            elif patternLengthComparedToPathLength == ">":
-                return generateResult(
-                    DottedDict({
-                        'affectedByParent': True,
-                        'patternToExtractData': pathPattern,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    })
-                )
-            else:
-                raise Exception('Implementation Error! This should not happen')
-        elif currentPath == currentPattern:
-            # The Patterns Match
-            # We now store the correct path of our segment.
-            partialPath = f'{partialPath}{SPLITCHAR}{currentPath}' if len(
-                partialPath) > 0 else currentPath
-        elif patternChar == MULTI_LEVEL_WILDCARD:
-
-            # We know, that MULTI_LEVEL_WILDCARDs are only at the end of the
-            # pattern. So it might happen, that:
-            # a)   our length of the pattern is the same length as the content path
-            # b)   our length of the pattern is smaller then length as the content path
-            #
-            # Our statement before alread tested, that either case a) or b) fits. Otherwise
-            # another ifstatement is valid and we wont enter this statement
-            # here.
-
-            # # We add the segment to testedCorrectPath
-            # testedCorrectPath = testedCorrectPath.length > 0 ?
-            # `{testedCorrectPath}{SPLITCHAR}{currentPath}` : currentPath;
-
-            if patternLengthComparedToPathLength == '=':
-                # Case a)
-                return generateResult(
-                    DottedDict(
-                        {
-                            'affectedOnSameLevel': True,
-                            'pathToExtractData': contentPath,
-                            'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                            'containsWildcards': _containsWildcards
-                        }
-                    )
-                )
-            elif patternLengthComparedToPathLength == '<':
-                # Case b)
-                return generateResult(DottedDict(
-                    {
-                        'affectedByChild': True,
-                        'pathToExtractData': contentPath,
-                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                        'containsWildcards': _containsWildcards
-                    }
-                ))
-            else:
-                raise Exception('Implementation Error!')
-        elif patternChar == SINGLE_LEVEL_WILDCARD:
-            # Store the correct path.
-            partialPath = f'{partialPath}{SPLITCHAR}{currentPath}' if len(
-                partialPath) > 0 else currentPath
-        elif patternChar != SINGLE_LEVEL_WILDCARD and currentPattern != currentPath:
-            return generateResult(DottedDict({
-                'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-                'containsWildcards': _containsWildcards
-            }))
-    diff = contentPath[len(partialPath):]
-    return generateResult(DottedDict({
-        'affectedOnSameLevel': len(diff) == 0,
-        'affectedByChild': len(diff) >= 1,
-        'pathToExtractData': partialPath,
-        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
-        'containsWildcards': _containsWildcards
-    }))
+from .dottedDict import ensureDottedAccess, DottedDict
+from .path import (MULTI_LEVEL_WILDCARD, SINGLE_LEVEL_WILDCARD, SPLITCHAR,
+                   containsWildcards, patternIsValid)
+
+
+def generateResult(res=DottedDict({})):
+    """ internal helper to generate the defined result.
+
+    Args:
+        res (dotted_dict, optional): The Result. Defaults to dotted_dict({}).
+
+    Returns:
+        dotted_dict: The Result
+    """
+    defaultResult = DottedDict({
+        'affected': False,
+        'affectedByChild': False,
+        'affectedByParent': False,
+        'affectedOnSameLevel': False,
+        'containsWildcards': False,
+        'patternToExtractData': False,
+        'patternLengthComparedToPathLength': '=',
+        'pathToExtractData': False
+    })
+
+    defaultResult.update(res)
+    defaultResult.affected = defaultResult.affectedByChild or defaultResult.affectedByParent or defaultResult.affectedOnSameLevel
+
+    return defaultResult
+
+
+def comparePatternAndPath(pathPattern: str, contentPath: str, _options=None):
+    """ Matches the given path, with the pattern and determines, if the path might affect the given pattern.
+
+        example: path = "a/b/c"; pattern = "a/#"; => totalPath = "a/b/c"; diffPath = "b/c"
+
+    Args:
+        pathPattern (str): The pattern to test
+        contentPath (str): The path to use as basis
+        options (dotted_dict, optional): _description_. Defaults to dotted_dict({'matchTopicsWithoutWildcards': False}).
+
+    Returns:
+        dotted_dict: The Result
+    """
+    options = ensureDottedAccess({'matchTopicsWithoutWildcards': False})
+    options.update(ensureDottedAccess(_options))
+
+    if containsWildcards(contentPath):
+        raise Exception(
+            "The Path is invalid. The path should not contain pattern-related chars '#' or '+'.")
+    if not patternIsValid(pathPattern):
+        raise Exception('The Pattern is invalid.')
+    if not patternIsValid(contentPath):
+        raise Exception('The Path is invalid.')
+
+    _containsWildcards = containsWildcards(pathPattern)
+    _patternSegments = pathPattern.split(SPLITCHAR)
+    _contentPathSegments = contentPath.split(SPLITCHAR)
+    _patternLength = len(_patternSegments)
+    _contentPathLength = len(_contentPathSegments)
+
+    # Define the Char for the comparer
+    patternLengthComparedToPathLength = '='
+    if _patternLength > _contentPathLength:
+        patternLengthComparedToPathLength = '>'
+    elif _patternLength < _contentPathLength:
+        patternLengthComparedToPathLength = '<'
+
+    # If both, the pattern and the path are equal => return the result.
+    if pathPattern == contentPath:
+        return generateResult(
+            DottedDict(
+                {
+                    'affectedOnSameLevel': True,
+                    'pathToExtractData': contentPath,
+                    'patternLengthComparedToPathLength': patternLengthComparedToPathLength
+                }
+            )
+        )
+
+    # If the Path is not realy defined.
+    if contentPath == '':
+        return generateResult(
+            DottedDict({
+                'affectedByParent': True,
+                'patternToExtractData': pathPattern if _containsWildcards else False,
+                'pathToExtractData': False if _containsWildcards else pathPattern,
+                'patternLengthComparedToPathLength': '>',
+                'containsWildcards': _containsWildcards
+            })
+        )
+    if pathPattern == '':
+        return generateResult(
+            DottedDict({
+                'affectedByChild': True,
+                'pathToExtractData': '',
+                'patternLengthComparedToPathLength': '<'
+            })
+        )
+    if options.matchTopicsWithoutWildcards:
+        if contentPath.startswith(pathPattern):
+            # Path is longer then the Pattern;
+            # => A Change is performed by "Child",
+            if _containsWildcards:
+                return generateResult(
+                    DottedDict({
+                        'affectedByChild': True,
+                        'pathToExtractData': contentPath,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
+            else:
+                return generateResult(
+                    DottedDict({
+                        'affectedByChild': True,
+                        'pathToExtractData': pathPattern,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
+        elif pathPattern.startswith(contentPath):
+            # Pattern is longer then the path;
+            # => A Change might be initated by
+            # the super element
+
+            # The PathToExtractData is allways false, if the path is smaller then the
+            # pattern
+
+            if _containsWildcards:
+                return generateResult(
+                    DottedDict({
+                        'affectedByParent': True,
+                        'patternToExtractData': pathPattern,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
+            else:
+                return generateResult(
+                    DottedDict({
+                        'affectedByParent': True,
+                        'pathToExtractData': pathPattern,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
+
+    partialPath = ''
+    i = 0
+
+    # Iterate over the Segments.
+    while i < _patternLength:
+        # Store the current Pattern Segment
+        currentPattern = _patternSegments[i]
+
+        # We need to know, if there is SINGLE_LEVEL_WILDCARD or MULTI_LEVEL_WILDCARD
+        # there fore we will extract the Wildlevels.
+        patternChar = currentPattern[0]
+        currentPath = _contentPathSegments[i] if i < _contentPathLength else None
+        i = i + 1
+        if currentPath is None:
+            # Our Pattern is larger then our contentPath.
+            # So we dont know, whether we will get some
+            # data. Therefore we have to perform a query
+            # later ==> Set The Path / Pattern.
+
+            if _containsWildcards:
+                # But we contain Patterns.
+                # So we are not allowed to build a
+                # diff object.
+                return generateResult(
+                    DottedDict({
+                        'affectedByParent': True,
+                        'patternToExtractData': pathPattern,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
+            elif patternLengthComparedToPathLength == ">":
+                return generateResult(
+                    DottedDict({
+                        'affectedByParent': True,
+                        'patternToExtractData': pathPattern,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    })
+                )
+            else:
+                raise Exception('Implementation Error! This should not happen')
+        elif currentPath == currentPattern:
+            # The Patterns Match
+            # We now store the correct path of our segment.
+            partialPath = f'{partialPath}{SPLITCHAR}{currentPath}' if len(
+                partialPath) > 0 else currentPath
+        elif patternChar == MULTI_LEVEL_WILDCARD:
+
+            # We know, that MULTI_LEVEL_WILDCARDs are only at the end of the
+            # pattern. So it might happen, that:
+            # a)   our length of the pattern is the same length as the content path
+            # b)   our length of the pattern is smaller then length as the content path
+            #
+            # Our statement before alread tested, that either case a) or b) fits. Otherwise
+            # another ifstatement is valid and we wont enter this statement
+            # here.
+
+            # # We add the segment to testedCorrectPath
+            # testedCorrectPath = testedCorrectPath.length > 0 ?
+            # `{testedCorrectPath}{SPLITCHAR}{currentPath}` : currentPath;
+
+            if patternLengthComparedToPathLength == '=':
+                # Case a)
+                return generateResult(
+                    DottedDict(
+                        {
+                            'affectedOnSameLevel': True,
+                            'pathToExtractData': contentPath,
+                            'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                            'containsWildcards': _containsWildcards
+                        }
+                    )
+                )
+            elif patternLengthComparedToPathLength == '<':
+                # Case b)
+                return generateResult(DottedDict(
+                    {
+                        'affectedByChild': True,
+                        'pathToExtractData': contentPath,
+                        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                        'containsWildcards': _containsWildcards
+                    }
+                ))
+            else:
+                raise Exception('Implementation Error!')
+        elif patternChar == SINGLE_LEVEL_WILDCARD:
+            # Store the correct path.
+            partialPath = f'{partialPath}{SPLITCHAR}{currentPath}' if len(
+                partialPath) > 0 else currentPath
+        elif patternChar != SINGLE_LEVEL_WILDCARD and currentPattern != currentPath:
+            return generateResult(DottedDict({
+                'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+                'containsWildcards': _containsWildcards
+            }))
+    diff = contentPath[len(partialPath):]
+    return generateResult(DottedDict({
+        'affectedOnSameLevel': len(diff) == 0,
+        'affectedByChild': len(diff) >= 1,
+        'pathToExtractData': partialPath,
+        'patternLengthComparedToPathLength': patternLengthComparedToPathLength,
+        'containsWildcards': _containsWildcards
+    }))
```

### Comparing `nope_py-1.7.8rc3/nope/helpers/prints.py` & `nope_py-1.7.9/nope/helpers/prints.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/helpers/runtime.py` & `nope_py-1.7.9/nope/helpers/runtime.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/helpers/timers.py` & `nope_py-1.7.9/nope/helpers/timers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/nope/loader/nopePackkageLoader.py` & `nope_py-1.7.9/nope/loader/nopePackkageLoader.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-import asyncio
-import itertools
-import logging
-import typing
-
-
-from ..dispatcher import NopeDispatcher
-from ..helpers import formatException, ensureDottedAccess
-from ..logger import defineNopeLogger
-from ..types import NopePackage
-
-
-class NopePackageLoader():
-    def __init__(self, dispatcher: NopeDispatcher, **options):
-        _options = ensureDottedAccess(options)
-        self._logger = defineNopeLogger(_options.log, 'package-loader')
-        self.packages: typing.Dict[str, NopePackage] = {}
-        self.dispatcher = dispatcher
-        self._instances = {}
-        self._dispose_default_instance = []
-
-    async def addPackage(self, package: NopePackage):
-        """ Loader Function. self function will register all provided functions,
-            create the desired instances. Additionally it will add all descriptors.
-
-            param package: The Package to add.
-        """
-        if package.nameOfPackage in self.packages:
-            raise Exception(
-                "Already loaded a Package with the name \"" +
-                package.nameOfPackage +
-                "\" !"
-            )
-
-        if self._logger:
-            self._logger.warn("loading package \"" +
-                              package.nameOfPackage + "\"")
-
-        # Store the Package:
-        self.packages[package.nameOfPackage] = package
-
-        # Based on the provided settings register a generator Function for the
-        # Instances:
-        for cl in package.providedClasses:
-            # Get the Settings
-            allowInstanceGeneration = cl.allowInstanceGeneration
-            maxAmountOfInstance = cl.maxAmountOfInstance
-
-            # Get the "create instance" function
-            async def _not_provided(dispatcher, identifier):
-                raise Exception(
-                    "A function to create the function must be provided")
-
-            createInstance = cl.createInstance
-            selector = cl.selector
-
-            if selector is not None and allowInstanceGeneration:
-                # Create a Function that will generate functions
-                async def _generate_instance(dispatcher, identifier):
-                    currentAmount = self._instances.get(selector, 0)
-
-                    if maxAmountOfInstance == -1 or currentAmount < maxAmountOfInstance:
-                        # Define the Instance:
-                        instance = await createInstance(dispatcher)
-                        # Assign the Name
-                        instance.identifier = identifier
-                        # Update the Used Instance
-                        self._instances[selector] = currentAmount + 1
-                        # return the instance
-                        return instance
-
-                    raise Exception("Not allowed to create instances")
-
-                await self.dispatcher.instanceManager.registerConstructor(
-                    selector,
-                    _generate_instance
-                )
-
-        for func in package.providedServices:
-            if self._logger:
-                self._logger.info("Package Loader generates the instances.")
-            await self.dispatcher.rpcManager.registerService(func.function, func.options)
-
-    async def generateInstances(self, test_requirements=True):
-        """ Function to initialize all the instances.
-        """
-        if self._logger:
-            self._logger.info("Package Loader generates the instances.")
-
-        if test_requirements:
-            # First extract all required Packages
-            reuqiredPackages = set()
-
-            for package in self.packages.values():
-                reuqiredPackages |= set(package.requiredPackages)
-
-            # Now check if the required packages are present or not.
-            for req in reuqiredPackages:
-                if req not in self.packages:
-                    raise Exception("Packages are not known")
-
-        # Now iterate over the Packages and define the defined instances.
-        for package in self.packages.values():
-            definitions = package.defaultInstances
-
-            # Iterate over the Defined Instances.
-            for definition in definitions:
-                definition = ensureDottedAccess(definition)
-
-                if self._logger:
-                    self._logger.info("Requesting Generating Instance \"" +
-                                      definition.identifier +
-                                      "\" of type \"" +
-                                      definition.type +
-                                      "\"")
-
-                instance = await self.dispatcher.instanceManager.createInstance(
-                    definition
-                )
-
-                # Store the Function, that the instance will be disposed on
-                # leaving.
-                async def _dispose():
-                    await instance.dispose()
-
-                self._dispose_default_instance.append(_dispose)
-
-                if self._logger:
-                    self._logger.info("Generated Instance" +
-                                      definition.identifier)
-
-                # Perform the autostart:
-                if definition.identifier in package.autostart:
-
-                    if self._logger:
-                        self._logger.info(
-                            "Trying to perform autostart Instance" + definition.identifier)
-
-                    try:
-                        for task in package.autostart[definition.identifier]:
-                            if task.delay > 0:
-                                await asyncio.sleep(task.delay)
-
-                            func = getattr(instance, task.name)
-                            await func(*task.params)
-                    except Exception as e:
-                        if self._logger:
-                            self._logger.error(
-                                "Failed performing autostart for " + definition.identifier)
-                            self._logger.error(formatException(e))
-                        else:
-                            print(
-                                "Failed performing autostart for " +
-                                definition.identifier)
-                            print(formatException(e))
-        if self._logger:
-            self._logger.info("generated all defined Instances")
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+import asyncio
+import itertools
+import logging
+import typing
+
+
+from ..dispatcher import NopeDispatcher
+from ..helpers import formatException, ensureDottedAccess
+from ..logger import defineNopeLogger
+from ..types import NopePackage
+
+
+class NopePackageLoader():
+    def __init__(self, dispatcher: NopeDispatcher, **options):
+        _options = ensureDottedAccess(options)
+        self._logger = defineNopeLogger(_options.log, 'package-loader')
+        self.packages: typing.Dict[str, NopePackage] = {}
+        self.dispatcher = dispatcher
+        self._instances = {}
+        self._dispose_default_instance = []
+
+    async def addPackage(self, package: NopePackage):
+        """ Loader Function. self function will register all provided functions,
+            create the desired instances. Additionally it will add all descriptors.
+
+            param package: The Package to add.
+        """
+        if package.nameOfPackage in self.packages:
+            raise Exception(
+                "Already loaded a Package with the name \"" +
+                package.nameOfPackage +
+                "\" !"
+            )
+
+        if self._logger:
+            self._logger.warn("loading package \"" +
+                              package.nameOfPackage + "\"")
+
+        # Store the Package:
+        self.packages[package.nameOfPackage] = package
+
+        # Based on the provided settings register a generator Function for the
+        # Instances:
+        for cl in package.providedClasses:
+            # Get the Settings
+            allowInstanceGeneration = cl.allowInstanceGeneration
+            maxAmountOfInstance = cl.maxAmountOfInstance
+
+            # Get the "create instance" function
+            async def _not_provided(dispatcher, identifier):
+                raise Exception(
+                    "A function to create the function must be provided")
+
+            createInstance = cl.createInstance
+            selector = cl.selector
+
+            if selector is not None and allowInstanceGeneration:
+                # Create a Function that will generate functions
+                async def _generate_instance(dispatcher, identifier):
+                    currentAmount = self._instances.get(selector, 0)
+
+                    if maxAmountOfInstance == -1 or currentAmount < maxAmountOfInstance:
+                        # Define the Instance:
+                        instance = await createInstance(dispatcher)
+                        # Assign the Name
+                        instance.identifier = identifier
+                        # Update the Used Instance
+                        self._instances[selector] = currentAmount + 1
+                        # return the instance
+                        return instance
+
+                    raise Exception("Not allowed to create instances")
+
+                await self.dispatcher.instanceManager.registerConstructor(
+                    selector,
+                    _generate_instance
+                )
+
+        for func in package.providedServices:
+            if self._logger:
+                self._logger.info("Package Loader generates the instances.")
+            await self.dispatcher.rpcManager.registerService(func.function, func.options)
+
+    async def generateInstances(self, test_requirements=True):
+        """ Function to initialize all the instances.
+        """
+        if self._logger:
+            self._logger.info("Package Loader generates the instances.")
+
+        if test_requirements:
+            # First extract all required Packages
+            reuqiredPackages = set()
+
+            for package in self.packages.values():
+                reuqiredPackages |= set(package.requiredPackages)
+
+            # Now check if the required packages are present or not.
+            for req in reuqiredPackages:
+                if req not in self.packages:
+                    raise Exception("Packages are not known")
+
+        # Now iterate over the Packages and define the defined instances.
+        for package in self.packages.values():
+            definitions = package.defaultInstances
+
+            # Iterate over the Defined Instances.
+            for definition in definitions:
+                definition = ensureDottedAccess(definition)
+
+                if self._logger:
+                    self._logger.info("Requesting Generating Instance \"" +
+                                      definition.identifier +
+                                      "\" of type \"" +
+                                      definition.type +
+                                      "\"")
+
+                instance = await self.dispatcher.instanceManager.createInstance(
+                    definition
+                )
+
+                # Store the Function, that the instance will be disposed on
+                # leaving.
+                async def _dispose():
+                    await instance.dispose()
+
+                self._dispose_default_instance.append(_dispose)
+
+                if self._logger:
+                    self._logger.info("Generated Instance" +
+                                      definition.identifier)
+
+                # Perform the autostart:
+                if definition.identifier in package.autostart:
+
+                    if self._logger:
+                        self._logger.info(
+                            "Trying to perform autostart Instance" + definition.identifier)
+
+                    try:
+                        for task in package.autostart[definition.identifier]:
+                            if task.delay > 0:
+                                await asyncio.sleep(task.delay)
+
+                            func = getattr(instance, task.name)
+                            await func(*task.params)
+                    except Exception as e:
+                        if self._logger:
+                            self._logger.error(
+                                "Failed performing autostart for " + definition.identifier)
+                            self._logger.error(formatException(e))
+                        else:
+                            print(
+                                "Failed performing autostart for " +
+                                definition.identifier)
+                            print(formatException(e))
+        if self._logger:
+            self._logger.info("generated all defined Instances")
```

### Comparing `nope_py-1.7.8rc3/nope/logger/logger.py` & `nope_py-1.7.9/nope/logger/logger.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-#!/usr/bin/env python
-
-import logging
-import sys
-
-DEBUG = logging.DEBUG
-INFO = logging.INFO
-ERROR = logging.ERROR
-WARNING = logging.WARNING
-CRITICAL = logging.CRITICAL
-
-LEVELS = {'info': INFO, 'debug': DEBUG, 'warn': WARNING, 'error': ERROR}
-
-_LOGGERS = {}
-
-
-class ColorizedFormatter(logging.Formatter):
-    """Logging colored formatter, adapted from https://stackoverflow.com/a/56944256/3638629"""
-
-    grey = '\x1b[38;21m'
-    blue = '\x1b[38;5;39m'
-    yellow = '\x1b[38;5;226m'
-    red = '\x1b[38;5;196m'
-    bold_red = '\x1b[31;1m'
-    reset = '\x1b[0m'
-
-    def __init__(self, fmt):
-        super().__init__()
-        self.fmt = fmt
-        self.FORMATS = {
-            logging.DEBUG: self.grey + self.fmt + self.reset,
-            logging.INFO: self.blue + self.fmt + self.reset,
-            logging.WARNING: self.yellow + self.fmt + self.reset,
-            logging.ERROR: self.red + self.fmt + self.reset,
-            logging.CRITICAL: self.bold_red + self.fmt + self.reset
-        }
-
-    def format(self, record):
-        log_fmt = self.FORMATS.get(record.levelno)
-        formatter = logging.Formatter(log_fmt)
-        return formatter.format(record)
-
-
-def getNopeLogger(name: str, level=logging.DEBUG):
-    """ Helper to return a specific logger.
-
-    """
-    global _LOGGERS
-
-    if name not in _LOGGERS:
-
-        nameToUse = name
-        length = 30
-
-        if len(nameToUse) > length:
-            nameToUse = nameToUse[:length - 3] + "..."
-
-        _logger = logging.getLogger(nameToUse)
-        # Define  a Logging Format
-
-        _format = ColorizedFormatter(
-            '%(asctime)s - %(levelname)-8s - %(name)-' + str(length) + 's - %(message)s')
-
-        # Create Console Output
-        _handler = logging.StreamHandler(sys.stdout)
-        # Add the Format to the Handler
-        _handler.setFormatter(_format)
-        # Set Loglevel to the Desired One.
-        _handler.setLevel(level)
-
-        # Finally add the Handler to the Logger:
-        _logger.addHandler(_handler)
-
-        # Set the Log Level of the Logger.
-        _logger.setLevel(level)
-
-        _LOGGERS[name] = _logger
-
-    return _LOGGERS[name]
-
-
-def defineNopeLogger(param, default_name: str):
-    """ Helper to define a Logger. The parameter 'param' is either a logger, None, or a Logger-Level
-
-    """
-    if not param:
-        return None
-    if isinstance(param, str):
-        return getNopeLogger(default_name, LEVELS[param])
-    return param
+#!/usr/bin/env python
+
+import logging
+import sys
+
+DEBUG = logging.DEBUG
+INFO = logging.INFO
+ERROR = logging.ERROR
+WARNING = logging.WARNING
+CRITICAL = logging.CRITICAL
+
+LEVELS = {'info': INFO, 'debug': DEBUG, 'warn': WARNING, 'error': ERROR}
+
+_LOGGERS = {}
+
+
+class ColorizedFormatter(logging.Formatter):
+    """Logging colored formatter, adapted from https://stackoverflow.com/a/56944256/3638629"""
+
+    grey = '\x1b[38;21m'
+    blue = '\x1b[38;5;39m'
+    yellow = '\x1b[38;5;226m'
+    red = '\x1b[38;5;196m'
+    bold_red = '\x1b[31;1m'
+    reset = '\x1b[0m'
+
+    def __init__(self, fmt):
+        super().__init__()
+        self.fmt = fmt
+        self.FORMATS = {
+            logging.DEBUG: self.grey + self.fmt + self.reset,
+            logging.INFO: self.blue + self.fmt + self.reset,
+            logging.WARNING: self.yellow + self.fmt + self.reset,
+            logging.ERROR: self.red + self.fmt + self.reset,
+            logging.CRITICAL: self.bold_red + self.fmt + self.reset
+        }
+
+    def format(self, record):
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt)
+        return formatter.format(record)
+
+
+def getNopeLogger(name: str, level=logging.DEBUG):
+    """ Helper to return a specific logger.
+
+    """
+    global _LOGGERS
+
+    if name not in _LOGGERS:
+
+        nameToUse = name
+        length = 30
+
+        if len(nameToUse) > length:
+            nameToUse = nameToUse[:length - 3] + "..."
+
+        _logger = logging.getLogger(nameToUse)
+        # Define  a Logging Format
+
+        _format = ColorizedFormatter(
+            '%(asctime)s - %(levelname)-8s - %(name)-' + str(length) + 's - %(message)s')
+
+        # Create Console Output
+        _handler = logging.StreamHandler(sys.stdout)
+        # Add the Format to the Handler
+        _handler.setFormatter(_format)
+        # Set Loglevel to the Desired One.
+        _handler.setLevel(level)
+
+        # Finally add the Handler to the Logger:
+        _logger.addHandler(_handler)
+
+        # Set the Log Level of the Logger.
+        _logger.setLevel(level)
+
+        _LOGGERS[name] = _logger
+
+    return _LOGGERS[name]
+
+
+def defineNopeLogger(param, default_name: str):
+    """ Helper to define a Logger. The parameter 'param' is either a logger, None, or a Logger-Level
+
+    """
+    if not param:
+        return None
+    if isinstance(param, str):
+        return getNopeLogger(default_name, LEVELS[param])
+    return param
```

### Comparing `nope_py-1.7.8rc3/nope/merging/mergeData.py` & `nope_py-1.7.9/nope/merging/mergeData.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from ..eventEmitter import NopeEventEmitter
-from ..helpers import DottedDict, extractUniqueValues, transformDict, determineDifference
-from ..observable import NopeObservable
-
-
-class MergeData:
-
-    def __init__(self, originalData, _extractData):
-        self.originalData = originalData
-        self._extractData = _extractData
-        self.onChange = NopeEventEmitter()
-        self.data = NopeObservable()
-        self.data.setContent([])
-        self.error = False
-
-        self.update(force=True)
-
-    def update(self, data=None, force=False):
-        if data is not None:
-            self.originalData = data
-        after_adding = self._extractData(self.originalData)
-        diff = determineDifference(self.data.getContent(), after_adding)
-        if force or ((len(diff.removed) > 0) or len(diff.added) > 0):
-            self.data.setContent(list(after_adding))
-            self.onChange.emit(DottedDict(
-                {'added': list(diff.added), 'removed': list(diff.removed)}))
-
-    def dispose(self):
-        self.data.dispose()
-        self.onChange.dispose()
-
-
-class DictBasedMergeData(MergeData):
-
-    def __init__(self, originalData, _path='', _pathKey=None):
-        def callback(m):
-            return extractUniqueValues(m, _path, _pathKey)
-
-        self._path = _path
-        self._pathKey = _pathKey
-        self.amountOf = dict()
-        self.simplified = dict()
-        self.keyMapping = dict()
-        self.keyMappingreverse = dict()
-        self.conflicts = dict()
-        self.orgKeyToExtractedValue = dict()
-        self.extracted_key = []
-        self.extracted_value = []
-
-        super().__init__(originalData, callback)
-
-    def update(self, data=None, force=False):
-        if data is not None:
-            self.originalData = data
-        result = transformDict(self.originalData, self._path, self._pathKey)
-
-        self.simplified = result.extracted_map
-        self.amountOf = result.amountOf
-        self.keyMapping = result.keyMapping
-        self.keyMappingreverse = result.keyMappingreverse
-        self.conflicts = result.conflicts
-        self.orgKeyToExtractedValue = result.orgKeyToExtractedValue
-        self.extracted_key = [*self.simplified.keys()]
-        self.extracted_value = [*self.simplified.values()]
-
-        super().update(data, force)
+from ..eventEmitter import NopeEventEmitter
+from ..helpers import DottedDict, extractUniqueValues, transformDict, determineDifference
+from ..observable import NopeObservable
+
+
+class MergeData:
+
+    def __init__(self, originalData, _extractData):
+        self.originalData = originalData
+        self._extractData = _extractData
+        self.onChange = NopeEventEmitter()
+        self.data = NopeObservable()
+        self.data.setContent([])
+        self.error = False
+
+        self.update(force=True)
+
+    def update(self, data=None, force=False):
+        if data is not None:
+            self.originalData = data
+        after_adding = self._extractData(self.originalData)
+        diff = determineDifference(self.data.getContent(), after_adding)
+        if force or ((len(diff.removed) > 0) or len(diff.added) > 0):
+            self.data.setContent(list(after_adding))
+            self.onChange.emit(DottedDict(
+                {'added': list(diff.added), 'removed': list(diff.removed)}))
+
+    def dispose(self):
+        self.data.dispose()
+        self.onChange.dispose()
+
+
+class DictBasedMergeData(MergeData):
+
+    def __init__(self, originalData, _path='', _pathKey=None):
+        def callback(m):
+            return extractUniqueValues(m, _path, _pathKey)
+
+        self._path = _path
+        self._pathKey = _pathKey
+        self.amountOf = dict()
+        self.simplified = dict()
+        self.keyMapping = dict()
+        self.keyMappingreverse = dict()
+        self.conflicts = dict()
+        self.orgKeyToExtractedValue = dict()
+        self.extracted_key = []
+        self.extracted_value = []
+
+        super().__init__(originalData, callback)
+
+    def update(self, data=None, force=False):
+        if data is not None:
+            self.originalData = data
+        result = transformDict(self.originalData, self._path, self._pathKey)
+
+        self.simplified = result.extracted_map
+        self.amountOf = result.amountOf
+        self.keyMapping = result.keyMapping
+        self.keyMappingreverse = result.keyMappingreverse
+        self.conflicts = result.conflicts
+        self.orgKeyToExtractedValue = result.orgKeyToExtractedValue
+        self.extracted_key = [*self.simplified.keys()]
+        self.extracted_value = [*self.simplified.values()]
+
+        super().update(data, force)
```

### Comparing `nope_py-1.7.8rc3/nope/observable/nopeObservable.py` & `nope_py-1.7.9/nope/observable/nopeObservable.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from ..eventEmitter import NopeEventEmitter
-from ..helpers import DottedDict, ensureDottedAccess, generateId
-
-
-class NopeObservable(NopeEventEmitter):
-    """ An Observable storing the last value in `content`.
-    """
-
-    def __init__(self, options=None):
-
-        if options is None:
-            options = DottedDict()
-
-        options.update({'showCurrent': True})
-        super().__init__(options)
-        self.id = generateId()
-        self._value = None
-        self._lastValue = None
-        self._lastRest = None
-
-    @property
-    def emitter(self):
-        return self._emitter
-
-    def setContent(self, value, options=None):
-        return self._emit(value, options)
-
-    def _emit(self, value, options=None):
-        options = ensureDottedAccess(options)
-        if self.setter is not None and callable(self.setter):
-            adapted = ensureDottedAccess(self.setter(value, options))
-            if not adapted.valid:
-                return False
-            self._value = adapted.data
-        else:
-            self._value = value
-        valueToPublish = self.getContent()
-        if (not self.disablePublishing) and (
-                options.forced or not (self._lastValue == valueToPublish)):
-            return self._publish(valueToPublish, options)
-        return False
-
-    # def emit(self, *args, **kwargs):
-    #     raise NotImplementedError("Not implemeneted on an Observable.")
-
-    def _informSpecificObserver(self, observer):
-        if self._lastRest is not None:
-            # Call the last rest
-            observer(ensureDottedAccess(
-                {"value": self._lastValue, **self._lastRest}))
-
-    def _publish(self, value, options=None):
-        options = ensureDottedAccess(options)
-        if options.forced or not self.disablePublishing:
-            options = self._updateSenderAndTimestamp(options)
-            self._lastRest = options
-            self._lastValue = value
-            self._emitter.emit(data=ensureDottedAccess(
-                {'value': value, **options}))
-            return self.hasSubscriptions
-        return False
-
-    def forcePublish(self, options=None):
-        options = ensureDottedAccess(options)
-        options.forced = True
-        return self._publish(self.getContent(), options)
-
-    def getContent(self):
-        if self.getter is not None:
-            return self.getter(self._value)
-        return self._value
-
-    @property
-    def content(self):
-        return self.getContent()
-
-    def subscribe(self, callback, options=None):
-        if options is None:
-            options = {'mode': [
-                'direct', 'sub', 'super'], 'skipCurrent': False}
-
-        customCallback = self._adaptCallback(
-            callback, ensureDottedAccess(options))
-
-        res = self._subscribe(customCallback)
-
-        # Because we are an observerable -> we will send the update:
-        self._informSpecificObserver(customCallback)
-
-        return res
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from ..eventEmitter import NopeEventEmitter
+from ..helpers import DottedDict, ensureDottedAccess, generateId
+
+
+class NopeObservable(NopeEventEmitter):
+    """ An Observable storing the last value in `content`.
+    """
+
+    def __init__(self, options=None):
+
+        if options is None:
+            options = DottedDict()
+
+        options.update({'showCurrent': True})
+        super().__init__(options)
+        self.id = generateId()
+        self._value = None
+        self._lastValue = None
+        self._lastRest = None
+
+    @property
+    def emitter(self):
+        return self._emitter
+
+    def setContent(self, value, options=None):
+        return self._emit(value, options)
+
+    def _emit(self, value, options=None):
+        options = ensureDottedAccess(options)
+        if self.setter is not None and callable(self.setter):
+            adapted = ensureDottedAccess(self.setter(value, options))
+            if not adapted.valid:
+                return False
+            self._value = adapted.data
+        else:
+            self._value = value
+        valueToPublish = self.getContent()
+        if (not self.disablePublishing) and (
+                options.forced or not (self._lastValue == valueToPublish)):
+            return self._publish(valueToPublish, options)
+        return False
+
+    # def emit(self, *args, **kwargs):
+    #     raise NotImplementedError("Not implemeneted on an Observable.")
+
+    def _informSpecificObserver(self, observer):
+        if self._lastRest is not None:
+            # Call the last rest
+            observer(ensureDottedAccess(
+                {"value": self._lastValue, **self._lastRest}))
+
+    def _publish(self, value, options=None):
+        options = ensureDottedAccess(options)
+        if options.forced or not self.disablePublishing:
+            options = self._updateSenderAndTimestamp(options)
+            self._lastRest = options
+            self._lastValue = value
+            self._emitter.emit(data=ensureDottedAccess(
+                {'value': value, **options}))
+            return self.hasSubscriptions
+        return False
+
+    def forcePublish(self, options=None):
+        options = ensureDottedAccess(options)
+        options.forced = True
+        return self._publish(self.getContent(), options)
+
+    def getContent(self):
+        if self.getter is not None:
+            return self.getter(self._value)
+        return self._value
+
+    @property
+    def content(self):
+        return self.getContent()
+
+    def subscribe(self, callback, options=None):
+        if options is None:
+            options = {'mode': [
+                'direct', 'sub', 'super'], 'skipCurrent': False}
+
+        customCallback = self._adaptCallback(
+            callback, ensureDottedAccess(options))
+
+        res = self._subscribe(customCallback)
+
+        # Because we are an observerable -> we will send the update:
+        self._informSpecificObserver(customCallback)
+
+        return res
```

### Comparing `nope_py-1.7.8rc3/nope/plugins/ack_messages.py` & `nope_py-1.7.9/nope/plugins/ack_messages.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-""" An example how to modify the Behavior of multiple elements using a Plugin.
-
-    In This case the Plugin allows the implementation of an ackknowledgement
-    message if required.
-"""
-
-from nope.eventEmitter import NopeEventEmitter
-from nope.helpers import generateId, EXECUTOR, ensureDottedAccess, formatException
-from nope.plugins import plugin
-
-
-@plugin([
-    "nope.communication.bridge",
-    "nope.dispatcher.connectivityManager"
-],
-    name="ackMessages")
-def extend(bridgeMod, conManagerMod):
-    "Extends the Bridge and adds the functionality of ack knowlededing messages."
-
-    class Bridge(bridgeMod.Bridge):
-        def __init__(self, *args, **kwargs):
-            bridgeMod.Bridge.__init__(self, *args, **kwargs)
-
-            # Define
-            self.defaultTargets = kwargs.get("defaultTargets", list())
-            self.ackReplyId = kwargs.get("ackReplyId", None)
-            self.onTransportError = NopeEventEmitter()
-            self._onMessageReceived = NopeEventEmitter()
-
-            # Dict containing the Messages, that have been send as key and containign the
-            # still open respones (dispatcher ids) as set as value
-            self._openMessages = {}
-
-            # Make shure to forward ackknowledge messages.
-            EXECUTOR.callParallel(
-                self.on,
-                "ackMessage",
-                lambda msg: self._onMessageReceived.emit(msg))
-
-            # Subscribe to Errors:
-            def onTransportError(err, *args):
-                if self._logger:
-                    self._logger.error(
-                        "Failed to receive an acknowledge message!")
-                    self._logger.error(formatException(err))
-                else:
-                    print(formatException(err))
-
-            self.onTransportError.subscribe(onTransportError)
-
-        async def emit(self, eventName, data, target=None, timeout=0, **kwargs):
-            promise = None
-
-            if eventName != "ackMessage" and self.ackReplyId is not None:
-                # Now lets define the Target:
-                if target is None or target == True:
-                    if self.defaultTargets:
-                        target = set(self.defaultTargets)
-                    elif "target" in data:
-                        target = set([data["target"]])
-                    else:
-                        target = set()
-                else:
-                    if isinstance(target, str):
-                        target = set([target])
-                    elif target == False:
-                        target = set()
-                    else:
-                        target = set(target)
-
-                # Only if we expect a target,
-                # we will wait for the message.
-                if len(target) > 0:
-                    messageId = generateId()
-                    data["messageId"] = messageId
-
-                    def callback(msg, *args):
-                        nonlocal messageId
-
-                        if msg.get(
-                                "messageId", False) == messageId and messageId in self._openMessages:
-
-                            data = self._openMessages.get(
-                                messageId, False)
-
-                            # Mark the Dispatcher as ready:
-                            data["received"].add(msg["dispatcherId"])
-
-                            if len(data["target"] - data["received"]) == 0:
-                                # Remove the Message, becaus it is finished
-                                self._openMessages.pop(messageId)
-
-                                return True
-
-                        return False
-
-                    promise = self._onMessageReceived.waitFor(
-                        callback, options={"timeout": timeout})
-
-                    # Store the Message
-                    self._openMessages[messageId] = {
-                        "received": set(),
-                        "target": target,
-                        "promise": promise
-                    }
-
-            res = await bridgeMod.Bridge.emit(self, eventName, data, **kwargs)
-
-            if promise:
-                await promise
-
-            return res
-
-        async def on(self, eventName, cb):
-            # In here we will define a custom callback,
-            # which will send an "ackMessage" after
-            # performing the original callback.
-
-            if eventName == "ackMessage":
-                return await bridgeMod.Bridge.on(self, eventName, cb)
-
-            def callback(msg):
-                cb(msg)
-
-                if "messageId" in msg and self.ackReplyId is not None:
-                    EXECUTOR.callParallel(
-                        self.emit,
-                        "ackMessage",
-                        ensureDottedAccess({
-                            "messageId": msg["messageId"],
-                            "dispatcherId": self.ackReplyId
-                        })
-                    )
-
-            return await bridgeMod.Bridge.on(self, eventName, callback)
-
-    class NopeConnectivityManager(conManagerMod.NopeConnectivityManager):
-        def __init__(self, *args, **kwargs):
-            conManagerMod.NopeConnectivityManager.__init__(
-                self, *args, **kwargs)
-
-            self._communicator.ackReplyId = self._id
-            self.forceAckMessage = True
-
-            # To extend
-            def cb(dispatchers: list, *args):
-                if self.forceAckMessage:
-                    # Get all Dispatchers running the Plugin.
-                    dispatchersWithPlugin = list(
-                        filter(
-                            lambda id: "ackMessages" in self.dispatchers.originalData[id].plugins,
-                            dispatchers))
-                    self._communicator.defaultTargets = dispatchersWithPlugin
-
-            self.dispatchers.data.subscribe(cb)
-
-        def _info(self):
-            ret = conManagerMod.NopeConnectivityManager._info(self)
-            ret.plugins.append("ackMessages")
-            return ret
-
-    return Bridge, NopeConnectivityManager
+""" An example how to modify the Behavior of multiple elements using a Plugin.
+
+    In This case the Plugin allows the implementation of an ackknowledgement
+    message if required.
+"""
+
+from nope.eventEmitter import NopeEventEmitter
+from nope.helpers import generateId, EXECUTOR, ensureDottedAccess, formatException
+from nope.plugins import plugin
+
+
+@plugin([
+    "nope.communication.bridge",
+    "nope.dispatcher.connectivityManager"
+],
+    name="ackMessages")
+def extend(bridgeMod, conManagerMod):
+    "Extends the Bridge and adds the functionality of ack knowlededing messages."
+
+    class Bridge(bridgeMod.Bridge):
+        def __init__(self, *args, **kwargs):
+            bridgeMod.Bridge.__init__(self, *args, **kwargs)
+
+            # Define
+            self.defaultTargets = kwargs.get("defaultTargets", list())
+            self.ackReplyId = kwargs.get("ackReplyId", None)
+            self.onTransportError = NopeEventEmitter()
+            self._onMessageReceived = NopeEventEmitter()
+
+            # Dict containing the Messages, that have been send as key and containign the
+            # still open respones (dispatcher ids) as set as value
+            self._openMessages = {}
+
+            # Make shure to forward ackknowledge messages.
+            EXECUTOR.callParallel(
+                self.on,
+                "ackMessage",
+                lambda msg: self._onMessageReceived.emit(msg))
+
+            # Subscribe to Errors:
+            def onTransportError(err, *args):
+                if self._logger:
+                    self._logger.error(
+                        "Failed to receive an acknowledge message!")
+                    self._logger.error(formatException(err))
+                else:
+                    print(formatException(err))
+
+            self.onTransportError.subscribe(onTransportError)
+
+        async def emit(self, eventName, data, target=None, timeout=0, **kwargs):
+            promise = None
+
+            if eventName != "ackMessage" and self.ackReplyId is not None:
+                # Now lets define the Target:
+                if target is None or target == True:
+                    if self.defaultTargets:
+                        target = set(self.defaultTargets)
+                    elif "target" in data:
+                        target = set([data["target"]])
+                    else:
+                        target = set()
+                else:
+                    if isinstance(target, str):
+                        target = set([target])
+                    elif target == False:
+                        target = set()
+                    else:
+                        target = set(target)
+
+                # Only if we expect a target,
+                # we will wait for the message.
+                if len(target) > 0:
+                    messageId = generateId()
+                    data["messageId"] = messageId
+
+                    def callback(msg, *args):
+                        nonlocal messageId
+
+                        if msg.get(
+                                "messageId", False) == messageId and messageId in self._openMessages:
+
+                            data = self._openMessages.get(
+                                messageId, False)
+
+                            # Mark the Dispatcher as ready:
+                            data["received"].add(msg["dispatcherId"])
+
+                            if len(data["target"] - data["received"]) == 0:
+                                # Remove the Message, becaus it is finished
+                                self._openMessages.pop(messageId)
+
+                                return True
+
+                        return False
+
+                    promise = self._onMessageReceived.waitFor(
+                        callback, options={"timeout": timeout})
+
+                    # Store the Message
+                    self._openMessages[messageId] = {
+                        "received": set(),
+                        "target": target,
+                        "promise": promise
+                    }
+
+            res = await bridgeMod.Bridge.emit(self, eventName, data, **kwargs)
+
+            if promise:
+                await promise
+
+            return res
+
+        async def on(self, eventName, cb):
+            # In here we will define a custom callback,
+            # which will send an "ackMessage" after
+            # performing the original callback.
+
+            if eventName == "ackMessage":
+                return await bridgeMod.Bridge.on(self, eventName, cb)
+
+            def callback(msg):
+                cb(msg)
+
+                if "messageId" in msg and self.ackReplyId is not None:
+                    EXECUTOR.callParallel(
+                        self.emit,
+                        "ackMessage",
+                        ensureDottedAccess({
+                            "messageId": msg["messageId"],
+                            "dispatcherId": self.ackReplyId
+                        })
+                    )
+
+            return await bridgeMod.Bridge.on(self, eventName, callback)
+
+    class NopeConnectivityManager(conManagerMod.NopeConnectivityManager):
+        def __init__(self, *args, **kwargs):
+            conManagerMod.NopeConnectivityManager.__init__(
+                self, *args, **kwargs)
+
+            self._communicator.ackReplyId = self._id
+            self.forceAckMessage = True
+
+            # To extend
+            def cb(dispatchers: list, *args):
+                if self.forceAckMessage:
+                    # Get all Dispatchers running the Plugin.
+                    dispatchersWithPlugin = list(
+                        filter(
+                            lambda id: "ackMessages" in self.dispatchers.originalData[id].plugins,
+                            dispatchers))
+                    self._communicator.defaultTargets = dispatchersWithPlugin
+
+            self.dispatchers.data.subscribe(cb)
+
+        def _info(self):
+            ret = conManagerMod.NopeConnectivityManager._info(self)
+            ret.plugins.append("ackMessages")
+            return ret
+
+    return Bridge, NopeConnectivityManager
```

### Comparing `nope_py-1.7.8rc3/nope/plugins/hello.py` & `nope_py-1.7.9/nope/plugins/hello.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-""" An example plugin that allows instances of `NopeRpcManager` to
-    say hello. The source code can be used as a starting example.
-
-    Please visist: nope/plugins/demo and "checkout" the examples.
-"""
-
-
-# @plugin("nope.dispatcher.rpcManager")
-def extend(module):
-    "Extends `module` - RPC-Manager"
-
-    class NopeRpcManager(module.NopeRpcManager):
-        def hello(self):
-            "Ask the plugin to say hello"
-            print("Hello from the Plugin")
-
-        async def performCall(self, *args, **kwargs):
-            """ Extend the original behavior """
-            print("calling 'performCall' inside of our addon")
-            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
-
-    def hello_func(self):
-        "Ask the plugin to say hello"
-        print("Hello from the Plugin")
-
-    hello_vars = {"hello": "Hello from the Plugin"}
-    return NopeRpcManager, hello_func, hello_vars
+""" An example plugin that allows instances of `NopeRpcManager` to
+    say hello. The source code can be used as a starting example.
+
+    Please visist: nope/plugins/demo and "checkout" the examples.
+"""
+
+
+# @plugin("nope.dispatcher.rpcManager")
+def extend(module):
+    "Extends `module` - RPC-Manager"
+
+    class NopeRpcManager(module.NopeRpcManager):
+        def hello(self):
+            "Ask the plugin to say hello"
+            print("Hello from the Plugin")
+
+        async def performCall(self, *args, **kwargs):
+            """ Extend the original behavior """
+            print("calling 'performCall' inside of our addon")
+            return await module.NopeRpcManager.performCall(self, *args, **kwargs)
+
+    def hello_func(self):
+        "Ask the plugin to say hello"
+        print("Hello from the Plugin")
+
+    hello_vars = {"hello": "Hello from the Plugin"}
+    return NopeRpcManager, hello_func, hello_vars
```

### Comparing `nope_py-1.7.8rc3/nope/plugins/rpc_with_callbacks.py` & `nope_py-1.7.9/nope/plugins/rpc_with_callbacks.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-""" An example how to modify the Behavior of multiple elements using a Plugin.
-
-    In This case the Plugin allows the implementation of an ackknowledgement
-    message if required.
-"""
-
-import asyncio
-
-from nope.eventEmitter import NopeEventEmitter
-from nope.helpers import generateId, EXECUTOR, ensureDottedAccess, formatException, isAsyncFunction
-from nope.plugins import plugin
-
-_DEFAULT_RESULT = object()
-
-
-@plugin([
-    "nope.dispatcher.rpcManager",
-    "nope.dispatcher.connectivityManager"
-],
-    name="rpcCallbacks")
-def extend(rpcMod, conManagerMod):
-    "Extends the Bridge and adds the functionality of ack knowlededing messages."
-
-    class NopeRpcManager(rpcMod.NopeRpcManager):
-        def __init__(self, *args, **kwargs):
-            rpcMod.NopeRpcManager.__init__(self, *args, **kwargs)
-            self.defaultKeepAlive = kwargs.get(
-                "defaultKeepAlive", 60 * 60 * 1000)
-
-        async def _handleExternalRequest(self, data, func=None):
-            try:
-                if not callable(func):
-                    if data.functionId not in self._registeredServices:
-                        return
-                    func = self._registeredServices[data.functionId].get(
-                        "func", None)
-
-                if self._logger:
-                    self._logger.debug(
-                        f'Dispatcher "{self.id}" received request: "{data.functionId}" -> task: "{data.taskId}"')
-
-                if callable(func):
-                    # Now we check, if we have to perform test, whether
-                    # we are allowed to execute the task:
-                    if data.get("target", self.id) != self.id:
-                        return
-
-                    # Define a list containing callbacks:
-                    cbs = []
-
-                    observer = None
-
-                    def on_cancel(reason, *args):
-                        nonlocal observer
-                        if reason.taskId == data.taskId:
-
-                            for cb in cbs:
-                                cb(reason)
-
-                            observer.unsubscribe()
-                            observer = None
-
-                    observer = self.onCancelTask.subscribe(on_cancel)
-
-                    # extract the arguments etc.
-                    # create an empty list and fill it afterwards
-                    args = [None] * (len(data.params) + len(data.callbacks))
-
-                    for item in data.params:
-                        args[item.idx] = item.data
-
-                    for optionsOfCallback in data.callbacks:
-
-                        async def callback(*args, id=optionsOfCallback.id, opts=optionsOfCallback, **kwargs):
-                            nonlocal cbs
-
-                            servicePromise = self.performCall(id, args, opts)
-
-                            def cancelCallback(reason):
-                                # The Main Task has been canceled =>
-                                # We are allowed to canel the Subtask as well.
-                                if servicePromise is not None and getattr(
-                                        servicePromise, 'cancelCallback', False):
-                                    servicePromise.cancelCallback(reason)
-
-                            idx = len(cbs)
-                            cbs.append(cancelCallback)
-
-                            # Await the Result. If an Task is canceled => The
-                            # Error is Thrown.
-                            result = await servicePromise
-
-                            # Remove the Index
-                            cbs.pop(idx)
-
-                            return result
-
-                        args[optionsOfCallback.idx] = callback
-
-                    # Perform the Task it self.
-                    _result = _DEFAULT_RESULT
-
-                    if not func.isAsync and not self.__warned and self._logger:
-                        self._logger.warn(
-                            "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                        self._logger.warn(
-                            "Offloading function to a separate thread.")
-                        # We only want to warn the user once.
-                        self.__warned = True
-
-                    resultPromise = func(*args)
-
-                    try:
-                        if resultPromise is not None and getattr(
-                                resultPromise, 'cancelCallback', False):
-                            def _cancel_main(reason):
-                                resultPromise.cancelCallback(reason)
-
-                            cbs.append(_cancel_main)
-
-                    except Exception as error:
-                        # The Cancel Function isn't available in
-                        # the provided promise.
-                        pass
-
-                    self._runningExternalRequestedTasks[data.taskId] = data.requestedBy
-
-                    # Wait for the Result to finish.
-                    _result = await resultPromise
-
-                    # Define the Result message
-                    result = {
-                        'result': _result if _result is not _DEFAULT_RESULT else None,
-                        'taskId': data.taskId,
-                        'type': 'response'
-                    }
-
-                    if self._logger:
-                        self._logger.debug(
-                            'Internally executed requested Function for Task: ' + str(data['taskId']) + " - Function \"" +
-                            data['functionId'] + '\". Sending result on ' + data['resultSink'])
-
-                    # Use the communicator to publish the result.
-                    await self._communicator.emit("rpcResponse", result)
-
-            except Exception as error:
-
-                if self._logger:
-                    self._logger.error(
-                        f'Dispatcher "{self.id}" failed with request: "{data.taskId}"')
-                    self._logger.error(formatException(error))
-                else:
-                    print(formatException(error))
-
-                self._runningExternalRequestedTasks.pop(data.requestedBy, None)
-
-                result = {
-                    'error': {
-                        'error': str(error),
-                        'msg': str(error)
-                    },
-                    'taskId': data.taskId,
-                    'type': 'response'
-                }
-
-                # Use the communicator to publish the result.
-                await self._communicator.emit("rpcResponse", result)
-
-        async def _performCall(self, serviceName, params, options=None):
-            optionsToUse = ensureDottedAccess({
-                "resultSink": self._getServiceName(serviceName, "response"),
-                "waitForResult": True,
-                "callbackOptions": [],
-                "timeToLifeAfterCall": self.defaultKeepAlive,
-                "calledOnce": [],
-            })
-            optionsToUse.update(ensureDottedAccess(options))
-
-            taskId = generateId()
-
-            _registeredCallbacks = []
-
-            # Create a Future of the Loop.
-            future = EXECUTOR.generatePromise(taskId=taskId)
-
-            def clear():
-                if taskId in self._runningInternalRequestedTasks:
-
-                    if self._logger:
-                        self._logger.debug('Clearing Callbacks from ' + taskId)
-
-                    for cb in _registeredCallbacks:
-                        EXECUTOR.callParallel(self.unregisterService, cb)
-
-                    task = self._runningInternalRequestedTasks[taskId]
-
-                    if task.timeout is not None:
-                        task.timeout.cancel()
-
-                    self._runningInternalRequestedTasks.pop(taskId)
-
-            try:
-                tastRequest = ensureDottedAccess({
-                    "future": future,
-                    "clear": clear,
-                    'serviceName': serviceName,
-                    'timeout': None,
-                })
-
-                # Store the Future as Task.
-                self._runningInternalRequestedTasks[taskId] = tastRequest
-
-                # Define the packet to send:
-                packet = {
-                    'functionId': serviceName,
-                    'params': [],
-                    'taskId': taskId,
-                    'resultSink': optionsToUse['resultSink'],
-                    'requestedBy': self._id,
-                    'target': None,
-                    'callbacks': []
-                }
-
-                callbackOptions = {
-                    item.idx: item for item in optionsToUse.callbackOptions}
-
-                # Iterate over all Parameters and
-                # Determin Callbacks. Based on the Parameter-
-                # Type assign it either to packet.params (
-                # for parsable Parameters) and packet.callbacks
-                # (for callback Parameters)
-                for idx, contentOfParameter in enumerate(params):
-                    if not callable(contentOfParameter):
-                        # The parameter isnt callable:
-                        packet['params'].append({
-                            'idx': idx,
-                            'data': contentOfParameter
-                        })
-                    else:
-
-                        if not self.__warned and not isAsyncFunction(
-                                contentOfParameter):
-                            if self._logger:
-                                self._logger.warn(
-                                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                                self._logger.warn(
-                                    f'The service of parameter {idx} is synchronous!')
-                            else:
-                                print(
-                                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
-                                print(
-                                    f'The service of parameter {idx} is synchronous!')
-                            # We only want to warn the user once.
-                            self.__warned = True
-
-                        _functionAsAsync = EXECUTOR.wrapFuncIfRequired(
-                            contentOfParameter)
-
-                        _timeToLifeAfterCall = callbackOptions.get(
-                            idx, {"timeToLifeAfterCall": optionsToUse.timeToLifeAfterCall})["timeToLifeAfterCall"]
-                        _calledOnce = callbackOptions.get(
-                            idx, {"calledOnce": idx in optionsToUse.calledOnce})["calledOnce"]
-
-                        # The Parameter is a Callback => store a
-                        # Description of the Callback and register
-                        # the callback inside of the Dispatcher
-
-                        _id = ""
-                        _timeout: asyncio.Task = None
-
-                        def removeCallback():
-                            nonlocal _id
-                            EXECUTOR.callParallel(self.unregisterService, _id)
-
-                        async def cbWithTimeout(*args, f=_functionAsAsync, t=_timeToLifeAfterCall, **kwargs):
-                            nonlocal _timeout
-
-                            if _timeout:
-                                _timeout.cancel()
-
-                            if t > 0:
-                                _timeout = EXECUTOR.setTimeout(
-                                    removeCallback, t)
-
-                            return await f(*args, **kwargs)
-
-                        async def cbOnce(*args, f=_functionAsAsync, **kwargs):
-
-                            res = await f(*args, **kwargs)
-                            await self.unregisterService(_id)
-                            return res
-
-                        if _timeToLifeAfterCall > 0:
-                            _timeout = EXECUTOR.setTimeout(
-                                removeCallback, _timeToLifeAfterCall)
-
-                        _func = await self.registerService(cbOnce if _calledOnce else cbWithTimeout, {
-                            "schema": {},
-                            "id": generateId(pre_string="callback")
-                        })
-
-                        # Assign the used id.
-                        _id = _func.id
-
-                        _registeredCallbacks.append(_func.id)
-
-                        # Register the Callback itself in the params object.
-                        packet['callbacks'].append(
-                            # Convert the Options to
-                            # Camel Case
-                            {
-                                "id": _id,
-                                "idx": idx
-                            }
-                        )
-
-                if not self.serviceExists(serviceName):
-                    error = Exception(
-                        f'No Service Provider known for "{serviceName}"')
-                    if self._logger:
-                        self._logger.error(
-                            f'No Service Provider known for "{serviceName}"')
-                        self._logger.error(formatException(error))
-
-                    raise error
-
-                if self.options.forceUsingSelectors or self.services.amountOf.get(
-                        serviceName, 0) > 1:
-
-                    optionsForSelector = ensureDottedAccess({
-                        "rpcManager": self,
-                        "serviceName": serviceName
-                    })
-
-                    if isinstance(optionsToUse.target, str):
-                        tastRequest.target = optionsToUse.target
-                    elif callable(optionsToUse.selector):
-                        tastRequest.target = await options.selector(optionsForSelector)
-                    elif isinstance(optionsToUse.selector, str):
-                        tastRequest.target = await self._defaultSelector(optionsForSelector)
-
-                else:
-                    tastRequest.target = list(
-                        self.services.keyMappingreverse[serviceName])[0]
-
-                packet["target"] = tastRequest.target
-
-                await self._communicator.emit("rpcRequest", packet)
-
-                if self._logger:
-                    self._logger.debug(
-                        f'Dispatcher "{self._id}" putting task "{taskId}" on: "{self._getServiceName(serviceName, "request")}"')
-
-                if optionsToUse.get("timeout", 0) > 0:
-                    async def onTimeout():
-                        await self.cancelTask(
-                            taskId,
-                            TimeoutError(
-                                f"TIMEOUT. The Service allowed execution time of {optionsToUse.timeout} [ms] has been excided")
-                        )
-
-                    # Create our timeout and store it.
-                    tastRequest.timeout = EXECUTOR.setTimeout(
-                        onTimeout, optionsToUse.timeout)
-
-            except Exception as err:
-                if self._logger:
-                    self._logger.error('Something went wrong on calling')
-                    self._logger.exception(formatException(err))
-                else:
-                    print(formatException(err))
-
-                # Call the Clear Function
-                clear()
-
-                # Throw an error.
-                future.set_exception(err)
-
-            # Define a Function, which could be used for cancelation.
-            def _cancelTask(reason):
-                EXECUTOR.callParallel(self.cancelTask, taskId, reason)
-
-            future.cancelCallback = _cancelTask
-
-            if not optionsToUse.waitForResult:
-                EXECUTOR.callParallel(future)
-                return future
-
-            return await future
-
-    class NopeConnectivityManager(conManagerMod.NopeConnectivityManager):
-        def _info(self):
-            ret = conManagerMod.NopeConnectivityManager._info(self)
-            ret.plugins.append("rpcCallbacks")
-            return ret
-
-    return NopeRpcManager, NopeConnectivityManager
+""" An example how to modify the Behavior of multiple elements using a Plugin.
+
+    In This case the Plugin allows the implementation of an ackknowledgement
+    message if required.
+"""
+
+import asyncio
+
+from nope.eventEmitter import NopeEventEmitter
+from nope.helpers import generateId, EXECUTOR, ensureDottedAccess, formatException, isAsyncFunction
+from nope.plugins import plugin
+
+_DEFAULT_RESULT = object()
+
+
+@plugin([
+    "nope.dispatcher.rpcManager",
+    "nope.dispatcher.connectivityManager"
+],
+    name="rpcCallbacks")
+def extend(rpcMod, conManagerMod):
+    "Extends the Bridge and adds the functionality of ack knowlededing messages."
+
+    class NopeRpcManager(rpcMod.NopeRpcManager):
+        def __init__(self, *args, **kwargs):
+            rpcMod.NopeRpcManager.__init__(self, *args, **kwargs)
+            self.defaultKeepAlive = kwargs.get(
+                "defaultKeepAlive", 60 * 60 * 1000)
+
+        async def _handleExternalRequest(self, data, func=None):
+            try:
+                if not callable(func):
+                    if data.functionId not in self._registeredServices:
+                        return
+                    func = self._registeredServices[data.functionId].get(
+                        "func", None)
+
+                if self._logger:
+                    self._logger.debug(
+                        f'Dispatcher "{self.id}" received request: "{data.functionId}" -> task: "{data.taskId}"')
+
+                if callable(func):
+                    # Now we check, if we have to perform test, whether
+                    # we are allowed to execute the task:
+                    if data.get("target", self.id) != self.id:
+                        return
+
+                    # Define a list containing callbacks:
+                    cbs = []
+
+                    observer = None
+
+                    def on_cancel(reason, *args):
+                        nonlocal observer
+                        if reason.taskId == data.taskId:
+
+                            for cb in cbs:
+                                cb(reason)
+
+                            observer.unsubscribe()
+                            observer = None
+
+                    observer = self.onCancelTask.subscribe(on_cancel)
+
+                    # extract the arguments etc.
+                    # create an empty list and fill it afterwards
+                    args = [None] * (len(data.params) + len(data.callbacks))
+
+                    for item in data.params:
+                        args[item.idx] = item.data
+
+                    for optionsOfCallback in data.callbacks:
+
+                        async def callback(*args, id=optionsOfCallback.id, opts=optionsOfCallback, **kwargs):
+                            nonlocal cbs
+
+                            servicePromise = self.performCall(id, args, opts)
+
+                            def cancelCallback(reason):
+                                # The Main Task has been canceled =>
+                                # We are allowed to canel the Subtask as well.
+                                if servicePromise is not None and getattr(
+                                        servicePromise, 'cancelCallback', False):
+                                    servicePromise.cancelCallback(reason)
+
+                            idx = len(cbs)
+                            cbs.append(cancelCallback)
+
+                            # Await the Result. If an Task is canceled => The
+                            # Error is Thrown.
+                            result = await servicePromise
+
+                            # Remove the Index
+                            cbs.pop(idx)
+
+                            return result
+
+                        args[optionsOfCallback.idx] = callback
+
+                    # Perform the Task it self.
+                    _result = _DEFAULT_RESULT
+
+                    if not func.isAsync and not self.__warned and self._logger:
+                        self._logger.warn(
+                            "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                        self._logger.warn(
+                            "Offloading function to a separate thread.")
+                        # We only want to warn the user once.
+                        self.__warned = True
+
+                    resultPromise = func(*args)
+
+                    try:
+                        if resultPromise is not None and getattr(
+                                resultPromise, 'cancelCallback', False):
+                            def _cancel_main(reason):
+                                resultPromise.cancelCallback(reason)
+
+                            cbs.append(_cancel_main)
+
+                    except Exception as error:
+                        # The Cancel Function isn't available in
+                        # the provided promise.
+                        pass
+
+                    self._runningExternalRequestedTasks[data.taskId] = data.requestedBy
+
+                    # Wait for the Result to finish.
+                    _result = await resultPromise
+
+                    # Define the Result message
+                    result = {
+                        'result': _result if _result is not _DEFAULT_RESULT else None,
+                        'taskId': data.taskId,
+                        'type': 'response'
+                    }
+
+                    if self._logger:
+                        self._logger.debug(
+                            'Internally executed requested Function for Task: ' + str(data['taskId']) + " - Function \"" +
+                            data['functionId'] + '\". Sending result on ' + data['resultSink'])
+
+                    # Use the communicator to publish the result.
+                    await self._communicator.emit("rpcResponse", result)
+
+            except Exception as error:
+
+                if self._logger:
+                    self._logger.error(
+                        f'Dispatcher "{self.id}" failed with request: "{data.taskId}"')
+                    self._logger.error(formatException(error))
+                else:
+                    print(formatException(error))
+
+                self._runningExternalRequestedTasks.pop(data.requestedBy, None)
+
+                result = {
+                    'error': {
+                        'error': str(error),
+                        'msg': str(error)
+                    },
+                    'taskId': data.taskId,
+                    'type': 'response'
+                }
+
+                # Use the communicator to publish the result.
+                await self._communicator.emit("rpcResponse", result)
+
+        async def _performCall(self, serviceName, params, options=None):
+            optionsToUse = ensureDottedAccess({
+                "resultSink": self._getServiceName(serviceName, "response"),
+                "waitForResult": True,
+                "callbackOptions": [],
+                "timeToLifeAfterCall": self.defaultKeepAlive,
+                "calledOnce": [],
+            })
+            optionsToUse.update(ensureDottedAccess(options))
+
+            taskId = generateId()
+
+            _registeredCallbacks = []
+
+            # Create a Future of the Loop.
+            future = EXECUTOR.generatePromise(taskId=taskId)
+
+            def clear():
+                if taskId in self._runningInternalRequestedTasks:
+
+                    if self._logger:
+                        self._logger.debug('Clearing Callbacks from ' + taskId)
+
+                    for cb in _registeredCallbacks:
+                        EXECUTOR.callParallel(self.unregisterService, cb)
+
+                    task = self._runningInternalRequestedTasks[taskId]
+
+                    if task.timeout is not None:
+                        task.timeout.cancel()
+
+                    self._runningInternalRequestedTasks.pop(taskId)
+
+            try:
+                tastRequest = ensureDottedAccess({
+                    "future": future,
+                    "clear": clear,
+                    'serviceName': serviceName,
+                    'timeout': None,
+                })
+
+                # Store the Future as Task.
+                self._runningInternalRequestedTasks[taskId] = tastRequest
+
+                # Define the packet to send:
+                packet = {
+                    'functionId': serviceName,
+                    'params': [],
+                    'taskId': taskId,
+                    'resultSink': optionsToUse['resultSink'],
+                    'requestedBy': self._id,
+                    'target': None,
+                    'callbacks': []
+                }
+
+                callbackOptions = {
+                    item.idx: item for item in optionsToUse.callbackOptions}
+
+                # Iterate over all Parameters and
+                # Determin Callbacks. Based on the Parameter-
+                # Type assign it either to packet.params (
+                # for parsable Parameters) and packet.callbacks
+                # (for callback Parameters)
+                for idx, contentOfParameter in enumerate(params):
+                    if not callable(contentOfParameter):
+                        # The parameter isnt callable:
+                        packet['params'].append({
+                            'idx': idx,
+                            'data': contentOfParameter
+                        })
+                    else:
+
+                        if not self.__warned and not isAsyncFunction(
+                                contentOfParameter):
+                            if self._logger:
+                                self._logger.warn(
+                                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                                self._logger.warn(
+                                    f'The service of parameter {idx} is synchronous!')
+                            else:
+                                print(
+                                    "!!! You have provided synchronous functions. They may break NoPE. Use them with care !!!")
+                                print(
+                                    f'The service of parameter {idx} is synchronous!')
+                            # We only want to warn the user once.
+                            self.__warned = True
+
+                        _functionAsAsync = EXECUTOR.wrapFuncIfRequired(
+                            contentOfParameter)
+
+                        _timeToLifeAfterCall = callbackOptions.get(
+                            idx, {"timeToLifeAfterCall": optionsToUse.timeToLifeAfterCall})["timeToLifeAfterCall"]
+                        _calledOnce = callbackOptions.get(
+                            idx, {"calledOnce": idx in optionsToUse.calledOnce})["calledOnce"]
+
+                        # The Parameter is a Callback => store a
+                        # Description of the Callback and register
+                        # the callback inside of the Dispatcher
+
+                        _id = ""
+                        _timeout: asyncio.Task = None
+
+                        def removeCallback():
+                            nonlocal _id
+                            EXECUTOR.callParallel(self.unregisterService, _id)
+
+                        async def cbWithTimeout(*args, f=_functionAsAsync, t=_timeToLifeAfterCall, **kwargs):
+                            nonlocal _timeout
+
+                            if _timeout:
+                                _timeout.cancel()
+
+                            if t > 0:
+                                _timeout = EXECUTOR.setTimeout(
+                                    removeCallback, t)
+
+                            return await f(*args, **kwargs)
+
+                        async def cbOnce(*args, f=_functionAsAsync, **kwargs):
+
+                            res = await f(*args, **kwargs)
+                            await self.unregisterService(_id)
+                            return res
+
+                        if _timeToLifeAfterCall > 0:
+                            _timeout = EXECUTOR.setTimeout(
+                                removeCallback, _timeToLifeAfterCall)
+
+                        _func = await self.registerService(cbOnce if _calledOnce else cbWithTimeout, {
+                            "schema": {},
+                            "id": generateId(pre_string="callback")
+                        })
+
+                        # Assign the used id.
+                        _id = _func.id
+
+                        _registeredCallbacks.append(_func.id)
+
+                        # Register the Callback itself in the params object.
+                        packet['callbacks'].append(
+                            # Convert the Options to
+                            # Camel Case
+                            {
+                                "id": _id,
+                                "idx": idx
+                            }
+                        )
+
+                if not self.serviceExists(serviceName):
+                    error = Exception(
+                        f'No Service Provider known for "{serviceName}"')
+                    if self._logger:
+                        self._logger.error(
+                            f'No Service Provider known for "{serviceName}"')
+                        self._logger.error(formatException(error))
+
+                    raise error
+
+                if self.options.forceUsingSelectors or self.services.amountOf.get(
+                        serviceName, 0) > 1:
+
+                    optionsForSelector = ensureDottedAccess({
+                        "rpcManager": self,
+                        "serviceName": serviceName
+                    })
+
+                    if isinstance(optionsToUse.target, str):
+                        tastRequest.target = optionsToUse.target
+                    elif callable(optionsToUse.selector):
+                        tastRequest.target = await options.selector(optionsForSelector)
+                    elif isinstance(optionsToUse.selector, str):
+                        tastRequest.target = await self._defaultSelector(optionsForSelector)
+
+                else:
+                    tastRequest.target = list(
+                        self.services.keyMappingreverse[serviceName])[0]
+
+                packet["target"] = tastRequest.target
+
+                await self._communicator.emit("rpcRequest", packet)
+
+                if self._logger:
+                    self._logger.debug(
+                        f'Dispatcher "{self._id}" putting task "{taskId}" on: "{self._getServiceName(serviceName, "request")}"')
+
+                if optionsToUse.get("timeout", 0) > 0:
+                    async def onTimeout():
+                        await self.cancelTask(
+                            taskId,
+                            TimeoutError(
+                                f"TIMEOUT. The Service allowed execution time of {optionsToUse.timeout} [ms] has been excided")
+                        )
+
+                    # Create our timeout and store it.
+                    tastRequest.timeout = EXECUTOR.setTimeout(
+                        onTimeout, optionsToUse.timeout)
+
+            except Exception as err:
+                if self._logger:
+                    self._logger.error('Something went wrong on calling')
+                    self._logger.exception(formatException(err))
+                else:
+                    print(formatException(err))
+
+                # Call the Clear Function
+                clear()
+
+                # Throw an error.
+                future.set_exception(err)
+
+            # Define a Function, which could be used for cancelation.
+            def _cancelTask(reason):
+                EXECUTOR.callParallel(self.cancelTask, taskId, reason)
+
+            future.cancelCallback = _cancelTask
+
+            if not optionsToUse.waitForResult:
+                EXECUTOR.callParallel(future)
+                return future
+
+            return await future
+
+    class NopeConnectivityManager(conManagerMod.NopeConnectivityManager):
+        def _info(self):
+            ret = conManagerMod.NopeConnectivityManager._info(self)
+            ret.plugins.append("rpcCallbacks")
+            return ret
+
+    return NopeRpcManager, NopeConnectivityManager
```

### Comparing `nope_py-1.7.8rc3/nope/pubSub/nopePubSubSystem.py` & `nope_py-1.7.9/nope/pubSub/nopePubSubSystem.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,651 +1,651 @@
-from ..eventEmitter import NopeEventEmitter
-from ..helpers import comparePatternAndPath, copy, generateId, DottedDict, ensureDottedAccess, rgetattr, \
-    containsWildcards, getTimestamp, isIterable, rsetattr, flattenObject
-from ..merging import DictBasedMergeData
-
-DEFAULT_OBJ = object()
-LAZY_UPDATE = True  # Way faster
-
-
-def _memoizedCompare(matchTopicsWithoutWildcards: bool):
-    """ Helper to memoize the
-
-    Args:
-        options (bool): Flag to match topics with or without a wildcard
-
-    Returns:
-        callable: a Function that stores the results.
-    """
-    cache = {}
-
-    def ret(pattern, path):
-        nonlocal cache
-        nonlocal matchTopicsWithoutWildcards
-
-        key = f'{pattern}-{path}'
-
-        if key not in cache:
-            cache[key] = comparePatternAndPath(pattern, path, {
-                'matchTopicsWithoutWildcards': matchTopicsWithoutWildcards
-            })
-
-        return cache[key]
-
-    return ret
-
-
-def _extractPubAndSubTopic(options: DottedDict):
-    """ Helper to extract the pub and sub topic based on the provided options
-
-    Args:
-        options (DottedDict): the emitter options
-
-    Returns:
-        subTopic, pubTopic: the strings.
-    """
-    pubTopic = None
-    if isinstance(options.topic, str):
-        pubTopic = options.topic
-    else:
-        pubTopic = options.topic.publish
-
-    subTopic = None
-    if isinstance(options.topic, str):
-        subTopic = options.topic
-    else:
-        subTopic = options.topic.subscribe
-
-    return subTopic, pubTopic
-
-
-class PubSubSystem:
-
-    def __init__(self, mqttPatternBasedSubscriptions=True, forwardChildData=True,
-                 forwardParentData=True, matchTopicsWithoutWildcards=True, **kwargs):
-
-        # Adapt the Options
-        self._options = ensureDottedAccess({
-            'mqttPatternBasedSubscriptions': mqttPatternBasedSubscriptions,
-            'forwardChildData': forwardChildData,
-            'forwardParentData': forwardParentData,
-            'matchTopicsWithoutWildcards': matchTopicsWithoutWildcards
-        })
-
-        self._sendCurrentDataOnSubscription = False
-        self.id = generateId()
-
-        self._emitters = dict()
-        self._emittersToObservers = dict()
-
-        self._matched = dict()
-        self._disposing = False
-
-        self._comparePatternAndPath = _memoizedCompare(self._options)
-        self.subscriptions = DictBasedMergeData(self._emitters, 'subTopic')
-        self.publishers = DictBasedMergeData(self._emitters, 'pubTopic')
-        self.onIncrementalDataChange = NopeEventEmitter()
-
-        self._data = ensureDottedAccess({}, useNoneAsDefaultValue=False)
-
-    @property
-    def options(self):
-        return self._options.copy()
-
-    def register(self, emitter, options):
-
-        options = ensureDottedAccess(options)
-
-        if options.topic is None:
-            raise Exception("A Topic must be provided")
-
-        if emitter not in self._emitters:
-            # Now we will assign the pub and sub topic.
-            # this is defined in the options.
-
-            pubTopic = None
-            if isinstance(options.topic, str):
-                pubTopic = options.topic
-            else:
-                pubTopic = options.topic.publish
-
-            subTopic = None
-            if isinstance(options.topic, str):
-                subTopic = options.topic
-            else:
-                subTopic = options.topic.subscribe
-
-            if options.mode is None or not ("publish" in options.mode):
-                pubTopic = False
-            if options.mode is None or not ("subscribe" in options.mode):
-                subTopic = False
-
-            observer = None
-            callback = None
-
-            if pubTopic:
-
-                def callbackToAssign(content, opts):
-                    # Internal Data-Update of the pub-sub-system
-                    # we wont push the data again. Otherwise, we
-                    # risk an recursive endloop.
-                    if opts.pubSubUpdate:
-                        return
-
-                    # We use this callback to forward the data into the system:
-                    self._pushData(pubTopic, pubTopic,
-                                   content, opts, False, emitter)
-
-                callback = callbackToAssign
-
-            # Register the emitter. This will be used during topic matching.
-            self._emitters[emitter] = ensureDottedAccess(
-                {'options': options, 'pubTopic': pubTopic, 'subTopic': subTopic, 'callback': callback,
-                 'observer': observer})
-
-            # Update the Matching Rules.
-            global LAZY_UPDATE
-            if (LAZY_UPDATE):
-                self._updatePartialMatching("add", emitter, pubTopic, subTopic)
-            else:
-                self.updateMatching()
-
-            if callback:
-                # If necessary. Add the Callback.
-                observer = emitter.subscribe(callback, ensureDottedAccess(
-                    {'skipCurrent': not self._sendCurrentDataOnSubscription}))
-                # Now lets store our binding.
-                self._emittersToObservers[emitter] = observer
-
-            if subTopic and self._sendCurrentDataOnSubscription:
-                if containsWildcards(subTopic):
-
-                    for item in self._patternbasedPullData(subTopic, None):
-                        # We check if the content is available
-                        if item.get("data", False):
-                            emitter.emit(
-                                item.data,
-                                ensureDottedAccess({
-                                    'sender': self.id,
-                                    'topicOfContent': item["path"],
-                                    'topicOfChange': item["path"],
-                                    'topicOfSubscription': subTopic
-                                })
-                            )
-                else:
-                    currentContent = self._pullData(subTopic, None)
-                    if currentContent is not None:
-                        emitter.emit(
-                            currentContent,
-                            ensureDottedAccess({
-                                'sender': self.id,
-                                'topicOfContent': subTopic,
-                                'topicOfChange': subTopic,
-                                'topicOfSubscription': subTopic
-                            })
-                        )
-        else:
-            raise Exception('Already registered Emitter!')
-        return emitter
-
-    def updateOptions(self, emitter, options):
-        # We will adapat the Options, for dotted access.
-        options = ensureDottedAccess(options)
-        if emitter in self._emitters:
-            subTopic, pubTopic = _extractPubAndSubTopic(options)
-            data = self._emitters.get(emitter)
-
-            if (LAZY_UPDATE):
-                self._updatePartialMatching(
-                    "remove",
-                    emitter,
-                    data.pubTopic,
-                    data.subTopic
-                )
-
-            data.options = options
-            data.subTopic = subTopic
-            data.pubTopic = pubTopic
-
-            self._emitters[emitter] = data
-
-            if (LAZY_UPDATE):
-                # Update the Matching Rules.
-                self._updatePartialMatching("add", emitter, pubTopic, subTopic)
-            else:
-                # Update the Matching Rules.
-                self.updateMatching()
-        else:
-            raise Exception('Emitter is not registered')
-
-    def unregister(self, emitter):
-        if emitter in self._emitters:
-            options = self._emitters.pop(emitter)
-            subTopic, pubTopic = _extractPubAndSubTopic(options["options"])
-
-            if (LAZY_UPDATE):
-                # Update the Matching Rules.
-                self._updatePartialMatching(
-                    "remove", emitter, pubTopic, subTopic)
-            else:
-                # Update the Matching Rules.
-                self.updateMatching()
-
-            return True
-        return False
-
-    def registerSubscription(self, topic, subscription):
-        emitter = NopeEventEmitter()
-        observer = emitter.subscribe(subscription)
-        self.register(emitter, {'mode': 'subscribe',
-                                'schema': {}, 'topic': topic})
-        return observer
-
-    @property
-    def emitters(self):
-        # TODO:
-        pass
-
-    def updateMatching(self):
-
-        self._matched.clear()
-
-        for item in self._emitters.values():
-            # Extract the publisher topic
-            pubTopic = item.get("pubTopic", False)
-
-            if pubTopic is not False:
-                self._updateMatchingForTopic(pubTopic)
-
-        self.subscriptions.update()
-        self.publishers.update()
-
-    def _addMatchingEntryIfRequired(self, pubTopic, subTopic, emitter):
-        result = self._comparePatternAndPath(subTopic, pubTopic)
-        if result.affected:
-            if not result.containsWildcards and ((result.affectedByChild and not self.options.forwardChildData) or
-                                                 (
-                result.affectedByParent and not self.options.forwardParentData)
-            ):
-                return
-
-            # We now have match the topic as following described:
-            # 1) subscription contains a pattern
-            #    - dircet change (same-level) => content
-            #    - parent based change => content
-            #    - child based change => content
-            # 2) subscription doesnt contains a pattern:
-            #    We more or less want the data on the path.
-            #    - direct change (topic = path) => content
-            #    - parent based change => a super change
-            if result.containsWildcards:
-                if self.options.mqttPatternBasedSubscriptions:
-                    if result.patternToExtractData is not False:
-                        self._addToMatchingStructure(
-                            'dataQuery', pubTopic, result.patternToExtractData, emitter)
-                    elif result.pathToExtractData is not False:
-                        self._addToMatchingStructure(
-                            'dataPull', pubTopic, result.pathToExtractData, emitter)
-                    else:
-                        raise Exception(
-                            'Implementation Error. Either the patternToExtractData or the pathToExtractData must be provided')
-                else:
-                    self._addToMatchingStructure(
-                        'dataQuery', pubTopic, pubTopic, emitter)
-            else:
-                if result.affectedByChild and not self.options.forwardChildData or result.affectedByParent and not self.options.forwardParentData:
-                    return
-                if result.pathToExtractData is not False:
-                    self._addToMatchingStructure(
-                        'dataPull', pubTopic, result.pathToExtractData, emitter)
-                else:
-                    raise Exception(
-                        "Implementation Error. The 'pathToExtractData' must be provided")
-
-    def __deleteMatchingEntry(self, _pubTopic: str, _subTopic: str, _emitter):
-        if _pubTopic in self._matched:
-            data = self._matched[_pubTopic]
-
-            if _subTopic in data.dataPull:
-                data.dataPull[_subTopic].remove(_emitter)
-
-            if _subTopic in data.dataQuery:
-                data.dataQuery[_subTopic].remove(_emitter)
-
-    def __addMatchingEntryIfRequired(self, pubTopic, subTopic, emitter):
-        # Now lets determine the Path
-        result = self._comparePatternAndPath(subTopic, pubTopic)
-
-        if (result.affected):
-            # We skip content related to the settings.
-            # If no wildcard and no forwardChildData or forwardParentData
-            # is allowed ==> we make shure, that we skip the topic.
-            if not result.containsWildcards and ((result.affectedByChild and not self._options.forwardChildData) or (
-                    result.affectedByParent and not self._options.forwardParentData)):
-                return
-
-            # We now have match the topic as following described:
-            # 1) subscription contains a pattern
-            #    - dircet change (same-level) => content
-            #    - parent based change => content
-            #    - child based change => content
-            # 2) subscription doesnt contains a pattern:
-            #    We more or less want the data on the path.
-            #    - direct change (topic = path) => content
-            #    - parent based change => a super change
-            if result.containsWildcards:
-                if self._options.mqttPatternBasedSubscriptions:
-                    if result.patternToExtractData:
-                        self._addToMatchingStructure(
-                            "dataQuery",
-                            pubTopic,
-                            result.patternToExtractData,
-                            emitter
-                        )
-                    elif isinstance(result.pathToExtractData, str):
-                        self._addToMatchingStructure(
-                            "dataPull",
-                            pubTopic,
-                            result.pathToExtractData,
-                            emitter
-                        )
-                    else:
-                        raise Exception(
-                            "Implementation Error. Either the patternToExtractData or the pathToExtractData must be provided")
-                else:
-                    self._addToMatchingStructure(
-                        "dataQuery",
-                        pubTopic,
-                        pubTopic,
-                        emitter
-                    )
-            else:
-                # We skip content related to the settings.
-                # If no wildcard and no forwardChildData or forwardParentData
-                # is allowed ==> we make shure, that we skip the topic.
-                if (result.affectedByChild and not self._options.forwardChildData) or (
-                        result.affectedByParent and not self._options.forwardParentData):
-                    return
-
-                if isinstance(result.pathToExtractData, str):
-                    self._addToMatchingStructure(
-                        "dataPull",
-                        pubTopic,
-                        result.pathToExtractData,
-                        emitter
-                    )
-                else:
-                    raise Exception(
-                        "Implementation Error. The 'pathToExtractData' must be provided")
-
-    def _updatePartialMatching(
-            self, mode: str, _emitter, _pubTopic: str | bool, _subTopic: str | bool):
-        consideredPublishedTopics = set()
-
-        if _subTopic is not False:
-            # Iterate through all Publishers and
-            for item in self._emitters.values():
-                # Extract the Pub-Topic
-                pubTopicOfOtherEmitter = item.pubTopic
-
-                if pubTopicOfOtherEmitter is not False and not (
-                        pubTopicOfOtherEmitter in consideredPublishedTopics):
-                    # Now, lets Update the Matching for the specific Topics.
-                    if (mode == "remove"):
-                        self.__deleteMatchingEntry(
-                            pubTopicOfOtherEmitter,
-                            _subTopic,
-                            _emitter
-                        )
-                    elif (mode == "add"):
-                        self.__addMatchingEntryIfRequired(
-                            pubTopicOfOtherEmitter,
-                            _subTopic,
-                            _emitter
-                        )
-
-                # Add this topic to the topics,
-                # that have already been checked.
-                consideredPublishedTopics.add(pubTopicOfOtherEmitter)
-
-            # Additionally, we test for the allready published events:
-            for topic in self._matched.keys():
-                # we only test already published topics:
-                if not topic in consideredPublishedTopics and not containsWildcards(
-                        topic):
-
-                    if (mode == "remove"):
-                        self.__deleteMatchingEntry(topic, _subTopic, _emitter)
-                    elif (mode == "add"):
-                        self.__addMatchingEntryIfRequired(
-                            topic, _subTopic, _emitter)
-
-                    consideredPublishedTopics.add(topic)
-
-        if (mode == "add"):
-            if (_pubTopic is not False):
-                self._updateMatchingForTopic(_pubTopic)
-
-        if (_subTopic is not False and not containsWildcards(_subTopic)):
-            self.__addMatchingEntryIfRequired(_subTopic, _subTopic, _emitter)
-
-        elif (mode == "remove"):
-            if (_subTopic is not False):
-                self.__deleteMatchingEntry(_subTopic, _subTopic, _emitter)
-
-        self.publishers.update()
-        self.subscriptions.update()
-
-    def emit(self, eventName, data, options=None):
-        return self._pushData(eventName, eventName, data,
-                              ensureDottedAccess(options))
-
-    async def dispose(self):
-        self._disposing = True
-
-        for emitter in self._emitters:
-            self.unregister(emitter)
-
-        self.onIncrementalDataChange.dispose()
-        self.publishers.dispose()
-        self.subscriptions.dispose()
-
-    def _addToMatchingStructure(
-            self, entry, topicOfChange, path_or_pattern, emitter):
-        if topicOfChange not in self._matched:
-            self._matched[topicOfChange] = ensureDottedAccess(
-                {'dataPull': {}, 'dataQuery': {}})
-        if path_or_pattern not in self._matched[topicOfChange][entry]:
-            self._matched[topicOfChange][entry][path_or_pattern] = set()
-
-        self._matched.get(topicOfChange)[entry].get(
-            path_or_pattern).add(emitter)
-
-    def _updateMatchingForTopic(self, topicOfChange):
-        if topicOfChange not in self._matched:
-            self._matched[topicOfChange] = ensureDottedAccess(
-                {
-                    'dataPull': {},
-                    'dataQuery': {}
-                }
-            )
-
-        # Find all matches
-        for emitter, item in self._emitters.items():
-            if item.subTopic is not False:
-                self._addMatchingEntryIfRequired(
-                    topicOfChange, item.subTopic, emitter)
-
-    def _notify(self, topicOfContent: str, topicOfChange: str,
-                options, emitterCausingUpdate=None):
-        """ Internal Function to _notify all subscribers
-
-        Args:
-            topicOfContent (str): _description_
-            topicOfChange (str): _description_
-            options (dict-like): _description_
-            _emitter (Emitter, optional): _description_. Defaults to None.
-        """
-        if self._disposing:
-            return
-
-        # Check whether a Matching exists for this
-        # Topic, if not add it.
-        if topicOfContent not in self._matched:
-            self._updateMatchingForTopic(topicOfContent)
-
-        referenceToMatch = self._matched[topicOfContent]
-
-        for path_to_pull, emitters in referenceToMatch.dataPull.items():
-
-            for emitter in emitters:
-                # Only if we want to _notify an exclusive emitter we
-                # have to continue, if our emitter isnt matched.
-                if emitterCausingUpdate is not None and emitterCausingUpdate == emitter:
-                    continue
-
-                data = self._pullData(path_to_pull, None)
-
-                emitter.emit(
-                    data,
-                    ensureDottedAccess({
-                        **options,
-                        'topicOfChange': topicOfChange,
-                        'topicOfContent': topicOfContent,
-                        'topicOfSubscription': self._emitters[emitter].subTopic
-                    })
-                )
-
-        for pattern, emitters in referenceToMatch.dataQuery.items():
-
-            # Get a copy of the filtered items.
-            data = self._pullData(pattern, None)
-
-            # Filter the items.
-            data = filter(
-                lambda item: self._comparePatternAndPath(
-                    topicOfChange, item.path).affected, data)
-
-            if len(data) > 0:
-
-                for emitter in emitters:
-                    if emitter is not None and emitterCausingUpdate == emitter:
-                        continue
-
-                    emitter.emit(
-                        data,
-                        ensureDottedAccess({
-                            **options,
-                            'mode': 'direct',
-                            'topicOfChange': topicOfChange,
-                            'topicOfContent': topicOfContent,
-                            'topicOfSubscription': self._emitters.get(emitter).subTopic
-                        })
-                    )
-
-    def _updateOptions(self, options):
-        if not options.timestamp:
-            options.timestamp = getTimestamp()
-        if not isinstance(options.forced, bool):
-            options.forced = False
-        if not isIterable(options.args):
-            options.args = []
-        if not options.sender:
-            options.sender = self.id
-        return options
-
-    def _pushData(self, pathOfContent: str, pathOfChange: str,
-                  data, options={}, quiet=False, emitter=None):
-        """ Internal helper to push data to the data property. This results in informing the subscribers.
-
-        Args:
-            pathOfContent (str): Path, that is used for pushing the data.
-            pathOfChange (str): The path, which caused the change.
-            data (any): The data to push
-            options (dict, optional): Options used during pushing. Defaults to {}.
-            quiet (bool, optional): _description_. Defaults to False.
-            emitter (_type_, optional): _description_. Defaults to None.
-        """
-
-        options = self._updateOptions(options)
-        options.pubSubUpdate = True
-        if containsWildcards(pathOfContent):
-            raise 'The Path contains wildcards. Please use the method "patternbasedPullData" instead'
-        elif pathOfContent == '':
-            self._data = copy(data)
-            self._notify(pathOfContent, pathOfChange, options, emitter)
-        else:
-            rsetattr(self._data, pathOfContent, copy(data))
-            self._notify(pathOfContent, pathOfChange, options, emitter)
-        if not quiet:
-            self.onIncrementalDataChange.emit(ensureDottedAccess({
-                'path': pathOfContent,
-                'data': data,
-                **options
-            }))
-
-    def _pullData(self, topic, default=None):
-        if containsWildcards(topic):
-            raise 'The Path contains wildcards. Please use the method "patternbasedPullData" instead'
-        return copy(rgetattr(self._data, topic, default))
-
-    def _patternbasedPullData(self, pattern: str, default=None):
-        """ Helper, which enable to perform a pattern based pull.
-            The code receives a pattern, and matches the existing content
-            (by using there path attributes) and return the corresponding data.
-
-        Args:
-            pattern (str): the pattern
-            default (any, optional): The default-value. Defaults to None.
-
-        Returns:
-            list:
-        """
-
-        # To extract the data based on a Pattern,
-        # we firstly, we check if the given pattern
-        # is a pattern.
-        if not containsWildcards(pattern):
-            # Its not a pattern so we will speed up
-            # things.
-            global DEFAULT_OBJ
-            data = self._pullData(pattern, DEFAULT_OBJ)
-
-            if data is not DEFAULT_OBJ:
-                return [
-                    ensureDottedAccess({
-                        'path': pattern,
-                        'data': data
-                    })
-                ]
-            elif default is not None:
-                return [
-                    ensureDottedAccess({
-                        'path': pattern,
-                        'data': default
-                    })
-                ]
-
-            return []
-
-        # Now we know, we have to work with the query,
-        # for that purpose, we will adapt the data object
-        # to the following form:
-        # {path: value}
-        flatten = flattenObject(self._data)
-        ret = []
-
-        # We will use our alternative representation of the
-        # object to compare the pattern with the path item.
-        # only if there is a direct match => we will extract it.
-        # That corresponds to a direct level extraction and
-        # prevents to grap multiple items.
-        for path, data in flatten.items():
-            result = self._comparePatternAndPath(pattern, path)
-            if result.affectedOnSameLevel or result.affectedByChild:
-                ret.append(ensureDottedAccess({
-                    'path': path,
-                    'data': data
-                }))
-
-        # Now we just return our created element.
-        return ret
+from ..eventEmitter import NopeEventEmitter
+from ..helpers import comparePatternAndPath, copy, generateId, DottedDict, ensureDottedAccess, rgetattr, \
+    containsWildcards, getTimestamp, isIterable, rsetattr, flattenObject
+from ..merging import DictBasedMergeData
+
+DEFAULT_OBJ = object()
+LAZY_UPDATE = True  # Way faster
+
+
+def _memoizedCompare(matchTopicsWithoutWildcards: bool):
+    """ Helper to memoize the
+
+    Args:
+        options (bool): Flag to match topics with or without a wildcard
+
+    Returns:
+        callable: a Function that stores the results.
+    """
+    cache = {}
+
+    def ret(pattern, path):
+        nonlocal cache
+        nonlocal matchTopicsWithoutWildcards
+
+        key = f'{pattern}-{path}'
+
+        if key not in cache:
+            cache[key] = comparePatternAndPath(pattern, path, {
+                'matchTopicsWithoutWildcards': matchTopicsWithoutWildcards
+            })
+
+        return cache[key]
+
+    return ret
+
+
+def _extractPubAndSubTopic(options: DottedDict):
+    """ Helper to extract the pub and sub topic based on the provided options
+
+    Args:
+        options (DottedDict): the emitter options
+
+    Returns:
+        subTopic, pubTopic: the strings.
+    """
+    pubTopic = None
+    if isinstance(options.topic, str):
+        pubTopic = options.topic
+    else:
+        pubTopic = options.topic.publish
+
+    subTopic = None
+    if isinstance(options.topic, str):
+        subTopic = options.topic
+    else:
+        subTopic = options.topic.subscribe
+
+    return subTopic, pubTopic
+
+
+class PubSubSystem:
+
+    def __init__(self, mqttPatternBasedSubscriptions=True, forwardChildData=True,
+                 forwardParentData=True, matchTopicsWithoutWildcards=True, **kwargs):
+
+        # Adapt the Options
+        self._options = ensureDottedAccess({
+            'mqttPatternBasedSubscriptions': mqttPatternBasedSubscriptions,
+            'forwardChildData': forwardChildData,
+            'forwardParentData': forwardParentData,
+            'matchTopicsWithoutWildcards': matchTopicsWithoutWildcards
+        })
+
+        self._sendCurrentDataOnSubscription = False
+        self.id = generateId()
+
+        self._emitters = dict()
+        self._emittersToObservers = dict()
+
+        self._matched = dict()
+        self._disposing = False
+
+        self._comparePatternAndPath = _memoizedCompare(self._options)
+        self.subscriptions = DictBasedMergeData(self._emitters, 'subTopic')
+        self.publishers = DictBasedMergeData(self._emitters, 'pubTopic')
+        self.onIncrementalDataChange = NopeEventEmitter()
+
+        self._data = ensureDottedAccess({}, useNoneAsDefaultValue=False)
+
+    @property
+    def options(self):
+        return self._options.copy()
+
+    def register(self, emitter, options):
+
+        options = ensureDottedAccess(options)
+
+        if options.topic is None:
+            raise Exception("A Topic must be provided")
+
+        if emitter not in self._emitters:
+            # Now we will assign the pub and sub topic.
+            # this is defined in the options.
+
+            pubTopic = None
+            if isinstance(options.topic, str):
+                pubTopic = options.topic
+            else:
+                pubTopic = options.topic.publish
+
+            subTopic = None
+            if isinstance(options.topic, str):
+                subTopic = options.topic
+            else:
+                subTopic = options.topic.subscribe
+
+            if options.mode is None or not ("publish" in options.mode):
+                pubTopic = False
+            if options.mode is None or not ("subscribe" in options.mode):
+                subTopic = False
+
+            observer = None
+            callback = None
+
+            if pubTopic:
+
+                def callbackToAssign(content, opts):
+                    # Internal Data-Update of the pub-sub-system
+                    # we wont push the data again. Otherwise, we
+                    # risk an recursive endloop.
+                    if opts.pubSubUpdate:
+                        return
+
+                    # We use this callback to forward the data into the system:
+                    self._pushData(pubTopic, pubTopic,
+                                   content, opts, False, emitter)
+
+                callback = callbackToAssign
+
+            # Register the emitter. This will be used during topic matching.
+            self._emitters[emitter] = ensureDottedAccess(
+                {'options': options, 'pubTopic': pubTopic, 'subTopic': subTopic, 'callback': callback,
+                 'observer': observer})
+
+            # Update the Matching Rules.
+            global LAZY_UPDATE
+            if (LAZY_UPDATE):
+                self._updatePartialMatching("add", emitter, pubTopic, subTopic)
+            else:
+                self.updateMatching()
+
+            if callback:
+                # If necessary. Add the Callback.
+                observer = emitter.subscribe(callback, ensureDottedAccess(
+                    {'skipCurrent': not self._sendCurrentDataOnSubscription}))
+                # Now lets store our binding.
+                self._emittersToObservers[emitter] = observer
+
+            if subTopic and self._sendCurrentDataOnSubscription:
+                if containsWildcards(subTopic):
+
+                    for item in self._patternbasedPullData(subTopic, None):
+                        # We check if the content is available
+                        if item.get("data", False):
+                            emitter.emit(
+                                item.data,
+                                ensureDottedAccess({
+                                    'sender': self.id,
+                                    'topicOfContent': item["path"],
+                                    'topicOfChange': item["path"],
+                                    'topicOfSubscription': subTopic
+                                })
+                            )
+                else:
+                    currentContent = self._pullData(subTopic, None)
+                    if currentContent is not None:
+                        emitter.emit(
+                            currentContent,
+                            ensureDottedAccess({
+                                'sender': self.id,
+                                'topicOfContent': subTopic,
+                                'topicOfChange': subTopic,
+                                'topicOfSubscription': subTopic
+                            })
+                        )
+        else:
+            raise Exception('Already registered Emitter!')
+        return emitter
+
+    def updateOptions(self, emitter, options):
+        # We will adapat the Options, for dotted access.
+        options = ensureDottedAccess(options)
+        if emitter in self._emitters:
+            subTopic, pubTopic = _extractPubAndSubTopic(options)
+            data = self._emitters.get(emitter)
+
+            if (LAZY_UPDATE):
+                self._updatePartialMatching(
+                    "remove",
+                    emitter,
+                    data.pubTopic,
+                    data.subTopic
+                )
+
+            data.options = options
+            data.subTopic = subTopic
+            data.pubTopic = pubTopic
+
+            self._emitters[emitter] = data
+
+            if (LAZY_UPDATE):
+                # Update the Matching Rules.
+                self._updatePartialMatching("add", emitter, pubTopic, subTopic)
+            else:
+                # Update the Matching Rules.
+                self.updateMatching()
+        else:
+            raise Exception('Emitter is not registered')
+
+    def unregister(self, emitter):
+        if emitter in self._emitters:
+            options = self._emitters.pop(emitter)
+            subTopic, pubTopic = _extractPubAndSubTopic(options["options"])
+
+            if (LAZY_UPDATE):
+                # Update the Matching Rules.
+                self._updatePartialMatching(
+                    "remove", emitter, pubTopic, subTopic)
+            else:
+                # Update the Matching Rules.
+                self.updateMatching()
+
+            return True
+        return False
+
+    def registerSubscription(self, topic, subscription):
+        emitter = NopeEventEmitter()
+        observer = emitter.subscribe(subscription)
+        self.register(emitter, {'mode': 'subscribe',
+                                'schema': {}, 'topic': topic})
+        return observer
+
+    @property
+    def emitters(self):
+        # TODO:
+        pass
+
+    def updateMatching(self):
+
+        self._matched.clear()
+
+        for item in self._emitters.values():
+            # Extract the publisher topic
+            pubTopic = item.get("pubTopic", False)
+
+            if pubTopic is not False:
+                self._updateMatchingForTopic(pubTopic)
+
+        self.subscriptions.update()
+        self.publishers.update()
+
+    def _addMatchingEntryIfRequired(self, pubTopic, subTopic, emitter):
+        result = self._comparePatternAndPath(subTopic, pubTopic)
+        if result.affected:
+            if not result.containsWildcards and ((result.affectedByChild and not self.options.forwardChildData) or
+                                                 (
+                result.affectedByParent and not self.options.forwardParentData)
+            ):
+                return
+
+            # We now have match the topic as following described:
+            # 1) subscription contains a pattern
+            #    - dircet change (same-level) => content
+            #    - parent based change => content
+            #    - child based change => content
+            # 2) subscription doesnt contains a pattern:
+            #    We more or less want the data on the path.
+            #    - direct change (topic = path) => content
+            #    - parent based change => a super change
+            if result.containsWildcards:
+                if self.options.mqttPatternBasedSubscriptions:
+                    if result.patternToExtractData is not False:
+                        self._addToMatchingStructure(
+                            'dataQuery', pubTopic, result.patternToExtractData, emitter)
+                    elif result.pathToExtractData is not False:
+                        self._addToMatchingStructure(
+                            'dataPull', pubTopic, result.pathToExtractData, emitter)
+                    else:
+                        raise Exception(
+                            'Implementation Error. Either the patternToExtractData or the pathToExtractData must be provided')
+                else:
+                    self._addToMatchingStructure(
+                        'dataQuery', pubTopic, pubTopic, emitter)
+            else:
+                if result.affectedByChild and not self.options.forwardChildData or result.affectedByParent and not self.options.forwardParentData:
+                    return
+                if result.pathToExtractData is not False:
+                    self._addToMatchingStructure(
+                        'dataPull', pubTopic, result.pathToExtractData, emitter)
+                else:
+                    raise Exception(
+                        "Implementation Error. The 'pathToExtractData' must be provided")
+
+    def __deleteMatchingEntry(self, _pubTopic: str, _subTopic: str, _emitter):
+        if _pubTopic in self._matched:
+            data = self._matched[_pubTopic]
+
+            if _subTopic in data.dataPull:
+                data.dataPull[_subTopic].remove(_emitter)
+
+            if _subTopic in data.dataQuery:
+                data.dataQuery[_subTopic].remove(_emitter)
+
+    def __addMatchingEntryIfRequired(self, pubTopic, subTopic, emitter):
+        # Now lets determine the Path
+        result = self._comparePatternAndPath(subTopic, pubTopic)
+
+        if (result.affected):
+            # We skip content related to the settings.
+            # If no wildcard and no forwardChildData or forwardParentData
+            # is allowed ==> we make shure, that we skip the topic.
+            if not result.containsWildcards and ((result.affectedByChild and not self._options.forwardChildData) or (
+                    result.affectedByParent and not self._options.forwardParentData)):
+                return
+
+            # We now have match the topic as following described:
+            # 1) subscription contains a pattern
+            #    - dircet change (same-level) => content
+            #    - parent based change => content
+            #    - child based change => content
+            # 2) subscription doesnt contains a pattern:
+            #    We more or less want the data on the path.
+            #    - direct change (topic = path) => content
+            #    - parent based change => a super change
+            if result.containsWildcards:
+                if self._options.mqttPatternBasedSubscriptions:
+                    if result.patternToExtractData:
+                        self._addToMatchingStructure(
+                            "dataQuery",
+                            pubTopic,
+                            result.patternToExtractData,
+                            emitter
+                        )
+                    elif isinstance(result.pathToExtractData, str):
+                        self._addToMatchingStructure(
+                            "dataPull",
+                            pubTopic,
+                            result.pathToExtractData,
+                            emitter
+                        )
+                    else:
+                        raise Exception(
+                            "Implementation Error. Either the patternToExtractData or the pathToExtractData must be provided")
+                else:
+                    self._addToMatchingStructure(
+                        "dataQuery",
+                        pubTopic,
+                        pubTopic,
+                        emitter
+                    )
+            else:
+                # We skip content related to the settings.
+                # If no wildcard and no forwardChildData or forwardParentData
+                # is allowed ==> we make shure, that we skip the topic.
+                if (result.affectedByChild and not self._options.forwardChildData) or (
+                        result.affectedByParent and not self._options.forwardParentData):
+                    return
+
+                if isinstance(result.pathToExtractData, str):
+                    self._addToMatchingStructure(
+                        "dataPull",
+                        pubTopic,
+                        result.pathToExtractData,
+                        emitter
+                    )
+                else:
+                    raise Exception(
+                        "Implementation Error. The 'pathToExtractData' must be provided")
+
+    def _updatePartialMatching(
+            self, mode: str, _emitter, _pubTopic: str | bool, _subTopic: str | bool):
+        consideredPublishedTopics = set()
+
+        if _subTopic is not False:
+            # Iterate through all Publishers and
+            for item in self._emitters.values():
+                # Extract the Pub-Topic
+                pubTopicOfOtherEmitter = item.pubTopic
+
+                if pubTopicOfOtherEmitter is not False and not (
+                        pubTopicOfOtherEmitter in consideredPublishedTopics):
+                    # Now, lets Update the Matching for the specific Topics.
+                    if (mode == "remove"):
+                        self.__deleteMatchingEntry(
+                            pubTopicOfOtherEmitter,
+                            _subTopic,
+                            _emitter
+                        )
+                    elif (mode == "add"):
+                        self.__addMatchingEntryIfRequired(
+                            pubTopicOfOtherEmitter,
+                            _subTopic,
+                            _emitter
+                        )
+
+                # Add this topic to the topics,
+                # that have already been checked.
+                consideredPublishedTopics.add(pubTopicOfOtherEmitter)
+
+            # Additionally, we test for the allready published events:
+            for topic in self._matched.keys():
+                # we only test already published topics:
+                if not topic in consideredPublishedTopics and not containsWildcards(
+                        topic):
+
+                    if (mode == "remove"):
+                        self.__deleteMatchingEntry(topic, _subTopic, _emitter)
+                    elif (mode == "add"):
+                        self.__addMatchingEntryIfRequired(
+                            topic, _subTopic, _emitter)
+
+                    consideredPublishedTopics.add(topic)
+
+        if (mode == "add"):
+            if (_pubTopic is not False):
+                self._updateMatchingForTopic(_pubTopic)
+
+        if (_subTopic is not False and not containsWildcards(_subTopic)):
+            self.__addMatchingEntryIfRequired(_subTopic, _subTopic, _emitter)
+
+        elif (mode == "remove"):
+            if (_subTopic is not False):
+                self.__deleteMatchingEntry(_subTopic, _subTopic, _emitter)
+
+        self.publishers.update()
+        self.subscriptions.update()
+
+    def emit(self, eventName, data, options=None):
+        return self._pushData(eventName, eventName, data,
+                              ensureDottedAccess(options))
+
+    async def dispose(self):
+        self._disposing = True
+
+        for emitter in self._emitters:
+            self.unregister(emitter)
+
+        self.onIncrementalDataChange.dispose()
+        self.publishers.dispose()
+        self.subscriptions.dispose()
+
+    def _addToMatchingStructure(
+            self, entry, topicOfChange, path_or_pattern, emitter):
+        if topicOfChange not in self._matched:
+            self._matched[topicOfChange] = ensureDottedAccess(
+                {'dataPull': {}, 'dataQuery': {}})
+        if path_or_pattern not in self._matched[topicOfChange][entry]:
+            self._matched[topicOfChange][entry][path_or_pattern] = set()
+
+        self._matched.get(topicOfChange)[entry].get(
+            path_or_pattern).add(emitter)
+
+    def _updateMatchingForTopic(self, topicOfChange):
+        if topicOfChange not in self._matched:
+            self._matched[topicOfChange] = ensureDottedAccess(
+                {
+                    'dataPull': {},
+                    'dataQuery': {}
+                }
+            )
+
+        # Find all matches
+        for emitter, item in self._emitters.items():
+            if item.subTopic is not False:
+                self._addMatchingEntryIfRequired(
+                    topicOfChange, item.subTopic, emitter)
+
+    def _notify(self, topicOfContent: str, topicOfChange: str,
+                options, emitterCausingUpdate=None):
+        """ Internal Function to _notify all subscribers
+
+        Args:
+            topicOfContent (str): _description_
+            topicOfChange (str): _description_
+            options (dict-like): _description_
+            _emitter (Emitter, optional): _description_. Defaults to None.
+        """
+        if self._disposing:
+            return
+
+        # Check whether a Matching exists for this
+        # Topic, if not add it.
+        if topicOfContent not in self._matched:
+            self._updateMatchingForTopic(topicOfContent)
+
+        referenceToMatch = self._matched[topicOfContent]
+
+        for path_to_pull, emitters in referenceToMatch.dataPull.items():
+
+            for emitter in emitters:
+                # Only if we want to _notify an exclusive emitter we
+                # have to continue, if our emitter isnt matched.
+                if emitterCausingUpdate is not None and emitterCausingUpdate == emitter:
+                    continue
+
+                data = self._pullData(path_to_pull, None)
+
+                emitter.emit(
+                    data,
+                    ensureDottedAccess({
+                        **options,
+                        'topicOfChange': topicOfChange,
+                        'topicOfContent': topicOfContent,
+                        'topicOfSubscription': self._emitters[emitter].subTopic
+                    })
+                )
+
+        for pattern, emitters in referenceToMatch.dataQuery.items():
+
+            # Get a copy of the filtered items.
+            data = self._pullData(pattern, None)
+
+            # Filter the items.
+            data = filter(
+                lambda item: self._comparePatternAndPath(
+                    topicOfChange, item.path).affected, data)
+
+            if len(data) > 0:
+
+                for emitter in emitters:
+                    if emitter is not None and emitterCausingUpdate == emitter:
+                        continue
+
+                    emitter.emit(
+                        data,
+                        ensureDottedAccess({
+                            **options,
+                            'mode': 'direct',
+                            'topicOfChange': topicOfChange,
+                            'topicOfContent': topicOfContent,
+                            'topicOfSubscription': self._emitters.get(emitter).subTopic
+                        })
+                    )
+
+    def _updateOptions(self, options):
+        if not options.timestamp:
+            options.timestamp = getTimestamp()
+        if not isinstance(options.forced, bool):
+            options.forced = False
+        if not isIterable(options.args):
+            options.args = []
+        if not options.sender:
+            options.sender = self.id
+        return options
+
+    def _pushData(self, pathOfContent: str, pathOfChange: str,
+                  data, options={}, quiet=False, emitter=None):
+        """ Internal helper to push data to the data property. This results in informing the subscribers.
+
+        Args:
+            pathOfContent (str): Path, that is used for pushing the data.
+            pathOfChange (str): The path, which caused the change.
+            data (any): The data to push
+            options (dict, optional): Options used during pushing. Defaults to {}.
+            quiet (bool, optional): _description_. Defaults to False.
+            emitter (_type_, optional): _description_. Defaults to None.
+        """
+
+        options = self._updateOptions(options)
+        options.pubSubUpdate = True
+        if containsWildcards(pathOfContent):
+            raise 'The Path contains wildcards. Please use the method "patternbasedPullData" instead'
+        elif pathOfContent == '':
+            self._data = copy(data)
+            self._notify(pathOfContent, pathOfChange, options, emitter)
+        else:
+            rsetattr(self._data, pathOfContent, copy(data))
+            self._notify(pathOfContent, pathOfChange, options, emitter)
+        if not quiet:
+            self.onIncrementalDataChange.emit(ensureDottedAccess({
+                'path': pathOfContent,
+                'data': data,
+                **options
+            }))
+
+    def _pullData(self, topic, default=None):
+        if containsWildcards(topic):
+            raise 'The Path contains wildcards. Please use the method "patternbasedPullData" instead'
+        return copy(rgetattr(self._data, topic, default))
+
+    def _patternbasedPullData(self, pattern: str, default=None):
+        """ Helper, which enable to perform a pattern based pull.
+            The code receives a pattern, and matches the existing content
+            (by using there path attributes) and return the corresponding data.
+
+        Args:
+            pattern (str): the pattern
+            default (any, optional): The default-value. Defaults to None.
+
+        Returns:
+            list:
+        """
+
+        # To extract the data based on a Pattern,
+        # we firstly, we check if the given pattern
+        # is a pattern.
+        if not containsWildcards(pattern):
+            # Its not a pattern so we will speed up
+            # things.
+            global DEFAULT_OBJ
+            data = self._pullData(pattern, DEFAULT_OBJ)
+
+            if data is not DEFAULT_OBJ:
+                return [
+                    ensureDottedAccess({
+                        'path': pattern,
+                        'data': data
+                    })
+                ]
+            elif default is not None:
+                return [
+                    ensureDottedAccess({
+                        'path': pattern,
+                        'data': default
+                    })
+                ]
+
+            return []
+
+        # Now we know, we have to work with the query,
+        # for that purpose, we will adapt the data object
+        # to the following form:
+        # {path: value}
+        flatten = flattenObject(self._data)
+        ret = []
+
+        # We will use our alternative representation of the
+        # object to compare the pattern with the path item.
+        # only if there is a direct match => we will extract it.
+        # That corresponds to a direct level extraction and
+        # prevents to grap multiple items.
+        for path, data in flatten.items():
+            result = self._comparePatternAndPath(pattern, path)
+            if result.affectedOnSameLevel or result.affectedByChild:
+                ret.append(ensureDottedAccess({
+                    'path': path,
+                    'data': data
+                }))
+
+        # Now we just return our created element.
+        return ret
```

### Comparing `nope_py-1.7.8rc3/nope/types/__init__.py` & `nope_py-1.7.9/nope/types/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from dataclasses import dataclass, field
-from typing import Any, Callable, List, Dict, Union
-
-
-@dataclass
-class ServiceUi:
-    """ Definition of an ui.
-
-        parameters:
-            file =                          An additional file (javascript) -> defining the ui. Defaults to False -> No extra File is required.
-            autoGenBySchema =               Autogenerates the ui to configure the service based on the given schema
-            requiredProvidersForRendering = Defined items (service), that must be present in the network, to define the ui-file.
-    """
-
-    file: str | bool = False
-    """ An additional file (javascript) -> defining the ui. Defaults to False -> No extra File is required.
-    """
-
-    autoGenBySchema: bool = False
-    """ Autogenerates the ui to configure the service based on the given schema
-    """
-
-    requiredProvidersForRendering: List[str] = field(default_factory=list)
-    """ Defined items, that must be present in the network,
-        to define the ui-file.
-    """
-
-
-@dataclass
-class CallOptions:
-    """ Options used in an RPC-Call
-
-        parameters:
-            resultSink  = Desired result sink. If implemented, the result will be published on this topic as well.
-            timeout     = A User Provided Timeout of the call. After the timeout has been ellapsed, the task is
-                          cancelled with a timeout error. The Time is given in **ms**
-    """
-    resultSink: str = None
-    """ Desired result sink. If implemented, the result will be published on this topic as well. """
-
-    timeout: int = -1
-    """ A User Provided Timeout of the call. After the timeout has been ellapsed, the task is
-        cancelled with a timeout error. The Time is given in **ms**
-    """
-
-
-@dataclass
-class ServiceOptions:
-
-    schema: Any
-    """ Schmea describing the Function.
-    """
-
-    resultSink: str = None
-    """ Desired result sink. If implemented, the result will be published on this topic as well. """
-
-    timeout: int = -1
-    """ A User Provided Timeout of the call. After the timeout has been ellapsed, the task is
-        cancelled with a timeout error. The Time is given in **ms**
-    """
-
-    id: str | bool = False
-    """ Instead of generating a uuid an id could be provided
-    """
-
-    ui: ServiceUi = field(default_factory=ServiceUi)
-    """ Defintion of the UI.
-    """
-
-    isDynamic: bool = False
-    """ Flag to mark the Function as Dynamically created
-    """
-
-
-@dataclass
-class ProvidedClass:
-    selector: str
-    createInstance: Callable[Any, Any]
-    allowInstanceGeneration: bool = True
-    maxAmountOfInstance: int = -1
-
-
-@dataclass
-class DefaultInstance:
-    identifier: str
-    type: str
-    params: List[Any] = field(default_factory=list)
-
-
-@dataclass
-class ProvidedService:
-    function: Callable[Any, Any]
-    options: ServiceOptions
-
-
-@dataclass
-class Autostart:
-    name: str
-    params: List[Any] = field(default_factory=list)
-    delay: int = -1
-
-
-@dataclass
-class NopePackage:
-    nameOfPackage: str
-    autostart: Dict[str, List[Autostart]] = field(default_factory=dict)
-    defaultInstances: List[DefaultInstance] = field(default_factory=list)
-    providedServices: List[ProvidedService] = field(default_factory=list)
-    providedClasses: List[ProvidedClass] = field(default_factory=list)
-    requiredPackages: List[str] = field(default_factory=list)
+from dataclasses import dataclass, field
+from typing import Any, Callable, List, Dict, Union
+
+
+@dataclass
+class ServiceUi:
+    """ Definition of an ui.
+
+        parameters:
+            file =                          An additional file (javascript) -> defining the ui. Defaults to False -> No extra File is required.
+            autoGenBySchema =               Autogenerates the ui to configure the service based on the given schema
+            requiredProvidersForRendering = Defined items (service), that must be present in the network, to define the ui-file.
+    """
+
+    file: str | bool = False
+    """ An additional file (javascript) -> defining the ui. Defaults to False -> No extra File is required.
+    """
+
+    autoGenBySchema: bool = False
+    """ Autogenerates the ui to configure the service based on the given schema
+    """
+
+    requiredProvidersForRendering: List[str] = field(default_factory=list)
+    """ Defined items, that must be present in the network,
+        to define the ui-file.
+    """
+
+
+@dataclass
+class CallOptions:
+    """ Options used in an RPC-Call
+
+        parameters:
+            resultSink  = Desired result sink. If implemented, the result will be published on this topic as well.
+            timeout     = A User Provided Timeout of the call. After the timeout has been ellapsed, the task is
+                          cancelled with a timeout error. The Time is given in **ms**
+    """
+    resultSink: str = None
+    """ Desired result sink. If implemented, the result will be published on this topic as well. """
+
+    timeout: int = -1
+    """ A User Provided Timeout of the call. After the timeout has been ellapsed, the task is
+        cancelled with a timeout error. The Time is given in **ms**
+    """
+
+
+@dataclass
+class ServiceOptions:
+
+    schema: Any
+    """ Schmea describing the Function.
+    """
+
+    resultSink: str = None
+    """ Desired result sink. If implemented, the result will be published on this topic as well. """
+
+    timeout: int = -1
+    """ A User Provided Timeout of the call. After the timeout has been ellapsed, the task is
+        cancelled with a timeout error. The Time is given in **ms**
+    """
+
+    id: str | bool = False
+    """ Instead of generating a uuid an id could be provided
+    """
+
+    ui: ServiceUi = field(default_factory=ServiceUi)
+    """ Defintion of the UI.
+    """
+
+    isDynamic: bool = False
+    """ Flag to mark the Function as Dynamically created
+    """
+
+
+@dataclass
+class ProvidedClass:
+    selector: str
+    createInstance: Callable[Any, Any]
+    allowInstanceGeneration: bool = True
+    maxAmountOfInstance: int = -1
+
+
+@dataclass
+class DefaultInstance:
+    identifier: str
+    type: str
+    params: List[Any] = field(default_factory=list)
+
+
+@dataclass
+class ProvidedService:
+    function: Callable[Any, Any]
+    options: ServiceOptions
+
+
+@dataclass
+class Autostart:
+    name: str
+    params: List[Any] = field(default_factory=list)
+    delay: int = -1
+
+
+@dataclass
+class NopePackage:
+    nameOfPackage: str
+    autostart: Dict[str, List[Autostart]] = field(default_factory=dict)
+    defaultInstances: List[DefaultInstance] = field(default_factory=list)
+    providedServices: List[ProvidedService] = field(default_factory=list)
+    providedClasses: List[ProvidedClass] = field(default_factory=list)
+    requiredPackages: List[str] = field(default_factory=list)
```

### Comparing `nope_py-1.7.8rc3/nope_py.egg-info/PKG-INFO` & `nope_py-1.7.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,251 +1,254 @@
-Metadata-Version: 2.1
-Name: nope-py
-Version: 1.7.8rc3
-Summary: NOPE-Lib represents the No Programming Environment Library for python.
-Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
-Author: Martin Karkowski
-Author-email: m.karkowski@zema.de
-Maintainer: Martin Karkowski
-Maintainer-email: m.karkowski@zema.de
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NoPE 
-
-## A Python wrapper for the Library
-
-Please visit our [Docu](https://zema-ggmbh.github.io/NoPE-Docs/)
-
-## Show me `NoPE` in 5 Minutes! 
-
-### 1. Create a `Nodejs` Project
-
-Get started by **creating a new project** distributed using `NoPE`.
-
-For our **PYTHON** project we will use the nope-js-node cli tools to create a Project.
-
-1. Installation using  npm:
-  ```bash
-  npm install -g nope-js-node
-  ```
-2. Start your first Project:
-  ```bash
-  nope-js project create
-  ```
-  This should open a `cli`.
-
-3. Answer the requried questions to complete create the directory.
-  - Name the project `HelloWorld`
-  - Give it a short summary. This summary will used during distributing your project.
-  - make shure you select `python` as project type    
-
-4. navigate to the create folder ( e.g. `cd ./HelloWorld` ) 
-
-  This creates a project structure.
-
-5. Open your IDE (e.g. vscode)
-
-By using the project-tool the following features are added to the project:
-- Debugging of the application using VS code (launch-file)
-- Creation of a doc file (see doc/make)
-- Helpers to build a browser related version
-- Use of a changelog
-- Deployment as a package
-- Simple extension using project-tool
-
-## 2. Add a Service in `Python`
-
-Our goal is to define a greeting service
-> The service creates a greeting message for a person. 
-
-### Why a Service
-
-> This service is independent of how many times it has been called.
-> Our functionality is stateless, this allows us to use a service.
-
-### Using the `CLI` to generate the Service
-
-1. To create the Service: 
-  use the `project-tool` to create the service 
-
-  ```bash
-  nope-js project edit
-  ```
-
-2. Perfom the following selection inside of the tool.
-  1. Selection `add`, to add a new element
-  2. Select `service`, because we want to create a service
-  3. Enter the name of the service, in our case `HelloWorld`
-  
-  Creation of the corresponding files and imports is done automatically
-
-  This will update our project folder.
-
-Now `NoPE` defined a new service file (`HelloWorldFunctions.py`) for us:
-
-```python
-#!/usr/bin/env python
-# @author Martin Karkowski
-# @email m.karkowski@zema.de
-
-from nope import getNopeLogger
-
-LOGGER = getNopeLogger("HelloWorldService")
-
-# Please provide the schema for the Function.
-# See the Example below.
-SCHEMA = {
-    "type": "function",
-        
-    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
-    # It contains a list of all required inputs.
-    "inputs": [
-    ],
-    # To describe the return of a function we added the field "outputs". It contains a 
-    # JSON-Schema Object.
-    "outputs":{
-    }
-}
-
-async def HelloWorld(greetings: str):
-    # Please overwrite me!
-    LOGGER.debug("calling service 'HelloWorld' with the following parameters:" + str(greetings))
-    return "Hello " + greetings + "!"
-```
-
-In that file, you will find a template for the service we want to implement. By default, the newly created service implements the hello-world behavior. This must changed. In our case it matches the desired behavior.
-
-
-> All services **must** be implemented `async` manner. This is necessary so that the runtime is not blocked.
-
-
-### Adding a Service interface
-
-We now want to describe our service, that it can be used correctly at different Runtimes. Therefore we will define the `schema` to the `SCHEMA` variable. This Schema follows the definition of a `JSON-Schema`:
-
-```python
-SCHEMA = {
-    "type": "function",
-        
-    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
-    # It contains a list of all required inputs.
-    "inputs": [
-        {
-            # The Description of the Parameter
-            "description": "The name which should receive a Greeting",
-            # Its used name in the function (see the arguments of the function)
-            "name": "greetings",
-            # The Schema follows a default JSON-Schema
-            "schema": {
-                "type": "string"
-            }
-        }
-    ],
-    # To describe the return of a function we added the field "outputs". It contains a 
-    # JSON-Schema Object.
-    "outputs":{
-        "type": "string",
-
-        # We provide some extra Info for the other users.
-        "description": "The greeting Message!"
-    }
-}
-```
-
-Because the python implementation is lacking some typings please checkout the docs
-
-## 3. Running the Service:
-
-To run the `service` and distribute to different `NoPE`-Runtimes we have to determine a configuration:
-
-```bash
-nope-py scan
-```
-The `cli` will find all defined `services` or `modules` exposed in a so called `NoPE-Package` (This has been created automatically during the initalization of the project). The tool will store its results in the following configuration (located at `./config/config.json`):
-
-```json
-[
-    {
-        "nameOfPackage": "HelloWorld",
-        "autostart": {},
-        "defaultInstances": [],
-        "providedServices": [
-            {
-                "options": {
-                    "schema": {
-                        ...
-                    },
-                    "resultSink": null,
-                    "timeout": -1,
-                    "id": "HelloWorld",
-                    "ui": {
-                        "file": false,
-                        "autoGenBySchema": false,
-                        "requiredProvidersForRendering": []
-                    },
-                    "isDynamic": false
-                }
-            }
-        ],
-        "providedClasses": [],
-        "requiredPackages": [],
-        "path": "C:\\Users\\m.karkowski\\Documents\\00-Repos\\TEST\\HelloWorld\\HelloWorld\\__init__.py"
-    }
-]
-```
-
-Finally we are ready to distribute our service by using the command:
-
-```bash
-nope-py run
-```
-
-This will start a runtime providing our service.
-
-## 4. Interact with the Runtime
-
-Currently our service is only run internally (nope is not connected and runs without an external connection layer). To check and play with the distribution, we kill our old process (`ctrl+c`) create a separate process (e.g. a bash) and provide a serve:
-
-```bash
-nope-js run -c io-server
-```
-
-This will spool up a `socket-io` server on our localhost. 
-
-Afterwards we will restart our Runtime hosting the created service using `io-sockets` as connection layer:
-
-```bash
-nope-py run -c io-client
-```
-
-Now we are able to start our `interact-tool` to manually execute our process:
-
-```bash
-nope-js interact -c io-client -s
-```
-
-To use the `interact`-**tool** follow the questions:
-
-1. What do you want to do?
-    - We want to inspect our distributed system -> `inspect`
-2. What do you want to inspect?
-    - We want to check if our service is present -> `service`
-    - We should be albe to see our `HelloWorld`-Service (see 1)
-3. Now we want to execute this service. Therefore we navigate `back` to the main menu
-4. Now we select `execute` and afterwards `service` because we want to execute our service
-5. Now the Tool renders the available services and we select `HelloWorld` (see 2) and it will render the previously defined Schema.
-6. Now we have to enter the inputs required by the Service:
-    - It is important that the parameters are entered as list (because there might be more the 1 Parameter)
-    - Enter the parameters as valid `JSON` Data.
-    - Press `enter`
-
-    > Executing services with the interact tool will perfom function immedialty. If you integrated Hardware be aware of that.
-
-7. The Tool shows the result (see 4)
-
-
-> You are now running a distributed System using **remote procedure calls** in ***python***
+Metadata-Version: 2.1
+Name: nope_py
+Version: 1.7.9
+Summary: NOPE-Lib represents the No Programming Environment Library for python.
+Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
+Author: Martin Karkowski
+Author-email: m.karkowski@zema.de
+Maintainer: Martin Karkowski
+Maintainer-email: m.karkowski@zema.de
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NoPE 
+
+## A Python wrapper for the Library
+
+Please visit our [Docu](https://zema-ggmbh.github.io/NoPE-Docs/)
+
+## Show me `NoPE` in 5 Minutes! 
+
+### 1. Create a `Nodejs` Project
+
+Get started by **creating a new project** distributed using `NoPE`.
+
+For our **PYTHON** project we will use the nope-js-node cli tools to create a Project.
+
+1. Installation using  npm:
+  ```bash
+  npm install -g nope-js-node
+  ```
+2. Start your first Project:
+  ```bash
+  nope-js project create
+  ```
+  This should open a `cli`.
+
+3. Answer the requried questions to complete create the directory.
+  - Name the project `HelloWorld`
+  - Give it a short summary. This summary will used during distributing your project.
+  - make shure you select `python` as project type    
+
+4. navigate to the create folder ( e.g. `cd ./HelloWorld` ) 
+
+  This creates a project structure.
+
+5. Open your IDE (e.g. vscode)
+
+By using the project-tool the following features are added to the project:
+- Debugging of the application using VS code (launch-file)
+- Creation of a doc file (see doc/make)
+- Helpers to build a browser related version
+- Use of a changelog
+- Deployment as a package
+- Simple extension using project-tool
+
+## 2. Add a Service in `Python`
+
+Our goal is to define a greeting service
+> The service creates a greeting message for a person. 
+
+### Why a Service
+
+> This service is independent of how many times it has been called.
+> Our functionality is stateless, this allows us to use a service.
+
+### Using the `CLI` to generate the Service
+
+1. To create the Service: 
+  use the `project-tool` to create the service 
+
+  ```bash
+  nope-js project edit
+  ```
+
+2. Perfom the following selection inside of the tool.
+  1. Selection `add`, to add a new element
+  2. Select `service`, because we want to create a service
+  3. Enter the name of the service, in our case `HelloWorld`
+  
+  Creation of the corresponding files and imports is done automatically
+
+  This will update our project folder.
+
+Now `NoPE` defined a new service file (`HelloWorldFunctions.py`) for us:
+
+```python
+#!/usr/bin/env python
+# @author Martin Karkowski
+# @email m.karkowski@zema.de
+
+from nope import getNopeLogger
+
+LOGGER = getNopeLogger("HelloWorldService")
+
+# Please provide the schema for the Function.
+# See the Example below.
+SCHEMA = {
+    "type": "function",
+        
+    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
+    # It contains a list of all required inputs.
+    "inputs": [
+    ],
+    # To describe the return of a function we added the field "outputs". It contains a 
+    # JSON-Schema Object.
+    "outputs":{
+    }
+}
+
+async def HelloWorld(greetings: str):
+    # Please overwrite me!
+    LOGGER.debug("calling service 'HelloWorld' with the following parameters:" + str(greetings))
+    return "Hello " + greetings + "!"
+```
+
+In that file, you will find a template for the service we want to implement. By default, the newly created service implements the hello-world behavior. This must changed. In our case it matches the desired behavior.
+
+
+> All services **must** be implemented `async` manner. This is necessary so that the runtime is not blocked.
+
+
+### Adding a Service interface
+
+We now want to describe our service, that it can be used correctly at different Runtimes. Therefore we will define the `schema` to the `SCHEMA` variable. This Schema follows the definition of a `JSON-Schema`:
+
+```python
+SCHEMA = {
+    "type": "function",
+        
+    # To describe the used inputs of a function or serive we added the field "inputs" to the schema.
+    # It contains a list of all required inputs.
+    "inputs": [
+        {
+            # The Description of the Parameter
+            "description": "The name which should receive a Greeting",
+            # Its used name in the function (see the arguments of the function)
+            "name": "greetings",
+            # The Schema follows a default JSON-Schema
+            "schema": {
+                "type": "string"
+            }
+        }
+    ],
+    # To describe the return of a function we added the field "outputs". It contains a 
+    # JSON-Schema Object.
+    "outputs":{
+        "type": "string",
+
+        # We provide some extra Info for the other users.
+        "description": "The greeting Message!"
+    }
+}
+```
+
+Because the python implementation is lacking some typings please checkout the docs
+
+## 3. Running the Service:
+
+To run the `service` and distribute to different `NoPE`-Runtimes we have to determine a configuration:
+
+```bash
+nope-py scan
+```
+The `cli` will find all defined `services` or `modules` exposed in a so called `NoPE-Package` (This has been created automatically during the initalization of the project). The tool will store its results in the following configuration (located at `./config/config.json`):
+
+```json
+[
+    {
+        "nameOfPackage": "HelloWorld",
+        "autostart": {},
+        "defaultInstances": [],
+        "providedServices": [
+            {
+                "options": {
+                    "schema": {
+                        ...
+                    },
+                    "resultSink": null,
+                    "timeout": -1,
+                    "id": "HelloWorld",
+                    "ui": {
+                        "file": false,
+                        "autoGenBySchema": false,
+                        "requiredProvidersForRendering": []
+                    },
+                    "isDynamic": false
+                }
+            }
+        ],
+        "providedClasses": [],
+        "requiredPackages": [],
+        "path": "C:\\Users\\m.karkowski\\Documents\\00-Repos\\TEST\\HelloWorld\\HelloWorld\\__init__.py"
+    }
+]
+```
+
+Finally we are ready to distribute our service by using the command:
+
+```bash
+nope-py run
+```
+
+This will start a runtime providing our service.
+
+## 4. Interact with the Runtime
+
+Currently our service is only run internally (nope is not connected and runs without an external connection layer). To check and play with the distribution, we kill our old process (`ctrl+c`) create a separate process (e.g. a bash) and provide a serve:
+
+```bash
+nope-js run -c io-server
+```
+
+This will spool up a `socket-io` server on our localhost. 
+
+Afterwards we will restart our Runtime hosting the created service using `io-sockets` as connection layer:
+
+```bash
+nope-py run -c io-client
+```
+
+Now we are able to start our `interact-tool` to manually execute our process:
+
+```bash
+nope-js interact -c io-client -s
+```
+
+To use the `interact`-**tool** follow the questions:
+
+1. What do you want to do?
+    - We want to inspect our distributed system -> `inspect`
+2. What do you want to inspect?
+    - We want to check if our service is present -> `service`
+    - We should be albe to see our `HelloWorld`-Service (see 1)
+3. Now we want to execute this service. Therefore we navigate `back` to the main menu
+4. Now we select `execute` and afterwards `service` because we want to execute our service
+5. Now the Tool renders the available services and we select `HelloWorld` (see 2) and it will render the previously defined Schema.
+6. Now we have to enter the inputs required by the Service:
+    - It is important that the parameters are entered as list (because there might be more the 1 Parameter)
+    - Enter the parameters as valid `JSON` Data.
+    - Press `enter`
+
+    > Executing services with the interact tool will perfom function immedialty. If you integrated Hardware be aware of that.
+
+7. The Tool shows the result (see 4)
+
+
+> You are now running a distributed System using **remote procedure calls** in ***python***
+
```

### Comparing `nope_py-1.7.8rc3/nope_py.egg-info/SOURCES.txt` & `nope_py-1.7.9/nope_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/setup.py` & `nope_py-1.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     long_description = open("./README.md").read()
 except BaseException:
     long_description = """NOPE-Python Backend. A Generic Backend for Python"""
 
 if __name__ == "__main__":
     setup(name="nope_py",
-          version="1.7.8rc3",
+          version="1.7.9",
           description="NOPE-Lib represents the No Programming Environment Library for python.",
           long_description=long_description,
           long_description_content_type="text/markdown",
           author="Martin Karkowski",
           author_email="m.karkowski@zema.de",
           maintainer="Martin Karkowski",
           maintainer_email="m.karkowski@zema.de",
```

### Comparing `nope_py-1.7.8rc3/test/test.py` & `nope_py-1.7.9/test/test.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc3/test/test_plugin_bridge.py` & `nope_py-1.7.9/test/test_plugin_bridge.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import asyncio
-from asyncio import sleep
-
-import pytest
-
-from nope.plugins import install
-
-"""
-This is an Example how to extend the behavior of any class inside of Nope.
-
-Therefore we want to load our sample plugin: "hello".
-Therefore we know
-"""
-
-
-# install(nope, "nope.plugins.hello", plugin_dest="nope.dispatcher.rpcManager")
-
-
-@pytest.fixture
-def event_loop():
-    loop = asyncio.new_event_loop()
-    nope.EXECUTOR.assignLoop(loop)
-    yield loop
-    loop.close()
-
-
-async def test_bridge_plugin():
-    import nope
-    nope, _, __ = install(nope, "nope.plugins.ack_messages")
-
-    dispatcher = nope.getDispatcher({
-        "communicator": await nope.getLayer("event"),
-        "logger": False,
-    })
-
-    # To make our Plugin work -> we have to manually assign the id
-    # dispatcher.communicator.ackReplyId = dispatcher.id
-
-    await dispatcher.ready.waitFor()
-
-    def sub(*args):
-        print(*args)
-
-    await dispatcher.communicator.on("test", sub)
-    dispatcher.dataDistributor.patternbasedPullData("test/+/a/#")
-    await dispatcher.communicator.emit("test", {"data": "test-data-1"}, target=dispatcher.id, timeout=1.0)
-    await sleep(1)
-    ex = Exception("Failed")
-    try:
-        await dispatcher.communicator.emit("test", {"data": "test-data-2"}, target="Wont possible", timeout=1.0)
-        raise ex
-    except Exception as e:
-        if e == ex:
-            raise ex
-
-    print(dispatcher.connectivityManager.info)
-
-
-if __name__ == "__main__":
-    import nope
-    nope.EXECUTOR.loop.run_until_complete(test_bridge_plugin())
+import asyncio
+from asyncio import sleep
+
+import pytest
+
+from nope.plugins import install
+
+"""
+This is an Example how to extend the behavior of any class inside of Nope.
+
+Therefore we want to load our sample plugin: "hello".
+Therefore we know
+"""
+
+
+# install(nope, "nope.plugins.hello", plugin_dest="nope.dispatcher.rpcManager")
+
+
+@pytest.fixture
+def event_loop():
+    loop = asyncio.new_event_loop()
+    nope.EXECUTOR.assignLoop(loop)
+    yield loop
+    loop.close()
+
+
+async def test_bridge_plugin():
+    import nope
+    nope, _, __ = install(nope, "nope.plugins.ack_messages")
+
+    dispatcher = nope.getDispatcher({
+        "communicator": await nope.getLayer("event"),
+        "logger": False,
+    })
+
+    # To make our Plugin work -> we have to manually assign the id
+    # dispatcher.communicator.ackReplyId = dispatcher.id
+
+    await dispatcher.ready.waitFor()
+
+    def sub(*args):
+        print(*args)
+
+    await dispatcher.communicator.on("test", sub)
+    dispatcher.dataDistributor.patternbasedPullData("test/+/a/#")
+    await dispatcher.communicator.emit("test", {"data": "test-data-1"}, target=dispatcher.id, timeout=1.0)
+    await sleep(1)
+    ex = Exception("Failed")
+    try:
+        await dispatcher.communicator.emit("test", {"data": "test-data-2"}, target="Wont possible", timeout=1.0)
+        raise ex
+    except Exception as e:
+        if e == ex:
+            raise ex
+
+    print(dispatcher.connectivityManager.info)
+
+
+if __name__ == "__main__":
+    import nope
+    nope.EXECUTOR.loop.run_until_complete(test_bridge_plugin())
```

### Comparing `nope_py-1.7.8rc3/test/test_plugin_rpc_callbacks.py` & `nope_py-1.7.9/test/test_plugin_rpc_callbacks.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import asyncio
-from asyncio import sleep
-
-import pytest
-
-from nope.plugins import install
-
-"""
-This is an Example how to extend the behavior of any class inside of Nope.
-
-Therefore we want to load our sample plugin: "hello".
-Therefore we know
-"""
-
-
-# install(nope, "nope.plugins.hello", plugin_dest="nope.dispatcher.rpcManager")
-
-
-@pytest.fixture
-def event_loop():
-    loop = asyncio.new_event_loop()
-    nope.EXECUTOR.assignLoop(loop)
-    yield loop
-    loop.close()
-
-
-async def test_bridge_plugin():
-    import nope
-    nope, _, __ = install(nope, "nope.plugins.rpc_with_callbacks")
-
-    dispatcher = nope.getDispatcher({
-        "communicator": await nope.getLayer("event"),
-        "logger": "info",
-    })
-
-    # To make our Plugin work -> we have to manually assign the id
-    # dispatcher.communicator.ackReplyId = dispatcher.id
-    await dispatcher.ready.waitFor()
-
-    async def funcWithCallback(p, cb1, cb2):
-        return await cb1(p, cb2)
-
-    await dispatcher.rpcManager.registerService(funcWithCallback, {
-        "id": "funcWithCallback"
-    })
-
-    async def cb(p, cb2):
-        print("inside of callback")
-        await cb2()
-
-    await dispatcher.rpcManager.performCall("funcWithCallback", ["jeah", cb, lambda *args: print("Here")], {
-        "calledOnce": [1]
-    })
-
-
-if __name__ == "__main__":
-    import nope
-    nope.EXECUTOR.loop.run_until_complete(test_bridge_plugin())
+import asyncio
+from asyncio import sleep
+
+import pytest
+
+from nope.plugins import install
+
+"""
+This is an Example how to extend the behavior of any class inside of Nope.
+
+Therefore we want to load our sample plugin: "hello".
+Therefore we know
+"""
+
+
+# install(nope, "nope.plugins.hello", plugin_dest="nope.dispatcher.rpcManager")
+
+
+@pytest.fixture
+def event_loop():
+    loop = asyncio.new_event_loop()
+    nope.EXECUTOR.assignLoop(loop)
+    yield loop
+    loop.close()
+
+
+async def test_bridge_plugin():
+    import nope
+    nope, _, __ = install(nope, "nope.plugins.rpc_with_callbacks")
+
+    dispatcher = nope.getDispatcher({
+        "communicator": await nope.getLayer("event"),
+        "logger": "info",
+    })
+
+    # To make our Plugin work -> we have to manually assign the id
+    # dispatcher.communicator.ackReplyId = dispatcher.id
+    await dispatcher.ready.waitFor()
+
+    async def funcWithCallback(p, cb1, cb2):
+        return await cb1(p, cb2)
+
+    await dispatcher.rpcManager.registerService(funcWithCallback, {
+        "id": "funcWithCallback"
+    })
+
+    async def cb(p, cb2):
+        print("inside of callback")
+        await cb2()
+
+    await dispatcher.rpcManager.performCall("funcWithCallback", ["jeah", cb, lambda *args: print("Here")], {
+        "calledOnce": [1]
+    })
+
+
+if __name__ == "__main__":
+    import nope
+    nope.EXECUTOR.loop.run_until_complete(test_bridge_plugin())
```

### Comparing `nope_py-1.7.8rc3/test/test_pub_sub.py` & `nope_py-1.7.9/test/test_pub_sub.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from nope import PubSubSystem, NopeEventEmitter
-
-called = 0
-
-pub_sub = PubSubSystem()
-
-publisher = NopeEventEmitter()
-subscriber = NopeEventEmitter()
-
-pub_sub.register(publisher, {
-    "mode": "publish",
-    "schema": {},
-    "topic": "this/is/a/test",
-})
-
-pub_sub.register(subscriber, {
-    "mode": "subscribe",
-    "schema": {},
-    "topic": "this/#",
-})
-
-
-def callback(data, rest):
-    global called
-    called += 1
-    assert data == "Hello World"
-
-
-def incremental(data, rest):
-    print(data, rest)
-
-
-pub_sub.onIncrementalDataChange.subscribe(incremental)
-
-subscriber.subscribe(callback)
-publisher.emit("Hello World")
-
-assert called == 1
+from nope import PubSubSystem, NopeEventEmitter
+
+called = 0
+
+pub_sub = PubSubSystem()
+
+publisher = NopeEventEmitter()
+subscriber = NopeEventEmitter()
+
+pub_sub.register(publisher, {
+    "mode": "publish",
+    "schema": {},
+    "topic": "this/is/a/test",
+})
+
+pub_sub.register(subscriber, {
+    "mode": "subscribe",
+    "schema": {},
+    "topic": "this/#",
+})
+
+
+def callback(data, rest):
+    global called
+    called += 1
+    assert data == "Hello World"
+
+
+def incremental(data, rest):
+    print(data, rest)
+
+
+pub_sub.onIncrementalDataChange.subscribe(incremental)
+
+subscriber.subscribe(callback)
+publisher.emit("Hello World")
+
+assert called == 1
```

### Comparing `nope_py-1.7.8rc3/test/test_rpc_manager.py` & `nope_py-1.7.9/test/test_rpc_manager.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import asyncio
-import time
-from asyncio import sleep
-
-import pytest
-
-from nope import getLayer, NopeRpcManager, formatException, getTimestamp, EXECUTOR
-
-IN_PY_TEST = False
-
-
-@pytest.fixture
-def event_loop():
-    global IN_PY_TEST
-    IN_PY_TEST = True
-    loop = asyncio.new_event_loop()
-    EXECUTOR.assignLoop(loop)
-    yield loop
-    loop.close()
-
-
-async def main():
-    manager = NopeRpcManager({
-        "communicator": await getLayer("event"),
-        "logger": False,
-    }, lambda *args: "test", "test")
-
-    await manager.ready.waitFor()
-
-    async def hello(name: str) -> str:
-        return f"Hello {name}!"
-
-    async def delayed(name: str) -> str:
-        await sleep(1)
-        return await hello(name)
-
-    manager.registerService(hello, {
-        "id": "hello"
-    })
-
-    manager.registerService(delayed, {
-        "id": "delayed"
-    })
-
-    await sleep(1.5)
-
-    assert "hello" in manager.services.extracted_key, "Failed to register the services"
-    assert "delayed" in manager.services.extracted_key, "Failed to register the services"
-
-    # Try calling the Service
-    res = await manager.performCall("hello", ["Pytest"])
-    assert res == "Hello Pytest!"
-
-    try:
-        res = await manager.performCall("delayed", ["Pytest"], {"timeout": 2000})
-        assert res == "Hello Pytest!"
-    except Exception as error:
-        print("HERE", error)
-
-    try:
-        res = await manager.performCall("delayed", ["Pytest"], {"timeout": 200})
-        assert res == "Hello Pytest!"
-    except Exception as error:
-        print(formatException(error))
-
-    start = getTimestamp()
-    res = await manager.performCall(["delayed"] * 5, ["Pytest"])
-    end = getTimestamp()
-
-    if not IN_PY_TEST:
-        delta = []
-        bench = 100000
-
-        start = time.process_time()
-        for i in range(bench):
-            # s = time.process_time()
-            await manager.performCall("hello", ["Benchmark"])
-            # delta = (time.process_time() - s) * 1000
-            # print(i, "mainloop:", delta, "[ms]")
-        end = time.process_time()
-        delta = end - start
-        print(delta, bench)
-        time_per_call = delta * 1000 / bench
-        qps = 1000.0 / time_per_call
-
-        print(
-            "NOPE    ",
-            round(
-                time_per_call,
-                5),
-            "[ms] ->",
-            round(
-                qps,
-                5),
-            "[R/s]")
-
-        start = getTimestamp()
-        for i in range(bench):
-            await hello("delayed")
-        end = getTimestamp()
-        delta = end - start
-        time_per_call = delta / bench
-        qps = 1000.0 / time_per_call
-
-        print(
-            "ORIGINAL",
-            round(
-                time_per_call,
-                5),
-            "[ms] ->",
-            round(
-                qps,
-                5),
-            "[R/s]")
-
-    # await manager.dispose()
-
-
-if __name__ == "__main__":
-    EXECUTOR.loop.run_until_complete(main())
-    # EXECUTOR.loop.run_forever()
-
-# yappi.set_clock_type("CPU")
-# with yappi.run():
-#     EXECUTOR.loop.run_until_complete(main())
-# yappi.get_func_stats().print_all()
+import asyncio
+import time
+from asyncio import sleep
+
+import pytest
+
+from nope import getLayer, NopeRpcManager, formatException, getTimestamp, EXECUTOR
+
+IN_PY_TEST = False
+
+
+@pytest.fixture
+def event_loop():
+    global IN_PY_TEST
+    IN_PY_TEST = True
+    loop = asyncio.new_event_loop()
+    EXECUTOR.assignLoop(loop)
+    yield loop
+    loop.close()
+
+
+async def main():
+    manager = NopeRpcManager({
+        "communicator": await getLayer("event"),
+        "logger": False,
+    }, lambda *args: "test", "test")
+
+    await manager.ready.waitFor()
+
+    async def hello(name: str) -> str:
+        return f"Hello {name}!"
+
+    async def delayed(name: str) -> str:
+        await sleep(1)
+        return await hello(name)
+
+    manager.registerService(hello, {
+        "id": "hello"
+    })
+
+    manager.registerService(delayed, {
+        "id": "delayed"
+    })
+
+    await sleep(1.5)
+
+    assert "hello" in manager.services.extracted_key, "Failed to register the services"
+    assert "delayed" in manager.services.extracted_key, "Failed to register the services"
+
+    # Try calling the Service
+    res = await manager.performCall("hello", ["Pytest"])
+    assert res == "Hello Pytest!"
+
+    try:
+        res = await manager.performCall("delayed", ["Pytest"], {"timeout": 2000})
+        assert res == "Hello Pytest!"
+    except Exception as error:
+        print("HERE", error)
+
+    try:
+        res = await manager.performCall("delayed", ["Pytest"], {"timeout": 200})
+        assert res == "Hello Pytest!"
+    except Exception as error:
+        print(formatException(error))
+
+    start = getTimestamp()
+    res = await manager.performCall(["delayed"] * 5, ["Pytest"])
+    end = getTimestamp()
+
+    if not IN_PY_TEST:
+        delta = []
+        bench = 100000
+
+        start = time.process_time()
+        for i in range(bench):
+            # s = time.process_time()
+            await manager.performCall("hello", ["Benchmark"])
+            # delta = (time.process_time() - s) * 1000
+            # print(i, "mainloop:", delta, "[ms]")
+        end = time.process_time()
+        delta = end - start
+        print(delta, bench)
+        time_per_call = delta * 1000 / bench
+        qps = 1000.0 / time_per_call
+
+        print(
+            "NOPE    ",
+            round(
+                time_per_call,
+                5),
+            "[ms] ->",
+            round(
+                qps,
+                5),
+            "[R/s]")
+
+        start = getTimestamp()
+        for i in range(bench):
+            await hello("delayed")
+        end = getTimestamp()
+        delta = end - start
+        time_per_call = delta / bench
+        qps = 1000.0 / time_per_call
+
+        print(
+            "ORIGINAL",
+            round(
+                time_per_call,
+                5),
+            "[ms] ->",
+            round(
+                qps,
+                5),
+            "[R/s]")
+
+    # await manager.dispose()
+
+
+if __name__ == "__main__":
+    EXECUTOR.loop.run_until_complete(main())
+    # EXECUTOR.loop.run_forever()
+
+# yappi.set_clock_type("CPU")
+# with yappi.run():
+#     EXECUTOR.loop.run_until_complete(main())
+# yappi.get_func_stats().print_all()
```

