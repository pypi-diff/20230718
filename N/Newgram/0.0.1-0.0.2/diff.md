# Comparing `tmp/Newgram-0.0.1.tar.gz` & `tmp/Newgram-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Newgram-0.0.1.tar", last modified: Mon Jul 17 15:35:07 2023, max compression
+gzip compressed data, was "Newgram-0.0.2.tar", last modified: Mon Jul 17 22:06:32 2023, max compression
```

## Comparing `Newgram-0.0.1.tar` & `Newgram-0.0.2.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.878416 Newgram-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 15:34:40.000000 Newgram-0.0.1/COPYING
--rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 15:34:40.000000 Newgram-0.0.1/COPYING.lesser
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-17 15:34:40.000000 Newgram-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      769 2023-07-17 15:34:40.000000 Newgram-0.0.1/NOTICE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/Newgram.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4369 2023-07-17 15:35:07.000000 Newgram-0.0.1/Newgram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18386 2023-07-17 15:35:07.000000 Newgram-0.0.1/Newgram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:35:07.000000 Newgram-0.0.1/Newgram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:35:07.000000 Newgram-0.0.1/Newgram.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 15:35:07.000000 Newgram-0.0.1/Newgram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 15:35:07.000000 Newgram-0.0.1/Newgram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4369 2023-07-17 15:35:07.874416 Newgram-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2467 2023-07-17 15:34:40.000000 Newgram-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/api/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22379 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/api/source/
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/source/auth_key.tl
--rw-r--r--   0 root         (0) root         (0)   168867 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/source/main_api.tl
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/api/template/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/template/combinator.txt
--rw-r--r--   0 root         (0) root         (0)      631 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/api/template/type.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/docs/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19205 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/docs/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/docs/template/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/docs/template/page.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.822413 Newgram-0.0.1/compiler/errors/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4910 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/compiler.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.826413 Newgram-0.0.1/compiler/errors/source/
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 root         (0) root         (0)    22642 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 root         (0) root         (0)     2000 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 root         (0) root         (0)     4219 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.826413 Newgram-0.0.1/compiler/errors/template/
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/template/class.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-17 15:34:40.000000 Newgram-0.0.1/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.826413 Newgram-0.0.1/newgram/
--rw-r--r--   0 root         (0) root         (0)     1394 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41945 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.826413 Newgram-0.0.1/newgram/connection/
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.826413 Newgram-0.0.1/newgram/connection/transport/
--rw-r--r--   0 root         (0) root         (0)      833 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.826413 Newgram-0.0.1/newgram/connection/transport/tcp/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4084 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/tcp.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.830413 Newgram-0.0.1/newgram/crypto/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4006 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/crypto/aes.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/crypto/mtproto.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/crypto/prime.py
--rw-r--r--   0 root         (0) root         (0)    13432 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/crypto/rsa.py
--rw-r--r--   0 root         (0) root         (0)    10033 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)   208016 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/emoji.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.830413 Newgram-0.0.1/newgram/enums/
--rw-r--r--   0 root         (0) root         (0)     1731 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/__init__.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/auto_name.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4197 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/chat_event_action.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/chat_member_status.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/chat_members_filter.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/chat_type.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/message_entity_type.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/message_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/message_service_type.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/messages_filter.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/next_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/parse_mode.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/poll_type.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/sent_code_type.py
--rw-r--r--   0 root         (0) root         (0)     1293 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/enums/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.830413 Newgram-0.0.1/newgram/errors/
--rw-r--r--   0 root         (0) root         (0)     2600 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/errors/rpc_error.py
--rw-r--r--   0 root         (0) root         (0)    15148 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/file_id.py
--rw-r--r--   0 root         (0) root         (0)    24798 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.830413 Newgram-0.0.1/newgram/handlers/
--rw-r--r--   0 root         (0) root         (0)     1470 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/callback_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/chat_join_request_handler.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/deleted_messages_handler.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/disconnect_handler.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/edited_message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/handler.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/inline_query_handler.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/message_handler.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/poll_handler.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/handlers/user_status_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.834414 Newgram-0.0.1/newgram/methods/
--rw-r--r--   0 root         (0) root         (0)     1315 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.834414 Newgram-0.0.1/newgram/methods/advanced/
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/advanced/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/advanced/invoke.py
--rw-r--r--   0 root         (0) root         (0)     4549 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/advanced/resolve_peer.py
--rw-r--r--   0 root         (0) root         (0)     8410 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/advanced/save_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.834414 Newgram-0.0.1/newgram/methods/auth/
--rw-r--r--   0 root         (0) root         (0)     1650 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/check_password.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/connect.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/disconnect.py
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/get_password_hint.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/log_out.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/recover_password.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/resend_code.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/send_code.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/send_recovery_code.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/sign_in.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/sign_in_bot.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/sign_up.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/auth/terminate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.838414 Newgram-0.0.1/newgram/methods/bots/
--rw-r--r--   0 root         (0) root         (0)     2036 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3303 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/answer_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     4979 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/answer_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/get_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 root         (0) root         (0)     3354 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 root         (0) root         (0)     2839 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/request_callback_answer.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/send_game.py
--rw-r--r--   0 root         (0) root         (0)     2816 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/set_bot_commands.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 root         (0) root         (0)     3936 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/bots/set_game_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.842414 Newgram-0.0.1/newgram/methods/chats/
--rw-r--r--   0 root         (0) root         (0)     3434 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3356 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/add_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/archive_chats.py
--rw-r--r--   0 root         (0) root         (0)     4610 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/ban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/create_channel.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/create_group.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/create_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/delete_channel.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/delete_supergroup.py
--rw-r--r--   0 root         (0) root         (0)     1961 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/delete_user_history.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_chat.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 root         (0) root         (0)     3327 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     5267 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_chat_members.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 root         (0) root         (0)     1715 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_dialogs.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/join_chat.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/leave_chat.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/pin_chat_message.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/promote_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_administrator_title.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_chat_description.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     1719 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_chat_title.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_chat_username.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/set_slow_mode.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/unarchive_chats.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/unban_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1932 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 root         (0) root         (0)     2131 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.842414 Newgram-0.0.1/newgram/methods/contacts/
--rw-r--r--   0 root         (0) root         (0)     1149 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/contacts/add_contact.py
--rw-r--r--   0 root         (0) root         (0)     2438 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/contacts/delete_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/contacts/get_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.846414 Newgram-0.0.1/newgram/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)     1619 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_disconnect.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_edited_message.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_message.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_poll.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.846414 Newgram-0.0.1/newgram/methods/invite_links/
--rw-r--r--   0 root         (0) root         (0)     2430 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     3358 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2023 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3523 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     3555 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.854415 Newgram-0.0.1/newgram/methods/messages/
--rw-r--r--   0 root         (0) root         (0)     3916 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5954 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/copy_media_group.py
--rw-r--r--   0 root         (0) root         (0)     5164 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/copy_message.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/delete_messages.py
--rw-r--r--   0 root         (0) root         (0)     7519 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/download_media.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 root         (0) root         (0)    10360 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_inline_media.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_inline_text.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_message_caption.py
--rw-r--r--   0 root         (0) root         (0)    13007 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_message_media.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/forward_messages.py
--rw-r--r--   0 root         (0) root         (0)     4031 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2380 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_discussion_message.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 root         (0) root         (0)     2937 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_media_group.py
--rw-r--r--   0 root         (0) root         (0)     4729 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/get_messages.py
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/inline_session.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/read_chat_history.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/retract_vote.py
--rw-r--r--   0 root         (0) root         (0)     4144 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/search_global.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/search_global_count.py
--rw-r--r--   0 root         (0) root         (0)     5337 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/search_messages.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/search_messages_count.py
--rw-r--r--   0 root         (0) root         (0)    12563 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_animation.py
--rw-r--r--   0 root         (0) root         (0)    11096 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_audio.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_cached_media.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_chat_action.py
--rw-r--r--   0 root         (0) root         (0)     4853 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_contact.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_dice.py
--rw-r--r--   0 root         (0) root         (0)    10447 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_document.py
--rw-r--r--   0 root         (0) root         (0)     4562 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_location.py
--rw-r--r--   0 root         (0) root         (0)    19889 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_media_group.py
--rw-r--r--   0 root         (0) root         (0)     7245 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_message.py
--rw-r--r--   0 root         (0) root         (0)     9417 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_photo.py
--rw-r--r--   0 root         (0) root         (0)     8051 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_poll.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_reaction.py
--rw-r--r--   0 root         (0) root         (0)     8319 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_sticker.py
--rw-r--r--   0 root         (0) root         (0)     5383 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_venue.py
--rw-r--r--   0 root         (0) root         (0)    11933 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_video.py
--rw-r--r--   0 root         (0) root         (0)     9293 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_video_note.py
--rw-r--r--   0 root         (0) root         (0)     9407 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/send_voice.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/stop_poll.py
--rw-r--r--   0 root         (0) root         (0)     3927 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/stream_media.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/messages/vote_poll.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.854415 Newgram-0.0.1/newgram/methods/password/
--rw-r--r--   0 root         (0) root         (0)     1083 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/password/change_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/password/enable_cloud_password.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.854415 Newgram-0.0.1/newgram/methods/users/
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/block_user.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/delete_profile_photos.py
--rw-r--r--   0 root         (0) root         (0)     4412 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/get_chat_photos.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 root         (0) root         (0)     2349 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/get_common_chats.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/get_me.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/get_users.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/set_emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/set_profile_photo.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/set_username.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/unblock_user.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/users/update_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.854415 Newgram-0.0.1/newgram/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)     1248 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/add_handler.py
--rw-r--r--   0 root         (0) root         (0)     2221 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/export_session_string.py
--rw-r--r--   0 root         (0) root         (0)     2743 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/remove_handler.py
--rw-r--r--   0 root         (0) root         (0)     2283 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/restart.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/stop.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/methods/utilities/stop_transmission.py
--rw-r--r--   0 root         (0) root         (0)    61910 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/mime_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/parser/
--rw-r--r--   0 root         (0) root         (0)      841 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/parser/html.py
--rw-r--r--   0 root         (0) root         (0)     5762 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/parser/markdown.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/parser/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/raw/
--rw-r--r--   0 root         (0) root         (0)     1035 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/raw/core/
--rw-r--r--   0 root         (0) root         (0)     1307 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/future_salt.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/future_salts.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/gzip_packed.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/list.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/message.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/msg_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/raw/core/primitives/
--rw-r--r--   0 root         (0) root         (0)     1007 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/bool.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/bytes.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/double.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/int.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/string.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/primitives/vector.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/raw/core/tl_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/session/
--rw-r--r--   0 root         (0) root         (0)      866 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11434 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/session/internals/
--rw-r--r--   0 root         (0) root         (0)      912 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/internals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/internals/data_center.py
--rw-r--r--   0 root         (0) root         (0)     1366 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/internals/msg_factory.py
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/internals/msg_id.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/internals/seq_no.py
--rw-r--r--   0 root         (0) root         (0)    13404 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/session/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/storage/
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/storage/file_storage.py
--rw-r--r--   0 root         (0) root         (0)     2745 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/storage/memory_storage.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/storage/storage.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.858415 Newgram-0.0.1/newgram/types/
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.862415 Newgram-0.0.1/newgram/types/authorization/
--rw-r--r--   0 root         (0) root         (0)      933 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/authorization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/authorization/sent_code.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.862415 Newgram-0.0.1/newgram/types/bots_and_keyboards/
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1250 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 root         (0) root         (0)    12768 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 root         (0) root         (0)     2206 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 root         (0) root         (0)     8107 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 root         (0) root         (0)     1201 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 root         (0) root         (0)     1204 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 root         (0) root         (0)     4565 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 root         (0) root         (0)     2331 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.866415 Newgram-0.0.1/newgram/types/inline_mode/
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3651 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 root         (0) root         (0)     7283 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query.py
--rw-r--r--   0 root         (0) root         (0)     2386 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     4493 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 root         (0) root         (0)     4017 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 root         (0) root         (0)     4382 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 root         (0) root         (0)     4190 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 root         (0) root         (0)     4122 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 root         (0) root         (0)     5228 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     4609 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 root         (0) root         (0)     5249 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.866415 Newgram-0.0.1/newgram/types/input_media/
--rw-r--r--   0 root         (0) root         (0)     1309 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_media.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_media_animation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_media_audio.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_media_document.py
--rw-r--r--   0 root         (0) root         (0)     2677 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_media_photo.py
--rw-r--r--   0 root         (0) root         (0)     3612 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_media_video.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.866415 Newgram-0.0.1/newgram/types/input_message_content/
--rw-r--r--   0 root         (0) root         (0)     1001 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_message_content/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_message_content/input_message_content.py
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.870416 Newgram-0.0.1/newgram/types/messages_and_media/
--rw-r--r--   0 root         (0) root         (0)     1831 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4033 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/animation.py
--rw-r--r--   0 root         (0) root         (0)     4058 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/audio.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/contact.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/dice.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/document.py
--rw-r--r--   0 root         (0) root         (0)     3033 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/game.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/location.py
--rw-r--r--   0 root         (0) root         (0)   144298 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/message.py
--rw-r--r--   0 root         (0) root         (0)     4337 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/message_entity.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 root         (0) root         (0)     4298 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/photo.py
--rw-r--r--   0 root         (0) root         (0)     7025 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/poll.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/poll_option.py
--rw-r--r--   0 root         (0) root         (0)     2607 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/reaction.py
--rw-r--r--   0 root         (0) root         (0)     6897 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/sticker.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     3746 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/venue.py
--rw-r--r--   0 root         (0) root         (0)     4378 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/video.py
--rw-r--r--   0 root         (0) root         (0)     3590 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/video_note.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/voice.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/messages_and_media/web_page.py
--rw-r--r--   0 root         (0) root         (0)     3850 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/object.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.874416 Newgram-0.0.1/newgram/types/user_and_chats/
--rw-r--r--   0 root         (0) root         (0)     2292 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32499 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 root         (0) root         (0)    19788 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_event.py
--rw-r--r--   0 root         (0) root         (0)     5508 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 root         (0) root         (0)     2553 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 root         (0) root         (0)     9427 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_member.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 root         (0) root         (0)     2671 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/dialog.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/restriction.py
--rw-r--r--   0 root         (0) root         (0)    12815 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/user.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-17 15:34:40.000000 Newgram-0.0.1/newgram/utils.py
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 15:34:40.000000 Newgram-0.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 15:35:07.878416 Newgram-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3502 2023-07-17 15:34:40.000000 Newgram-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.874416 Newgram-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.874416 Newgram-0.0.1/tests/filters/
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-17 15:34:40.000000 Newgram-0.0.1/tests/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-07-17 15:34:40.000000 Newgram-0.0.1/tests/filters/test_command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:35:07.874416 Newgram-0.0.1/tests/parser/
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 15:34:40.000000 Newgram-0.0.1/tests/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6200 2023-07-17 15:34:40.000000 Newgram-0.0.1/tests/parser/test_html.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-07-17 15:34:40.000000 Newgram-0.0.1/tests/test_file_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.825854 Newgram-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    35148 2023-07-17 22:04:52.000000 Newgram-0.0.2/COPYING
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-07-17 22:04:52.000000 Newgram-0.0.2/COPYING.lesser
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-17 22:04:52.000000 Newgram-0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-17 22:04:52.000000 Newgram-0.0.2/NOTICE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/Newgram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-07-17 22:06:32.000000 Newgram-0.0.2/Newgram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18386 2023-07-17 22:06:32.000000 Newgram-0.0.2/Newgram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 22:06:32.000000 Newgram-0.0.2/Newgram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 22:06:32.000000 Newgram-0.0.2/Newgram.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 22:06:32.000000 Newgram-0.0.2/Newgram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 22:06:32.000000 Newgram-0.0.2/Newgram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-07-17 22:06:32.825854 Newgram-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-07-17 22:04:52.000000 Newgram-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/api/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22379 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/api/source/
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/source/auth_key.tl
+-rw-r--r--   0 root         (0) root         (0)   168867 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/source/main_api.tl
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/api/template/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/template/combinator.txt
+-rw-r--r--   0 root         (0) root         (0)      631 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/api/template/type.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/docs/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19205 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/docs/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/docs/template/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/docs/template/page.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/errors/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/errors/source/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 root         (0) root         (0)    22642 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.777852 Newgram-0.0.2/compiler/errors/template/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/template/class.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-17 22:04:52.000000 Newgram-0.0.2/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.781852 Newgram-0.0.2/newgram/
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41945 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.781852 Newgram-0.0.2/newgram/connection/
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.781852 Newgram-0.0.2/newgram/connection/transport/
+-rw-r--r--   0 root         (0) root         (0)      833 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.781852 Newgram-0.0.2/newgram/connection/transport/tcp/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4084 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.781852 Newgram-0.0.2/newgram/crypto/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/crypto/aes.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/crypto/mtproto.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/crypto/prime.py
+-rw-r--r--   0 root         (0) root         (0)    13432 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/crypto/rsa.py
+-rw-r--r--   0 root         (0) root         (0)    10033 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)   208016 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/emoji.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.781852 Newgram-0.0.2/newgram/enums/
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/auto_name.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/chat_event_action.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/chat_member_status.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/chat_members_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/chat_type.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/message_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/message_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/message_service_type.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/messages_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/next_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/parse_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/poll_type.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/sent_code_type.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/enums/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.785852 Newgram-0.0.2/newgram/errors/
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/errors/rpc_error.py
+-rw-r--r--   0 root         (0) root         (0)    15148 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/file_id.py
+-rw-r--r--   0 root         (0) root         (0)    24798 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.785852 Newgram-0.0.2/newgram/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/callback_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/disconnect_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/edited_message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/inline_query_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/message_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/poll_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/handlers/user_status_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.785852 Newgram-0.0.2/newgram/methods/
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.785852 Newgram-0.0.2/newgram/methods/advanced/
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/advanced/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/advanced/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     4549 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 root         (0) root         (0)     8410 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/advanced/save_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.785852 Newgram-0.0.2/newgram/methods/auth/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/check_password.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/get_password_hint.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/log_out.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/recover_password.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/resend_code.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/send_code.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/sign_in.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/sign_up.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/auth/terminate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.789852 Newgram-0.0.2/newgram/methods/bots/
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     4979 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 root         (0) root         (0)     3354 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/send_game.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/bots/set_game_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.793853 Newgram-0.0.2/newgram/methods/chats/
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/add_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/archive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     4610 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/create_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/create_group.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/create_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/delete_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/delete_user_history.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_chat.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_chat_members.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_dialogs.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/join_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/leave_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_chat_description.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_chat_title.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_chat_username.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2131 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.793853 Newgram-0.0.2/newgram/methods/contacts/
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/contacts/add_contact.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/contacts/get_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.797853 Newgram-0.0.2/newgram/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_message.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_poll.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.797853 Newgram-0.0.2/newgram/methods/invite_links/
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.801853 Newgram-0.0.2/newgram/methods/messages/
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/copy_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     5164 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/copy_message.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/delete_messages.py
+-rw-r--r--   0 root         (0) root         (0)     7519 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/download_media.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 root         (0) root         (0)    10360 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 root         (0) root         (0)    13007 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_message_media.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/forward_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     4729 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/get_messages.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/inline_session.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/read_chat_history.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/retract_vote.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/search_global.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/search_global_count.py
+-rw-r--r--   0 root         (0) root         (0)     5337 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/search_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/search_messages_count.py
+-rw-r--r--   0 root         (0) root         (0)    12563 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_animation.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_audio.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_cached_media.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_chat_action.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_dice.py
+-rw-r--r--   0 root         (0) root         (0)    10447 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_document.py
+-rw-r--r--   0 root         (0) root         (0)     4562 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_location.py
+-rw-r--r--   0 root         (0) root         (0)    19889 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_media_group.py
+-rw-r--r--   0 root         (0) root         (0)     7245 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_message.py
+-rw-r--r--   0 root         (0) root         (0)     9417 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_photo.py
+-rw-r--r--   0 root         (0) root         (0)     8051 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_poll.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     8319 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     5383 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_venue.py
+-rw-r--r--   0 root         (0) root         (0)    11933 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_video.py
+-rw-r--r--   0 root         (0) root         (0)     9293 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_video_note.py
+-rw-r--r--   0 root         (0) root         (0)     9407 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/send_voice.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/stop_poll.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/stream_media.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/messages/vote_poll.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.805853 Newgram-0.0.2/newgram/methods/password/
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/password/change_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.805853 Newgram-0.0.2/newgram/methods/users/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/block_user.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 root         (0) root         (0)     4412 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/get_chat_photos.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/get_common_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/get_me.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/get_users.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/set_emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/set_profile_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/set_username.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/unblock_user.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/users/update_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.805853 Newgram-0.0.2/newgram/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/add_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/export_session_string.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/remove_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/restart.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/stop.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 root         (0) root         (0)    61910 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/mime_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.805853 Newgram-0.0.2/newgram/parser/
+-rw-r--r--   0 root         (0) root         (0)      841 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/parser/html.py
+-rw-r--r--   0 root         (0) root         (0)     5762 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/parser/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.805853 Newgram-0.0.2/newgram/raw/
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/raw/core/
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/future_salt.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/future_salts.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/gzip_packed.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/list.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/msg_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/raw/core/primitives/
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/bool.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/bytes.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/double.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/int.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/string.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/primitives/vector.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/raw/core/tl_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/session/
+-rw-r--r--   0 root         (0) root         (0)      866 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11434 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/session/internals/
+-rw-r--r--   0 root         (0) root         (0)      912 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/internals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/internals/data_center.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/internals/msg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/internals/msg_id.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/internals/seq_no.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/session/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/storage/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/storage/file_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/storage/memory_storage.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/storage/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/types/
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.809853 Newgram-0.0.2/newgram/types/authorization/
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/authorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/authorization/sent_code.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.813854 Newgram-0.0.2/newgram/types/bots_and_keyboards/
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 root         (0) root         (0)    12768 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 root         (0) root         (0)     8107 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.817854 Newgram-0.0.2/newgram/types/inline_mode/
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     4493 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.817854 Newgram-0.0.2/newgram/types/input_media/
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_media.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_media_animation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_media_audio.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_media_document.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_media_photo.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_media_video.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.817854 Newgram-0.0.2/newgram/types/input_message_content/
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_message_content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.821854 Newgram-0.0.2/newgram/types/messages_and_media/
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4033 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/animation.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/audio.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/dice.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/document.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/game.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/location.py
+-rw-r--r--   0 root         (0) root         (0)   144298 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/message.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/photo.py
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/reaction.py
+-rw-r--r--   0 root         (0) root         (0)     6897 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/venue.py
+-rw-r--r--   0 root         (0) root         (0)     4378 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/video.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/video_note.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/messages_and_media/web_page.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/object.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.821854 Newgram-0.0.2/newgram/types/user_and_chats/
+-rw-r--r--   0 root         (0) root         (0)     2292 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32499 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 root         (0) root         (0)    19788 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 root         (0) root         (0)     9427 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/dialog.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/restriction.py
+-rw-r--r--   0 root         (0) root         (0)    12815 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/user.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-17 22:04:52.000000 Newgram-0.0.2/newgram/utils.py
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-17 22:04:52.000000 Newgram-0.0.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 22:06:32.825854 Newgram-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-07-17 22:06:29.000000 Newgram-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.821854 Newgram-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.821854 Newgram-0.0.2/tests/filters/
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-17 22:04:52.000000 Newgram-0.0.2/tests/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-07-17 22:04:52.000000 Newgram-0.0.2/tests/filters/test_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:06:32.821854 Newgram-0.0.2/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-17 22:04:52.000000 Newgram-0.0.2/tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-07-17 22:04:52.000000 Newgram-0.0.2/tests/parser/test_html.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-07-17 22:04:52.000000 Newgram-0.0.2/tests/test_file_id.py
```

### Comparing `Newgram-0.0.1/COPYING` & `Newgram-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/COPYING.lesser` & `Newgram-0.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/NOTICE` & `Newgram-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/Newgram.egg-info/PKG-INFO` & `Newgram-0.0.2/Newgram.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 Metadata-Version: 2.1
 Name: Newgram
-Version: 0.0.1
+Version: 0.0.2
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/jokokendi
 Author: Noel
 Author-email: noel@newgram.org
 License: LGPLv3
 Download-URL: https://github.com/jokokendi/newgram/releases/latest
 Project-URL: Tracker, https://github.com/jokokendi/newgram/issues
 Project-URL: Community, https://t.me/newgram
 Project-URL: Source, https://github.com/jokokendi/newgram
 Project-URL: Documentation, https://docs.newgram.org
 Keywords: telegram chat messenger mtproto api client library python
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet
-Classifier: Topic :: Communications
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1 Name: Newgram Version: 0.0.1 Summary: Elegant, modern and
+Metadata-Version: 2.1 Name: Newgram Version: 0.0.2 Summary: Elegant, modern and
 asynchronous Telegram MTProto API framework in Python for users and bots Home-
 page: https://github.com/jokokendi Author: Noel Author-email: noel@newgram.org
 License: LGPLv3 Download-URL: https://github.com/jokokendi/newgram/releases/
 latest Project-URL: Tracker, https://github.com/jokokendi/newgram/issues
 Project-URL: Community, https://t.me/newgram Project-URL: Source, https://
 github.com/jokokendi/newgram Project-URL: Documentation, https://
 docs.newgram.org Keywords: telegram chat messenger mtproto api client library
-python Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
-:: English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
-Implementation Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
-Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
-License-File: COPYING License-File: COPYING.lesser License-File: NOTICE
+python Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent Requires-Python: ~=3.7
+Description-Content-Type: text/markdown License-File: COPYING License-File:
+COPYING.lesser License-File: NOTICE
                                   [Pyrogram]
                   Telegram MTProto API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Newgram > Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots ``` python from newgram import Client, filters app =
 Client("my_account") @app.on_message(filters.private) async def hello(client,
 message): await message.reply("Hello from Newgram!") app.run() ``` **Newgram**
```

### Comparing `Newgram-0.0.1/Newgram.egg-info/SOURCES.txt` & `Newgram-0.0.2/Newgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/PKG-INFO` & `Newgram-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 Metadata-Version: 2.1
 Name: Newgram
-Version: 0.0.1
+Version: 0.0.2
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/jokokendi
 Author: Noel
 Author-email: noel@newgram.org
 License: LGPLv3
 Download-URL: https://github.com/jokokendi/newgram/releases/latest
 Project-URL: Tracker, https://github.com/jokokendi/newgram/issues
 Project-URL: Community, https://t.me/newgram
 Project-URL: Source, https://github.com/jokokendi/newgram
 Project-URL: Documentation, https://docs.newgram.org
 Keywords: telegram chat messenger mtproto api client library python
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet
-Classifier: Topic :: Communications
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1 Name: Newgram Version: 0.0.1 Summary: Elegant, modern and
+Metadata-Version: 2.1 Name: Newgram Version: 0.0.2 Summary: Elegant, modern and
 asynchronous Telegram MTProto API framework in Python for users and bots Home-
 page: https://github.com/jokokendi Author: Noel Author-email: noel@newgram.org
 License: LGPLv3 Download-URL: https://github.com/jokokendi/newgram/releases/
 latest Project-URL: Tracker, https://github.com/jokokendi/newgram/issues
 Project-URL: Community, https://t.me/newgram Project-URL: Source, https://
 github.com/jokokendi/newgram Project-URL: Documentation, https://
 docs.newgram.org Keywords: telegram chat messenger mtproto api client library
-python Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
-:: English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
-Implementation Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
-Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
-License-File: COPYING License-File: COPYING.lesser License-File: NOTICE
+python Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent Requires-Python: ~=3.7
+Description-Content-Type: text/markdown License-File: COPYING License-File:
+COPYING.lesser License-File: NOTICE
                                   [Pyrogram]
                   Telegram MTProto API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Newgram > Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots ``` python from newgram import Client, filters app =
 Client("my_account") @app.on_message(filters.private) async def hello(client,
 message): await message.reply("Hello from Newgram!") app.run() ``` **Newgram**
```

### Comparing `Newgram-0.0.1/README.md` & `Newgram-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/__init__.py` & `Newgram-0.0.2/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/__init__.py` & `Newgram-0.0.2/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/compiler.py` & `Newgram-0.0.2/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/source/auth_key.tl` & `Newgram-0.0.2/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/source/main_api.tl` & `Newgram-0.0.2/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/source/sys_msgs.tl` & `Newgram-0.0.2/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/template/combinator.txt` & `Newgram-0.0.2/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/api/template/type.txt` & `Newgram-0.0.2/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/docs/__init__.py` & `Newgram-0.0.2/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/docs/compiler.py` & `Newgram-0.0.2/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/__init__.py` & `Newgram-0.0.2/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/compiler.py` & `Newgram-0.0.2/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/sort.py` & `Newgram-0.0.2/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv` & `Newgram-0.0.2/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv` & `Newgram-0.0.2/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv` & `Newgram-0.0.2/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `Newgram-0.0.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `Newgram-0.0.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/__init__.py` & `Newgram-0.0.2/newgram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Newgram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2023-present Noel <https://github.com/jokokendi>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `Newgram-0.0.1/newgram/client.py` & `Newgram-0.0.2/newgram/client.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/__init__.py` & `Newgram-0.0.2/newgram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/connection.py` & `Newgram-0.0.2/newgram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/__init__.py` & `Newgram-0.0.2/newgram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/__init__.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/tcp.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/tcp_abridged.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/tcp_abridged_o.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/tcp_full.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/tcp_intermediate.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/connection/transport/tcp/tcp_intermediate_o.py` & `Newgram-0.0.2/newgram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/crypto/__init__.py` & `Newgram-0.0.2/newgram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/crypto/aes.py` & `Newgram-0.0.2/newgram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/crypto/mtproto.py` & `Newgram-0.0.2/newgram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/crypto/prime.py` & `Newgram-0.0.2/newgram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/crypto/rsa.py` & `Newgram-0.0.2/newgram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/dispatcher.py` & `Newgram-0.0.2/newgram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/emoji.py` & `Newgram-0.0.2/newgram/emoji.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/__init__.py` & `Newgram-0.0.2/newgram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/auto_name.py` & `Newgram-0.0.2/newgram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/chat_action.py` & `Newgram-0.0.2/newgram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/chat_event_action.py` & `Newgram-0.0.2/newgram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/chat_member_status.py` & `Newgram-0.0.2/newgram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/chat_members_filter.py` & `Newgram-0.0.2/newgram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/chat_type.py` & `Newgram-0.0.2/newgram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/message_entity_type.py` & `Newgram-0.0.2/newgram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/message_media_type.py` & `Newgram-0.0.2/newgram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/message_service_type.py` & `Newgram-0.0.2/newgram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/messages_filter.py` & `Newgram-0.0.2/newgram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/next_code_type.py` & `Newgram-0.0.2/newgram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/parse_mode.py` & `Newgram-0.0.2/newgram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/poll_type.py` & `Newgram-0.0.2/newgram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/sent_code_type.py` & `Newgram-0.0.2/newgram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/enums/user_status.py` & `Newgram-0.0.2/newgram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/errors/__init__.py` & `Newgram-0.0.2/newgram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/errors/rpc_error.py` & `Newgram-0.0.2/newgram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/file_id.py` & `Newgram-0.0.2/newgram/file_id.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/filters.py` & `Newgram-0.0.2/newgram/filters.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/__init__.py` & `Newgram-0.0.2/newgram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/callback_query_handler.py` & `Newgram-0.0.2/newgram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/chat_join_request_handler.py` & `Newgram-0.0.2/newgram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/chat_member_updated_handler.py` & `Newgram-0.0.2/newgram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/chosen_inline_result_handler.py` & `Newgram-0.0.2/newgram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/deleted_messages_handler.py` & `Newgram-0.0.2/newgram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/disconnect_handler.py` & `Newgram-0.0.2/newgram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/edited_message_handler.py` & `Newgram-0.0.2/newgram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/handler.py` & `Newgram-0.0.2/newgram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/inline_query_handler.py` & `Newgram-0.0.2/newgram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/message_handler.py` & `Newgram-0.0.2/newgram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/poll_handler.py` & `Newgram-0.0.2/newgram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/raw_update_handler.py` & `Newgram-0.0.2/newgram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/handlers/user_status_handler.py` & `Newgram-0.0.2/newgram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/__init__.py` & `Newgram-0.0.2/newgram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/advanced/__init__.py` & `Newgram-0.0.2/newgram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/advanced/invoke.py` & `Newgram-0.0.2/newgram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/advanced/resolve_peer.py` & `Newgram-0.0.2/newgram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/advanced/save_file.py` & `Newgram-0.0.2/newgram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/__init__.py` & `Newgram-0.0.2/newgram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/accept_terms_of_service.py` & `Newgram-0.0.2/newgram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/check_password.py` & `Newgram-0.0.2/newgram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/connect.py` & `Newgram-0.0.2/newgram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/disconnect.py` & `Newgram-0.0.2/newgram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/get_password_hint.py` & `Newgram-0.0.2/newgram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/initialize.py` & `Newgram-0.0.2/newgram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/log_out.py` & `Newgram-0.0.2/newgram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/recover_password.py` & `Newgram-0.0.2/newgram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/resend_code.py` & `Newgram-0.0.2/newgram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/send_code.py` & `Newgram-0.0.2/newgram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/send_recovery_code.py` & `Newgram-0.0.2/newgram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/sign_in.py` & `Newgram-0.0.2/newgram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/sign_in_bot.py` & `Newgram-0.0.2/newgram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/sign_up.py` & `Newgram-0.0.2/newgram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/auth/terminate.py` & `Newgram-0.0.2/newgram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/__init__.py` & `Newgram-0.0.2/newgram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/answer_callback_query.py` & `Newgram-0.0.2/newgram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/answer_inline_query.py` & `Newgram-0.0.2/newgram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/answer_web_app_query.py` & `Newgram-0.0.2/newgram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/delete_bot_commands.py` & `Newgram-0.0.2/newgram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/get_bot_commands.py` & `Newgram-0.0.2/newgram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/get_bot_default_privileges.py` & `Newgram-0.0.2/newgram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/get_chat_menu_button.py` & `Newgram-0.0.2/newgram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/get_game_high_scores.py` & `Newgram-0.0.2/newgram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/get_inline_bot_results.py` & `Newgram-0.0.2/newgram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/request_callback_answer.py` & `Newgram-0.0.2/newgram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/send_game.py` & `Newgram-0.0.2/newgram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/send_inline_bot_result.py` & `Newgram-0.0.2/newgram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/set_bot_commands.py` & `Newgram-0.0.2/newgram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/set_bot_default_privileges.py` & `Newgram-0.0.2/newgram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/set_chat_menu_button.py` & `Newgram-0.0.2/newgram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/bots/set_game_score.py` & `Newgram-0.0.2/newgram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/__init__.py` & `Newgram-0.0.2/newgram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/add_chat_members.py` & `Newgram-0.0.2/newgram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/archive_chats.py` & `Newgram-0.0.2/newgram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/ban_chat_member.py` & `Newgram-0.0.2/newgram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/create_channel.py` & `Newgram-0.0.2/newgram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/create_group.py` & `Newgram-0.0.2/newgram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/create_supergroup.py` & `Newgram-0.0.2/newgram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/delete_channel.py` & `Newgram-0.0.2/newgram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/delete_chat_photo.py` & `Newgram-0.0.2/newgram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/delete_supergroup.py` & `Newgram-0.0.2/newgram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/delete_user_history.py` & `Newgram-0.0.2/newgram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_chat.py` & `Newgram-0.0.2/newgram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_chat_event_log.py` & `Newgram-0.0.2/newgram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_chat_member.py` & `Newgram-0.0.2/newgram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_chat_members.py` & `Newgram-0.0.2/newgram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_chat_members_count.py` & `Newgram-0.0.2/newgram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_chat_online_count.py` & `Newgram-0.0.2/newgram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_dialogs.py` & `Newgram-0.0.2/newgram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_dialogs_count.py` & `Newgram-0.0.2/newgram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_nearby_chats.py` & `Newgram-0.0.2/newgram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/get_send_as_chats.py` & `Newgram-0.0.2/newgram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/join_chat.py` & `Newgram-0.0.2/newgram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/leave_chat.py` & `Newgram-0.0.2/newgram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/mark_chat_unread.py` & `Newgram-0.0.2/newgram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/pin_chat_message.py` & `Newgram-0.0.2/newgram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/promote_chat_member.py` & `Newgram-0.0.2/newgram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/restrict_chat_member.py` & `Newgram-0.0.2/newgram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_administrator_title.py` & `Newgram-0.0.2/newgram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_chat_description.py` & `Newgram-0.0.2/newgram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_chat_permissions.py` & `Newgram-0.0.2/newgram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_chat_photo.py` & `Newgram-0.0.2/newgram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_chat_protected_content.py` & `Newgram-0.0.2/newgram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_chat_title.py` & `Newgram-0.0.2/newgram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_chat_username.py` & `Newgram-0.0.2/newgram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_send_as_chat.py` & `Newgram-0.0.2/newgram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/set_slow_mode.py` & `Newgram-0.0.2/newgram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/unarchive_chats.py` & `Newgram-0.0.2/newgram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/unban_chat_member.py` & `Newgram-0.0.2/newgram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/unpin_all_chat_messages.py` & `Newgram-0.0.2/newgram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/chats/unpin_chat_message.py` & `Newgram-0.0.2/newgram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/contacts/__init__.py` & `Newgram-0.0.2/newgram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/contacts/add_contact.py` & `Newgram-0.0.2/newgram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/contacts/delete_contacts.py` & `Newgram-0.0.2/newgram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/contacts/get_contacts.py` & `Newgram-0.0.2/newgram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/contacts/get_contacts_count.py` & `Newgram-0.0.2/newgram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/contacts/import_contacts.py` & `Newgram-0.0.2/newgram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/__init__.py` & `Newgram-0.0.2/newgram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_callback_query.py` & `Newgram-0.0.2/newgram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_chat_join_request.py` & `Newgram-0.0.2/newgram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_chat_member_updated.py` & `Newgram-0.0.2/newgram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_chosen_inline_result.py` & `Newgram-0.0.2/newgram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_deleted_messages.py` & `Newgram-0.0.2/newgram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_disconnect.py` & `Newgram-0.0.2/newgram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_edited_message.py` & `Newgram-0.0.2/newgram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_inline_query.py` & `Newgram-0.0.2/newgram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_message.py` & `Newgram-0.0.2/newgram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_poll.py` & `Newgram-0.0.2/newgram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_raw_update.py` & `Newgram-0.0.2/newgram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/decorators/on_user_status.py` & `Newgram-0.0.2/newgram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/__init__.py` & `Newgram-0.0.2/newgram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/approve_all_chat_join_requests.py` & `Newgram-0.0.2/newgram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/approve_chat_join_request.py` & `Newgram-0.0.2/newgram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/create_chat_invite_link.py` & `Newgram-0.0.2/newgram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/decline_all_chat_join_requests.py` & `Newgram-0.0.2/newgram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/decline_chat_join_request.py` & `Newgram-0.0.2/newgram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/delete_chat_admin_invite_links.py` & `Newgram-0.0.2/newgram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/delete_chat_invite_link.py` & `Newgram-0.0.2/newgram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/edit_chat_invite_link.py` & `Newgram-0.0.2/newgram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/export_chat_invite_link.py` & `Newgram-0.0.2/newgram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_admin_invite_links.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_admin_invite_links_count.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_admins_with_invite_links.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_invite_link.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_invite_link_joiners.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/get_chat_join_requests.py` & `Newgram-0.0.2/newgram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/invite_links/revoke_chat_invite_link.py` & `Newgram-0.0.2/newgram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/__init__.py` & `Newgram-0.0.2/newgram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/copy_media_group.py` & `Newgram-0.0.2/newgram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/copy_message.py` & `Newgram-0.0.2/newgram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/delete_messages.py` & `Newgram-0.0.2/newgram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/download_media.py` & `Newgram-0.0.2/newgram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_inline_caption.py` & `Newgram-0.0.2/newgram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_inline_media.py` & `Newgram-0.0.2/newgram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_inline_reply_markup.py` & `Newgram-0.0.2/newgram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_inline_text.py` & `Newgram-0.0.2/newgram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_message_caption.py` & `Newgram-0.0.2/newgram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_message_media.py` & `Newgram-0.0.2/newgram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_message_reply_markup.py` & `Newgram-0.0.2/newgram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/edit_message_text.py` & `Newgram-0.0.2/newgram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/forward_messages.py` & `Newgram-0.0.2/newgram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_chat_history.py` & `Newgram-0.0.2/newgram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_chat_history_count.py` & `Newgram-0.0.2/newgram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_custom_emoji_stickers.py` & `Newgram-0.0.2/newgram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_discussion_message.py` & `Newgram-0.0.2/newgram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_discussion_replies.py` & `Newgram-0.0.2/newgram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_discussion_replies_count.py` & `Newgram-0.0.2/newgram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_media_group.py` & `Newgram-0.0.2/newgram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/get_messages.py` & `Newgram-0.0.2/newgram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/inline_session.py` & `Newgram-0.0.2/newgram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/read_chat_history.py` & `Newgram-0.0.2/newgram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/retract_vote.py` & `Newgram-0.0.2/newgram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/search_global.py` & `Newgram-0.0.2/newgram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/search_global_count.py` & `Newgram-0.0.2/newgram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/search_messages.py` & `Newgram-0.0.2/newgram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/search_messages_count.py` & `Newgram-0.0.2/newgram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_animation.py` & `Newgram-0.0.2/newgram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_audio.py` & `Newgram-0.0.2/newgram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_cached_media.py` & `Newgram-0.0.2/newgram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_chat_action.py` & `Newgram-0.0.2/newgram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_contact.py` & `Newgram-0.0.2/newgram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_dice.py` & `Newgram-0.0.2/newgram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_document.py` & `Newgram-0.0.2/newgram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_location.py` & `Newgram-0.0.2/newgram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_media_group.py` & `Newgram-0.0.2/newgram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_message.py` & `Newgram-0.0.2/newgram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_photo.py` & `Newgram-0.0.2/newgram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_poll.py` & `Newgram-0.0.2/newgram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_reaction.py` & `Newgram-0.0.2/newgram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_sticker.py` & `Newgram-0.0.2/newgram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_venue.py` & `Newgram-0.0.2/newgram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_video.py` & `Newgram-0.0.2/newgram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_video_note.py` & `Newgram-0.0.2/newgram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/send_voice.py` & `Newgram-0.0.2/newgram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/stop_poll.py` & `Newgram-0.0.2/newgram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/stream_media.py` & `Newgram-0.0.2/newgram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/messages/vote_poll.py` & `Newgram-0.0.2/newgram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/password/__init__.py` & `Newgram-0.0.2/newgram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/password/change_cloud_password.py` & `Newgram-0.0.2/newgram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/password/enable_cloud_password.py` & `Newgram-0.0.2/newgram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/password/remove_cloud_password.py` & `Newgram-0.0.2/newgram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/__init__.py` & `Newgram-0.0.2/newgram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/block_user.py` & `Newgram-0.0.2/newgram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/delete_profile_photos.py` & `Newgram-0.0.2/newgram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/get_chat_photos.py` & `Newgram-0.0.2/newgram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/get_chat_photos_count.py` & `Newgram-0.0.2/newgram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/get_common_chats.py` & `Newgram-0.0.2/newgram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/get_default_emoji_statuses.py` & `Newgram-0.0.2/newgram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/get_me.py` & `Newgram-0.0.2/newgram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/get_users.py` & `Newgram-0.0.2/newgram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/set_emoji_status.py` & `Newgram-0.0.2/newgram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/set_profile_photo.py` & `Newgram-0.0.2/newgram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/set_username.py` & `Newgram-0.0.2/newgram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/unblock_user.py` & `Newgram-0.0.2/newgram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/users/update_profile.py` & `Newgram-0.0.2/newgram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/__init__.py` & `Newgram-0.0.2/newgram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/add_handler.py` & `Newgram-0.0.2/newgram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/compose.py` & `Newgram-0.0.2/newgram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/export_session_string.py` & `Newgram-0.0.2/newgram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/idle.py` & `Newgram-0.0.2/newgram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/remove_handler.py` & `Newgram-0.0.2/newgram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/restart.py` & `Newgram-0.0.2/newgram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/run.py` & `Newgram-0.0.2/newgram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/start.py` & `Newgram-0.0.2/newgram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/stop.py` & `Newgram-0.0.2/newgram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/methods/utilities/stop_transmission.py` & `Newgram-0.0.2/newgram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/mime_types.py` & `Newgram-0.0.2/newgram/mime_types.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/parser/__init__.py` & `Newgram-0.0.2/newgram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/parser/html.py` & `Newgram-0.0.2/newgram/parser/html.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/parser/markdown.py` & `Newgram-0.0.2/newgram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/parser/parser.py` & `Newgram-0.0.2/newgram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/parser/utils.py` & `Newgram-0.0.2/newgram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/__init__.py` & `Newgram-0.0.2/newgram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/__init__.py` & `Newgram-0.0.2/newgram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/future_salt.py` & `Newgram-0.0.2/newgram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/future_salts.py` & `Newgram-0.0.2/newgram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/gzip_packed.py` & `Newgram-0.0.2/newgram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/list.py` & `Newgram-0.0.2/newgram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/message.py` & `Newgram-0.0.2/newgram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/msg_container.py` & `Newgram-0.0.2/newgram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/__init__.py` & `Newgram-0.0.2/newgram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/bool.py` & `Newgram-0.0.2/newgram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/bytes.py` & `Newgram-0.0.2/newgram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/double.py` & `Newgram-0.0.2/newgram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/int.py` & `Newgram-0.0.2/newgram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/string.py` & `Newgram-0.0.2/newgram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/primitives/vector.py` & `Newgram-0.0.2/newgram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/raw/core/tl_object.py` & `Newgram-0.0.2/newgram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/__init__.py` & `Newgram-0.0.2/newgram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/auth.py` & `Newgram-0.0.2/newgram/session/auth.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/internals/__init__.py` & `Newgram-0.0.2/newgram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/internals/data_center.py` & `Newgram-0.0.2/newgram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/internals/msg_factory.py` & `Newgram-0.0.2/newgram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/internals/msg_id.py` & `Newgram-0.0.2/newgram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/internals/seq_no.py` & `Newgram-0.0.2/newgram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/session/session.py` & `Newgram-0.0.2/newgram/session/session.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/storage/__init__.py` & `Newgram-0.0.2/newgram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/storage/file_storage.py` & `Newgram-0.0.2/newgram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/storage/memory_storage.py` & `Newgram-0.0.2/newgram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/storage/sqlite_storage.py` & `Newgram-0.0.2/newgram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/storage/storage.py` & `Newgram-0.0.2/newgram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/sync.py` & `Newgram-0.0.2/newgram/sync.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/__init__.py` & `Newgram-0.0.2/newgram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/authorization/__init__.py` & `Newgram-0.0.2/newgram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/authorization/sent_code.py` & `Newgram-0.0.2/newgram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/authorization/terms_of_service.py` & `Newgram-0.0.2/newgram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/__init__.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_chat.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/bot_command_scope_default.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/callback_game.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/callback_query.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/force_reply.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/game_high_score.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/inline_keyboard_button.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/inline_keyboard_markup.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/keyboard_button.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/login_url.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button_commands.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button_default.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/menu_button_web_app.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/reply_keyboard_markup.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/reply_keyboard_remove.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/sent_web_app_message.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/bots_and_keyboards/web_app_info.py` & `Newgram-0.0.2/newgram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/__init__.py` & `Newgram-0.0.2/newgram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/chosen_inline_result.py` & `Newgram-0.0.2/newgram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_animation.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_article.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_audio.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_animation.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_audio.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_document.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_photo.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_sticker.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_video.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_cached_voice.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_contact.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_document.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_location.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_photo.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_venue.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_video.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/inline_mode/inline_query_result_voice.py` & `Newgram-0.0.2/newgram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/__init__.py` & `Newgram-0.0.2/newgram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_media.py` & `Newgram-0.0.2/newgram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_media_animation.py` & `Newgram-0.0.2/newgram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_media_audio.py` & `Newgram-0.0.2/newgram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_media_document.py` & `Newgram-0.0.2/newgram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_media_photo.py` & `Newgram-0.0.2/newgram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_media_video.py` & `Newgram-0.0.2/newgram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_media/input_phone_contact.py` & `Newgram-0.0.2/newgram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_message_content/__init__.py` & `Newgram-0.0.2/newgram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_message_content/input_message_content.py` & `Newgram-0.0.2/newgram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/input_message_content/input_text_message_content.py` & `Newgram-0.0.2/newgram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/list.py` & `Newgram-0.0.2/newgram/types/list.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/__init__.py` & `Newgram-0.0.2/newgram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/animation.py` & `Newgram-0.0.2/newgram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/audio.py` & `Newgram-0.0.2/newgram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/contact.py` & `Newgram-0.0.2/newgram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/dice.py` & `Newgram-0.0.2/newgram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/document.py` & `Newgram-0.0.2/newgram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/game.py` & `Newgram-0.0.2/newgram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/location.py` & `Newgram-0.0.2/newgram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/message.py` & `Newgram-0.0.2/newgram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/message_entity.py` & `Newgram-0.0.2/newgram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/message_reactions.py` & `Newgram-0.0.2/newgram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/photo.py` & `Newgram-0.0.2/newgram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/poll.py` & `Newgram-0.0.2/newgram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/poll_option.py` & `Newgram-0.0.2/newgram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/reaction.py` & `Newgram-0.0.2/newgram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/sticker.py` & `Newgram-0.0.2/newgram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/stripped_thumbnail.py` & `Newgram-0.0.2/newgram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/thumbnail.py` & `Newgram-0.0.2/newgram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/venue.py` & `Newgram-0.0.2/newgram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/video.py` & `Newgram-0.0.2/newgram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/video_note.py` & `Newgram-0.0.2/newgram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/voice.py` & `Newgram-0.0.2/newgram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/web_app_data.py` & `Newgram-0.0.2/newgram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/messages_and_media/web_page.py` & `Newgram-0.0.2/newgram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/object.py` & `Newgram-0.0.2/newgram/types/object.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/update.py` & `Newgram-0.0.2/newgram/types/update.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/__init__.py` & `Newgram-0.0.2/newgram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_admin_with_invite_links.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_event.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_event_filter.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_invite_link.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_join_request.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_joiner.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_member.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_member_updated.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_permissions.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_photo.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_preview.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_privileges.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/chat_reactions.py` & `Newgram-0.0.2/newgram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/dialog.py` & `Newgram-0.0.2/newgram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/emoji_status.py` & `Newgram-0.0.2/newgram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/invite_link_importer.py` & `Newgram-0.0.2/newgram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/restriction.py` & `Newgram-0.0.2/newgram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/user.py` & `Newgram-0.0.2/newgram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/video_chat_ended.py` & `Newgram-0.0.2/newgram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/video_chat_members_invited.py` & `Newgram-0.0.2/newgram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/video_chat_scheduled.py` & `Newgram-0.0.2/newgram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/types/user_and_chats/video_chat_started.py` & `Newgram-0.0.2/newgram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/newgram/utils.py` & `Newgram-0.0.2/newgram/utils.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/tests/__init__.py` & `Newgram-0.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/tests/filters/__init__.py` & `Newgram-0.0.2/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/tests/filters/test_command.py` & `Newgram-0.0.2/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/tests/parser/__init__.py` & `Newgram-0.0.2/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/tests/parser/test_html.py` & `Newgram-0.0.2/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `Newgram-0.0.1/tests/test_file_id.py` & `Newgram-0.0.2/tests/test_file_id.py`

 * *Files identical despite different names*

