# Comparing `tmp/flytekit-1.8.0.tar.gz` & `tmp/flytekit-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.8.0.tar", last modified: Tue Jul 11 22:07:06 2023, max compression
+gzip compressed data, was "flytekit-1.8.1.tar", last modified: Tue Jul 18 18:01:28 2023, max compression
```

## Comparing `flytekit-1.8.0.tar` & `flytekit-1.8.1.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 22:06:52.000000 flytekit-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-11 22:06:52.000000 flytekit-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-11 22:07:06.787602 flytekit-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-11 22:06:52.000000 flytekit-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.755602 flytekit-1.8.0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-11 22:07:04.000000 flytekit-1.8.0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.763602 flytekit-1.8.0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31873 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.763602 flytekit-1.8.0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31360 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    78535 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38243 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/backend/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extend/backend/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.771602 flytekit-1.8.0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.775602 flytekit-1.8.0/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.779602 flytekit-1.8.0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.779602 flytekit-1.8.0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.783602 flytekit-1.8.0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.783602 flytekit-1.8.0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87410 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.783602 flytekit-1.8.0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/iterator/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/iterator/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.759602 flytekit-1.8.0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 22:07:06.000000 flytekit-1.8.0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:06.787602 flytekit-1.8.0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 22:06:52.000000 flytekit-1.8.0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-11 22:06:52.000000 flytekit-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-11 22:07:06.791602 flytekit-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-11 22:07:04.000000 flytekit-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-18 18:01:17.000000 flytekit-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 18:01:17.000000 flytekit-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-18 18:01:28.547015 flytekit-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-18 18:01:17.000000 flytekit-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-18 18:01:27.000000 flytekit-1.8.1/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.535015 flytekit-1.8.1/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31873 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.535015 flytekit-1.8.1/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31360 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18490 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78535 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38243 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.539015 flytekit-1.8.1/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87410 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.543015 flytekit-1.8.1/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit/types/iterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/iterator/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44578 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.531015 flytekit-1.8.1/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-18 18:01:28.000000 flytekit-1.8.1/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-18 18:01:28.000000 flytekit-1.8.1/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:28.000000 flytekit-1.8.1/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 18:01:28.000000 flytekit-1.8.1/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-18 18:01:28.000000 flytekit-1.8.1/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 18:01:28.000000 flytekit-1.8.1/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:28.547015 flytekit-1.8.1/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 18:01:17.000000 flytekit-1.8.1/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-18 18:01:17.000000 flytekit-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-18 18:01:28.547015 flytekit-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-18 18:01:27.000000 flytekit-1.8.1/setup.py
```

### Comparing `flytekit-1.8.0/LICENSE` & `flytekit-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/MANIFEST.in` & `flytekit-1.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/PKG-INFO` & `flytekit-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.8.0
+Version: 1.8.1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.8.0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.8.1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.8.0/README.md` & `flytekit-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/__init__.py` & `flytekit-1.8.1/flytekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.8.0/flytekit/bin/entrypoint.py` & `flytekit-1.8.1/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/auth/auth_client.py` & `flytekit-1.8.1/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/auth/authenticator.py` & `flytekit-1.8.1/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/auth/keyring.py` & `flytekit-1.8.1/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/auth/token_client.py` & `flytekit-1.8.1/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/auth_helper.py` & `flytekit-1.8.1/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/friendly.py` & `flytekit-1.8.1/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.8.1/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.8.1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/helpers.py` & `flytekit-1.8.1/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clients/raw.py` & `flytekit-1.8.1/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.8.1/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/helpers.py` & `flytekit-1.8.1/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.8.1/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/configuration/__init__.py` & `flytekit-1.8.1/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/configuration/default_images.py` & `flytekit-1.8.1/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/configuration/feature_flags.py` & `flytekit-1.8.1/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/configuration/file.py` & `flytekit-1.8.1/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/configuration/internal.py` & `flytekit-1.8.1/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/annotation.py` & `flytekit-1.8.1/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/base_sql_task.py` & `flytekit-1.8.1/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/base_task.py` & `flytekit-1.8.1/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/checkpointer.py` & `flytekit-1.8.1/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/class_based_resolver.py` & `flytekit-1.8.1/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/condition.py` & `flytekit-1.8.1/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/constants.py` & `flytekit-1.8.1/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/container_task.py` & `flytekit-1.8.1/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/context_manager.py` & `flytekit-1.8.1/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/data_persistence.py` & `flytekit-1.8.1/flytekit/core/data_persistence.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/docstring.py` & `flytekit-1.8.1/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.8.1/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/gate.py` & `flytekit-1.8.1/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/interface.py` & `flytekit-1.8.1/flytekit/core/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,18 +245,20 @@
         )
 
     inputs_map = transform_variable_map(interface.inputs, input_descriptions)
     outputs_map = transform_variable_map(interface.outputs, output_descriptions)
     return _interface_models.TypedInterface(inputs_map, outputs_map)
 
 
-def transform_types_to_list_of_type(m: Dict[str, type], bound_inputs: typing.Set[str]) -> Dict[str, type]:
+def transform_types_to_list_of_type(
+    m: Dict[str, type], bound_inputs: typing.Set[str], list_as_optional: bool = False
+) -> Dict[str, type]:
     """
-    Converts a given variables to be collections of their type. This is useful for array jobs / map style code.
-    It will create a collection of types even if any one these types is not a collection type
+    Converts unbound inputs into the equivalent (optional) collections. This is useful for array jobs / map style code.
+    It will create a collection of types even if any one these types is not a collection type.
     """
     if m is None:
         return {}
 
     all_types_are_collection = True
     for k, v in m.items():
         if k in bound_inputs:
@@ -272,27 +274,29 @@
         return m
 
     om = {}
     for k, v in m.items():
         if k in bound_inputs:
             om[k] = v
         else:
-            om[k] = typing.List[v]  # type: ignore
+            om[k] = typing.List[typing.Optional[v] if list_as_optional else v]  # type: ignore
     return om  # type: ignore
 
 
-def transform_interface_to_list_interface(interface: Interface, bound_inputs: typing.Set[str]) -> Interface:
+def transform_interface_to_list_interface(
+    interface: Interface, bound_inputs: typing.Set[str], optional_outputs: bool = False
+) -> Interface:
     """
     Takes a single task interface and interpolates it to an array interface - to allow performing distributed python map
     like functions
     :param interface: Interface to be upgraded toa list interface
     :param bound_inputs: fixed inputs that should not upgraded to a list and will be maintained as scalars.
     """
     map_inputs = transform_types_to_list_of_type(interface.inputs, bound_inputs)
-    map_outputs = transform_types_to_list_of_type(interface.outputs, set())
+    map_outputs = transform_types_to_list_of_type(interface.outputs, set(), optional_outputs)
 
     return Interface(inputs=map_inputs, outputs=map_outputs)
 
 
 def transform_function_to_interface(fn: typing.Callable, docstring: Optional[Docstring] = None) -> Interface:
     """
     From the annotations on a task function that the user should have provided, and the output names they want to use
```

### Comparing `flytekit-1.8.0/flytekit/core/launch_plan.py` & `flytekit-1.8.1/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/local_cache.py` & `flytekit-1.8.1/flytekit/core/local_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 # Location on the filesystem where serialized objects will be stored
 # TODO: read from config
 CACHE_LOCATION = "~/.flyte/local-cache"
 
 
 def _recursive_hash_placement(literal: Literal) -> Literal:
-    if literal.collection is not None:
-        literals = [_recursive_hash_placement(literal) for literal in literal.collection.literals]
+    # Base case, hash gets passed through always if set
+    if literal.hash is not None:
+        return Literal(hash=literal.hash)
+    elif literal.collection is not None:
+        literals = [_recursive_hash_placement(lit) for lit in literal.collection.literals]
         return Literal(collection=LiteralCollection(literals=literals))
     elif literal.map is not None:
         literal_map = {}
-        for key, literal in literal.map.literals.items():
-            literal_map[key] = _recursive_hash_placement(literal)
+        for key, literal_value in literal.map.literals.items():
+            literal_map[key] = _recursive_hash_placement(literal_value)
         return Literal(map=LiteralMap(literal_map))
-
-    # Base case
-    if literal.hash is not None:
-        return Literal(hash=literal.hash)
     else:
         return literal
 
 
 def _calculate_cache_key(task_name: str, cache_version: str, input_literal_map: LiteralMap) -> str:
     # Traverse the literals and replace the literal with a new literal that only contains the hash
     literal_map_overridden = {}
```

### Comparing `flytekit-1.8.0/flytekit/core/map_task.py` & `flytekit-1.8.1/flytekit/core/map_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from flytekit.core import tracker
 from flytekit.core.base_task import PythonTask, Task, TaskResolverMixin
 from flytekit.core.constants import SdkTaskType
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.interface import transform_interface_to_list_interface
 from flytekit.core.python_function_task import PythonFunctionTask, PythonInstanceTask
 from flytekit.core.tracker import TrackedInstance
-from flytekit.core.type_engine import UnionTransformer
 from flytekit.core.utils import timeit
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.models.array_job import ArrayJob
 from flytekit.models.interface import Variable
 from flytekit.models.task import Container, K8sPod, Sql
 from flytekit.tools.module_loader import load_object_from_module
 
@@ -67,29 +66,28 @@
 
         if not isinstance(actual_task, PythonFunctionTask):
             if isinstance(actual_task, PythonInstanceTask):
                 pass
             else:
                 raise ValueError("Map tasks can only compose of PythonFuncton and PythonInstanceTasks currently")
 
-        if len(actual_task.python_interface.outputs.keys()) > 1:
+        n_outputs = len(actual_task.python_interface.outputs.keys())
+        if n_outputs > 1:
             raise ValueError("Map tasks only accept python function tasks with 0 or 1 outputs")
 
-        if (
-            min_success_ratio
-            and min_success_ratio != 1
-            and not UnionTransformer.is_optional_type(actual_task.python_interface.outputs["o0"])
-        ):
-            raise ValueError("Map tasks with min_success_ratio < 1 must have an optional output")
-
         self._bound_inputs: typing.Set[str] = set(bound_inputs) if bound_inputs else set()
         if self._partial:
             self._bound_inputs = set(self._partial.keywords.keys())
 
-        collection_interface = transform_interface_to_list_interface(actual_task.python_interface, self._bound_inputs)
+        # Transform the interface to List[Optional[T]] in case `min_success_ratio` is set
+        output_as_list_of_optionals = min_success_ratio is not None and min_success_ratio != 1 and n_outputs == 1
+        collection_interface = transform_interface_to_list_interface(
+            actual_task.python_interface, self._bound_inputs, output_as_list_of_optionals
+        )
+
         self._run_task: typing.Union[PythonFunctionTask, PythonInstanceTask] = actual_task  # type: ignore
         if isinstance(actual_task, PythonInstanceTask):
             mod = actual_task.task_type
             f = actual_task.lhs
         else:
             _, mod, f, _ = tracker.extract_task_module(typing.cast(PythonFunctionTask, actual_task).task_function)
         h = hashlib.md5(collection_interface.__str__().encode("utf-8")).hexdigest()
```

### Comparing `flytekit-1.8.0/flytekit/core/mock_stats.py` & `flytekit-1.8.1/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/node.py` & `flytekit-1.8.1/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/node_creation.py` & `flytekit-1.8.1/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/notification.py` & `flytekit-1.8.1/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/pod_template.py` & `flytekit-1.8.1/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/promise.py` & `flytekit-1.8.1/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/python_auto_container.py` & `flytekit-1.8.1/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/python_customized_container_task.py` & `flytekit-1.8.1/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/python_function_task.py` & `flytekit-1.8.1/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/reference.py` & `flytekit-1.8.1/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/reference_entity.py` & `flytekit-1.8.1/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/resources.py` & `flytekit-1.8.1/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/schedule.py` & `flytekit-1.8.1/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/shim_task.py` & `flytekit-1.8.1/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/task.py` & `flytekit-1.8.1/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/testing.py` & `flytekit-1.8.1/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/tracker.py` & `flytekit-1.8.1/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/type_engine.py` & `flytekit-1.8.1/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/type_helpers.py` & `flytekit-1.8.1/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/utils.py` & `flytekit-1.8.1/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/core/workflow.py` & `flytekit-1.8.1/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/deck/deck.py` & `flytekit-1.8.1/flytekit/deck/deck.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         def t2() -> Annotated[pd.DataFrame, TopFrameRenderer(10)]:
             return iris_df
 
     """
 
     def __init__(self, name: str, html: Optional[str] = ""):
         self._name = name
-        # self.renderers = renderers if isinstance(renderers, list) else [renderers]
         self._html = html
         FlyteContextManager.current_context().user_space_params.decks.append(self)
 
     def append(self, html: str) -> "Deck":
         assert isinstance(html, str)
         self._html = self._html + "\n" + html
         return self
@@ -143,24 +142,28 @@
     return raw_html
 
 
 def _output_deck(task_name: str, new_user_params: ExecutionParameters):
     ctx = FlyteContext.current_context()
     local_dir = ctx.file_access.get_random_local_directory()
     local_path = f"{local_dir}{os.sep}{DECK_FILE_NAME}"
-    with open(local_path, "w") as f:
-        f.write(_get_deck(new_user_params, ignore_jupyter=True))
-    logger.info(f"{task_name} task creates flyte deck html to file://{local_path}")
-    if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
-        remote_path = f"{new_user_params.output_metadata_prefix}{os.sep}{DECK_FILE_NAME}"
-        kwargs: typing.Dict[str, str] = {
-            "ContentType": "text/html",  # For s3
-            "content_type": "text/html",  # For gcs
-        }
-        ctx.file_access.put_data(local_path, remote_path, **kwargs)
+    try:
+        with open(local_path, "w", encoding="utf-8") as f:
+            f.write(_get_deck(new_user_params, ignore_jupyter=True))
+        logger.info(f"{task_name} task creates flyte deck html to file://{local_path}")
+        if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
+            fs = ctx.file_access.get_filesystem_for_path(new_user_params.output_metadata_prefix)
+            remote_path = f"{new_user_params.output_metadata_prefix}{ctx.file_access.sep(fs)}{DECK_FILE_NAME}"
+            kwargs: typing.Dict[str, str] = {
+                "ContentType": "text/html",  # For s3
+                "content_type": "text/html",  # For gcs
+            }
+            ctx.file_access.put_data(local_path, remote_path, **kwargs)
+    except Exception as e:
+        logger.error(f"Failed to write flyte deck html with error {e}.")
 
 
 def get_deck_template() -> "Template":
     from jinja2 import Environment, FileSystemLoader, select_autoescape
 
     root = os.path.dirname(os.path.abspath(__file__))
     templates_dir = os.path.join(root, "html")
```

### Comparing `flytekit-1.8.0/flytekit/deck/html/template.html` & `flytekit-1.8.1/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/deck/renderer.py` & `flytekit-1.8.1/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/exceptions/scopes.py` & `flytekit-1.8.1/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/exceptions/system.py` & `flytekit-1.8.1/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/exceptions/user.py` & `flytekit-1.8.1/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extend/__init__.py` & `flytekit-1.8.1/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extend/backend/agent_service.py` & `flytekit-1.8.1/flytekit/extend/backend/agent_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extend/backend/base_agent.py` & `flytekit-1.8.1/flytekit/extend/backend/base_agent.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.8.1/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.8.1/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.8.1/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/pytorch/native.py` & `flytekit-1.8.1/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.8.1/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/sklearn/native.py` & `flytekit-1.8.1/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/sqlite3/task.py` & `flytekit-1.8.1/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/tasks/shell.py` & `flytekit-1.8.1/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.8.1/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/tensorflow/model.py` & `flytekit-1.8.1/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/extras/tensorflow/record.py` & `flytekit-1.8.1/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/image_spec/image_spec.py` & `flytekit-1.8.1/flytekit/image_spec/image_spec.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/interaction/parse_stdin.py` & `flytekit-1.8.1/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.8.1/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/interfaces/random.py` & `flytekit-1.8.1/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/interfaces/stats/client.py` & `flytekit-1.8.1/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.8.1/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/lazy_import/lazy_module.py` & `flytekit-1.8.1/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/loggers.py` & `flytekit-1.8.1/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/admin/common.py` & `flytekit-1.8.1/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/admin/task_execution.py` & `flytekit-1.8.1/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/admin/workflow.py` & `flytekit-1.8.1/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/annotation.py` & `flytekit-1.8.1/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/array_job.py` & `flytekit-1.8.1/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/common.py` & `flytekit-1.8.1/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/catalog.py` & `flytekit-1.8.1/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/compiler.py` & `flytekit-1.8.1/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/condition.py` & `flytekit-1.8.1/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/errors.py` & `flytekit-1.8.1/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/execution.py` & `flytekit-1.8.1/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/identifier.py` & `flytekit-1.8.1/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/types.py` & `flytekit-1.8.1/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/core/workflow.py` & `flytekit-1.8.1/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/documentation.py` & `flytekit-1.8.1/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/dynamic_job.py` & `flytekit-1.8.1/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/execution.py` & `flytekit-1.8.1/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/filters.py` & `flytekit-1.8.1/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/interface.py` & `flytekit-1.8.1/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/launch_plan.py` & `flytekit-1.8.1/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/literals.py` & `flytekit-1.8.1/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/matchable_resource.py` & `flytekit-1.8.1/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/named_entity.py` & `flytekit-1.8.1/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/node_execution.py` & `flytekit-1.8.1/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/presto.py` & `flytekit-1.8.1/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/project.py` & `flytekit-1.8.1/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/qubole.py` & `flytekit-1.8.1/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/schedule.py` & `flytekit-1.8.1/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/security.py` & `flytekit-1.8.1/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/task.py` & `flytekit-1.8.1/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/types.py` & `flytekit-1.8.1/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/models/workflow_closure.py` & `flytekit-1.8.1/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/__init__.py` & `flytekit-1.8.1/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/backfill.py` & `flytekit-1.8.1/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/entities.py` & `flytekit-1.8.1/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/executions.py` & `flytekit-1.8.1/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/lazy_entity.py` & `flytekit-1.8.1/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/remote.py` & `flytekit-1.8.1/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/remote/remote_callable.py` & `flytekit-1.8.1/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/testing/__init__.py` & `flytekit-1.8.1/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/fast_registration.py` & `flytekit-1.8.1/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/ignore.py` & `flytekit-1.8.1/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/module_loader.py` & `flytekit-1.8.1/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/repo.py` & `flytekit-1.8.1/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/script_mode.py` & `flytekit-1.8.1/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/serialize_helpers.py` & `flytekit-1.8.1/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/subprocess.py` & `flytekit-1.8.1/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/tools/translator.py` & `flytekit-1.8.1/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/directory/__init__.py` & `flytekit-1.8.1/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/directory/types.py` & `flytekit-1.8.1/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/file/__init__.py` & `flytekit-1.8.1/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/file/file.py` & `flytekit-1.8.1/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/iterator/iterator.py` & `flytekit-1.8.1/flytekit/types/iterator/iterator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/numpy/ndarray.py` & `flytekit-1.8.1/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/pickle/pickle.py` & `flytekit-1.8.1/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/schema/types.py` & `flytekit-1.8.1/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/schema/types_pandas.py` & `flytekit-1.8.1/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/structured/__init__.py` & `flytekit-1.8.1/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.8.1/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/structured/bigquery.py` & `flytekit-1.8.1/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.8.1/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit.egg-info/PKG-INFO` & `flytekit-1.8.1/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.8.0
+Version: 1.8.1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.8.0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.8.1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.8.0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.8.1/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.8.1/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.8.0/setup.py` & `flytekit-1.8.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -48,24 +48,27 @@
         "s3fs>=0.6.0",
         "gcsfs",
         "pyopenssl",
         "joblib",
         "python-json-logger>=2.0.0",
         "pytimeparse>=1.1.8,<2.0.0",
         "pytz",
-        "pyyaml",
+        "pyyaml>=6.0.0; python_version>='3.10'",
+        "pyyaml<6.0.0; python_version<'3.10'",
         "keyring>=18.0.1",
         "requests>=2.18.4,<3.0.0",
         "responses>=0.10.7",
         "sortedcontainers>=1.5.9,<3.0.0",
         "statsd>=3.0.0,<4.0.0",
         "urllib3>=1.22,<2.0.0",
         "wrapt>=1.0.0,<2.0.0",
-        "dataclasses-json>=0.5.2",
+        # TODO: remove upper-bound after fixing change in contract
+        "dataclasses-json>=0.5.2,<0.5.12",
         "marshmallow-jsonschema>=0.12.0",
+        "marshmallow-enum",
         "natsort>=7.0.1",
         "docker-image-py>=0.1.10",
         "typing_extensions",
         "docstring-parser>=0.9.0",
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
```

