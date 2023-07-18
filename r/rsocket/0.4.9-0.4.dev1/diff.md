# Comparing `tmp/rsocket-0.4.9.tar.gz` & `tmp/rsocket-0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsocket-0.4.9.tar", last modified: Sun Mar  5 16:59:50 2023, max compression
+gzip compressed data, was "rsocket-0.4.dev1.tar", last modified: Fri Oct 14 06:48:18 2022, max compression
```

## Comparing `rsocket-0.4.9.tar` & `rsocket-0.4.dev1.tar`

### file list

```diff
@@ -1,180 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.040989 rsocket-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-05 16:59:40.000000 rsocket-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-03-05 16:59:50.040989 rsocket-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-03-05 16:59:40.000000 rsocket-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.020988 rsocket-0.4.9/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.020988 rsocket-0.4.9/examples/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/reactivex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/reactivex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/reactivex/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/reactivex/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/reactivex/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step1/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step1/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step2/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step2/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step3/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step3/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step3/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step4/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step4/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step4/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step5/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step5/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step5/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step6/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step6/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step6/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.024988 rsocket-0.4.9/examples/tutorial/step7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step7/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step7/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step7/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.028988 rsocket-0.4.9/examples/tutorial/step8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step8/chat_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step8/chat_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/step8/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-05 16:59:40.000000 rsocket-0.4.9/examples/tutorial/test_tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.028988 rsocket-0.4.9/performance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-05 16:59:40.000000 rsocket-0.4.9/performance/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-03-05 16:59:40.000000 rsocket-0.4.9/performance/performance_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-05 16:59:40.000000 rsocket-0.4.9/performance/performance_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-05 16:59:40.000000 rsocket-0.4.9/performance/sample_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-05 16:59:40.000000 rsocket-0.4.9/performance/test_performance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.028988 rsocket-0.4.9/reactivestreams/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-05 16:59:40.000000 rsocket-0.4.9/reactivestreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-05 16:59:40.000000 rsocket-0.4.9/reactivestreams/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-05 16:59:40.000000 rsocket-0.4.9/reactivestreams/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-05 16:59:40.000000 rsocket-0.4.9/reactivestreams/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.032988 rsocket-0.4.9/rsocket/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/async_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.032988 rsocket-0.4.9/rsocket/awaitable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/awaitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/awaitable/awaitable_rsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/awaitable/collector_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.032988 rsocket-0.4.9/rsocket/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/datetime_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/disposable.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.032988 rsocket-0.4.9/rsocket/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/authentication_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/authentication_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/composite_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/composite_metadata_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/mimetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/stream_data_mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/extensions/tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame_fragment_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame_fragmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/frame_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.032988 rsocket-0.4.9/rsocket/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_cahnnel_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_cahnnel_responder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_channel_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_response_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_response_responder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_stream_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/handlers/request_stream_responder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/lease.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.036989 rsocket-0.4.9/rsocket/load_balancer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/load_balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/load_balancer/load_balancer_rsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/load_balancer/load_balancer_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/load_balancer/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/load_balancer/round_robin.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/local_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/queue_peekable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.036989 rsocket-0.4.9/rsocket/reactivex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/back_pressure_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/from_rsocket_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/reactivex_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/reactivex_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/reactivex_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/reactivex_handler_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/reactivex/subscriber_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.036989 rsocket-0.4.9/rsocket/routing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/routing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/routing/request_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/routing/routing_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rsocket_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rsocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rsocket_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rsocket_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.036989 rsocket-0.4.9/rsocket/rx_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/back_pressure_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/from_rsocket_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/rx_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/rx_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/rx_handler_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/rx_rsocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/rx_support/subscriber_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/stream_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.040989 rsocket-0.4.9/rsocket/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/backpressureapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/empty_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/error_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/null_subscrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/stream_from_async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/stream_from_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/streams/stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.040989 rsocket-0.4.9/rsocket/transports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/abstract_messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/aiohttp_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/aioquic_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/http3_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/quart_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-05 16:59:40.000000 rsocket-0.4.9/rsocket/transports/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:59:50.032988 rsocket-0.4.9/rsocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-03-05 16:59:50.000000 rsocket-0.4.9/rsocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-05 16:59:50.000000 rsocket-0.4.9/rsocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:59:50.000000 rsocket-0.4.9/rsocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-05 16:59:50.000000 rsocket-0.4.9/rsocket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-05 16:59:50.000000 rsocket-0.4.9/rsocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-05 16:59:50.000000 rsocket-0.4.9/rsocket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:59:49.000000 rsocket-0.4.9/rsocket.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-05 16:59:50.040989 rsocket-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-05 16:59:40.000000 rsocket-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.498523 rsocket-0.4.dev1/reactivestreams/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/reactivestreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/reactivestreams/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/reactivestreams/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/reactivestreams/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.502523 rsocket-0.4.dev1/rsocket/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.502523 rsocket-0.4.dev1/rsocket/awaitable/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/awaitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/awaitable/awaitable_rsocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/awaitable/collector_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/datetime_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.502523 rsocket-0.4.dev1/rsocket/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/authentication_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/authentication_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/composite_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/composite_metadata_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/mimetypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/routing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/stream_data_mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/extensions/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23321 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4131 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame_builders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame_fragment_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame_fragmenter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/frame_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_cahnnel_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_cahnnel_responder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_channel_requester.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_response_requester.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_response_responder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_stream_requester.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/handlers/request_stream_responder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/lease.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/load_balancer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/load_balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/load_balancer/load_balancer_rsocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/load_balancer/load_balancer_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/load_balancer/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/load_balancer/round_robin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/local_typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/queue_peekable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/reactivex/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/reactivex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/reactivex/back_pressure_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/reactivex/from_rsocket_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/reactivex/reactivex_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/reactivex/subscriber_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/routing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/routing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/routing/request_router.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4353 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/routing/routing_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rsocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21853 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rsocket_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6911 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rsocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rsocket_internal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rsocket_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/rx_support/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rx_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rx_support/back_pressure_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rx_support/from_rsocket_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rx_support/rx_rsocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/rx_support/subscriber_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/stream_control.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/streams/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/backpressureapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/error_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/null_subscrier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/stream_from_async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/stream_from_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/streams/stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.506523 rsocket-0.4.dev1/rsocket/transports/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/abstract_messaging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/aiohttp_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/aioquic_transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/quart_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/rsocket/transports/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 06:48:18.502523 rsocket-0.4.dev1/rsocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-10-14 06:48:18.000000 rsocket-0.4.dev1/rsocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3049 2022-10-14 06:48:18.000000 rsocket-0.4.dev1/rsocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 06:48:18.000000 rsocket-0.4.dev1/rsocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-14 06:48:18.000000 rsocket-0.4.dev1/rsocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-14 06:48:18.000000 rsocket-0.4.dev1/rsocket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 06:48:18.000000 rsocket-0.4.dev1/rsocket.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-14 06:48:18.510523 rsocket-0.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-10-14 06:48:07.000000 rsocket-0.4.dev1/setup.py
```

### Comparing `rsocket-0.4.9/LICENSE` & `rsocket-0.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/PKG-INFO` & `rsocket-0.4.dev1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: rsocket
-Version: 0.4.9
+Version: 0.4.dev1
 Summary: Python RSocket library
 Home-page: https://github.com/rsocket/rsocket-py
 Author: Gabriel Shaar
 Author-email: workofishi@pm.me
 License: MIT
-Project-URL: Documentation, https://rsocket.io/guides/rsocket-py
-Project-URL: Changelog, https://github.com/rsocket/rsocket-py/blob/master/CHANGELOG.rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
@@ -25,88 +22,80 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rx
 Provides-Extra: reactivex
 Provides-Extra: aiohttp
 Provides-Extra: quart
 Provides-Extra: quic
-Provides-Extra: cli
-Provides-Extra: optimized
 License-File: LICENSE
 
 # RSocket-py
 
 Python implementation of [RSocket](http://rsocket.io)
 
-| NOTE: The python api is not final and may be broken between minor versions<br/>See CHANGELOG for <b>Breaking Changes</b> |
-|--------------------------------------------------------------------------------------------------------------------------------|
-
 # Installation
 
 The latest version from [pypi](https://pypi.org/project/rsocket/) can be installed using:
 
 ```shell
 pip install rsocket
 ```
 
-You may also install using some **extras**:
+or install any of the extras:
+
+* rx (RxPy3)
+* reactivex (RxPy4)
+* aiohttp
+* quart
+* uic
 
-| Extra     | Functionality                       |
-|-----------|-------------------------------------|
-| rx        | ReactiveX (v3) integration          |
-| reactivex | ReactiveX (v4) integration          |
-| aiohttp   | Websocket transport (server/client) |
-| quart     | Websocket transport (server only)   |
-| quic      | QUIC transport                      |
-| cli       | Command line                        |
-| optimized | Frame parse/serialize optimizations |
+Example:
 
 ```shell
-pip install rsocket[reactivex]
+pip install --pre rsocket[reactivex]
 ```
 
 Alternatively, download the source code, build a package:
 
 ```shell
 python3 setup.py bdist_wheel
 ```
 
-Use the resulting package from the **./dist** folder, or install locally:
+and use the resulting package from the **./dist** folder, or install locally:
 
 ```shell
 python3 setup.py install
 ```
 
 # Documentation
 
 [Documentation](https://rsocket.io/guides/rsocket-py) is available on the official rsocket.io site.
 
 # Examples
 
-Examples can be found in the **/examples** folder. It contains various server and client usages. The following is a table
-denoting which client example is constructed to be run against which server example. Some examples
-are in java to show compatibility with a different implementation. To run the java examples first build using <code>mvn
-package</code>.
-
-The **examples/test_examples.py** can be used to execute the relevant example server/client pairs.
-
-client_springboot.py is set up to work against the [Spring RSocket demo](https://github.com/benwilcock/spring-rsocket-demo).
-
-| server (python)                    | server (java)           | client (python)                    | client(java)    |
-|------------------------------------|-------------------------|------------------------------------|-----------------|
-| server.py                          |                         | client.py                          |                 |
-| server_quic.py                     |                         | client_quic.py                     |                 |
-| server_with_lease.py               |                         |                                    | ClientWithLease |
-| server_with_routing.py             |                         | client_with_routing.py             | Client          |
-| server_with_routing.py             |                         | client_rx.py                       |                 |
-| server_with_routing.py             |                         | client_reconnect.py                |                 |
-|                                    | Server                  | run_against_example_java_server.py |                 |
-|                                    | ServerWithFragmentation | client_with_routing.py             |                 |
-| server_quart_websocket.py          |                         | client_websocket.py                |                 |
-| server_aiohttp_websocket.py        |                         | client_websocket.py                |                 |
+Examples can be found in the /examples folder. It contains various server and client usages. The following is a table
+denoting which <b>client</b> example is constructed to be run against which <b>server</b> example. Some of the examples
+are in java to show compatibility with a different implementation.
+
+The **examples/test_examples.py** shows which pairs of client/server work with each other, and can be used to execute
+all the examples
+(except for the client_springboot.py which is set up to work against https://github.com/benwilcock/spring-rsocket-demo)
+
+| server (python)             | server (java)           | client (python)                    | client(java)    |
+|-----------------------------|-------------------------|------------------------------------|-----------------|
+| server.py                   |                         | client.py                          |                 |
+| server_quic.py              |                         | client_quic.py                     |                 |
+| server_with_lease.py        |                         |                                    | ClientWithLease |
+| server_with_routing.py      |                         | client_with_routing.py             | Client          |
+| server_with_routing.py      |                         | client_rx.py                       |                 |
+| server_with_routing.py      |                         | client_reconnect.py                |                 |
+|                             | Server                  | run_against_example_java_server.py |                 |
+|                             | ServerWithFragmentation | client_with_routing.py             |                 |
+| server_quart_websocket.py   |                         | client_websocket.py                |                 |
+| server_aiohttp_websocket.py |                         | client_websocket.py                |                 |
 
 # Build Status
 
 ![build master](https://github.com/rsocket/rsocket-py/actions/workflows/python-package.yml/badge.svg?branch=master)
 [![Coverage Status](https://coveralls.io/repos/github/rsocket/rsocket-py/badge.svg?branch=master)](https://coveralls.io/github/rsocket/rsocket-py?branch=master)
 [![CodeQL](https://github.com/rsocket/rsocket-py/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/rsocket/rsocket-py/actions/workflows/codeql-analysis.yml)
 
@@ -126,23 +115,20 @@
 - [X] Extensions
     - [X] Composite metadata
     - [X] Per Stream Mimetype
     - [X] Routing
     - [X] Authentication
 - [ ] Transports
     - [X] TCP
-    - [X] Websocket (WS, WSS) - Quart and aiohttp integration
+    - [X] Websocket
     - [X] QUIC
-    - [X] HTTP/3
     - [ ] HTTP/2
     - [ ] Aeron
 - [X] RxPy Integration
     - [X] Stream Response
     - [X] Channel Response
     - [X] Channel Requester stream
     - [X] Response
-- [X] Other
+- [ ] Other
+    - [ ] Error handling all scenarios in the protocol spec
     - [X] Reconnect
     - [X] Load balancing
-    - [X] Server routing definition helper (Flask like syntax)
-    - [X] Reactivex integration (v3, v4) server/client side
-    - [X] Command line interface
```

### Comparing `rsocket-0.4.9/README.md` & `rsocket-0.4.dev1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,71 @@
 # RSocket-py
 
 Python implementation of [RSocket](http://rsocket.io)
 
-| NOTE: The python api is not final and may be broken between minor versions<br/>See CHANGELOG for <b>Breaking Changes</b> |
-|--------------------------------------------------------------------------------------------------------------------------------|
-
 # Installation
 
 The latest version from [pypi](https://pypi.org/project/rsocket/) can be installed using:
 
 ```shell
 pip install rsocket
 ```
 
-You may also install using some **extras**:
+or install any of the extras:
+
+* rx (RxPy3)
+* reactivex (RxPy4)
+* aiohttp
+* quart
+* uic
 
-| Extra     | Functionality                       |
-|-----------|-------------------------------------|
-| rx        | ReactiveX (v3) integration          |
-| reactivex | ReactiveX (v4) integration          |
-| aiohttp   | Websocket transport (server/client) |
-| quart     | Websocket transport (server only)   |
-| quic      | QUIC transport                      |
-| cli       | Command line                        |
-| optimized | Frame parse/serialize optimizations |
+Example:
 
 ```shell
-pip install rsocket[reactivex]
+pip install --pre rsocket[reactivex]
 ```
 
 Alternatively, download the source code, build a package:
 
 ```shell
 python3 setup.py bdist_wheel
 ```
 
-Use the resulting package from the **./dist** folder, or install locally:
+and use the resulting package from the **./dist** folder, or install locally:
 
 ```shell
 python3 setup.py install
 ```
 
 # Documentation
 
 [Documentation](https://rsocket.io/guides/rsocket-py) is available on the official rsocket.io site.
 
 # Examples
 
-Examples can be found in the **/examples** folder. It contains various server and client usages. The following is a table
-denoting which client example is constructed to be run against which server example. Some examples
-are in java to show compatibility with a different implementation. To run the java examples first build using <code>mvn
-package</code>.
-
-The **examples/test_examples.py** can be used to execute the relevant example server/client pairs.
-
-client_springboot.py is set up to work against the [Spring RSocket demo](https://github.com/benwilcock/spring-rsocket-demo).
-
-| server (python)                    | server (java)           | client (python)                    | client(java)    |
-|------------------------------------|-------------------------|------------------------------------|-----------------|
-| server.py                          |                         | client.py                          |                 |
-| server_quic.py                     |                         | client_quic.py                     |                 |
-| server_with_lease.py               |                         |                                    | ClientWithLease |
-| server_with_routing.py             |                         | client_with_routing.py             | Client          |
-| server_with_routing.py             |                         | client_rx.py                       |                 |
-| server_with_routing.py             |                         | client_reconnect.py                |                 |
-|                                    | Server                  | run_against_example_java_server.py |                 |
-|                                    | ServerWithFragmentation | client_with_routing.py             |                 |
-| server_quart_websocket.py          |                         | client_websocket.py                |                 |
-| server_aiohttp_websocket.py        |                         | client_websocket.py                |                 |
+Examples can be found in the /examples folder. It contains various server and client usages. The following is a table
+denoting which <b>client</b> example is constructed to be run against which <b>server</b> example. Some of the examples
+are in java to show compatibility with a different implementation.
+
+The **examples/test_examples.py** shows which pairs of client/server work with each other, and can be used to execute
+all the examples
+(except for the client_springboot.py which is set up to work against https://github.com/benwilcock/spring-rsocket-demo)
+
+| server (python)             | server (java)           | client (python)                    | client(java)    |
+|-----------------------------|-------------------------|------------------------------------|-----------------|
+| server.py                   |                         | client.py                          |                 |
+| server_quic.py              |                         | client_quic.py                     |                 |
+| server_with_lease.py        |                         |                                    | ClientWithLease |
+| server_with_routing.py      |                         | client_with_routing.py             | Client          |
+| server_with_routing.py      |                         | client_rx.py                       |                 |
+| server_with_routing.py      |                         | client_reconnect.py                |                 |
+|                             | Server                  | run_against_example_java_server.py |                 |
+|                             | ServerWithFragmentation | client_with_routing.py             |                 |
+| server_quart_websocket.py   |                         | client_websocket.py                |                 |
+| server_aiohttp_websocket.py |                         | client_websocket.py                |                 |
 
 # Build Status
 
 ![build master](https://github.com/rsocket/rsocket-py/actions/workflows/python-package.yml/badge.svg?branch=master)
 [![Coverage Status](https://coveralls.io/repos/github/rsocket/rsocket-py/badge.svg?branch=master)](https://coveralls.io/github/rsocket/rsocket-py?branch=master)
 [![CodeQL](https://github.com/rsocket/rsocket-py/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/rsocket/rsocket-py/actions/workflows/codeql-analysis.yml)
 
@@ -91,23 +85,20 @@
 - [X] Extensions
     - [X] Composite metadata
     - [X] Per Stream Mimetype
     - [X] Routing
     - [X] Authentication
 - [ ] Transports
     - [X] TCP
-    - [X] Websocket (WS, WSS) - Quart and aiohttp integration
+    - [X] Websocket
     - [X] QUIC
-    - [X] HTTP/3
     - [ ] HTTP/2
     - [ ] Aeron
 - [X] RxPy Integration
     - [X] Stream Response
     - [X] Channel Response
     - [X] Channel Requester stream
     - [X] Response
-- [X] Other
+- [ ] Other
+    - [ ] Error handling all scenarios in the protocol spec
     - [X] Reconnect
     - [X] Load balancing
-    - [X] Server routing definition helper (Flask like syntax)
-    - [X] Reactivex integration (v3, v4) server/client side
-    - [X] Command line interface
```

### Comparing `rsocket-0.4.9/performance/performance_server.py` & `rsocket-0.4.dev1/rsocket/routing/routing_request_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,100 @@
-import asyncio
-import json
-import logging
-import sys
-from dataclasses import dataclass
-from datetime import timedelta
-from typing import Optional
+from asyncio import Future
+from typing import Callable, Union, Optional, Coroutine, Tuple
 
-from rsocket.extensions.authentication import Authentication, AuthenticationSimple
+from reactivestreams.publisher import Publisher
+from reactivestreams.subscriber import Subscriber
+from rsocket.extensions.authentication import Authentication
+from rsocket.extensions.authentication_content import AuthenticationContent
 from rsocket.extensions.composite_metadata import CompositeMetadata
-from rsocket.helpers import create_future
+from rsocket.extensions.helpers import require_route
+from rsocket.extensions.mimetypes import WellKnownMimeTypes
+from rsocket.frame import FrameType
+from rsocket.helpers import create_error_future
+from rsocket.local_typing import Awaitable
+from rsocket.logger import logger
 from rsocket.payload import Payload
+from rsocket.request_handler import BaseRequestHandler
 from rsocket.routing.request_router import RequestRouter
-from rsocket.routing.routing_request_handler import RoutingRequestHandler
-from rsocket.rsocket_server import RSocketServer
-from rsocket.transports.tcp import TransportTCP
-from performance.sample_responses import response_stream_2, response_stream_1, LoggingSubscriber
-from tests.rsocket.helpers import create_large_random_data
+from rsocket.streams.error_stream import ErrorStream
+from rsocket.streams.null_subscrier import NullSubscriber
 
-data_size = 1920 * 1080 * 3
-large_data = create_large_random_data(data_size)
 
-router = RequestRouter()
+class RoutingRequestHandler(BaseRequestHandler):
+    __slots__ = (
+        'router',
+        'data_encoding',
+        'metadata_encoding',
+        'authentication_verifier',
+    )
+
+    def __init__(self,
+                 socket,
+                 router: RequestRouter,
+                 authentication_verifier: Optional[
+                     Callable[[str, Authentication], Coroutine[None, None, None]]] = None):
+        super().__init__(socket)
+        self.router = router
+        self.authentication_verifier = authentication_verifier
+        self.data_encoding = None
+        self.metadata_encoding = None
+
+    async def on_setup(self,
+                       data_encoding: bytes,
+                       metadata_encoding: bytes,
+                       payload: Payload):
+
+        if metadata_encoding != WellKnownMimeTypes.MESSAGE_RSOCKET_COMPOSITE_METADATA.value.name:
+            raise Exception('Setup frame did not specify composite metadata. required for routing handler')
+        else:
+            self.data_encoding = data_encoding
+            self.metadata_encoding = metadata_encoding
+            await super().on_setup(data_encoding, metadata_encoding, payload)
+
+    async def request_channel(self, payload: Payload) -> Tuple[Optional[Publisher], Optional[Subscriber]]:
+        try:
+            return await self._parse_and_route(FrameType.REQUEST_CHANNEL, payload)
+        except Exception as exception:
+            return ErrorStream(exception), NullSubscriber()
+
+    async def request_fire_and_forget(self, payload: Payload):
+        try:
+            await self._parse_and_route(FrameType.REQUEST_FNF, payload)
+        except Exception:
+            logger().error('Fire and forget error: %s', payload, exc_info=True)
+
+    async def request_response(self, payload: Payload) -> Awaitable[Payload]:
+        try:
+            return await self._parse_and_route(FrameType.REQUEST_RESPONSE, payload)
+        except Exception as exception:
+            return create_error_future(exception)
+
+    async def request_stream(self, payload: Payload) -> Publisher:
+        try:
+            return await self._parse_and_route(FrameType.REQUEST_STREAM, payload)
+        except Exception as exception:
+            return ErrorStream(exception)
+
+    async def on_metadata_push(self, payload: Payload):
+        try:
+            await self._parse_and_route(FrameType.METADATA_PUSH, payload)
+        except Exception:
+            logger().error('Metadata push error: %s', payload, exc_info=True)
+
+    async def _parse_and_route(
+            self,
+            frame_type: FrameType,
+            payload: Payload
+    ) -> Union[Future, Publisher, None, Tuple[Optional[Publisher], Optional[Subscriber]]]:
+        composite_metadata = self._parse_composite_metadata(payload.metadata)
+        route = require_route(composite_metadata)
+        await self._verify_authentication(route, composite_metadata)
+        return await self.router.route(frame_type, route, payload, composite_metadata)
+
+    async def _verify_authentication(self, route: str, composite_metadata: CompositeMetadata):
+        if self.authentication_verifier is not None:
+            for item in composite_metadata.items:
+                if isinstance(item, AuthenticationContent):
+                    await self.authentication_verifier(route, item.authentication)
+                    return
 
-
-@dataclass
-class Storage:
-    last_metadata_push: Optional[bytes] = None
-    last_fire_and_forget: Optional[bytes] = None
-
-
-storage = Storage()
-
-
-@router.response('single_request')
-async def single_request_response(payload, composite_metadata):
-    logging.info('Got single request')
-    return create_future(Payload(b'single_response'))
-
-
-@router.response('large')
-async def single_request_response(payload, composite_metadata):
-    logging.info('Got single request')
-    return create_future(Payload(large_data))
-
-
-@router.response('last_fnf')
-async def get_last_fnf():
-    logging.info('Got single request')
-    return create_future(Payload(storage.last_fire_and_forget))
-
-
-@router.response('last_metadata_push')
-async def get_last_metadata_push():
-    logging.info('Got single request')
-    return create_future(Payload(storage.last_metadata_push))
-
-
-@router.stream('stream')
-async def stream_response(payload: Payload, composite_metadata):
-    data = json.loads(payload.data)
-
-    logging.info('Got stream request')
-
-    return response_stream_1(**data)
-
-
-@router.stream('fragmented_stream')
-async def fragmented_stream(payload, composite_metadata):
-    logging.info('Got fragmented stream request')
-    return response_stream_2(fragment_size=6)
-
-
-@router.fire_and_forget('no_response')
-async def no_response(payload: Payload, composite_metadata):
-    storage.last_fire_and_forget = payload.data
-    logging.info('No response sent to client')
-
-
-@router.metadata_push('metadata_push')
-async def metadata_push(payload: Payload, composite_metadata: CompositeMetadata):
-    for item in composite_metadata.items:
-        if item.encoding == b'text/plain':
-            storage.last_metadata_push = item.content
-
-
-@router.channel('channel')
-async def channel_response(payload, composite_metadata):
-    logging.info('Got channel request')
-    subscriber = LoggingSubscriber()
-    channel = response_stream_1(local_subscriber=subscriber)
-    return channel, subscriber
-
-
-@router.stream('slow_stream')
-async def stream_slow(**kwargs):
-    logging.info('Got slow stream request')
-    return response_stream_2(delay_between_messages=timedelta(seconds=2))
-
-
-async def authenticator(route: str, authentication: Authentication):
-    if isinstance(authentication, AuthenticationSimple):
-        if authentication.password != b'12345':
-            raise Exception('Authentication error')
-    else:
-        raise Exception('Unsupported authentication')
-
-
-def handler_factory():
-    return RoutingRequestHandler(router, authenticator)
-
-
-def client_handler_factory(on_ready=None):
-    def handle_client(reader, writer):
-        RSocketServer(TransportTCP(reader, writer, read_buffer_size=data_size + 3000),
-                      handler_factory=handler_factory,
-                      # fragment_size_bytes=64_000,
-                      on_ready=on_ready
-                      )
-
-    return handle_client
-
-
-async def run_server(server_port, on_ready=None):
-    logging.info('Starting server at localhost:%s', server_port)
-
-    server = await asyncio.start_server(client_handler_factory(on_ready), 'localhost', server_port, limit=data_size)
-
-    async with server:
-        await server.serve_forever()
-
-
-if __name__ == '__main__':
-    port = sys.argv[1] if len(sys.argv) > 1 else 6565
-    logging.basicConfig(level=logging.ERROR)
-    asyncio.run(run_server(port))
+            raise Exception('Authentication required but not provided')
```

### Comparing `rsocket-0.4.9/rsocket/awaitable/awaitable_rsocket.py` & `rsocket-0.4.dev1/rsocket/handlers/request_stream_requester.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-import asyncio
-from typing import List, Optional
-
-from reactivestreams.publisher import Publisher
-from rsocket.awaitable.collector_subscriber import CollectorSubscriber
-from rsocket.frame import MAX_REQUEST_N
-from rsocket.local_typing import Awaitable
+from reactivestreams.subscriber import Subscriber
+from rsocket.frame import ErrorFrame, PayloadFrame, Frame, error_frame_to_exception
+from rsocket.frame_builders import to_request_stream_frame
+from rsocket.helpers import payload_from_frame, DefaultPublisherSubscription
 from rsocket.payload import Payload
 from rsocket.rsocket import RSocket
+from rsocket.streams.stream_handler import StreamHandler
 
 
-class AwaitableRSocket:
-
-    def __init__(self, rsocket: RSocket):
-        self._rsocket = rsocket
-
-    def fire_and_forget(self, payload: Payload) -> Awaitable[None]:
-        return self._rsocket.fire_and_forget(payload)
-
-    def metadata_push(self, metadata: bytes) -> Awaitable[None]:
-        return self._rsocket.metadata_push(metadata)
-
-    async def request_response(self, payload: Payload) -> Payload:
-        return await self._rsocket.request_response(payload)
-
-    async def request_stream(self,
-                             payload: Payload,
-                             limit_rate=MAX_REQUEST_N) -> List[Payload]:
-        subscriber = CollectorSubscriber(limit_rate)
-
-        self._rsocket.request_stream(payload).initial_request_n(limit_rate).subscribe(subscriber)
-
-        return await subscriber.run()
-
-    async def request_channel(self,
-                              payload: Payload,
-                              publisher: Optional[Publisher] = None,
-                              limit_rate=MAX_REQUEST_N,
-                              sending_done: Optional[asyncio.Event] = None) -> List[Payload]:
-        subscriber = CollectorSubscriber(limit_rate)
-
-        self._rsocket.request_channel(payload,
-                                      publisher=publisher,
-                                      sending_done=sending_done).initial_request_n(limit_rate).subscribe(subscriber)
-
-        return await subscriber.run()
-
-    async def __aenter__(self):
-        await self._rsocket.__aenter__()
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self._rsocket.__aexit__(exc_type, exc_val, exc_tb)
-
-    async def connect(self):
-        return await self._rsocket.connect()
-
-    def close(self):
-        self._rsocket.close()
+class RequestStreamRequester(StreamHandler, DefaultPublisherSubscription):
+    def __init__(self, socket: RSocket, payload: Payload):
+        super().__init__(socket)
+        self.payload = payload
+
+    def setup(self):
+        pass
+
+    def subscribe(self, subscriber: Subscriber):
+        super().subscribe(subscriber)
+        self._send_stream_request(self.payload)
+
+    def cancel(self):
+        super().cancel()
+        self.send_cancel()
+
+    def request(self, n: int):
+        self.send_request_n(n)
+
+    def frame_received(self, frame: Frame):
+        if isinstance(frame, PayloadFrame):
+            if frame.flags_next:
+                self._subscriber.on_next(payload_from_frame(frame),
+                                         is_complete=frame.flags_complete)
+            elif frame.flags_complete:
+                self._subscriber.on_complete()
+
+            if frame.flags_complete:
+                self._finish_stream()
+        elif isinstance(frame, ErrorFrame):
+            self._subscriber.on_error(error_frame_to_exception(frame))
+            self._finish_stream()
+
+    def _send_stream_request(self, payload: Payload):
+        self.socket.send_request(to_request_stream_frame(
+            stream_id=self.stream_id,
+            payload=payload,
+            initial_request_n=self._initial_request_n,
+            fragment_size_bytes=self.socket.get_fragment_size_bytes()
+        ))
```

### Comparing `rsocket-0.4.9/rsocket/exceptions.py` & `rsocket-0.4.dev1/rsocket/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,46 +12,28 @@
 
 
 class RSocketUnknownMimetype(RSocketError):
     def __init__(self, mimetype_id):
         self.mimetype_id = mimetype_id
 
 
-class RSocketUnknownAuthType(RSocketError):
-    def __init__(self, auth_type_id):
-        self.auth_type_id = auth_type_id
-
-
 class RSocketMimetypeTooLong(RSocketError):
     def __init__(self, mimetype):
         self.mimetype = mimetype
 
 
 class RSocketUnknownFrameType(RSocketError):
     def __init__(self, frame_type_id):
         self.frame_type_id = frame_type_id
 
 
 class RSocketApplicationError(RSocketError):
     pass
 
 
-class RSocketEmptyRoute(RSocketApplicationError):
-    def __init__(self, method_name: str):
-        self.method_name = method_name
-
-    def __str__(self) -> str:
-        return f'Empty route set on method {self.method_name}'
-
-
-class RSocketUnknownRoute(RSocketApplicationError):
-    def __init__(self, route_id: str):
-        self.route_id = route_id
-
-
 class RSocketStreamAllocationFailure(RSocketError):
     pass
 
 
 class RSocketValueError(RSocketError):
     pass
 
@@ -76,13 +58,9 @@
     pass
 
 
 class RSocketTransportError(RSocketError):
     pass
 
 
-class RSocketTransportClosed(RSocketError):
-    pass
-
-
 class RSocketNoAvailableTransport(RSocketError):
     pass
```

### Comparing `rsocket-0.4.9/rsocket/extensions/authentication.py` & `rsocket-0.4.dev1/rsocket/extensions/authentication.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/extensions/authentication_content.py` & `rsocket-0.4.dev1/rsocket/extensions/authentication_content.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,28 @@
     __slots__ = 'authentication'
 
     def __init__(self, authentication: Optional[Authentication] = None):
         super().__init__(WellKnownMimeTypes.MESSAGE_RSOCKET_AUTHENTICATION.value.name, None)
         self.authentication = authentication
 
     def serialize(self) -> bytes:
-        serialized = serialize_well_known_encoding(self.authentication.type, WellKnownAuthenticationTypes.get_by_name)
+        serialized = b''
+
+        serialized += serialize_well_known_encoding(self.authentication.type, WellKnownAuthenticationTypes.get_by_name)
 
         serialized += self.authentication.serialize()
 
         return serialized
 
     def parse(self, buffer: bytes):
         authentication_type, offset = parse_well_known_encoding(buffer, WellKnownAuthenticationTypes.require_by_id)
         self.authentication = authentication_item_factory(authentication_type)()
         self.authentication.parse(buffer[offset:])
 
 
-metadata_item_factory_by_type = {
-    WellKnownAuthenticationTypes.SIMPLE.value.name: AuthenticationSimple,
-    WellKnownAuthenticationTypes.BEARER.value.name: AuthenticationBearer,
-}
-
-
 def authentication_item_factory(metadata_encoding: bytes) -> Type[Authentication]:
+    metadata_item_factory_by_type = {
+        WellKnownAuthenticationTypes.SIMPLE.value.name: AuthenticationSimple,
+        WellKnownAuthenticationTypes.BEARER.value.name: AuthenticationBearer,
+    }
+
     return metadata_item_factory_by_type[metadata_encoding]
```

### Comparing `rsocket-0.4.9/rsocket/extensions/authentication_types.py` & `rsocket-0.4.dev1/rsocket/extensions/authentication_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from enum import unique, Enum
 from typing import Optional
 
-from rsocket.exceptions import RSocketUnknownAuthType
-from rsocket.helpers import WellKnownType, map_type_names_by_id, \
-    map_type_ids_by_name
+from rsocket.helpers import WellKnownType
 
 
 class WellKnownAuthenticationType(WellKnownType):
     pass
 
 
 @unique
 class WellKnownAuthenticationTypes(Enum):
     SIMPLE = WellKnownAuthenticationType(b'simple', 0x00)
     BEARER = WellKnownAuthenticationType(b'bearer', 0x01)
 
     @classmethod
-    def require_by_id(cls, numeric_id: int) -> WellKnownAuthenticationType:
-        try:
-            return type_by_id[numeric_id]
-        except KeyError:
-            raise RSocketUnknownAuthType(numeric_id)
+    def require_by_id(cls, metadata_numeric_id: int) -> WellKnownAuthenticationType:
+        for value in cls:
+            if value.value.id == metadata_numeric_id:
+                return value.value
+
+        raise Exception('Unknown authentication type id')
 
     @classmethod
     def get_by_name(cls, metadata_name: str) -> Optional[WellKnownAuthenticationType]:
-        return type_by_name.get(metadata_name)
-
+        for value in cls:
+            if value.value.name == metadata_name:
+                return value.value
 
-type_by_id = map_type_names_by_id(WellKnownAuthenticationTypes)
-type_by_name = map_type_ids_by_name(WellKnownAuthenticationTypes)
+        return None
```

### Comparing `rsocket-0.4.9/rsocket/extensions/composite_metadata.py` & `rsocket-0.4.dev1/rsocket/extensions/composite_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import List, Type, Union
+from typing import List, Type
 
 from rsocket.extensions.authentication_content import AuthenticationContent
 from rsocket.extensions.composite_metadata_item import CompositeMetadataItem
-from rsocket.extensions.mimetypes import WellKnownMimeTypes, ensure_encoding_name
+from rsocket.extensions.mimetypes import WellKnownMimeTypes
 from rsocket.extensions.routing import RoutingMetadata
 from rsocket.extensions.stream_data_mimetype import StreamDataMimetype
 from rsocket.extensions.stream_data_mimetype import StreamDataMimetypes
 from rsocket.frame_helpers import (pack_24bit_length, unpack_24bit)
 from rsocket.helpers import parse_well_known_encoding, serialize_well_known_encoding
 
 _default = object()
@@ -14,46 +14,41 @@
 
 def default_or_value(value, default=None):
     if value is _default:
         return default
     return value
 
 
-metadata_item_factory_by_type = {
-    WellKnownMimeTypes.MESSAGE_RSOCKET_ROUTING.value.name: RoutingMetadata,
-    WellKnownMimeTypes.MESSAGE_RSOCKET_MIMETYPE.value.name: StreamDataMimetype,
-    WellKnownMimeTypes.MESSAGE_RSOCKET_ACCEPT_MIMETYPES.value.name: StreamDataMimetypes,
-    WellKnownMimeTypes.MESSAGE_RSOCKET_AUTHENTICATION.value.name: AuthenticationContent
-}
-
-
 def metadata_item_factory(metadata_encoding: bytes) -> Type[CompositeMetadataItem]:
+    metadata_item_factory_by_type = {
+        WellKnownMimeTypes.MESSAGE_RSOCKET_ROUTING.value.name: RoutingMetadata,
+        WellKnownMimeTypes.MESSAGE_RSOCKET_MIMETYPE.value.name: StreamDataMimetype,
+        WellKnownMimeTypes.MESSAGE_RSOCKET_ACCEPT_MIMETYPES.value.name: StreamDataMimetypes,
+        WellKnownMimeTypes.MESSAGE_RSOCKET_AUTHENTICATION.value.name: AuthenticationContent
+    }
+
     return metadata_item_factory_by_type.get(metadata_encoding, CompositeMetadataItem)
 
 
 class CompositeMetadata:
     __slots__ = 'items'
 
     def __init__(self, items: List[CompositeMetadataItem] = _default):
 
         self.items: List[CompositeMetadataItem] = default_or_value(items, [])
 
     def append(self, item: CompositeMetadataItem) -> 'CompositeMetadata':
         self.items.append(item)
         return self
 
-    def find_by_mimetype(self, mimetype: Union[WellKnownMimeTypes, str, bytes]) -> List[CompositeMetadataItem]:
-        mimetype_name = ensure_encoding_name(mimetype)
-        return [item for item in self.items if ensure_encoding_name(item.encoding) == mimetype_name]
-
     def extend(self, *items: CompositeMetadataItem) -> 'CompositeMetadata':
         self.items.extend(items)
         return self
 
-    def parse(self, metadata: bytes) -> 'CompositeMetadata':
+    def parse(self, metadata: bytes):
         composite_length = len(metadata)
         offset = 0
 
         while offset < composite_length:
             metadata_encoding, relative_offset = parse_well_known_encoding(metadata[offset:],
                                                                            WellKnownMimeTypes.require_by_id)
             offset += relative_offset
@@ -67,16 +62,14 @@
             item_metadata = metadata[offset:offset + length]
             metadata_length = len(item_metadata)
             item.parse(item_metadata)
 
             self.append(item)
             offset += metadata_length
 
-        return self
-
     def serialize(self) -> bytes:
         serialized = b''
 
         for item in self.items:
             metadata_header = serialize_well_known_encoding(item.encoding, WellKnownMimeTypes.get_by_name)
             item_metadata = item.serialize()
```

### Comparing `rsocket-0.4.9/rsocket/extensions/composite_metadata_item.py` & `rsocket-0.4.dev1/rsocket/extensions/composite_metadata_item.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, Optional
 
-from rsocket.extensions.mimetypes import WellKnownMimeTypes, WellKnownMimeType, ensure_well_known_encoding_enum_value
+from rsocket.extensions.mimetypes import WellKnownMimeTypes
 
 _default = object()
 
 
 def default_or_value(value, default=None):
     if value is _default:
         return default
@@ -14,17 +14,17 @@
 class CompositeMetadataItem:
     __slots__ = (
         'encoding',
         'content'
     )
 
     def __init__(self,
-                 encoding: Union[bytes, WellKnownMimeTypes, WellKnownMimeType] = _default,
+                 encoding: Union[bytes, WellKnownMimeTypes] = _default,
                  body: Optional[bytes] = _default):
-        self.encoding = ensure_well_known_encoding_enum_value(default_or_value(encoding))
+        self.encoding = default_or_value(encoding)
         self.content = default_or_value(body)
 
     def parse(self, buffer: bytes):
         self.content = buffer
 
     def serialize(self) -> bytes:
         return self.content
```

### Comparing `rsocket-0.4.9/rsocket/extensions/helpers.py` & `rsocket-0.4.dev1/rsocket/extensions/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 def composite(*items) -> bytes:
     metadata = CompositeMetadata()
     metadata.extend(*items)
     return metadata.serialize()
 
 
-def metadata_item(data: bytes,
-                  encoding: Union[bytes, WellKnownMimeTypes, WellKnownMimeType]) -> CompositeMetadataItem:
+def metadata_item(data: bytes, encoding: Union[bytes, WellKnownMimeTypes]) -> CompositeMetadataItem:
     return CompositeMetadataItem(encoding, data)
 
 
 def authenticate_simple(username: str, password: str) -> CompositeMetadataItem:
     return AuthenticationContent(AuthenticationSimple(username, password))
 
 
@@ -27,19 +26,19 @@
     return AuthenticationContent(AuthenticationBearer(token))
 
 
 def route(*paths: str) -> CompositeMetadataItem:
     return RoutingMetadata(list(paths))
 
 
-def data_mime_type(metadata_mime_type: Union[bytes, WellKnownMimeType]) -> StreamDataMimetype:
+def data_mime_type(metadata_mime_type: Union[bytes, WellKnownMimeType]) -> CompositeMetadataItem:
     return StreamDataMimetype(metadata_mime_type)
 
 
-def data_mime_types(*metadata_mime_types: Union[bytes, WellKnownMimeType]) -> StreamDataMimetypes:
+def data_mime_types(*metadata_mime_types: Union[bytes, WellKnownMimeType]) -> CompositeMetadataItem:
     return StreamDataMimetypes(list(metadata_mime_types))
 
 
 def require_route(composite_metadata: CompositeMetadata) -> str:
     for item in composite_metadata.items:
         if isinstance(item, RoutingMetadata):
             return item.tags[0].decode()
```

### Comparing `rsocket-0.4.9/rsocket/extensions/mimetypes.py` & `rsocket-0.4.dev1/rsocket/extensions/mimetypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from enum import Enum, unique
-from typing import Optional, Union
+from typing import Optional
 
 from rsocket.exceptions import RSocketUnknownMimetype
-from rsocket.extensions.mimetype import WellKnownMimeType
 from rsocket.frame_helpers import ensure_bytes
-from rsocket.helpers import map_type_names_by_id, map_type_ids_by_name
+from rsocket.helpers import WellKnownType
+
+
+class WellKnownMimeType(WellKnownType):
+    pass
 
 
 @unique
 class WellKnownMimeTypes(Enum):
     UNPARSEABLE_MIME_TYPE = WellKnownMimeType(b'UNPARSEABLE_MIME_TYPE_DO_NOT_USE', -2)
     UNKNOWN_RESERVED_MIME_TYPE = WellKnownMimeType(b'UNKNOWN_YET_RESERVED_DO_NOT_USE', -1)
 
@@ -66,33 +69,27 @@
     MESSAGE_RSOCKET_AUTHENTICATION = WellKnownMimeType(b'message/x.rsocket.authentication.v0', 0x7C)
     MESSAGE_RSOCKET_TRACING_ZIPKIN = WellKnownMimeType(b'message/x.rsocket.tracing-zipkin.v0', 0x7D)
     MESSAGE_RSOCKET_ROUTING = WellKnownMimeType(b'message/x.rsocket.routing.v0', 0x7E)
     MESSAGE_RSOCKET_COMPOSITE_METADATA = WellKnownMimeType(b'message/x.rsocket.composite-metadata.v0', 0x7F)
 
     @classmethod
     def require_by_id(cls, metadata_numeric_id: int) -> WellKnownMimeType:
-        try:
-            return mimetype_by_id[metadata_numeric_id]
-        except KeyError:
-            raise RSocketUnknownMimetype(metadata_numeric_id)
+        for value in cls:
+            if value.value.id == metadata_numeric_id:
+                return value.value
+
+        raise RSocketUnknownMimetype(metadata_numeric_id)
 
     @classmethod
     def get_by_name(cls, metadata_name: str) -> Optional[WellKnownMimeType]:
-        return mimetype_by_name.get(metadata_name)
-
+        for value in cls:
+            if value.value.name == metadata_name:
+                return value.value
 
-mimetype_by_id = map_type_names_by_id(WellKnownMimeTypes)
-mimetype_by_name = map_type_ids_by_name(WellKnownMimeTypes)
+        return None
 
 
-def ensure_encoding_name(encoding: Union[WellKnownMimeTypes, str, bytes]) -> bytes:
+def ensure_encoding_name(encoding) -> bytes:
     if isinstance(encoding, WellKnownMimeTypes):
         return encoding.value.name
 
     return ensure_bytes(encoding)
-
-
-def ensure_well_known_encoding_enum_value(data_encoding):
-    if isinstance(data_encoding, WellKnownMimeTypes):
-        data_encoding = data_encoding.value
-
-    return data_encoding
```

### Comparing `rsocket-0.4.9/rsocket/extensions/stream_data_mimetype.py` & `rsocket-0.4.dev1/rsocket/extensions/stream_data_mimetype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from typing import Optional, List, Union
 
 from rsocket.extensions.composite_metadata_item import CompositeMetadataItem
-from rsocket.extensions.mimetypes import WellKnownMimeTypes, WellKnownMimeType, ensure_well_known_encoding_enum_value
+from rsocket.extensions.mimetypes import WellKnownMimeTypes, WellKnownMimeType
 from rsocket.helpers import parse_well_known_encoding, serialize_well_known_encoding
 
 
+def ensure_well_known_encoding_enum_value(data_encoding):
+    if isinstance(data_encoding, WellKnownMimeTypes):
+        data_encoding = data_encoding.value
+
+    return data_encoding
+
+
 class StreamDataMimetype(CompositeMetadataItem):
     __slots__ = (
         'data_encoding'
     )
 
     def __init__(self, data_encoding: Optional[Union[bytes, WellKnownMimeType, WellKnownMimeTypes]] = None):
         super().__init__(WellKnownMimeTypes.MESSAGE_RSOCKET_MIMETYPE.value.name, None)
```

### Comparing `rsocket-0.4.9/rsocket/extensions/tagging.py` & `rsocket-0.4.dev1/rsocket/extensions/tagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,7 +44,8 @@
             offset += tag_length
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.tags == other.tags and self.encoding == other.encoding
 
         return False
+
```

### Comparing `rsocket-0.4.9/rsocket/fragment.py` & `rsocket-0.4.dev1/rsocket/fragment.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/frame.py` & `rsocket-0.4.dev1/rsocket/frame.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import abc
 import struct
 from abc import ABCMeta
 from asyncio import Future
 from enum import IntEnum, unique
-from typing import Optional, Union, Callable
+from typing import Tuple, Optional
 
 from rsocket.error_codes import ErrorCode
 from rsocket.exceptions import RSocketProtocolError, ParseError, RSocketUnknownFrameType
 from rsocket.fragment import Fragment
 from rsocket.frame_fragmenter import data_to_fragments_if_required
-from rsocket.frame_helpers import unpack_position, pack_position, unpack_24bit, pack_24bit, unpack_32bit, \
+from rsocket.frame_helpers import is_flag_set, unpack_position, pack_position, unpack_24bit, pack_24bit, unpack_32bit, \
     ensure_bytes, pack_string, unpack_string
 from rsocket.logger import logger
 
 PROTOCOL_MAJOR_VERSION = 1
 PROTOCOL_MINOR_VERSION = 0
 
 MASK_31_BITS = 0x7FFFFFFF
 CONNECTION_STREAM_ID = 0
 MAX_REQUEST_N = 0x7FFFFFFF
 
-_FLAG_IGNORE_BIT = 0x200
 _FLAG_METADATA_BIT = 0x100
+_FLAG_IGNORE_BIT = 0x200
+_FLAG_COMPLETE_BIT = 0x40
 _FLAG_FOLLOWS_BIT = 0x80
+_FLAG_LEASE_BIT = 0x40
 _FLAG_RESUME_BIT = 0x80
 _FLAG_RESPOND_BIT = 0x80
-_FLAG_LEASE_BIT = 0x40
-_FLAG_COMPLETE_BIT = 0x40
 _FLAG_NEXT_BIT = 0x20
 
 MINIMUM_FRAGMENT_SIZE_BYTES = 64
 
 
 @unique
 class FrameType(IntEnum):
@@ -46,106 +46,57 @@
     PAYLOAD = 10
     ERROR = 11
     METADATA_PUSH = 12
     RESUME = 13
     RESUME_OK = 14
     EXT = 0xFFFF
 
-    @staticmethod
-    def from_id(frame_type_id):
-        try:
-            return FrameType(frame_type_id)
-        except ValueError as exception:
-            raise RSocketUnknownFrameType(frame_type_id) from exception
-
 
 HEADER_LENGTH = 6  # A full header is 4 (stream) + 2 (type, flags) bytes.
 
 
 class Header:
     __slots__ = (
         'length',
-        'prefix_length',
         'frame_type',
         'stream_id',
         'flags_ignore',
-        '_flags_metadata'
+        'flags_metadata'
     )
 
-    @property
-    def flags_metadata(self):
-        return self._flags_metadata
-
-    @flags_metadata.setter
-    def flags_metadata(self, value):
-        self._flags_metadata = value
-
 
 def is_blank(value: Optional[bytes]) -> bool:
     return value is None or len(value) == 0
 
 
-class Flags:
-    __slots__ = [
-        'flags_ignore',
-        'flags_metadata',
-        'flags_follows_resume_respond',
-        'flags_complete_lease',
-        'flags_next',
-    ]
-
-
-class ParseHelper:
-    parse_header: Callable = None
-
-
-try:
-    import cbitstruct
-
-
-    def parse_header_cbitstruct(frame: Header, buffer: bytes, offset: int) -> Flags:
-        frame.length = len(buffer)
-        flags = Flags()
-        (_, frame.stream_id, frame_type_id,
-         frame.flags_ignore,
-         frame.flags_metadata,
-         flags.flags_follows_resume_respond,
-         flags.flags_complete_lease,
-         flags.flags_next) = cbitstruct.unpack_from('u1u31u6b1b1b1b1b1', buffer, offset)
-
-        frame.frame_type = FrameType.from_id(frame_type_id)
-
-        return flags
+def parse_header(frame: Header, buffer: bytes, offset: int) -> int:
+    frame.length = len(buffer)
+    frame.stream_id, frame.frame_type, flags = struct.unpack_from('>IBB', buffer, offset)
+    flags |= (frame.frame_type & 3) << 8
+    frame_type_id = frame.frame_type >> 2
 
+    try:
+        frame.frame_type = FrameType(frame_type_id)
+    except ValueError as exception:
+        raise RSocketUnknownFrameType(frame_type_id) from exception
 
-    parse_header = parse_header_cbitstruct
-except ImportError:
-    from rsocket.frame_helpers import is_flag_set
-
-    def parse_header_native(frame: Header, buffer: bytes, offset: int) -> Flags:
-        frame.length = len(buffer)
-        frame.stream_id, frame.frame_type, flag_bits = struct.unpack_from('>IBB', buffer, offset)
-        flag_bits |= (frame.frame_type & 3) << 8
-        frame_type_id = frame.frame_type >> 2
-
-        flags = Flags()
-        frame.frame_type = FrameType.from_id(frame_type_id)
-
-        frame.flags_ignore = is_flag_set(flag_bits, _FLAG_IGNORE_BIT)
-        frame.flags_metadata = is_flag_set(flag_bits, _FLAG_METADATA_BIT)
-        flags.flags_follows_resume_respond = is_flag_set(flag_bits, _FLAG_FOLLOWS_BIT)
-        flags.flags_complete_lease = is_flag_set(flag_bits, _FLAG_COMPLETE_BIT)
-        flags.flags_next = is_flag_set(flag_bits, _FLAG_NEXT_BIT)
-
-        return flags
-
+    frame.flags_ignore = is_flag_set(flags, _FLAG_IGNORE_BIT)
+    frame.flags_metadata = is_flag_set(flags, _FLAG_METADATA_BIT)
+    return flags
 
-    parse_header = parse_header_native
 
-ParseHelper.parse_header = parse_header
+class FragmentableFrame:
+    __slots__ = (
+        'metadata',
+        'data',
+        'flags_follows',
+        'flags_complete',
+        'flags_next',
+        'stream_id'
+    )
 
 
 class Frame(Header, metaclass=ABCMeta):
     __slots__ = (
         'metadata',
         'data',
         'flags_follows',
@@ -154,15 +105,14 @@
         'sent_future',
         'fragment_size_bytes',
         'fragment_generator'
     )
 
     def __init__(self, frame_type: FrameType):
         self.length = 0
-        self.prefix_length = 0
         self.frame_type = frame_type
         self.stream_id = CONNECTION_STREAM_ID
         self.metadata = b''
         self.data = b''
 
         self.flags_ignore = False
         self.flags_metadata = False
@@ -170,22 +120,14 @@
         self.flags_complete = False
         self.metadata_only = False
 
         self.fragment_size_bytes: Optional[int] = None
         self.fragment_generator = None
         self.sent_future: Optional[Future] = None
 
-    @property
-    def flags_metadata(self):
-        return self.metadata or self._flags_metadata
-
-    @flags_metadata.setter
-    def flags_metadata(self, value):
-        self._flags_metadata = value
-
     def parse_metadata(self, buffer: bytes, offset: int) -> int:
         if not self.flags_metadata:
             return 0
 
         if not self.metadata_only:
             length = unpack_24bit(buffer, offset)
             offset += 3
@@ -201,93 +143,64 @@
         self.data = buffer[offset:offset + length]
         return length
 
     @abc.abstractmethod
     def parse(self, buffer: bytes, offset: int):
         ...
 
-    def serialize_frame_prefix(self, middle=b'', flags: int = 0) -> bytes:
+    def serialize(self, middle=b'', flags: int = 0) -> bytes:
         flags &= ~(_FLAG_IGNORE_BIT | _FLAG_METADATA_BIT)
         if self.flags_ignore:
             flags |= _FLAG_IGNORE_BIT
         if self.metadata:
+            self.flags_metadata = True
             flags |= _FLAG_METADATA_BIT
 
-        self.length = self.compute_frame_length(middle)
-        self.prefix_length = self._compute_frame_prefix_length(middle)
+        self.length = self._compute_frame_length(middle)
 
         offset = 0
-        buffer = bytearray(self.prefix_length)
+        buffer = bytearray(self.length)
 
         struct.pack_into('>I', buffer, offset, self.stream_id)
         offset += 4
 
         buffer[offset] = (self.frame_type << 2) | (flags >> 8)
         offset += 1
         buffer[offset] = flags & 0xff
         offset += 1
 
         buffer[offset:offset + len(middle)] = middle[:]
         offset += len(middle)
 
-        if self.metadata:
-            if not self.metadata_only:
-                buffer[offset:offset + 3] = pack_24bit(len(self.metadata))
-                offset += 3
-
-        return buffer
-
-    def serialize(self, middle=b'', flags: int = 0) -> bytes:
-        prefix_buffer = self.serialize_frame_prefix(middle, flags)
-
-        offset = 0
-        buffer = bytearray(len(prefix_buffer) + self._compute_data_metadata_length())
-        buffer[:len(prefix_buffer)] = prefix_buffer
-        offset += len(prefix_buffer)
-
         if self.flags_metadata and self.metadata:
             length = len(self.metadata)
+            if not self.metadata_only:
+                buffer[offset:offset + 3] = pack_24bit(length)
+                offset += 3
             buffer[offset:offset + length] = self.metadata[:]
             offset += length
 
         if not self.metadata_only and self.data:
             buffer[offset:offset + len(self.data)] = self.data[:]
             offset += len(self.data)
 
         return bytes(buffer)
 
-    def write_data_metadata(self, writer_method):
-        if self.metadata:
-            writer_method(self.metadata)
-
-        if not self.metadata_only and self.data:
-            writer_method(self.data)
-
-    def compute_frame_length(self, middle: bytes = b'') -> int:
-        return self._compute_frame_prefix_length(middle) + self._compute_data_metadata_length()
-
-    def _compute_data_metadata_length(self):
-        length = 0
-
-        if self.flags_metadata and self.metadata:
-            length += len(self.metadata)
-
-        if not self.metadata_only and self.data:
-            length += len(self.data)
-
-        return length
-
-    def _compute_frame_prefix_length(self, middle: bytes = b'') -> int:
+    def _compute_frame_length(self, middle: bytes) -> int:
         header_length = HEADER_LENGTH
         length = header_length + len(middle)
 
         if self.flags_metadata and self.metadata:
+            length += len(self.metadata)
             if not self.metadata_only:
                 length += 3
 
+        if not self.metadata_only and self.data:
+            length += len(self.data)
+
         return length
 
     def __str__(self):
         return str(f'({FrameType(self.frame_type).name},{self.data},{self.metadata},{self.flags_complete})')
 
 
 class FrameFragmentMixin(metaclass=abc.ABCMeta):
@@ -300,20 +213,49 @@
                 get_header_length(self),
                 self.fragment_size_bytes,
                 requires_length_header
             )
 
         try:
             fragment = self.fragment_generator.__next__()
-            return new_frame_fragment(self, fragment)
+            return self._new_frame_fragment(fragment)
         except GeneratorExit:
             return None
         except StopIteration:
             return None
 
+    def _new_frame_fragment(self, fragment: Fragment) -> 'Frame':
+        if fragment.is_first:
+            frame = self.__class__()
+        else:
+            frame = PayloadFrame()
+
+        if isinstance(frame, PayloadFrame):
+            if not is_blank(frame.data) or not is_blank(frame.metadata):
+                frame.flags_next = True
+
+        frame.stream_id = self.stream_id
+
+        frame.flags_ignore = self.flags_ignore
+        frame.flags_metadata = self.flags_metadata
+        frame.metadata_only = self.metadata_only
+
+        if hasattr(self, 'initial_request_n'):
+            frame.initial_request_n = self.initial_request_n
+
+        frame.data = fragment.data
+        frame.metadata = fragment.metadata
+        frame.flags_follows = fragment.is_last is False
+
+        if fragment.is_last is None or fragment.is_last:
+            frame.sent_future = self.sent_future
+            frame.flags_complete = self.flags_complete
+
+        return frame
+
 
 class SetupFrame(Frame):
     __slots__ = (
         'major_version',
         'minor_version',
         'keep_alive_milliseconds',
         'max_lifetime_milliseconds',
@@ -330,18 +272,18 @@
         self.major_version = PROTOCOL_MAJOR_VERSION
         self.minor_version = PROTOCOL_MINOR_VERSION
         self.flags_lease = False
         self.flags_resume = False
 
     # noinspection PyAttributeOutsideInit
     def parse(self, buffer: bytes, offset: int):
-        flags = ParseHelper.parse_header(self, buffer, offset)
+        flags = parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
-        self.flags_lease = flags.flags_complete_lease
-        self.flags_resume = flags.flags_follows_resume_respond
+        self.flags_lease = is_flag_set(flags, _FLAG_LEASE_BIT)
+        self.flags_resume = is_flag_set(flags, _FLAG_RESUME_BIT)
 
         (self.major_version, self.minor_version,
          self.keep_alive_milliseconds, self.max_lifetime_milliseconds) = (
             struct.unpack_from('>HHII', buffer, offset))
 
         offset += 12
 
@@ -356,60 +298,54 @@
         offset += length + 1
         length, self.data_encoding = unpack_string(buffer, offset)
         offset += length + 1
 
         offset += self.parse_metadata(buffer, offset)
         offset += self.parse_data(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0) -> bytes:
+    def serialize(self, middle=b'', flags=0) -> bytes:
         flags &= ~(_FLAG_LEASE_BIT | _FLAG_RESUME_BIT)
-
         if self.flags_lease:
             flags |= _FLAG_LEASE_BIT
-
         if self.flags_resume:
             flags |= _FLAG_RESUME_BIT
-
         middle = struct.pack(
             '>HHII', self.major_version, self.minor_version,
             self.keep_alive_milliseconds, self.max_lifetime_milliseconds)
-
         if self.flags_resume:
             middle += struct.pack('>H', self.token_length)
             # assert len(self.resume_identification_token) == self.token_length
             # assert isinstance(self.resume_identification_token, bytes)
             middle += self.resume_identification_token
-
         middle += pack_string(self.metadata_encoding)
         middle += pack_string(self.data_encoding)
-
-        return super().serialize_frame_prefix(middle, flags)
+        return Frame.serialize(self, middle, flags)
 
 
 class InvalidFrame:
-    frame_type = None
+    pass
 
 
 class ErrorFrame(Frame):
     __slots__ = 'error_code'
 
     def __init__(self):
         super().__init__(FrameType.ERROR)
 
     # noinspection PyAttributeOutsideInit
     def parse(self, buffer: bytes, offset: int):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
         self.error_code = ErrorCode(unpack_32bit(buffer, offset))
         offset += 4
         offset += self.parse_data(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0) -> bytes:
+    def serialize(self, middle=b'', flags=0) -> bytes:
         middle = struct.pack('>I', self.error_code)
-        return super().serialize_frame_prefix(middle, flags)
+        return Frame.serialize(self, middle, flags)
 
 
 class LeaseFrame(Frame):
     __slots__ = (
         'time_to_live',
         'number_of_requests'
     )
@@ -417,123 +353,123 @@
     def __init__(self):
         super().__init__(FrameType.LEASE)
         self.metadata_only = True
         self.time_to_live = None
         self.number_of_requests = None
 
     def parse(self, buffer: bytes, offset: int):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
         time_to_live, number_of_requests = struct.unpack_from('>II', buffer, offset)
         self.time_to_live = time_to_live & MASK_31_BITS
         self.number_of_requests = number_of_requests & MASK_31_BITS
         offset += self.parse_metadata(buffer, offset + 8)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0):
+    def serialize(self, middle=b'', flags=0):
         middle = struct.pack('>II',
                              self.time_to_live & MASK_31_BITS,
                              self.number_of_requests & MASK_31_BITS)
-        return super().serialize_frame_prefix(middle, flags)
+        return Frame.serialize(self, middle, flags)
 
 
 class KeepAliveFrame(Frame):
     __slots__ = ('flags_respond', 'last_received_position')
 
     def __init__(self, data=b'', metadata=b''):
         super().__init__(FrameType.KEEPALIVE)
         self.stream_id = CONNECTION_STREAM_ID
         self.flags_respond = False
         self.data = data
         self.metadata = metadata
         self.last_received_position = 0
 
     def parse(self, buffer: bytes, offset: int):
-        flags = ParseHelper.parse_header(self, buffer, offset)
+        flags = parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
-        self.flags_respond = flags.flags_follows_resume_respond
+        self.flags_respond = is_flag_set(flags, _FLAG_RESPOND_BIT)
         self.last_received_position = unpack_position(buffer[offset:offset + 8])
         offset += 8
         offset += self.parse_data(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags: int = 0) -> bytes:
+    def serialize(self, middle=b'', flags: int = 0) -> bytes:
         flags &= ~_FLAG_RESPOND_BIT
         if self.flags_respond:
             flags |= _FLAG_RESPOND_BIT
         middle += pack_position(self.last_received_position)
-        return super().serialize_frame_prefix(middle, flags)
+        return Frame.serialize(self, middle, flags)
 
 
 class RequestFrame(Frame):
     __slots__ = (
         'flags_follows',
     )
 
     def __init__(self, frame_type):
         super().__init__(frame_type)
         self.flags_follows = False
 
-    def parse(self, buffer, offset: int):
-        flags = ParseHelper.parse_header(self, buffer, offset)
-        self.flags_follows = flags.flags_follows_resume_respond
-        return flags
+    def parse(self, buffer, offset: int) -> Tuple[int, int]:
+        flags = parse_header(self, buffer, offset)
+        self.flags_follows = is_flag_set(flags, _FLAG_FOLLOWS_BIT)
+        return HEADER_LENGTH, flags
 
-    def serialize_frame_prefix(self, middle=b'', flags: int = 0) -> bytes:
+    def serialize(self, middle=b'', flags: int = 0) -> bytes:
         flags &= ~_FLAG_FOLLOWS_BIT
 
         if self.flags_follows:
             flags |= _FLAG_FOLLOWS_BIT
 
-        return super().serialize_frame_prefix(middle, flags)
+        return Frame.serialize(self, middle, flags)
 
     def _parse_payload(self, buffer: bytes, offset: int):
         offset += self.parse_metadata(buffer, offset)
         offset += self.parse_data(buffer, offset)
 
 
 class RequestResponseFrame(RequestFrame, FrameFragmentMixin):
     __slots__ = ()
 
     def __init__(self):
         super().__init__(FrameType.REQUEST_RESPONSE)
 
     def parse(self, buffer, offset):
-        RequestFrame.parse(self, buffer, offset)
-        offset += HEADER_LENGTH
+        header = RequestFrame.parse(self, buffer, offset)
+        offset += header[0]
         self._parse_payload(buffer, offset)
 
 
 class RequestFireAndForgetFrame(RequestFrame, FrameFragmentMixin):
     __slots__ = ()
 
     def __init__(self):
         super().__init__(FrameType.REQUEST_FNF)
 
     def parse(self, buffer, offset):
-        RequestFrame.parse(self, buffer, offset)
-        offset += HEADER_LENGTH
+        header = RequestFrame.parse(self, buffer, offset)
+        offset += header[0]
         self._parse_payload(buffer, offset)
 
 
 class RequestStreamFrame(RequestFrame, FrameFragmentMixin):
     __slots__ = 'initial_request_n'
 
     def __init__(self):
         super().__init__(FrameType.REQUEST_STREAM)
         self.initial_request_n = 0
 
     def parse(self, buffer, offset):
-        RequestFrame.parse(self, buffer, offset)
-        offset += HEADER_LENGTH
+        header = RequestFrame.parse(self, buffer, offset)
+        offset += header[0]
         self.initial_request_n = unpack_32bit(buffer, offset)
         offset += 4
         self._parse_payload(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0):
+    def serialize(self, middle=b'', flags=0):
         middle = struct.pack('>I', self.initial_request_n)
-        return super().serialize_frame_prefix(middle)
+        return RequestFrame.serialize(self, middle)
 
 
 class RequestChannelFrame(RequestFrame, FrameFragmentMixin):
     __slots__ = (
         'initial_request_n',
         'flags_complete',
         'flags_follows',
@@ -541,57 +477,57 @@
 
     def __init__(self):
         super().__init__(FrameType.REQUEST_CHANNEL)
         self.flags_complete = False
 
     # noinspection PyAttributeOutsideInit
     def parse(self, buffer, offset):
-        flags = RequestFrame.parse(self, buffer, offset)
-        offset += HEADER_LENGTH
-        self.flags_complete = flags.flags_complete_lease
-        self.flags_follows = flags.flags_follows_resume_respond
+        header = RequestFrame.parse(self, buffer, offset)
+        offset += header[0]
+        flags = header[1]
+        self.flags_complete = is_flag_set(flags, _FLAG_COMPLETE_BIT)
+        self.flags_follows = is_flag_set(flags, _FLAG_FOLLOWS_BIT)
         self.initial_request_n = unpack_32bit(buffer, offset)
         offset += 4
         self._parse_payload(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0):
+    def serialize(self, middle=b'', flags=0):
         middle = struct.pack('>I', self.initial_request_n)
 
         flags &= ~_FLAG_COMPLETE_BIT
-
         if self.flags_complete:
             flags |= _FLAG_COMPLETE_BIT
 
-        return super().serialize_frame_prefix(middle, flags)
+        return RequestFrame.serialize(self, middle, flags)
 
 
 class RequestNFrame(RequestFrame):
     __slots__ = 'request_n'
 
     def __init__(self):
         super().__init__(FrameType.REQUEST_N)
 
     # noinspection PyAttributeOutsideInit
     def parse(self, buffer, offset):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
         self.request_n = unpack_32bit(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0):
+    def serialize(self, middle=b'', flags=0):
         middle = struct.pack('>I', self.request_n)
-        return super().serialize_frame_prefix(middle, flags)
+        return Frame.serialize(self, middle, flags)
 
 
 class CancelFrame(Frame):
 
     def __init__(self):
         super().__init__(FrameType.CANCEL)
 
     def parse(self, buffer, offset):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
 
 
 class PayloadFrame(Frame, FrameFragmentMixin):
     __slots__ = (
         'flags_follows',
         'flags_complete',
         'flags_next'
@@ -600,23 +536,23 @@
     def __init__(self):
         super().__init__(FrameType.PAYLOAD)
         self.flags_follows = False
         self.flags_complete = False
         self.flags_next = False
 
     def parse(self, buffer, offset):
-        flags = ParseHelper.parse_header(self, buffer, offset)
+        flags = parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
-        self.flags_follows = flags.flags_follows_resume_respond
-        self.flags_complete = flags.flags_complete_lease
-        self.flags_next = flags.flags_next
+        self.flags_follows = is_flag_set(flags, _FLAG_FOLLOWS_BIT)
+        self.flags_complete = is_flag_set(flags, _FLAG_COMPLETE_BIT)
+        self.flags_next = is_flag_set(flags, _FLAG_NEXT_BIT)
         offset += self.parse_metadata(buffer, offset)
         offset += self.parse_data(buffer, offset)
 
-    def serialize_frame_prefix(self, middle=b'', flags=0):
+    def serialize(self, middle=b'', flags=0):
         flags &= ~(_FLAG_FOLLOWS_BIT | _FLAG_COMPLETE_BIT |
                    _FLAG_NEXT_BIT)
 
         if self.flags_follows:
             flags |= _FLAG_FOLLOWS_BIT
 
         if self.flags_complete:
@@ -624,28 +560,28 @@
 
         if not is_blank(self.data) or not is_blank(self.metadata):
             self.flags_next = True
 
         if self.flags_next:
             flags |= _FLAG_NEXT_BIT
 
-        return super().serialize_frame_prefix(flags=flags)
+        return Frame.serialize(self, flags=flags)
 
 
 class MetadataPushFrame(Frame):
     __slots__ = ()
 
     def __init__(self):
         super().__init__(FrameType.METADATA_PUSH)
         self.stream_id = CONNECTION_STREAM_ID
         self.metadata_only = True
         self.flags_metadata = True
 
     def parse(self, buffer, offset):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
         offset += self.parse_metadata(buffer, offset)
 
 
 class ResumeFrame(Frame):
     __slots__ = (
         'major_version',
@@ -659,62 +595,64 @@
     def __init__(self):
         super().__init__(FrameType.RESUME)
         self.major_version = PROTOCOL_MAJOR_VERSION
         self.minor_version = PROTOCOL_MINOR_VERSION
 
     # noinspection PyAttributeOutsideInit
     def parse(self, buffer: bytes, offset: int):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
 
-        self.major_version, self.minor_version = (
+        (self.major_version, self.minor_version) = (
             struct.unpack_from('>HH', buffer, offset))
 
         offset += 4
 
         self.token_length = struct.unpack_from('>H', buffer, offset)[0]
         offset += 2
-        self.resume_identification_token = buffer[offset:offset + self.token_length]
+        self.resume_identification_token = (
+            buffer[offset:offset + self.token_length])
         offset += self.token_length
+
         self.last_server_position = unpack_position(buffer[offset:offset + 8])
         offset += 8
         self.first_client_position = unpack_position(buffer[offset:])
 
-    def serialize_frame_prefix(self, middle=b'', flags=0) -> bytes:
+    def serialize(self, middle=b'', flags=0) -> bytes:
         flags &= ~(_FLAG_LEASE_BIT | _FLAG_RESUME_BIT)
 
         middle = struct.pack('>HH', self.major_version, self.minor_version)
         middle += struct.pack('>H', len(self.resume_identification_token))
         # assert len(self.resume_identification_token) == self.token_length
         # assert isinstance(self.resume_identification_token, bytes)
         middle += self.resume_identification_token
 
         middle += pack_position(self.last_server_position)
         middle += pack_position(self.first_client_position)
 
-        return super().serialize_frame_prefix(middle)
+        return Frame.serialize(self, middle)
 
 
 class ResumeOKFrame(Frame):
     __slots__ = (
         'last_received_client_position'
     )
 
     def __init__(self):
         super().__init__(FrameType.RESUME_OK)
         self.last_received_client_position = 0
 
     def parse(self, buffer: bytes, offset: int):
-        ParseHelper.parse_header(self, buffer, offset)
+        parse_header(self, buffer, offset)
         offset += HEADER_LENGTH
         self.last_received_client_position = unpack_position(buffer[offset:offset + 8])
 
-    def serialize_frame_prefix(self, middle=b'', flags: int = 0) -> bytes:
+    def serialize(self, middle=b'', flags: int = 0) -> bytes:
         serialized = pack_position(self.last_received_client_position)
-        return super().serialize_frame_prefix(serialized)
+        return super().serialize(serialized)
 
 
 class ExtendedFrame(Frame, metaclass=abc.ABCMeta):
     __slots__ = (
         'extended_type'
     )
 
@@ -745,15 +683,15 @@
 
 
 def parse_or_ignore(buffer: bytes) -> Optional[Frame]:
     if len(buffer) < HEADER_LENGTH:
         raise ParseError('Frame too short: {} bytes'.format(len(buffer)))
 
     header = Header()
-    ParseHelper.parse_header(header, buffer, 0)
+    parse_header(header, buffer, 0)
 
     frame = _frame_class_by_id[header.frame_type]()
 
     try:
         frame.parse(buffer, 0)
 
         if not is_frame_to_ignore(frame):
@@ -778,61 +716,24 @@
         RequestResponseFrame,
         RequestChannelFrame,
         RequestStreamFrame,
         RequestFireAndForgetFrame
     ))
 
 
-FragmentableFrame = Union[PayloadFrame,
-RequestResponseFrame,
-RequestChannelFrame,
-RequestStreamFrame,
-RequestFireAndForgetFrame]
-
-
-def new_frame_fragment(base_frame: FragmentableFrame, fragment: Fragment) -> Frame:
-    if fragment.is_first:
-        frame = base_frame.__class__()
-    else:
-        frame = PayloadFrame()
-
-    if isinstance(frame, PayloadFrame):
-        if not is_blank(frame.data) or not is_blank(frame.metadata):
-            frame.flags_next = True
-
-    frame.stream_id = base_frame.stream_id
-
-    frame.flags_ignore = base_frame.flags_ignore
-    frame.flags_metadata = base_frame.flags_metadata
-    frame.metadata_only = base_frame.metadata_only
-
-    if hasattr(base_frame, 'initial_request_n'):
-        frame.initial_request_n = base_frame.initial_request_n
-
-    frame.data = fragment.data
-    frame.metadata = fragment.metadata
-    frame.flags_follows = fragment.is_last is False
-
-    if fragment.is_last is None or fragment.is_last:
-        frame.sent_future = base_frame.sent_future
-        frame.flags_complete = base_frame.flags_complete
-
-    return frame
-
-
 def exception_to_error_frame(stream_id: int, exception: Exception) -> ErrorFrame:
     frame = ErrorFrame()
     frame.stream_id = stream_id
 
     if isinstance(exception, RSocketProtocolError):
         frame.error_code = exception.error_code
         frame.data = ensure_bytes(exception.data)
     else:
         frame.error_code = ErrorCode.APPLICATION_ERROR
-        frame.data = ensure_bytes(str(exception))
+        frame.data = str(exception).encode()
 
     return frame
 
 
 def error_frame_to_exception(frame: ErrorFrame) -> Exception:
     if frame.error_code != ErrorCode.APPLICATION_ERROR:
         return RSocketProtocolError(frame.error_code, data=frame.data.decode())
@@ -843,21 +744,14 @@
 def serialize_with_frame_size_header(frame: Frame) -> bytes:
     serialized_frame = frame.serialize()
     header = struct.pack('>I', len(serialized_frame))[1:]
     full_frame = header + serialized_frame
     return full_frame
 
 
-def serialize_prefix_with_frame_size_header(frame: Frame) -> bytes:
-    serialized_frame_prefix = frame.serialize_frame_prefix()
-    header = struct.pack('>I', frame.length)[1:]
-    full_frame = header + serialized_frame_prefix
-    return full_frame
-
-
 initiate_request_frame_types = (RequestResponseFrame,
                                 RequestStreamFrame,
                                 RequestChannelFrame,
                                 RequestFireAndForgetFrame
                                 )
 
 frame_header_length = {
@@ -865,9 +759,9 @@
     RequestResponseFrame: 6,
     RequestFireAndForgetFrame: 6,
     RequestStreamFrame: 10,
     RequestChannelFrame: 10,
 }
 
 
-def get_header_length(frame: FragmentableFrame) -> int:
+def get_header_length(frame: Frame) -> int:
     return frame_header_length[frame.__class__]
```

### Comparing `rsocket-0.4.9/rsocket/frame_builders.py` & `rsocket-0.4.dev1/rsocket/frame_builders.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/frame_fragment_cache.py` & `rsocket-0.4.dev1/rsocket/frame_fragment_cache.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/frame_fragmenter.py` & `rsocket-0.4.dev1/rsocket/frame_fragmenter.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,18 +34,14 @@
         if self._is_first:
             return self.first_fragment_size_bytes
         else:
             return self.next_frame_header_size
 
     def __iter__(self):
 
-        if self._data_length == 0 and self._metadata_length == 0:
-            yield Fragment(None, None, is_last=True, is_first=True)
-            return
-
         data_reader = BytesIO(self.data)
         metadata_reader = BytesIO(self.metadata)
 
         while True:
             metadata_fragment = metadata_reader.read(self._get_next_fragment_body_size())
             self._metadata_read_length += len(metadata_fragment)
```

### Comparing `rsocket-0.4.9/rsocket/frame_parser.py` & `rsocket-0.4.dev1/rsocket/frame_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import struct
 from typing import AsyncGenerator
 
+from rsocket import frame
 from rsocket.logger import logger
 
 __all__ = ['FrameParser']
 
-from rsocket.frame import Frame, InvalidFrame, parse_or_ignore
+from rsocket.frame import Frame, InvalidFrame
 
 
 class FrameParser:
     def __init__(self):
         self._buffer = bytearray()
 
     async def receive_data(self, data: bytes, header_length=3) -> AsyncGenerator[Frame, None]:
@@ -24,15 +25,16 @@
             else:
                 length = len(data)
 
             if total < length + frame_length_byte_count:
                 return
 
             try:
-                new_frame = parse_or_ignore(self._buffer[frame_length_byte_count:length + frame_length_byte_count])
+                new_frame = frame.parse_or_ignore(
+                    self._buffer[frame_length_byte_count:length + frame_length_byte_count])
 
                 if new_frame is not None:
                     yield new_frame
             except Exception:
                 logger().error('Error parsing frame', exc_info=True)
                 yield InvalidFrame()
```

### Comparing `rsocket-0.4.9/rsocket/handlers/request_cahnnel_common.py` & `rsocket-0.4.dev1/rsocket/handlers/request_cahnnel_common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import abc
-import asyncio
 from typing import Optional
 
 from reactivestreams.publisher import Publisher
 from reactivestreams.subscriber import Subscriber, DefaultSubscriber
 from reactivestreams.subscription import Subscription
-from rsocket.disposable import Disposable
 from rsocket.frame import CancelFrame, ErrorFrame, RequestNFrame, \
     PayloadFrame, Frame, error_frame_to_exception
 from rsocket.helpers import payload_from_frame
 from rsocket.logger import logger
 from rsocket.payload import Payload
 from rsocket.rsocket import RSocket
 from rsocket.streams.stream_handler import StreamHandler
@@ -35,38 +33,34 @@
         self._requester.mark_completed_and_finish(sent=True)
 
     def on_error(self, exception):
         self._socket.send_error(self._stream_id, exception)
         self._requester.mark_completed_and_finish(sent=True)
 
 
-class RequestChannelCommon(StreamHandler, Publisher, Subscription, Disposable, metaclass=abc.ABCMeta):
+class RequestChannelCommon(StreamHandler, Publisher, Subscription, metaclass=abc.ABCMeta):
 
-    def __init__(self,
-                 socket: RSocket,
-                 publisher: Optional[Publisher] = None,
-                 sending_done: Optional[asyncio.Event] = None):
+    def __init__(self, socket: RSocket, remote_publisher: Optional[Publisher] = None):
         super().__init__(socket)
-        self._sending_done = sending_done
         self.remote_subscriber = None
         self._sent_complete = False
         self._received_complete = False
-        self._publisher = publisher
+        self._remote_publisher = remote_publisher
         self.subscriber = None
 
     def setup(self):
         self.subscriber = StreamSubscriber(self.stream_id, self.socket, self)
 
-        if self._publisher is not None:
-            self._publisher.subscribe(self.subscriber)
+        if self._remote_publisher is not None:
+            self._remote_publisher.subscribe(self.subscriber)
 
     def frame_received(self, frame: Frame):
         if isinstance(frame, CancelFrame):
             self.subscriber.subscription.cancel()
-            self.mark_completed_and_finish(sent=True)
+            self._finish_stream()
         elif isinstance(frame, RequestNFrame):
             if self.subscriber.subscription is not None:
                 self.subscriber.subscription.request(frame.request_n)
             else:
                 logger().warning('%s: Received request_n but no publisher provided', self.__class__.__name__)
 
         elif isinstance(frame, PayloadFrame):
@@ -78,49 +72,36 @@
 
             if frame.flags_complete:
                 self.mark_completed_and_finish(received=True)
         elif isinstance(frame, ErrorFrame):
             self.remote_subscriber.on_error(error_frame_to_exception(frame))
             self.mark_completed_and_finish(received=True)
 
-    def dispose(self):
-        if self.subscriber is not None and self.subscriber.subscription is not None:
-            self.subscriber.subscription.cancel()
-
     def _complete_remote_subscriber(self):
         if self.remote_subscriber is not None:
             self.remote_subscriber.on_complete()
 
         self.mark_completed_and_finish(received=True)
 
     def mark_completed_and_finish(self, received=None, sent=None):
-
         if received:
             self._received_complete = True
-
         if sent:
             self._sent_complete = True
-            self._set_sending_done()
-
         self._finish_if_both_closed()
 
     def _finish_if_both_closed(self):
         if self._received_complete and self._sent_complete:
             self._finish_stream()
 
-    def subscribe(self, subscriber: Optional[Subscriber]):
+    def subscribe(self, subscriber: Subscriber):
         if subscriber is not None:
             self.remote_subscriber = subscriber
             self.remote_subscriber.on_subscribe(self)
         else:
             self.mark_completed_and_finish(received=True)
 
     def cancel(self):
         self.send_cancel()
-        self.mark_completed_and_finish(received=True)
-
-    def _set_sending_done(self):
-        if self._sending_done is not None:
-            self._sending_done.set()
 
     def request(self, n: int):
         self.send_request_n(n)
```

### Comparing `rsocket-0.4.9/rsocket/handlers/request_cahnnel_responder.py` & `rsocket-0.4.dev1/rsocket/handlers/request_cahnnel_responder.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/handlers/request_channel_requester.py` & `rsocket-0.4.dev1/rsocket/awaitable/awaitable_rsocket.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,55 @@
-import asyncio
-from typing import Optional
+from typing import List, Optional
 
 from reactivestreams.publisher import Publisher
-from reactivestreams.subscriber import Subscriber
-from rsocket.frame_builders import to_request_channel_frame
-from rsocket.handlers.interfaces import Requester
-from rsocket.handlers.request_cahnnel_common import RequestChannelCommon
+from rsocket.awaitable.collector_subscriber import CollectorSubscriber
+from rsocket.frame import MAX_REQUEST_N
+from rsocket.local_typing import Awaitable
 from rsocket.payload import Payload
 from rsocket.rsocket import RSocket
 
 
-class RequestChannelRequester(RequestChannelCommon, Requester):
+class AwaitableRSocket:
 
-    def __init__(self,
-                 socket: RSocket,
-                 payload: Payload,
-                 publisher: Optional[Publisher] = None,
-                 sending_done: Optional[asyncio.Event] = None):
-        super().__init__(socket, publisher, sending_done)
-        self._payload = payload
-
-    def setup(self):
-        super().setup()
-
-    def _send_channel_request(self, payload: Payload):
-        self.socket.send_request(
-            to_request_channel_frame(stream_id=self.stream_id,
-                                     payload=payload,
-                                     initial_request_n=self._initial_request_n,
-                                     complete=self._publisher is None,
-                                     fragment_size_bytes=self.socket.get_fragment_size_bytes())
-        )
-
-    def subscribe(self, subscriber: Subscriber):
-        self.setup()
-        super().subscribe(subscriber)
-        self._send_channel_request(self._payload)
+    def __init__(self, rsocket: RSocket):
+        self._rsocket = rsocket
 
-        if self._publisher is None:
-            self.mark_completed_and_finish(sent=True)
+    def fire_and_forget(self, payload: Payload) -> Awaitable[None]:
+        return self._rsocket.fire_and_forget(payload)
+
+    def metadata_push(self, metadata: bytes) -> Awaitable[None]:
+        return self._rsocket.metadata_push(metadata)
+
+    async def request_response(self, payload: Payload) -> Payload:
+        return await self._rsocket.request_response(payload)
+
+    async def request_stream(self,
+                             payload: Payload,
+                             initial_request_n=MAX_REQUEST_N) -> List[Payload]:
+        subscriber = CollectorSubscriber()
+
+        self._rsocket.request_stream(payload).initial_request_n(initial_request_n).subscribe(subscriber)
+
+        return await subscriber.run()
+
+    async def request_channel(self,
+                              payload: Payload,
+                              publisher: Optional[Publisher] = None,
+                              initial_request_n=MAX_REQUEST_N) -> List[Payload]:
+        subscriber = CollectorSubscriber()
+
+        self._rsocket.request_channel(payload, publisher).initial_request_n(initial_request_n).subscribe(subscriber)
+
+        return await subscriber.run()
+
+    async def __aenter__(self):
+        await self._rsocket.__aenter__()
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self._rsocket.__aexit__(exc_type, exc_val, exc_tb)
+
+    async def connect(self):
+        return await self._rsocket.connect()
+
+    def close(self):
+        self._rsocket.close()
```

### Comparing `rsocket-0.4.9/rsocket/handlers/request_response_requester.py` & `rsocket-0.4.dev1/rsocket/handlers/request_response_requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 
 from rsocket.frame import ErrorFrame, PayloadFrame, Frame, error_frame_to_exception
 from rsocket.frame_builders import to_request_response_frame
-from rsocket.handlers.interfaces import Requester
 from rsocket.helpers import create_future, payload_from_frame
 from rsocket.local_typing import Awaitable
 from rsocket.payload import Payload
 from rsocket.rsocket import RSocket
 from rsocket.streams.stream_handler import StreamHandler
 
 
-class RequestResponseRequester(StreamHandler, Requester):
+class RequestResponseRequester(StreamHandler):
     def __init__(self, socket: RSocket, payload: Payload):
         super().__init__(socket)
         self._payload = payload
         self._future = create_future()
 
     def setup(self):
         self._future.add_done_callback(self._on_future_complete)
@@ -36,8 +35,7 @@
 
     def _on_future_complete(self, future: asyncio.Future):
         if future.cancelled():
             self.cancel()
 
     def cancel(self):
         self.send_cancel()
-        self._finish_stream()
```

### Comparing `rsocket-0.4.9/rsocket/handlers/request_response_responder.py` & `rsocket-0.4.dev1/rsocket/handlers/request_response_responder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from asyncio import Future
 
-from rsocket.disposable import Disposable
 from rsocket.frame import CancelFrame, Frame
 from rsocket.rsocket import RSocket
 from rsocket.streams.stream_handler import StreamHandler
 
 
-class RequestResponseResponder(StreamHandler, Disposable):
+class RequestResponseResponder(StreamHandler):
     def __init__(self, socket: RSocket, future: Future):
         super().__init__(socket)
         self.future = future
 
     def setup(self):
         self.future.add_done_callback(self.future_done)
 
@@ -21,14 +20,11 @@
             self.socket.send_payload(
                 self.stream_id, future.result(), complete=True)
         else:
             self.socket.send_error(self.stream_id, future.exception())
 
         self._finish_stream()
 
-    def dispose(self):
-        self.future.cancel()
-
     def frame_received(self, frame: Frame):
         if isinstance(frame, CancelFrame):
             self.future.cancel()
             self._finish_stream()
```

### Comparing `rsocket-0.4.9/rsocket/handlers/request_stream_requester.py` & `rsocket-0.4.dev1/rsocket/stream_control.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,67 @@
-from reactivestreams.subscriber import Subscriber
-from rsocket.frame import ErrorFrame, PayloadFrame, Frame, error_frame_to_exception
-from rsocket.frame_builders import to_request_stream_frame
-from rsocket.handlers.interfaces import Requester
-from rsocket.helpers import payload_from_frame, DefaultPublisherSubscription
-from rsocket.payload import Payload
-from rsocket.rsocket import RSocket
+from typing import Dict
+
+from rsocket.error_codes import ErrorCode
+from rsocket.exceptions import RSocketStreamAllocationFailure, RSocketStreamIdInUse
+from rsocket.frame import CONNECTION_STREAM_ID, Frame, ErrorFrame
 from rsocket.streams.stream_handler import StreamHandler
 
+MAX_STREAM_ID = 0x7FFFFFFF
+
+
+class StreamControl:
+    def __init__(self, first_stream_id: int):
+        self._first_stream_id = first_stream_id
+        self._current_stream_id = self._first_stream_id
+        self._streams: Dict[int, StreamHandler] = {}
+        self._maximum_stream_id = MAX_STREAM_ID
+
+    def allocate_stream(self) -> int:
+        attempt_counter = 0
+
+        while (self._current_stream_id == CONNECTION_STREAM_ID
+               or self._current_stream_id in self._streams):
+
+            if attempt_counter > self._maximum_stream_id / 2:
+                raise RSocketStreamAllocationFailure()
+
+            self._increment_stream_id()
+            attempt_counter += 1
+
+        return self._current_stream_id
+
+    def _increment_stream_id(self):
+        self._current_stream_id = (self._current_stream_id + 2) & self._maximum_stream_id
+
+    def finish_stream(self, stream_id: int):
+        self._streams.pop(stream_id, None)
+
+    def register_stream(self, stream_id: int, handler: StreamHandler):
+        if stream_id == CONNECTION_STREAM_ID:
+            raise RuntimeError('Attempt to allocate handler to connection stream id')
+
+        if stream_id > self._maximum_stream_id:
+            raise RuntimeError('Stream id larger then maximum allowed')
+
+        self._streams[stream_id] = handler
+
+    def handle_stream(self, frame: Frame) -> bool:
+        stream_id = frame.stream_id
+
+        if stream_id in self._streams:
+            self._streams[stream_id].frame_received(frame)
+            return True
+
+        return False
+
+    def stop_all_streams(self, error_code=ErrorCode.CANCELED, data=b''):
+        for stream_id, stream in list(self._streams.items()):
+            frame = ErrorFrame()
+            frame.stream_id = stream_id
+            frame.error_code = error_code
+            frame.data = data
+            stream.frame_received(frame)
+            self.finish_stream(stream_id)
 
-class RequestStreamRequester(StreamHandler, DefaultPublisherSubscription, Requester):
-    def __init__(self, socket: RSocket, payload: Payload):
-        super().__init__(socket)
-        self.payload = payload
-
-    def setup(self):
-        pass
-
-    def subscribe(self, subscriber: Subscriber):
-        super().subscribe(subscriber)
-        self._send_stream_request(self.payload)
-
-    def cancel(self):
-        self.send_cancel()
-        self._finish_stream()
-
-    def request(self, n: int):
-        self.send_request_n(n)
-
-    def frame_received(self, frame: Frame):
-        if isinstance(frame, PayloadFrame):
-            if frame.flags_next:
-                self._subscriber.on_next(payload_from_frame(frame),
-                                         is_complete=frame.flags_complete)
-            elif frame.flags_complete:
-                self._subscriber.on_complete()
-
-            if frame.flags_complete:
-                self._finish_stream()
-        elif isinstance(frame, ErrorFrame):
-            self._subscriber.on_error(error_frame_to_exception(frame))
-            self._finish_stream()
-
-    def _send_stream_request(self, payload: Payload):
-        self.socket.send_request(to_request_stream_frame(
-            stream_id=self.stream_id,
-            payload=payload,
-            initial_request_n=self._initial_request_n,
-            fragment_size_bytes=self.socket.get_fragment_size_bytes()
-        ))
+    def assert_stream_id_available(self, stream_id: int):
+        if stream_id in self._streams:
+            raise RSocketStreamIdInUse(stream_id)
```

### Comparing `rsocket-0.4.9/rsocket/handlers/request_stream_responder.py` & `rsocket-0.4.dev1/rsocket/handlers/request_stream_responder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from typing import Union
-
 from reactivestreams.publisher import Publisher
 from reactivestreams.subscriber import DefaultSubscriber
-from rsocket.disposable import Disposable
 from rsocket.frame import CancelFrame, RequestNFrame, \
     RequestStreamFrame, Frame
 from rsocket.payload import Payload
 from rsocket.rsocket import RSocket
 from rsocket.streams.stream_handler import StreamHandler
 
 
@@ -30,17 +27,17 @@
         self.socket.finish_stream(self.stream_id)
 
     def on_error(self, exception: Exception):
         self.socket.send_error(self.stream_id, exception)
         self.socket.finish_stream(self.stream_id)
 
 
-class RequestStreamResponder(StreamHandler, Disposable):
+class RequestStreamResponder(StreamHandler):
 
-    def __init__(self, socket: RSocket, publisher: Union[Publisher, Disposable]):
+    def __init__(self, socket: RSocket, publisher: Publisher):
         super().__init__(socket)
         self.publisher = publisher
         self.subscriber = None
 
     def setup(self):
         self.subscriber = StreamSubscriber(self.stream_id, self.socket)
         self.publisher.subscribe(self.subscriber)
@@ -50,11 +47,7 @@
             self.setup()
             self.subscriber.subscription.request(frame.initial_request_n)
         elif isinstance(frame, CancelFrame):
             self.subscriber.subscription.cancel()
             self._finish_stream()
         elif isinstance(frame, RequestNFrame):
             self.subscriber.subscription.request(frame.request_n)
-
-    def dispose(self):
-        if self.subscriber is not None and self.subscriber.subscription is not None:
-            self.subscriber.subscription.cancel()
```

### Comparing `rsocket-0.4.9/rsocket/lease.py` & `rsocket-0.4.dev1/rsocket/lease.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/load_balancer/load_balancer_rsocket.py` & `rsocket-0.4.dev1/rsocket/load_balancer/load_balancer_rsocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import Union, Optional, Any
 
 from reactivestreams.publisher import Publisher
 from rsocket.load_balancer.load_balancer_strategy import LoadBalancerStrategy
 from rsocket.local_typing import Awaitable
 from rsocket.payload import Payload
 from rsocket.rsocket import RSocket
@@ -10,20 +9,17 @@
 
 
 class LoadBalancerRSocket(RSocket):
 
     def __init__(self, strategy: LoadBalancerStrategy):
         self._strategy = strategy
 
-    def request_channel(self,
-                        payload: Payload,
-                        publisher: Optional[Publisher] = None,
-                        sending_done: Optional[asyncio.Event] = None) -> Union[Any, Publisher]:
+    def request_channel(self, payload: Payload, local_publisher: Optional[Publisher] = None) -> Union[Any, Publisher]:
         return self._select_client().request_channel(
-            payload, publisher, sending_done
+            payload, local_publisher
         )
 
     def request_response(self, payload: Payload) -> Awaitable[Payload]:
         return self._select_client().request_response(payload)
 
     def fire_and_forget(self, payload: Payload) -> Awaitable[None]:
         return self._select_client().fire_and_forget(payload)
```

### Comparing `rsocket-0.4.9/rsocket/load_balancer/random_client.py` & `rsocket-0.4.dev1/rsocket/load_balancer/random_client.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/load_balancer/round_robin.py` & `rsocket-0.4.dev1/rsocket/load_balancer/round_robin.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/queue_peekable.py` & `rsocket-0.4.dev1/rsocket/queue_peekable.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/reactivex/from_rsocket_publisher.py` & `rsocket-0.4.dev1/rsocket/rx_support/from_rsocket_publisher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import asyncio
 import functools
 
-import reactivex
-from reactivex import Observable, Observer
-from reactivex.disposable import Disposable
+import rx
+from rx import Observable
+from rx.core import Observer
+from rx.disposable import Disposable
 
 from reactivestreams.publisher import Publisher
 from reactivestreams.subscriber import Subscriber
 from reactivestreams.subscription import Subscription
-from rsocket.frame import MAX_REQUEST_N
 from rsocket.logger import logger
 
 
 class RxSubscriber(Subscriber):
-    def __init__(self, observer: Observer, limit_rate: int = MAX_REQUEST_N):
+    def __init__(self, observer, limit_rate: int):
         self.limit_rate = limit_rate
         self.observer = observer
         self._received_messages = 0
         self.done = asyncio.Event()
         self.get_next_n = asyncio.Event()
         self.subscription = None
 
     def on_subscribe(self, subscription: Subscription):
         self.subscription = subscription
 
     def on_next(self, value, is_complete=False):
         self._received_messages += 1
         self.observer.on_next(value)
-
         if is_complete:
             self.observer.on_completed()
             self._finish()
 
         else:
             if self._received_messages == self.limit_rate:
                 self._received_messages = 0
@@ -57,25 +56,25 @@
     except asyncio.CancelledError:
         if not subscriber.done.is_set():
             subscriber.subscription.cancel()
     except Exception as exception:
         loop.call_soon(functools.partial(observer.on_error, exception))
 
 
-async def _trigger_next_request_n(subscriber: RxSubscriber, limit_rate):
+async def _trigger_next_request_n(subscriber, limit_rate):
     try:
         while True:
             await subscriber.get_next_n.wait()
             subscriber.subscription.request(limit_rate)
             subscriber.get_next_n.clear()
     except asyncio.CancelledError:
         logger().debug('Asyncio task canceled: trigger_next_request_n')
 
 
-def from_rsocket_publisher(publisher: Publisher, limit_rate: int = MAX_REQUEST_N) -> Observable:
+def from_rsocket_publisher(publisher: Publisher, limit_rate=5) -> Observable:
     loop = asyncio.get_event_loop()
 
     # noinspection PyUnusedLocal
     def on_subscribe(observer: Observer, scheduler):
         subscriber = RxSubscriber(observer, limit_rate)
 
         get_next_task = asyncio.create_task(
@@ -87,38 +86,8 @@
 
         def dispose():
             get_next_task.cancel()
             task.cancel()
 
         return Disposable(dispose)
 
-    return reactivex.create(on_subscribe)
-
-
-class RxSubscriberFromObserver(Subscriber):
-    def __init__(self, observer: Observer, limit_rate: int):
-        self.limit_rate = limit_rate
-        self.observer = observer
-        self._received_messages = 0
-        self.subscription = None
-
-    def on_subscribe(self, subscription: Subscription):
-        self.subscription = subscription
-        self.subscription.request(self.limit_rate)
-
-    def on_next(self, value, is_complete=False):
-        self._received_messages += 1
-        self.observer.on_next(value)
-
-        if is_complete:
-            self.observer.on_completed()
-
-        else:
-            if self._received_messages == self.limit_rate:
-                self._received_messages = 0
-                self.subscription.request(self.limit_rate)
-
-    def on_error(self, exception: Exception):
-        self.observer.on_error(exception)
-
-    def on_complete(self):
-        self.observer.on_completed()
+    return rx.create(on_subscribe)
```

### Comparing `rsocket-0.4.9/rsocket/reactivex/reactivex_client.py` & `rsocket-0.4.dev1/rsocket/reactivex/reactivex_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-import asyncio
 from asyncio import Future
-from typing import Optional, cast, Union, Callable
+
+from typing import Optional, cast
 
 import reactivex
-from reactivex import Observable, Subject, operators
+from reactivex import Observable
 
 from rsocket.frame import MAX_REQUEST_N
-from rsocket.helpers import is_non_empty_payload
 from rsocket.payload import Payload
-from rsocket.reactivex.back_pressure_publisher import observable_to_publisher
-from rsocket.reactivex.from_rsocket_publisher import from_rsocket_publisher
 from rsocket.rsocket import RSocket
+from rsocket.reactivex.back_pressure_publisher import BackPressurePublisher
+from rsocket.reactivex.from_rsocket_publisher import from_rsocket_publisher
 
 
 class ReactiveXClient:
     def __init__(self, rsocket: RSocket):
         self._rsocket = rsocket
 
     def request_stream(self, request: Payload, request_limit: int = MAX_REQUEST_N) -> Observable:
         response_publisher = self._rsocket.request_stream(request).initial_request_n(request_limit)
         return from_rsocket_publisher(response_publisher, request_limit)
 
     def request_response(self, request: Payload) -> Observable:
-        return reactivex.from_future(cast(Future, self._rsocket.request_response(request))).pipe(
-            operators.filter(is_non_empty_payload)
-        )
+        return reactivex.from_future(cast(Future, self._rsocket.request_response(request)))
 
     def request_channel(self,
                         request: Payload,
                         request_limit: int = MAX_REQUEST_N,
-                        observable: Optional[Union[Observable, Callable[[Subject], Observable]]] = None,
-                        sending_done: Optional[asyncio.Event] = None) -> Observable:
-        requester_publisher = observable_to_publisher(observable)
+                        observable: Optional[Observable] = None) -> Observable:
+        if observable is not None:
+            local_publisher = BackPressurePublisher(observable)
+        else:
+            local_publisher = None
 
         response_publisher = self._rsocket.request_channel(
-            request, requester_publisher, sending_done
+            request, local_publisher
         ).initial_request_n(request_limit)
         return from_rsocket_publisher(response_publisher, request_limit)
 
     def fire_and_forget(self, request: Payload) -> Observable:
         return reactivex.from_future(cast(Future, self._rsocket.fire_and_forget(request)))
 
     def metadata_push(self, metadata: bytes) -> Observable:
```

### Comparing `rsocket-0.4.9/rsocket/reactivex/reactivex_handler.py` & `rsocket-0.4.dev1/rsocket/request_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,107 @@
-from abc import abstractmethod
+import asyncio
+from abc import ABCMeta, abstractmethod
 from datetime import timedelta
-from typing import Optional, Union, Callable
-
-from reactivex import Observable, Subject
+from typing import Tuple, Optional
 
+from reactivestreams.publisher import Publisher
+from reactivestreams.subscriber import Subscriber
 from rsocket.error_codes import ErrorCode
 from rsocket.extensions.composite_metadata import CompositeMetadata
+from rsocket.helpers import create_error_future
+from rsocket.local_typing import Awaitable
 from rsocket.logger import logger
 from rsocket.payload import Payload
-from rsocket.reactivex.reactivex_channel import ReactivexChannel
 
 
-class ReactivexHandler:
+class RequestHandler(metaclass=ABCMeta):
+
+    def __init__(self, socket):
+        super().__init__()
+        self.socket = socket
 
     @abstractmethod
     async def on_setup(self,
                        data_encoding: bytes,
                        metadata_encoding: bytes,
                        payload: Payload):
         ...
 
     @abstractmethod
     async def on_metadata_push(self, metadata: Payload):
         ...
 
     @abstractmethod
-    async def request_channel(self, payload: Payload) -> ReactivexChannel:
-        ...
+    async def request_channel(self,
+                              payload: Payload
+                              ) -> Tuple[Optional[Publisher], Optional[Subscriber]]:
+        """
+        Bi-Directional communication.  A publisher on each end is connected
+        to a subscriber on the other end.
+        """
 
     @abstractmethod
     async def request_fire_and_forget(self, payload: Payload):
         ...
 
     @abstractmethod
-    async def request_response(self, payload: Payload) -> Observable:
+    async def request_response(self, payload: Payload) -> asyncio.Future:
         ...
 
     @abstractmethod
-    async def request_stream(self, payload: Payload) -> Union[Observable, Callable[[Subject], Observable]]:
+    async def request_stream(self, payload: Payload) -> Publisher:
         ...
 
     @abstractmethod
     async def on_error(self, error_code: ErrorCode, payload: Payload):
         ...
 
     @abstractmethod
     async def on_keepalive_timeout(self,
                                    time_since_last_keepalive: timedelta,
                                    rsocket):
         ...
 
     @abstractmethod
-    async def on_connection_error(self, rsocket, exception: Exception):
-        ...
-
-    @abstractmethod
-    async def on_close(self, rsocket, exception: Optional[Exception] = None):
+    async def on_connection_lost(self, rsocket, exception):
         ...
 
     # noinspection PyMethodMayBeStatic
     def _parse_composite_metadata(self, metadata: bytes) -> CompositeMetadata:
-        return CompositeMetadata().parse(metadata)
+        composite_metadata = CompositeMetadata()
+        composite_metadata.parse(metadata)
+        return composite_metadata
 
 
-class BaseReactivexHandler(ReactivexHandler):
+class BaseRequestHandler(RequestHandler):
 
-    async def on_setup(self, data_encoding: bytes, metadata_encoding: bytes, payload: Payload):
+    async def on_setup(self,
+                       data_encoding: bytes,
+                       metadata_encoding: bytes,
+                       payload: Payload):
         """Nothing to do on setup by default"""
 
-    async def on_metadata_push(self, metadata: Payload):
-        """Nothing by default"""
-
-    async def request_channel(self, payload: Payload) -> ReactivexChannel:
+    async def request_channel(self, payload: Payload) -> Tuple[Optional[Publisher], Optional[Subscriber]]:
         raise RuntimeError('Not implemented')
 
     async def request_fire_and_forget(self, payload: Payload):
         """The requester isn't listening for errors.  Nothing to do."""
 
-    async def request_response(self, payload: Payload) -> Observable:
-        raise RuntimeError('Not implemented')
+    async def on_metadata_push(self, payload: Payload):
+        """Nothing by default"""
+
+    async def request_response(self, payload: Payload) -> Awaitable[Payload]:
+        return create_error_future(RuntimeError('Not implemented'))
 
-    async def request_stream(self, payload: Payload) -> Observable:
+    async def request_stream(self, payload: Payload) -> Publisher:
         raise RuntimeError('Not implemented')
 
     async def on_error(self, error_code: ErrorCode, payload: Payload):
-        logger().error('Error handler: %s, %s', error_code.name, payload)
+        logger().error('Error handler: %s, %s', error_code, payload)
 
-    async def on_keepalive_timeout(self, time_since_last_keepalive: timedelta, rsocket):
-        pass
+    async def on_connection_lost(self, rsocket, exception: Exception):
+        await rsocket.close()
 
-    async def on_close(self, rsocket, exception: Optional[Exception] = None):
-        pass
-
-    async def on_connection_error(self, rsocket, exception: Exception):
+    async def on_keepalive_timeout(self,
+                                   time_since_last_keepalive: timedelta,
+                                   rsocket):
         pass
```

### Comparing `rsocket-0.4.9/rsocket/reactivex/reactivex_handler_adapter.py` & `rsocket-0.4.dev1/rsocket/rx_support/rx_rsocket.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,55 @@
-import asyncio
-from datetime import timedelta
-from typing import Tuple, Optional, Callable
-
-from reactivex import operators
-
-from reactivestreams.publisher import Publisher
-from reactivestreams.subscriber import Subscriber
-from rsocket.error_codes import ErrorCode
-from rsocket.payload import Payload
-from rsocket.reactivex.back_pressure_publisher import observable_to_publisher
-from rsocket.reactivex.from_rsocket_publisher import RxSubscriberFromObserver
-from rsocket.reactivex.reactivex_handler import ReactivexHandler
-from rsocket.request_handler import RequestHandler
-
-
-def reactivex_handler_factory(handler_factory: Callable[[], ReactivexHandler]):
-    def create_handler():
-        return ReactivexHandlerAdapter(handler_factory())
-
-    return create_handler
-
-
-class ReactivexHandlerAdapter(RequestHandler):
-
-    def __init__(self, delegate: ReactivexHandler):
-        self.delegate = delegate
-
-    async def on_setup(self, data_encoding: bytes, metadata_encoding: bytes, payload: Payload):
-        await self.delegate.on_setup(data_encoding, metadata_encoding, payload)
-
-    async def on_metadata_push(self, metadata: Payload):
-        await self.on_metadata_push(metadata)
+from typing import Optional
 
-    async def request_channel(self, payload: Payload) -> Tuple[Optional[Publisher], Optional[Subscriber]]:
-        reactivex_channel = await self.delegate.request_channel(payload)
+import rx
+from rx import Observable
 
-        subscriber = None
-        publisher = observable_to_publisher(reactivex_channel.observable)
-
-        if reactivex_channel.observer is not None:
-            subscriber = RxSubscriberFromObserver(reactivex_channel.observer,
-                                                  reactivex_channel.limit_rate)
-
-        return publisher, subscriber
-
-    async def request_fire_and_forget(self, payload: Payload):
-        await self.delegate.request_fire_and_forget(payload)
-
-    async def request_response(self, payload: Payload) -> asyncio.Future:
-        observable = await self.delegate.request_response(payload)
-        return observable.pipe(
-            operators.default_if_empty(Payload()),
-            operators.to_future()
-        )
-
-    async def request_stream(self, payload: Payload) -> Publisher:
-        return observable_to_publisher(await self.delegate.request_stream(payload))
-
-    async def on_error(self, error_code: ErrorCode, payload: Payload):
-        await self.delegate.on_error(error_code, payload)
-
-    async def on_keepalive_timeout(self, time_since_last_keepalive: timedelta, rsocket):
-        await self.delegate.on_keepalive_timeout(time_since_last_keepalive, rsocket)
-
-    async def on_connection_error(self, rsocket, exception: Exception):
-        await self.delegate.on_connection_error(rsocket, exception)
+from rsocket.frame import MAX_REQUEST_N
+from rsocket.payload import Payload
+from rsocket.rsocket import RSocket
+from rsocket.rx_support.back_pressure_publisher import BackPressurePublisher
+from rsocket.rx_support.from_rsocket_publisher import from_rsocket_publisher
+
+
+class RxRSocket:
+    def __init__(self, rsocket: RSocket):
+        self._rsocket = rsocket
+
+    def request_stream(self, request: Payload, request_limit: int = MAX_REQUEST_N) -> Observable:
+        response_publisher = self._rsocket.request_stream(request).initial_request_n(request_limit)
+        return from_rsocket_publisher(response_publisher, request_limit)
+
+    def request_response(self, request: Payload) -> Observable:
+        return rx.from_future(self._rsocket.request_response(request))
+
+    def request_channel(self,
+                        request: Payload,
+                        request_limit: int = MAX_REQUEST_N,
+                        observable: Optional[Observable] = None) -> Observable:
+        if observable is not None:
+            local_publisher = BackPressurePublisher(observable)
+        else:
+            local_publisher = None
+
+        response_publisher = self._rsocket.request_channel(
+            request, local_publisher
+        ).initial_request_n(request_limit)
+        return from_rsocket_publisher(response_publisher, request_limit)
+
+    def fire_and_forget(self, request: Payload) -> rx.Observable:
+        return rx.from_future(self._rsocket.fire_and_forget(request))
+
+    def metadata_push(self, metadata: bytes) -> rx.Observable:
+        return rx.from_future(self._rsocket.metadata_push(metadata))
+
+    async def connect(self):
+        return await self._rsocket.connect()
+
+    async def close(self):
+        await self._rsocket.close()
+
+    async def __aenter__(self):
+        await self._rsocket.__aenter__()
+        return self
 
-    async def on_close(self, rsocket, exception: Optional[Exception] = None):
-        await self.delegate.on_close(rsocket, exception)
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self._rsocket.__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `rsocket-0.4.9/rsocket/routing/helpers.py` & `rsocket-0.4.dev1/rsocket/routing/helpers.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/rsocket.py` & `rsocket-0.4.dev1/rsocket/rsocket_internal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 import abc
-import asyncio
-from typing import Union, Optional, Any
+from typing import Optional
 
-from reactivestreams.publisher import Publisher
-from rsocket.local_typing import Awaitable
+from rsocket.error_codes import ErrorCode
+from rsocket.frame import Frame, RequestFrame
 from rsocket.payload import Payload
-from rsocket.streams.backpressureapi import BackpressureApi
 
 
-class RSocket(metaclass=abc.ABCMeta):
-
-    @abc.abstractmethod
-    def request_channel(
-            self,
-            payload: Payload,
-            publisher: Optional[Publisher] = None,
-            sending_done: Optional[asyncio.Event] = None) -> Union[Any, Publisher]:
-        ...
-
+class RSocketInternal(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def request_response(self, payload: Payload) -> Awaitable[Payload]:
+    def send_frame(self, frame: Frame):
         ...
 
     @abc.abstractmethod
-    def fire_and_forget(self, payload: Payload) -> Awaitable[None]:
+    def send_complete(self, stream_id: int):
         ...
 
     @abc.abstractmethod
-    def request_stream(self, payload: Payload) -> Union[BackpressureApi, Publisher]:
+    def finish_stream(self, stream_id: int):
         ...
 
     @abc.abstractmethod
-    def metadata_push(self, metadata: bytes) -> Awaitable[None]:
+    def send_request(self, frame: RequestFrame):
         ...
 
     @abc.abstractmethod
-    async def connect(self):
+    def send_payload(self, stream_id: int, payload: Payload, complete=False, is_next=True):
         ...
 
     @abc.abstractmethod
-    async def close(self):
+    def send_error(self, stream_id: int, exception: Exception):
         ...
 
     @abc.abstractmethod
-    async def __aenter__(self) -> 'RSocket':
+    def stop_all_streams(self, error_code=ErrorCode.CANCELED, data=b''):
         ...
 
     @abc.abstractmethod
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    def get_fragment_size_bytes(self) -> Optional[int]:
         ...
```

### Comparing `rsocket-0.4.9/rsocket/rsocket_base.py` & `rsocket-0.4.dev1/rsocket/rsocket_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             super().__init__()
             self._socket = socket
 
         def on_next(self, value, is_complete=False):
             self._socket.send_lease(value)
 
     def __init__(self,
-                 handler_factory: Callable[[], RequestHandler] = BaseRequestHandler,
+                 handler_factory: Callable[['RSocketBase'], RequestHandler] = BaseRequestHandler,
                  honor_lease=False,
                  lease_publisher: Optional[Publisher] = None,
                  request_queue_size: int = 0,
                  data_encoding: Union[str, bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
                  metadata_encoding: Union[str, bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
                  keep_alive_period: timedelta = timedelta(milliseconds=500),
                  max_lifetime_period: timedelta = timedelta(minutes=10),
@@ -78,21 +78,34 @@
         self._keep_alive_period = keep_alive_period
         self._setup_payload = setup_payload
         self._data_encoding = ensure_encoding_name(data_encoding)
         self._metadata_encoding = ensure_encoding_name(metadata_encoding)
         self._lease_publisher = lease_publisher
         self._sender_task = None
         self._receiver_task = None
-        self._handler = self._handler_factory()
+        self._handler = self._handler_factory(self)
         self._responder_lease = None
         self._requester_lease = None
         self._is_closing = False
         self._connecting = True
         self._fragment_size_bytes = fragment_size_bytes
 
+        self._async_frame_handler_by_type: Dict[Type[Frame], Any] = {
+            RequestResponseFrame: self.handle_request_response,
+            RequestStreamFrame: self.handle_request_stream,
+            RequestChannelFrame: self.handle_request_channel,
+            SetupFrame: self.handle_setup,
+            RequestFireAndForgetFrame: self.handle_fire_and_forget,
+            MetadataPushFrame: self.handle_metadata_push,
+            ResumeFrame: self.handle_resume,
+            LeaseFrame: self.handle_lease,
+            KeepAliveFrame: self.handle_keep_alive,
+            ErrorFrame: self.handle_error
+        }
+
         self._setup_internals()
 
     def get_fragment_size_bytes(self) -> Optional[int]:
         return self._fragment_size_bytes
 
     def _setup_internals(self):
         pass
@@ -111,15 +124,15 @@
         else:
             self._requester_lease = NullLease()
 
         self._responder_lease = NullLease()
         self._stream_control = StreamControl(self._get_first_stream_id())
         self._is_closing = False
 
-    def stop_all_streams(self, error_code=ErrorCode.CONNECTION_ERROR, data=b''):
+    def stop_all_streams(self, error_code=ErrorCode.CANCELED, data=b''):
         self._stream_control.stop_all_streams(error_code, data)
 
     def _start_tasks(self):
         self._receiver_task = self._start_task_if_not_closing(self._receiver)
         self._sender_task = self._start_task_if_not_closing(self._sender)
 
     async def connect(self):
@@ -133,15 +146,15 @@
         return self
 
     def _start_task_if_not_closing(self, task_factory: Callable[[], Coroutine]) -> Optional[Task]:
         if not self._is_closing:
             return asyncio.create_task(task_factory())
 
     def set_handler_using_factory(self, handler_factory) -> RequestHandler:
-        self._handler = handler_factory()
+        self._handler = handler_factory(self)
         return self._handler
 
     def _allocate_stream(self) -> int:
         return self._stream_control.allocate_stream()
 
     @abc.abstractmethod
     def _get_first_stream_id(self) -> int:
@@ -304,68 +317,50 @@
             self._request_queue.task_done()
 
     async def _receiver(self):
         try:
             await self._receiver_listen()
         except asyncio.CancelledError:
             logger().debug('%s: Asyncio task canceled: receiver', self._log_identifier())
-        except RSocketTransportError:
-            pass
+        except RSocketTransportError as exception:
+            await self._on_connection_lost(exception)
         except Exception:
             logger().error('%s: Unknown error', self._log_identifier(), exc_info=True)
             raise
 
-        await self._on_connection_closed()
-
-    async def _on_connection_error(self, exception: Exception):
+    async def _on_connection_lost(self, exception: Exception):
         logger().warning(str(exception))
         logger().debug(str(exception), exc_info=exception)
-        await self._handler.on_connection_error(self, exception)
-
-    async def _on_connection_closed(self):
-        self.stop_all_streams()
-        await self._handler.on_close(self)
-        await self._stop_tasks()
+        self.stop_all_streams(ErrorCode.CONNECTION_ERROR, b'Connection error')
+        await self._handler.on_connection_lost(self, exception)
 
     @abc.abstractmethod
     def is_server_alive(self) -> bool:
         ...
 
     async def _receiver_listen(self):
-        async_frame_handler_by_type: Dict[Type[Frame], Any] = {
-            RequestResponseFrame: self.handle_request_response,
-            RequestStreamFrame: self.handle_request_stream,
-            RequestChannelFrame: self.handle_request_channel,
-            SetupFrame: self.handle_setup,
-            RequestFireAndForgetFrame: self.handle_fire_and_forget,
-            MetadataPushFrame: self.handle_metadata_push,
-            ResumeFrame: self.handle_resume,
-            LeaseFrame: self.handle_lease,
-            KeepAliveFrame: self.handle_keep_alive,
-            ErrorFrame: self.handle_error
-        }
 
         transport = await self._current_transport()
         while self.is_server_alive():
             next_frame_generator = await transport.next_frame_generator()
             if next_frame_generator is None:
                 break
             async for frame in next_frame_generator:
                 try:
-                    await self._handle_next_frame(frame, async_frame_handler_by_type)
+                    await self._handle_next_frame(frame)
                 except RSocketProtocolError as exception:
                     logger().error('%s: Protocol error %s', self._log_identifier(), str(exception))
                     self.send_error(frame.stream_id, exception)
                 except RSocketTransportError:
                     raise
                 except Exception as exception:
                     logger().error('%s: Unknown error', self._log_identifier(), exc_info=True)
                     self.send_error(frame.stream_id, exception)
 
-    async def _handle_next_frame(self, frame: Frame, async_frame_handler_by_type):
+    async def _handle_next_frame(self, frame: Frame):
 
         log_frame(frame, self._log_identifier())
 
         if isinstance(frame, InvalidFrame):
             return
 
         if is_fragmentable_frame(frame):
@@ -373,23 +368,23 @@
             if complete_frame is None:
                 return
         else:
             complete_frame = frame
 
         if (complete_frame.stream_id == CONNECTION_STREAM_ID or
                 isinstance(complete_frame, initiate_request_frame_types)):
-            await self._handle_frame_by_type(complete_frame, async_frame_handler_by_type)
+            await self._handle_frame_by_type(complete_frame)
         elif self._stream_control.handle_stream(complete_frame):
             return
         else:
-            logger().warning('%s: Dropping frame from unknown stream %d', self._log_identifier(),
-                             complete_frame.stream_id)
+            logger().debug('%s: Dropping frame from unknown stream %d', self._log_identifier(),
+                           complete_frame.stream_id)
 
-    async def _handle_frame_by_type(self, frame: Frame, async_frame_handler_by_type):
-        frame_handler = async_frame_handler_by_type.get(type(frame), async_noop)
+    async def _handle_frame_by_type(self, frame: Frame):
+        frame_handler = self._async_frame_handler_by_type.get(type(frame), async_noop)
         await frame_handler(frame)
 
     def _send_new_keepalive(self, data: bytes = b''):
         self.send_frame(to_keepalive_frame(data))
 
     def _before_sender(self):
         pass
@@ -400,17 +395,15 @@
     @asynccontextmanager
     async def _get_next_frame_to_send(self, transport: Transport) -> Frame:
         next_frame_source = await self._send_queue.peek()
 
         if isinstance(next_frame_source, FrameFragmentMixin):
             next_fragment = next_frame_source.get_next_fragment(transport.requires_length_header())
 
-            if next_fragment.flags_follows:
-                self._send_queue.put_nowait(self._send_queue.get_nowait())  # cycle to next frame source in queue
-            else:
+            if not next_fragment.flags_follows:
                 next_frame_source.get_next_fragment(
                     transport.requires_length_header())  # workaround to clean-up generator.
                 self._send_queue.get_nowait()
 
             yield next_fragment
 
         else:
@@ -429,40 +422,35 @@
                         log_frame(frame, self._log_identifier(), 'Sent')
 
                         if frame.sent_future is not None:
                             frame.sent_future.set_result(None)
 
                     if self._send_queue.empty():
                         await transport.on_send_queue_empty()
-            except RSocketTransportError:
-                pass
+            except RSocketTransportError as exception:
+                await self._on_connection_lost(exception)
 
         except asyncio.CancelledError:
             logger().debug('%s: Asyncio task canceled: sender', self._log_identifier())
+        except RSocketTransportError as exception:
+            await self._on_connection_lost(exception)
         except Exception:
             logger().error('%s: RSocket error', self._log_identifier(), exc_info=True)
             raise
         finally:
             await self._finally_sender()
 
     async def close(self):
         logger().debug('%s: Closing', self._log_identifier())
 
-        await self._stop_tasks()
-
-        await self._close_transport()
-
-    async def _stop_tasks(self):
-        logger().debug('%s: Cleanup', self._log_identifier())
-
         self._is_closing = True
         await cancel_if_task_exists(self._sender_task)
-        self._sender_task = None
         await cancel_if_task_exists(self._receiver_task)
-        self._receiver_task = None
+
+        await self._close_transport()
 
     async def _close_transport(self):
         if self._current_transport().done():
             logger().debug('%s: Closing transport', self._log_identifier())
             try:
                 transport = await self._current_transport()
             except asyncio.CancelledError:
@@ -477,66 +465,45 @@
     async def __aenter__(self) -> 'RSocketBase':
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
     def request_response(self, payload: Payload) -> Awaitable[Payload]:
-        """
-        Initiate a request-response interaction.
-        """
-
         logger().debug('%s: request-response: %s', self._log_identifier(), payload)
 
         requester = RequestResponseRequester(self, payload)
         self.register_new_stream(requester).setup()
         return requester.run()
 
     def fire_and_forget(self, payload: Payload) -> Awaitable[None]:
-        """
-        Initiate a fire-and-forget interaction.
-        """
-
         logger().debug('%s: fire-and-forget: %s', self._log_identifier(), payload)
 
         stream_id = self._allocate_stream()
         frame = to_fire_and_forget_frame(stream_id, payload)
         self.send_request(frame)
-        frame.sent_future.add_done_callback(lambda _: self.finish_stream(stream_id))
+        self.finish_stream(stream_id)
         return frame.sent_future
 
     def request_stream(self, payload: Payload) -> Union[BackpressureApi, Publisher]:
-        """
-        Initiate a request-stream interaction.
-        """
-
         logger().debug('%s: request-stream: %s', self._log_identifier(), payload)
 
         requester = RequestStreamRequester(self, payload)
         return self.register_new_stream(requester)
 
     def request_channel(
             self,
             payload: Payload,
-            publisher: Optional[Publisher] = None,
-            sending_done: Optional[asyncio.Event] = None) -> Union[BackpressureApi, Publisher]:
-        """
-        Initiate a request-channel interaction.
-        """
-
+            local_publisher: Optional[Publisher] = None) -> Union[BackpressureApi, Publisher]:
         logger().debug('%s: request-channel: %s', self._log_identifier(), payload)
 
-        requester = RequestChannelRequester(self, payload, publisher, sending_done)
+        requester = RequestChannelRequester(self, payload, local_publisher)
         return self.register_new_stream(requester)
 
     def metadata_push(self, metadata: bytes) -> Awaitable[None]:
-        """
-        Initiate a metadata-push interaction.
-        """
-
         logger().debug('%s: metadata-push: %s', self._log_identifier(), metadata)
 
         frame = to_metadata_push_frame(metadata)
         self.send_frame(frame)
         return frame.sent_future
 
     def _is_frame_allowed_to_send(self, frame: Frame) -> bool:
```

### Comparing `rsocket-0.4.9/rsocket/rsocket_client.py` & `rsocket-0.4.dev1/rsocket/rsocket_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,23 @@
 from rsocket.request_handler import BaseRequestHandler
 from rsocket.request_handler import RequestHandler
 from rsocket.rsocket_base import RSocketBase
 from rsocket.transports.transport import Transport
 
 
 class RSocketClient(RSocketBase):
-    """
-    Server side instance of an rsocket connection.
-    """
 
     def __init__(self,
                  transport_provider: AsyncGenerator[Transport, Any],
                  handler_factory: Callable[[RSocketBase], RequestHandler] = BaseRequestHandler,
                  honor_lease=False,
                  lease_publisher: Optional[Publisher] = None,
                  request_queue_size: int = 0,
-                 data_encoding: Union[str, bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
-                 metadata_encoding: Union[str, bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
+                 data_encoding: Union[bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
+                 metadata_encoding: Union[bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
                  keep_alive_period: timedelta = timedelta(milliseconds=500),
                  max_lifetime_period: timedelta = timedelta(minutes=10),
                  setup_payload: Optional[Payload] = None,
                  fragment_size_bytes: Optional[int] = None
                  ):
         self._transport_provider = transport_provider.__aiter__()
         self._is_server_alive = True
@@ -65,29 +62,21 @@
         logger().debug('%s: connecting', self._log_identifier())
         self._is_closing = False
         self._reset_internals()
         self._start_tasks()
 
         try:
             await self._connect_new_transport()
-        except RSocketNoAvailableTransport:
-            logger().error('%s: No available transport', self._log_identifier(), exc_info=True)
-            return
         except Exception as exception:
             logger().error('%s: Connection error', self._log_identifier(), exc_info=True)
-            await self._on_connection_error(exception)
+            await self._on_connection_lost(exception)
             return
 
         return await super().connect()
 
-    async def _stop_tasks(self):
-        await super()._stop_tasks()
-        await cancel_if_task_exists(self._keepalive_task)
-        self._keepalive_task = None
-
     async def _connect_new_transport(self):
         try:
             new_transport = await self._get_new_transport()
 
             if new_transport is None:
                 raise RSocketNoAvailableTransport()
 
@@ -103,15 +92,14 @@
         except StopAsyncIteration:
             return
 
     async def close(self):
         await self._close()
 
     async def _close(self, reconnect=False):
-
         if not reconnect:
             await cancel_if_task_exists(self._reconnect_task)
         else:
             logger().debug('%s: Closing before reconnect', self._log_identifier())
 
         await super().close()
 
@@ -119,36 +107,31 @@
         await self.connect()
         return self
 
     def _get_first_stream_id(self) -> int:
         return 1
 
     async def reconnect(self):
-        logger().info('%s: Reconnecting', self._log_identifier())
-
         self._connect_request_event.set()
 
     async def _reconnect_listener(self):
         try:
             while True:
-                try:
-                    await self._connect_request_event.wait()
+                await self._connect_request_event.wait()
 
-                    logger().debug('%s: Got reconnect request', self._log_identifier())
+                logger().debug('%s: Got reconnect request', self._log_identifier())
 
-                    if self._connecting:
-                        continue
+                if self._connecting:
+                    continue
 
-                    self._connecting = True
-                    self._connect_request_event.clear()
-                    await self._close(reconnect=True)
-                    self._next_transport = create_future()
-                    await self.connect()
-                finally:
-                    self._connect_request_event.clear()
+                self._connecting = True
+                self._connect_request_event.clear()
+                await self._close(reconnect=True)
+                self._next_transport = create_future()
+                await self.connect()
         except CancelledError:
             logger().debug('%s: Asyncio task canceled: reconnect_listener', self._log_identifier())
         except Exception:
             logger().error('%s: Reconnect listener', self._log_identifier(), exc_info=True)
         finally:
             self.stop_all_streams()
```

### Comparing `rsocket-0.4.9/rsocket/rsocket_server.py` & `rsocket-0.4.dev1/rsocket/rsocket_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 from datetime import timedelta
 from typing import Optional, Union, Callable
 
 from reactivestreams.publisher import Publisher
 from rsocket.extensions.mimetypes import WellKnownMimeTypes
-from rsocket.helpers import create_future, noop
+from rsocket.helpers import create_future
 from rsocket.local_typing import Awaitable
 from rsocket.payload import Payload
 from rsocket.request_handler import RequestHandler, BaseRequestHandler
 from rsocket.rsocket_base import RSocketBase
 from rsocket.transports.transport import Transport
 
 
 class RSocketServer(RSocketBase):
-    """
-    Server side instance of an rsocket connection.
-    """
 
     def __init__(self,
                  transport: Transport,
-                 handler_factory: Callable[[], RequestHandler] = BaseRequestHandler,
+                 handler_factory: Callable[[RSocketBase], RequestHandler] = BaseRequestHandler,
                  honor_lease=False,
                  lease_publisher: Optional[Publisher] = None,
                  request_queue_size: int = 0,
                  data_encoding: Union[str, bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
                  metadata_encoding: Union[str, bytes, WellKnownMimeTypes] = WellKnownMimeTypes.APPLICATION_JSON,
                  keep_alive_period: timedelta = timedelta(milliseconds=500),
                  max_lifetime_period: timedelta = timedelta(minutes=10),
                  setup_payload: Optional[Payload] = None,
-                 fragment_size_bytes: Optional[int] = None,
-                 on_ready: Optional[Callable[[RSocketBase], None]] = None
+                 fragment_size_bytes: Optional[int] = None
                  ):
-        self._on_ready = on_ready or noop
-        self._transport = transport
-
         super().__init__(handler_factory,
                          honor_lease,
                          lease_publisher,
                          request_queue_size,
                          data_encoding,
                          metadata_encoding,
                          keep_alive_period,
                          max_lifetime_period,
                          setup_payload,
                          fragment_size_bytes=fragment_size_bytes)
+        self._transport = transport
 
     def _current_transport(self) -> Awaitable[Transport]:
         return create_future(self._transport)
 
     def _setup_internals(self):
         self._reset_internals()
         self._start_tasks()
-        self._on_ready(self)
 
     def _log_identifier(self) -> str:
         return 'server'
 
     def _get_first_stream_id(self) -> int:
         return 2
```

### Comparing `rsocket-0.4.9/rsocket/streams/stream_from_async_generator.py` & `rsocket-0.4.dev1/rsocket/streams/stream_from_async_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-import asyncio
-from datetime import timedelta
-from typing import AsyncGenerator, Tuple, Callable
+from typing import AsyncGenerator, Tuple
 
-from rsocket.async_helpers import async_range
 from rsocket.payload import Payload
 from rsocket.streams.exceptions import FinishedIterator
 from rsocket.streams.stream_from_generator import StreamFromGenerator
 
 
 class StreamFromAsyncGenerator(StreamFromGenerator):
-
-    def __init__(self,
-                 generator: Callable[[], AsyncGenerator[Tuple[Payload, bool], None]],
-                 delay_between_messages=timedelta(0),
-                 on_cancel=None,
-                 on_complete=None):
-        super().__init__(generator, delay_between_messages, on_cancel, on_complete)
-
     async def _start_generator(self):
-        self._generator: AsyncGenerator = self._generator_factory()
-        self._iteration = self._generator.__aiter__()
+        self._iteration = self._generator().__aiter__()
 
     async def _generate_next_n(self, n: int) -> AsyncGenerator[Tuple[Payload, bool], None]:
         is_complete_sent = False
-        async for i in async_range(n):
+        for i in range(n):
             try:
                 next_value = await self._iteration.__anext__()
                 is_complete_sent = next_value[1]
                 yield next_value
             except StopAsyncIteration:
                 if not is_complete_sent:
                     raise FinishedIterator()
                 return
-
-    def _cancel_generator(self):
-        asyncio.create_task(self._generator.aclose())
```

### Comparing `rsocket-0.4.9/rsocket/streams/stream_from_generator.py` & `rsocket-0.4.dev1/rsocket/streams/stream_from_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,48 @@
+import abc
 import asyncio
 from datetime import timedelta
-from typing import AsyncGenerator, Tuple, Optional, Callable, Generator
+from typing import AsyncGenerator, Tuple, Optional
 
 from reactivestreams.subscriber import Subscriber
-from rsocket.async_helpers import async_range
-from rsocket.disposable import Disposable
 from rsocket.helpers import DefaultPublisherSubscription
 from rsocket.logger import logger
 from rsocket.payload import Payload
 
 __all__ = ['StreamFromGenerator']
 
 from rsocket.streams.exceptions import FinishedIterator
 
 _finished_iterator = object()
 
 
-class StreamFromGenerator(DefaultPublisherSubscription, Disposable):
+class StreamFromGenerator(DefaultPublisherSubscription, metaclass=abc.ABCMeta):
 
     def __init__(self,
-                 generator: Callable[[], Generator[Tuple[Payload, bool], None, None]],
+                 generator,
                  delay_between_messages=timedelta(0),
                  on_cancel=None,
                  on_complete=None):
-        self._generator_factory = generator
+        self._generator = generator
         self._queue = asyncio.Queue()
         self._delay_between_messages = delay_between_messages
         self._subscriber: Optional[Subscriber] = None
         self._payload_feeder = None
         self._iteration = None
         self._request_n_queue = asyncio.Queue()
         self._n_feeder = None
         self._on_complete = on_complete
         self._on_cancel = on_cancel
 
     async def _start_generator(self):
-        self._generator = self._generator_factory()
-        self._iteration = iter(self._generator)
-
-    def dispose(self):
-        self._generator.close()
+        self._iteration = iter(self._generator())
 
     def subscribe(self, subscriber: Subscriber):
         super().subscribe(subscriber)
-
-        if self._payload_feeder is None:
-            self._payload_feeder = asyncio.create_task(self.feed_subscriber())
+        self._payload_feeder = asyncio.create_task(self.feed_subscriber())
 
     def request(self, n: int):
         if self._n_feeder is None:
             self._n_feeder = asyncio.create_task(self.queue_next_n())
 
         self._request_n_queue.put_nowait(n)
 
@@ -57,62 +50,54 @@
         try:
             await self._start_generator()
 
             while True:
                 n = await self._request_n_queue.get()
 
                 async for payload, is_complete in self._generate_next_n(n):
-                    self._queue.put_nowait((payload, is_complete))
-                    if is_complete:
-                        return
-
+                    await self._queue.put((payload, is_complete))
         except FinishedIterator:
             self._queue.put_nowait((Payload(), True))
         except asyncio.CancelledError:
             logger().debug('Asyncio task canceled: queue_next_n')
         except Exception as exception:
-            logger().error('Stream error', exc_info=True)
             self._subscriber.on_error(exception)
             self._cancel_feeders()
 
     async def _generate_next_n(self, n: int) -> AsyncGenerator[Tuple[Payload, bool], None]:
         is_complete_sent = False
-        async for i in async_range(n):
+        for i in range(n):
             next_value = next(self._iteration, _finished_iterator)
 
             if next_value is _finished_iterator:
                 if not is_complete_sent:
                     raise FinishedIterator()
                 return
 
             is_complete_sent = next_value[1]
             yield next_value
 
     def cancel(self):
         self._cancel_feeders()
 
-        if self._generator is not None:
-            self._cancel_generator()
-
         if self._on_cancel is not None:
             self._on_cancel()
 
     def _cancel_feeders(self):
         self._cancel_payload_feeder()
+
         self._cancel_n_feeder()
 
     def _cancel_payload_feeder(self):
         if self._payload_feeder is not None:
             self._payload_feeder.cancel()
-            self._payload_feeder = None
 
     def _cancel_n_feeder(self):
         if self._n_feeder is not None:
             self._n_feeder.cancel()
-            self._n_feeder = None
 
     async def feed_subscriber(self):
 
         try:
             while True:
                 payload, is_complete = await self._queue.get()
 
@@ -132,10 +117,7 @@
             self._cancel_n_feeder()
 
     def _send_to_subscriber(self, payload: Optional[Payload], is_complete=False):
         if payload is None and is_complete:
             self._subscriber.on_complete()
         else:
             self._subscriber.on_next(payload, is_complete)
-
-    def _cancel_generator(self):
-        self._generator.close()
```

### Comparing `rsocket-0.4.9/rsocket/streams/stream_handler.py` & `rsocket-0.4.dev1/rsocket/streams/stream_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from abc import abstractmethod, ABCMeta
 from typing import Optional, Union
 
 from rsocket.exceptions import RSocketValueError
 from rsocket.frame import Frame, MAX_REQUEST_N
 from rsocket.frame_builders import to_cancel_frame, to_request_n_frame
+from rsocket.logger import logger
 from rsocket.rsocket import RSocket
 from rsocket.rsocket_internal import RSocketInternal
 from rsocket.streams.backpressureapi import BackpressureApi
 
 
 class StreamHandler(BackpressureApi, metaclass=ABCMeta):
-    def __init__(self, socket: Union[RSocket, RSocketInternal]):
+    def __init__(self, socket):
         super().__init__()
         self.stream_id: Optional[int] = None
-        self.socket = socket
+        self.socket: Union[RSocket, RSocketInternal] = socket
         self._initial_request_n = MAX_REQUEST_N
 
     @abstractmethod
     def setup(self):
         ...
 
     def initial_request_n(self, n: int):
@@ -33,15 +34,19 @@
 
     @abstractmethod
     def frame_received(self, frame: Frame):
         ...
 
     def send_cancel(self):
         """Convenience method for use by requester subclasses."""
+        logger().debug('Sending cancel')
 
         self.socket.send_frame(to_cancel_frame(self.stream_id))
+        self._finish_stream()
 
     def send_request_n(self, n: int):
+        logger().debug('Sending request N: %d', n)
+
         self.socket.send_frame(to_request_n_frame(self.stream_id, n))
 
     def _finish_stream(self):
         self.socket.finish_stream(self.stream_id)
```

### Comparing `rsocket-0.4.9/rsocket/transports/abstract_messaging.py` & `rsocket-0.4.dev1/rsocket/transports/abstract_messaging.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket/transports/aioquic_transport.py` & `rsocket-0.4.dev1/rsocket/transports/aioquic_transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from contextlib import asynccontextmanager
 
 from aioquic.asyncio import QuicConnectionProtocol, connect, serve
 from aioquic.quic.configuration import QuicConfiguration
 from aioquic.quic.events import QuicEvent, StreamDataReceived, ConnectionTerminated
 
 from rsocket.exceptions import RSocketTransportError
-from rsocket.frame import Frame, serialize_with_frame_size_header
+from rsocket.frame import Frame
 from rsocket.helpers import wrap_transport_exception, cancel_if_task_exists
 from rsocket.logger import logger
 from rsocket.rsocket_server import RSocketServer
 from rsocket.transports.abstract_messaging import AbstractMessagingTransport
 from rsocket.transports.transport import Transport
 
 
@@ -59,15 +59,15 @@
 class RSocketQuicProtocol(QuicConnectionProtocol):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.frame_queue = asyncio.Queue()
         self._stream_id = self._quic.get_next_available_stream_id()
 
     async def query(self, frame: Frame) -> None:
-        data = serialize_with_frame_size_header(frame)
+        data = frame.serialize()
         self._quic.send_stream_data(self._stream_id, data, end_stream=False)
         self.transmit()
 
     def quic_event_received(self, event: QuicEvent) -> None:
         logger().debug('Quic event received: %s', event)
 
         if isinstance(event, ConnectionTerminated):
@@ -76,51 +76,43 @@
         elif isinstance(event, StreamDataReceived):
             self.frame_queue.put_nowait(event.data)
 
         super().quic_event_received(event)
 
 
 class RSocketQuicTransport(AbstractMessagingTransport):
-    """
-    RSocket transport over server/client side quic connection.
-    """
-
     def __init__(self, quic_protocol: RSocketQuicProtocol):
         super().__init__()
         self._quic_protocol = quic_protocol
         self._incoming_bytes_queue = quic_protocol.frame_queue
         self._listener = asyncio.create_task(self.incoming_data_listener())
 
     async def send_frame(self, frame: Frame):
         await self._quic_protocol.wait_connected()
 
         with wrap_transport_exception():
             await self._quic_protocol.query(frame)
-            await asyncio.sleep(0)
 
     async def incoming_data_listener(self):
         try:
             await self._quic_protocol.wait_connected()
 
             while True:
                 data = await self._incoming_bytes_queue.get()
 
                 if isinstance(data, Exception):
                     self._incoming_frame_queue.put_nowait(data)
                     return
                 else:
-                    async for frame in self._frame_parser.receive_data(data):
+                    async for frame in self._frame_parser.receive_data(data, 0):
                         self._incoming_frame_queue.put_nowait(frame)
 
         except asyncio.CancelledError:
             logger().debug('Asyncio task canceled: incoming_data_listener')
         except Exception:
             self._incoming_frame_queue.put_nowait(RSocketTransportError())
 
     async def close(self):
         await cancel_if_task_exists(self._listener)
         self._quic_protocol.close()
 
         await self._quic_protocol.wait_closed()
-
-    def requires_length_header(self) -> bool:
-        return True
```

### Comparing `rsocket-0.4.9/rsocket/transports/quart_websocket.py` & `rsocket-0.4.dev1/rsocket/transports/quart_websocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,31 +6,24 @@
 from rsocket.helpers import wrap_transport_exception
 from rsocket.logger import logger
 from rsocket.rsocket_server import RSocketServer
 from rsocket.transports.abstract_messaging import AbstractMessagingTransport
 
 
 async def websocket_handler(on_server_create=None, **kwargs):
-    """
-    Helper method to instantiate an RSocket server using a quart websocket connection.
-    """
-
     transport = TransportQuartWebsocket()
     server = RSocketServer(transport, **kwargs)
 
     if on_server_create is not None:
         on_server_create(server)
 
     await transport.handle_incoming_ws_messages()
 
 
 class TransportQuartWebsocket(AbstractMessagingTransport):
-    """
-    RSocket transport over server side quart websocket.
-    """
 
     async def handle_incoming_ws_messages(self):
         try:
             while True:
                 data = await websocket.receive()
 
                 async for frame in self._frame_parser.receive_data(data, 0):
```

### Comparing `rsocket-0.4.9/rsocket/transports/transport.py` & `rsocket-0.4.dev1/rsocket/transports/transport.py`

 * *Files identical despite different names*

### Comparing `rsocket-0.4.9/rsocket.egg-info/PKG-INFO` & `rsocket-0.4.dev1/rsocket.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: rsocket
-Version: 0.4.9
+Version: 0.4.dev1
 Summary: Python RSocket library
 Home-page: https://github.com/rsocket/rsocket-py
 Author: Gabriel Shaar
 Author-email: workofishi@pm.me
 License: MIT
-Project-URL: Documentation, https://rsocket.io/guides/rsocket-py
-Project-URL: Changelog, https://github.com/rsocket/rsocket-py/blob/master/CHANGELOG.rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
@@ -25,88 +22,80 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rx
 Provides-Extra: reactivex
 Provides-Extra: aiohttp
 Provides-Extra: quart
 Provides-Extra: quic
-Provides-Extra: cli
-Provides-Extra: optimized
 License-File: LICENSE
 
 # RSocket-py
 
 Python implementation of [RSocket](http://rsocket.io)
 
-| NOTE: The python api is not final and may be broken between minor versions<br/>See CHANGELOG for <b>Breaking Changes</b> |
-|--------------------------------------------------------------------------------------------------------------------------------|
-
 # Installation
 
 The latest version from [pypi](https://pypi.org/project/rsocket/) can be installed using:
 
 ```shell
 pip install rsocket
 ```
 
-You may also install using some **extras**:
+or install any of the extras:
+
+* rx (RxPy3)
+* reactivex (RxPy4)
+* aiohttp
+* quart
+* uic
 
-| Extra     | Functionality                       |
-|-----------|-------------------------------------|
-| rx        | ReactiveX (v3) integration          |
-| reactivex | ReactiveX (v4) integration          |
-| aiohttp   | Websocket transport (server/client) |
-| quart     | Websocket transport (server only)   |
-| quic      | QUIC transport                      |
-| cli       | Command line                        |
-| optimized | Frame parse/serialize optimizations |
+Example:
 
 ```shell
-pip install rsocket[reactivex]
+pip install --pre rsocket[reactivex]
 ```
 
 Alternatively, download the source code, build a package:
 
 ```shell
 python3 setup.py bdist_wheel
 ```
 
-Use the resulting package from the **./dist** folder, or install locally:
+and use the resulting package from the **./dist** folder, or install locally:
 
 ```shell
 python3 setup.py install
 ```
 
 # Documentation
 
 [Documentation](https://rsocket.io/guides/rsocket-py) is available on the official rsocket.io site.
 
 # Examples
 
-Examples can be found in the **/examples** folder. It contains various server and client usages. The following is a table
-denoting which client example is constructed to be run against which server example. Some examples
-are in java to show compatibility with a different implementation. To run the java examples first build using <code>mvn
-package</code>.
-
-The **examples/test_examples.py** can be used to execute the relevant example server/client pairs.
-
-client_springboot.py is set up to work against the [Spring RSocket demo](https://github.com/benwilcock/spring-rsocket-demo).
-
-| server (python)                    | server (java)           | client (python)                    | client(java)    |
-|------------------------------------|-------------------------|------------------------------------|-----------------|
-| server.py                          |                         | client.py                          |                 |
-| server_quic.py                     |                         | client_quic.py                     |                 |
-| server_with_lease.py               |                         |                                    | ClientWithLease |
-| server_with_routing.py             |                         | client_with_routing.py             | Client          |
-| server_with_routing.py             |                         | client_rx.py                       |                 |
-| server_with_routing.py             |                         | client_reconnect.py                |                 |
-|                                    | Server                  | run_against_example_java_server.py |                 |
-|                                    | ServerWithFragmentation | client_with_routing.py             |                 |
-| server_quart_websocket.py          |                         | client_websocket.py                |                 |
-| server_aiohttp_websocket.py        |                         | client_websocket.py                |                 |
+Examples can be found in the /examples folder. It contains various server and client usages. The following is a table
+denoting which <b>client</b> example is constructed to be run against which <b>server</b> example. Some of the examples
+are in java to show compatibility with a different implementation.
+
+The **examples/test_examples.py** shows which pairs of client/server work with each other, and can be used to execute
+all the examples
+(except for the client_springboot.py which is set up to work against https://github.com/benwilcock/spring-rsocket-demo)
+
+| server (python)             | server (java)           | client (python)                    | client(java)    |
+|-----------------------------|-------------------------|------------------------------------|-----------------|
+| server.py                   |                         | client.py                          |                 |
+| server_quic.py              |                         | client_quic.py                     |                 |
+| server_with_lease.py        |                         |                                    | ClientWithLease |
+| server_with_routing.py      |                         | client_with_routing.py             | Client          |
+| server_with_routing.py      |                         | client_rx.py                       |                 |
+| server_with_routing.py      |                         | client_reconnect.py                |                 |
+|                             | Server                  | run_against_example_java_server.py |                 |
+|                             | ServerWithFragmentation | client_with_routing.py             |                 |
+| server_quart_websocket.py   |                         | client_websocket.py                |                 |
+| server_aiohttp_websocket.py |                         | client_websocket.py                |                 |
 
 # Build Status
 
 ![build master](https://github.com/rsocket/rsocket-py/actions/workflows/python-package.yml/badge.svg?branch=master)
 [![Coverage Status](https://coveralls.io/repos/github/rsocket/rsocket-py/badge.svg?branch=master)](https://coveralls.io/github/rsocket/rsocket-py?branch=master)
 [![CodeQL](https://github.com/rsocket/rsocket-py/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/rsocket/rsocket-py/actions/workflows/codeql-analysis.yml)
 
@@ -126,23 +115,20 @@
 - [X] Extensions
     - [X] Composite metadata
     - [X] Per Stream Mimetype
     - [X] Routing
     - [X] Authentication
 - [ ] Transports
     - [X] TCP
-    - [X] Websocket (WS, WSS) - Quart and aiohttp integration
+    - [X] Websocket
     - [X] QUIC
-    - [X] HTTP/3
     - [ ] HTTP/2
     - [ ] Aeron
 - [X] RxPy Integration
     - [X] Stream Response
     - [X] Channel Response
     - [X] Channel Requester stream
     - [X] Response
-- [X] Other
+- [ ] Other
+    - [ ] Error handling all scenarios in the protocol spec
     - [X] Reconnect
     - [X] Load balancing
-    - [X] Server routing definition helper (Flask like syntax)
-    - [X] Reactivex integration (v3, v4) server/client side
-    - [X] Command line interface
```

