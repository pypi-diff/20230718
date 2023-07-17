# Comparing `tmp/parsl-2023.7.17.tar.gz` & `tmp/parsl-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.7.17.tar", last modified: Mon Jul 17 22:42:59 2023, max compression
+gzip compressed data, was "parsl-2023.7.3.tar", last modified: Mon Jul  3 22:43:00 2023, max compression
```

## Comparing `parsl-2023.7.17.tar` & `parsl-2023.7.3.tar`

### file list

```diff
@@ -1,474 +1,473 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.740771 parsl-2023.7.17/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 22:42:52.000000 parsl-2023.7.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-17 22:42:52.000000 parsl-2023.7.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-17 22:42:59.740771 parsl-2023.7.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-17 22:42:52.000000 parsl-2023.7.17/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.676771 parsl-2023.7.17/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.684771 parsl-2023.7.17/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.684771 parsl-2023.7.17/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.688771 parsl-2023.7.17/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62717 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.688771 parsl-2023.7.17/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.688771 parsl-2023.7.17/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.692771 parsl-2023.7.17/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33172 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32997 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.692771 parsl-2023.7.17/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48948 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.692771 parsl-2023.7.17/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48130 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.692771 parsl-2023.7.17/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.696771 parsl-2023.7.17/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.696771 parsl-2023.7.17/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.696771 parsl-2023.7.17/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.696771 parsl-2023.7.17/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.696771 parsl-2023.7.17/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.696771 parsl-2023.7.17/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.700771 parsl-2023.7.17/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.704771 parsl-2023.7.17/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.708771 parsl-2023.7.17/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.712771 parsl-2023.7.17/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.712771 parsl-2023.7.17/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.712771 parsl-2023.7.17/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.716771 parsl-2023.7.17/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.716771 parsl-2023.7.17/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.716771 parsl-2023.7.17/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.716771 parsl-2023.7.17/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.720771 parsl-2023.7.17/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.720771 parsl-2023.7.17/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.720771 parsl-2023.7.17/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.720771 parsl-2023.7.17/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.724771 parsl-2023.7.17/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.724771 parsl-2023.7.17/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.724771 parsl-2023.7.17/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_data/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_data/test_output_chain_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.728771 parsl-2023.7.17/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.728771 parsl-2023.7.17/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.728771 parsl-2023.7.17/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.728771 parsl-2023.7.17/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.728771 parsl-2023.7.17/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.736771 parsl-2023.7.17/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.736771 parsl-2023.7.17/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_69b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.736771 parsl-2023.7.17/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.736771 parsl-2023.7.17/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_serialization/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.740771 parsl-2023.7.17/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.740771 parsl-2023.7.17/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.740771 parsl-2023.7.17/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-07-17 22:42:52.000000 parsl-2023.7.17/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 22:42:57.000000 parsl-2023.7.17/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:42:59.680771 parsl-2023.7.17/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-17 22:42:59.000000 parsl-2023.7.17/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-07-17 22:42:59.000000 parsl-2023.7.17/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:42:59.000000 parsl-2023.7.17/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-17 22:42:59.000000 parsl-2023.7.17/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-17 22:42:59.000000 parsl-2023.7.17/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 22:42:59.000000 parsl-2023.7.17/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 22:42:52.000000 parsl-2023.7.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:42:59.740771 parsl-2023.7.17/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2626 2023-07-17 22:42:52.000000 parsl-2023.7.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.767384 parsl-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 22:42:55.000000 parsl-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 22:42:55.000000 parsl-2023.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:43:00.767384 parsl-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-03 22:42:55.000000 parsl-2023.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.699383 parsl-2023.7.3/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.703384 parsl-2023.7.3/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.703384 parsl-2023.7.3/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.707383 parsl-2023.7.3/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48948 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.711384 parsl-2023.7.3/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48130 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.715384 parsl-2023.7.3/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.719384 parsl-2023.7.3/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.723384 parsl-2023.7.3/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.727384 parsl-2023.7.3/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.731384 parsl-2023.7.3/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.735384 parsl-2023.7.3/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.739384 parsl-2023.7.3/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.739384 parsl-2023.7.3/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.743384 parsl-2023.7.3/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.747384 parsl-2023.7.3/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.751384 parsl-2023.7.3/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_data/test_output_chain_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.751384 parsl-2023.7.3/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.755384 parsl-2023.7.3/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.759384 parsl-2023.7.3/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_serialization/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.763384 parsl-2023.7.3/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.767384 parsl-2023.7.3/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-03 22:42:55.000000 parsl-2023.7.3/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-03 22:42:59.000000 parsl-2023.7.3/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:43:00.695383 parsl-2023.7.3/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:43:00.000000 parsl-2023.7.3/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 22:42:55.000000 parsl-2023.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:43:00.767384 parsl-2023.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2626 2023-07-03 22:42:55.000000 parsl-2023.7.3/setup.py
```

### Comparing `parsl-2023.7.17/LICENSE` & `parsl-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/README.rst` & `parsl-2023.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/__init__.py` & `parsl-2023.7.3/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/addresses.py` & `parsl-2023.7.3/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/app/app.py` & `parsl-2023.7.3/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/app/bash.py` & `parsl-2023.7.3/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/app/errors.py` & `parsl-2023.7.3/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/app/futures.py` & `parsl-2023.7.3/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/app/python.py` & `parsl-2023.7.3/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/benchmark/perf.py` & `parsl-2023.7.3/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/channels/base.py` & `parsl-2023.7.3/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/channels/errors.py` & `parsl-2023.7.3/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/channels/local/local.py` & `parsl-2023.7.3/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.7.3/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/channels/ssh/ssh.py` & `parsl-2023.7.3/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.7.3/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/concurrent/__init__.py` & `parsl-2023.7.3/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/config.py` & `parsl-2023.7.3/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/ASPIRE1.py` & `parsl-2023.7.3/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/Azure.py` & `parsl-2023.7.3/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/ad_hoc.py` & `parsl-2023.7.3/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/bluewaters.py` & `parsl-2023.7.3/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/bridges.py` & `parsl-2023.7.3/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/cc_in2p3.py` & `parsl-2023.7.3/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/comet.py` & `parsl-2023.7.3/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/cooley.py` & `parsl-2023.7.3/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/ec2.py` & `parsl-2023.7.3/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/frontera.py` & `parsl-2023.7.3/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/illinoiscluster.py` & `parsl-2023.7.3/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/kubernetes.py` & `parsl-2023.7.3/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/midway.py` & `parsl-2023.7.3/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/osg.py` & `parsl-2023.7.3/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/polaris.py` & `parsl-2023.7.3/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/stampede2.py` & `parsl-2023.7.3/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/summit.py` & `parsl-2023.7.3/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/theta.py` & `parsl-2023.7.3/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/toss3_llnl.py` & `parsl-2023.7.3/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/vineex_local.py` & `parsl-2023.7.3/parsl/configs/vineex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/configs/wqex_local.py` & `parsl-2023.7.3/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/data_provider/data_manager.py` & `parsl-2023.7.3/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/data_provider/files.py` & `parsl-2023.7.3/parsl/data_provider/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Define the File Type.
 
 The primary purpose of the File object is to track the protocol to be used
 to transfer the file as well as to give the appropriate filepath depending
 on where (client-side, remote-side, intermediary-side) the File.filepath is
 being called from.
 """
-import os
 
+import os
 import typeguard
 import logging
-from typing import Optional, Union
+from typing import Optional
 from urllib.parse import urlparse
 
 logger = logging.getLogger(__name__)
 
 
 class File:
     """The Parsl File Class.
@@ -24,26 +24,25 @@
     the path at the far end of a staging action. It is up to the user of
     the File object to track which local scope that local path actually
     refers to.
 
     """
 
     @typeguard.typechecked
-    def __init__(self, url: Union[os.PathLike, str]):
+    def __init__(self, url: str):
         """Construct a File object from a url string.
 
         Args:
-           - url (string or PathLike) : url of the file e.g.
+           - url (string) : url string of the file e.g.
               - 'input.txt'
-              - pathlib.Path('input.txt')
               - 'file:///scratch/proj101/input.txt'
               - 'globus://go#ep1/~/data/input.txt'
               - 'globus://ddb59aef-6d04-11e5-ba46-22000b92c6ec/home/johndoe/data/input.txt'
         """
-        self.url = str(url)
+        self.url = url
         parsed_url = urlparse(self.url)
         self.scheme = parsed_url.scheme if parsed_url.scheme else 'file'
         self.netloc = parsed_url.netloc
         self.path = parsed_url.path
         self.filename = os.path.basename(self.path)
         self.local_path: Optional[str] = None
```

### Comparing `parsl-2023.7.17/parsl/data_provider/ftp.py` & `parsl-2023.7.3/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/data_provider/globus.py` & `parsl-2023.7.3/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/data_provider/http.py` & `parsl-2023.7.3/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/data_provider/rsync.py` & `parsl-2023.7.3/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/data_provider/staging.py` & `parsl-2023.7.3/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/dflow.py` & `parsl-2023.7.3/parsl/dataflow/dflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,20 +376,14 @@
                     # something we can't join on.
                     if isinstance(joinable, Future):
                         self.update_task_state(task_record, States.joining)
                         task_record['joins'] = joinable
                         task_record['join_lock'] = threading.Lock()
                         self._send_task_log_info(task_record)
                         joinable.add_done_callback(partial(self.handle_join_update, task_record))
-                    elif joinable == []:  # got a list, but it had no entries, and specifically, no Futures.
-                        self.update_task_state(task_record, States.joining)
-                        task_record['joins'] = joinable
-                        task_record['join_lock'] = threading.Lock()
-                        self._send_task_log_info(task_record)
-                        self.handle_join_update(task_record, None)
                     elif isinstance(joinable, list) and [j for j in joinable if not isinstance(j, Future)] == []:
                         self.update_task_state(task_record, States.joining)
                         task_record['joins'] = joinable
                         task_record['join_lock'] = threading.Lock()
                         self._send_task_log_info(task_record)
                         for inner_future in joinable:
                             inner_future.add_done_callback(partial(self.handle_join_update, task_record))
@@ -405,15 +399,15 @@
         self._log_std_streams(task_record)
 
         # it might be that in the course of the update, we've gone back to being
         # pending - in which case, we should consider ourself for relaunch
         if task_record['status'] == States.pending:
             self.launch_if_ready(task_record)
 
-    def handle_join_update(self, task_record: TaskRecord, inner_app_future: Optional[AppFuture]) -> None:
+    def handle_join_update(self, task_record: TaskRecord, inner_app_future: AppFuture) -> None:
         with task_record['join_lock']:
             # inner_app_future has completed, which is one (potentially of many)
             # futures the outer task is joining on.
 
             # If the outer task is joining on a single future, then
             # use the result of the inner_app_future as the final result of
             # the outer app future.
```

### Comparing `parsl-2023.7.17/parsl/dataflow/errors.py` & `parsl-2023.7.3/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/futures.py` & `parsl-2023.7.3/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/job_error_handler.py` & `parsl-2023.7.3/parsl/dataflow/job_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/job_status_poller.py` & `parsl-2023.7.3/parsl/dataflow/job_status_poller.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/memoization.py` & `parsl-2023.7.3/parsl/dataflow/memoization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 import hashlib
 from functools import lru_cache, singledispatch
 import logging
-import pickle
 from parsl.dataflow.taskrecord import TaskRecord
 
 from typing import Dict, Any, List, Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from parsl import DataFlowKernel  # import loop at runtime - needed for typechecking - TODO turn into "if typing:"
 
 from concurrent.futures import Future
 
+from parsl.serialize import serialize
 import types
 
 logger = logging.getLogger(__name__)
 
 
 @singledispatch
 def id_for_memo(obj: object, output_ref: bool = False) -> bytes:
@@ -50,42 +50,42 @@
     raise ValueError("unknown type for memoization: {}".format(type(obj)))
 
 
 @id_for_memo.register(str)
 @id_for_memo.register(int)
 @id_for_memo.register(float)
 @id_for_memo.register(type(None))
-def id_for_memo_pickle(obj: object, output_ref: bool = False) -> bytes:
-    return pickle.dumps(obj)
+def id_for_memo_serialize(obj: object, output_ref: bool = False) -> bytes:
+    return serialize(obj)
 
 
 @id_for_memo.register(list)
 def id_for_memo_list(denormalized_list: list, output_ref: bool = False) -> bytes:
     if type(denormalized_list) != list:
         raise ValueError("id_for_memo_list cannot work on subclasses of list")
 
     normalized_list = []
 
     for e in denormalized_list:
         normalized_list.append(id_for_memo(e, output_ref=output_ref))
 
-    return pickle.dumps(normalized_list)
+    return serialize(normalized_list)
 
 
 @id_for_memo.register(tuple)
 def id_for_memo_tuple(denormalized_tuple: tuple, output_ref: bool = False) -> bytes:
     if type(denormalized_tuple) != tuple:
         raise ValueError("id_for_memo_tuple cannot work on subclasses of tuple")
 
     normalized_list = []
 
     for e in denormalized_tuple:
         normalized_list.append(id_for_memo(e, output_ref=output_ref))
 
-    return pickle.dumps(normalized_list)
+    return serialize(normalized_list)
 
 
 @id_for_memo.register(dict)
 def id_for_memo_dict(denormalized_dict: dict, output_ref: bool = False) -> bytes:
     """This normalises the keys and values of the supplied dictionary.
 
     When output_ref=True, the values are normalised as output refs, but
@@ -96,27 +96,27 @@
 
     keys = sorted(denormalized_dict)
 
     normalized_list = []
     for k in keys:
         normalized_list.append(id_for_memo(k))
         normalized_list.append(id_for_memo(denormalized_dict[k], output_ref=output_ref))
-    return pickle.dumps(normalized_list)
+    return serialize(normalized_list)
 
 
 # the LRU cache decorator must be applied closer to the id_for_memo_function call
 # that the .register() call, so that the cache-decorated version is registered.
 @id_for_memo.register(types.FunctionType)
 @lru_cache()
 def id_for_memo_function(f: types.FunctionType, output_ref: bool = False) -> bytes:
     """This will checkpoint a function based only on its name and module name.
     This means that changing source code (other than the function name) will
     not cause a checkpoint invalidation.
     """
-    return pickle.dumps(["types.FunctionType", f.__name__, f.__module__])
+    return serialize(["types.FunctionType", f.__name__, f.__module__])
 
 
 class Memoizer:
     """Memoizer is responsible for ensuring that identical work is not repeated.
 
     When a task is repeated, i.e., the same function is called with the same exact arguments, the
     result from a previous execution is reused. `wiki <https://en.wikipedia.org/wiki/Memoization>`_
```

### Comparing `parsl-2023.7.17/parsl/dataflow/rundirs.py` & `parsl-2023.7.3/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/states.py` & `parsl-2023.7.3/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/strategy.py` & `parsl-2023.7.3/parsl/dataflow/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/dataflow/taskrecord.py` & `parsl-2023.7.3/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/errors.py` & `parsl-2023.7.3/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/base.py` & `parsl-2023.7.3/parsl/executors/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/errors.py` & `parsl-2023.7.3/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.7.3/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/flux/executor.py` & `parsl-2023.7.3/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.7.3/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/high_throughput/executor.py` & `parsl-2023.7.3/parsl/executors/high_throughput/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,17 +591,18 @@
 
         try:
             fn_buf = pack_apply_message(func, args, kwargs,
                                         buffer_threshold=1024 * 1024)
         except TypeError:
             raise SerializationError(func.__name__)
 
-        msg = {"task_id": task_id, "buffer": fn_buf}
+        msg = {"task_id": task_id,
+               "buffer": fn_buf}
 
-        # Post task to the outgoing queue
+        # Post task to the the outgoing queue
         self.outgoing_q.put(msg)
 
         # Return the future
         return fut
 
     def create_monitoring_info(self, status):
         """ Create a msg for monitoring based on the poll status
```

### Comparing `parsl-2023.7.17/parsl/executors/high_throughput/interchange.py` & `parsl-2023.7.3/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/high_throughput/probe.py` & `parsl-2023.7.3/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.7.3/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,26 +366,26 @@
                     logger.debug("Result send: No items to push")
             else:
                 logger.debug(f"Result send: check condition not met - deferring {len(items)} result items")
 
         logger.critical("Exiting")
 
     @wrap_with_logs
-    def worker_watchdog(self, kill_event: threading.Event):
+    def worker_watchdog(self, kill_event):
         """Keeps workers alive.
 
         Parameters:
         -----------
         kill_event : threading.Event
               Event to let the thread know when it is time to die.
         """
 
         logger.debug("Starting worker watchdog")
 
-        while not kill_event.wait(self.heartbeat_period):
+        while not kill_event.is_set():
             for worker_id, p in self.procs.items():
                 if not p.is_alive():
                     logger.error("Worker {} has died".format(worker_id))
                     try:
                         task = self._tasks_in_progress.pop(worker_id)
                         logger.info("Worker {} was busy when it died".format(worker_id))
                         try:
@@ -405,14 +405,15 @@
                                                             self.pending_result_queue,
                                                             self.ready_worker_queue,
                                                             self._tasks_in_progress,
                                                             self.cpu_affinity),
                                        name="HTEX-Worker-{}".format(worker_id))
                     self.procs[worker_id] = p
                     logger.info("Worker {} has been restarted".format(worker_id))
+                time.sleep(self.heartbeat_period)
 
         logger.critical("Exiting")
 
     def start(self):
         """ Start the worker processes.
 
         TODO: Move task receiving to a thread
```

### Comparing `parsl-2023.7.17/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.7.3/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/status_handling.py` & `parsl-2023.7.3/parsl/executors/status_handling.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2023.7.3/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/taskvine/executor.py` & `parsl-2023.7.3/parsl/executors/taskvine/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/threads.py` & `parsl-2023.7.3/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2023.7.3/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/workqueue/executor.py` & `parsl-2023.7.3/parsl/executors/workqueue/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.7.3/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/launchers/__init__.py` & `parsl-2023.7.3/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/launchers/base.py` & `parsl-2023.7.3/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/launchers/launchers.py` & `parsl-2023.7.3/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/log_utils.py` & `parsl-2023.7.3/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/db_manager.py` & `parsl-2023.7.3/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/monitoring.py` & `parsl-2023.7.3/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/queries/pandas.py` & `parsl-2023.7.3/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/radios.py` & `parsl-2023.7.3/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/remote.py` & `parsl-2023.7.3/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/types.py` & `parsl-2023.7.3/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/app.py` & `parsl-2023.7.3/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/models.py` & `parsl-2023.7.3/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.7.3/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.7.3/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.7.3/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/monitoring/visualization/views.py` & `parsl-2023.7.3/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/multiprocessing.py` & `parsl-2023.7.3/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/process_loggers.py` & `parsl-2023.7.3/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/__init__.py` & `parsl-2023.7.3/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.7.3/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/aws/aws.py` & `parsl-2023.7.3/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/azure/azure.py` & `parsl-2023.7.3/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/base.py` & `parsl-2023.7.3/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/cluster_provider.py` & `parsl-2023.7.3/parsl/providers/cluster_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from abc import abstractmethod
 from string import Template
 
 from parsl.providers.errors import SchedulerMissingArgs, ScriptPathError
-from parsl.launchers.base import Launcher
 from parsl.launchers.errors import BadLauncher
 from parsl.providers.base import ExecutionProvider
 
 logger = logging.getLogger(__name__)
 
 
 class ClusterProvider(ExecutionProvider):
@@ -63,15 +62,15 @@
         self.init_blocks = init_blocks
         self.min_blocks = min_blocks
         self.max_blocks = max_blocks
         self.parallelism = parallelism
         self.launcher = launcher
         self.walltime = walltime
         self.cmd_timeout = cmd_timeout
-        if not isinstance(self.launcher, Launcher):
+        if not callable(self.launcher):
             raise BadLauncher(self.launcher)
 
         self.script_dir = None
 
         # Dictionary that keeps track of jobs, keyed on job_id
         self.resources = {}
```

### Comparing `parsl-2023.7.17/parsl/providers/cobalt/cobalt.py` & `parsl-2023.7.3/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/condor/condor.py` & `parsl-2023.7.3/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/condor/template.py` & `parsl-2023.7.3/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/errors.py` & `parsl-2023.7.3/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.7.3/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.7.3/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/kubernetes/kube.py` & `parsl-2023.7.3/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/local/local.py` & `parsl-2023.7.3/parsl/providers/local/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
         job_id = None
         remote_pid = None
         if self._should_move_files():
             logger.debug("Pushing start script")
             script_path = self.channel.push_file(script_path, self.channel.script_dir)
 
-        logger.debug("Launching")
+        logger.debug("Launching in remote mode")
         # We need to capture the exit code and the streams, so we put them in files. We also write
         # '-' to the exit code file to isolate potential problems with writing to files in the
         # script directory
         #
         # The basic flow is:
         #   1. write "-" to the exit code file. If this fails, exit
         #   2. Launch the following sequence in the background:
```

### Comparing `parsl-2023.7.17/parsl/providers/lsf/lsf.py` & `parsl-2023.7.3/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/pbspro/pbspro.py` & `parsl-2023.7.3/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/slurm/slurm.py` & `parsl-2023.7.3/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/providers/torque/torque.py` & `parsl-2023.7.3/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/serialize/base.py` & `parsl-2023.7.3/parsl/serialize/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import abstractmethod
 import logging
+import functools
 
 from typing import Any
 
 logger = logging.getLogger(__name__)
 
 # GLOBALS
 METHODS_MAP_CODE = {}
@@ -27,23 +28,32 @@
 
     _identifier: bytes
     _for_code: bool
     _for_data: bool
 
     @property
     def identifier(self) -> bytes:
-        """Get that identifier that will be used to indicate in byte streams
-        that this class should be used for deserialization.
+        """ Get the identifier of the serialization method
 
         Returns
         -------
-        identifier : bytes
+        identifier : str
         """
         return self._identifier
 
+    def enable_caching(self, maxsize: int = 128) -> None:
+        """ Add functools.lru_cache onto the serialize, deserialize methods
+        """
+
+        # ignore types here because mypy at the moment is not fond of monkeypatching
+        self.serialize = functools.lru_cache(maxsize=maxsize)(self.serialize)  # type: ignore[method-assign]
+        self.deserialize = functools.lru_cache(maxsize=maxsize)(self.deserialize)  # type: ignore[method-assign]
+
+        return
+
     @abstractmethod
     def serialize(self, data: Any) -> bytes:
         pass
 
     @abstractmethod
     def deserialize(self, payload: bytes) -> Any:
         pass
```

### Comparing `parsl-2023.7.17/parsl/serialize/concretes.py` & `parsl-2023.7.3/parsl/serialize/concretes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import dill
-import functools
 import pickle
 import logging
 
 logger = logging.getLogger(__name__)
 from parsl.serialize.base import SerializerBase
 
 from typing import Any
@@ -11,18 +10,19 @@
 
 class PickleSerializer(SerializerBase):
     """ Pickle serialization covers most python objects, with some notable exceptions:
 
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * closures, generators and coroutines
+    * [sometimes] issues with wrapped/decorated functions
     """
 
     _identifier = b'01'
-    _for_code = False
+    _for_code = True
     _for_data = True
 
     def serialize(self, data: Any) -> bytes:
         return pickle.dumps(data)
 
     def deserialize(self, body: bytes) -> Any:
         return pickle.loads(body)
@@ -37,34 +37,15 @@
     * functions defined in a interpreter/notebook
     * classes defined in local context and not importable using a fully qualified name
     * functions that are wrapped/decorated by other functions/classes
     * closures
     """
 
     _identifier = b'02'
-    _for_code = False
-    _for_data = True
-
-    def serialize(self, data: Any) -> bytes:
-        return dill.dumps(data)
-
-    def deserialize(self, body: bytes) -> Any:
-        return dill.loads(body)
-
-
-class DillCallableSerializer(SerializerBase):
-    """This serializer is a variant of the DillSerializer that will
-    serialize and deserialize callables using an lru_cache, under the
-    assumption that callables are immutable and so can be cached.
-    """
-
-    _identifier = b'C2'
     _for_code = True
-    _for_data = False
+    _for_data = True
 
-    @functools.lru_cache
     def serialize(self, data: Any) -> bytes:
         return dill.dumps(data)
 
-    @functools.lru_cache
     def deserialize(self, body: bytes) -> Any:
         return dill.loads(body)
```

### Comparing `parsl-2023.7.17/parsl/serialize/facade.py` & `parsl-2023.7.3/parsl/serialize/facade.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from parsl.serialize.concretes import *  # noqa: F403,F401
-from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE
+from parsl.serialize.base import METHODS_MAP_DATA, METHODS_MAP_CODE, SerializerBase
 import logging
 
-from typing import Any, List, Union
+from typing import Any, Dict, List, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
 """ Instantiate the appropriate classes
 """
 methods_for_code = {}
 methods_for_data = {}
 
 for key in METHODS_MAP_CODE:
     methods_for_code[key] = METHODS_MAP_CODE[key]()
+    methods_for_code[key].enable_caching(maxsize=128)
 
 for key in METHODS_MAP_DATA:
     methods_for_data[key] = METHODS_MAP_DATA[key]()
 
 
+def _list_methods() -> Tuple[Dict[bytes, SerializerBase], Dict[bytes, SerializerBase]]:
+    return methods_for_code, methods_for_data
+
+
 def pack_apply_message(func: Any, args: Any, kwargs: Any, buffer_threshold: int = int(128 * 1e6)) -> bytes:
     """Serialize and pack function and parameters
 
     Parameters
     ----------
 
     func: Function
@@ -56,26 +61,31 @@
     """ Try available serialization methods one at a time
 
     Individual serialization methods might raise a TypeError (eg. if objects are non serializable)
     This method will raise the exception from the last method that was tried, if all methods fail.
     """
     result: Union[bytes, Exception]
     if callable(obj):
-        methods = methods_for_code
+        for method in methods_for_code.values():
+            try:
+                result = method._identifier + b'\n' + method.serialize(obj)
+            except Exception as e:
+                result = e
+                continue
+            else:
+                break
     else:
-        methods = methods_for_data
-
-    for method in methods.values():
-        try:
-            result = method._identifier + b'\n' + method.serialize(obj)
-        except Exception as e:
-            result = e
-            continue
-        else:
-            break
+        for method in methods_for_data.values():
+            try:
+                result = method._identifier + b'\n' + method.serialize(obj)
+            except Exception as e:
+                result = e
+                continue
+            else:
+                break
 
     if isinstance(result, BaseException):
         raise result
     else:
         if len(result) > buffer_threshold:
             logger.warning(f"Serialized object exceeds buffer threshold of {buffer_threshold} bytes, this could cause overflows")
         return result
```

### Comparing `parsl-2023.7.17/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.7.3/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/azure_single_node.py` & `parsl-2023.7.3/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/bluewaters.py` & `parsl-2023.7.3/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/bridges.py` & `parsl-2023.7.3/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.7.3/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/comet.py` & `parsl-2023.7.3/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/cooley_htex.py` & `parsl-2023.7.3/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.7.3/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/ec2_spot.py` & `parsl-2023.7.3/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/frontera.py` & `parsl-2023.7.3/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.7.3/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/htex_local.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.7.3/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.7.3/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/midway.py` & `parsl-2023.7.3/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.7.3/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/osg_htex.py` & `parsl-2023.7.3/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/petrelkube.py` & `parsl-2023.7.3/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/summit.py` & `parsl-2023.7.3/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/swan_htex.py` & `parsl-2023.7.3/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/theta.py` & `parsl-2023.7.3/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/configs/user_opts.py` & `parsl-2023.7.3/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/latency.py` & `parsl-2023.7.3/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.7.3/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.7.3/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.7.3/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.7.3/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/scaling_tests/htex_local.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/scaling_tests/test_scale.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2023.7.3/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.7.3/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/site_tests/test_provider.py` & `parsl-2023.7.3/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/site_tests/test_site.py` & `parsl-2023.7.3/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_affinity.py` & `parsl-2023.7.3/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_concurrent.py` & `parsl-2023.7.3/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.7.3/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_ec2.py` & `parsl-2023.7.3/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.7.3/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_start_method.py` & `parsl-2023.7.3/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/sites/test_worker_info.py` & `parsl-2023.7.3/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_aalst_patterns.py` & `parsl-2023.7.3/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_basic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,115 @@
+import argparse
 import os
+import pytest
+import shutil
+import time
 import random
 import re
 
-import pytest
-
 import parsl
 from parsl import File
 from parsl.app.app import bash_app
 
+from parsl.tests.configs.local_threads import config
+
 
 @bash_app
-def echo_to_file(inputs=(), outputs=(), stderr=None, stdout=None):
+def echo_to_file(inputs=[], outputs=[], stderr='std.err', stdout='std.out'):
     res = ""
-    for o in outputs:
-        for i in inputs:
+    for i in inputs:
+        for o in outputs:
             res += "echo {} >& {}".format(i, o)
     return res
 
 
 @bash_app
 def foo(x, y, z=10, stdout=None, label=None):
-    return f"echo {x} {y} {z}"
+    return """echo {0} {1} {z}
+    """.format(x, y, z=z)
 
 
 @pytest.mark.issue363
-def test_command_format_1(tmpd_cwd):
-    """Testing command format for BashApps"""
+def test_command_format_1():
+    """Testing command format for BashApps
+    """
 
-    outdir = tmpd_cwd / "outputs"
-    outdir.mkdir()
-    stdout = outdir / "foo-std.out"
+    outdir = os.path.abspath('outputs')
+    stdout = os.path.join(outdir, 'foo-std.out')
+    if os.path.exists(stdout):
+        os.remove(stdout)
+
+    foo_future = foo(1, 4, stdout=stdout)
+    print("[test_command_format_1] foo_future: ", foo_future)
+    contents = None
 
-    foo_future = foo(1, 4, stdout=str(stdout))
-    assert foo_future.result() == 0, "BashApp had non-zero exit code"
+    assert foo_future.result() == 0, "BashApp exited with an error code : {0}".format(
+        foo_future.result())
 
-    so_content = stdout.read_text().strip()
-    assert so_content == "1 4 10"
+    with open(stdout, 'r') as stdout_f:
+        contents = stdout_f.read()
+
+    assert contents == '1 4 10\n', 'Output does not match expected string "1 4 10", Got: "{0}"'.format(
+        contents)
+    return True
 
 
 @pytest.mark.issue363
 def test_auto_log_filename_format():
     """Testing auto log filename format for BashApps
     """
     app_label = "label_test_auto_log_filename_format"
     rand_int = random.randint(1000, 1000000000)
 
     foo_future = foo(1, rand_int, stdout=parsl.AUTO_LOGNAME, label=app_label)
+    print("[test_auto_log_filename_format] foo_future: ", foo_future)
+    contents = None
 
     assert foo_future.result() == 0, "BashApp exited with an error code : {0}".format(
         foo_future.result())
 
     log_fpath = foo_future.stdout
     log_pattern = fr".*/task_\d+_foo_{app_label}"
     assert re.match(log_pattern, log_fpath), 'Output file "{0}" does not match pattern "{1}"'.format(
         log_fpath, log_pattern)
     assert os.path.exists(log_fpath), 'Output file does not exist "{0}"'.format(log_fpath)
     with open(log_fpath, 'r') as stdout_f:
         contents = stdout_f.read()
 
     assert contents == '1 {0} 10\n'.format(rand_int), \
         'Output does not match expected string "1 {0} 10", Got: "{1}"'.format(rand_int, contents)
+    return True
 
 
 @pytest.mark.issue363
-def test_parallel_for(tmpd_cwd, n=3):
-    """Testing a simple parallel for loop"""
-    outdir = tmpd_cwd / "outputs/test_parallel"
-    outdir.mkdir(parents=True)
-    futs = [
-        echo_to_file(
-            inputs=[f"Hello World {i}"],
-            outputs=[File(str(outdir / f"out.{i}.txt"))],
-            stdout=str(outdir / f"std.{i}.out"),
-            stderr=str(outdir / f"std.{i}.err"),
+def test_parallel_for(n=3):
+    """Testing a simple parallel for loop
+    """
+    outdir = os.path.join(os.path.abspath('outputs'), 'test_parallel')
+    if not os.path.exists(outdir):
+        os.makedirs(outdir)
+    else:
+        shutil.rmtree(outdir)
+        os.makedirs(outdir)
+
+    d = {}
+
+    start = time.time()
+    for i in range(0, n):
+        d[i] = echo_to_file(
+            inputs=['Hello World {0}'.format(i)],
+            outputs=[File('{0}/out.{1}.txt'.format(outdir, i))],
+            stdout='{0}/std.{1}.out'.format(outdir, i),
+            stderr='{0}/std.{1}.err'.format(outdir, i),
         )
-        for i in range(n)
-    ]
 
-    for f in futs:
-        f.result()
+    assert len(
+        d.keys()) == n, "Only {0}/{1} keys in dict".format(len(d.keys()), n)
 
-    stdout_file_count = len(list(outdir.glob("*.out")))
-    assert stdout_file_count == n, sorted(outdir.iterdir())
+    [d[i].result() for i in d]
+    print("Duration : {0}s".format(time.time() - start))
+    stdout_file_count = len(
+        [item for item in os.listdir(outdir) if item.endswith('.out')])
+    assert stdout_file_count == n, "Only {0}/{1} files in '{2}' ".format(len(os.listdir('outputs/')),
+                                                                         n, outdir)
+    print("[TEST STATUS] test_parallel_for [SUCCESS]")
+    return d
```

### Comparing `parsl-2023.7.17/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.7.3/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import argparse
 import os
 
 import pytest
 
+import parsl
 import parsl.app.errors as perror
 from parsl.app.app import bash_app
+from parsl.tests.configs.local_threads import config
 
 
 @bash_app
-def echo_to_streams(msg, stderr=None, stdout=None):
+def echo_to_streams(msg, stderr='std.err', stdout='std.out'):
     return 'echo "{0}"; echo "{0}" >&2'.format(msg)
 
 
 whitelist = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'configs', '*threads*')
 
 speclist = (
     '/bad/dir/t.out',
@@ -33,68 +36,80 @@
     'bad_mode'
 ]
 
 
 @pytest.mark.issue363
 @pytest.mark.parametrize('spec', speclist, ids=testids)
 def test_bad_stdout_specs(spec):
-    """Testing bad stdout spec cases"""
+    """Testing bad stdout spec cases
+    """
 
     fn = echo_to_streams("Hello world", stdout=spec, stderr='t.err')
 
     try:
         fn.result()
     except Exception as e:
         assert isinstance(e, TypeError) or isinstance(e, perror.BadStdStreamFile), "Exception is wrong type"
     else:
         assert False, "Did not raise expected exception"
 
+    return
+
 
 @pytest.mark.issue363
 def test_bad_stderr_file():
-    """Testing bad stderr file"""
 
+    """ Testing bad stderr file """
+
+    out = "t2.out"
     err = "/bad/dir/t2.err"
 
-    fn = echo_to_streams("Hello world", stderr=err)
+    fn = echo_to_streams("Hello world", stdout=out, stderr=err)
 
     try:
         fn.result()
     except perror.BadStdStreamFile:
         pass
     else:
         assert False, "Did not raise expected exception BadStdStreamFile"
 
     return
 
 
 @pytest.mark.issue363
-def test_stdout_truncate(tmpd_cwd):
-    """Testing truncation of prior content of stdout"""
+def test_stdout_truncate():
+
+    """ Testing truncation of prior content of stdout """
 
-    out = (str(tmpd_cwd / 't1.out'), 'w')
-    err = str(tmpd_cwd / 't1.err')
+    out = ('t1.out', 'w')
+    err = 't1.err'
+    os.system('rm -f ' + out[0] + ' ' + err)
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len1 = len(open(out[0]).readlines())
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out[0]).readlines())
 
-    assert len1 == 1
-    assert len1 == len2
+    assert len1 == len2 == 1, "Line count of output files should both be 1, but: len1={} len2={}".format(len1, len2)
+
+    os.system('rm -f ' + out[0] + ' ' + err)
 
 
 @pytest.mark.issue363
-def test_stdout_append(tmpd_cwd):
-    """Testing appending to prior content of stdout (default open() mode)"""
+def test_stdout_append():
+
+    """ Testing appending to prior content of stdout (default open() mode) """
 
-    out = str(tmpd_cwd / 't1.out')
-    err = str(tmpd_cwd / 't1.err')
+    out = 't1.out'
+    err = 't1.err'
+    os.system('rm -f ' + out + ' ' + err)
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len1 = len(open(out).readlines())
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out).readlines())
 
-    assert len1 == 1 and len2 == 2
+    assert len1 == 1 and len2 == 2, "Line count of output files should be 1 and 2, but:  len1={} len2={}".format(len1, len2)
+
+    os.system('rm -f ' + out + ' ' + err)
```

### Comparing `parsl-2023.7.17/parsl/tests/test_callables.py` & `parsl-2023.7.3/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.7.3/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.7.3/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_data/test_file.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file_apps.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,51 +8,53 @@
 def cat(inputs=(), outputs=(), stdout=None, stderr=None):
     infiles = " ".join(i.filepath for i in inputs)
     return f"cat {infiles} &> {outputs[0]}"
 
 
 @pytest.mark.staging_required
 def test_files(setup_data):
-    fs = sorted(setup_data / f for f in setup_data.iterdir())
+    fs = sorted(str(setup_data / f) for f in setup_data.iterdir())
     fs = list(map(File, fs))
     x = cat(
         inputs=fs,
-        outputs=[File(setup_data / "cat_out.txt")],
-        stdout=setup_data / "f_app.out",
-        stderr=setup_data / "f_app.err",
+        outputs=[File(str(setup_data / "cat_out.txt"))],
+        stdout=str(setup_data / "f_app.out"),
+        stderr=str(setup_data / "f_app.err"),
     )
     x.result()
     d_x = x.outputs[0]
     data = open(d_x.filepath).read().strip()
     assert "1\n2" == data, "Per setup_data fixture"
 
 
 @bash_app
 def increment(inputs=(), outputs=(), stdout=None, stderr=None):
-    return (
-        f"x=$(cat {inputs[0]})\n"
-        f"echo $(($x+1)) > {outputs[0]}"
-    )
+    # Place double braces to avoid python complaining about missing keys for {item = $1}
+    return """
+    x=$(cat {i})
+    echo $(($x+1)) > {o}
+    """.format(i=inputs[0], o=outputs[0])
 
 
 @pytest.mark.staging_required
 def test_increment(tmp_path, depth=5):
-    """Test simple pipeline A->B...->N"""
+    """Test simple pipeline A->B...->N
+    """
     # Test setup
     first_fpath = tmp_path / "test0.txt"
     first_fpath.write_text("0\n")
 
-    prev = [File(first_fpath)]
+    prev = [File(str(first_fpath))]
     futs = []
     for i in range(1, depth):
         f = increment(
             inputs=prev,
-            outputs=[File(tmp_path / f"test{i}.txt")],
-            stdout=tmp_path / f"incr{i}.out",
-            stderr=tmp_path / f"incr{i}.err",
+            outputs=[File(str(tmp_path / f"test{i}.txt"))],
+            stdout=str(tmp_path / f"incr{i}.out"),
+            stderr=str(tmp_path / f"incr{i}.err"),
         )
         prev = f.outputs
         futs.append((i, prev[0]))
 
     for i, f in futs:
         data = open(f.result().filepath).read().strip()
         assert data == str(i)
```

### Comparing `parsl-2023.7.17/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.7.3/parsl/tests/test_data/test_file_staging.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from parsl.app.app import bash_app
 from parsl.data_provider.files import File
 
 
 @bash_app
 def cat(inputs=(), outputs=(), stdout=None, stderr=None):
     infiles = " ".join(i.filepath for i in inputs)
-    return f"cat {infiles} &> {outputs[0]}"
+    return f"cat {infiles} &> {outputs[0]}\n"
 
 
 @pytest.mark.staging_required
 def test_regression_200(tmp_path):
     """Regression test for #200. Pickleablility of Files"""
     opath = tmp_path / "test_output.txt"
     fpath = tmp_path / "test.txt"
 
     fpath.write_text("Hello World")
-    f = cat(inputs=[File(fpath)], outputs=[File(opath)])
+    f = cat(inputs=[File(str(fpath))], outputs=[File(str(opath))])
 
     f.result()
     with open(f.outputs[0].filepath) as f:
         data = f.read()
         assert "Hello World" == data
```

### Comparing `parsl-2023.7.17/parsl/tests/test_data/test_output_chain_filenames.py` & `parsl-2023.7.3/parsl/tests/test_data/test_output_chain_filenames.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,46 @@
-from concurrent.futures import Future
+import argparse
+import os
+
+import pytest
+
+import parsl
 
+from concurrent.futures import Future
 from parsl import File
 from parsl.app.app import bash_app
 
 
 @bash_app
-def app1(inputs=(), outputs=(), stdout=None, stderr=None, mock=False):
-    return f"echo 'test' > {outputs[0]}"
+def app1(inputs=[], outputs=[], stdout=None, stderr=None, mock=False):
+    cmd_line = f"""echo 'test' > {outputs[0]}"""
+    return cmd_line
 
 
 @bash_app
-def app2(inputs=(), outputs=(), stdout=None, stderr=None, mock=False):
-    return f"echo '{inputs[0]}' > {outputs[0]}"
+def app2(inputs=[], outputs=[], stdout=None, stderr=None, mock=False):
+
+    with open('somefile.txt', 'w') as f:
+        f.write("%s\n" % inputs[0])
+    cmd_line = f"""echo '{inputs[0]}' > {outputs[0]}"""
+    return cmd_line
 
 
-def test_behavior(tmpd_cwd):
-    expected_path = str(tmpd_cwd / "simple-out.txt")
-    app1_future = app1(
-        inputs=[],
-        outputs=[File(expected_path)]
-    )
+def test_behavior():
+    app1_future = app1(inputs=[],
+                       outputs=[File("simple-out.txt")])
 
     o = app1_future.outputs[0]
     assert isinstance(o, Future)
 
-    app2_future = app2(
-        inputs=[o],
-        outputs=[File(str(tmpd_cwd / "simple-out2.txt"))]
-    )
+    app2_future = app2(inputs=[o],
+                       outputs=[File("simple-out2.txt")])
     app2_future.result()
 
+    expected_name = 'b'
+    with open('somefile.txt', 'r') as f:
+        name = f.read()
+
     with open(app2_future.outputs[0].filepath, 'r') as f:
-        name = f.read().strip()
+        expected_name = f.read()
 
-    assert name == expected_path, "Filename mangled due to DataFuture handling"
+    assert name == expected_name, "Filename mangled due to DataFuture handling"
```

### Comparing `parsl-2023.7.17/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.7.3/parsl/tests/test_docs/test_workflow4.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,53 @@
-import pytest
+import os
+import parsl
 
 from parsl.app.app import bash_app, python_app
+from parsl.tests.configs.local_threads import config
 from parsl.data_provider.files import File
 
+import pytest
+
+# parsl.set_stream_logger()
+
 
 @bash_app
-def generate(outputs=()):
-    return "echo 1 &> {o}".format(o=outputs[0])
+def generate(outputs=[]):
+    return "echo $(( RANDOM % (10 - 5 + 1 ) + 5 )) &> {o}".format(o=outputs[0])
 
 
 @bash_app
-def concat(inputs=(), outputs=(), stdout=None, stderr=None):
+def concat(inputs=[], outputs=[], stdout="stdout.txt", stderr='stderr.txt'):
     return "cat {0} >> {1}".format(" ".join(map(lambda x: x.filepath, inputs)), outputs[0])
 
 
 @python_app
-def total(inputs=()):
-    with open(inputs[0].filepath, "r") as f:
-        return sum(int(line) for line in f)
+def total(inputs=[]):
+    total = 0
+    with open(inputs[0].filepath, 'r') as f:
+        for line in f:
+            total += int(line)
+    return total
 
 
 @pytest.mark.staging_required
-@pytest.mark.parametrize("width", (5, 10, 15))
-def test_parallel_dataflow(tmpd_cwd, width):
+def test_parallel_dataflow():
     """Test parallel dataflow from docs on Composing workflows
     """
 
+    if os.path.exists('all.txt'):
+        os.remove('all.txt')
+
     # create 5 files with random numbers
-    output_files = [
-        generate(outputs=[File(str(tmpd_cwd / f"random-{i}.txt"))])
-        for i in range(width)
-    ]
+    output_files = []
+    for i in range(5):
+        if os.path.exists('random-%s.txt' % i):
+            os.remove('random-%s.txt' % i)
+        output_files.append(generate(outputs=[File('random-%s.txt' % i)]))
 
     # concatenate the files into a single file
-    cc = concat(
-        inputs=[i.outputs[0] for i in output_files],
-        outputs=[File(str(tmpd_cwd / "all.txt"))]
-    )
+    cc = concat(inputs=[i.outputs[0]
+                        for i in output_files], outputs=[File("all.txt")])
 
     # calculate the average of the random numbers
     totals = total(inputs=[cc.outputs[0]])
-    assert totals.result() == len(output_files)
+    print(totals.result())
```

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import pytest
 
+import parsl
 from parsl.app.app import python_app
+from parsl.tests.configs.htex_local import fresh_config
+
 from parsl.executors.high_throughput.errors import WorkerLost
 
 
-def local_config():
-    from parsl.tests.configs.htex_local import fresh_config
+def local_setup():
     config = fresh_config()
     config.executors[0].poll_period = 1
     config.executors[0].max_workers = 1
-    config.executors[0].heartbeat_period = 1
-    return config
+    parsl.load(config)
+
+
+def local_teardown():
+    parsl.dfk().cleanup()
+    parsl.clear()
 
 
 @python_app
 def kill_worker():
-    raise SystemExit(2)
+    import sys
+    sys.exit(2)
 
 
 @pytest.mark.local
 def test_htex_worker_failure():
     with pytest.raises(WorkerLost):
         f = kill_worker()
         f.result()
```

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.7.3/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_flux.py` & `parsl-2023.7.3/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2023.7.3/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.7.3/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-import threading
+import parsl
 import time
 
-import pytest
-
-import parsl
 from parsl.app.app import python_app
-from parsl.tests.configs.local_threads import fresh_config as local_config  # noqa
 
 
 @python_app
-def slow_double(x, may_continue: threading.Event):
-    may_continue.wait()
+def slow_double(x):
+    import time
+    time.sleep(0.1)
     return x * 2
 
 
-@pytest.mark.local
 def test_garbage_collect():
     """ Launches an app with a dependency and waits till it's done and asserts that
     the internal refs were wiped
     """
-    evt = threading.Event()
-    x = slow_double(10, evt)
-    x = slow_double(x, evt)
+    x = slow_double(slow_double(10))
 
-    assert parsl.dfk().tasks[x.tid]['app_fu'] == x, "Tasks table should have app_fu ref before done"
+    if x.done() is False:
+        assert parsl.dfk().tasks[x.tid]['app_fu'] == x, "Tasks table should have app_fu ref before done"
 
-    evt.set()
-    assert x.result() == 10 * 4
+    x.result()
     if parsl.dfk().checkpoint_mode is not None:
         # We explicit call checkpoint if checkpoint_mode is enabled covering
         # cases like manual/periodic where checkpointing may be deferred.
         parsl.dfk().checkpoint()
 
-    time.sleep(0.01)  # Give enough time for task wipes to work
+    time.sleep(0.2)  # Give enough time for task wipes to work
     assert x.tid not in parsl.dfk().tasks, "Task record should be wiped after task completion"
```

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_join.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import pytest
+import time
 
 from parsl import join_app, python_app
 from parsl.dataflow.errors import JoinError
 
+from parsl.tests.configs.local_threads import fresh_config as local_config
 
 RESULT_CONSTANT = 3
 
 
-@python_app
+@python_app(cache=True)
 def inner_app():
+    time.sleep(1)
     return RESULT_CONSTANT
 
 
 @join_app
 def outer_app():
     fut = inner_app()
     return fut
@@ -27,25 +30,32 @@
 def combine(*args):
     """Wait for an arbitrary list of futures and return them as a list"""
     return list(args)
 
 
 @join_app
 def outer_make_a_dag_combine(n):
-    return combine(*(inner_app() for _ in range(n)))
+    futs = []
+    for _ in range(n):
+        futs.append(inner_app())
+    return combine(*futs)
 
 
 @join_app
 def outer_make_a_dag_multi(n):
-    return [inner_app() for _ in range(n)]
+    futs = []
+    for _ in range(n):
+        futs.append(inner_app())
+    return futs
 
 
 def test_result_flow():
     f = outer_app()
-    assert f.result() == RESULT_CONSTANT
+    res = f.result()
+    assert res == RESULT_CONSTANT
 
 
 @join_app
 def join_wrong_type_app():
     return 3
 
 
@@ -53,25 +63,28 @@
     f = join_wrong_type_app()
     with pytest.raises(TypeError):
         f.result()
 
 
 def test_dependency_on_joined():
     g = add_one(outer_app())
-    assert g.result() == RESULT_CONSTANT + 1
+    res = g.result()
+    assert res == RESULT_CONSTANT + 1
 
 
 def test_combine():
     f = outer_make_a_dag_combine(inner_app())
-    assert f.result() == [RESULT_CONSTANT] * RESULT_CONSTANT
+    res = f.result()
+    assert res == [RESULT_CONSTANT] * RESULT_CONSTANT
 
 
 def test_multiple_return():
     f = outer_make_a_dag_multi(inner_app())
-    assert f.result() == [RESULT_CONSTANT] * RESULT_CONSTANT
+    res = f.result()
+    assert res == [RESULT_CONSTANT] * RESULT_CONSTANT
 
 
 class InnerError(RuntimeError):
     pass
 
 
 @python_app
@@ -122,19 +135,7 @@
 
     assert isinstance(e, JoinError)
     assert len(e.dependent_exceptions_tids) == 1
 
     de0 = e.dependent_exceptions_tids[0][0]
     assert isinstance(de0, InnerError)
     assert de0.args[0] == "Error A"
-
-
-@join_app
-def app_no_futures():
-    return []
-
-
-def test_no_futures():
-    # tests that a list of futures that contains no futures will
-    # complete - regression test for issue #2792
-    f = app_no_futures()
-    assert f.result() == []
```

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 @python_app(cache=True)
 def noop_app(x, inputs=[], cache=True):
     return None
 
 
 @python_app
-def some_func(_t):
-    pass
+def sleep(t):
+    import time
+    time.sleep(t)
 
 
 def test_python_unmemoizable():
     """Testing behaviour when an unmemoizable parameter is used
     """
     fut = noop_app(Unmemoizable())
     with pytest.raises(ValueError):
@@ -46,18 +47,18 @@
     """
     fut = noop_app(FailingMemoizable())
     with pytest.raises(FailingMemoizerTestError):
         fut.result()
 
 
 def test_python_unmemoizable_after_dep():
-    memoizable_fut = some_func(1)
-    fut = noop_app(Unmemoizable(), inputs=[memoizable_fut])
+    sleep_fut = sleep(1)
+    fut = noop_app(Unmemoizable(), inputs=[sleep_fut])
     with pytest.raises(ValueError):
         fut.result()
 
 
 def test_python_failing_memoizer_afer_dep():
-    memoizable_fut = some_func(1)
-    fut = noop_app(FailingMemoizable(), inputs=[memoizable_fut])
+    sleep_fut = sleep(1)
+    fut = noop_app(FailingMemoizable(), inputs=[sleep_fut])
     with pytest.raises(ValueError):
         fut.result()
```

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import argparse
 
-import pytest
-
 import parsl
 from parsl.app.app import python_app
 from parsl.tests.configs.local_threads import config
 
 
 @python_app
 def increment(x):
     return x + 1
 
 
 @python_app
-def slow_increment(x):
+def slow_increment(x, dur):
     import time
-    time.sleep(0.001)
+    time.sleep(dur)
     return x + 1
 
 
-@pytest.mark.parametrize("depth", (2, 3))
-def test_increment(depth):
-    """Test simple pipeline A->B...->N"""
-    futs = [increment(0)]
-    futs.extend(increment(futs[i - 1]) for i in range(1, depth))
-    assert sum(f.result() for f in futs) == sum(range(1, depth + 1))
-
+def test_increment(depth=2):
+    """Test simple pipeline A->B...->N
+    """
+    futs = {0: 0}
+    for i in range(1, depth):
+        futs[i] = increment(futs[i - 1])
+
+    print([futs[i].result() for i in futs if not isinstance(futs[i], int)])
+
+
+def test_increment_slow(depth=2):
+    """Test simple pipeline A->B...->N with delay
+    """
+    futs = {0: 0}
+    for i in range(1, depth):
+        futs[i] = slow_increment(futs[i - 1], 0.5)
 
-@pytest.mark.parametrize("depth", (2, 3))
-def test_increment_slow(depth):
-    """Test simple pipeline A->B...->N with delay"""
-    futs = [slow_increment(0)]
-    futs.extend(slow_increment(futs[i - 1]) for i in range(1, depth))
-    assert sum(f.result() for f in futs) == sum(range(1, depth + 1))
+    print(futs[i])
+    print([futs[i].result() for i in futs if not isinstance(futs[i], int)])
```

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_timeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_python_apps/test_type5.py` & `parsl-2023.7.3/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_1480.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_1653.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_221.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_226.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_2652.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_69a.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_69b.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_69b.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_854.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2023.7.3/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2023.7.3/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-import threading
-
-import pytest
+# this test is intended to ensure that only one block is launched when only
+# one app is invoked. this is a regression test.
 
+import logging
 import parsl
 from parsl.channels import LocalChannel
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
 from parsl.launchers import SimpleLauncher
 from parsl.providers import LocalProvider
+import pytest
+
+
+logger = logging.getLogger(__name__)
 
 
 @parsl.python_app
 def app():
     import time
-    time.sleep(1)
+    time.sleep(45)
 
 
 class OneShotLocalProvider(LocalProvider):
     def __init__(self, *args, **kwargs):
+        logger.info("OneShotLocalProvider __init__ with MRO: {}".format(type(self).mro()))
         self.recorded_submits = 0
         super().__init__(*args, **kwargs)
 
     def submit(self, *args, **kwargs):
+        logger.info("OneShotLocalProvider submit")
         self.recorded_submits += 1
         return super().submit(*args, **kwargs)
 
     status_polling_interval = 600
 
 
 @pytest.mark.local
-def test_one_block(tmpd_cwd):
-    """
-    this test is intended to ensure that only one block is launched when only
-    one app is invoked. this is a regression test.
-    """
+def test_one_block():
+
     oneshot_provider = OneShotLocalProvider(
-        channel=LocalChannel(),
-        init_blocks=0,
-        min_blocks=0,
-        max_blocks=10,
-        launcher=SimpleLauncher(),
-    )
+                    channel=LocalChannel(),
+                    init_blocks=0,
+                    min_blocks=0,
+                    max_blocks=10,
+                    launcher=SimpleLauncher(),
+                )
 
     config = Config(
         executors=[
             HighThroughputExecutor(
                 label="htex_local",
-                address="127.0.0.1",
                 worker_debug=True,
                 cores_per_worker=1,
                 provider=oneshot_provider,
-                worker_logdir_root=str(tmpd_cwd)
             )
         ],
         strategy='simple',
     )
 
     parsl.load(config)
-    dfk = parsl.dfk()
-
-    def poller():
-        import time
-        while True:
-            dfk.job_status_poller.poll()
-            time.sleep(0.1)
 
-    threading.Thread(target=poller, daemon=True).start()
-    app().result()
+    f = app()
+    f.result()
     parsl.dfk().cleanup()
     parsl.clear()
 
     assert oneshot_provider.recorded_submits == 1
```

### Comparing `parsl-2023.7.17/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.7.3/parsl/tests/test_scaling/test_scale_down.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,80 @@
 import logging
-import time
-
-import pytest
-
 import parsl
+import pytest
+import time
+from parsl import python_app
 
-from parsl import File, python_app
 from parsl.providers import LocalProvider
 from parsl.channels import LocalChannel
+# from parsl.launchers import SimpleLauncher
 from parsl.launchers import SingleNodeLauncher
+
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
 
 logger = logging.getLogger(__name__)
 
-_max_blocks = 5
-_min_blocks = 2
-
 
 def local_config():
     return Config(
         executors=[
             HighThroughputExecutor(
-                heartbeat_period=1,
-                heartbeat_threshold=2,
-                poll_period=100,
+                heartbeat_period=2,
+                heartbeat_threshold=6,
+                poll_period=1,
                 label="htex_local",
-                address="127.0.0.1",
                 max_workers=1,
                 provider=LocalProvider(
                     channel=LocalChannel(),
                     init_blocks=0,
-                    max_blocks=_max_blocks,
-                    min_blocks=_min_blocks,
+                    max_blocks=5,
+                    min_blocks=2,
                     launcher=SingleNodeLauncher(),
                 ),
             )
         ],
-        max_idletime=0.5,
+        max_idletime=5,
         strategy='htex_auto_scale',
     )
 
 
 @python_app
-def waiting_app(ident: int, inputs=()):
-    import pathlib
+def sleeper(t):
     import time
-
-    # Approximate an Event by writing to files; the test logic will poll this file
-    with open(inputs[0], "a") as f:
-        f.write(f"Ready: {ident}\n")
-
-    # Similarly, use Event approximation (file check!) by polling.
-    may_finish_file = pathlib.Path(inputs[1])
-    while not may_finish_file.exists():
-        time.sleep(0.01)
+    time.sleep(t)
 
 
 # see issue #1885 for details of failures of this test.
 # at the time of issue #1885 this test was failing frequently
 # in CI.
 @pytest.mark.local
-def test_scale_out(tmpd_cwd, try_assert):
+def test_scale_out():
+    logger.info("start")
     dfk = parsl.dfk()
 
-    num_managers = len(dfk.executors['htex_local'].connected_managers())
-
-    assert num_managers == 0, "Expected 0 managers at start"
+    logger.info("initial asserts")
+    assert len(dfk.executors['htex_local'].connected_managers()) == 0, "Expected 0 managers at start"
     assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 tasks at start"
 
-    ntasks = 10
-    ready_path = tmpd_cwd / "workers_ready"
-    finish_path = tmpd_cwd / "workers_may_continue"
-    ready_path.touch()
-    inputs = [File(str(ready_path)), File(str(finish_path))]
+    logger.info("launching tasks")
+    fus = [sleeper(i) for i in [15 for x in range(0, 10)]]
 
-    futs = [waiting_app(i, inputs=inputs) for i in range(ntasks)]
+    logger.info("waiting for warm up")
+    time.sleep(15)
 
-    while ready_path.read_text().count("\n") < _max_blocks:
-        time.sleep(0.5)
+    logger.info("asserting 5 managers")
+    assert len(dfk.executors['htex_local'].connected_managers()) == 5, "Expected 5 managers after some time"
 
-    assert len(dfk.executors['htex_local'].connected_managers()) == _max_blocks
+    logger.info("waiting for all futures to complete")
+    [x.result() for x in fus]
 
-    finish_path.touch()  # Approximation of Event, via files
-    [x.result() for x in futs]
+    logger.info("asserting 0 outstanding tasks after completion")
+    assert dfk.executors['htex_local'].outstanding == 0, "Expected 0 outstanding tasks after future completion"
 
-    assert dfk.executors['htex_local'].outstanding == 0
+    logger.info("waiting a while for scale down")
+    time.sleep(25)
 
-    def assert_kernel():
-        return len(dfk.executors['htex_local'].connected_managers()) == _min_blocks
+    logger.info("asserting 2 managers remain")
+    assert len(dfk.executors['htex_local'].connected_managers()) == 2, "Expected 2 managers when no tasks, lower bound by min_blocks"
 
-    try_assert(
-        assert_kernel,
-        fail_msg=f"Expected {_min_blocks} managers when no tasks (min_blocks)",
-        timeout_ms=15000,
-    )
+    logger.info("test passed")
```

### Comparing `parsl-2023.7.17/parsl/tests/test_serialization/test_basic.py` & `parsl-2023.7.3/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.7.3/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_1316.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.7.3/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_summary.py` & `parsl-2023.7.3/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_thread_parallelism.py` & `parsl-2023.7.3/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_threads/test_configs.py` & `parsl-2023.7.3/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.7.3/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/usage_tracking/usage.py` & `parsl-2023.7.3/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/parsl/utils.py` & `parsl-2023.7.3/parsl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import inspect
 import logging
 import os
 import shlex
 import subprocess
 import threading
 import time
-from contextlib import contextmanager
 from types import TracebackType
-from typing import Any, Callable, List, Tuple, Union, Generator, IO, AnyStr, Dict, Optional
 
 import typeguard
+from contextlib import contextmanager
+from typing import Any, Callable, List, Tuple, Union, Generator, IO, AnyStr, Dict, Optional
+
 from typing_extensions import Type
 
 import parsl
 from parsl.version import VERSION
 
 
 try:
@@ -105,29 +106,26 @@
     if not os.path.isdir(last_checkpoint):
         return []
 
     return [last_checkpoint]
 
 
 @typeguard.typechecked
-def get_std_fname_mode(
-    fdname: str,
-    stdfspec: Union[os.PathLike, str, Tuple[str, str], Tuple[os.PathLike, str]]
-) -> Tuple[str, str]:
+def get_std_fname_mode(fdname: str, stdfspec: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
     import parsl.app.errors as pe
-    if isinstance(stdfspec, (str, os.PathLike)):
+    if isinstance(stdfspec, str):
         fname = stdfspec
         mode = 'a+'
     elif isinstance(stdfspec, tuple):
         if len(stdfspec) != 2:
             msg = (f"std descriptor {fdname} has incorrect tuple length "
                    f"{len(stdfspec)}")
             raise pe.BadStdStreamFile(msg, TypeError('Bad Tuple Length'))
         fname, mode = stdfspec
-    return str(fname), mode
+    return fname, mode
 
 
 @contextmanager
 def wait_for_file(path: str, seconds: int = 10) -> Generator[None, None, None]:
     for i in range(0, int(seconds * 100)):
         time.sleep(seconds / 100.)
         if os.path.exists(path):
```

### Comparing `parsl-2023.7.17/parsl.egg-info/SOURCES.txt` & `parsl-2023.7.3/parsl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,14 @@
 parsl/tests/test_regression/test_854.py
 parsl/tests/test_regression/test_97_parallelism_0.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
 parsl/tests/test_scaling/test_regression_1621.py
 parsl/tests/test_scaling/test_scale_down.py
 parsl/tests/test_serialization/__init__.py
-parsl/tests/test_serialization/test_2555_caching_deserializer.py
 parsl/tests/test_serialization/test_basic.py
 parsl/tests/test_staging/__init__.py
 parsl/tests/test_staging/staging_provider.py
 parsl/tests/test_staging/test_1316.py
 parsl/tests/test_staging/test_docs_1.py
 parsl/tests/test_staging/test_docs_2.py
 parsl/tests/test_staging/test_elaborate_noop_file.py
```

### Comparing `parsl-2023.7.17/parsl.egg-info/requires.txt` & `parsl-2023.7.3/parsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parsl-2023.7.17/setup.py` & `parsl-2023.7.3/setup.py`

 * *Files identical despite different names*

