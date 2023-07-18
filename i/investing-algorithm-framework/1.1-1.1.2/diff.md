# Comparing `tmp/investing_algorithm_framework-1.1.tar.gz` & `tmp/investing_algorithm_framework-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-1.1.tar", last modified: Mon Jul 17 20:48:36 2023, max compression
+gzip compressed data, was "investing_algorithm_framework-1.1.2.tar", last modified: Tue Jul 18 19:26:30 2023, max compression
```

## Comparing `investing_algorithm_framework-1.1.tar` & `investing_algorithm_framework-1.1.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/run_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/dependency_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/asset_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/position_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/synchronized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/model_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position_cost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/market_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/services/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/market_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15968 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/order_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_configuration_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/position_cost_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/setup_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/tests/test_create_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.543023 investing_algorithm_framework-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-18 19:26:30.543023 investing_algorithm_framework-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.523022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.527022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.527022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.527022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.527022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.527022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/run_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.531022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/dependency_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.531022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.531022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.531022 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/asset_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/position/position_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.535023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/model_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.539023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.539023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.539023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/position/position_cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.539023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.539023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/services/market_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.543023 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/market_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15968 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/order_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/portfolio_configuration_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/portfolio_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/position_cost_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework/setup_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.523022 investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-18 19:26:30.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-18 19:26:30.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:26:30.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 19:26:30.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 19:26:30.000000 investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 19:26:30.543023 investing_algorithm_framework-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:26:30.543023 investing_algorithm_framework-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-18 19:25:45.000000 investing_algorithm_framework-1.1.2/tests/test_create_app.py
```

### Comparing `investing_algorithm_framework-1.1/LICENSE` & `investing_algorithm_framework-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/PKG-INFO` & `investing_algorithm_framework-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing_algorithm_framework
-Version: 1.1
+Version: 1.1.2
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
 Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
 Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
```

### Comparing `investing_algorithm_framework-1.1/README.md` & `investing_algorithm_framework-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/algorithm.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             self.strategy = CheckOnlineHandler()
         else:
             raise OperationalException("Action not supported")
 
     @staticmethod
     def get_action_type(payload):
 
+        if payload is None or ("ACTION" not in payload and "action" not in payload):
+            raise OperationalException("Action type is not defined")
+
         if "action" in payload:
             action = payload["action"]
         else:
             action = payload["ACTION"]
 
-        if action is None:
-            raise OperationalException("Action type not supported")
-
         return action
```

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,20 +6,28 @@
 
 class RunStrategyHandler(ActionHandlerStrategy):
     MESSAGE = {"message": "Ok"}
 
     def handle_event(self, payload, algorithm):
         strategies = algorithm.strategy_orchestrator_service\
             .get_strategies(payload.get("strategies", None))
+        tasks = algorithm.strategy_orchestrator_service.get_tasks()
 
         for strategy in strategies:
             algorithm.strategy_orchestrator_service.run_strategy(
                 strategy=strategy,
                 algorithm=algorithm,
                 sync=True
             )
 
+        for task in tasks:
+            algorithm.strategy_orchestrator_service.run_task(
+                task=task,
+                algorithm=algorithm,
+                sync=True
+            )
+
         return {
             "statusCode": 200,
             "headers": {"Content-Type": "application/json"},
             "body": json.dumps({"message": RunStrategyHandler.MESSAGE})
         }
```

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/dependency_container.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/asset_price.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/asset_price.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ohlcv.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/ohlcv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/order_book.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/order_book.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ticker.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/market_data/ticker.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/position_cost.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/position/position_cost.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position_cost.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/models/position/position_cost.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/market_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/infrastructure/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/market_data_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/market_data_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/order_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/order_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_configuration_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,17 @@
         strategies = []
         for strategy in self.strategies:
             if strategy.worker_id in identifiers:
                 strategies.append(strategy)
 
         return strategies
 
+    def get_tasks(self):
+        return self._tasks
+
     def get_jobs(self):
         return schedule.jobs
 
     def run_pending_jobs(self):
 
         if self.max_iterations is not None and \
                 self.max_iterations != -1 and \
```

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework/setup_logging.py` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework/setup_logging.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/PKG-INFO` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 1.1
+Version: 1.1.2
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
 Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
 Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
```

### Comparing `investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/SOURCES.txt` & `investing_algorithm_framework-1.1.2/investing_algorithm_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/setup.py` & `investing_algorithm_framework-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.1/tests/test_create_app.py` & `investing_algorithm_framework-1.1.2/tests/test_create_app.py`

 * *Files identical despite different names*

