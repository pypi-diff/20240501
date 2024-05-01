# Comparing `tmp/tinkoff_investments-0.2.0b97.tar.gz` & `tmp/tinkoff_investments-0.2.0b98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinkoff_investments-0.2.0b97.tar", max compression
+gzip compressed data, was "tinkoff_investments-0.2.0b98.tar", max compression
```

## Comparing `tinkoff_investments-0.2.0b97.tar` & `tinkoff_investments-0.2.0b98.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    11338 2024-03-27 13:25:57.619885 tinkoff_investments-0.2.0b97/LICENSE
--rw-r--r--   0        0        0     2908 2024-03-27 13:25:57.619885 tinkoff_investments-0.2.0b97/README.md
--rw-r--r--   0        0        0     2957 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/pyproject.toml
--rw-r--r--   0        0        0    12529 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/__init__.py
--rw-r--r--   0        0        0     4742 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/_errors.py
--rw-r--r--   0        0        0    13378 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/_grpc_helpers.py
--rw-r--r--   0        0        0    70800 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/async_services.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/__init__.py
--rw-r--r--   0        0        0     2685 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/instrument_storage.py
--rw-r--r--   0        0        0     7135 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/instruments_cache.py
--rw-r--r--   0        0        0     2167 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/interface.py
--rw-r--r--   0        0        0      187 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/models.py
--rw-r--r--   0        0        0      379 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/protocol.py
--rw-r--r--   0        0        0      148 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/settings.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.627885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/__init__.py
--rw-r--r--   0        0        0     5302 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/cache.py
--rw-r--r--   0        0        0     1388 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/cache_settings.py
--rw-r--r--   0        0        0       98 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/datetime_range.py
--rw-r--r--   0        0        0      315 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/instrument_date_range_market_data.py
--rw-r--r--   0        0        0    11766 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py
--rw-r--r--   0        0        0      376 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/interface.py
--rw-r--r--   0        0        0      218 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/serialization.py
--rw-r--r--   0        0        0      305 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/caching/overrides.py
--rw-r--r--   0        0        0      411 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/candle_getter_protocol.py
--rw-r--r--   0        0        0     1504 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/channels.py
--rw-r--r--   0        0        0     3016 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/clients.py
--rw-r--r--   0        0        0      439 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/constants.py
--rw-r--r--   0        0        0      914 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/__init__.py
--rw-r--r--   0        0        0     4818 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/common_pb2.py
--rw-r--r--   0        0        0    15679 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/common_pb2_grpc.py
--rw-r--r--   0        0        0     1871 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/google/api/field_behavior_pb2.py
--rw-r--r--   0        0        0     6343 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/google/api/field_behavior_pb2_grpc.py
--rw-r--r--   0        0        0    76329 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/instruments_pb2.py
--rw-r--r--   0        0        0   272114 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/instruments_pb2.pyi
--rw-r--r--   0        0        0    63760 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/instruments_pb2_grpc.py
--rw-r--r--   0        0        0    36331 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/marketdata_pb2.py
--rw-r--r--   0        0        0   117772 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/marketdata_pb2.pyi
--rw-r--r--   0        0        0    21465 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/marketdata_pb2_grpc.py
--rw-r--r--   0        0        0    35099 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/operations_pb2.py
--rw-r--r--   0        0        0   113219 2024-03-27 13:25:57.631885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/operations_pb2.pyi
--rw-r--r--   0        0        0    20550 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/operations_pb2_grpc.py
--rw-r--r--   0        0        0    19296 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/orders_pb2.py
--rw-r--r--   0        0        0    52382 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/orders_pb2.pyi
--rw-r--r--   0        0        0    17156 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/orders_pb2_grpc.py
--rw-r--r--   0        0        0     6219 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/sandbox_pb2.py
--rw-r--r--   0        0        0     4578 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/sandbox_pb2.pyi
--rw-r--r--   0        0        0    27909 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/sandbox_pb2_grpc.py
--rw-r--r--   0        0        0    12432 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/stoporders_pb2.py
--rw-r--r--   0        0        0    30740 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/stoporders_pb2.pyi
--rw-r--r--   0        0        0     7177 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/stoporders_pb2_grpc.py
--rw-r--r--   0        0        0     7030 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/users_pb2.py
--rw-r--r--   0        0        0    17677 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/users_pb2.pyi
--rw-r--r--   0        0        0     8756 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/users_pb2_grpc.py
--rw-r--r--   0        0        0     3485 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/logging.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/__init__.py
--rw-r--r--   0        0        0     2971 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py
--rw-r--r--   0        0        0     1362 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/market_data_stream_interface.py
--rw-r--r--   0        0        0     2799 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/market_data_stream_manager.py
--rw-r--r--   0        0        0     5101 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/stream_managers.py
--rw-r--r--   0        0        0      128 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/typevars.py
--rw-r--r--   0        0        0      289 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/metadata.py
--rw-r--r--   0        0        0    12487 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/mock_services.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/py.typed
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/__init__.py
--rw-r--r--   0        0        0      825 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/client.py
--rw-r--r--   0        0        0      772 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/grpc_interceptor.py
--rw-r--r--   0        0        0     1163 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/retry_manager.py
--rw-r--r--   0        0        0      796 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/base_retry_manager.py
--rw-r--r--   0        0        0      243 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/settings.py
--rw-r--r--   0        0        0      122 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/settings_protocol.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/__init__.py
--rw-r--r--   0        0        0      792 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/client.py
--rw-r--r--   0        0        0      696 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/grpc_interceptor.py
--rw-r--r--   0        0        0     1027 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/retry_manager.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/sandbox/__init__.py
--rw-r--r--   0        0        0      296 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/sandbox/client.py
--rw-r--r--   0        0        0   118974 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/schemas.py
--rw-r--r--   0        0        0    69084 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/services.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/__init__.py
--rw-r--r--   0        0        0     1457 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/account_manager.py
--rw-r--r--   0        0        0      555 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/errors.py
--rw-r--r--   0        0        0      401 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/event.py
--rw-r--r--   0        0        0      341 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/models.py
--rw-r--r--   0        0        0      847 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/signal.py
--rw-r--r--   0        0        0     2032 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/signal_executor_base.py
--rw-r--r--   0        0        0      387 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/strategy_interface.py
--rw-r--r--   0        0        0      541 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/strategy_settings_base.py
--rw-r--r--   0        0        0      754 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/strategy_supervisor.py
--rw-r--r--   0        0        0     2435 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/trader_base.py
--rw-r--r--   0        0        0       89 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/trader_interface.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/__init__.py
--rw-r--r--   0        0        0     7419 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/plotter.py
--rw-r--r--   0        0        0     2244 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/signal_executor.py
--rw-r--r--   0        0        0    10442 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/strategy.py
--rw-r--r--   0        0        0      295 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/strategy_settings.py
--rw-r--r--   0        0        0      705 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/strategy_state.py
--rw-r--r--   0        0        0      970 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/supervisor.py
--rw-r--r--   0        0        0     6514 2024-03-27 13:25:57.635885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/trader.py
--rw-r--r--   0        0        0        0 2024-03-27 13:25:57.639885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/plotting/__init__.py
--rw-r--r--   0        0        0     1973 2024-03-27 13:25:57.639885 tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/plotting/plotter.py
--rw-r--r--   0        0        0      170 2024-03-27 13:25:57.639885 tinkoff_investments-0.2.0b97/tinkoff/invest/typedefs.py
--rw-r--r--   0        0        0     7651 2024-03-27 13:25:57.639885 tinkoff_investments-0.2.0b97/tinkoff/invest/utils.py
--rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 tinkoff_investments-0.2.0b97/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-05-01 17:29:30.010029 tinkoff_investments-0.2.0b98/LICENSE
+-rw-r--r--   0        0        0     2908 2024-05-01 17:29:30.010029 tinkoff_investments-0.2.0b98/README.md
+-rw-r--r--   0        0        0     2957 2024-05-01 17:29:30.014029 tinkoff_investments-0.2.0b98/pyproject.toml
+-rw-r--r--   0        0        0    12529 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/__init__.py
+-rw-r--r--   0        0        0     4742 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/_errors.py
+-rw-r--r--   0        0        0    13378 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/_grpc_helpers.py
+-rw-r--r--   0        0        0    72216 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/async_services.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/__init__.py
+-rw-r--r--   0        0        0     2685 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instrument_storage.py
+-rw-r--r--   0        0        0     7135 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instruments_cache.py
+-rw-r--r--   0        0        0     2167 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/interface.py
+-rw-r--r--   0        0        0      187 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/models.py
+-rw-r--r--   0        0        0      379 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/protocol.py
+-rw-r--r--   0        0        0      148 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/settings.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/__init__.py
+-rw-r--r--   0        0        0     5302 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache.py
+-rw-r--r--   0        0        0     1388 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache_settings.py
+-rw-r--r--   0        0        0       98 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/datetime_range.py
+-rw-r--r--   0        0        0      315 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/instrument_date_range_market_data.py
+-rw-r--r--   0        0        0    11766 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py
+-rw-r--r--   0        0        0      376 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/interface.py
+-rw-r--r--   0        0        0      218 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/serialization.py
+-rw-r--r--   0        0        0      305 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/caching/overrides.py
+-rw-r--r--   0        0        0      411 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/candle_getter_protocol.py
+-rw-r--r--   0        0        0     1504 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/channels.py
+-rw-r--r--   0        0        0     3016 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/clients.py
+-rw-r--r--   0        0        0      439 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/constants.py
+-rw-r--r--   0        0        0      914 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/__init__.py
+-rw-r--r--   0        0        0     4818 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.py
+-rw-r--r--   0        0        0    15679 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2_grpc.py
+-rw-r--r--   0        0        0     1871 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.py
+-rw-r--r--   0        0        0     6343 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2_grpc.py
+-rw-r--r--   0        0        0    77252 2024-05-01 17:29:30.018029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.py
+-rw-r--r--   0        0        0   275576 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.pyi
+-rw-r--r--   0        0        0    63760 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2_grpc.py
+-rw-r--r--   0        0        0    36932 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.py
+-rw-r--r--   0        0        0   119955 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.pyi
+-rw-r--r--   0        0        0    21465 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2_grpc.py
+-rw-r--r--   0        0        0    35099 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.py
+-rw-r--r--   0        0        0   113219 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.pyi
+-rw-r--r--   0        0        0    20550 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2_grpc.py
+-rw-r--r--   0        0        0    24889 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.py
+-rw-r--r--   0        0        0    74934 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.pyi
+-rw-r--r--   0        0        0    19021 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2_grpc.py
+-rw-r--r--   0        0        0     6383 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.py
+-rw-r--r--   0        0        0     4578 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.pyi
+-rw-r--r--   0        0        0    29360 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2_grpc.py
+-rw-r--r--   0        0        0    12547 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.py
+-rw-r--r--   0        0        0    31067 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.pyi
+-rw-r--r--   0        0        0     7177 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2_grpc.py
+-rw-r--r--   0        0        0     7030 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.py
+-rw-r--r--   0        0        0    17677 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.pyi
+-rw-r--r--   0        0        0     8756 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2_grpc.py
+-rw-r--r--   0        0        0     3485 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/logging.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/__init__.py
+-rw-r--r--   0        0        0     2971 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py
+-rw-r--r--   0        0        0     1362 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_interface.py
+-rw-r--r--   0        0        0     2799 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_manager.py
+-rw-r--r--   0        0        0     5101 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/stream_managers.py
+-rw-r--r--   0        0        0      128 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/typevars.py
+-rw-r--r--   0        0        0      289 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/metadata.py
+-rw-r--r--   0        0        0    12487 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/mock_services.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/__init__.py
+-rw-r--r--   0        0        0      825 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/client.py
+-rw-r--r--   0        0        0      772 2024-05-01 17:29:30.022029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/grpc_interceptor.py
+-rw-r--r--   0        0        0     1163 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/retry_manager.py
+-rw-r--r--   0        0        0      796 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/base_retry_manager.py
+-rw-r--r--   0        0        0      243 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/settings.py
+-rw-r--r--   0        0        0      122 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/settings_protocol.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/client.py
+-rw-r--r--   0        0        0      696 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/grpc_interceptor.py
+-rw-r--r--   0        0        0     1027 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/retry_manager.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/sandbox/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/sandbox/client.py
+-rw-r--r--   0        0        0   123566 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/schemas.py
+-rw-r--r--   0        0        0    70635 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/services.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/__init__.py
+-rw-r--r--   0        0        0     1457 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/account_manager.py
+-rw-r--r--   0        0        0      555 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/errors.py
+-rw-r--r--   0        0        0      401 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/event.py
+-rw-r--r--   0        0        0      341 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/models.py
+-rw-r--r--   0        0        0      847 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal.py
+-rw-r--r--   0        0        0     2032 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal_executor_base.py
+-rw-r--r--   0        0        0      387 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_interface.py
+-rw-r--r--   0        0        0      541 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_settings_base.py
+-rw-r--r--   0        0        0      754 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_supervisor.py
+-rw-r--r--   0        0        0     2435 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/trader_base.py
+-rw-r--r--   0        0        0       89 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/trader_interface.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/__init__.py
+-rw-r--r--   0        0        0     7419 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/plotter.py
+-rw-r--r--   0        0        0     2244 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/signal_executor.py
+-rw-r--r--   0        0        0    10442 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy.py
+-rw-r--r--   0        0        0      295 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy_settings.py
+-rw-r--r--   0        0        0      705 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy_state.py
+-rw-r--r--   0        0        0      970 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/supervisor.py
+-rw-r--r--   0        0        0     6514 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/trader.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/plotting/__init__.py
+-rw-r--r--   0        0        0     1973 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/plotting/plotter.py
+-rw-r--r--   0        0        0      170 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/typedefs.py
+-rw-r--r--   0        0        0     7651 2024-05-01 17:29:30.026029 tinkoff_investments-0.2.0b98/tinkoff/invest/utils.py
+-rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 tinkoff_investments-0.2.0b98/PKG-INFO
```

### Comparing `tinkoff_investments-0.2.0b97/LICENSE` & `tinkoff_investments-0.2.0b98/LICENSE`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/README.md` & `tinkoff_investments-0.2.0b98/README.md`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/pyproject.toml` & `tinkoff_investments-0.2.0b98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tinkoff-investments"
-version = "0.2.0-beta97"
+version = "0.2.0-beta98"
 description = "Tinkoff Python SDK"
 authors = ["Tinkoff Team <python@tinkoff.ru>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/RussianInvestments/invest-python"
 homepage = "https://github.com/RussianInvestments/invest-python"
 packages = [
@@ -106,15 +106,15 @@
 
 [tool.black]
 exclude = "tinkoff/invest/grpc"
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
-fail_under = 65
+fail_under = 64
 exclude_lines = [
   "raise NotImplementedError",
   "def __repr__",
   "pragma: no cover"
 ]
 omit = [
   "*/.local/*",
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/__init__.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     TradingSchedulesResponse,
     TradingStatus,
     UnaryLimit,
     WithdrawLimitsRequest,
     WithdrawLimitsResponse,
 )
 
-__version__ = "0.2.0-beta97"
+__version__ = "0.2.0-beta98"
 
 __all__ = (
     "__version__",
     "AccessLevel",
     "Account",
     "AccountStatus",
     "AccountSubscriptionStatus",
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/_errors.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/_errors.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/_grpc_helpers.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/_grpc_helpers.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/async_services.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/async_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     GetTradingStatusResponse,
     GetUserTariffRequest,
     GetUserTariffResponse,
     HistoricCandle,
     IndicativesRequest,
     IndicativesResponse,
     InstrumentClosePriceRequest,
+    InstrumentExchangeType,
     InstrumentIdType,
     InstrumentRequest,
     InstrumentResponse,
     InstrumentsRequest,
     InstrumentStatus,
     InstrumentType,
     MarketDataRequest,
@@ -145,14 +146,16 @@
     OperationsRequest,
     OperationsResponse,
     OperationState,
     OptionResponse,
     OptionsResponse,
     OrderDirection,
     OrderState,
+    OrderStateStreamRequest,
+    OrderStateStreamResponse,
     OrderType,
     Page,
     PortfolioRequest,
     PortfolioResponse,
     PortfolioStreamRequest,
     PortfolioStreamResponse,
     PositionsRequest,
@@ -324,18 +327,22 @@
         )
         response = await response_coro
         log_request(await get_tracking_id_from_coro(response_coro), "BondBy")
         return _grpc_helpers.protobuf_to_dataclass(response, BondResponse)
 
     @handle_aio_request_error("Bonds")
     async def bonds(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> BondsResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response_coro = self.stub.Bonds(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         response = await response_coro
@@ -362,18 +369,22 @@
         )
         response = await response_coro
         log_request(await get_tracking_id_from_coro(response_coro), "CurrencyBy")
         return _grpc_helpers.protobuf_to_dataclass(response, CurrencyResponse)
 
     @handle_aio_request_error("Currencies")
     async def currencies(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> CurrenciesResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response_coro = self.stub.Currencies(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         response = await response_coro
@@ -400,18 +411,22 @@
         )
         response = await response_coro
         log_request(await get_tracking_id_from_coro(response_coro), "EtfBy")
         return _grpc_helpers.protobuf_to_dataclass(response, EtfResponse)
 
     @handle_aio_request_error("Etfs")
     async def etfs(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> EtfsResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response_coro = self.stub.Etfs(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         response = await response_coro
@@ -438,18 +453,22 @@
         )
         response = await response_coro
         log_request(await get_tracking_id_from_coro(response_coro), "FutureBy")
         return _grpc_helpers.protobuf_to_dataclass(response, FutureResponse)
 
     @handle_aio_request_error("Futures")
     async def futures(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> FuturesResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response_coro = self.stub.Futures(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         response = await response_coro
@@ -532,18 +551,22 @@
         )
         response = await response_coro
         log_request(await get_tracking_id_from_coro(response_coro), "ShareBy")
         return _grpc_helpers.protobuf_to_dataclass(response, ShareResponse)
 
     @handle_aio_request_error("Shares")
     async def shares(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> SharesResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response_coro = self.stub.Shares(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         response = await response_coro
@@ -1300,14 +1323,28 @@
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, orders_pb2.TradesStreamRequest()
             ),
             metadata=self.metadata,
         ):
             yield _grpc_helpers.protobuf_to_dataclass(response, TradesStreamResponse)
 
+    @handle_aio_request_error_gen("OrderStateStream")
+    async def order_state_stream(
+        self, *, request: OrderStateStreamRequest
+    ) -> AsyncIterable[OrderStateStreamResponse]:
+        async for response in self.stub.OrderStateStream(
+            request=_grpc_helpers.dataclass_to_protobuff(
+                request, orders_pb2.OrderStateStreamRequest()
+            ),
+            metadata=self.metadata,
+        ):
+            yield _grpc_helpers.protobuf_to_dataclass(
+                response, OrderStateStreamResponse
+            )
+
 
 class OrdersService(_grpc_helpers.Service):
     _stub_factory = orders_pb2_grpc.OrdersServiceStub
 
     @handle_aio_request_error("PostOrder")
     async def post_order(
         self,
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/instrument_storage.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instrument_storage.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/instruments_cache.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/instruments_cache.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/caching/instruments_cache/interface.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/instruments_cache/interface.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/cache.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/cache_settings.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/cache_settings.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/caching/market_data_cache/instrument_market_data_storage.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/channels.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/channels.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/clients.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/clients.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/exceptions.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/common_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/common_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/google/api/field_behavior_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/instruments_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from tinkoff.invest.grpc import (
     common_pb2 as tinkoff_dot_invest_dot_grpc_dot_common__pb2,
 )
 from tinkoff.invest.grpc.google.api import (
     field_behavior_pb2 as tinkoff_dot_invest_dot_grpc_dot_google_dot_api_dot_field__behavior__pb2,
 )
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%tinkoff/invest/grpc/instruments.proto\x12%tinkoff.public.invest.api.contract.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a tinkoff/invest/grpc/common.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"\xa9\x01\n\x17TradingSchedulesRequest\x12\x15\n\x08\x65xchange\x18\x01 \x01(\tH\x00\x88\x01\x01\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x42\x0b\n\t_exchangeB\x07\n\x05_fromB\x05\n\x03_to\"e\n\x18TradingSchedulesResponse\x12I\n\texchanges\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.TradingSchedule\"d\n\x0fTradingSchedule\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12?\n\x04\x64\x61ys\x18\x02 \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.TradingDay\"\x97\x07\n\nTradingDay\x12(\n\x04\x64\x61te\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0eis_trading_day\x18\x02 \x01(\x08\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x1aopening_auction_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x18\x63losing_auction_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x46\n\"evening_opening_auction_start_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12\x65vening_start_time\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x65vening_end_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13\x63learing_start_time\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11\x63learing_end_time\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14premarket_start_time\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12premarket_end_time\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x1a\x63losing_auction_start_time\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x18opening_auction_end_time\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\tintervals\x18\x12 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.TradingIntervalJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"\x9d\x01\n\x11InstrumentRequest\x12N\n\x07id_type\x18\x01 \x01(\x0e\x32\x37.tinkoff.public.invest.api.contract.v1.InstrumentIdTypeB\x04\xe2\x41\x01\x02\x12\x17\n\nclass_code\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x02id\x18\x03 \x01(\tB\x04\xe2\x41\x01\x02\x42\r\n\x0b_class_code\"\x83\x01\n\x12InstrumentsRequest\x12W\n\x11instrument_status\x18\x01 \x01(\x0e\x32\x37.tinkoff.public.invest.api.contract.v1.InstrumentStatusH\x00\x88\x01\x01\x42\x14\n\x12_instrument_status\"\x8c\x01\n\x14\x46ilterOptionsRequest\x12\x1c\n\x0f\x62\x61sic_asset_uid\x18\x01 \x01(\tH\x00\x88\x01\x01\x12%\n\x18\x62\x61sic_asset_position_uid\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x12\n\x10_basic_asset_uidB\x1b\n\x19_basic_asset_position_uid\"O\n\x0c\x42ondResponse\x12?\n\ninstrument\x18\x01 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.Bond\"Q\n\rBondsResponse\x12@\n\x0binstruments\x18\x01 \x03(\x0b\x32+.tinkoff.public.invest.api.contract.v1.Bond\"\xb2\x01\n\x15GetBondCouponsRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\x42\x07\n\x05_fromB\x05\n\x03_to\"W\n\x16GetBondCouponsResponse\x12=\n\x06\x65vents\x18\x01 \x03(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Coupon\"\xef\x02\n\x14GetBondEventsRequest\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\x12S\n\x04type\x18\x05 \x01(\x0e\x32\x45.tinkoff.public.invest.api.contract.v1.GetBondEventsRequest.EventType\"y\n\tEventType\x12\x1a\n\x16\x45VENT_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x45VENT_TYPE_CPN\x10\x01\x12\x13\n\x0f\x45VENT_TYPE_CALL\x10\x02\x12\x12\n\x0e\x45VENT_TYPE_MTY\x10\x03\x12\x13\n\x0f\x45VENT_TYPE_CONV\x10\x04\x42\x07\n\x05_fromB\x05\n\x03_to\"\xf1\x08\n\x15GetBondEventsResponse\x12V\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x46.tinkoff.public.invest.api.contract.v1.GetBondEventsResponse.BondEvent\x1a\xff\x07\n\tBondEvent\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\x12\x14\n\x0c\x65vent_number\x18\x03 \x01(\x05\x12.\n\nevent_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12Y\n\nevent_type\x18\x05 \x01(\x0e\x32\x45.tinkoff.public.invest.api.contract.v1.GetBondEventsRequest.EventType\x12I\n\x0f\x65vent_total_vol\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12,\n\x08\x66ix_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\trate_date\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x64\x65\x66\x61ult_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rreal_pay_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08pay_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12G\n\x0cpay_one_bond\x18\x0c \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12I\n\x0emoney_flow_val\x18\r \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x11\n\texecution\x18\x0e \x01(\t\x12\x16\n\x0eoperation_type\x18\x0f \x01(\t\x12?\n\x05value\x18\x10 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x0c\n\x04note\x18\x11 \x01(\t\x12\x1e\n\x16\x63onvert_to_fin_tool_id\x18\x12 \x01(\t\x12\x35\n\x11\x63oupon_start_date\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63oupon_end_date\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rcoupon_period\x18\x15 \x01(\x05\x12N\n\x14\x63oupon_interest_rate\x18\x16 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xa0\x03\n\x06\x43oupon\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12/\n\x0b\x63oupon_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rcoupon_number\x18\x03 \x01(\x03\x12,\n\x08\x66ix_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12G\n\x0cpay_one_bond\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x46\n\x0b\x63oupon_type\x18\x06 \x01(\x0e\x32\x31.tinkoff.public.invest.api.contract.v1.CouponType\x12\x35\n\x11\x63oupon_start_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63oupon_end_date\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rcoupon_period\x18\t \x01(\x05\"W\n\x10\x43urrencyResponse\x12\x43\n\ninstrument\x18\x01 \x01(\x0b\x32/.tinkoff.public.invest.api.contract.v1.Currency\"Z\n\x12\x43urrenciesResponse\x12\x44\n\x0binstruments\x18\x01 \x03(\x0b\x32/.tinkoff.public.invest.api.contract.v1.Currency\"M\n\x0b\x45tfResponse\x12>\n\ninstrument\x18\x01 \x01(\x0b\x32*.tinkoff.public.invest.api.contract.v1.Etf\"O\n\x0c\x45tfsResponse\x12?\n\x0binstruments\x18\x01 \x03(\x0b\x32*.tinkoff.public.invest.api.contract.v1.Etf\"S\n\x0e\x46utureResponse\x12\x41\n\ninstrument\x18\x01 \x01(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Future\"U\n\x0f\x46uturesResponse\x12\x42\n\x0binstruments\x18\x01 \x03(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Future\"S\n\x0eOptionResponse\x12\x41\n\ninstrument\x18\x01 \x01(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Option\"U\n\x0fOptionsResponse\x12\x42\n\x0binstruments\x18\x01 \x03(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Option\"\xef\x0f\n\x06Option\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x14\n\x0cposition_uid\x18\x02 \x01(\t\x12\x0e\n\x06ticker\x18\x03 \x01(\t\x12\x12\n\nclass_code\x18\x04 \x01(\t\x12 \n\x18\x62\x61sic_asset_position_uid\x18\x05 \x01(\t\x12T\n\x0etrading_status\x18\x15 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12J\n\rreal_exchange\x18\x1f \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12I\n\tdirection\x18) \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.OptionDirection\x12N\n\x0cpayment_type\x18* \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.OptionPaymentType\x12\x41\n\x05style\x18+ \x01(\x0e\x32\x32.tinkoff.public.invest.api.contract.v1.OptionStyle\x12T\n\x0fsettlement_type\x18, \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.OptionSettlementType\x12\x0c\n\x04name\x18\x65 \x01(\t\x12\x10\n\x08\x63urrency\x18o \x01(\t\x12\x1b\n\x13settlement_currency\x18p \x01(\t\x12\x13\n\nasset_type\x18\x83\x01 \x01(\t\x12\x14\n\x0b\x62\x61sic_asset\x18\x84\x01 \x01(\t\x12\x11\n\x08\x65xchange\x18\x8d\x01 \x01(\t\x12\x18\n\x0f\x63ountry_of_risk\x18\x97\x01 \x01(\t\x12\x1d\n\x14\x63ountry_of_risk_name\x18\x98\x01 \x01(\t\x12\x0f\n\x06sector\x18\xa1\x01 \x01(\t\x12@\n\x05\x62rand\x18\xa2\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\x12\x0c\n\x03lot\x18\xc9\x01 \x01(\x05\x12K\n\x10\x62\x61sic_asset_size\x18\xd3\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x05klong\x18\xdd\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x06kshort\x18\xde\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x05\x64long\x18\xdf\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x06\x64short\x18\xe0\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\tdlong_min\x18\xe1\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\ndshort_min\x18\xe2\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12N\n\x13min_price_increment\x18\xe7\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12H\n\x0cstrike_price\x18\xf1\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x34\n\x0f\x65xpiration_date\x18\xad\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x10\x66irst_trade_date\x18\xb7\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x0flast_trade_date\x18\xb8\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x16\x66irst_1min_candle_date\x18\xc1\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x16\x66irst_1day_candle_date\x18\xc2\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x12short_enabled_flag\x18\x91\x03 \x01(\x08\x12\x15\n\x0c\x66or_iis_flag\x18\x92\x03 \x01(\x08\x12\x11\n\x08otc_flag\x18\x93\x03 \x01(\x08\x12\x1b\n\x12\x62uy_available_flag\x18\x94\x03 \x01(\x08\x12\x1c\n\x13sell_available_flag\x18\x95\x03 \x01(\x08\x12\x1f\n\x16\x66or_qual_investor_flag\x18\x96\x03 \x01(\x08\x12\x15\n\x0cweekend_flag\x18\x97\x03 \x01(\x08\x12\x19\n\x10\x62locked_tca_flag\x18\x98\x03 \x01(\x08\x12!\n\x18\x61pi_trade_available_flag\x18\x99\x03 \x01(\x08\"Q\n\rShareResponse\x12@\n\ninstrument\x18\x01 \x01(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Share\"S\n\x0eSharesResponse\x12\x41\n\x0binstruments\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Share\"\x96\x10\n\x04\x42ond\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12 \n\x18\x63oupon_quantity_per_year\x18\x11 \x01(\x05\x12\x31\n\rmaturity_date\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x07nominal\x18\x13 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12J\n\x0finitial_nominal\x18\x14 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x32\n\x0estate_reg_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0eplacement_date\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12J\n\x0fplacement_price\x18\x17 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x44\n\taci_value\x18\x18 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x17\n\x0f\x63ountry_of_risk\x18\x19 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x1a \x01(\t\x12\x0e\n\x06sector\x18\x1b \x01(\t\x12\x12\n\nissue_kind\x18\x1c \x01(\t\x12\x12\n\nissue_size\x18\x1d \x01(\x03\x12\x17\n\x0fissue_size_plan\x18\x1e \x01(\x03\x12T\n\x0etrading_status\x18\x1f \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18  \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18! \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\" \x01(\x08\x12\x1c\n\x14\x66loating_coupon_flag\x18# \x01(\x08\x12\x16\n\x0eperpetual_flag\x18$ \x01(\x08\x12\x19\n\x11\x61mortization_flag\x18% \x01(\x08\x12M\n\x13min_price_increment\x18& \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\' \x01(\x08\x12\x0b\n\x03uid\x18( \x01(\t\x12J\n\rreal_exchange\x18) \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18* \x01(\t\x12\x11\n\tasset_uid\x18+ \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18\x33 \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18\x34 \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x35 \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x36 \x01(\x08\x12\x19\n\x11subordinated_flag\x18\x37 \x01(\x08\x12\x16\n\x0eliquidity_flag\x18\x38 \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18= \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18> \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x44\n\nrisk_level\x18? \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.RiskLevel\x12?\n\x05\x62rand\x18@ \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xec\n\n\x08\x43urrency\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12\x42\n\x07nominal\x18\x11 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x17\n\x0f\x63ountry_of_risk\x18\x12 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x13 \x01(\t\x12T\n\x0etrading_status\x18\x14 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x15 \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x16 \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x17 \x01(\x08\x12\x19\n\x11iso_currency_name\x18\x18 \x01(\t\x12M\n\x13min_price_increment\x18\x19 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x1a \x01(\x08\x12\x0b\n\x03uid\x18\x1b \x01(\t\x12J\n\rreal_exchange\x18\x1c \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18\x1d \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18) \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18\x34 \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x35 \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x36 \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xb6\x0c\n\x03\x45tf\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12J\n\x10\x66ixed_commission\x18\x11 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x12\n\nfocus_type\x18\x12 \x01(\t\x12\x31\n\rreleased_date\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x44\n\nnum_shares\x18\x14 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x17\n\x0f\x63ountry_of_risk\x18\x15 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x16 \x01(\t\x12\x0e\n\x06sector\x18\x17 \x01(\t\x12\x18\n\x10rebalancing_freq\x18\x18 \x01(\t\x12T\n\x0etrading_status\x18\x19 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x1a \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x1b \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x1c \x01(\x08\x12M\n\x13min_price_increment\x18\x1d \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x1e \x01(\x08\x12\x0b\n\x03uid\x18\x1f \x01(\t\x12J\n\rreal_exchange\x18  \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18! \x01(\t\x12\x11\n\tasset_uid\x18\" \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18) \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18* \x01(\x08\x12\x14\n\x0cweekend_flag\x18+ \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18, \x01(\x08\x12\x16\n\x0eliquidity_flag\x18- \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xd5\x0e\n\x06\x46uture\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0b\n\x03lot\x18\x04 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x05 \x01(\t\x12?\n\x05klong\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\x0c \x01(\x08\x12\x0c\n\x04name\x18\r \x01(\t\x12\x10\n\x08\x65xchange\x18\x0e \x01(\t\x12\x34\n\x10\x66irst_trade_date\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_trade_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x66utures_type\x18\x11 \x01(\t\x12\x12\n\nasset_type\x18\x12 \x01(\t\x12\x13\n\x0b\x62\x61sic_asset\x18\x13 \x01(\t\x12J\n\x10\x62\x61sic_asset_size\x18\x14 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x17\n\x0f\x63ountry_of_risk\x18\x15 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x16 \x01(\t\x12\x0e\n\x06sector\x18\x17 \x01(\t\x12\x33\n\x0f\x65xpiration_date\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0etrading_status\x18\x19 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x1a \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x1b \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x1c \x01(\x08\x12M\n\x13min_price_increment\x18\x1d \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x1e \x01(\x08\x12\x0b\n\x03uid\x18\x1f \x01(\t\x12J\n\rreal_exchange\x18  \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18! \x01(\t\x12 \n\x18\x62\x61sic_asset_position_uid\x18\" \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18) \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18* \x01(\x08\x12\x14\n\x0cweekend_flag\x18+ \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18, \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12P\n\x15initial_margin_on_buy\x18= \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x16initial_margin_on_sell\x18> \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12T\n\x1amin_price_increment_amount\x18? \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x62rand\x18@ \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xc2\x0c\n\x05Share\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12,\n\x08ipo_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nissue_size\x18\x12 \x01(\x03\x12\x17\n\x0f\x63ountry_of_risk\x18\x13 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x14 \x01(\t\x12\x0e\n\x06sector\x18\x15 \x01(\t\x12\x17\n\x0fissue_size_plan\x18\x16 \x01(\x03\x12\x42\n\x07nominal\x18\x17 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12T\n\x0etrading_status\x18\x19 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x1a \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x1b \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x1c \x01(\x08\x12\x16\n\x0e\x64iv_yield_flag\x18\x1d \x01(\x08\x12\x44\n\nshare_type\x18\x1e \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.ShareType\x12M\n\x13min_price_increment\x18\x1f \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18  \x01(\x08\x12\x0b\n\x03uid\x18! \x01(\t\x12J\n\rreal_exchange\x18\" \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18# \x01(\t\x12\x11\n\tasset_uid\x18$ \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18. \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18/ \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x30 \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x31 \x01(\x08\x12\x16\n\x0eliquidity_flag\x18\x32 \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xa9\x01\n\x1aGetAccruedInterestsRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12.\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\"p\n\x1bGetAccruedInterestsResponse\x12Q\n\x11\x61\x63\x63rued_interests\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.AccruedInterest\"\x88\x02\n\x0f\x41\x63\x63ruedInterest\x12(\n\x04\x64\x61te\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05value\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12G\n\rvalue_percent\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x07nominal\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"H\n\x17GetFuturesMarginRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\"\xe4\x02\n\x18GetFuturesMarginResponse\x12P\n\x15initial_margin_on_buy\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x16initial_margin_on_sell\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x13min_price_increment\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12T\n\x1amin_price_increment_amount\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"[\n\x12InstrumentResponse\x12\x45\n\ninstrument\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.Instrument\"\x8b\x0b\n\nInstrument\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x10\n\x08\x65xchange\x18\x0f \x01(\t\x12\x17\n\x0f\x63ountry_of_risk\x18\x10 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x11 \x01(\t\x12\x17\n\x0finstrument_type\x18\x12 \x01(\t\x12T\n\x0etrading_status\x18\x13 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x14 \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x15 \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x16 \x01(\x08\x12M\n\x13min_price_increment\x18\x17 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x18 \x01(\x08\x12\x0b\n\x03uid\x18\x19 \x01(\t\x12J\n\rreal_exchange\x18\x1a \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18\x1b \x01(\t\x12\x11\n\tasset_uid\x18\x1c \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18$ \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18% \x01(\x08\x12\x14\n\x0cweekend_flag\x18& \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\' \x01(\x08\x12N\n\x0finstrument_kind\x18( \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xb0\x01\n\x13GetDividendsRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\x42\x07\n\x05_fromB\x05\n\x03_to\"Z\n\x14GetDividendsResponse\x12\x42\n\tdividends\x18\x01 \x03(\x0b\x32/.tinkoff.public.invest.api.contract.v1.Dividend\"\x86\x04\n\x08\x44ividend\x12G\n\x0c\x64ividend_net\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x30\n\x0cpayment_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rdeclared_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rlast_buy_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rdividend_type\x18\x05 \x01(\t\x12/\n\x0brecord_date\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nregularity\x18\x07 \x01(\t\x12\x46\n\x0b\x63lose_price\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x45\n\x0byield_value\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12.\n\ncreated_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\" \n\x0c\x41ssetRequest\x12\x10\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"P\n\rAssetResponse\x12?\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.AssetFull\"x\n\rAssetsRequest\x12S\n\x0finstrument_type\x18\x01 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentTypeH\x00\x88\x01\x01\x42\x12\n\x10_instrument_type\"N\n\x0e\x41ssetsResponse\x12<\n\x06\x61ssets\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Asset\"\x98\x05\n\tAssetFull\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12>\n\x04type\x18\x02 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.AssetType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nname_brief\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12.\n\ndeleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0erequired_tests\x18\x07 \x03(\t\x12H\n\x08\x63urrency\x18\x08 \x01(\x0b\x32\x34.tinkoff.public.invest.api.contract.v1.AssetCurrencyH\x00\x12H\n\x08security\x18\t \x01(\x0b\x32\x34.tinkoff.public.invest.api.contract.v1.AssetSecurityH\x00\x12\x14\n\x0cgos_reg_code\x18\n \x01(\t\x12\x0b\n\x03\x63\x66i\x18\x0b \x01(\t\x12\x10\n\x08\x63ode_nsd\x18\x0c \x01(\t\x12\x0e\n\x06status\x18\r \x01(\t\x12;\n\x05\x62rand\x18\x0e \x01(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Brand\x12.\n\nupdated_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x62r_code\x18\x10 \x01(\t\x12\x14\n\x0c\x62r_code_name\x18\x11 \x01(\t\x12K\n\x0binstruments\x18\x12 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.AssetInstrumentB\x05\n\x03\x65xt\"\xaf\x01\n\x05\x41sset\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12>\n\x04type\x18\x02 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.AssetType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12K\n\x0binstruments\x18\x04 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.AssetInstrument\"&\n\rAssetCurrency\x12\x15\n\rbase_currency\x18\x01 \x01(\t\"\xf6\x03\n\rAssetSecurity\x12\x0c\n\x04isin\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12\x42\n\x05share\x18\x03 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.AssetShareH\x00\x12@\n\x04\x62ond\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.AssetBondH\x00\x12K\n\x02sp\x18\x05 \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.AssetStructuredProductH\x00\x12>\n\x03\x65tf\x18\x06 \x01(\x0b\x32/.tinkoff.public.invest.api.contract.v1.AssetEtfH\x00\x12_\n\x14\x63learing_certificate\x18\x07 \x01(\x0b\x32?.tinkoff.public.invest.api.contract.v1.AssetClearingCertificateH\x00\x42\x05\n\x03\x65xt\"\xd5\x05\n\nAssetShare\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.ShareType\x12\x44\n\nissue_size\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x07nominal\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x04 \x01(\t\x12\x15\n\rprimary_index\x18\x05 \x01(\t\x12G\n\rdividend_rate\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1c\n\x14preferred_share_type\x18\x07 \x01(\t\x12,\n\x08ipo_date\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rregistry_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x64iv_yield_flag\x18\n \x01(\x08\x12\x12\n\nissue_kind\x18\x0b \x01(\t\x12\x32\n\x0eplacement_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brepres_isin\x18\r \x01(\t\x12I\n\x0fissue_size_plan\x18\x0e \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\x0btotal_float\x18\x0f \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xe0\x06\n\tAssetBond\x12I\n\x0f\x63urrent_nominal\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x13\n\x0b\x62orrow_name\x18\x02 \x01(\t\x12\x44\n\nissue_size\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x07nominal\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x05 \x01(\t\x12\x12\n\nissue_kind\x18\x06 \x01(\t\x12\x15\n\rinterest_kind\x18\x07 \x01(\t\x12 \n\x18\x63oupon_quantity_per_year\x18\x08 \x01(\x05\x12\x1c\n\x14indexed_nominal_flag\x18\t \x01(\x08\x12\x19\n\x11subordinated_flag\x18\n \x01(\x08\x12\x17\n\x0f\x63ollateral_flag\x18\x0b \x01(\x08\x12\x15\n\rtax_free_flag\x18\x0c \x01(\x08\x12\x19\n\x11\x61mortization_flag\x18\r \x01(\x08\x12\x1c\n\x14\x66loating_coupon_flag\x18\x0e \x01(\x08\x12\x16\n\x0eperpetual_flag\x18\x0f \x01(\x08\x12\x31\n\rmaturity_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10return_condition\x18\x11 \x01(\t\x12\x32\n\x0estate_reg_date\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0eplacement_date\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x0fplacement_price\x18\x14 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12I\n\x0fissue_size_plan\x18\x15 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xa0\x05\n\x16\x41ssetStructuredProduct\x12\x13\n\x0b\x62orrow_name\x18\x01 \x01(\t\x12\x41\n\x07nominal\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x03 \x01(\t\x12J\n\x04type\x18\x04 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.StructuredProductType\x12\x17\n\x0flogic_portfolio\x18\x05 \x01(\t\x12\x44\n\nasset_type\x18\x06 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.AssetType\x12\x13\n\x0b\x62\x61sic_asset\x18\x07 \x01(\t\x12H\n\x0esafety_barrier\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x31\n\rmaturity_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x0fissue_size_plan\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nissue_size\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x32\n\x0eplacement_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nissue_kind\x18\r \x01(\t\"\xd8\n\n\x08\x41ssetEtf\x12G\n\rtotal_expense\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\x0bhurdle_rate\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12I\n\x0fperformance_fee\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10\x66ixed_commission\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x14\n\x0cpayment_type\x18\x05 \x01(\t\x12\x16\n\x0ewatermark_flag\x18\x06 \x01(\x08\x12\x45\n\x0b\x62uy_premium\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12G\n\rsell_discount\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10rebalancing_flag\x18\t \x01(\x08\x12\x18\n\x10rebalancing_freq\x18\n \x01(\t\x12\x17\n\x0fmanagement_type\x18\x0b \x01(\t\x12\x15\n\rprimary_index\x18\x0c \x01(\t\x12\x12\n\nfocus_type\x18\r \x01(\t\x12\x16\n\x0eleveraged_flag\x18\x0e \x01(\x08\x12\x43\n\tnum_share\x18\x0f \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x12\n\nucits_flag\x18\x10 \x01(\x08\x12\x31\n\rreleased_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x12 \x01(\t\x12!\n\x19primary_index_description\x18\x13 \x01(\t\x12\x1d\n\x15primary_index_company\x18\x14 \x01(\t\x12O\n\x15index_recovery_period\x18\x15 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x11\n\tinav_code\x18\x16 \x01(\t\x12\x16\n\x0e\x64iv_yield_flag\x18\x17 \x01(\x08\x12L\n\x12\x65xpense_commission\x18\x18 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12V\n\x1cprimary_index_tracking_error\x18\x19 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10rebalancing_plan\x18\x1a \x01(\t\x12\x10\n\x08tax_rate\x18\x1b \x01(\t\x12\x35\n\x11rebalancing_dates\x18\x1c \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nissue_kind\x18\x1d \x01(\t\x12\x41\n\x07nominal\x18\x1e \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x1f \x01(\t\"w\n\x18\x41ssetClearingCertificate\x12\x41\n\x07nominal\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x02 \x01(\t\"\x9d\x01\n\x05\x42rand\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04info\x18\x04 \x01(\t\x12\x0f\n\x07\x63ompany\x18\x05 \x01(\t\x12\x0e\n\x06sector\x18\x06 \x01(\t\x12\x17\n\x0f\x63ountry_of_risk\x18\x07 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x08 \x01(\t\"\x95\x02\n\x0f\x41ssetInstrument\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0c\n\x04\x66igi\x18\x02 \x01(\t\x12\x17\n\x0finstrument_type\x18\x03 \x01(\t\x12\x0e\n\x06ticker\x18\x04 \x01(\t\x12\x12\n\nclass_code\x18\x05 \x01(\t\x12\x44\n\x05links\x18\x06 \x03(\x0b\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentLink\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12\x14\n\x0cposition_uid\x18\x0b \x01(\t\"6\n\x0eInstrumentLink\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0einstrument_uid\x18\x02 \x01(\t\"\x15\n\x13GetFavoritesRequest\"o\n\x14GetFavoritesResponse\x12W\n\x14\x66\x61vorite_instruments\x18\x01 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.FavoriteInstrument\"\x8c\x02\n\x12\x46\x61voriteInstrument\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x17\n\x0finstrument_type\x18\x0b \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x0b\n\x03uid\x18\r \x01(\t\x12\x10\n\x08otc_flag\x18\x10 \x01(\x08\x12 \n\x18\x61pi_trade_available_flag\x18\x11 \x01(\x08\x12N\n\x0finstrument_kind\x18\x12 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\"\xd3\x01\n\x14\x45\x64itFavoritesRequest\x12`\n\x0binstruments\x18\x01 \x03(\x0b\x32\x45.tinkoff.public.invest.api.contract.v1.EditFavoritesRequestInstrumentB\x04\xe2\x41\x01\x02\x12Y\n\x0b\x61\x63tion_type\x18\x06 \x01(\x0e\x32>.tinkoff.public.invest.api.contract.v1.EditFavoritesActionTypeB\x04\xe2\x41\x01\x02\"]\n\x1e\x45\x64itFavoritesRequestInstrument\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x42\x07\n\x05_figi\"p\n\x15\x45\x64itFavoritesResponse\x12W\n\x14\x66\x61vorite_instruments\x18\x01 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.FavoriteInstrument\"\x15\n\x13GetCountriesRequest\"a\n\x14GetCountriesResponse\x12I\n\tcountries\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.CountryResponse\"\x14\n\x12IndicativesRequest\"e\n\x13IndicativesResponse\x12N\n\x0binstruments\x18\x01 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.IndicativeResponse\"\x90\x02\n\x12IndicativeResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x10\n\x08\x63urrency\x18\x04 \x01(\t\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08\x65xchange\x18\r \x01(\t\x12\x0b\n\x03uid\x18\x0e \x01(\t\x12\x1b\n\x12\x62uy_available_flag\x18\x94\x03 \x01(\x08\x12\x1c\n\x13sell_available_flag\x18\x95\x03 \x01(\x08\"Y\n\x0f\x43ountryResponse\x12\x10\n\x08\x61lfa_two\x18\x01 \x01(\t\x12\x12\n\nalfa_three\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nname_brief\x18\x04 \x01(\t\"\xd9\x01\n\x15\x46indInstrumentRequest\x12\x13\n\x05query\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12S\n\x0finstrument_kind\x18\x02 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentTypeH\x00\x88\x01\x01\x12%\n\x18\x61pi_trade_available_flag\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x12\n\x10_instrument_kindB\x1b\n\x19_api_trade_available_flag\"e\n\x16\x46indInstrumentResponse\x12K\n\x0binstruments\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.InstrumentShort\"\xeb\x03\n\x0fInstrumentShort\x12\x0c\n\x04isin\x18\x01 \x01(\t\x12\x0c\n\x04\x66igi\x18\x02 \x01(\t\x12\x0e\n\x06ticker\x18\x03 \x01(\t\x12\x12\n\nclass_code\x18\x04 \x01(\t\x12\x17\n\x0finstrument_type\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x0b\n\x03uid\x18\x07 \x01(\t\x12\x14\n\x0cposition_uid\x18\x08 \x01(\t\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12 \n\x18\x61pi_trade_available_flag\x18\x0b \x01(\x08\x12\x14\n\x0c\x66or_iis_flag\x18\x0c \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x1a \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x1b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16\x66or_qual_investor_flag\x18\x1c \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x1d \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x1e \x01(\x08\"O\n\x10GetBrandsRequest\x12;\n\x06paging\x18\x01 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.Page\"#\n\x0fGetBrandRequest\x12\x10\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"\x96\x01\n\x11GetBrandsResponse\x12<\n\x06\x62rands\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Brand\x12\x43\n\x06paging\x18\x02 \x01(\x0b\x32\x33.tinkoff.public.invest.api.contract.v1.PageResponse\"3\n\x1bGetAssetFundamentalsRequest\x12\x14\n\x06\x61ssets\x18\x01 \x03(\tB\x04\xe2\x41\x01\x02\"\xfd\x0e\n\x1cGetAssetFundamentalsResponse\x12k\n\x0c\x66undamentals\x18\x01 \x03(\x0b\x32U.tinkoff.public.invest.api.contract.v1.GetAssetFundamentalsResponse.StatisticResponse\x1a\xef\r\n\x11StatisticResponse\x12\x11\n\tasset_uid\x18\x01 \x01(\t\x12\x10\n\x08\x63urrency\x18\x02 \x01(\t\x12\x1d\n\x15market_capitalization\x18\x03 \x01(\x01\x12 \n\x18high_price_last_52_weeks\x18\x04 \x01(\x01\x12\x1f\n\x17low_price_last_52_weeks\x18\x05 \x01(\x01\x12)\n!average_daily_volume_last_10_days\x18\x06 \x01(\x01\x12)\n!average_daily_volume_last_4_weeks\x18\x07 \x01(\x01\x12\x0c\n\x04\x62\x65ta\x18\x08 \x01(\x01\x12\x12\n\nfree_float\x18\t \x01(\x01\x12%\n\x1d\x66orward_annual_dividend_yield\x18\n \x01(\x01\x12\x1a\n\x12shares_outstanding\x18\x0b \x01(\x01\x12\x13\n\x0brevenue_ttm\x18\x0c \x01(\x01\x12\x12\n\nebitda_ttm\x18\r \x01(\x01\x12\x16\n\x0enet_income_ttm\x18\x0e \x01(\x01\x12\x0f\n\x07\x65ps_ttm\x18\x0f \x01(\x01\x12\x17\n\x0f\x64iluted_eps_ttm\x18\x10 \x01(\x01\x12\x1a\n\x12\x66ree_cash_flow_ttm\x18\x11 \x01(\x01\x12,\n$five_year_annual_revenue_growth_rate\x18\x12 \x01(\x01\x12-\n%three_year_annual_revenue_growth_rate\x18\x13 \x01(\x01\x12\x14\n\x0cpe_ratio_ttm\x18\x14 \x01(\x01\x12\x1a\n\x12price_to_sales_ttm\x18\x15 \x01(\x01\x12\x19\n\x11price_to_book_ttm\x18\x16 \x01(\x01\x12#\n\x1bprice_to_free_cash_flow_ttm\x18\x17 \x01(\x01\x12\"\n\x1atotal_enterprise_value_mrq\x18\x18 \x01(\x01\x12\x18\n\x10\x65v_to_ebitda_mrq\x18\x19 \x01(\x01\x12\x16\n\x0enet_margin_mrq\x18\x1a \x01(\x01\x12\x1f\n\x17net_interest_margin_mrq\x18\x1b \x01(\x01\x12\x0b\n\x03roe\x18\x1c \x01(\x01\x12\x0b\n\x03roa\x18\x1d \x01(\x01\x12\x0c\n\x04roic\x18\x1e \x01(\x01\x12\x16\n\x0etotal_debt_mrq\x18\x1f \x01(\x01\x12 \n\x18total_debt_to_equity_mrq\x18  \x01(\x01\x12 \n\x18total_debt_to_ebitda_mrq\x18! \x01(\x01\x12\x1f\n\x17\x66ree_cash_flow_to_price\x18\" \x01(\x01\x12\x1a\n\x12net_debt_to_ebitda\x18# \x01(\x01\x12\x19\n\x11\x63urrent_ratio_mrq\x18$ \x01(\x01\x12&\n\x1e\x66ixed_charge_coverage_ratio_fy\x18% \x01(\x01\x12 \n\x18\x64ividend_yield_daily_ttm\x18& \x01(\x01\x12\x19\n\x11\x64ividend_rate_ttm\x18\' \x01(\x01\x12\x1b\n\x13\x64ividends_per_share\x18( \x01(\x01\x12)\n!five_years_average_dividend_yield\x18) \x01(\x01\x12-\n%five_year_annual_dividend_growth_rate\x18* \x01(\x01\x12 \n\x18\x64ividend_payout_ratio_fy\x18+ \x01(\x01\x12\x14\n\x0c\x62uy_back_ttm\x18, \x01(\x01\x12+\n#one_year_annual_revenue_growth_rate\x18- \x01(\x01\x12\x1f\n\x17\x64omicile_indicator_code\x18. \x01(\t\x12!\n\x19\x61\x64r_to_common_share_ratio\x18/ \x01(\x01\x12\x1b\n\x13number_of_employees\x18\x30 \x01(\x01\x12\x34\n\x10\x65x_dividend_date\x18\x31 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x18\x66iscal_period_start_date\x18\x32 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66iscal_period_end_date\x18\x33 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x19revenue_change_five_years\x18\x35 \x01(\x01\x12\x1d\n\x15\x65ps_change_five_years\x18\x36 \x01(\x01\x12 \n\x18\x65\x62itda_change_five_years\x18\x37 \x01(\x01\x12$\n\x1ctotal_debt_change_five_years\x18\x38 \x01(\x01\x12\x13\n\x0b\x65v_to_sales\x18\x39 \x01(\x01\"\xa1\x01\n\x16GetAssetReportsRequest\x12\x1b\n\rinstrument_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_to\"\xa7\x04\n\x17GetAssetReportsResponse\x12\x63\n\x06\x65vents\x18\x01 \x03(\x0b\x32S.tinkoff.public.invest.api.contract.v1.GetAssetReportsResponse.GetAssetReportsEvent\x1a\xa2\x02\n\x14GetAssetReportsEvent\x12\x15\n\rinstrument_id\x18\x01 \x01(\t\x12/\n\x0breport_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bperiod_year\x18\x03 \x01(\x05\x12\x12\n\nperiod_num\x18\x04 \x01(\x05\x12i\n\x0bperiod_type\x18\x05 \x01(\x0e\x32T.tinkoff.public.invest.api.contract.v1.GetAssetReportsResponse.AssetReportPeriodType\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x81\x01\n\x15\x41ssetReportPeriodType\x12\x1b\n\x17PERIOD_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13PERIOD_TYPE_QUARTER\x10\x01\x12\x1a\n\x16PERIOD_TYPE_SEMIANNUAL\x10\x02\x12\x16\n\x12PERIOD_TYPE_ANNUAL\x10\x03\"k\n\x1cGetConsensusForecastsRequest\x12@\n\x06paging\x18\x01 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PageH\x00\x88\x01\x01\x42\t\n\x07_paging\"\x86\x06\n\x1dGetConsensusForecastsResponse\x12j\n\x05items\x18\x01 \x03(\x0b\x32[.tinkoff.public.invest.api.contract.v1.GetConsensusForecastsResponse.ConsensusForecastsItem\x12\x41\n\x04page\x18\x02 \x01(\x0b\x32\x33.tinkoff.public.invest.api.contract.v1.PageResponse\x1a\xb5\x04\n\x16\x43onsensusForecastsItem\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x11\n\tasset_uid\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12K\n\x11\x62\x65st_target_price\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12I\n\x0f\x62\x65st_target_low\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10\x62\x65st_target_high\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1b\n\x13total_buy_recommend\x18\x07 \x01(\x05\x12\x1c\n\x14total_hold_recommend\x18\x08 \x01(\x05\x12\x1c\n\x14total_sell_recommend\x18\t \x01(\x05\x12\x10\n\x08\x63urrency\x18\n \x01(\t\x12H\n\tconsensus\x18\x0b \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.Recommendation\x12\x32\n\x0eprognosis_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"+\n\x12GetForecastRequest\x12\x15\n\rinstrument_id\x18\x01 \x01(\t\"\x97\n\n\x13GetForecastResponse\x12V\n\x07targets\x18\x01 \x03(\x0b\x32\x45.tinkoff.public.invest.api.contract.v1.GetForecastResponse.TargetItem\x12[\n\tconsensus\x18\x02 \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetForecastResponse.ConsensusItem\x1a\x8c\x04\n\nTargetItem\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0f\n\x07\x63ompany\x18\x03 \x01(\t\x12M\n\x0erecommendation\x18\x04 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.Recommendation\x12\x37\n\x13recommendation_date\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12G\n\rcurrent_price\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x46\n\x0ctarget_price\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x46\n\x0cprice_change\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10price_change_rel\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x11\n\tshow_name\x18\x0b \x01(\t\x1a\xbb\x04\n\rConsensusItem\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12M\n\x0erecommendation\x18\x03 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.Recommendation\x12\x10\n\x08\x63urrency\x18\x04 \x01(\t\x12G\n\rcurrent_price\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tconsensus\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nmin_target\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nmax_target\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x46\n\x0cprice_change\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10price_change_rel\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xe0\x01\n\x0fTradingInterval\x12\x0c\n\x04type\x18\x01 \x01(\t\x12U\n\x08interval\x18\x02 \x01(\x0b\x32\x43.tinkoff.public.invest.api.contract.v1.TradingInterval.TimeInterval\x1ah\n\x0cTimeInterval\x12,\n\x08start_ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_ts\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp*\xd7\x01\n\nCouponType\x12\x1b\n\x17\x43OUPON_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OUPON_TYPE_CONSTANT\x10\x01\x12\x18\n\x14\x43OUPON_TYPE_FLOATING\x10\x02\x12\x18\n\x14\x43OUPON_TYPE_DISCOUNT\x10\x03\x12\x18\n\x14\x43OUPON_TYPE_MORTGAGE\x10\x04\x12\x13\n\x0f\x43OUPON_TYPE_FIX\x10\x05\x12\x18\n\x14\x43OUPON_TYPE_VARIABLE\x10\x06\x12\x15\n\x11\x43OUPON_TYPE_OTHER\x10\x07*h\n\x0fOptionDirection\x12 \n\x1cOPTION_DIRECTION_UNSPECIFIED\x10\x00\x12\x18\n\x14OPTION_DIRECTION_PUT\x10\x01\x12\x19\n\x15OPTION_DIRECTION_CALL\x10\x02*{\n\x11OptionPaymentType\x12#\n\x1fOPTION_PAYMENT_TYPE_UNSPECIFIED\x10\x00\x12\x1f\n\x1bOPTION_PAYMENT_TYPE_PREMIUM\x10\x01\x12 \n\x1cOPTION_PAYMENT_TYPE_MARGINAL\x10\x02*a\n\x0bOptionStyle\x12\x1c\n\x18OPTION_STYLE_UNSPECIFIED\x10\x00\x12\x19\n\x15OPTION_STYLE_AMERICAN\x10\x01\x12\x19\n\x15OPTION_STYLE_EUROPEAN\x10\x02*\x95\x01\n\x14OptionSettlementType\x12%\n!OPTION_EXECUTION_TYPE_UNSPECIFIED\x10\x00\x12+\n\'OPTION_EXECUTION_TYPE_PHYSICAL_DELIVERY\x10\x01\x12)\n%OPTION_EXECUTION_TYPE_CASH_SETTLEMENT\x10\x02*\xae\x01\n\x10InstrumentIdType\x12\x1d\n\x19INSTRUMENT_ID_UNSPECIFIED\x10\x00\x12\x1b\n\x17INSTRUMENT_ID_TYPE_FIGI\x10\x01\x12\x1d\n\x19INSTRUMENT_ID_TYPE_TICKER\x10\x02\x12\x1a\n\x16INSTRUMENT_ID_TYPE_UID\x10\x03\x12#\n\x1fINSTRUMENT_ID_TYPE_POSITION_UID\x10\x04*l\n\x10InstrumentStatus\x12!\n\x1dINSTRUMENT_STATUS_UNSPECIFIED\x10\x00\x12\x1a\n\x16INSTRUMENT_STATUS_BASE\x10\x01\x12\x19\n\x15INSTRUMENT_STATUS_ALL\x10\x02*\xe5\x01\n\tShareType\x12\x1a\n\x16SHARE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11SHARE_TYPE_COMMON\x10\x01\x12\x18\n\x14SHARE_TYPE_PREFERRED\x10\x02\x12\x12\n\x0eSHARE_TYPE_ADR\x10\x03\x12\x12\n\x0eSHARE_TYPE_GDR\x10\x04\x12\x12\n\x0eSHARE_TYPE_MLP\x10\x05\x12\x1a\n\x16SHARE_TYPE_NY_REG_SHRS\x10\x06\x12\x1e\n\x1aSHARE_TYPE_CLOSED_END_FUND\x10\x07\x12\x13\n\x0fSHARE_TYPE_REIT\x10\x08*\x89\x01\n\tAssetType\x12\x1a\n\x16\x41SSET_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13\x41SSET_TYPE_CURRENCY\x10\x01\x12\x18\n\x14\x41SSET_TYPE_COMMODITY\x10\x02\x12\x14\n\x10\x41SSET_TYPE_INDEX\x10\x03\x12\x17\n\x13\x41SSET_TYPE_SECURITY\x10\x04*f\n\x15StructuredProductType\x12\x17\n\x13SP_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13SP_TYPE_DELIVERABLE\x10\x01\x12\x1b\n\x17SP_TYPE_NON_DELIVERABLE\x10\x02*\x8d\x01\n\x17\x45\x64itFavoritesActionType\x12*\n&EDIT_FAVORITES_ACTION_TYPE_UNSPECIFIED\x10\x00\x12\"\n\x1e\x45\x44IT_FAVORITES_ACTION_TYPE_ADD\x10\x01\x12\"\n\x1e\x45\x44IT_FAVORITES_ACTION_TYPE_DEL\x10\x02*s\n\x0cRealExchange\x12\x1d\n\x19REAL_EXCHANGE_UNSPECIFIED\x10\x00\x12\x16\n\x12REAL_EXCHANGE_MOEX\x10\x01\x12\x15\n\x11REAL_EXCHANGE_RTS\x10\x02\x12\x15\n\x11REAL_EXCHANGE_OTC\x10\x03*z\n\x0eRecommendation\x12\x1e\n\x1aRECOMMENDATION_UNSPECIFIED\x10\x00\x12\x16\n\x12RECOMMENDATION_BUY\x10\x01\x12\x17\n\x13RECOMMENDATION_HOLD\x10\x02\x12\x17\n\x13RECOMMENDATION_SELL\x10\x03*i\n\tRiskLevel\x12\x1a\n\x16RISK_LEVEL_UNSPECIFIED\x10\x00\x12\x12\n\x0eRISK_LEVEL_LOW\x10\x01\x12\x17\n\x13RISK_LEVEL_MODERATE\x10\x02\x12\x13\n\x0fRISK_LEVEL_HIGH\x10\x03\x32\xef\"\n\x12InstrumentsService\x12\x93\x01\n\x10TradingSchedules\x12>.tinkoff.public.invest.api.contract.v1.TradingSchedulesRequest\x1a?.tinkoff.public.invest.api.contract.v1.TradingSchedulesResponse\x12w\n\x06\x42ondBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x33.tinkoff.public.invest.api.contract.v1.BondResponse\x12x\n\x05\x42onds\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x34.tinkoff.public.invest.api.contract.v1.BondsResponse\x12\x8d\x01\n\x0eGetBondCoupons\x12<.tinkoff.public.invest.api.contract.v1.GetBondCouponsRequest\x1a=.tinkoff.public.invest.api.contract.v1.GetBondCouponsResponse\x12\x8a\x01\n\rGetBondEvents\x12;.tinkoff.public.invest.api.contract.v1.GetBondEventsRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetBondEventsResponse\x12\x7f\n\nCurrencyBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x37.tinkoff.public.invest.api.contract.v1.CurrencyResponse\x12\x82\x01\n\nCurrencies\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.CurrenciesResponse\x12u\n\x05\x45tfBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x32.tinkoff.public.invest.api.contract.v1.EtfResponse\x12v\n\x04\x45tfs\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x33.tinkoff.public.invest.api.contract.v1.EtfsResponse\x12{\n\x08\x46utureBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.FutureResponse\x12|\n\x07\x46utures\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x36.tinkoff.public.invest.api.contract.v1.FuturesResponse\x12{\n\x08OptionBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.OptionResponse\x12\x81\x01\n\x07Options\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x36.tinkoff.public.invest.api.contract.v1.OptionsResponse\"\x03\x88\x02\x01\x12\x80\x01\n\tOptionsBy\x12;.tinkoff.public.invest.api.contract.v1.FilterOptionsRequest\x1a\x36.tinkoff.public.invest.api.contract.v1.OptionsResponse\x12y\n\x07ShareBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x34.tinkoff.public.invest.api.contract.v1.ShareResponse\x12z\n\x06Shares\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.SharesResponse\x12\x84\x01\n\x0bIndicatives\x12\x39.tinkoff.public.invest.api.contract.v1.IndicativesRequest\x1a:.tinkoff.public.invest.api.contract.v1.IndicativesResponse\x12\x9c\x01\n\x13GetAccruedInterests\x12\x41.tinkoff.public.invest.api.contract.v1.GetAccruedInterestsRequest\x1a\x42.tinkoff.public.invest.api.contract.v1.GetAccruedInterestsResponse\x12\x93\x01\n\x10GetFuturesMargin\x12>.tinkoff.public.invest.api.contract.v1.GetFuturesMarginRequest\x1a?.tinkoff.public.invest.api.contract.v1.GetFuturesMarginResponse\x12\x86\x01\n\x0fGetInstrumentBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.InstrumentResponse\x12\x87\x01\n\x0cGetDividends\x12:.tinkoff.public.invest.api.contract.v1.GetDividendsRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetDividendsResponse\x12w\n\nGetAssetBy\x12\x33.tinkoff.public.invest.api.contract.v1.AssetRequest\x1a\x34.tinkoff.public.invest.api.contract.v1.AssetResponse\x12x\n\tGetAssets\x12\x34.tinkoff.public.invest.api.contract.v1.AssetsRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.AssetsResponse\x12\x87\x01\n\x0cGetFavorites\x12:.tinkoff.public.invest.api.contract.v1.GetFavoritesRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetFavoritesResponse\x12\x8a\x01\n\rEditFavorites\x12;.tinkoff.public.invest.api.contract.v1.EditFavoritesRequest\x1a<.tinkoff.public.invest.api.contract.v1.EditFavoritesResponse\x12\x87\x01\n\x0cGetCountries\x12:.tinkoff.public.invest.api.contract.v1.GetCountriesRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetCountriesResponse\x12\x8d\x01\n\x0e\x46indInstrument\x12<.tinkoff.public.invest.api.contract.v1.FindInstrumentRequest\x1a=.tinkoff.public.invest.api.contract.v1.FindInstrumentResponse\x12~\n\tGetBrands\x12\x37.tinkoff.public.invest.api.contract.v1.GetBrandsRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.GetBrandsResponse\x12r\n\nGetBrandBy\x12\x36.tinkoff.public.invest.api.contract.v1.GetBrandRequest\x1a,.tinkoff.public.invest.api.contract.v1.Brand\x12\x9f\x01\n\x14GetAssetFundamentals\x12\x42.tinkoff.public.invest.api.contract.v1.GetAssetFundamentalsRequest\x1a\x43.tinkoff.public.invest.api.contract.v1.GetAssetFundamentalsResponse\x12\x90\x01\n\x0fGetAssetReports\x12=.tinkoff.public.invest.api.contract.v1.GetAssetReportsRequest\x1a>.tinkoff.public.invest.api.contract.v1.GetAssetReportsResponse\x12\xa2\x01\n\x15GetConsensusForecasts\x12\x43.tinkoff.public.invest.api.contract.v1.GetConsensusForecastsRequest\x1a\x44.tinkoff.public.invest.api.contract.v1.GetConsensusForecastsResponse\x12\x86\x01\n\rGetForecastBy\x12\x39.tinkoff.public.invest.api.contract.v1.GetForecastRequest\x1a:.tinkoff.public.invest.api.contract.v1.GetForecastResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%tinkoff/invest/grpc/instruments.proto\x12%tinkoff.public.invest.api.contract.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a tinkoff/invest/grpc/common.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"\xa9\x01\n\x17TradingSchedulesRequest\x12\x15\n\x08\x65xchange\x18\x01 \x01(\tH\x00\x88\x01\x01\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x42\x0b\n\t_exchangeB\x07\n\x05_fromB\x05\n\x03_to\"e\n\x18TradingSchedulesResponse\x12I\n\texchanges\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.TradingSchedule\"d\n\x0fTradingSchedule\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12?\n\x04\x64\x61ys\x18\x02 \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.TradingDay\"\x97\x07\n\nTradingDay\x12(\n\x04\x64\x61te\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0eis_trading_day\x18\x02 \x01(\x08\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x1aopening_auction_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x18\x63losing_auction_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x46\n\"evening_opening_auction_start_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12\x65vening_start_time\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x65vening_end_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13\x63learing_start_time\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11\x63learing_end_time\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14premarket_start_time\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12premarket_end_time\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x1a\x63losing_auction_start_time\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x18opening_auction_end_time\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\tintervals\x18\x12 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.TradingIntervalJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"\x9d\x01\n\x11InstrumentRequest\x12N\n\x07id_type\x18\x01 \x01(\x0e\x32\x37.tinkoff.public.invest.api.contract.v1.InstrumentIdTypeB\x04\xe2\x41\x01\x02\x12\x17\n\nclass_code\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x02id\x18\x03 \x01(\tB\x04\xe2\x41\x01\x02\x42\r\n\x0b_class_code\"\xfc\x01\n\x12InstrumentsRequest\x12W\n\x11instrument_status\x18\x01 \x01(\x0e\x32\x37.tinkoff.public.invest.api.contract.v1.InstrumentStatusH\x00\x88\x01\x01\x12_\n\x13instrument_exchange\x18\x02 \x01(\x0e\x32=.tinkoff.public.invest.api.contract.v1.InstrumentExchangeTypeH\x01\x88\x01\x01\x42\x14\n\x12_instrument_statusB\x16\n\x14_instrument_exchange\"\x8c\x01\n\x14\x46ilterOptionsRequest\x12\x1c\n\x0f\x62\x61sic_asset_uid\x18\x01 \x01(\tH\x00\x88\x01\x01\x12%\n\x18\x62\x61sic_asset_position_uid\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x12\n\x10_basic_asset_uidB\x1b\n\x19_basic_asset_position_uid\"O\n\x0c\x42ondResponse\x12?\n\ninstrument\x18\x01 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.Bond\"Q\n\rBondsResponse\x12@\n\x0binstruments\x18\x01 \x03(\x0b\x32+.tinkoff.public.invest.api.contract.v1.Bond\"\xb2\x01\n\x15GetBondCouponsRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\x42\x07\n\x05_fromB\x05\n\x03_to\"W\n\x16GetBondCouponsResponse\x12=\n\x06\x65vents\x18\x01 \x03(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Coupon\"\xef\x02\n\x14GetBondEventsRequest\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\x12S\n\x04type\x18\x05 \x01(\x0e\x32\x45.tinkoff.public.invest.api.contract.v1.GetBondEventsRequest.EventType\"y\n\tEventType\x12\x1a\n\x16\x45VENT_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x45VENT_TYPE_CPN\x10\x01\x12\x13\n\x0f\x45VENT_TYPE_CALL\x10\x02\x12\x12\n\x0e\x45VENT_TYPE_MTY\x10\x03\x12\x13\n\x0f\x45VENT_TYPE_CONV\x10\x04\x42\x07\n\x05_fromB\x05\n\x03_to\"\xf1\x08\n\x15GetBondEventsResponse\x12V\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x46.tinkoff.public.invest.api.contract.v1.GetBondEventsResponse.BondEvent\x1a\xff\x07\n\tBondEvent\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\x12\x14\n\x0c\x65vent_number\x18\x03 \x01(\x05\x12.\n\nevent_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12Y\n\nevent_type\x18\x05 \x01(\x0e\x32\x45.tinkoff.public.invest.api.contract.v1.GetBondEventsRequest.EventType\x12I\n\x0f\x65vent_total_vol\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12,\n\x08\x66ix_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\trate_date\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x64\x65\x66\x61ult_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rreal_pay_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08pay_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12G\n\x0cpay_one_bond\x18\x0c \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12I\n\x0emoney_flow_val\x18\r \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x11\n\texecution\x18\x0e \x01(\t\x12\x16\n\x0eoperation_type\x18\x0f \x01(\t\x12?\n\x05value\x18\x10 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x0c\n\x04note\x18\x11 \x01(\t\x12\x1e\n\x16\x63onvert_to_fin_tool_id\x18\x12 \x01(\t\x12\x35\n\x11\x63oupon_start_date\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63oupon_end_date\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rcoupon_period\x18\x15 \x01(\x05\x12N\n\x14\x63oupon_interest_rate\x18\x16 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xa0\x03\n\x06\x43oupon\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12/\n\x0b\x63oupon_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rcoupon_number\x18\x03 \x01(\x03\x12,\n\x08\x66ix_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12G\n\x0cpay_one_bond\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x46\n\x0b\x63oupon_type\x18\x06 \x01(\x0e\x32\x31.tinkoff.public.invest.api.contract.v1.CouponType\x12\x35\n\x11\x63oupon_start_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63oupon_end_date\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rcoupon_period\x18\t \x01(\x05\"W\n\x10\x43urrencyResponse\x12\x43\n\ninstrument\x18\x01 \x01(\x0b\x32/.tinkoff.public.invest.api.contract.v1.Currency\"Z\n\x12\x43urrenciesResponse\x12\x44\n\x0binstruments\x18\x01 \x03(\x0b\x32/.tinkoff.public.invest.api.contract.v1.Currency\"M\n\x0b\x45tfResponse\x12>\n\ninstrument\x18\x01 \x01(\x0b\x32*.tinkoff.public.invest.api.contract.v1.Etf\"O\n\x0c\x45tfsResponse\x12?\n\x0binstruments\x18\x01 \x03(\x0b\x32*.tinkoff.public.invest.api.contract.v1.Etf\"S\n\x0e\x46utureResponse\x12\x41\n\ninstrument\x18\x01 \x01(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Future\"U\n\x0f\x46uturesResponse\x12\x42\n\x0binstruments\x18\x01 \x03(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Future\"S\n\x0eOptionResponse\x12\x41\n\ninstrument\x18\x01 \x01(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Option\"U\n\x0fOptionsResponse\x12\x42\n\x0binstruments\x18\x01 \x03(\x0b\x32-.tinkoff.public.invest.api.contract.v1.Option\"\xef\x0f\n\x06Option\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x14\n\x0cposition_uid\x18\x02 \x01(\t\x12\x0e\n\x06ticker\x18\x03 \x01(\t\x12\x12\n\nclass_code\x18\x04 \x01(\t\x12 \n\x18\x62\x61sic_asset_position_uid\x18\x05 \x01(\t\x12T\n\x0etrading_status\x18\x15 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12J\n\rreal_exchange\x18\x1f \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12I\n\tdirection\x18) \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.OptionDirection\x12N\n\x0cpayment_type\x18* \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.OptionPaymentType\x12\x41\n\x05style\x18+ \x01(\x0e\x32\x32.tinkoff.public.invest.api.contract.v1.OptionStyle\x12T\n\x0fsettlement_type\x18, \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.OptionSettlementType\x12\x0c\n\x04name\x18\x65 \x01(\t\x12\x10\n\x08\x63urrency\x18o \x01(\t\x12\x1b\n\x13settlement_currency\x18p \x01(\t\x12\x13\n\nasset_type\x18\x83\x01 \x01(\t\x12\x14\n\x0b\x62\x61sic_asset\x18\x84\x01 \x01(\t\x12\x11\n\x08\x65xchange\x18\x8d\x01 \x01(\t\x12\x18\n\x0f\x63ountry_of_risk\x18\x97\x01 \x01(\t\x12\x1d\n\x14\x63ountry_of_risk_name\x18\x98\x01 \x01(\t\x12\x0f\n\x06sector\x18\xa1\x01 \x01(\t\x12@\n\x05\x62rand\x18\xa2\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\x12\x0c\n\x03lot\x18\xc9\x01 \x01(\x05\x12K\n\x10\x62\x61sic_asset_size\x18\xd3\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x05klong\x18\xdd\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x06kshort\x18\xde\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x05\x64long\x18\xdf\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x06\x64short\x18\xe0\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\tdlong_min\x18\xe1\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\ndshort_min\x18\xe2\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12N\n\x13min_price_increment\x18\xe7\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12H\n\x0cstrike_price\x18\xf1\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x34\n\x0f\x65xpiration_date\x18\xad\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x10\x66irst_trade_date\x18\xb7\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x0flast_trade_date\x18\xb8\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x16\x66irst_1min_candle_date\x18\xc1\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x16\x66irst_1day_candle_date\x18\xc2\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x12short_enabled_flag\x18\x91\x03 \x01(\x08\x12\x15\n\x0c\x66or_iis_flag\x18\x92\x03 \x01(\x08\x12\x11\n\x08otc_flag\x18\x93\x03 \x01(\x08\x12\x1b\n\x12\x62uy_available_flag\x18\x94\x03 \x01(\x08\x12\x1c\n\x13sell_available_flag\x18\x95\x03 \x01(\x08\x12\x1f\n\x16\x66or_qual_investor_flag\x18\x96\x03 \x01(\x08\x12\x15\n\x0cweekend_flag\x18\x97\x03 \x01(\x08\x12\x19\n\x10\x62locked_tca_flag\x18\x98\x03 \x01(\x08\x12!\n\x18\x61pi_trade_available_flag\x18\x99\x03 \x01(\x08\"Q\n\rShareResponse\x12@\n\ninstrument\x18\x01 \x01(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Share\"S\n\x0eSharesResponse\x12\x41\n\x0binstruments\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Share\"\xda\x10\n\x04\x42ond\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12 \n\x18\x63oupon_quantity_per_year\x18\x11 \x01(\x05\x12\x31\n\rmaturity_date\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x07nominal\x18\x13 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12J\n\x0finitial_nominal\x18\x14 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x32\n\x0estate_reg_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0eplacement_date\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12J\n\x0fplacement_price\x18\x17 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x44\n\taci_value\x18\x18 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x17\n\x0f\x63ountry_of_risk\x18\x19 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x1a \x01(\t\x12\x0e\n\x06sector\x18\x1b \x01(\t\x12\x12\n\nissue_kind\x18\x1c \x01(\t\x12\x12\n\nissue_size\x18\x1d \x01(\x03\x12\x17\n\x0fissue_size_plan\x18\x1e \x01(\x03\x12T\n\x0etrading_status\x18\x1f \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18  \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18! \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\" \x01(\x08\x12\x1c\n\x14\x66loating_coupon_flag\x18# \x01(\x08\x12\x16\n\x0eperpetual_flag\x18$ \x01(\x08\x12\x19\n\x11\x61mortization_flag\x18% \x01(\x08\x12M\n\x13min_price_increment\x18& \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\' \x01(\x08\x12\x0b\n\x03uid\x18( \x01(\t\x12J\n\rreal_exchange\x18) \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18* \x01(\t\x12\x11\n\tasset_uid\x18+ \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18\x33 \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18\x34 \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x35 \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x36 \x01(\x08\x12\x19\n\x11subordinated_flag\x18\x37 \x01(\x08\x12\x16\n\x0eliquidity_flag\x18\x38 \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18= \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18> \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x44\n\nrisk_level\x18? \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.RiskLevel\x12?\n\x05\x62rand\x18@ \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\x12\x42\n\tbond_type\x18\x41 \x01(\x0e\x32/.tinkoff.public.invest.api.contract.v1.BondType\"\xec\n\n\x08\x43urrency\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12\x42\n\x07nominal\x18\x11 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x17\n\x0f\x63ountry_of_risk\x18\x12 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x13 \x01(\t\x12T\n\x0etrading_status\x18\x14 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x15 \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x16 \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x17 \x01(\x08\x12\x19\n\x11iso_currency_name\x18\x18 \x01(\t\x12M\n\x13min_price_increment\x18\x19 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x1a \x01(\x08\x12\x0b\n\x03uid\x18\x1b \x01(\t\x12J\n\rreal_exchange\x18\x1c \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18\x1d \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18) \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18\x34 \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x35 \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x36 \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\x92\r\n\x03\x45tf\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12J\n\x10\x66ixed_commission\x18\x11 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x12\n\nfocus_type\x18\x12 \x01(\t\x12\x31\n\rreleased_date\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x44\n\nnum_shares\x18\x14 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x17\n\x0f\x63ountry_of_risk\x18\x15 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x16 \x01(\t\x12\x0e\n\x06sector\x18\x17 \x01(\t\x12\x18\n\x10rebalancing_freq\x18\x18 \x01(\t\x12T\n\x0etrading_status\x18\x19 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x1a \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x1b \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x1c \x01(\x08\x12M\n\x13min_price_increment\x18\x1d \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x1e \x01(\x08\x12\x0b\n\x03uid\x18\x1f \x01(\t\x12J\n\rreal_exchange\x18  \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18! \x01(\t\x12\x11\n\tasset_uid\x18\" \x01(\t\x12Z\n\x13instrument_exchange\x18# \x01(\x0e\x32=.tinkoff.public.invest.api.contract.v1.InstrumentExchangeType\x12\x14\n\x0c\x66or_iis_flag\x18) \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18* \x01(\x08\x12\x14\n\x0cweekend_flag\x18+ \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18, \x01(\x08\x12\x16\n\x0eliquidity_flag\x18- \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xd5\x0e\n\x06\x46uture\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0b\n\x03lot\x18\x04 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x05 \x01(\t\x12?\n\x05klong\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\x0c \x01(\x08\x12\x0c\n\x04name\x18\r \x01(\t\x12\x10\n\x08\x65xchange\x18\x0e \x01(\t\x12\x34\n\x10\x66irst_trade_date\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flast_trade_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x66utures_type\x18\x11 \x01(\t\x12\x12\n\nasset_type\x18\x12 \x01(\t\x12\x13\n\x0b\x62\x61sic_asset\x18\x13 \x01(\t\x12J\n\x10\x62\x61sic_asset_size\x18\x14 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x17\n\x0f\x63ountry_of_risk\x18\x15 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x16 \x01(\t\x12\x0e\n\x06sector\x18\x17 \x01(\t\x12\x33\n\x0f\x65xpiration_date\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0etrading_status\x18\x19 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x1a \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x1b \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x1c \x01(\x08\x12M\n\x13min_price_increment\x18\x1d \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x1e \x01(\x08\x12\x0b\n\x03uid\x18\x1f \x01(\t\x12J\n\rreal_exchange\x18  \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18! \x01(\t\x12 \n\x18\x62\x61sic_asset_position_uid\x18\" \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18) \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18* \x01(\x08\x12\x14\n\x0cweekend_flag\x18+ \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18, \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12P\n\x15initial_margin_on_buy\x18= \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x16initial_margin_on_sell\x18> \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12T\n\x1amin_price_increment_amount\x18? \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x62rand\x18@ \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\x9e\r\n\x05Share\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x10\n\x08\x65xchange\x18\x10 \x01(\t\x12,\n\x08ipo_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nissue_size\x18\x12 \x01(\x03\x12\x17\n\x0f\x63ountry_of_risk\x18\x13 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x14 \x01(\t\x12\x0e\n\x06sector\x18\x15 \x01(\t\x12\x17\n\x0fissue_size_plan\x18\x16 \x01(\x03\x12\x42\n\x07nominal\x18\x17 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12T\n\x0etrading_status\x18\x19 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x1a \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x1b \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x1c \x01(\x08\x12\x16\n\x0e\x64iv_yield_flag\x18\x1d \x01(\x08\x12\x44\n\nshare_type\x18\x1e \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.ShareType\x12M\n\x13min_price_increment\x18\x1f \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18  \x01(\x08\x12\x0b\n\x03uid\x18! \x01(\t\x12J\n\rreal_exchange\x18\" \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18# \x01(\t\x12\x11\n\tasset_uid\x18$ \x01(\t\x12Z\n\x13instrument_exchange\x18% \x01(\x0e\x32=.tinkoff.public.invest.api.contract.v1.InstrumentExchangeType\x12\x14\n\x0c\x66or_iis_flag\x18. \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18/ \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x30 \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x31 \x01(\x08\x12\x16\n\x0eliquidity_flag\x18\x32 \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xa9\x01\n\x1aGetAccruedInterestsRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12.\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\"p\n\x1bGetAccruedInterestsResponse\x12Q\n\x11\x61\x63\x63rued_interests\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.AccruedInterest\"\x88\x02\n\x0f\x41\x63\x63ruedInterest\x12(\n\x04\x64\x61te\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05value\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12G\n\rvalue_percent\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x07nominal\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"H\n\x17GetFuturesMarginRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\"\xe4\x02\n\x18GetFuturesMarginResponse\x12P\n\x15initial_margin_on_buy\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x16initial_margin_on_sell\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x13min_price_increment\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12T\n\x1amin_price_increment_amount\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"[\n\x12InstrumentResponse\x12\x45\n\ninstrument\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.Instrument\"\x8b\x0b\n\nInstrument\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x0b\n\x03lot\x18\x05 \x01(\x05\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12?\n\x05klong\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06kshort\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x64long\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12@\n\x06\x64short\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tdlong_min\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\ndshort_min\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1a\n\x12short_enabled_flag\x18\r \x01(\x08\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x10\n\x08\x65xchange\x18\x0f \x01(\t\x12\x17\n\x0f\x63ountry_of_risk\x18\x10 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x11 \x01(\t\x12\x17\n\x0finstrument_type\x18\x12 \x01(\t\x12T\n\x0etrading_status\x18\x13 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\x10\n\x08otc_flag\x18\x14 \x01(\x08\x12\x1a\n\x12\x62uy_available_flag\x18\x15 \x01(\x08\x12\x1b\n\x13sell_available_flag\x18\x16 \x01(\x08\x12M\n\x13min_price_increment\x18\x17 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12 \n\x18\x61pi_trade_available_flag\x18\x18 \x01(\x08\x12\x0b\n\x03uid\x18\x19 \x01(\t\x12J\n\rreal_exchange\x18\x1a \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.RealExchange\x12\x14\n\x0cposition_uid\x18\x1b \x01(\t\x12\x11\n\tasset_uid\x18\x1c \x01(\t\x12\x14\n\x0c\x66or_iis_flag\x18$ \x01(\x08\x12\x1e\n\x16\x66or_qual_investor_flag\x18% \x01(\x08\x12\x14\n\x0cweekend_flag\x18& \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\' \x01(\x08\x12N\n\x0finstrument_kind\x18( \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12:\n\x16\x66irst_1min_candle_date\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x39 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05\x62rand\x18< \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.BrandData\"\xb0\x01\n\x13GetDividendsRequest\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x04 \x01(\tB\x04\xe2\x41\x01\x02\x42\x07\n\x05_fromB\x05\n\x03_to\"Z\n\x14GetDividendsResponse\x12\x42\n\tdividends\x18\x01 \x03(\x0b\x32/.tinkoff.public.invest.api.contract.v1.Dividend\"\x86\x04\n\x08\x44ividend\x12G\n\x0c\x64ividend_net\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x30\n\x0cpayment_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rdeclared_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rlast_buy_date\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rdividend_type\x18\x05 \x01(\t\x12/\n\x0brecord_date\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nregularity\x18\x07 \x01(\t\x12\x46\n\x0b\x63lose_price\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x45\n\x0byield_value\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12.\n\ncreated_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\" \n\x0c\x41ssetRequest\x12\x10\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"P\n\rAssetResponse\x12?\n\x05\x61sset\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.AssetFull\"x\n\rAssetsRequest\x12S\n\x0finstrument_type\x18\x01 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentTypeH\x00\x88\x01\x01\x42\x12\n\x10_instrument_type\"N\n\x0e\x41ssetsResponse\x12<\n\x06\x61ssets\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Asset\"\x98\x05\n\tAssetFull\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12>\n\x04type\x18\x02 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.AssetType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nname_brief\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12.\n\ndeleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0erequired_tests\x18\x07 \x03(\t\x12H\n\x08\x63urrency\x18\x08 \x01(\x0b\x32\x34.tinkoff.public.invest.api.contract.v1.AssetCurrencyH\x00\x12H\n\x08security\x18\t \x01(\x0b\x32\x34.tinkoff.public.invest.api.contract.v1.AssetSecurityH\x00\x12\x14\n\x0cgos_reg_code\x18\n \x01(\t\x12\x0b\n\x03\x63\x66i\x18\x0b \x01(\t\x12\x10\n\x08\x63ode_nsd\x18\x0c \x01(\t\x12\x0e\n\x06status\x18\r \x01(\t\x12;\n\x05\x62rand\x18\x0e \x01(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Brand\x12.\n\nupdated_at\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x62r_code\x18\x10 \x01(\t\x12\x14\n\x0c\x62r_code_name\x18\x11 \x01(\t\x12K\n\x0binstruments\x18\x12 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.AssetInstrumentB\x05\n\x03\x65xt\"\xaf\x01\n\x05\x41sset\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12>\n\x04type\x18\x02 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.AssetType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12K\n\x0binstruments\x18\x04 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.AssetInstrument\"&\n\rAssetCurrency\x12\x15\n\rbase_currency\x18\x01 \x01(\t\"\xf6\x03\n\rAssetSecurity\x12\x0c\n\x04isin\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12\x42\n\x05share\x18\x03 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.AssetShareH\x00\x12@\n\x04\x62ond\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.AssetBondH\x00\x12K\n\x02sp\x18\x05 \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.AssetStructuredProductH\x00\x12>\n\x03\x65tf\x18\x06 \x01(\x0b\x32/.tinkoff.public.invest.api.contract.v1.AssetEtfH\x00\x12_\n\x14\x63learing_certificate\x18\x07 \x01(\x0b\x32?.tinkoff.public.invest.api.contract.v1.AssetClearingCertificateH\x00\x42\x05\n\x03\x65xt\"\xd5\x05\n\nAssetShare\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.ShareType\x12\x44\n\nissue_size\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x07nominal\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x04 \x01(\t\x12\x15\n\rprimary_index\x18\x05 \x01(\t\x12G\n\rdividend_rate\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1c\n\x14preferred_share_type\x18\x07 \x01(\t\x12,\n\x08ipo_date\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rregistry_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x64iv_yield_flag\x18\n \x01(\x08\x12\x12\n\nissue_kind\x18\x0b \x01(\t\x12\x32\n\x0eplacement_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brepres_isin\x18\r \x01(\t\x12I\n\x0fissue_size_plan\x18\x0e \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\x0btotal_float\x18\x0f \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xe0\x06\n\tAssetBond\x12I\n\x0f\x63urrent_nominal\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x13\n\x0b\x62orrow_name\x18\x02 \x01(\t\x12\x44\n\nissue_size\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x41\n\x07nominal\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x05 \x01(\t\x12\x12\n\nissue_kind\x18\x06 \x01(\t\x12\x15\n\rinterest_kind\x18\x07 \x01(\t\x12 \n\x18\x63oupon_quantity_per_year\x18\x08 \x01(\x05\x12\x1c\n\x14indexed_nominal_flag\x18\t \x01(\x08\x12\x19\n\x11subordinated_flag\x18\n \x01(\x08\x12\x17\n\x0f\x63ollateral_flag\x18\x0b \x01(\x08\x12\x15\n\rtax_free_flag\x18\x0c \x01(\x08\x12\x19\n\x11\x61mortization_flag\x18\r \x01(\x08\x12\x1c\n\x14\x66loating_coupon_flag\x18\x0e \x01(\x08\x12\x16\n\x0eperpetual_flag\x18\x0f \x01(\x08\x12\x31\n\rmaturity_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10return_condition\x18\x11 \x01(\t\x12\x32\n\x0estate_reg_date\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0eplacement_date\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x0fplacement_price\x18\x14 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12I\n\x0fissue_size_plan\x18\x15 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xa0\x05\n\x16\x41ssetStructuredProduct\x12\x13\n\x0b\x62orrow_name\x18\x01 \x01(\t\x12\x41\n\x07nominal\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x03 \x01(\t\x12J\n\x04type\x18\x04 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.StructuredProductType\x12\x17\n\x0flogic_portfolio\x18\x05 \x01(\t\x12\x44\n\nasset_type\x18\x06 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.AssetType\x12\x13\n\x0b\x62\x61sic_asset\x18\x07 \x01(\t\x12H\n\x0esafety_barrier\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x31\n\rmaturity_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x0fissue_size_plan\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nissue_size\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x32\n\x0eplacement_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nissue_kind\x18\r \x01(\t\"\xd8\n\n\x08\x41ssetEtf\x12G\n\rtotal_expense\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\x0bhurdle_rate\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12I\n\x0fperformance_fee\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10\x66ixed_commission\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x14\n\x0cpayment_type\x18\x05 \x01(\t\x12\x16\n\x0ewatermark_flag\x18\x06 \x01(\x08\x12\x45\n\x0b\x62uy_premium\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12G\n\rsell_discount\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10rebalancing_flag\x18\t \x01(\x08\x12\x18\n\x10rebalancing_freq\x18\n \x01(\t\x12\x17\n\x0fmanagement_type\x18\x0b \x01(\t\x12\x15\n\rprimary_index\x18\x0c \x01(\t\x12\x12\n\nfocus_type\x18\r \x01(\t\x12\x16\n\x0eleveraged_flag\x18\x0e \x01(\x08\x12\x43\n\tnum_share\x18\x0f \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x12\n\nucits_flag\x18\x10 \x01(\x08\x12\x31\n\rreleased_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x64\x65scription\x18\x12 \x01(\t\x12!\n\x19primary_index_description\x18\x13 \x01(\t\x12\x1d\n\x15primary_index_company\x18\x14 \x01(\t\x12O\n\x15index_recovery_period\x18\x15 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x11\n\tinav_code\x18\x16 \x01(\t\x12\x16\n\x0e\x64iv_yield_flag\x18\x17 \x01(\x08\x12L\n\x12\x65xpense_commission\x18\x18 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12V\n\x1cprimary_index_tracking_error\x18\x19 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10rebalancing_plan\x18\x1a \x01(\t\x12\x10\n\x08tax_rate\x18\x1b \x01(\t\x12\x35\n\x11rebalancing_dates\x18\x1c \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nissue_kind\x18\x1d \x01(\t\x12\x41\n\x07nominal\x18\x1e \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x1f \x01(\t\"w\n\x18\x41ssetClearingCertificate\x12\x41\n\x07nominal\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x18\n\x10nominal_currency\x18\x02 \x01(\t\"\x9d\x01\n\x05\x42rand\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04info\x18\x04 \x01(\t\x12\x0f\n\x07\x63ompany\x18\x05 \x01(\t\x12\x0e\n\x06sector\x18\x06 \x01(\t\x12\x17\n\x0f\x63ountry_of_risk\x18\x07 \x01(\t\x12\x1c\n\x14\x63ountry_of_risk_name\x18\x08 \x01(\t\"\x95\x02\n\x0f\x41ssetInstrument\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0c\n\x04\x66igi\x18\x02 \x01(\t\x12\x17\n\x0finstrument_type\x18\x03 \x01(\t\x12\x0e\n\x06ticker\x18\x04 \x01(\t\x12\x12\n\nclass_code\x18\x05 \x01(\t\x12\x44\n\x05links\x18\x06 \x03(\x0b\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentLink\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12\x14\n\x0cposition_uid\x18\x0b \x01(\t\"6\n\x0eInstrumentLink\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0einstrument_uid\x18\x02 \x01(\t\"\x15\n\x13GetFavoritesRequest\"o\n\x14GetFavoritesResponse\x12W\n\x14\x66\x61vorite_instruments\x18\x01 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.FavoriteInstrument\"\x8c\x02\n\x12\x46\x61voriteInstrument\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x0c\n\x04isin\x18\x04 \x01(\t\x12\x17\n\x0finstrument_type\x18\x0b \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x0b\n\x03uid\x18\r \x01(\t\x12\x10\n\x08otc_flag\x18\x10 \x01(\x08\x12 \n\x18\x61pi_trade_available_flag\x18\x11 \x01(\x08\x12N\n\x0finstrument_kind\x18\x12 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\"\xd3\x01\n\x14\x45\x64itFavoritesRequest\x12`\n\x0binstruments\x18\x01 \x03(\x0b\x32\x45.tinkoff.public.invest.api.contract.v1.EditFavoritesRequestInstrumentB\x04\xe2\x41\x01\x02\x12Y\n\x0b\x61\x63tion_type\x18\x06 \x01(\x0e\x32>.tinkoff.public.invest.api.contract.v1.EditFavoritesActionTypeB\x04\xe2\x41\x01\x02\"]\n\x1e\x45\x64itFavoritesRequestInstrument\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x42\x07\n\x05_figi\"p\n\x15\x45\x64itFavoritesResponse\x12W\n\x14\x66\x61vorite_instruments\x18\x01 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.FavoriteInstrument\"\x15\n\x13GetCountriesRequest\"a\n\x14GetCountriesResponse\x12I\n\tcountries\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.CountryResponse\"\x14\n\x12IndicativesRequest\"e\n\x13IndicativesResponse\x12N\n\x0binstruments\x18\x01 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.IndicativeResponse\"\x90\x02\n\x12IndicativeResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x12\n\nclass_code\x18\x03 \x01(\t\x12\x10\n\x08\x63urrency\x18\x04 \x01(\t\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08\x65xchange\x18\r \x01(\t\x12\x0b\n\x03uid\x18\x0e \x01(\t\x12\x1b\n\x12\x62uy_available_flag\x18\x94\x03 \x01(\x08\x12\x1c\n\x13sell_available_flag\x18\x95\x03 \x01(\x08\"Y\n\x0f\x43ountryResponse\x12\x10\n\x08\x61lfa_two\x18\x01 \x01(\t\x12\x12\n\nalfa_three\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\nname_brief\x18\x04 \x01(\t\"\xd9\x01\n\x15\x46indInstrumentRequest\x12\x13\n\x05query\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12S\n\x0finstrument_kind\x18\x02 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentTypeH\x00\x88\x01\x01\x12%\n\x18\x61pi_trade_available_flag\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x12\n\x10_instrument_kindB\x1b\n\x19_api_trade_available_flag\"e\n\x16\x46indInstrumentResponse\x12K\n\x0binstruments\x18\x01 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.InstrumentShort\"\xeb\x03\n\x0fInstrumentShort\x12\x0c\n\x04isin\x18\x01 \x01(\t\x12\x0c\n\x04\x66igi\x18\x02 \x01(\t\x12\x0e\n\x06ticker\x18\x03 \x01(\t\x12\x12\n\nclass_code\x18\x04 \x01(\t\x12\x17\n\x0finstrument_type\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x0b\n\x03uid\x18\x07 \x01(\t\x12\x14\n\x0cposition_uid\x18\x08 \x01(\t\x12N\n\x0finstrument_kind\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.InstrumentType\x12 \n\x18\x61pi_trade_available_flag\x18\x0b \x01(\x08\x12\x14\n\x0c\x66or_iis_flag\x18\x0c \x01(\x08\x12:\n\x16\x66irst_1min_candle_date\x18\x1a \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66irst_1day_candle_date\x18\x1b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16\x66or_qual_investor_flag\x18\x1c \x01(\x08\x12\x14\n\x0cweekend_flag\x18\x1d \x01(\x08\x12\x18\n\x10\x62locked_tca_flag\x18\x1e \x01(\x08\"O\n\x10GetBrandsRequest\x12;\n\x06paging\x18\x01 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.Page\"#\n\x0fGetBrandRequest\x12\x10\n\x02id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"\x96\x01\n\x11GetBrandsResponse\x12<\n\x06\x62rands\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Brand\x12\x43\n\x06paging\x18\x02 \x01(\x0b\x32\x33.tinkoff.public.invest.api.contract.v1.PageResponse\"3\n\x1bGetAssetFundamentalsRequest\x12\x14\n\x06\x61ssets\x18\x01 \x03(\tB\x04\xe2\x41\x01\x02\"\xfd\x0e\n\x1cGetAssetFundamentalsResponse\x12k\n\x0c\x66undamentals\x18\x01 \x03(\x0b\x32U.tinkoff.public.invest.api.contract.v1.GetAssetFundamentalsResponse.StatisticResponse\x1a\xef\r\n\x11StatisticResponse\x12\x11\n\tasset_uid\x18\x01 \x01(\t\x12\x10\n\x08\x63urrency\x18\x02 \x01(\t\x12\x1d\n\x15market_capitalization\x18\x03 \x01(\x01\x12 \n\x18high_price_last_52_weeks\x18\x04 \x01(\x01\x12\x1f\n\x17low_price_last_52_weeks\x18\x05 \x01(\x01\x12)\n!average_daily_volume_last_10_days\x18\x06 \x01(\x01\x12)\n!average_daily_volume_last_4_weeks\x18\x07 \x01(\x01\x12\x0c\n\x04\x62\x65ta\x18\x08 \x01(\x01\x12\x12\n\nfree_float\x18\t \x01(\x01\x12%\n\x1d\x66orward_annual_dividend_yield\x18\n \x01(\x01\x12\x1a\n\x12shares_outstanding\x18\x0b \x01(\x01\x12\x13\n\x0brevenue_ttm\x18\x0c \x01(\x01\x12\x12\n\nebitda_ttm\x18\r \x01(\x01\x12\x16\n\x0enet_income_ttm\x18\x0e \x01(\x01\x12\x0f\n\x07\x65ps_ttm\x18\x0f \x01(\x01\x12\x17\n\x0f\x64iluted_eps_ttm\x18\x10 \x01(\x01\x12\x1a\n\x12\x66ree_cash_flow_ttm\x18\x11 \x01(\x01\x12,\n$five_year_annual_revenue_growth_rate\x18\x12 \x01(\x01\x12-\n%three_year_annual_revenue_growth_rate\x18\x13 \x01(\x01\x12\x14\n\x0cpe_ratio_ttm\x18\x14 \x01(\x01\x12\x1a\n\x12price_to_sales_ttm\x18\x15 \x01(\x01\x12\x19\n\x11price_to_book_ttm\x18\x16 \x01(\x01\x12#\n\x1bprice_to_free_cash_flow_ttm\x18\x17 \x01(\x01\x12\"\n\x1atotal_enterprise_value_mrq\x18\x18 \x01(\x01\x12\x18\n\x10\x65v_to_ebitda_mrq\x18\x19 \x01(\x01\x12\x16\n\x0enet_margin_mrq\x18\x1a \x01(\x01\x12\x1f\n\x17net_interest_margin_mrq\x18\x1b \x01(\x01\x12\x0b\n\x03roe\x18\x1c \x01(\x01\x12\x0b\n\x03roa\x18\x1d \x01(\x01\x12\x0c\n\x04roic\x18\x1e \x01(\x01\x12\x16\n\x0etotal_debt_mrq\x18\x1f \x01(\x01\x12 \n\x18total_debt_to_equity_mrq\x18  \x01(\x01\x12 \n\x18total_debt_to_ebitda_mrq\x18! \x01(\x01\x12\x1f\n\x17\x66ree_cash_flow_to_price\x18\" \x01(\x01\x12\x1a\n\x12net_debt_to_ebitda\x18# \x01(\x01\x12\x19\n\x11\x63urrent_ratio_mrq\x18$ \x01(\x01\x12&\n\x1e\x66ixed_charge_coverage_ratio_fy\x18% \x01(\x01\x12 \n\x18\x64ividend_yield_daily_ttm\x18& \x01(\x01\x12\x19\n\x11\x64ividend_rate_ttm\x18\' \x01(\x01\x12\x1b\n\x13\x64ividends_per_share\x18( \x01(\x01\x12)\n!five_years_average_dividend_yield\x18) \x01(\x01\x12-\n%five_year_annual_dividend_growth_rate\x18* \x01(\x01\x12 \n\x18\x64ividend_payout_ratio_fy\x18+ \x01(\x01\x12\x14\n\x0c\x62uy_back_ttm\x18, \x01(\x01\x12+\n#one_year_annual_revenue_growth_rate\x18- \x01(\x01\x12\x1f\n\x17\x64omicile_indicator_code\x18. \x01(\t\x12!\n\x19\x61\x64r_to_common_share_ratio\x18/ \x01(\x01\x12\x1b\n\x13number_of_employees\x18\x30 \x01(\x01\x12\x34\n\x10\x65x_dividend_date\x18\x31 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12<\n\x18\x66iscal_period_start_date\x18\x32 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16\x66iscal_period_end_date\x18\x33 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x19revenue_change_five_years\x18\x35 \x01(\x01\x12\x1d\n\x15\x65ps_change_five_years\x18\x36 \x01(\x01\x12 \n\x18\x65\x62itda_change_five_years\x18\x37 \x01(\x01\x12$\n\x1ctotal_debt_change_five_years\x18\x38 \x01(\x01\x12\x13\n\x0b\x65v_to_sales\x18\x39 \x01(\x01\"\xa1\x01\n\x16GetAssetReportsRequest\x12\x1b\n\rinstrument_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12-\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x12+\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_to\"\xa7\x04\n\x17GetAssetReportsResponse\x12\x63\n\x06\x65vents\x18\x01 \x03(\x0b\x32S.tinkoff.public.invest.api.contract.v1.GetAssetReportsResponse.GetAssetReportsEvent\x1a\xa2\x02\n\x14GetAssetReportsEvent\x12\x15\n\rinstrument_id\x18\x01 \x01(\t\x12/\n\x0breport_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bperiod_year\x18\x03 \x01(\x05\x12\x12\n\nperiod_num\x18\x04 \x01(\x05\x12i\n\x0bperiod_type\x18\x05 \x01(\x0e\x32T.tinkoff.public.invest.api.contract.v1.GetAssetReportsResponse.AssetReportPeriodType\x12.\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x81\x01\n\x15\x41ssetReportPeriodType\x12\x1b\n\x17PERIOD_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13PERIOD_TYPE_QUARTER\x10\x01\x12\x1a\n\x16PERIOD_TYPE_SEMIANNUAL\x10\x02\x12\x16\n\x12PERIOD_TYPE_ANNUAL\x10\x03\"k\n\x1cGetConsensusForecastsRequest\x12@\n\x06paging\x18\x01 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PageH\x00\x88\x01\x01\x42\t\n\x07_paging\"\x86\x06\n\x1dGetConsensusForecastsResponse\x12j\n\x05items\x18\x01 \x03(\x0b\x32[.tinkoff.public.invest.api.contract.v1.GetConsensusForecastsResponse.ConsensusForecastsItem\x12\x41\n\x04page\x18\x02 \x01(\x0b\x32\x33.tinkoff.public.invest.api.contract.v1.PageResponse\x1a\xb5\x04\n\x16\x43onsensusForecastsItem\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x11\n\tasset_uid\x18\x02 \x01(\t\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12K\n\x11\x62\x65st_target_price\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12I\n\x0f\x62\x65st_target_low\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10\x62\x65st_target_high\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x1b\n\x13total_buy_recommend\x18\x07 \x01(\x05\x12\x1c\n\x14total_hold_recommend\x18\x08 \x01(\x05\x12\x1c\n\x14total_sell_recommend\x18\t \x01(\x05\x12\x10\n\x08\x63urrency\x18\n \x01(\t\x12H\n\tconsensus\x18\x0b \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.Recommendation\x12\x32\n\x0eprognosis_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"+\n\x12GetForecastRequest\x12\x15\n\rinstrument_id\x18\x01 \x01(\t\"\x97\n\n\x13GetForecastResponse\x12V\n\x07targets\x18\x01 \x03(\x0b\x32\x45.tinkoff.public.invest.api.contract.v1.GetForecastResponse.TargetItem\x12[\n\tconsensus\x18\x02 \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetForecastResponse.ConsensusItem\x1a\x8c\x04\n\nTargetItem\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12\x0f\n\x07\x63ompany\x18\x03 \x01(\t\x12M\n\x0erecommendation\x18\x04 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.Recommendation\x12\x37\n\x13recommendation_date\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x63urrency\x18\x06 \x01(\t\x12G\n\rcurrent_price\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x46\n\x0ctarget_price\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x46\n\x0cprice_change\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10price_change_rel\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x11\n\tshow_name\x18\x0b \x01(\t\x1a\xbb\x04\n\rConsensusItem\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0e\n\x06ticker\x18\x02 \x01(\t\x12M\n\x0erecommendation\x18\x03 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.Recommendation\x12\x10\n\x08\x63urrency\x18\x04 \x01(\t\x12G\n\rcurrent_price\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x43\n\tconsensus\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nmin_target\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nmax_target\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x46\n\x0cprice_change\x18\t \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12J\n\x10price_change_rel\x18\n \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xe0\x01\n\x0fTradingInterval\x12\x0c\n\x04type\x18\x01 \x01(\t\x12U\n\x08interval\x18\x02 \x01(\x0b\x32\x43.tinkoff.public.invest.api.contract.v1.TradingInterval.TimeInterval\x1ah\n\x0cTimeInterval\x12,\n\x08start_ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_ts\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp*\xd7\x01\n\nCouponType\x12\x1b\n\x17\x43OUPON_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OUPON_TYPE_CONSTANT\x10\x01\x12\x18\n\x14\x43OUPON_TYPE_FLOATING\x10\x02\x12\x18\n\x14\x43OUPON_TYPE_DISCOUNT\x10\x03\x12\x18\n\x14\x43OUPON_TYPE_MORTGAGE\x10\x04\x12\x13\n\x0f\x43OUPON_TYPE_FIX\x10\x05\x12\x18\n\x14\x43OUPON_TYPE_VARIABLE\x10\x06\x12\x15\n\x11\x43OUPON_TYPE_OTHER\x10\x07*h\n\x0fOptionDirection\x12 \n\x1cOPTION_DIRECTION_UNSPECIFIED\x10\x00\x12\x18\n\x14OPTION_DIRECTION_PUT\x10\x01\x12\x19\n\x15OPTION_DIRECTION_CALL\x10\x02*{\n\x11OptionPaymentType\x12#\n\x1fOPTION_PAYMENT_TYPE_UNSPECIFIED\x10\x00\x12\x1f\n\x1bOPTION_PAYMENT_TYPE_PREMIUM\x10\x01\x12 \n\x1cOPTION_PAYMENT_TYPE_MARGINAL\x10\x02*a\n\x0bOptionStyle\x12\x1c\n\x18OPTION_STYLE_UNSPECIFIED\x10\x00\x12\x19\n\x15OPTION_STYLE_AMERICAN\x10\x01\x12\x19\n\x15OPTION_STYLE_EUROPEAN\x10\x02*\x95\x01\n\x14OptionSettlementType\x12%\n!OPTION_EXECUTION_TYPE_UNSPECIFIED\x10\x00\x12+\n\'OPTION_EXECUTION_TYPE_PHYSICAL_DELIVERY\x10\x01\x12)\n%OPTION_EXECUTION_TYPE_CASH_SETTLEMENT\x10\x02*\xae\x01\n\x10InstrumentIdType\x12\x1d\n\x19INSTRUMENT_ID_UNSPECIFIED\x10\x00\x12\x1b\n\x17INSTRUMENT_ID_TYPE_FIGI\x10\x01\x12\x1d\n\x19INSTRUMENT_ID_TYPE_TICKER\x10\x02\x12\x1a\n\x16INSTRUMENT_ID_TYPE_UID\x10\x03\x12#\n\x1fINSTRUMENT_ID_TYPE_POSITION_UID\x10\x04*l\n\x10InstrumentStatus\x12!\n\x1dINSTRUMENT_STATUS_UNSPECIFIED\x10\x00\x12\x1a\n\x16INSTRUMENT_STATUS_BASE\x10\x01\x12\x19\n\x15INSTRUMENT_STATUS_ALL\x10\x02*\xe5\x01\n\tShareType\x12\x1a\n\x16SHARE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11SHARE_TYPE_COMMON\x10\x01\x12\x18\n\x14SHARE_TYPE_PREFERRED\x10\x02\x12\x12\n\x0eSHARE_TYPE_ADR\x10\x03\x12\x12\n\x0eSHARE_TYPE_GDR\x10\x04\x12\x12\n\x0eSHARE_TYPE_MLP\x10\x05\x12\x1a\n\x16SHARE_TYPE_NY_REG_SHRS\x10\x06\x12\x1e\n\x1aSHARE_TYPE_CLOSED_END_FUND\x10\x07\x12\x13\n\x0fSHARE_TYPE_REIT\x10\x08*\x89\x01\n\tAssetType\x12\x1a\n\x16\x41SSET_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13\x41SSET_TYPE_CURRENCY\x10\x01\x12\x18\n\x14\x41SSET_TYPE_COMMODITY\x10\x02\x12\x14\n\x10\x41SSET_TYPE_INDEX\x10\x03\x12\x17\n\x13\x41SSET_TYPE_SECURITY\x10\x04*f\n\x15StructuredProductType\x12\x17\n\x13SP_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13SP_TYPE_DELIVERABLE\x10\x01\x12\x1b\n\x17SP_TYPE_NON_DELIVERABLE\x10\x02*\x8d\x01\n\x17\x45\x64itFavoritesActionType\x12*\n&EDIT_FAVORITES_ACTION_TYPE_UNSPECIFIED\x10\x00\x12\"\n\x1e\x45\x44IT_FAVORITES_ACTION_TYPE_ADD\x10\x01\x12\"\n\x1e\x45\x44IT_FAVORITES_ACTION_TYPE_DEL\x10\x02*s\n\x0cRealExchange\x12\x1d\n\x19REAL_EXCHANGE_UNSPECIFIED\x10\x00\x12\x16\n\x12REAL_EXCHANGE_MOEX\x10\x01\x12\x15\n\x11REAL_EXCHANGE_RTS\x10\x02\x12\x15\n\x11REAL_EXCHANGE_OTC\x10\x03*z\n\x0eRecommendation\x12\x1e\n\x1aRECOMMENDATION_UNSPECIFIED\x10\x00\x12\x16\n\x12RECOMMENDATION_BUY\x10\x01\x12\x17\n\x13RECOMMENDATION_HOLD\x10\x02\x12\x17\n\x13RECOMMENDATION_SELL\x10\x03*i\n\tRiskLevel\x12\x1a\n\x16RISK_LEVEL_UNSPECIFIED\x10\x00\x12\x12\n\x0eRISK_LEVEL_LOW\x10\x01\x12\x17\n\x13RISK_LEVEL_MODERATE\x10\x02\x12\x13\n\x0fRISK_LEVEL_HIGH\x10\x03*=\n\x08\x42ondType\x12\x19\n\x15\x42OND_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42OND_TYPE_REPLACED\x10\x01*]\n\x16InstrumentExchangeType\x12#\n\x1fINSTRUMENT_EXCHANGE_UNSPECIFIED\x10\x00\x12\x1e\n\x1aINSTRUMENT_EXCHANGE_DEALER\x10\x01\x32\xef\"\n\x12InstrumentsService\x12\x93\x01\n\x10TradingSchedules\x12>.tinkoff.public.invest.api.contract.v1.TradingSchedulesRequest\x1a?.tinkoff.public.invest.api.contract.v1.TradingSchedulesResponse\x12w\n\x06\x42ondBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x33.tinkoff.public.invest.api.contract.v1.BondResponse\x12x\n\x05\x42onds\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x34.tinkoff.public.invest.api.contract.v1.BondsResponse\x12\x8d\x01\n\x0eGetBondCoupons\x12<.tinkoff.public.invest.api.contract.v1.GetBondCouponsRequest\x1a=.tinkoff.public.invest.api.contract.v1.GetBondCouponsResponse\x12\x8a\x01\n\rGetBondEvents\x12;.tinkoff.public.invest.api.contract.v1.GetBondEventsRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetBondEventsResponse\x12\x7f\n\nCurrencyBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x37.tinkoff.public.invest.api.contract.v1.CurrencyResponse\x12\x82\x01\n\nCurrencies\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.CurrenciesResponse\x12u\n\x05\x45tfBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x32.tinkoff.public.invest.api.contract.v1.EtfResponse\x12v\n\x04\x45tfs\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x33.tinkoff.public.invest.api.contract.v1.EtfsResponse\x12{\n\x08\x46utureBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.FutureResponse\x12|\n\x07\x46utures\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x36.tinkoff.public.invest.api.contract.v1.FuturesResponse\x12{\n\x08OptionBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.OptionResponse\x12\x81\x01\n\x07Options\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x36.tinkoff.public.invest.api.contract.v1.OptionsResponse\"\x03\x88\x02\x01\x12\x80\x01\n\tOptionsBy\x12;.tinkoff.public.invest.api.contract.v1.FilterOptionsRequest\x1a\x36.tinkoff.public.invest.api.contract.v1.OptionsResponse\x12y\n\x07ShareBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x34.tinkoff.public.invest.api.contract.v1.ShareResponse\x12z\n\x06Shares\x12\x39.tinkoff.public.invest.api.contract.v1.InstrumentsRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.SharesResponse\x12\x84\x01\n\x0bIndicatives\x12\x39.tinkoff.public.invest.api.contract.v1.IndicativesRequest\x1a:.tinkoff.public.invest.api.contract.v1.IndicativesResponse\x12\x9c\x01\n\x13GetAccruedInterests\x12\x41.tinkoff.public.invest.api.contract.v1.GetAccruedInterestsRequest\x1a\x42.tinkoff.public.invest.api.contract.v1.GetAccruedInterestsResponse\x12\x93\x01\n\x10GetFuturesMargin\x12>.tinkoff.public.invest.api.contract.v1.GetFuturesMarginRequest\x1a?.tinkoff.public.invest.api.contract.v1.GetFuturesMarginResponse\x12\x86\x01\n\x0fGetInstrumentBy\x12\x38.tinkoff.public.invest.api.contract.v1.InstrumentRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.InstrumentResponse\x12\x87\x01\n\x0cGetDividends\x12:.tinkoff.public.invest.api.contract.v1.GetDividendsRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetDividendsResponse\x12w\n\nGetAssetBy\x12\x33.tinkoff.public.invest.api.contract.v1.AssetRequest\x1a\x34.tinkoff.public.invest.api.contract.v1.AssetResponse\x12x\n\tGetAssets\x12\x34.tinkoff.public.invest.api.contract.v1.AssetsRequest\x1a\x35.tinkoff.public.invest.api.contract.v1.AssetsResponse\x12\x87\x01\n\x0cGetFavorites\x12:.tinkoff.public.invest.api.contract.v1.GetFavoritesRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetFavoritesResponse\x12\x8a\x01\n\rEditFavorites\x12;.tinkoff.public.invest.api.contract.v1.EditFavoritesRequest\x1a<.tinkoff.public.invest.api.contract.v1.EditFavoritesResponse\x12\x87\x01\n\x0cGetCountries\x12:.tinkoff.public.invest.api.contract.v1.GetCountriesRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetCountriesResponse\x12\x8d\x01\n\x0e\x46indInstrument\x12<.tinkoff.public.invest.api.contract.v1.FindInstrumentRequest\x1a=.tinkoff.public.invest.api.contract.v1.FindInstrumentResponse\x12~\n\tGetBrands\x12\x37.tinkoff.public.invest.api.contract.v1.GetBrandsRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.GetBrandsResponse\x12r\n\nGetBrandBy\x12\x36.tinkoff.public.invest.api.contract.v1.GetBrandRequest\x1a,.tinkoff.public.invest.api.contract.v1.Brand\x12\x9f\x01\n\x14GetAssetFundamentals\x12\x42.tinkoff.public.invest.api.contract.v1.GetAssetFundamentalsRequest\x1a\x43.tinkoff.public.invest.api.contract.v1.GetAssetFundamentalsResponse\x12\x90\x01\n\x0fGetAssetReports\x12=.tinkoff.public.invest.api.contract.v1.GetAssetReportsRequest\x1a>.tinkoff.public.invest.api.contract.v1.GetAssetReportsResponse\x12\xa2\x01\n\x15GetConsensusForecasts\x12\x43.tinkoff.public.invest.api.contract.v1.GetConsensusForecastsRequest\x1a\x44.tinkoff.public.invest.api.contract.v1.GetConsensusForecastsResponse\x12\x86\x01\n\rGetForecastBy\x12\x39.tinkoff.public.invest.api.contract.v1.GetForecastRequest\x1a:.tinkoff.public.invest.api.contract.v1.GetForecastResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tinkoff.invest.grpc.instruments_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034ru.tinkoff.piapi.contract.v1P\001Z\014./;investapi\242\002\005TIAPI\252\002\024Tinkoff.InvestApi.V1\312\002\021Tinkoff\\Invest\\V1'
@@ -73,222 +73,226 @@
   _GETBRANDREQUEST.fields_by_name['id']._serialized_options = b'\342A\001\002'
   _GETASSETFUNDAMENTALSREQUEST.fields_by_name['assets']._options = None
   _GETASSETFUNDAMENTALSREQUEST.fields_by_name['assets']._serialized_options = b'\342A\001\002'
   _GETASSETREPORTSREQUEST.fields_by_name['instrument_id']._options = None
   _GETASSETREPORTSREQUEST.fields_by_name['instrument_id']._serialized_options = b'\342A\001\002'
   _INSTRUMENTSSERVICE.methods_by_name['Options']._options = None
   _INSTRUMENTSSERVICE.methods_by_name['Options']._serialized_options = b'\210\002\001'
-  _globals['_COUPONTYPE']._serialized_start=32674
-  _globals['_COUPONTYPE']._serialized_end=32889
-  _globals['_OPTIONDIRECTION']._serialized_start=32891
-  _globals['_OPTIONDIRECTION']._serialized_end=32995
-  _globals['_OPTIONPAYMENTTYPE']._serialized_start=32997
-  _globals['_OPTIONPAYMENTTYPE']._serialized_end=33120
-  _globals['_OPTIONSTYLE']._serialized_start=33122
-  _globals['_OPTIONSTYLE']._serialized_end=33219
-  _globals['_OPTIONSETTLEMENTTYPE']._serialized_start=33222
-  _globals['_OPTIONSETTLEMENTTYPE']._serialized_end=33371
-  _globals['_INSTRUMENTIDTYPE']._serialized_start=33374
-  _globals['_INSTRUMENTIDTYPE']._serialized_end=33548
-  _globals['_INSTRUMENTSTATUS']._serialized_start=33550
-  _globals['_INSTRUMENTSTATUS']._serialized_end=33658
-  _globals['_SHARETYPE']._serialized_start=33661
-  _globals['_SHARETYPE']._serialized_end=33890
-  _globals['_ASSETTYPE']._serialized_start=33893
-  _globals['_ASSETTYPE']._serialized_end=34030
-  _globals['_STRUCTUREDPRODUCTTYPE']._serialized_start=34032
-  _globals['_STRUCTUREDPRODUCTTYPE']._serialized_end=34134
-  _globals['_EDITFAVORITESACTIONTYPE']._serialized_start=34137
-  _globals['_EDITFAVORITESACTIONTYPE']._serialized_end=34278
-  _globals['_REALEXCHANGE']._serialized_start=34280
-  _globals['_REALEXCHANGE']._serialized_end=34395
-  _globals['_RECOMMENDATION']._serialized_start=34397
-  _globals['_RECOMMENDATION']._serialized_end=34519
-  _globals['_RISKLEVEL']._serialized_start=34521
-  _globals['_RISKLEVEL']._serialized_end=34626
+  _globals['_COUPONTYPE']._serialized_start=33047
+  _globals['_COUPONTYPE']._serialized_end=33262
+  _globals['_OPTIONDIRECTION']._serialized_start=33264
+  _globals['_OPTIONDIRECTION']._serialized_end=33368
+  _globals['_OPTIONPAYMENTTYPE']._serialized_start=33370
+  _globals['_OPTIONPAYMENTTYPE']._serialized_end=33493
+  _globals['_OPTIONSTYLE']._serialized_start=33495
+  _globals['_OPTIONSTYLE']._serialized_end=33592
+  _globals['_OPTIONSETTLEMENTTYPE']._serialized_start=33595
+  _globals['_OPTIONSETTLEMENTTYPE']._serialized_end=33744
+  _globals['_INSTRUMENTIDTYPE']._serialized_start=33747
+  _globals['_INSTRUMENTIDTYPE']._serialized_end=33921
+  _globals['_INSTRUMENTSTATUS']._serialized_start=33923
+  _globals['_INSTRUMENTSTATUS']._serialized_end=34031
+  _globals['_SHARETYPE']._serialized_start=34034
+  _globals['_SHARETYPE']._serialized_end=34263
+  _globals['_ASSETTYPE']._serialized_start=34266
+  _globals['_ASSETTYPE']._serialized_end=34403
+  _globals['_STRUCTUREDPRODUCTTYPE']._serialized_start=34405
+  _globals['_STRUCTUREDPRODUCTTYPE']._serialized_end=34507
+  _globals['_EDITFAVORITESACTIONTYPE']._serialized_start=34510
+  _globals['_EDITFAVORITESACTIONTYPE']._serialized_end=34651
+  _globals['_REALEXCHANGE']._serialized_start=34653
+  _globals['_REALEXCHANGE']._serialized_end=34768
+  _globals['_RECOMMENDATION']._serialized_start=34770
+  _globals['_RECOMMENDATION']._serialized_end=34892
+  _globals['_RISKLEVEL']._serialized_start=34894
+  _globals['_RISKLEVEL']._serialized_end=34999
+  _globals['_BONDTYPE']._serialized_start=35001
+  _globals['_BONDTYPE']._serialized_end=35062
+  _globals['_INSTRUMENTEXCHANGETYPE']._serialized_start=35064
+  _globals['_INSTRUMENTEXCHANGETYPE']._serialized_end=35157
   _globals['_TRADINGSCHEDULESREQUEST']._serialized_start=201
   _globals['_TRADINGSCHEDULESREQUEST']._serialized_end=370
   _globals['_TRADINGSCHEDULESRESPONSE']._serialized_start=372
   _globals['_TRADINGSCHEDULESRESPONSE']._serialized_end=473
   _globals['_TRADINGSCHEDULE']._serialized_start=475
   _globals['_TRADINGSCHEDULE']._serialized_end=575
   _globals['_TRADINGDAY']._serialized_start=578
   _globals['_TRADINGDAY']._serialized_end=1497
   _globals['_INSTRUMENTREQUEST']._serialized_start=1500
   _globals['_INSTRUMENTREQUEST']._serialized_end=1657
   _globals['_INSTRUMENTSREQUEST']._serialized_start=1660
-  _globals['_INSTRUMENTSREQUEST']._serialized_end=1791
-  _globals['_FILTEROPTIONSREQUEST']._serialized_start=1794
-  _globals['_FILTEROPTIONSREQUEST']._serialized_end=1934
-  _globals['_BONDRESPONSE']._serialized_start=1936
-  _globals['_BONDRESPONSE']._serialized_end=2015
-  _globals['_BONDSRESPONSE']._serialized_start=2017
-  _globals['_BONDSRESPONSE']._serialized_end=2098
-  _globals['_GETBONDCOUPONSREQUEST']._serialized_start=2101
-  _globals['_GETBONDCOUPONSREQUEST']._serialized_end=2279
-  _globals['_GETBONDCOUPONSRESPONSE']._serialized_start=2281
-  _globals['_GETBONDCOUPONSRESPONSE']._serialized_end=2368
-  _globals['_GETBONDEVENTSREQUEST']._serialized_start=2371
-  _globals['_GETBONDEVENTSREQUEST']._serialized_end=2738
-  _globals['_GETBONDEVENTSREQUEST_EVENTTYPE']._serialized_start=2601
-  _globals['_GETBONDEVENTSREQUEST_EVENTTYPE']._serialized_end=2722
-  _globals['_GETBONDEVENTSRESPONSE']._serialized_start=2741
-  _globals['_GETBONDEVENTSRESPONSE']._serialized_end=3878
-  _globals['_GETBONDEVENTSRESPONSE_BONDEVENT']._serialized_start=2855
-  _globals['_GETBONDEVENTSRESPONSE_BONDEVENT']._serialized_end=3878
-  _globals['_COUPON']._serialized_start=3881
-  _globals['_COUPON']._serialized_end=4297
-  _globals['_CURRENCYRESPONSE']._serialized_start=4299
-  _globals['_CURRENCYRESPONSE']._serialized_end=4386
-  _globals['_CURRENCIESRESPONSE']._serialized_start=4388
-  _globals['_CURRENCIESRESPONSE']._serialized_end=4478
-  _globals['_ETFRESPONSE']._serialized_start=4480
-  _globals['_ETFRESPONSE']._serialized_end=4557
-  _globals['_ETFSRESPONSE']._serialized_start=4559
-  _globals['_ETFSRESPONSE']._serialized_end=4638
-  _globals['_FUTURERESPONSE']._serialized_start=4640
-  _globals['_FUTURERESPONSE']._serialized_end=4723
-  _globals['_FUTURESRESPONSE']._serialized_start=4725
-  _globals['_FUTURESRESPONSE']._serialized_end=4810
-  _globals['_OPTIONRESPONSE']._serialized_start=4812
-  _globals['_OPTIONRESPONSE']._serialized_end=4895
-  _globals['_OPTIONSRESPONSE']._serialized_start=4897
-  _globals['_OPTIONSRESPONSE']._serialized_end=4982
-  _globals['_OPTION']._serialized_start=4985
-  _globals['_OPTION']._serialized_end=7016
-  _globals['_SHARERESPONSE']._serialized_start=7018
-  _globals['_SHARERESPONSE']._serialized_end=7099
-  _globals['_SHARESRESPONSE']._serialized_start=7101
-  _globals['_SHARESRESPONSE']._serialized_end=7184
-  _globals['_BOND']._serialized_start=7187
-  _globals['_BOND']._serialized_end=9257
-  _globals['_CURRENCY']._serialized_start=9260
-  _globals['_CURRENCY']._serialized_end=10648
-  _globals['_ETF']._serialized_start=10651
-  _globals['_ETF']._serialized_end=12241
-  _globals['_FUTURE']._serialized_start=12244
-  _globals['_FUTURE']._serialized_end=14121
-  _globals['_SHARE']._serialized_start=14124
-  _globals['_SHARE']._serialized_end=15726
-  _globals['_GETACCRUEDINTERESTSREQUEST']._serialized_start=15729
-  _globals['_GETACCRUEDINTERESTSREQUEST']._serialized_end=15898
-  _globals['_GETACCRUEDINTERESTSRESPONSE']._serialized_start=15900
-  _globals['_GETACCRUEDINTERESTSRESPONSE']._serialized_end=16012
-  _globals['_ACCRUEDINTEREST']._serialized_start=16015
-  _globals['_ACCRUEDINTEREST']._serialized_end=16279
-  _globals['_GETFUTURESMARGINREQUEST']._serialized_start=16281
-  _globals['_GETFUTURESMARGINREQUEST']._serialized_end=16353
-  _globals['_GETFUTURESMARGINRESPONSE']._serialized_start=16356
-  _globals['_GETFUTURESMARGINRESPONSE']._serialized_end=16712
-  _globals['_INSTRUMENTRESPONSE']._serialized_start=16714
-  _globals['_INSTRUMENTRESPONSE']._serialized_end=16805
-  _globals['_INSTRUMENT']._serialized_start=16808
-  _globals['_INSTRUMENT']._serialized_end=18227
-  _globals['_GETDIVIDENDSREQUEST']._serialized_start=18230
-  _globals['_GETDIVIDENDSREQUEST']._serialized_end=18406
-  _globals['_GETDIVIDENDSRESPONSE']._serialized_start=18408
-  _globals['_GETDIVIDENDSRESPONSE']._serialized_end=18498
-  _globals['_DIVIDEND']._serialized_start=18501
-  _globals['_DIVIDEND']._serialized_end=19019
-  _globals['_ASSETREQUEST']._serialized_start=19021
-  _globals['_ASSETREQUEST']._serialized_end=19053
-  _globals['_ASSETRESPONSE']._serialized_start=19055
-  _globals['_ASSETRESPONSE']._serialized_end=19135
-  _globals['_ASSETSREQUEST']._serialized_start=19137
-  _globals['_ASSETSREQUEST']._serialized_end=19257
-  _globals['_ASSETSRESPONSE']._serialized_start=19259
-  _globals['_ASSETSRESPONSE']._serialized_end=19337
-  _globals['_ASSETFULL']._serialized_start=19340
-  _globals['_ASSETFULL']._serialized_end=20004
-  _globals['_ASSET']._serialized_start=20007
-  _globals['_ASSET']._serialized_end=20182
-  _globals['_ASSETCURRENCY']._serialized_start=20184
-  _globals['_ASSETCURRENCY']._serialized_end=20222
-  _globals['_ASSETSECURITY']._serialized_start=20225
-  _globals['_ASSETSECURITY']._serialized_end=20727
-  _globals['_ASSETSHARE']._serialized_start=20730
-  _globals['_ASSETSHARE']._serialized_end=21455
-  _globals['_ASSETBOND']._serialized_start=21458
-  _globals['_ASSETBOND']._serialized_end=22322
-  _globals['_ASSETSTRUCTUREDPRODUCT']._serialized_start=22325
-  _globals['_ASSETSTRUCTUREDPRODUCT']._serialized_end=22997
-  _globals['_ASSETETF']._serialized_start=23000
-  _globals['_ASSETETF']._serialized_end=24368
-  _globals['_ASSETCLEARINGCERTIFICATE']._serialized_start=24370
-  _globals['_ASSETCLEARINGCERTIFICATE']._serialized_end=24489
-  _globals['_BRAND']._serialized_start=24492
-  _globals['_BRAND']._serialized_end=24649
-  _globals['_ASSETINSTRUMENT']._serialized_start=24652
-  _globals['_ASSETINSTRUMENT']._serialized_end=24929
-  _globals['_INSTRUMENTLINK']._serialized_start=24931
-  _globals['_INSTRUMENTLINK']._serialized_end=24985
-  _globals['_GETFAVORITESREQUEST']._serialized_start=24987
-  _globals['_GETFAVORITESREQUEST']._serialized_end=25008
-  _globals['_GETFAVORITESRESPONSE']._serialized_start=25010
-  _globals['_GETFAVORITESRESPONSE']._serialized_end=25121
-  _globals['_FAVORITEINSTRUMENT']._serialized_start=25124
-  _globals['_FAVORITEINSTRUMENT']._serialized_end=25392
-  _globals['_EDITFAVORITESREQUEST']._serialized_start=25395
-  _globals['_EDITFAVORITESREQUEST']._serialized_end=25606
-  _globals['_EDITFAVORITESREQUESTINSTRUMENT']._serialized_start=25608
-  _globals['_EDITFAVORITESREQUESTINSTRUMENT']._serialized_end=25701
-  _globals['_EDITFAVORITESRESPONSE']._serialized_start=25703
-  _globals['_EDITFAVORITESRESPONSE']._serialized_end=25815
-  _globals['_GETCOUNTRIESREQUEST']._serialized_start=25817
-  _globals['_GETCOUNTRIESREQUEST']._serialized_end=25838
-  _globals['_GETCOUNTRIESRESPONSE']._serialized_start=25840
-  _globals['_GETCOUNTRIESRESPONSE']._serialized_end=25937
-  _globals['_INDICATIVESREQUEST']._serialized_start=25939
-  _globals['_INDICATIVESREQUEST']._serialized_end=25959
-  _globals['_INDICATIVESRESPONSE']._serialized_start=25961
-  _globals['_INDICATIVESRESPONSE']._serialized_end=26062
-  _globals['_INDICATIVERESPONSE']._serialized_start=26065
-  _globals['_INDICATIVERESPONSE']._serialized_end=26337
-  _globals['_COUNTRYRESPONSE']._serialized_start=26339
-  _globals['_COUNTRYRESPONSE']._serialized_end=26428
-  _globals['_FINDINSTRUMENTREQUEST']._serialized_start=26431
-  _globals['_FINDINSTRUMENTREQUEST']._serialized_end=26648
-  _globals['_FINDINSTRUMENTRESPONSE']._serialized_start=26650
-  _globals['_FINDINSTRUMENTRESPONSE']._serialized_end=26751
-  _globals['_INSTRUMENTSHORT']._serialized_start=26754
-  _globals['_INSTRUMENTSHORT']._serialized_end=27245
-  _globals['_GETBRANDSREQUEST']._serialized_start=27247
-  _globals['_GETBRANDSREQUEST']._serialized_end=27326
-  _globals['_GETBRANDREQUEST']._serialized_start=27328
-  _globals['_GETBRANDREQUEST']._serialized_end=27363
-  _globals['_GETBRANDSRESPONSE']._serialized_start=27366
-  _globals['_GETBRANDSRESPONSE']._serialized_end=27516
-  _globals['_GETASSETFUNDAMENTALSREQUEST']._serialized_start=27518
-  _globals['_GETASSETFUNDAMENTALSREQUEST']._serialized_end=27569
-  _globals['_GETASSETFUNDAMENTALSRESPONSE']._serialized_start=27572
-  _globals['_GETASSETFUNDAMENTALSRESPONSE']._serialized_end=29489
-  _globals['_GETASSETFUNDAMENTALSRESPONSE_STATISTICRESPONSE']._serialized_start=27714
-  _globals['_GETASSETFUNDAMENTALSRESPONSE_STATISTICRESPONSE']._serialized_end=29489
-  _globals['_GETASSETREPORTSREQUEST']._serialized_start=29492
-  _globals['_GETASSETREPORTSREQUEST']._serialized_end=29653
-  _globals['_GETASSETREPORTSRESPONSE']._serialized_start=29656
-  _globals['_GETASSETREPORTSRESPONSE']._serialized_end=30207
-  _globals['_GETASSETREPORTSRESPONSE_GETASSETREPORTSEVENT']._serialized_start=29785
-  _globals['_GETASSETREPORTSRESPONSE_GETASSETREPORTSEVENT']._serialized_end=30075
-  _globals['_GETASSETREPORTSRESPONSE_ASSETREPORTPERIODTYPE']._serialized_start=30078
-  _globals['_GETASSETREPORTSRESPONSE_ASSETREPORTPERIODTYPE']._serialized_end=30207
-  _globals['_GETCONSENSUSFORECASTSREQUEST']._serialized_start=30209
-  _globals['_GETCONSENSUSFORECASTSREQUEST']._serialized_end=30316
-  _globals['_GETCONSENSUSFORECASTSRESPONSE']._serialized_start=30319
-  _globals['_GETCONSENSUSFORECASTSRESPONSE']._serialized_end=31093
-  _globals['_GETCONSENSUSFORECASTSRESPONSE_CONSENSUSFORECASTSITEM']._serialized_start=30528
-  _globals['_GETCONSENSUSFORECASTSRESPONSE_CONSENSUSFORECASTSITEM']._serialized_end=31093
-  _globals['_GETFORECASTREQUEST']._serialized_start=31095
-  _globals['_GETFORECASTREQUEST']._serialized_end=31138
-  _globals['_GETFORECASTRESPONSE']._serialized_start=31141
-  _globals['_GETFORECASTRESPONSE']._serialized_end=32444
-  _globals['_GETFORECASTRESPONSE_TARGETITEM']._serialized_start=31346
-  _globals['_GETFORECASTRESPONSE_TARGETITEM']._serialized_end=31870
-  _globals['_GETFORECASTRESPONSE_CONSENSUSITEM']._serialized_start=31873
-  _globals['_GETFORECASTRESPONSE_CONSENSUSITEM']._serialized_end=32444
-  _globals['_TRADINGINTERVAL']._serialized_start=32447
-  _globals['_TRADINGINTERVAL']._serialized_end=32671
-  _globals['_TRADINGINTERVAL_TIMEINTERVAL']._serialized_start=32567
-  _globals['_TRADINGINTERVAL_TIMEINTERVAL']._serialized_end=32671
-  _globals['_INSTRUMENTSSERVICE']._serialized_start=34629
-  _globals['_INSTRUMENTSSERVICE']._serialized_end=39092
+  _globals['_INSTRUMENTSREQUEST']._serialized_end=1912
+  _globals['_FILTEROPTIONSREQUEST']._serialized_start=1915
+  _globals['_FILTEROPTIONSREQUEST']._serialized_end=2055
+  _globals['_BONDRESPONSE']._serialized_start=2057
+  _globals['_BONDRESPONSE']._serialized_end=2136
+  _globals['_BONDSRESPONSE']._serialized_start=2138
+  _globals['_BONDSRESPONSE']._serialized_end=2219
+  _globals['_GETBONDCOUPONSREQUEST']._serialized_start=2222
+  _globals['_GETBONDCOUPONSREQUEST']._serialized_end=2400
+  _globals['_GETBONDCOUPONSRESPONSE']._serialized_start=2402
+  _globals['_GETBONDCOUPONSRESPONSE']._serialized_end=2489
+  _globals['_GETBONDEVENTSREQUEST']._serialized_start=2492
+  _globals['_GETBONDEVENTSREQUEST']._serialized_end=2859
+  _globals['_GETBONDEVENTSREQUEST_EVENTTYPE']._serialized_start=2722
+  _globals['_GETBONDEVENTSREQUEST_EVENTTYPE']._serialized_end=2843
+  _globals['_GETBONDEVENTSRESPONSE']._serialized_start=2862
+  _globals['_GETBONDEVENTSRESPONSE']._serialized_end=3999
+  _globals['_GETBONDEVENTSRESPONSE_BONDEVENT']._serialized_start=2976
+  _globals['_GETBONDEVENTSRESPONSE_BONDEVENT']._serialized_end=3999
+  _globals['_COUPON']._serialized_start=4002
+  _globals['_COUPON']._serialized_end=4418
+  _globals['_CURRENCYRESPONSE']._serialized_start=4420
+  _globals['_CURRENCYRESPONSE']._serialized_end=4507
+  _globals['_CURRENCIESRESPONSE']._serialized_start=4509
+  _globals['_CURRENCIESRESPONSE']._serialized_end=4599
+  _globals['_ETFRESPONSE']._serialized_start=4601
+  _globals['_ETFRESPONSE']._serialized_end=4678
+  _globals['_ETFSRESPONSE']._serialized_start=4680
+  _globals['_ETFSRESPONSE']._serialized_end=4759
+  _globals['_FUTURERESPONSE']._serialized_start=4761
+  _globals['_FUTURERESPONSE']._serialized_end=4844
+  _globals['_FUTURESRESPONSE']._serialized_start=4846
+  _globals['_FUTURESRESPONSE']._serialized_end=4931
+  _globals['_OPTIONRESPONSE']._serialized_start=4933
+  _globals['_OPTIONRESPONSE']._serialized_end=5016
+  _globals['_OPTIONSRESPONSE']._serialized_start=5018
+  _globals['_OPTIONSRESPONSE']._serialized_end=5103
+  _globals['_OPTION']._serialized_start=5106
+  _globals['_OPTION']._serialized_end=7137
+  _globals['_SHARERESPONSE']._serialized_start=7139
+  _globals['_SHARERESPONSE']._serialized_end=7220
+  _globals['_SHARESRESPONSE']._serialized_start=7222
+  _globals['_SHARESRESPONSE']._serialized_end=7305
+  _globals['_BOND']._serialized_start=7308
+  _globals['_BOND']._serialized_end=9446
+  _globals['_CURRENCY']._serialized_start=9449
+  _globals['_CURRENCY']._serialized_end=10837
+  _globals['_ETF']._serialized_start=10840
+  _globals['_ETF']._serialized_end=12522
+  _globals['_FUTURE']._serialized_start=12525
+  _globals['_FUTURE']._serialized_end=14402
+  _globals['_SHARE']._serialized_start=14405
+  _globals['_SHARE']._serialized_end=16099
+  _globals['_GETACCRUEDINTERESTSREQUEST']._serialized_start=16102
+  _globals['_GETACCRUEDINTERESTSREQUEST']._serialized_end=16271
+  _globals['_GETACCRUEDINTERESTSRESPONSE']._serialized_start=16273
+  _globals['_GETACCRUEDINTERESTSRESPONSE']._serialized_end=16385
+  _globals['_ACCRUEDINTEREST']._serialized_start=16388
+  _globals['_ACCRUEDINTEREST']._serialized_end=16652
+  _globals['_GETFUTURESMARGINREQUEST']._serialized_start=16654
+  _globals['_GETFUTURESMARGINREQUEST']._serialized_end=16726
+  _globals['_GETFUTURESMARGINRESPONSE']._serialized_start=16729
+  _globals['_GETFUTURESMARGINRESPONSE']._serialized_end=17085
+  _globals['_INSTRUMENTRESPONSE']._serialized_start=17087
+  _globals['_INSTRUMENTRESPONSE']._serialized_end=17178
+  _globals['_INSTRUMENT']._serialized_start=17181
+  _globals['_INSTRUMENT']._serialized_end=18600
+  _globals['_GETDIVIDENDSREQUEST']._serialized_start=18603
+  _globals['_GETDIVIDENDSREQUEST']._serialized_end=18779
+  _globals['_GETDIVIDENDSRESPONSE']._serialized_start=18781
+  _globals['_GETDIVIDENDSRESPONSE']._serialized_end=18871
+  _globals['_DIVIDEND']._serialized_start=18874
+  _globals['_DIVIDEND']._serialized_end=19392
+  _globals['_ASSETREQUEST']._serialized_start=19394
+  _globals['_ASSETREQUEST']._serialized_end=19426
+  _globals['_ASSETRESPONSE']._serialized_start=19428
+  _globals['_ASSETRESPONSE']._serialized_end=19508
+  _globals['_ASSETSREQUEST']._serialized_start=19510
+  _globals['_ASSETSREQUEST']._serialized_end=19630
+  _globals['_ASSETSRESPONSE']._serialized_start=19632
+  _globals['_ASSETSRESPONSE']._serialized_end=19710
+  _globals['_ASSETFULL']._serialized_start=19713
+  _globals['_ASSETFULL']._serialized_end=20377
+  _globals['_ASSET']._serialized_start=20380
+  _globals['_ASSET']._serialized_end=20555
+  _globals['_ASSETCURRENCY']._serialized_start=20557
+  _globals['_ASSETCURRENCY']._serialized_end=20595
+  _globals['_ASSETSECURITY']._serialized_start=20598
+  _globals['_ASSETSECURITY']._serialized_end=21100
+  _globals['_ASSETSHARE']._serialized_start=21103
+  _globals['_ASSETSHARE']._serialized_end=21828
+  _globals['_ASSETBOND']._serialized_start=21831
+  _globals['_ASSETBOND']._serialized_end=22695
+  _globals['_ASSETSTRUCTUREDPRODUCT']._serialized_start=22698
+  _globals['_ASSETSTRUCTUREDPRODUCT']._serialized_end=23370
+  _globals['_ASSETETF']._serialized_start=23373
+  _globals['_ASSETETF']._serialized_end=24741
+  _globals['_ASSETCLEARINGCERTIFICATE']._serialized_start=24743
+  _globals['_ASSETCLEARINGCERTIFICATE']._serialized_end=24862
+  _globals['_BRAND']._serialized_start=24865
+  _globals['_BRAND']._serialized_end=25022
+  _globals['_ASSETINSTRUMENT']._serialized_start=25025
+  _globals['_ASSETINSTRUMENT']._serialized_end=25302
+  _globals['_INSTRUMENTLINK']._serialized_start=25304
+  _globals['_INSTRUMENTLINK']._serialized_end=25358
+  _globals['_GETFAVORITESREQUEST']._serialized_start=25360
+  _globals['_GETFAVORITESREQUEST']._serialized_end=25381
+  _globals['_GETFAVORITESRESPONSE']._serialized_start=25383
+  _globals['_GETFAVORITESRESPONSE']._serialized_end=25494
+  _globals['_FAVORITEINSTRUMENT']._serialized_start=25497
+  _globals['_FAVORITEINSTRUMENT']._serialized_end=25765
+  _globals['_EDITFAVORITESREQUEST']._serialized_start=25768
+  _globals['_EDITFAVORITESREQUEST']._serialized_end=25979
+  _globals['_EDITFAVORITESREQUESTINSTRUMENT']._serialized_start=25981
+  _globals['_EDITFAVORITESREQUESTINSTRUMENT']._serialized_end=26074
+  _globals['_EDITFAVORITESRESPONSE']._serialized_start=26076
+  _globals['_EDITFAVORITESRESPONSE']._serialized_end=26188
+  _globals['_GETCOUNTRIESREQUEST']._serialized_start=26190
+  _globals['_GETCOUNTRIESREQUEST']._serialized_end=26211
+  _globals['_GETCOUNTRIESRESPONSE']._serialized_start=26213
+  _globals['_GETCOUNTRIESRESPONSE']._serialized_end=26310
+  _globals['_INDICATIVESREQUEST']._serialized_start=26312
+  _globals['_INDICATIVESREQUEST']._serialized_end=26332
+  _globals['_INDICATIVESRESPONSE']._serialized_start=26334
+  _globals['_INDICATIVESRESPONSE']._serialized_end=26435
+  _globals['_INDICATIVERESPONSE']._serialized_start=26438
+  _globals['_INDICATIVERESPONSE']._serialized_end=26710
+  _globals['_COUNTRYRESPONSE']._serialized_start=26712
+  _globals['_COUNTRYRESPONSE']._serialized_end=26801
+  _globals['_FINDINSTRUMENTREQUEST']._serialized_start=26804
+  _globals['_FINDINSTRUMENTREQUEST']._serialized_end=27021
+  _globals['_FINDINSTRUMENTRESPONSE']._serialized_start=27023
+  _globals['_FINDINSTRUMENTRESPONSE']._serialized_end=27124
+  _globals['_INSTRUMENTSHORT']._serialized_start=27127
+  _globals['_INSTRUMENTSHORT']._serialized_end=27618
+  _globals['_GETBRANDSREQUEST']._serialized_start=27620
+  _globals['_GETBRANDSREQUEST']._serialized_end=27699
+  _globals['_GETBRANDREQUEST']._serialized_start=27701
+  _globals['_GETBRANDREQUEST']._serialized_end=27736
+  _globals['_GETBRANDSRESPONSE']._serialized_start=27739
+  _globals['_GETBRANDSRESPONSE']._serialized_end=27889
+  _globals['_GETASSETFUNDAMENTALSREQUEST']._serialized_start=27891
+  _globals['_GETASSETFUNDAMENTALSREQUEST']._serialized_end=27942
+  _globals['_GETASSETFUNDAMENTALSRESPONSE']._serialized_start=27945
+  _globals['_GETASSETFUNDAMENTALSRESPONSE']._serialized_end=29862
+  _globals['_GETASSETFUNDAMENTALSRESPONSE_STATISTICRESPONSE']._serialized_start=28087
+  _globals['_GETASSETFUNDAMENTALSRESPONSE_STATISTICRESPONSE']._serialized_end=29862
+  _globals['_GETASSETREPORTSREQUEST']._serialized_start=29865
+  _globals['_GETASSETREPORTSREQUEST']._serialized_end=30026
+  _globals['_GETASSETREPORTSRESPONSE']._serialized_start=30029
+  _globals['_GETASSETREPORTSRESPONSE']._serialized_end=30580
+  _globals['_GETASSETREPORTSRESPONSE_GETASSETREPORTSEVENT']._serialized_start=30158
+  _globals['_GETASSETREPORTSRESPONSE_GETASSETREPORTSEVENT']._serialized_end=30448
+  _globals['_GETASSETREPORTSRESPONSE_ASSETREPORTPERIODTYPE']._serialized_start=30451
+  _globals['_GETASSETREPORTSRESPONSE_ASSETREPORTPERIODTYPE']._serialized_end=30580
+  _globals['_GETCONSENSUSFORECASTSREQUEST']._serialized_start=30582
+  _globals['_GETCONSENSUSFORECASTSREQUEST']._serialized_end=30689
+  _globals['_GETCONSENSUSFORECASTSRESPONSE']._serialized_start=30692
+  _globals['_GETCONSENSUSFORECASTSRESPONSE']._serialized_end=31466
+  _globals['_GETCONSENSUSFORECASTSRESPONSE_CONSENSUSFORECASTSITEM']._serialized_start=30901
+  _globals['_GETCONSENSUSFORECASTSRESPONSE_CONSENSUSFORECASTSITEM']._serialized_end=31466
+  _globals['_GETFORECASTREQUEST']._serialized_start=31468
+  _globals['_GETFORECASTREQUEST']._serialized_end=31511
+  _globals['_GETFORECASTRESPONSE']._serialized_start=31514
+  _globals['_GETFORECASTRESPONSE']._serialized_end=32817
+  _globals['_GETFORECASTRESPONSE_TARGETITEM']._serialized_start=31719
+  _globals['_GETFORECASTRESPONSE_TARGETITEM']._serialized_end=32243
+  _globals['_GETFORECASTRESPONSE_CONSENSUSITEM']._serialized_start=32246
+  _globals['_GETFORECASTRESPONSE_CONSENSUSITEM']._serialized_end=32817
+  _globals['_TRADINGINTERVAL']._serialized_start=32820
+  _globals['_TRADINGINTERVAL']._serialized_end=33044
+  _globals['_TRADINGINTERVAL_TIMEINTERVAL']._serialized_start=32940
+  _globals['_TRADINGINTERVAL_TIMEINTERVAL']._serialized_end=33044
+  _globals['_INSTRUMENTSSERVICE']._serialized_start=35160
+  _globals['_INSTRUMENTSSERVICE']._serialized_end=39623
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/instruments_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,53 @@
 """Низкий уровень риска"""
 RISK_LEVEL_MODERATE: RiskLevel.ValueType  # 2
 """Средний уровень риска"""
 RISK_LEVEL_HIGH: RiskLevel.ValueType  # 3
 """Высокий уровень риска"""
 global___RiskLevel = RiskLevel
 
+class _BondType:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _BondTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BondType.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    BOND_TYPE_UNSPECIFIED: _BondType.ValueType  # 0
+    """Тип облигации не определен."""
+    BOND_TYPE_REPLACED: _BondType.ValueType  # 1
+    """Замещающая облигация."""
+
+class BondType(_BondType, metaclass=_BondTypeEnumTypeWrapper): ...
+
+BOND_TYPE_UNSPECIFIED: BondType.ValueType  # 0
+"""Тип облигации не определен."""
+BOND_TYPE_REPLACED: BondType.ValueType  # 1
+"""Замещающая облигация."""
+global___BondType = BondType
+
+class _InstrumentExchangeType:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _InstrumentExchangeTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_InstrumentExchangeType.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    INSTRUMENT_EXCHANGE_UNSPECIFIED: _InstrumentExchangeType.ValueType  # 0
+    """Площадка торговли не определена."""
+    INSTRUMENT_EXCHANGE_DEALER: _InstrumentExchangeType.ValueType  # 1
+    """Бумага, торгуемая у дилера."""
+
+class InstrumentExchangeType(_InstrumentExchangeType, metaclass=_InstrumentExchangeTypeEnumTypeWrapper):
+    """Площадка торговли"""
+
+INSTRUMENT_EXCHANGE_UNSPECIFIED: InstrumentExchangeType.ValueType  # 0
+"""Площадка торговли не определена."""
+INSTRUMENT_EXCHANGE_DEALER: InstrumentExchangeType.ValueType  # 1
+"""Бумага, торгуемая у дилера."""
+global___InstrumentExchangeType = InstrumentExchangeType
+
 @typing_extensions.final
 class TradingSchedulesRequest(google.protobuf.message.Message):
     """Запрос расписания торгов."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXCHANGE_FIELD_NUMBER: builtins.int
@@ -625,23 +664,30 @@
 @typing_extensions.final
 class InstrumentsRequest(google.protobuf.message.Message):
     """Запрос получения инструментов."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INSTRUMENT_STATUS_FIELD_NUMBER: builtins.int
+    INSTRUMENT_EXCHANGE_FIELD_NUMBER: builtins.int
     instrument_status: global___InstrumentStatus.ValueType
     """Статус запрашиваемых инструментов. Возможные значения: [InstrumentStatus](#instrumentstatus)"""
+    instrument_exchange: global___InstrumentExchangeType.ValueType
+    """Тип площадки торговли. Возможные значения: [InstrumentExchangeType](#instrumentexchangetype)"""
     def __init__(
         self,
         *,
         instrument_status: global___InstrumentStatus.ValueType | None = ...,
+        instrument_exchange: global___InstrumentExchangeType.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_instrument_status", b"_instrument_status", "instrument_status", b"instrument_status"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_instrument_status", b"_instrument_status", "instrument_status", b"instrument_status"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_instrument_exchange", b"_instrument_exchange", "_instrument_status", b"_instrument_status", "instrument_exchange", b"instrument_exchange", "instrument_status", b"instrument_status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_instrument_exchange", b"_instrument_exchange", "_instrument_status", b"_instrument_status", "instrument_exchange", b"instrument_exchange", "instrument_status", b"instrument_status"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_instrument_exchange", b"_instrument_exchange"]) -> typing_extensions.Literal["instrument_exchange"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_instrument_status", b"_instrument_status"]) -> typing_extensions.Literal["instrument_status"] | None: ...
 
 global___InstrumentsRequest = InstrumentsRequest
 
 @typing_extensions.final
 class FilterOptionsRequest(google.protobuf.message.Message):
     """Параметры фильтрации опционов"""
@@ -1462,14 +1508,15 @@
     BLOCKED_TCA_FLAG_FIELD_NUMBER: builtins.int
     SUBORDINATED_FLAG_FIELD_NUMBER: builtins.int
     LIQUIDITY_FLAG_FIELD_NUMBER: builtins.int
     FIRST_1MIN_CANDLE_DATE_FIELD_NUMBER: builtins.int
     FIRST_1DAY_CANDLE_DATE_FIELD_NUMBER: builtins.int
     RISK_LEVEL_FIELD_NUMBER: builtins.int
     BRAND_FIELD_NUMBER: builtins.int
+    BOND_TYPE_FIELD_NUMBER: builtins.int
     figi: builtins.str
     """Figi-идентификатор инструмента."""
     ticker: builtins.str
     """Тикер инструмента."""
     class_code: builtins.str
     """Класс-код (секция торгов)."""
     isin: builtins.str
@@ -1583,14 +1630,16 @@
     def first_1day_candle_date(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Дата первой дневной свечи."""
     risk_level: global___RiskLevel.ValueType
     """Уровень риска."""
     @property
     def brand(self) -> tinkoff.invest.grpc.common_pb2.BrandData:
         """Информация о бренде."""
+    bond_type: global___BondType.ValueType
+    """Тип облигации."""
     def __init__(
         self,
         *,
         figi: builtins.str = ...,
         ticker: builtins.str = ...,
         class_code: builtins.str = ...,
         isin: builtins.str = ...,
@@ -1638,17 +1687,18 @@
         blocked_tca_flag: builtins.bool = ...,
         subordinated_flag: builtins.bool = ...,
         liquidity_flag: builtins.bool = ...,
         first_1min_candle_date: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         first_1day_candle_date: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         risk_level: global___RiskLevel.ValueType = ...,
         brand: tinkoff.invest.grpc.common_pb2.BrandData | None = ...,
+        bond_type: global___BondType.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["aci_value", b"aci_value", "brand", b"brand", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "initial_nominal", b"initial_nominal", "klong", b"klong", "kshort", b"kshort", "maturity_date", b"maturity_date", "min_price_increment", b"min_price_increment", "nominal", b"nominal", "placement_date", b"placement_date", "placement_price", b"placement_price", "state_reg_date", b"state_reg_date"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aci_value", b"aci_value", "amortization_flag", b"amortization_flag", "api_trade_available_flag", b"api_trade_available_flag", "asset_uid", b"asset_uid", "blocked_tca_flag", b"blocked_tca_flag", "brand", b"brand", "buy_available_flag", b"buy_available_flag", "class_code", b"class_code", "country_of_risk", b"country_of_risk", "country_of_risk_name", b"country_of_risk_name", "coupon_quantity_per_year", b"coupon_quantity_per_year", "currency", b"currency", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "exchange", b"exchange", "figi", b"figi", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "floating_coupon_flag", b"floating_coupon_flag", "for_iis_flag", b"for_iis_flag", "for_qual_investor_flag", b"for_qual_investor_flag", "initial_nominal", b"initial_nominal", "isin", b"isin", "issue_kind", b"issue_kind", "issue_size", b"issue_size", "issue_size_plan", b"issue_size_plan", "klong", b"klong", "kshort", b"kshort", "liquidity_flag", b"liquidity_flag", "lot", b"lot", "maturity_date", b"maturity_date", "min_price_increment", b"min_price_increment", "name", b"name", "nominal", b"nominal", "otc_flag", b"otc_flag", "perpetual_flag", b"perpetual_flag", "placement_date", b"placement_date", "placement_price", b"placement_price", "position_uid", b"position_uid", "real_exchange", b"real_exchange", "risk_level", b"risk_level", "sector", b"sector", "sell_available_flag", b"sell_available_flag", "short_enabled_flag", b"short_enabled_flag", "state_reg_date", b"state_reg_date", "subordinated_flag", b"subordinated_flag", "ticker", b"ticker", "trading_status", b"trading_status", "uid", b"uid", "weekend_flag", b"weekend_flag"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["aci_value", b"aci_value", "amortization_flag", b"amortization_flag", "api_trade_available_flag", b"api_trade_available_flag", "asset_uid", b"asset_uid", "blocked_tca_flag", b"blocked_tca_flag", "bond_type", b"bond_type", "brand", b"brand", "buy_available_flag", b"buy_available_flag", "class_code", b"class_code", "country_of_risk", b"country_of_risk", "country_of_risk_name", b"country_of_risk_name", "coupon_quantity_per_year", b"coupon_quantity_per_year", "currency", b"currency", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "exchange", b"exchange", "figi", b"figi", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "floating_coupon_flag", b"floating_coupon_flag", "for_iis_flag", b"for_iis_flag", "for_qual_investor_flag", b"for_qual_investor_flag", "initial_nominal", b"initial_nominal", "isin", b"isin", "issue_kind", b"issue_kind", "issue_size", b"issue_size", "issue_size_plan", b"issue_size_plan", "klong", b"klong", "kshort", b"kshort", "liquidity_flag", b"liquidity_flag", "lot", b"lot", "maturity_date", b"maturity_date", "min_price_increment", b"min_price_increment", "name", b"name", "nominal", b"nominal", "otc_flag", b"otc_flag", "perpetual_flag", b"perpetual_flag", "placement_date", b"placement_date", "placement_price", b"placement_price", "position_uid", b"position_uid", "real_exchange", b"real_exchange", "risk_level", b"risk_level", "sector", b"sector", "sell_available_flag", b"sell_available_flag", "short_enabled_flag", b"short_enabled_flag", "state_reg_date", b"state_reg_date", "subordinated_flag", b"subordinated_flag", "ticker", b"ticker", "trading_status", b"trading_status", "uid", b"uid", "weekend_flag", b"weekend_flag"]) -> None: ...
 
 global___Bond = Bond
 
 @typing_extensions.final
 class Currency(google.protobuf.message.Message):
     """Объект передачи информации о валюте."""
 
@@ -1849,14 +1899,15 @@
     SELL_AVAILABLE_FLAG_FIELD_NUMBER: builtins.int
     MIN_PRICE_INCREMENT_FIELD_NUMBER: builtins.int
     API_TRADE_AVAILABLE_FLAG_FIELD_NUMBER: builtins.int
     UID_FIELD_NUMBER: builtins.int
     REAL_EXCHANGE_FIELD_NUMBER: builtins.int
     POSITION_UID_FIELD_NUMBER: builtins.int
     ASSET_UID_FIELD_NUMBER: builtins.int
+    INSTRUMENT_EXCHANGE_FIELD_NUMBER: builtins.int
     FOR_IIS_FLAG_FIELD_NUMBER: builtins.int
     FOR_QUAL_INVESTOR_FLAG_FIELD_NUMBER: builtins.int
     WEEKEND_FLAG_FIELD_NUMBER: builtins.int
     BLOCKED_TCA_FLAG_FIELD_NUMBER: builtins.int
     LIQUIDITY_FLAG_FIELD_NUMBER: builtins.int
     FIRST_1MIN_CANDLE_DATE_FIELD_NUMBER: builtins.int
     FIRST_1DAY_CANDLE_DATE_FIELD_NUMBER: builtins.int
@@ -1933,14 +1984,16 @@
     """Уникальный идентификатор инструмента."""
     real_exchange: global___RealExchange.ValueType
     """Реальная площадка исполнения расчётов (биржа)."""
     position_uid: builtins.str
     """Уникальный идентификатор позиции инструмента."""
     asset_uid: builtins.str
     """Уникальный идентификатор актива."""
+    instrument_exchange: global___InstrumentExchangeType.ValueType
+    """Тип площадки торговли."""
     for_iis_flag: builtins.bool
     """Признак доступности для ИИС."""
     for_qual_investor_flag: builtins.bool
     """Флаг отображающий доступность торговли инструментом только для квалифицированных инвесторов."""
     weekend_flag: builtins.bool
     """Флаг отображающий доступность торговли инструментом по выходным."""
     blocked_tca_flag: builtins.bool
@@ -1988,25 +2041,26 @@
         sell_available_flag: builtins.bool = ...,
         min_price_increment: tinkoff.invest.grpc.common_pb2.Quotation | None = ...,
         api_trade_available_flag: builtins.bool = ...,
         uid: builtins.str = ...,
         real_exchange: global___RealExchange.ValueType = ...,
         position_uid: builtins.str = ...,
         asset_uid: builtins.str = ...,
+        instrument_exchange: global___InstrumentExchangeType.ValueType = ...,
         for_iis_flag: builtins.bool = ...,
         for_qual_investor_flag: builtins.bool = ...,
         weekend_flag: builtins.bool = ...,
         blocked_tca_flag: builtins.bool = ...,
         liquidity_flag: builtins.bool = ...,
         first_1min_candle_date: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         first_1day_candle_date: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         brand: tinkoff.invest.grpc.common_pb2.BrandData | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["brand", b"brand", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "fixed_commission", b"fixed_commission", "klong", b"klong", "kshort", b"kshort", "min_price_increment", b"min_price_increment", "num_shares", b"num_shares", "released_date", b"released_date"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["api_trade_available_flag", b"api_trade_available_flag", "asset_uid", b"asset_uid", "blocked_tca_flag", b"blocked_tca_flag", "brand", b"brand", "buy_available_flag", b"buy_available_flag", "class_code", b"class_code", "country_of_risk", b"country_of_risk", "country_of_risk_name", b"country_of_risk_name", "currency", b"currency", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "exchange", b"exchange", "figi", b"figi", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "fixed_commission", b"fixed_commission", "focus_type", b"focus_type", "for_iis_flag", b"for_iis_flag", "for_qual_investor_flag", b"for_qual_investor_flag", "isin", b"isin", "klong", b"klong", "kshort", b"kshort", "liquidity_flag", b"liquidity_flag", "lot", b"lot", "min_price_increment", b"min_price_increment", "name", b"name", "num_shares", b"num_shares", "otc_flag", b"otc_flag", "position_uid", b"position_uid", "real_exchange", b"real_exchange", "rebalancing_freq", b"rebalancing_freq", "released_date", b"released_date", "sector", b"sector", "sell_available_flag", b"sell_available_flag", "short_enabled_flag", b"short_enabled_flag", "ticker", b"ticker", "trading_status", b"trading_status", "uid", b"uid", "weekend_flag", b"weekend_flag"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["api_trade_available_flag", b"api_trade_available_flag", "asset_uid", b"asset_uid", "blocked_tca_flag", b"blocked_tca_flag", "brand", b"brand", "buy_available_flag", b"buy_available_flag", "class_code", b"class_code", "country_of_risk", b"country_of_risk", "country_of_risk_name", b"country_of_risk_name", "currency", b"currency", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "exchange", b"exchange", "figi", b"figi", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "fixed_commission", b"fixed_commission", "focus_type", b"focus_type", "for_iis_flag", b"for_iis_flag", "for_qual_investor_flag", b"for_qual_investor_flag", "instrument_exchange", b"instrument_exchange", "isin", b"isin", "klong", b"klong", "kshort", b"kshort", "liquidity_flag", b"liquidity_flag", "lot", b"lot", "min_price_increment", b"min_price_increment", "name", b"name", "num_shares", b"num_shares", "otc_flag", b"otc_flag", "position_uid", b"position_uid", "real_exchange", b"real_exchange", "rebalancing_freq", b"rebalancing_freq", "released_date", b"released_date", "sector", b"sector", "sell_available_flag", b"sell_available_flag", "short_enabled_flag", b"short_enabled_flag", "ticker", b"ticker", "trading_status", b"trading_status", "uid", b"uid", "weekend_flag", b"weekend_flag"]) -> None: ...
 
 global___Etf = Etf
 
 @typing_extensions.final
 class Future(google.protobuf.message.Message):
     """Объект передачи информации о фьючерсе."""
 
@@ -2250,14 +2304,15 @@
     SHARE_TYPE_FIELD_NUMBER: builtins.int
     MIN_PRICE_INCREMENT_FIELD_NUMBER: builtins.int
     API_TRADE_AVAILABLE_FLAG_FIELD_NUMBER: builtins.int
     UID_FIELD_NUMBER: builtins.int
     REAL_EXCHANGE_FIELD_NUMBER: builtins.int
     POSITION_UID_FIELD_NUMBER: builtins.int
     ASSET_UID_FIELD_NUMBER: builtins.int
+    INSTRUMENT_EXCHANGE_FIELD_NUMBER: builtins.int
     FOR_IIS_FLAG_FIELD_NUMBER: builtins.int
     FOR_QUAL_INVESTOR_FLAG_FIELD_NUMBER: builtins.int
     WEEKEND_FLAG_FIELD_NUMBER: builtins.int
     BLOCKED_TCA_FLAG_FIELD_NUMBER: builtins.int
     LIQUIDITY_FLAG_FIELD_NUMBER: builtins.int
     FIRST_1MIN_CANDLE_DATE_FIELD_NUMBER: builtins.int
     FIRST_1DAY_CANDLE_DATE_FIELD_NUMBER: builtins.int
@@ -2335,14 +2390,16 @@
     """Уникальный идентификатор инструмента."""
     real_exchange: global___RealExchange.ValueType
     """Реальная площадка исполнения расчётов (биржа)."""
     position_uid: builtins.str
     """Уникальный идентификатор позиции инструмента."""
     asset_uid: builtins.str
     """Уникальный идентификатор актива."""
+    instrument_exchange: global___InstrumentExchangeType.ValueType
+    """Тип площадки торговли."""
     for_iis_flag: builtins.bool
     """Признак доступности для ИИС."""
     for_qual_investor_flag: builtins.bool
     """Флаг отображающий доступность торговли инструментом только для квалифицированных инвесторов."""
     weekend_flag: builtins.bool
     """Флаг отображающий доступность торговли инструментом по выходным"""
     blocked_tca_flag: builtins.bool
@@ -2391,25 +2448,26 @@
         share_type: global___ShareType.ValueType = ...,
         min_price_increment: tinkoff.invest.grpc.common_pb2.Quotation | None = ...,
         api_trade_available_flag: builtins.bool = ...,
         uid: builtins.str = ...,
         real_exchange: global___RealExchange.ValueType = ...,
         position_uid: builtins.str = ...,
         asset_uid: builtins.str = ...,
+        instrument_exchange: global___InstrumentExchangeType.ValueType = ...,
         for_iis_flag: builtins.bool = ...,
         for_qual_investor_flag: builtins.bool = ...,
         weekend_flag: builtins.bool = ...,
         blocked_tca_flag: builtins.bool = ...,
         liquidity_flag: builtins.bool = ...,
         first_1min_candle_date: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         first_1day_candle_date: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         brand: tinkoff.invest.grpc.common_pb2.BrandData | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["brand", b"brand", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "ipo_date", b"ipo_date", "klong", b"klong", "kshort", b"kshort", "min_price_increment", b"min_price_increment", "nominal", b"nominal"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["api_trade_available_flag", b"api_trade_available_flag", "asset_uid", b"asset_uid", "blocked_tca_flag", b"blocked_tca_flag", "brand", b"brand", "buy_available_flag", b"buy_available_flag", "class_code", b"class_code", "country_of_risk", b"country_of_risk", "country_of_risk_name", b"country_of_risk_name", "currency", b"currency", "div_yield_flag", b"div_yield_flag", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "exchange", b"exchange", "figi", b"figi", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "for_iis_flag", b"for_iis_flag", "for_qual_investor_flag", b"for_qual_investor_flag", "ipo_date", b"ipo_date", "isin", b"isin", "issue_size", b"issue_size", "issue_size_plan", b"issue_size_plan", "klong", b"klong", "kshort", b"kshort", "liquidity_flag", b"liquidity_flag", "lot", b"lot", "min_price_increment", b"min_price_increment", "name", b"name", "nominal", b"nominal", "otc_flag", b"otc_flag", "position_uid", b"position_uid", "real_exchange", b"real_exchange", "sector", b"sector", "sell_available_flag", b"sell_available_flag", "share_type", b"share_type", "short_enabled_flag", b"short_enabled_flag", "ticker", b"ticker", "trading_status", b"trading_status", "uid", b"uid", "weekend_flag", b"weekend_flag"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["api_trade_available_flag", b"api_trade_available_flag", "asset_uid", b"asset_uid", "blocked_tca_flag", b"blocked_tca_flag", "brand", b"brand", "buy_available_flag", b"buy_available_flag", "class_code", b"class_code", "country_of_risk", b"country_of_risk", "country_of_risk_name", b"country_of_risk_name", "currency", b"currency", "div_yield_flag", b"div_yield_flag", "dlong", b"dlong", "dlong_min", b"dlong_min", "dshort", b"dshort", "dshort_min", b"dshort_min", "exchange", b"exchange", "figi", b"figi", "first_1day_candle_date", b"first_1day_candle_date", "first_1min_candle_date", b"first_1min_candle_date", "for_iis_flag", b"for_iis_flag", "for_qual_investor_flag", b"for_qual_investor_flag", "instrument_exchange", b"instrument_exchange", "ipo_date", b"ipo_date", "isin", b"isin", "issue_size", b"issue_size", "issue_size_plan", b"issue_size_plan", "klong", b"klong", "kshort", b"kshort", "liquidity_flag", b"liquidity_flag", "lot", b"lot", "min_price_increment", b"min_price_increment", "name", b"name", "nominal", b"nominal", "otc_flag", b"otc_flag", "position_uid", b"position_uid", "real_exchange", b"real_exchange", "sector", b"sector", "sell_available_flag", b"sell_available_flag", "share_type", b"share_type", "short_enabled_flag", b"short_enabled_flag", "ticker", b"ticker", "trading_status", b"trading_status", "uid", b"uid", "weekend_flag", b"weekend_flag"]) -> None: ...
 
 global___Share = Share
 
 @typing_extensions.final
 class GetAccruedInterestsRequest(google.protobuf.message.Message):
     """Запрос НКД по облигации"""
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/instruments_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/instruments_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/marketdata_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from tinkoff.invest.grpc import (
     common_pb2 as tinkoff_dot_invest_dot_grpc_dot_common__pb2,
 )
 from tinkoff.invest.grpc.google.api import (
     field_behavior_pb2 as tinkoff_dot_invest_dot_grpc_dot_google_dot_api_dot_field__behavior__pb2,
 )
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tinkoff/invest/grpc/marketdata.proto\x12%tinkoff.public.invest.api.contract.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a tinkoff/invest/grpc/common.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"\xf4\x04\n\x11MarketDataRequest\x12\x63\n\x19subscribe_candles_request\x18\x01 \x01(\x0b\x32>.tinkoff.public.invest.api.contract.v1.SubscribeCandlesRequestH\x00\x12h\n\x1csubscribe_order_book_request\x18\x02 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeOrderBookRequestH\x00\x12\x61\n\x18subscribe_trades_request\x18\x03 \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.SubscribeTradesRequestH\x00\x12]\n\x16subscribe_info_request\x18\x04 \x01(\x0b\x32;.tinkoff.public.invest.api.contract.v1.SubscribeInfoRequestH\x00\x12h\n\x1csubscribe_last_price_request\x18\x05 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeLastPriceRequestH\x00\x12Y\n\x14get_my_subscriptions\x18\x06 \x01(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.GetMySubscriptionsH\x00\x42\t\n\x07payload\"\x94\x04\n!MarketDataServerSideStreamRequest\x12\x61\n\x19subscribe_candles_request\x18\x01 \x01(\x0b\x32>.tinkoff.public.invest.api.contract.v1.SubscribeCandlesRequest\x12\x66\n\x1csubscribe_order_book_request\x18\x02 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeOrderBookRequest\x12_\n\x18subscribe_trades_request\x18\x03 \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.SubscribeTradesRequest\x12[\n\x16subscribe_info_request\x18\x04 \x01(\x0b\x32;.tinkoff.public.invest.api.contract.v1.SubscribeInfoRequest\x12\x66\n\x1csubscribe_last_price_request\x18\x05 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeLastPriceRequest\"\xc0\x07\n\x12MarketDataResponse\x12\x65\n\x1asubscribe_candles_response\x18\x01 \x01(\x0b\x32?.tinkoff.public.invest.api.contract.v1.SubscribeCandlesResponseH\x00\x12j\n\x1dsubscribe_order_book_response\x18\x02 \x01(\x0b\x32\x41.tinkoff.public.invest.api.contract.v1.SubscribeOrderBookResponseH\x00\x12\x63\n\x19subscribe_trades_response\x18\x03 \x01(\x0b\x32>.tinkoff.public.invest.api.contract.v1.SubscribeTradesResponseH\x00\x12_\n\x17subscribe_info_response\x18\x04 \x01(\x0b\x32<.tinkoff.public.invest.api.contract.v1.SubscribeInfoResponseH\x00\x12?\n\x06\x63\x61ndle\x18\x05 \x01(\x0b\x32-.tinkoff.public.invest.api.contract.v1.CandleH\x00\x12=\n\x05trade\x18\x06 \x01(\x0b\x32,.tinkoff.public.invest.api.contract.v1.TradeH\x00\x12\x45\n\torderbook\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.OrderBookH\x00\x12N\n\x0etrading_status\x18\x08 \x01(\x0b\x32\x34.tinkoff.public.invest.api.contract.v1.TradingStatusH\x00\x12;\n\x04ping\x18\t \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PingH\x00\x12j\n\x1dsubscribe_last_price_response\x18\n \x01(\x0b\x32\x41.tinkoff.public.invest.api.contract.v1.SubscribeLastPriceResponseH\x00\x12\x46\n\nlast_price\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.LastPriceH\x00\x42\t\n\x07payload\"\xd6\x01\n\x17SubscribeCandlesRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12L\n\x0binstruments\x18\x02 \x03(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.CandleInstrument\x12\x15\n\rwaiting_close\x18\x03 \x01(\x08\"\x8a\x01\n\x10\x43\x61ndleInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12M\n\x08interval\x18\x02 \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.SubscriptionInterval\x12\x15\n\rinstrument_id\x18\x03 \x01(\t\"\x89\x01\n\x18SubscribeCandlesResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12X\n\x15\x63\x61ndles_subscriptions\x18\x02 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.CandleSubscription\"\xa4\x02\n\x12\x43\x61ndleSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12M\n\x08interval\x18\x02 \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.SubscriptionInterval\x12V\n\x13subscription_status\x18\x03 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x04 \x01(\t\x12\x15\n\rwaiting_close\x18\x05 \x01(\x08\x12\x11\n\tstream_id\x18\x06 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x07 \x01(\t\"\xc4\x01\n\x19SubscribeOrderBookRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12O\n\x0binstruments\x18\x02 \x03(\x0b\x32:.tinkoff.public.invest.api.contract.v1.OrderBookInstrument\"\x9c\x01\n\x13OrderBookInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12\x15\n\rinstrument_id\x18\x03 \x01(\t\x12M\n\x0forder_book_type\x18\x04 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.OrderBookType\"\x91\x01\n\x1aSubscribeOrderBookResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12^\n\x18order_book_subscriptions\x18\x02 \x03(\x0b\x32<.tinkoff.public.invest.api.contract.v1.OrderBookSubscription\"\x9f\x02\n\x15OrderBookSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12V\n\x13subscription_status\x18\x03 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x04 \x01(\t\x12\x11\n\tstream_id\x18\x05 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x06 \x01(\t\x12M\n\x0forder_book_type\x18\x07 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.OrderBookType\"\xbd\x01\n\x16SubscribeTradesRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12K\n\x0binstruments\x18\x02 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.TradeInstrument\":\n\x0fTradeInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\"\x85\x01\n\x17SubscribeTradesResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12U\n\x13trade_subscriptions\x18\x02 \x03(\x0b\x32\x38.tinkoff.public.invest.api.contract.v1.TradeSubscription\"\xbd\x01\n\x11TradeSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12V\n\x13subscription_status\x18\x02 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x03 \x01(\t\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x05 \x01(\t\"\xba\x01\n\x14SubscribeInfoRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12J\n\x0binstruments\x18\x02 \x03(\x0b\x32\x35.tinkoff.public.invest.api.contract.v1.InfoInstrument\"9\n\x0eInfoInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\"\x81\x01\n\x15SubscribeInfoResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12S\n\x12info_subscriptions\x18\x02 \x03(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.InfoSubscription\"\xbc\x01\n\x10InfoSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12V\n\x13subscription_status\x18\x02 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x03 \x01(\t\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x05 \x01(\t\"\xc4\x01\n\x19SubscribeLastPriceRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12O\n\x0binstruments\x18\x02 \x03(\x0b\x32:.tinkoff.public.invest.api.contract.v1.LastPriceInstrument\">\n\x13LastPriceInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\"\x91\x01\n\x1aSubscribeLastPriceResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12^\n\x18last_price_subscriptions\x18\x02 \x03(\x0b\x32<.tinkoff.public.invest.api.contract.v1.LastPriceSubscription\"\xc1\x01\n\x15LastPriceSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12V\n\x13subscription_status\x18\x02 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x03 \x01(\t\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x05 \x01(\t\"\xea\x03\n\x06\x43\x61ndle\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12M\n\x08interval\x18\x02 \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.SubscriptionInterval\x12>\n\x04open\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12>\n\x04high\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12=\n\x03low\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x63lose\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x0e\n\x06volume\x18\x07 \x01(\x03\x12(\n\x04time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rlast_trade_ts\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\n \x01(\t\"\xd2\x03\n\tOrderBook\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12\x15\n\ris_consistent\x18\x03 \x01(\x08\x12:\n\x04\x62ids\x18\x04 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12:\n\x04\x61sks\x18\x05 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12(\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x08limit_up\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nlimit_down\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x16\n\x0einstrument_uid\x18\t \x01(\t\x12M\n\x0forder_book_type\x18\n \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.OrderBookType\"Z\n\x05Order\x12?\n\x05price\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x10\n\x08quantity\x18\x02 \x01(\x03\"\xf4\x01\n\x05Trade\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12H\n\tdirection\x18\x02 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.TradeDirection\x12?\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x10\n\x08quantity\x18\x04 \x01(\x03\x12(\n\x04time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\x06 \x01(\t\"\xfe\x01\n\rTradingStatus\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12T\n\x0etrading_status\x18\x02 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12(\n\x04time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x1alimit_order_available_flag\x18\x04 \x01(\x08\x12#\n\x1bmarket_order_available_flag\x18\x05 \x01(\x08\x12\x16\n\x0einstrument_uid\x18\x06 \x01(\t\"\xd8\x03\n\x11GetCandlesRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12.\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12M\n\x08interval\x18\x04 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.CandleIntervalB\x04\xe2\x41\x01\x02\x12\x1a\n\rinstrument_id\x18\x05 \x01(\tH\x01\x88\x01\x01\x12\x66\n\x12\x63\x61ndle_source_type\x18\x07 \x01(\x0e\x32\x45.tinkoff.public.invest.api.contract.v1.GetCandlesRequest.CandleSourceH\x02\x88\x01\x01\"I\n\x0c\x43\x61ndleSource\x12\x1d\n\x19\x43\x41NDLE_SOURCE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x43\x41NDLE_SOURCE_EXCHANGE\x10\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_idB\x15\n\x13_candle_source_type\"\\\n\x12GetCandlesResponse\x12\x46\n\x07\x63\x61ndles\x18\x01 \x03(\x0b\x32\x35.tinkoff.public.invest.api.contract.v1.HistoricCandle\"\xab\x03\n\x0eHistoricCandle\x12>\n\x04open\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12>\n\x04high\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12=\n\x03low\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x63lose\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x0e\n\x06volume\x18\x05 \x01(\x03\x12(\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bis_complete\x18\x07 \x01(\x08\x12J\n\rcandle_source\x18\t \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.CandleSource\"?\n\x14GetLastPricesRequest\x12\x10\n\x04\x66igi\x18\x01 \x03(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x03(\t\"^\n\x15GetLastPricesResponse\x12\x45\n\x0blast_prices\x18\x01 \x03(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.LastPrice\"\x9c\x01\n\tLastPrice\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12?\n\x05price\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12(\n\x04time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\x0b \x01(\t\"x\n\x13GetOrderBookRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x13\n\x05\x64\x65pth\x18\x02 \x01(\x05\x42\x04\xe2\x41\x01\x02\x12\x1a\n\rinstrument_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_id\"\xf3\x04\n\x14GetOrderBookResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12:\n\x04\x62ids\x18\x03 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12:\n\x04\x61sks\x18\x04 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12\x44\n\nlast_price\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\x0b\x63lose_price\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x42\n\x08limit_up\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nlimit_down\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x31\n\rlast_price_ts\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63lose_price_ts\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0corderbook_ts\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\t \x01(\t\"g\n\x17GetTradingStatusRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x1a\n\rinstrument_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_id\"2\n\x19GetTradingStatusesRequest\x12\x15\n\rinstrument_id\x18\x01 \x03(\t\"w\n\x1aGetTradingStatusesResponse\x12Y\n\x10trading_statuses\x18\x01 \x03(\x0b\x32?.tinkoff.public.invest.api.contract.v1.GetTradingStatusResponse\"\xc2\x02\n\x18GetTradingStatusResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12T\n\x0etrading_status\x18\x02 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\"\n\x1alimit_order_available_flag\x18\x03 \x01(\x08\x12#\n\x1bmarket_order_available_flag\x18\x04 \x01(\x08\x12 \n\x18\x61pi_trade_available_flag\x18\x05 \x01(\x08\x12\x16\n\x0einstrument_uid\x18\x06 \x01(\t\x12&\n\x1e\x62\x65stprice_order_available_flag\x18\x08 \x01(\x08\x12\x17\n\x0fonly_best_price\x18\t \x01(\x08\"\xc2\x01\n\x14GetLastTradesRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12.\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12\x1a\n\rinstrument_id\x18\x04 \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_id\"U\n\x15GetLastTradesResponse\x12<\n\x06trades\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Trade\"\x14\n\x12GetMySubscriptions\"v\n\x15GetClosePricesRequest\x12]\n\x0binstruments\x18\x01 \x03(\x0b\x32\x42.tinkoff.public.invest.api.contract.v1.InstrumentClosePriceRequestB\x04\xe2\x41\x01\x02\"4\n\x1bInstrumentClosePriceRequest\x12\x15\n\rinstrument_id\x18\x01 \x01(\t\"s\n\x16GetClosePricesResponse\x12Y\n\x0c\x63lose_prices\x18\x01 \x03(\x0b\x32\x43.tinkoff.public.invest.api.contract.v1.InstrumentClosePriceResponse\"\x80\x02\n\x1cInstrumentClosePriceResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x16\n\x0einstrument_uid\x18\x02 \x01(\t\x12?\n\x05price\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12O\n\x15\x65vening_session_price\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12(\n\x04time\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xf4\x0c\n\x16GetTechAnalysisRequest\x12i\n\x0eindicator_type\x18\x01 \x01(\x0e\x32K.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.IndicatorTypeB\x04\xe2\x41\x01\x02\x12\x1c\n\x0einstrument_uid\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x12.\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12g\n\x08interval\x18\x05 \x01(\x0e\x32O.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.IndicatorIntervalB\x04\xe2\x41\x01\x02\x12\x66\n\rtype_of_price\x18\x06 \x01(\x0e\x32I.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.TypeOfPriceB\x04\xe2\x41\x01\x02\x12\x0e\n\x06length\x18\x07 \x01(\x05\x12Z\n\tdeviation\x18\x08 \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.Deviation\x12Z\n\tsmoothing\x18\t \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.Smoothing\x1aO\n\tSmoothing\x12\x13\n\x0b\x66\x61st_length\x18\x01 \x01(\x05\x12\x13\n\x0bslow_length\x18\x02 \x01(\x05\x12\x18\n\x10signal_smoothing\x18\x03 \x01(\x05\x1a[\n\tDeviation\x12N\n\x14\x64\x65viation_multiplier\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xdb\x03\n\x11IndicatorInterval\x12\"\n\x1eINDICATOR_INTERVAL_UNSPECIFIED\x10\x00\x12!\n\x1dINDICATOR_INTERVAL_ONE_MINUTE\x10\x01\x12#\n\x1fINDICATOR_INTERVAL_FIVE_MINUTES\x10\x02\x12&\n\"INDICATOR_INTERVAL_FIFTEEN_MINUTES\x10\x03\x12\x1f\n\x1bINDICATOR_INTERVAL_ONE_HOUR\x10\x04\x12\x1e\n\x1aINDICATOR_INTERVAL_ONE_DAY\x10\x05\x12\x1c\n\x18INDICATOR_INTERVAL_2_MIN\x10\x06\x12\x1c\n\x18INDICATOR_INTERVAL_3_MIN\x10\x07\x12\x1d\n\x19INDICATOR_INTERVAL_10_MIN\x10\x08\x12\x1d\n\x19INDICATOR_INTERVAL_30_MIN\x10\t\x12\x1d\n\x19INDICATOR_INTERVAL_2_HOUR\x10\n\x12\x1d\n\x19INDICATOR_INTERVAL_4_HOUR\x10\x0b\x12\x1b\n\x17INDICATOR_INTERVAL_WEEK\x10\x0c\x12\x1c\n\x18INDICATOR_INTERVAL_MONTH\x10\r\"\xa3\x01\n\x0bTypeOfPrice\x12\x1d\n\x19TYPE_OF_PRICE_UNSPECIFIED\x10\x00\x12\x17\n\x13TYPE_OF_PRICE_CLOSE\x10\x01\x12\x16\n\x12TYPE_OF_PRICE_OPEN\x10\x02\x12\x16\n\x12TYPE_OF_PRICE_HIGH\x10\x03\x12\x15\n\x11TYPE_OF_PRICE_LOW\x10\x04\x12\x15\n\x11TYPE_OF_PRICE_AVG\x10\x05\"\xa7\x01\n\rIndicatorType\x12\x1e\n\x1aINDICATOR_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11INDICATOR_TYPE_BB\x10\x01\x12\x16\n\x12INDICATOR_TYPE_EMA\x10\x02\x12\x16\n\x12INDICATOR_TYPE_RSI\x10\x03\x12\x17\n\x13INDICATOR_TYPE_MACD\x10\x04\x12\x16\n\x12INDICATOR_TYPE_SMA\x10\x05\"\xfc\x04\n\x17GetTechAnalysisResponse\x12m\n\x14technical_indicators\x18\x01 \x03(\x0b\x32O.tinkoff.public.invest.api.contract.v1.GetTechAnalysisResponse.TechAnalysisItem\x1a\xf1\x03\n\x10TechAnalysisItem\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12J\n\x0bmiddle_band\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x00\x88\x01\x01\x12I\n\nupper_band\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x01\x88\x01\x01\x12I\n\nlower_band\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x02\x88\x01\x01\x12\x45\n\x06signal\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x03\x88\x01\x01\x12\x43\n\x04macd\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x04\x88\x01\x01\x42\x0e\n\x0c_middle_bandB\r\n\x0b_upper_bandB\r\n\x0b_lower_bandB\t\n\x07_signalB\x07\n\x05_macd*\x81\x01\n\x12SubscriptionAction\x12#\n\x1fSUBSCRIPTION_ACTION_UNSPECIFIED\x10\x00\x12!\n\x1dSUBSCRIPTION_ACTION_SUBSCRIBE\x10\x01\x12#\n\x1fSUBSCRIPTION_ACTION_UNSUBSCRIBE\x10\x02*\x88\x04\n\x14SubscriptionInterval\x12%\n!SUBSCRIPTION_INTERVAL_UNSPECIFIED\x10\x00\x12$\n SUBSCRIPTION_INTERVAL_ONE_MINUTE\x10\x01\x12&\n\"SUBSCRIPTION_INTERVAL_FIVE_MINUTES\x10\x02\x12)\n%SUBSCRIPTION_INTERVAL_FIFTEEN_MINUTES\x10\x03\x12\"\n\x1eSUBSCRIPTION_INTERVAL_ONE_HOUR\x10\x04\x12!\n\x1dSUBSCRIPTION_INTERVAL_ONE_DAY\x10\x05\x12\x1f\n\x1bSUBSCRIPTION_INTERVAL_2_MIN\x10\x06\x12\x1f\n\x1bSUBSCRIPTION_INTERVAL_3_MIN\x10\x07\x12 \n\x1cSUBSCRIPTION_INTERVAL_10_MIN\x10\x08\x12 \n\x1cSUBSCRIPTION_INTERVAL_30_MIN\x10\t\x12 \n\x1cSUBSCRIPTION_INTERVAL_2_HOUR\x10\n\x12 \n\x1cSUBSCRIPTION_INTERVAL_4_HOUR\x10\x0b\x12\x1e\n\x1aSUBSCRIPTION_INTERVAL_WEEK\x10\x0c\x12\x1f\n\x1bSUBSCRIPTION_INTERVAL_MONTH\x10\r*\xc5\x03\n\x12SubscriptionStatus\x12#\n\x1fSUBSCRIPTION_STATUS_UNSPECIFIED\x10\x00\x12\x1f\n\x1bSUBSCRIPTION_STATUS_SUCCESS\x10\x01\x12,\n(SUBSCRIPTION_STATUS_INSTRUMENT_NOT_FOUND\x10\x02\x12\x36\n2SUBSCRIPTION_STATUS_SUBSCRIPTION_ACTION_IS_INVALID\x10\x03\x12(\n$SUBSCRIPTION_STATUS_DEPTH_IS_INVALID\x10\x04\x12+\n\'SUBSCRIPTION_STATUS_INTERVAL_IS_INVALID\x10\x05\x12)\n%SUBSCRIPTION_STATUS_LIMIT_IS_EXCEEDED\x10\x06\x12&\n\"SUBSCRIPTION_STATUS_INTERNAL_ERROR\x10\x07\x12)\n%SUBSCRIPTION_STATUS_TOO_MANY_REQUESTS\x10\x08\x12.\n*SUBSCRIPTION_STATUS_SUBSCRIPTION_NOT_FOUND\x10\t*d\n\x0eTradeDirection\x12\x1f\n\x1bTRADE_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13TRADE_DIRECTION_BUY\x10\x01\x12\x18\n\x14TRADE_DIRECTION_SELL\x10\x02*\x91\x03\n\x0e\x43\x61ndleInterval\x12\x1f\n\x1b\x43\x41NDLE_INTERVAL_UNSPECIFIED\x10\x00\x12\x19\n\x15\x43\x41NDLE_INTERVAL_1_MIN\x10\x01\x12\x19\n\x15\x43\x41NDLE_INTERVAL_5_MIN\x10\x02\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_15_MIN\x10\x03\x12\x18\n\x14\x43\x41NDLE_INTERVAL_HOUR\x10\x04\x12\x17\n\x13\x43\x41NDLE_INTERVAL_DAY\x10\x05\x12\x19\n\x15\x43\x41NDLE_INTERVAL_2_MIN\x10\x06\x12\x19\n\x15\x43\x41NDLE_INTERVAL_3_MIN\x10\x07\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_10_MIN\x10\x08\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_30_MIN\x10\t\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_2_HOUR\x10\n\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_4_HOUR\x10\x0b\x12\x18\n\x14\x43\x41NDLE_INTERVAL_WEEK\x10\x0c\x12\x19\n\x15\x43\x41NDLE_INTERVAL_MONTH\x10\r*k\n\x0c\x43\x61ndleSource\x12\x1d\n\x19\x43\x41NDLE_SOURCE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x43\x41NDLE_SOURCE_EXCHANGE\x10\x01\x12 \n\x1c\x43\x41NDLE_SOURCE_DEALER_WEEKEND\x10\x02*g\n\rOrderBookType\x12\x1e\n\x1aORDERBOOK_TYPE_UNSPECIFIED\x10\x00\x12\x1b\n\x17ORDERBOOK_TYPE_EXCHANGE\x10\x01\x12\x19\n\x15ORDERBOOK_TYPE_DEALER\x10\x02\x32\x90\t\n\x11MarketDataService\x12\x81\x01\n\nGetCandles\x12\x38.tinkoff.public.invest.api.contract.v1.GetCandlesRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.GetCandlesResponse\x12\x8a\x01\n\rGetLastPrices\x12;.tinkoff.public.invest.api.contract.v1.GetLastPricesRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetLastPricesResponse\x12\x87\x01\n\x0cGetOrderBook\x12:.tinkoff.public.invest.api.contract.v1.GetOrderBookRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetOrderBookResponse\x12\x93\x01\n\x10GetTradingStatus\x12>.tinkoff.public.invest.api.contract.v1.GetTradingStatusRequest\x1a?.tinkoff.public.invest.api.contract.v1.GetTradingStatusResponse\x12\x99\x01\n\x12GetTradingStatuses\x12@.tinkoff.public.invest.api.contract.v1.GetTradingStatusesRequest\x1a\x41.tinkoff.public.invest.api.contract.v1.GetTradingStatusesResponse\x12\x8a\x01\n\rGetLastTrades\x12;.tinkoff.public.invest.api.contract.v1.GetLastTradesRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetLastTradesResponse\x12\x8d\x01\n\x0eGetClosePrices\x12<.tinkoff.public.invest.api.contract.v1.GetClosePricesRequest\x1a=.tinkoff.public.invest.api.contract.v1.GetClosePricesResponse\x12\x90\x01\n\x0fGetTechAnalysis\x12=.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest\x1a>.tinkoff.public.invest.api.contract.v1.GetTechAnalysisResponse2\xcd\x02\n\x17MarketDataStreamService\x12\x8b\x01\n\x10MarketDataStream\x12\x38.tinkoff.public.invest.api.contract.v1.MarketDataRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.MarketDataResponse(\x01\x30\x01\x12\xa3\x01\n\x1aMarketDataServerSideStream\x12H.tinkoff.public.invest.api.contract.v1.MarketDataServerSideStreamRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.MarketDataResponse0\x01\x42\x61\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tinkoff/invest/grpc/marketdata.proto\x12%tinkoff.public.invest.api.contract.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a tinkoff/invest/grpc/common.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"\xf4\x04\n\x11MarketDataRequest\x12\x63\n\x19subscribe_candles_request\x18\x01 \x01(\x0b\x32>.tinkoff.public.invest.api.contract.v1.SubscribeCandlesRequestH\x00\x12h\n\x1csubscribe_order_book_request\x18\x02 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeOrderBookRequestH\x00\x12\x61\n\x18subscribe_trades_request\x18\x03 \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.SubscribeTradesRequestH\x00\x12]\n\x16subscribe_info_request\x18\x04 \x01(\x0b\x32;.tinkoff.public.invest.api.contract.v1.SubscribeInfoRequestH\x00\x12h\n\x1csubscribe_last_price_request\x18\x05 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeLastPriceRequestH\x00\x12Y\n\x14get_my_subscriptions\x18\x06 \x01(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.GetMySubscriptionsH\x00\x42\t\n\x07payload\"\x94\x04\n!MarketDataServerSideStreamRequest\x12\x61\n\x19subscribe_candles_request\x18\x01 \x01(\x0b\x32>.tinkoff.public.invest.api.contract.v1.SubscribeCandlesRequest\x12\x66\n\x1csubscribe_order_book_request\x18\x02 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeOrderBookRequest\x12_\n\x18subscribe_trades_request\x18\x03 \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.SubscribeTradesRequest\x12[\n\x16subscribe_info_request\x18\x04 \x01(\x0b\x32;.tinkoff.public.invest.api.contract.v1.SubscribeInfoRequest\x12\x66\n\x1csubscribe_last_price_request\x18\x05 \x01(\x0b\x32@.tinkoff.public.invest.api.contract.v1.SubscribeLastPriceRequest\"\xc0\x07\n\x12MarketDataResponse\x12\x65\n\x1asubscribe_candles_response\x18\x01 \x01(\x0b\x32?.tinkoff.public.invest.api.contract.v1.SubscribeCandlesResponseH\x00\x12j\n\x1dsubscribe_order_book_response\x18\x02 \x01(\x0b\x32\x41.tinkoff.public.invest.api.contract.v1.SubscribeOrderBookResponseH\x00\x12\x63\n\x19subscribe_trades_response\x18\x03 \x01(\x0b\x32>.tinkoff.public.invest.api.contract.v1.SubscribeTradesResponseH\x00\x12_\n\x17subscribe_info_response\x18\x04 \x01(\x0b\x32<.tinkoff.public.invest.api.contract.v1.SubscribeInfoResponseH\x00\x12?\n\x06\x63\x61ndle\x18\x05 \x01(\x0b\x32-.tinkoff.public.invest.api.contract.v1.CandleH\x00\x12=\n\x05trade\x18\x06 \x01(\x0b\x32,.tinkoff.public.invest.api.contract.v1.TradeH\x00\x12\x45\n\torderbook\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.OrderBookH\x00\x12N\n\x0etrading_status\x18\x08 \x01(\x0b\x32\x34.tinkoff.public.invest.api.contract.v1.TradingStatusH\x00\x12;\n\x04ping\x18\t \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PingH\x00\x12j\n\x1dsubscribe_last_price_response\x18\n \x01(\x0b\x32\x41.tinkoff.public.invest.api.contract.v1.SubscribeLastPriceResponseH\x00\x12\x46\n\nlast_price\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.LastPriceH\x00\x42\t\n\x07payload\"\xd6\x01\n\x17SubscribeCandlesRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12L\n\x0binstruments\x18\x02 \x03(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.CandleInstrument\x12\x15\n\rwaiting_close\x18\x03 \x01(\x08\"\x8a\x01\n\x10\x43\x61ndleInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12M\n\x08interval\x18\x02 \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.SubscriptionInterval\x12\x15\n\rinstrument_id\x18\x03 \x01(\t\"\x89\x01\n\x18SubscribeCandlesResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12X\n\x15\x63\x61ndles_subscriptions\x18\x02 \x03(\x0b\x32\x39.tinkoff.public.invest.api.contract.v1.CandleSubscription\"\xa4\x02\n\x12\x43\x61ndleSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12M\n\x08interval\x18\x02 \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.SubscriptionInterval\x12V\n\x13subscription_status\x18\x03 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x04 \x01(\t\x12\x15\n\rwaiting_close\x18\x05 \x01(\x08\x12\x11\n\tstream_id\x18\x06 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x07 \x01(\t\"\xc4\x01\n\x19SubscribeOrderBookRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12O\n\x0binstruments\x18\x02 \x03(\x0b\x32:.tinkoff.public.invest.api.contract.v1.OrderBookInstrument\"\x9c\x01\n\x13OrderBookInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12\x15\n\rinstrument_id\x18\x03 \x01(\t\x12M\n\x0forder_book_type\x18\x04 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.OrderBookType\"\x91\x01\n\x1aSubscribeOrderBookResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12^\n\x18order_book_subscriptions\x18\x02 \x03(\x0b\x32<.tinkoff.public.invest.api.contract.v1.OrderBookSubscription\"\x9f\x02\n\x15OrderBookSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12V\n\x13subscription_status\x18\x03 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x04 \x01(\t\x12\x11\n\tstream_id\x18\x05 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x06 \x01(\t\x12M\n\x0forder_book_type\x18\x07 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.OrderBookType\"\x89\x02\n\x16SubscribeTradesRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12K\n\x0binstruments\x18\x02 \x03(\x0b\x32\x36.tinkoff.public.invest.api.contract.v1.TradeInstrument\x12J\n\ntrade_type\x18\x03 \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.TradeSourceType\":\n\x0fTradeInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\"\xd1\x01\n\x17SubscribeTradesResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12U\n\x13trade_subscriptions\x18\x02 \x03(\x0b\x32\x38.tinkoff.public.invest.api.contract.v1.TradeSubscription\x12J\n\ntrade_type\x18\x03 \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.TradeSourceType\"\xbd\x01\n\x11TradeSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12V\n\x13subscription_status\x18\x02 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x03 \x01(\t\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x05 \x01(\t\"\xba\x01\n\x14SubscribeInfoRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12J\n\x0binstruments\x18\x02 \x03(\x0b\x32\x35.tinkoff.public.invest.api.contract.v1.InfoInstrument\"9\n\x0eInfoInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\"\x81\x01\n\x15SubscribeInfoResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12S\n\x12info_subscriptions\x18\x02 \x03(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.InfoSubscription\"\xbc\x01\n\x10InfoSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12V\n\x13subscription_status\x18\x02 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x03 \x01(\t\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x05 \x01(\t\"\xc4\x01\n\x19SubscribeLastPriceRequest\x12V\n\x13subscription_action\x18\x01 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionAction\x12O\n\x0binstruments\x18\x02 \x03(\x0b\x32:.tinkoff.public.invest.api.contract.v1.LastPriceInstrument\">\n\x13LastPriceInstrument\x12\x10\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\"\x91\x01\n\x1aSubscribeLastPriceResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12^\n\x18last_price_subscriptions\x18\x02 \x03(\x0b\x32<.tinkoff.public.invest.api.contract.v1.LastPriceSubscription\"\xc1\x01\n\x15LastPriceSubscription\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12V\n\x13subscription_status\x18\x02 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.SubscriptionStatus\x12\x16\n\x0einstrument_uid\x18\x03 \x01(\t\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x17\n\x0fsubscription_id\x18\x05 \x01(\t\"\xea\x03\n\x06\x43\x61ndle\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12M\n\x08interval\x18\x02 \x01(\x0e\x32;.tinkoff.public.invest.api.contract.v1.SubscriptionInterval\x12>\n\x04open\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12>\n\x04high\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12=\n\x03low\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x63lose\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x0e\n\x06volume\x18\x07 \x01(\x03\x12(\n\x04time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rlast_trade_ts\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\n \x01(\t\"\xd2\x03\n\tOrderBook\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12\x15\n\ris_consistent\x18\x03 \x01(\x08\x12:\n\x04\x62ids\x18\x04 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12:\n\x04\x61sks\x18\x05 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12(\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x08limit_up\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nlimit_down\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x16\n\x0einstrument_uid\x18\t \x01(\t\x12M\n\x0forder_book_type\x18\n \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.OrderBookType\"Z\n\x05Order\x12?\n\x05price\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x10\n\x08quantity\x18\x02 \x01(\x03\"\xc1\x02\n\x05Trade\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12H\n\tdirection\x18\x02 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.TradeDirection\x12?\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x10\n\x08quantity\x18\x04 \x01(\x03\x12(\n\x04time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\x06 \x01(\t\x12K\n\x0btradeSource\x18\x07 \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.TradeSourceType\"\xfe\x01\n\rTradingStatus\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12T\n\x0etrading_status\x18\x02 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12(\n\x04time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x1alimit_order_available_flag\x18\x04 \x01(\x08\x12#\n\x1bmarket_order_available_flag\x18\x05 \x01(\x08\x12\x16\n\x0einstrument_uid\x18\x06 \x01(\t\"\xd8\x03\n\x11GetCandlesRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12.\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12M\n\x08interval\x18\x04 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.CandleIntervalB\x04\xe2\x41\x01\x02\x12\x1a\n\rinstrument_id\x18\x05 \x01(\tH\x01\x88\x01\x01\x12\x66\n\x12\x63\x61ndle_source_type\x18\x07 \x01(\x0e\x32\x45.tinkoff.public.invest.api.contract.v1.GetCandlesRequest.CandleSourceH\x02\x88\x01\x01\"I\n\x0c\x43\x61ndleSource\x12\x1d\n\x19\x43\x41NDLE_SOURCE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x43\x41NDLE_SOURCE_EXCHANGE\x10\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_idB\x15\n\x13_candle_source_type\"\\\n\x12GetCandlesResponse\x12\x46\n\x07\x63\x61ndles\x18\x01 \x03(\x0b\x32\x35.tinkoff.public.invest.api.contract.v1.HistoricCandle\"\xab\x03\n\x0eHistoricCandle\x12>\n\x04open\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12>\n\x04high\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12=\n\x03low\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12?\n\x05\x63lose\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x0e\n\x06volume\x18\x05 \x01(\x03\x12(\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bis_complete\x18\x07 \x01(\x08\x12J\n\rcandle_source\x18\t \x01(\x0e\x32\x33.tinkoff.public.invest.api.contract.v1.CandleSource\"?\n\x14GetLastPricesRequest\x12\x10\n\x04\x66igi\x18\x01 \x03(\tB\x02\x18\x01\x12\x15\n\rinstrument_id\x18\x02 \x03(\t\"^\n\x15GetLastPricesResponse\x12\x45\n\x0blast_prices\x18\x01 \x03(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.LastPrice\"\x9c\x01\n\tLastPrice\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12?\n\x05price\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12(\n\x04time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\x0b \x01(\t\"x\n\x13GetOrderBookRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x13\n\x05\x64\x65pth\x18\x02 \x01(\x05\x42\x04\xe2\x41\x01\x02\x12\x1a\n\rinstrument_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_id\"\xf3\x04\n\x14GetOrderBookResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\r\n\x05\x64\x65pth\x18\x02 \x01(\x05\x12:\n\x04\x62ids\x18\x03 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12:\n\x04\x61sks\x18\x04 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Order\x12\x44\n\nlast_price\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x45\n\x0b\x63lose_price\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x42\n\x08limit_up\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x44\n\nlimit_down\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x31\n\rlast_price_ts\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63lose_price_ts\x18\x16 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0corderbook_ts\x18\x17 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\t \x01(\t\"g\n\x17GetTradingStatusRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x1a\n\rinstrument_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_id\"2\n\x19GetTradingStatusesRequest\x12\x15\n\rinstrument_id\x18\x01 \x03(\t\"w\n\x1aGetTradingStatusesResponse\x12Y\n\x10trading_statuses\x18\x01 \x03(\x0b\x32?.tinkoff.public.invest.api.contract.v1.GetTradingStatusResponse\"\xc2\x02\n\x18GetTradingStatusResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12T\n\x0etrading_status\x18\x02 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.SecurityTradingStatus\x12\"\n\x1alimit_order_available_flag\x18\x03 \x01(\x08\x12#\n\x1bmarket_order_available_flag\x18\x04 \x01(\x08\x12 \n\x18\x61pi_trade_available_flag\x18\x05 \x01(\x08\x12\x16\n\x0einstrument_uid\x18\x06 \x01(\t\x12&\n\x1e\x62\x65stprice_order_available_flag\x18\x08 \x01(\x08\x12\x17\n\x0fonly_best_price\x18\t \x01(\x08\"\xc2\x01\n\x14GetLastTradesRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12.\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12\x1a\n\rinstrument_id\x18\x04 \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_figiB\x10\n\x0e_instrument_id\"U\n\x15GetLastTradesResponse\x12<\n\x06trades\x18\x01 \x03(\x0b\x32,.tinkoff.public.invest.api.contract.v1.Trade\"\x14\n\x12GetMySubscriptions\"v\n\x15GetClosePricesRequest\x12]\n\x0binstruments\x18\x01 \x03(\x0b\x32\x42.tinkoff.public.invest.api.contract.v1.InstrumentClosePriceRequestB\x04\xe2\x41\x01\x02\"4\n\x1bInstrumentClosePriceRequest\x12\x15\n\rinstrument_id\x18\x01 \x01(\t\"s\n\x16GetClosePricesResponse\x12Y\n\x0c\x63lose_prices\x18\x01 \x03(\x0b\x32\x43.tinkoff.public.invest.api.contract.v1.InstrumentClosePriceResponse\"\x80\x02\n\x1cInstrumentClosePriceResponse\x12\x0c\n\x04\x66igi\x18\x01 \x01(\t\x12\x16\n\x0einstrument_uid\x18\x02 \x01(\t\x12?\n\x05price\x18\x0b \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12O\n\x15\x65vening_session_price\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12(\n\x04time\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xf4\x0c\n\x16GetTechAnalysisRequest\x12i\n\x0eindicator_type\x18\x01 \x01(\x0e\x32K.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.IndicatorTypeB\x04\xe2\x41\x01\x02\x12\x1c\n\x0einstrument_uid\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x12.\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12,\n\x02to\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x04\xe2\x41\x01\x02\x12g\n\x08interval\x18\x05 \x01(\x0e\x32O.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.IndicatorIntervalB\x04\xe2\x41\x01\x02\x12\x66\n\rtype_of_price\x18\x06 \x01(\x0e\x32I.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.TypeOfPriceB\x04\xe2\x41\x01\x02\x12\x0e\n\x06length\x18\x07 \x01(\x05\x12Z\n\tdeviation\x18\x08 \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.Deviation\x12Z\n\tsmoothing\x18\t \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest.Smoothing\x1aO\n\tSmoothing\x12\x13\n\x0b\x66\x61st_length\x18\x01 \x01(\x05\x12\x13\n\x0bslow_length\x18\x02 \x01(\x05\x12\x18\n\x10signal_smoothing\x18\x03 \x01(\x05\x1a[\n\tDeviation\x12N\n\x14\x64\x65viation_multiplier\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\"\xdb\x03\n\x11IndicatorInterval\x12\"\n\x1eINDICATOR_INTERVAL_UNSPECIFIED\x10\x00\x12!\n\x1dINDICATOR_INTERVAL_ONE_MINUTE\x10\x01\x12#\n\x1fINDICATOR_INTERVAL_FIVE_MINUTES\x10\x02\x12&\n\"INDICATOR_INTERVAL_FIFTEEN_MINUTES\x10\x03\x12\x1f\n\x1bINDICATOR_INTERVAL_ONE_HOUR\x10\x04\x12\x1e\n\x1aINDICATOR_INTERVAL_ONE_DAY\x10\x05\x12\x1c\n\x18INDICATOR_INTERVAL_2_MIN\x10\x06\x12\x1c\n\x18INDICATOR_INTERVAL_3_MIN\x10\x07\x12\x1d\n\x19INDICATOR_INTERVAL_10_MIN\x10\x08\x12\x1d\n\x19INDICATOR_INTERVAL_30_MIN\x10\t\x12\x1d\n\x19INDICATOR_INTERVAL_2_HOUR\x10\n\x12\x1d\n\x19INDICATOR_INTERVAL_4_HOUR\x10\x0b\x12\x1b\n\x17INDICATOR_INTERVAL_WEEK\x10\x0c\x12\x1c\n\x18INDICATOR_INTERVAL_MONTH\x10\r\"\xa3\x01\n\x0bTypeOfPrice\x12\x1d\n\x19TYPE_OF_PRICE_UNSPECIFIED\x10\x00\x12\x17\n\x13TYPE_OF_PRICE_CLOSE\x10\x01\x12\x16\n\x12TYPE_OF_PRICE_OPEN\x10\x02\x12\x16\n\x12TYPE_OF_PRICE_HIGH\x10\x03\x12\x15\n\x11TYPE_OF_PRICE_LOW\x10\x04\x12\x15\n\x11TYPE_OF_PRICE_AVG\x10\x05\"\xa7\x01\n\rIndicatorType\x12\x1e\n\x1aINDICATOR_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11INDICATOR_TYPE_BB\x10\x01\x12\x16\n\x12INDICATOR_TYPE_EMA\x10\x02\x12\x16\n\x12INDICATOR_TYPE_RSI\x10\x03\x12\x17\n\x13INDICATOR_TYPE_MACD\x10\x04\x12\x16\n\x12INDICATOR_TYPE_SMA\x10\x05\"\xfc\x04\n\x17GetTechAnalysisResponse\x12m\n\x14technical_indicators\x18\x01 \x03(\x0b\x32O.tinkoff.public.invest.api.contract.v1.GetTechAnalysisResponse.TechAnalysisItem\x1a\xf1\x03\n\x10TechAnalysisItem\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12J\n\x0bmiddle_band\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x00\x88\x01\x01\x12I\n\nupper_band\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x01\x88\x01\x01\x12I\n\nlower_band\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x02\x88\x01\x01\x12\x45\n\x06signal\x18\x05 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x03\x88\x01\x01\x12\x43\n\x04macd\x18\x06 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x04\x88\x01\x01\x42\x0e\n\x0c_middle_bandB\r\n\x0b_upper_bandB\r\n\x0b_lower_bandB\t\n\x07_signalB\x07\n\x05_macd*\x81\x01\n\x12SubscriptionAction\x12#\n\x1fSUBSCRIPTION_ACTION_UNSPECIFIED\x10\x00\x12!\n\x1dSUBSCRIPTION_ACTION_SUBSCRIBE\x10\x01\x12#\n\x1fSUBSCRIPTION_ACTION_UNSUBSCRIBE\x10\x02*\x88\x04\n\x14SubscriptionInterval\x12%\n!SUBSCRIPTION_INTERVAL_UNSPECIFIED\x10\x00\x12$\n SUBSCRIPTION_INTERVAL_ONE_MINUTE\x10\x01\x12&\n\"SUBSCRIPTION_INTERVAL_FIVE_MINUTES\x10\x02\x12)\n%SUBSCRIPTION_INTERVAL_FIFTEEN_MINUTES\x10\x03\x12\"\n\x1eSUBSCRIPTION_INTERVAL_ONE_HOUR\x10\x04\x12!\n\x1dSUBSCRIPTION_INTERVAL_ONE_DAY\x10\x05\x12\x1f\n\x1bSUBSCRIPTION_INTERVAL_2_MIN\x10\x06\x12\x1f\n\x1bSUBSCRIPTION_INTERVAL_3_MIN\x10\x07\x12 \n\x1cSUBSCRIPTION_INTERVAL_10_MIN\x10\x08\x12 \n\x1cSUBSCRIPTION_INTERVAL_30_MIN\x10\t\x12 \n\x1cSUBSCRIPTION_INTERVAL_2_HOUR\x10\n\x12 \n\x1cSUBSCRIPTION_INTERVAL_4_HOUR\x10\x0b\x12\x1e\n\x1aSUBSCRIPTION_INTERVAL_WEEK\x10\x0c\x12\x1f\n\x1bSUBSCRIPTION_INTERVAL_MONTH\x10\r*\xc5\x03\n\x12SubscriptionStatus\x12#\n\x1fSUBSCRIPTION_STATUS_UNSPECIFIED\x10\x00\x12\x1f\n\x1bSUBSCRIPTION_STATUS_SUCCESS\x10\x01\x12,\n(SUBSCRIPTION_STATUS_INSTRUMENT_NOT_FOUND\x10\x02\x12\x36\n2SUBSCRIPTION_STATUS_SUBSCRIPTION_ACTION_IS_INVALID\x10\x03\x12(\n$SUBSCRIPTION_STATUS_DEPTH_IS_INVALID\x10\x04\x12+\n\'SUBSCRIPTION_STATUS_INTERVAL_IS_INVALID\x10\x05\x12)\n%SUBSCRIPTION_STATUS_LIMIT_IS_EXCEEDED\x10\x06\x12&\n\"SUBSCRIPTION_STATUS_INTERNAL_ERROR\x10\x07\x12)\n%SUBSCRIPTION_STATUS_TOO_MANY_REQUESTS\x10\x08\x12.\n*SUBSCRIPTION_STATUS_SUBSCRIPTION_NOT_FOUND\x10\t*y\n\x0fTradeSourceType\x12\x1c\n\x18TRADE_SOURCE_UNSPECIFIED\x10\x00\x12\x19\n\x15TRADE_SOURCE_EXCHANGE\x10\x01\x12\x17\n\x13TRADE_SOURCE_DEALER\x10\x02\x12\x14\n\x10TRADE_SOURCE_ALL\x10\x03*d\n\x0eTradeDirection\x12\x1f\n\x1bTRADE_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13TRADE_DIRECTION_BUY\x10\x01\x12\x18\n\x14TRADE_DIRECTION_SELL\x10\x02*\x91\x03\n\x0e\x43\x61ndleInterval\x12\x1f\n\x1b\x43\x41NDLE_INTERVAL_UNSPECIFIED\x10\x00\x12\x19\n\x15\x43\x41NDLE_INTERVAL_1_MIN\x10\x01\x12\x19\n\x15\x43\x41NDLE_INTERVAL_5_MIN\x10\x02\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_15_MIN\x10\x03\x12\x18\n\x14\x43\x41NDLE_INTERVAL_HOUR\x10\x04\x12\x17\n\x13\x43\x41NDLE_INTERVAL_DAY\x10\x05\x12\x19\n\x15\x43\x41NDLE_INTERVAL_2_MIN\x10\x06\x12\x19\n\x15\x43\x41NDLE_INTERVAL_3_MIN\x10\x07\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_10_MIN\x10\x08\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_30_MIN\x10\t\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_2_HOUR\x10\n\x12\x1a\n\x16\x43\x41NDLE_INTERVAL_4_HOUR\x10\x0b\x12\x18\n\x14\x43\x41NDLE_INTERVAL_WEEK\x10\x0c\x12\x19\n\x15\x43\x41NDLE_INTERVAL_MONTH\x10\r*k\n\x0c\x43\x61ndleSource\x12\x1d\n\x19\x43\x41NDLE_SOURCE_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x43\x41NDLE_SOURCE_EXCHANGE\x10\x01\x12 \n\x1c\x43\x41NDLE_SOURCE_DEALER_WEEKEND\x10\x02*g\n\rOrderBookType\x12\x1e\n\x1aORDERBOOK_TYPE_UNSPECIFIED\x10\x00\x12\x1b\n\x17ORDERBOOK_TYPE_EXCHANGE\x10\x01\x12\x19\n\x15ORDERBOOK_TYPE_DEALER\x10\x02\x32\x90\t\n\x11MarketDataService\x12\x81\x01\n\nGetCandles\x12\x38.tinkoff.public.invest.api.contract.v1.GetCandlesRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.GetCandlesResponse\x12\x8a\x01\n\rGetLastPrices\x12;.tinkoff.public.invest.api.contract.v1.GetLastPricesRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetLastPricesResponse\x12\x87\x01\n\x0cGetOrderBook\x12:.tinkoff.public.invest.api.contract.v1.GetOrderBookRequest\x1a;.tinkoff.public.invest.api.contract.v1.GetOrderBookResponse\x12\x93\x01\n\x10GetTradingStatus\x12>.tinkoff.public.invest.api.contract.v1.GetTradingStatusRequest\x1a?.tinkoff.public.invest.api.contract.v1.GetTradingStatusResponse\x12\x99\x01\n\x12GetTradingStatuses\x12@.tinkoff.public.invest.api.contract.v1.GetTradingStatusesRequest\x1a\x41.tinkoff.public.invest.api.contract.v1.GetTradingStatusesResponse\x12\x8a\x01\n\rGetLastTrades\x12;.tinkoff.public.invest.api.contract.v1.GetLastTradesRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetLastTradesResponse\x12\x8d\x01\n\x0eGetClosePrices\x12<.tinkoff.public.invest.api.contract.v1.GetClosePricesRequest\x1a=.tinkoff.public.invest.api.contract.v1.GetClosePricesResponse\x12\x90\x01\n\x0fGetTechAnalysis\x12=.tinkoff.public.invest.api.contract.v1.GetTechAnalysisRequest\x1a>.tinkoff.public.invest.api.contract.v1.GetTechAnalysisResponse2\xcd\x02\n\x17MarketDataStreamService\x12\x8b\x01\n\x10MarketDataStream\x12\x38.tinkoff.public.invest.api.contract.v1.MarketDataRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.MarketDataResponse(\x01\x30\x01\x12\xa3\x01\n\x1aMarketDataServerSideStream\x12H.tinkoff.public.invest.api.contract.v1.MarketDataServerSideStreamRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.MarketDataResponse0\x01\x42\x61\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tinkoff.invest.grpc.marketdata_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034ru.tinkoff.piapi.contract.v1P\001Z\014./;investapi\242\002\005TIAPI\252\002\024Tinkoff.InvestApi.V1\312\002\021Tinkoff\\Invest\\V1'
@@ -73,28 +73,30 @@
   _GETTECHANALYSISREQUEST.fields_by_name['from']._serialized_options = b'\342A\001\002'
   _GETTECHANALYSISREQUEST.fields_by_name['to']._options = None
   _GETTECHANALYSISREQUEST.fields_by_name['to']._serialized_options = b'\342A\001\002'
   _GETTECHANALYSISREQUEST.fields_by_name['interval']._options = None
   _GETTECHANALYSISREQUEST.fields_by_name['interval']._serialized_options = b'\342A\001\002'
   _GETTECHANALYSISREQUEST.fields_by_name['type_of_price']._options = None
   _GETTECHANALYSISREQUEST.fields_by_name['type_of_price']._serialized_options = b'\342A\001\002'
-  _globals['_SUBSCRIPTIONACTION']._serialized_start=13058
-  _globals['_SUBSCRIPTIONACTION']._serialized_end=13187
-  _globals['_SUBSCRIPTIONINTERVAL']._serialized_start=13190
-  _globals['_SUBSCRIPTIONINTERVAL']._serialized_end=13710
-  _globals['_SUBSCRIPTIONSTATUS']._serialized_start=13713
-  _globals['_SUBSCRIPTIONSTATUS']._serialized_end=14166
-  _globals['_TRADEDIRECTION']._serialized_start=14168
-  _globals['_TRADEDIRECTION']._serialized_end=14268
-  _globals['_CANDLEINTERVAL']._serialized_start=14271
-  _globals['_CANDLEINTERVAL']._serialized_end=14672
-  _globals['_CANDLESOURCE']._serialized_start=14674
-  _globals['_CANDLESOURCE']._serialized_end=14781
-  _globals['_ORDERBOOKTYPE']._serialized_start=14783
-  _globals['_ORDERBOOKTYPE']._serialized_end=14886
+  _globals['_SUBSCRIPTIONACTION']._serialized_start=13287
+  _globals['_SUBSCRIPTIONACTION']._serialized_end=13416
+  _globals['_SUBSCRIPTIONINTERVAL']._serialized_start=13419
+  _globals['_SUBSCRIPTIONINTERVAL']._serialized_end=13939
+  _globals['_SUBSCRIPTIONSTATUS']._serialized_start=13942
+  _globals['_SUBSCRIPTIONSTATUS']._serialized_end=14395
+  _globals['_TRADESOURCETYPE']._serialized_start=14397
+  _globals['_TRADESOURCETYPE']._serialized_end=14518
+  _globals['_TRADEDIRECTION']._serialized_start=14520
+  _globals['_TRADEDIRECTION']._serialized_end=14620
+  _globals['_CANDLEINTERVAL']._serialized_start=14623
+  _globals['_CANDLEINTERVAL']._serialized_end=15024
+  _globals['_CANDLESOURCE']._serialized_start=15026
+  _globals['_CANDLESOURCE']._serialized_end=15133
+  _globals['_ORDERBOOKTYPE']._serialized_start=15135
+  _globals['_ORDERBOOKTYPE']._serialized_end=15238
   _globals['_MARKETDATAREQUEST']._serialized_start=200
   _globals['_MARKETDATAREQUEST']._serialized_end=828
   _globals['_MARKETDATASERVERSIDESTREAMREQUEST']._serialized_start=831
   _globals['_MARKETDATASERVERSIDESTREAMREQUEST']._serialized_end=1363
   _globals['_MARKETDATARESPONSE']._serialized_start=1366
   _globals['_MARKETDATARESPONSE']._serialized_end=2326
   _globals['_SUBSCRIBECANDLESREQUEST']._serialized_start=2329
@@ -110,101 +112,101 @@
   _globals['_ORDERBOOKINSTRUMENT']._serialized_start=3321
   _globals['_ORDERBOOKINSTRUMENT']._serialized_end=3477
   _globals['_SUBSCRIBEORDERBOOKRESPONSE']._serialized_start=3480
   _globals['_SUBSCRIBEORDERBOOKRESPONSE']._serialized_end=3625
   _globals['_ORDERBOOKSUBSCRIPTION']._serialized_start=3628
   _globals['_ORDERBOOKSUBSCRIPTION']._serialized_end=3915
   _globals['_SUBSCRIBETRADESREQUEST']._serialized_start=3918
-  _globals['_SUBSCRIBETRADESREQUEST']._serialized_end=4107
-  _globals['_TRADEINSTRUMENT']._serialized_start=4109
-  _globals['_TRADEINSTRUMENT']._serialized_end=4167
-  _globals['_SUBSCRIBETRADESRESPONSE']._serialized_start=4170
-  _globals['_SUBSCRIBETRADESRESPONSE']._serialized_end=4303
-  _globals['_TRADESUBSCRIPTION']._serialized_start=4306
-  _globals['_TRADESUBSCRIPTION']._serialized_end=4495
-  _globals['_SUBSCRIBEINFOREQUEST']._serialized_start=4498
-  _globals['_SUBSCRIBEINFOREQUEST']._serialized_end=4684
-  _globals['_INFOINSTRUMENT']._serialized_start=4686
-  _globals['_INFOINSTRUMENT']._serialized_end=4743
-  _globals['_SUBSCRIBEINFORESPONSE']._serialized_start=4746
-  _globals['_SUBSCRIBEINFORESPONSE']._serialized_end=4875
-  _globals['_INFOSUBSCRIPTION']._serialized_start=4878
-  _globals['_INFOSUBSCRIPTION']._serialized_end=5066
-  _globals['_SUBSCRIBELASTPRICEREQUEST']._serialized_start=5069
-  _globals['_SUBSCRIBELASTPRICEREQUEST']._serialized_end=5265
-  _globals['_LASTPRICEINSTRUMENT']._serialized_start=5267
-  _globals['_LASTPRICEINSTRUMENT']._serialized_end=5329
-  _globals['_SUBSCRIBELASTPRICERESPONSE']._serialized_start=5332
-  _globals['_SUBSCRIBELASTPRICERESPONSE']._serialized_end=5477
-  _globals['_LASTPRICESUBSCRIPTION']._serialized_start=5480
-  _globals['_LASTPRICESUBSCRIPTION']._serialized_end=5673
-  _globals['_CANDLE']._serialized_start=5676
-  _globals['_CANDLE']._serialized_end=6166
-  _globals['_ORDERBOOK']._serialized_start=6169
-  _globals['_ORDERBOOK']._serialized_end=6635
-  _globals['_ORDER']._serialized_start=6637
-  _globals['_ORDER']._serialized_end=6727
-  _globals['_TRADE']._serialized_start=6730
-  _globals['_TRADE']._serialized_end=6974
-  _globals['_TRADINGSTATUS']._serialized_start=6977
-  _globals['_TRADINGSTATUS']._serialized_end=7231
-  _globals['_GETCANDLESREQUEST']._serialized_start=7234
-  _globals['_GETCANDLESREQUEST']._serialized_end=7706
-  _globals['_GETCANDLESREQUEST_CANDLESOURCE']._serialized_start=7583
-  _globals['_GETCANDLESREQUEST_CANDLESOURCE']._serialized_end=7656
-  _globals['_GETCANDLESRESPONSE']._serialized_start=7708
-  _globals['_GETCANDLESRESPONSE']._serialized_end=7800
-  _globals['_HISTORICCANDLE']._serialized_start=7803
-  _globals['_HISTORICCANDLE']._serialized_end=8230
-  _globals['_GETLASTPRICESREQUEST']._serialized_start=8232
-  _globals['_GETLASTPRICESREQUEST']._serialized_end=8295
-  _globals['_GETLASTPRICESRESPONSE']._serialized_start=8297
-  _globals['_GETLASTPRICESRESPONSE']._serialized_end=8391
-  _globals['_LASTPRICE']._serialized_start=8394
-  _globals['_LASTPRICE']._serialized_end=8550
-  _globals['_GETORDERBOOKREQUEST']._serialized_start=8552
-  _globals['_GETORDERBOOKREQUEST']._serialized_end=8672
-  _globals['_GETORDERBOOKRESPONSE']._serialized_start=8675
-  _globals['_GETORDERBOOKRESPONSE']._serialized_end=9302
-  _globals['_GETTRADINGSTATUSREQUEST']._serialized_start=9304
-  _globals['_GETTRADINGSTATUSREQUEST']._serialized_end=9407
-  _globals['_GETTRADINGSTATUSESREQUEST']._serialized_start=9409
-  _globals['_GETTRADINGSTATUSESREQUEST']._serialized_end=9459
-  _globals['_GETTRADINGSTATUSESRESPONSE']._serialized_start=9461
-  _globals['_GETTRADINGSTATUSESRESPONSE']._serialized_end=9580
-  _globals['_GETTRADINGSTATUSRESPONSE']._serialized_start=9583
-  _globals['_GETTRADINGSTATUSRESPONSE']._serialized_end=9905
-  _globals['_GETLASTTRADESREQUEST']._serialized_start=9908
-  _globals['_GETLASTTRADESREQUEST']._serialized_end=10102
-  _globals['_GETLASTTRADESRESPONSE']._serialized_start=10104
-  _globals['_GETLASTTRADESRESPONSE']._serialized_end=10189
-  _globals['_GETMYSUBSCRIPTIONS']._serialized_start=10191
-  _globals['_GETMYSUBSCRIPTIONS']._serialized_end=10211
-  _globals['_GETCLOSEPRICESREQUEST']._serialized_start=10213
-  _globals['_GETCLOSEPRICESREQUEST']._serialized_end=10331
-  _globals['_INSTRUMENTCLOSEPRICEREQUEST']._serialized_start=10333
-  _globals['_INSTRUMENTCLOSEPRICEREQUEST']._serialized_end=10385
-  _globals['_GETCLOSEPRICESRESPONSE']._serialized_start=10387
-  _globals['_GETCLOSEPRICESRESPONSE']._serialized_end=10502
-  _globals['_INSTRUMENTCLOSEPRICERESPONSE']._serialized_start=10505
-  _globals['_INSTRUMENTCLOSEPRICERESPONSE']._serialized_end=10761
-  _globals['_GETTECHANALYSISREQUEST']._serialized_start=10764
-  _globals['_GETTECHANALYSISREQUEST']._serialized_end=12416
-  _globals['_GETTECHANALYSISREQUEST_SMOOTHING']._serialized_start=11430
-  _globals['_GETTECHANALYSISREQUEST_SMOOTHING']._serialized_end=11509
-  _globals['_GETTECHANALYSISREQUEST_DEVIATION']._serialized_start=11511
-  _globals['_GETTECHANALYSISREQUEST_DEVIATION']._serialized_end=11602
-  _globals['_GETTECHANALYSISREQUEST_INDICATORINTERVAL']._serialized_start=11605
-  _globals['_GETTECHANALYSISREQUEST_INDICATORINTERVAL']._serialized_end=12080
-  _globals['_GETTECHANALYSISREQUEST_TYPEOFPRICE']._serialized_start=12083
-  _globals['_GETTECHANALYSISREQUEST_TYPEOFPRICE']._serialized_end=12246
-  _globals['_GETTECHANALYSISREQUEST_INDICATORTYPE']._serialized_start=12249
-  _globals['_GETTECHANALYSISREQUEST_INDICATORTYPE']._serialized_end=12416
-  _globals['_GETTECHANALYSISRESPONSE']._serialized_start=12419
-  _globals['_GETTECHANALYSISRESPONSE']._serialized_end=13055
-  _globals['_GETTECHANALYSISRESPONSE_TECHANALYSISITEM']._serialized_start=12558
-  _globals['_GETTECHANALYSISRESPONSE_TECHANALYSISITEM']._serialized_end=13055
-  _globals['_MARKETDATASERVICE']._serialized_start=14889
-  _globals['_MARKETDATASERVICE']._serialized_end=16057
-  _globals['_MARKETDATASTREAMSERVICE']._serialized_start=16060
-  _globals['_MARKETDATASTREAMSERVICE']._serialized_end=16393
+  _globals['_SUBSCRIBETRADESREQUEST']._serialized_end=4183
+  _globals['_TRADEINSTRUMENT']._serialized_start=4185
+  _globals['_TRADEINSTRUMENT']._serialized_end=4243
+  _globals['_SUBSCRIBETRADESRESPONSE']._serialized_start=4246
+  _globals['_SUBSCRIBETRADESRESPONSE']._serialized_end=4455
+  _globals['_TRADESUBSCRIPTION']._serialized_start=4458
+  _globals['_TRADESUBSCRIPTION']._serialized_end=4647
+  _globals['_SUBSCRIBEINFOREQUEST']._serialized_start=4650
+  _globals['_SUBSCRIBEINFOREQUEST']._serialized_end=4836
+  _globals['_INFOINSTRUMENT']._serialized_start=4838
+  _globals['_INFOINSTRUMENT']._serialized_end=4895
+  _globals['_SUBSCRIBEINFORESPONSE']._serialized_start=4898
+  _globals['_SUBSCRIBEINFORESPONSE']._serialized_end=5027
+  _globals['_INFOSUBSCRIPTION']._serialized_start=5030
+  _globals['_INFOSUBSCRIPTION']._serialized_end=5218
+  _globals['_SUBSCRIBELASTPRICEREQUEST']._serialized_start=5221
+  _globals['_SUBSCRIBELASTPRICEREQUEST']._serialized_end=5417
+  _globals['_LASTPRICEINSTRUMENT']._serialized_start=5419
+  _globals['_LASTPRICEINSTRUMENT']._serialized_end=5481
+  _globals['_SUBSCRIBELASTPRICERESPONSE']._serialized_start=5484
+  _globals['_SUBSCRIBELASTPRICERESPONSE']._serialized_end=5629
+  _globals['_LASTPRICESUBSCRIPTION']._serialized_start=5632
+  _globals['_LASTPRICESUBSCRIPTION']._serialized_end=5825
+  _globals['_CANDLE']._serialized_start=5828
+  _globals['_CANDLE']._serialized_end=6318
+  _globals['_ORDERBOOK']._serialized_start=6321
+  _globals['_ORDERBOOK']._serialized_end=6787
+  _globals['_ORDER']._serialized_start=6789
+  _globals['_ORDER']._serialized_end=6879
+  _globals['_TRADE']._serialized_start=6882
+  _globals['_TRADE']._serialized_end=7203
+  _globals['_TRADINGSTATUS']._serialized_start=7206
+  _globals['_TRADINGSTATUS']._serialized_end=7460
+  _globals['_GETCANDLESREQUEST']._serialized_start=7463
+  _globals['_GETCANDLESREQUEST']._serialized_end=7935
+  _globals['_GETCANDLESREQUEST_CANDLESOURCE']._serialized_start=7812
+  _globals['_GETCANDLESREQUEST_CANDLESOURCE']._serialized_end=7885
+  _globals['_GETCANDLESRESPONSE']._serialized_start=7937
+  _globals['_GETCANDLESRESPONSE']._serialized_end=8029
+  _globals['_HISTORICCANDLE']._serialized_start=8032
+  _globals['_HISTORICCANDLE']._serialized_end=8459
+  _globals['_GETLASTPRICESREQUEST']._serialized_start=8461
+  _globals['_GETLASTPRICESREQUEST']._serialized_end=8524
+  _globals['_GETLASTPRICESRESPONSE']._serialized_start=8526
+  _globals['_GETLASTPRICESRESPONSE']._serialized_end=8620
+  _globals['_LASTPRICE']._serialized_start=8623
+  _globals['_LASTPRICE']._serialized_end=8779
+  _globals['_GETORDERBOOKREQUEST']._serialized_start=8781
+  _globals['_GETORDERBOOKREQUEST']._serialized_end=8901
+  _globals['_GETORDERBOOKRESPONSE']._serialized_start=8904
+  _globals['_GETORDERBOOKRESPONSE']._serialized_end=9531
+  _globals['_GETTRADINGSTATUSREQUEST']._serialized_start=9533
+  _globals['_GETTRADINGSTATUSREQUEST']._serialized_end=9636
+  _globals['_GETTRADINGSTATUSESREQUEST']._serialized_start=9638
+  _globals['_GETTRADINGSTATUSESREQUEST']._serialized_end=9688
+  _globals['_GETTRADINGSTATUSESRESPONSE']._serialized_start=9690
+  _globals['_GETTRADINGSTATUSESRESPONSE']._serialized_end=9809
+  _globals['_GETTRADINGSTATUSRESPONSE']._serialized_start=9812
+  _globals['_GETTRADINGSTATUSRESPONSE']._serialized_end=10134
+  _globals['_GETLASTTRADESREQUEST']._serialized_start=10137
+  _globals['_GETLASTTRADESREQUEST']._serialized_end=10331
+  _globals['_GETLASTTRADESRESPONSE']._serialized_start=10333
+  _globals['_GETLASTTRADESRESPONSE']._serialized_end=10418
+  _globals['_GETMYSUBSCRIPTIONS']._serialized_start=10420
+  _globals['_GETMYSUBSCRIPTIONS']._serialized_end=10440
+  _globals['_GETCLOSEPRICESREQUEST']._serialized_start=10442
+  _globals['_GETCLOSEPRICESREQUEST']._serialized_end=10560
+  _globals['_INSTRUMENTCLOSEPRICEREQUEST']._serialized_start=10562
+  _globals['_INSTRUMENTCLOSEPRICEREQUEST']._serialized_end=10614
+  _globals['_GETCLOSEPRICESRESPONSE']._serialized_start=10616
+  _globals['_GETCLOSEPRICESRESPONSE']._serialized_end=10731
+  _globals['_INSTRUMENTCLOSEPRICERESPONSE']._serialized_start=10734
+  _globals['_INSTRUMENTCLOSEPRICERESPONSE']._serialized_end=10990
+  _globals['_GETTECHANALYSISREQUEST']._serialized_start=10993
+  _globals['_GETTECHANALYSISREQUEST']._serialized_end=12645
+  _globals['_GETTECHANALYSISREQUEST_SMOOTHING']._serialized_start=11659
+  _globals['_GETTECHANALYSISREQUEST_SMOOTHING']._serialized_end=11738
+  _globals['_GETTECHANALYSISREQUEST_DEVIATION']._serialized_start=11740
+  _globals['_GETTECHANALYSISREQUEST_DEVIATION']._serialized_end=11831
+  _globals['_GETTECHANALYSISREQUEST_INDICATORINTERVAL']._serialized_start=11834
+  _globals['_GETTECHANALYSISREQUEST_INDICATORINTERVAL']._serialized_end=12309
+  _globals['_GETTECHANALYSISREQUEST_TYPEOFPRICE']._serialized_start=12312
+  _globals['_GETTECHANALYSISREQUEST_TYPEOFPRICE']._serialized_end=12475
+  _globals['_GETTECHANALYSISREQUEST_INDICATORTYPE']._serialized_start=12478
+  _globals['_GETTECHANALYSISREQUEST_INDICATORTYPE']._serialized_end=12645
+  _globals['_GETTECHANALYSISRESPONSE']._serialized_start=12648
+  _globals['_GETTECHANALYSISRESPONSE']._serialized_end=13284
+  _globals['_GETTECHANALYSISRESPONSE_TECHANALYSISITEM']._serialized_start=12787
+  _globals['_GETTECHANALYSISRESPONSE_TECHANALYSISITEM']._serialized_end=13284
+  _globals['_MARKETDATASERVICE']._serialized_start=15241
+  _globals['_MARKETDATASERVICE']._serialized_end=16409
+  _globals['_MARKETDATASTREAMSERVICE']._serialized_start=16412
+  _globals['_MARKETDATASTREAMSERVICE']._serialized_end=16745
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/marketdata_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,42 @@
 """Внутренняя ошибка сервиса."""
 SUBSCRIPTION_STATUS_TOO_MANY_REQUESTS: SubscriptionStatus.ValueType  # 8
 """Превышен лимит на количество запросов на подписки в течение установленного отрезка времени"""
 SUBSCRIPTION_STATUS_SUBSCRIPTION_NOT_FOUND: SubscriptionStatus.ValueType  # 9
 """Активная подписка не найдена. Ошибка может возникнуть только при отписке от не существующей отписки"""
 global___SubscriptionStatus = SubscriptionStatus
 
+class _TradeSourceType:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _TradeSourceTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_TradeSourceType.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    TRADE_SOURCE_UNSPECIFIED: _TradeSourceType.ValueType  # 0
+    """Тип сделки не определён."""
+    TRADE_SOURCE_EXCHANGE: _TradeSourceType.ValueType  # 1
+    """биржевые сделки"""
+    TRADE_SOURCE_DEALER: _TradeSourceType.ValueType  # 2
+    """сделки дилера"""
+    TRADE_SOURCE_ALL: _TradeSourceType.ValueType  # 3
+    """все сделки"""
+
+class TradeSourceType(_TradeSourceType, metaclass=_TradeSourceTypeEnumTypeWrapper):
+    """Источники сделок"""
+
+TRADE_SOURCE_UNSPECIFIED: TradeSourceType.ValueType  # 0
+"""Тип сделки не определён."""
+TRADE_SOURCE_EXCHANGE: TradeSourceType.ValueType  # 1
+"""биржевые сделки"""
+TRADE_SOURCE_DEALER: TradeSourceType.ValueType  # 2
+"""сделки дилера"""
+TRADE_SOURCE_ALL: TradeSourceType.ValueType  # 3
+"""все сделки"""
+global___TradeSourceType = TradeSourceType
+
 class _TradeDirection:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _TradeDirectionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_TradeDirection.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     TRADE_DIRECTION_UNSPECIFIED: _TradeDirection.ValueType  # 0
@@ -697,26 +725,30 @@
 class SubscribeTradesRequest(google.protobuf.message.Message):
     """Изменение статуса подписки на поток обезличенных сделок."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBSCRIPTION_ACTION_FIELD_NUMBER: builtins.int
     INSTRUMENTS_FIELD_NUMBER: builtins.int
+    TRADE_TYPE_FIELD_NUMBER: builtins.int
     subscription_action: global___SubscriptionAction.ValueType
     """Изменение статуса подписки."""
     @property
     def instruments(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TradeInstrument]:
         """Массив инструментов для подписки на поток обезличенных сделок."""
+    trade_type: global___TradeSourceType.ValueType
+    """Источник сделок"""
     def __init__(
         self,
         *,
         subscription_action: global___SubscriptionAction.ValueType = ...,
         instruments: collections.abc.Iterable[global___TradeInstrument] | None = ...,
+        trade_type: global___TradeSourceType.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instruments", b"instruments", "subscription_action", b"subscription_action"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instruments", b"instruments", "subscription_action", b"subscription_action", "trade_type", b"trade_type"]) -> None: ...
 
 global___SubscribeTradesRequest = SubscribeTradesRequest
 
 @typing_extensions.final
 class TradeInstrument(google.protobuf.message.Message):
     """Запрос подписки на поток обезличенных сделок."""
 
@@ -742,26 +774,30 @@
 class SubscribeTradesResponse(google.protobuf.message.Message):
     """Результат изменения статуса подписки на поток обезличенных сделок."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRACKING_ID_FIELD_NUMBER: builtins.int
     TRADE_SUBSCRIPTIONS_FIELD_NUMBER: builtins.int
+    TRADE_TYPE_FIELD_NUMBER: builtins.int
     tracking_id: builtins.str
     """Уникальный идентификатор запроса, подробнее: [tracking_id](https://russianinvestments.github.io/investAPI/grpc#tracking-id)."""
     @property
     def trade_subscriptions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TradeSubscription]:
         """Массив статусов подписки на поток сделок."""
+    trade_type: global___TradeSourceType.ValueType
+    """Источник сделок"""
     def __init__(
         self,
         *,
         tracking_id: builtins.str = ...,
         trade_subscriptions: collections.abc.Iterable[global___TradeSubscription] | None = ...,
+        trade_type: global___TradeSourceType.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tracking_id", b"tracking_id", "trade_subscriptions", b"trade_subscriptions"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["tracking_id", b"tracking_id", "trade_subscriptions", b"trade_subscriptions", "trade_type", b"trade_type"]) -> None: ...
 
 global___SubscribeTradesResponse = SubscribeTradesResponse
 
 @typing_extensions.final
 class TradeSubscription(google.protobuf.message.Message):
     """Статус подписки."""
 
@@ -1152,40 +1188,44 @@
 
     FIGI_FIELD_NUMBER: builtins.int
     DIRECTION_FIELD_NUMBER: builtins.int
     PRICE_FIELD_NUMBER: builtins.int
     QUANTITY_FIELD_NUMBER: builtins.int
     TIME_FIELD_NUMBER: builtins.int
     INSTRUMENT_UID_FIELD_NUMBER: builtins.int
+    TRADESOURCE_FIELD_NUMBER: builtins.int
     figi: builtins.str
     """Figi-идентификатор инструмента."""
     direction: global___TradeDirection.ValueType
     """Направление сделки."""
     @property
     def price(self) -> tinkoff.invest.grpc.common_pb2.Quotation:
         """Цена за 1 инструмент. Для получения стоимости лота требуется умножить на лотность инструмента. Для перевод цен в валюту рекомендуем использовать [информацию со страницы](https://russianinvestments.github.io/investAPI/faq_marketdata/)"""
     quantity: builtins.int
     """Количество лотов."""
     @property
     def time(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Время сделки в часовом поясе UTC по времени биржи."""
     instrument_uid: builtins.str
     """Uid инструмента"""
+    tradeSource: global___TradeSourceType.ValueType
+    """Источник сделки"""
     def __init__(
         self,
         *,
         figi: builtins.str = ...,
         direction: global___TradeDirection.ValueType = ...,
         price: tinkoff.invest.grpc.common_pb2.Quotation | None = ...,
         quantity: builtins.int = ...,
         time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         instrument_uid: builtins.str = ...,
+        tradeSource: global___TradeSourceType.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["price", b"price", "time", b"time"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["direction", b"direction", "figi", b"figi", "instrument_uid", b"instrument_uid", "price", b"price", "quantity", b"quantity", "time", b"time"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["direction", b"direction", "figi", b"figi", "instrument_uid", b"instrument_uid", "price", b"price", "quantity", b"quantity", "time", b"time", "tradeSource", b"tradeSource"]) -> None: ...
 
 global___Trade = Trade
 
 @typing_extensions.final
 class TradingStatus(google.protobuf.message.Message):
     """Пакет изменения торгового статуса."""
 
@@ -1696,15 +1736,15 @@
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["trades", b"trades"]) -> None: ...
 
 global___GetLastTradesResponse = GetLastTradesResponse
 
 @typing_extensions.final
 class GetMySubscriptions(google.protobuf.message.Message):
-    """Запрос активных подписок."""
+    """Запрос активных подписок. Запрос вернет по одному сообщению на каждый тип активных подписок (SubscribeLastPriceResponse, SubscribeInfoResponse, SubscribeTradesResponse, SubscribeOrderBookResponse, SubscribeCandlesResponse)"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/marketdata_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/marketdata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/operations_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/operations_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/operations_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/orders_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from tinkoff.invest.grpc import (
     common_pb2 as tinkoff_dot_invest_dot_grpc_dot_common__pb2,
 )
 from tinkoff.invest.grpc.google.api import (
     field_behavior_pb2 as tinkoff_dot_invest_dot_grpc_dot_google_dot_api_dot_field__behavior__pb2,
 )
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tinkoff/invest/grpc/orders.proto\x12%tinkoff.public.invest.api.contract.v1\x1a tinkoff/invest/grpc/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"\'\n\x13TradesStreamRequest\x12\x10\n\x08\x61\x63\x63ounts\x18\x01 \x03(\t\"\xaa\x01\n\x14TradesStreamResponse\x12J\n\x0corder_trades\x18\x01 \x01(\x0b\x32\x32.tinkoff.public.invest.api.contract.v1.OrderTradesH\x00\x12;\n\x04ping\x18\x02 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PingH\x00\x42\t\n\x07payload\"\x96\x02\n\x0bOrderTrades\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12H\n\tdirection\x18\x03 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12\x0c\n\x04\x66igi\x18\x04 \x01(\t\x12\x41\n\x06trades\x18\x05 \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderTrade\x12\x12\n\naccount_id\x18\x06 \x01(\t\x12\x16\n\x0einstrument_uid\x18\x07 \x01(\t\"\xa0\x01\n\nOrderTrade\x12-\n\tdate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05price\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x10\n\x08quantity\x18\x03 \x01(\x03\x12\x10\n\x08trade_id\x18\x04 \x01(\t\"\x94\x04\n\x10PostOrderRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x16\n\x08quantity\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x01\x88\x01\x01\x12N\n\tdirection\x18\x04 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirectionB\x04\xe2\x41\x01\x02\x12\x18\n\naccount_id\x18\x05 \x01(\tB\x04\xe2\x41\x01\x02\x12J\n\norder_type\x18\x06 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderTypeB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x07 \x01(\tB\x04\xe2\x41\x01\x02\x12\x15\n\rinstrument_id\x18\x08 \x01(\t\x12M\n\rtime_in_force\x18\t \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.TimeInForceType\x12\x44\n\nprice_type\x18\n \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceTypeB\x07\n\x05_figiB\x08\n\x06_price\"\xe8\x08\n\x11PostOrderResponse\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x62\n\x17\x65xecution_report_status\x18\x02 \x01(\x0e\x32\x41.tinkoff.public.invest.api.contract.v1.OrderExecutionReportStatus\x12\x16\n\x0elots_requested\x18\x03 \x01(\x03\x12\x15\n\rlots_executed\x18\x04 \x01(\x03\x12N\n\x13initial_order_price\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12O\n\x14\x65xecuted_order_price\x18\x06 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12total_order_amount\x18\x07 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12initial_commission\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12N\n\x13\x65xecuted_commission\x18\t \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x44\n\taci_value\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x0c\n\x04\x66igi\x18\x0b \x01(\t\x12H\n\tdirection\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12Q\n\x16initial_security_price\x18\r \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x44\n\norder_type\x18\x0e \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderType\x12\x0f\n\x07message\x18\x0f \x01(\t\x12P\n\x16initial_order_price_pt\x18\x10 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x16\n\x0einstrument_uid\x18\x11 \x01(\t\x12\x18\n\x10order_request_id\x18\x14 \x01(\t\x12S\n\x11response_metadata\x18\xfe\x01 \x01(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.ResponseMetadata\"F\n\x12\x43\x61ncelOrderRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\"\x94\x01\n\x13\x43\x61ncelOrderResponse\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12S\n\x11response_metadata\x18\xfe\x01 \x01(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.ResponseMetadata\"\x8e\x01\n\x14GetOrderStateRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x12\x44\n\nprice_type\x18\x03 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceType\",\n\x10GetOrdersRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"V\n\x11GetOrdersResponse\x12\x41\n\x06orders\x18\x01 \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderState\"\x8a\t\n\nOrderState\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x62\n\x17\x65xecution_report_status\x18\x02 \x01(\x0e\x32\x41.tinkoff.public.invest.api.contract.v1.OrderExecutionReportStatus\x12\x16\n\x0elots_requested\x18\x03 \x01(\x03\x12\x15\n\rlots_executed\x18\x04 \x01(\x03\x12N\n\x13initial_order_price\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12O\n\x14\x65xecuted_order_price\x18\x06 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12total_order_amount\x18\x07 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x16\x61verage_position_price\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12initial_commission\x18\t \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12N\n\x13\x65xecuted_commission\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x0c\n\x04\x66igi\x18\x0b \x01(\t\x12H\n\tdirection\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12Q\n\x16initial_security_price\x18\r \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x41\n\x06stages\x18\x0e \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderStage\x12M\n\x12service_commission\x18\x0f \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x10\n\x08\x63urrency\x18\x10 \x01(\t\x12\x44\n\norder_type\x18\x11 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderType\x12.\n\norder_date\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\x13 \x01(\t\x12\x18\n\x10order_request_id\x18\x14 \x01(\t\"\xa6\x01\n\nOrderStage\x12@\n\x05price\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x10\n\x08quantity\x18\x02 \x01(\x03\x12\x10\n\x08trade_id\x18\x03 \x01(\t\x12\x32\n\x0e\x65xecution_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa8\x02\n\x13ReplaceOrderRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02\x12\x1d\n\x0fidempotency_key\x18\x07 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08quantity\x18\x0b \x01(\x03\x42\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x00\x88\x01\x01\x12I\n\nprice_type\x18\r \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceTypeH\x01\x88\x01\x01\x42\x08\n\x06_priceB\r\n\x0b_price_type\"\x9a\x01\n\x11GetMaxLotsRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x1b\n\rinstrument_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x00\x88\x01\x01\x42\x08\n\x06_price\"\xe6\x04\n\x12GetMaxLotsResponse\x12\x10\n\x08\x63urrency\x18\x01 \x01(\t\x12[\n\nbuy_limits\x18\x02 \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.BuyLimitsView\x12\x62\n\x11\x62uy_margin_limits\x18\x03 \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.BuyLimitsView\x12]\n\x0bsell_limits\x18\x04 \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.SellLimitsView\x12\x64\n\x12sell_margin_limits\x18\x05 \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.SellLimitsView\x1a\x8e\x01\n\rBuyLimitsView\x12J\n\x10\x62uy_money_amount\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x14\n\x0c\x62uy_max_lots\x18\x02 \x01(\x03\x12\x1b\n\x13\x62uy_max_market_lots\x18\x03 \x01(\x03\x1a\'\n\x0eSellLimitsView\x12\x15\n\rsell_max_lots\x18\x01 \x01(\x03\"\xde\x01\n\x14GetOrderPriceRequest\x12\x12\n\naccount_id\x18\x01 \x01(\t\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\x12?\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12H\n\tdirection\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12\x10\n\x08quantity\x18\r \x01(\x03\"\xe3\x07\n\x15GetOrderPriceResponse\x12M\n\x12total_order_amount\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12O\n\x14initial_order_amount\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x16\n\x0elots_requested\x18\x03 \x01(\x03\x12N\n\x13\x65xecuted_commission\x18\x07 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12R\n\x17\x65xecuted_commission_rub\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12service_commission\x18\t \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12J\n\x0f\x64\x65\x61l_commission\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\\\n\nextra_bond\x18\x0c \x01(\x0b\x32\x46.tinkoff.public.invest.api.contract.v1.GetOrderPriceResponse.ExtraBondH\x00\x12`\n\x0c\x65xtra_future\x18\r \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetOrderPriceResponse.ExtraFutureH\x00\x1a\xa4\x01\n\tExtraBond\x12\x44\n\taci_value\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x17nominal_conversion_rate\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x1aX\n\x0b\x45xtraFuture\x12I\n\x0einitial_margin\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValueB\x12\n\x10instrument_extra*d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_BUY\x10\x01\x12\x18\n\x14ORDER_DIRECTION_SELL\x10\x02*n\n\tOrderType\x12\x1a\n\x16ORDER_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10ORDER_TYPE_LIMIT\x10\x01\x12\x15\n\x11ORDER_TYPE_MARKET\x10\x02\x12\x18\n\x14ORDER_TYPE_BESTPRICE\x10\x03*\x80\x02\n\x1aOrderExecutionReportStatus\x12\'\n#EXECUTION_REPORT_STATUS_UNSPECIFIED\x10\x00\x12 \n\x1c\x45XECUTION_REPORT_STATUS_FILL\x10\x01\x12$\n EXECUTION_REPORT_STATUS_REJECTED\x10\x02\x12%\n!EXECUTION_REPORT_STATUS_CANCELLED\x10\x03\x12\x1f\n\x1b\x45XECUTION_REPORT_STATUS_NEW\x10\x04\x12)\n%EXECUTION_REPORT_STATUS_PARTIALLYFILL\x10\x05*\x88\x01\n\x0fTimeInForceType\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_DAY\x10\x01\x12\x1f\n\x1bTIME_IN_FORCE_FILL_AND_KILL\x10\x02\x12\x1e\n\x1aTIME_IN_FORCE_FILL_OR_KILL\x10\x03\x32\xa1\x01\n\x13OrdersStreamService\x12\x89\x01\n\x0cTradesStream\x12:.tinkoff.public.invest.api.contract.v1.TradesStreamRequest\x1a;.tinkoff.public.invest.api.contract.v1.TradesStreamResponse0\x01\x32\xaf\x07\n\rOrdersService\x12~\n\tPostOrder\x12\x37.tinkoff.public.invest.api.contract.v1.PostOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x84\x01\n\x0b\x43\x61ncelOrder\x12\x39.tinkoff.public.invest.api.contract.v1.CancelOrderRequest\x1a:.tinkoff.public.invest.api.contract.v1.CancelOrderResponse\x12\x7f\n\rGetOrderState\x12;.tinkoff.public.invest.api.contract.v1.GetOrderStateRequest\x1a\x31.tinkoff.public.invest.api.contract.v1.OrderState\x12~\n\tGetOrders\x12\x37.tinkoff.public.invest.api.contract.v1.GetOrdersRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.GetOrdersResponse\x12\x84\x01\n\x0cReplaceOrder\x12:.tinkoff.public.invest.api.contract.v1.ReplaceOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x81\x01\n\nGetMaxLots\x12\x38.tinkoff.public.invest.api.contract.v1.GetMaxLotsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse\x12\x8a\x01\n\rGetOrderPrice\x12;.tinkoff.public.invest.api.contract.v1.GetOrderPriceRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetOrderPriceResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tinkoff/invest/grpc/orders.proto\x12%tinkoff.public.invest.api.contract.v1\x1a tinkoff/invest/grpc/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"\'\n\x13TradesStreamRequest\x12\x10\n\x08\x61\x63\x63ounts\x18\x01 \x03(\t\"\xaa\x01\n\x14TradesStreamResponse\x12J\n\x0corder_trades\x18\x01 \x01(\x0b\x32\x32.tinkoff.public.invest.api.contract.v1.OrderTradesH\x00\x12;\n\x04ping\x18\x02 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PingH\x00\x42\t\n\x07payload\"\x96\x02\n\x0bOrderTrades\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12H\n\tdirection\x18\x03 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12\x0c\n\x04\x66igi\x18\x04 \x01(\t\x12\x41\n\x06trades\x18\x05 \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderTrade\x12\x12\n\naccount_id\x18\x06 \x01(\t\x12\x16\n\x0einstrument_uid\x18\x07 \x01(\t\"\xa0\x01\n\nOrderTrade\x12-\n\tdate_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x05price\x18\x02 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x10\n\x08quantity\x18\x03 \x01(\x03\x12\x10\n\x08trade_id\x18\x04 \x01(\t\"\x94\x04\n\x10PostOrderRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x16\n\x08quantity\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x01\x88\x01\x01\x12N\n\tdirection\x18\x04 \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirectionB\x04\xe2\x41\x01\x02\x12\x18\n\naccount_id\x18\x05 \x01(\tB\x04\xe2\x41\x01\x02\x12J\n\norder_type\x18\x06 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderTypeB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x07 \x01(\tB\x04\xe2\x41\x01\x02\x12\x15\n\rinstrument_id\x18\x08 \x01(\t\x12M\n\rtime_in_force\x18\t \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.TimeInForceType\x12\x44\n\nprice_type\x18\n \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceTypeB\x07\n\x05_figiB\x08\n\x06_price\"\xe8\x08\n\x11PostOrderResponse\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x62\n\x17\x65xecution_report_status\x18\x02 \x01(\x0e\x32\x41.tinkoff.public.invest.api.contract.v1.OrderExecutionReportStatus\x12\x16\n\x0elots_requested\x18\x03 \x01(\x03\x12\x15\n\rlots_executed\x18\x04 \x01(\x03\x12N\n\x13initial_order_price\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12O\n\x14\x65xecuted_order_price\x18\x06 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12total_order_amount\x18\x07 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12initial_commission\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12N\n\x13\x65xecuted_commission\x18\t \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x44\n\taci_value\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x0c\n\x04\x66igi\x18\x0b \x01(\t\x12H\n\tdirection\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12Q\n\x16initial_security_price\x18\r \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x44\n\norder_type\x18\x0e \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderType\x12\x0f\n\x07message\x18\x0f \x01(\t\x12P\n\x16initial_order_price_pt\x18\x10 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x16\n\x0einstrument_uid\x18\x11 \x01(\t\x12\x18\n\x10order_request_id\x18\x14 \x01(\t\x12S\n\x11response_metadata\x18\xfe\x01 \x01(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.ResponseMetadata\"F\n\x12\x43\x61ncelOrderRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\"\x94\x01\n\x13\x43\x61ncelOrderResponse\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12S\n\x11response_metadata\x18\xfe\x01 \x01(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.ResponseMetadata\"\x8e\x01\n\x14GetOrderStateRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x12\x44\n\nprice_type\x18\x03 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceType\",\n\x10GetOrdersRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"V\n\x11GetOrdersResponse\x12\x41\n\x06orders\x18\x01 \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderState\"\x8a\t\n\nOrderState\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x62\n\x17\x65xecution_report_status\x18\x02 \x01(\x0e\x32\x41.tinkoff.public.invest.api.contract.v1.OrderExecutionReportStatus\x12\x16\n\x0elots_requested\x18\x03 \x01(\x03\x12\x15\n\rlots_executed\x18\x04 \x01(\x03\x12N\n\x13initial_order_price\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12O\n\x14\x65xecuted_order_price\x18\x06 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12total_order_amount\x18\x07 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x16\x61verage_position_price\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12initial_commission\x18\t \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12N\n\x13\x65xecuted_commission\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x0c\n\x04\x66igi\x18\x0b \x01(\t\x12H\n\tdirection\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12Q\n\x16initial_security_price\x18\r \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x41\n\x06stages\x18\x0e \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderStage\x12M\n\x12service_commission\x18\x0f \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x10\n\x08\x63urrency\x18\x10 \x01(\t\x12\x44\n\norder_type\x18\x11 \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderType\x12.\n\norder_date\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0einstrument_uid\x18\x13 \x01(\t\x12\x18\n\x10order_request_id\x18\x14 \x01(\t\"\xa6\x01\n\nOrderStage\x12@\n\x05price\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x10\n\x08quantity\x18\x02 \x01(\x03\x12\x10\n\x08trade_id\x18\x03 \x01(\t\x12\x32\n\x0e\x65xecution_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa8\x02\n\x13ReplaceOrderRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08order_id\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02\x12\x1d\n\x0fidempotency_key\x18\x07 \x01(\tB\x04\xe2\x41\x01\x02\x12\x16\n\x08quantity\x18\x0b \x01(\x03\x42\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x0c \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x00\x88\x01\x01\x12I\n\nprice_type\x18\r \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceTypeH\x01\x88\x01\x01\x42\x08\n\x06_priceB\r\n\x0b_price_type\"\x9a\x01\n\x11GetMaxLotsRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x1b\n\rinstrument_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x00\x88\x01\x01\x42\x08\n\x06_price\"\xe6\x04\n\x12GetMaxLotsResponse\x12\x10\n\x08\x63urrency\x18\x01 \x01(\t\x12[\n\nbuy_limits\x18\x02 \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.BuyLimitsView\x12\x62\n\x11\x62uy_margin_limits\x18\x03 \x01(\x0b\x32G.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.BuyLimitsView\x12]\n\x0bsell_limits\x18\x04 \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.SellLimitsView\x12\x64\n\x12sell_margin_limits\x18\x05 \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse.SellLimitsView\x1a\x8e\x01\n\rBuyLimitsView\x12J\n\x10\x62uy_money_amount\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12\x14\n\x0c\x62uy_max_lots\x18\x02 \x01(\x03\x12\x1b\n\x13\x62uy_max_market_lots\x18\x03 \x01(\x03\x1a\'\n\x0eSellLimitsView\x12\x15\n\rsell_max_lots\x18\x01 \x01(\x03\"\xde\x01\n\x14GetOrderPriceRequest\x12\x12\n\naccount_id\x18\x01 \x01(\t\x12\x15\n\rinstrument_id\x18\x02 \x01(\t\x12?\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12H\n\tdirection\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12\x10\n\x08quantity\x18\r \x01(\x03\"\xe3\x07\n\x15GetOrderPriceResponse\x12M\n\x12total_order_amount\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12O\n\x14initial_order_amount\x18\x05 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x16\n\x0elots_requested\x18\x03 \x01(\x03\x12N\n\x13\x65xecuted_commission\x18\x07 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12R\n\x17\x65xecuted_commission_rub\x18\x08 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12M\n\x12service_commission\x18\t \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12J\n\x0f\x64\x65\x61l_commission\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\\\n\nextra_bond\x18\x0c \x01(\x0b\x32\x46.tinkoff.public.invest.api.contract.v1.GetOrderPriceResponse.ExtraBondH\x00\x12`\n\x0c\x65xtra_future\x18\r \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.GetOrderPriceResponse.ExtraFutureH\x00\x1a\xa4\x01\n\tExtraBond\x12\x44\n\taci_value\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12Q\n\x17nominal_conversion_rate\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x1aX\n\x0b\x45xtraFuture\x12I\n\x0einitial_margin\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValueB\x12\n\x10instrument_extra\"a\n\x17OrderStateStreamRequest\x12\x10\n\x08\x61\x63\x63ounts\x18\x01 \x03(\t\x12\x1e\n\x11ping_delay_millis\x18\x0f \x01(\x05H\x00\x88\x01\x01\x42\x14\n\x12_ping_delay_millis\"\xc3\x14\n\x18OrderStateStreamResponse\x12\x61\n\x0border_state\x18\x01 \x01(\x0b\x32J.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse.OrderStateH\x00\x12;\n\x04ping\x18\x02 \x01(\x0b\x32+.tinkoff.public.invest.api.contract.v1.PingH\x00\x12l\n\x0csubscription\x18\x03 \x01(\x0b\x32T.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse.SubscriptionResponseH\x00\x1a\xed\x03\n\x14SubscriptionResponse\x12\x13\n\x0btracking_id\x18\x01 \x01(\t\x12w\n\x06status\x18\x02 \x01(\x0e\x32g.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse.SubscriptionResponse.SubscriptionStatus\x12\x11\n\tstream_id\x18\x04 \x01(\t\x12\x10\n\x08\x61\x63\x63ounts\x18\x05 \x03(\t\x12t\n\x05\x65rror\x18\x07 \x01(\x0b\x32`.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse.SubscriptionResponse.ErrorDetailH\x00\x88\x01\x01\x1a,\n\x0b\x45rrorDetail\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"t\n\x12SubscriptionStatus\x12#\n\x1fSUBSCRIPTION_STATUS_UNSPECIFIED\x10\x00\x12\x1a\n\x16SUBSCRIPTION_STATUS_OK\x10\x01\x12\x1d\n\x19SUBSCRIPTION_STATUS_ERROR\x10\rB\x08\n\x06_error\x1a\xd5\n\n\nOrderState\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x1d\n\x10order_request_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x0b\x63lient_code\x18\x03 \x01(\t\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x62\n\x17\x65xecution_report_status\x18\x05 \x01(\x0e\x32\x41.tinkoff.public.invest.api.contract.v1.OrderExecutionReportStatus\x12i\n\x0bstatus_info\x18\x06 \x01(\x0e\x32O.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse.StatusCauseInfoH\x01\x88\x01\x01\x12\x0e\n\x06ticker\x18\x07 \x01(\t\x12\x12\n\nclass_code\x18\x08 \x01(\t\x12\x10\n\x08lot_size\x18\t \x01(\x05\x12H\n\tdirection\x18\n \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.OrderDirection\x12M\n\rtime_in_force\x18\x0b \x01(\x0e\x32\x36.tinkoff.public.invest.api.contract.v1.TimeInForceType\x12\x44\n\norder_type\x18\x0c \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.OrderType\x12\x12\n\naccount_id\x18\r \x01(\t\x12N\n\x13initial_order_price\x18\x16 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x46\n\x0border_price\x18\x17 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x46\n\x06\x61mount\x18\x18 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValueH\x02\x88\x01\x01\x12O\n\x14\x65xecuted_order_price\x18\x19 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x10\n\x08\x63urrency\x18\x1a \x01(\t\x12\x16\n\x0elots_requested\x18\x1b \x01(\x03\x12\x15\n\rlots_executed\x18\x1c \x01(\x03\x12\x11\n\tlots_left\x18\x1d \x01(\x03\x12\x16\n\x0elots_cancelled\x18\x1e \x01(\x03\x12_\n\x06marker\x18\x1f \x01(\x0e\x32J.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse.MarkerTypeH\x03\x88\x01\x01\x12\x41\n\x06trades\x18! \x03(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.OrderTrade\x12\x33\n\x0f\x63ompletion_time\x18# \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x65xchange\x18$ \x01(\t\x12\x16\n\x0einstrument_uid\x18) \x01(\tB\x13\n\x11_order_request_idB\x0e\n\x0c_status_infoB\t\n\x07_amountB\t\n\x07_marker\"\xaf\x01\n\nMarkerType\x12\x12\n\x0eMARKER_UNKNOWN\x10\x00\x12\x11\n\rMARKER_BROKER\x10\x01\x12\x0f\n\x0bMARKER_CHAT\x10\x02\x12\x10\n\x0cMARKER_PAPER\x10\x03\x12\x11\n\rMARKER_MARGIN\x10\x04\x12\x10\n\x0cMARKER_TKBNM\x10\x05\x12\x10\n\x0cMARKER_SHORT\x10\x06\x12\x11\n\rMARKER_SPECMM\x10\x07\x12\r\n\tMARKER_PO\x10\x08\"\x93\x02\n\x0fStatusCauseInfo\x12\x15\n\x11\x43\x41USE_UNSPECIFIED\x10\x00\x12\x1d\n\x19\x43\x41USE_CANCELLED_BY_CLIENT\x10\x0f\x12\x1f\n\x1b\x43\x41USE_CANCELLED_BY_EXCHANGE\x10\x01\x12\'\n#CAUSE_CANCELLED_NOT_ENOUGH_POSITION\x10\x02\x12#\n\x1f\x43\x41USE_CANCELLED_BY_CLIENT_BLOCK\x10\x03\x12\x1c\n\x18\x43\x41USE_REJECTED_BY_BROKER\x10\x04\x12\x1e\n\x1a\x43\x41USE_REJECTED_BY_EXCHANGE\x10\x05\x12\x1d\n\x19\x43\x41USE_CANCELLED_BY_BROKER\x10\x06\x42\t\n\x07payload*d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_BUY\x10\x01\x12\x18\n\x14ORDER_DIRECTION_SELL\x10\x02*n\n\tOrderType\x12\x1a\n\x16ORDER_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10ORDER_TYPE_LIMIT\x10\x01\x12\x15\n\x11ORDER_TYPE_MARKET\x10\x02\x12\x18\n\x14ORDER_TYPE_BESTPRICE\x10\x03*\x80\x02\n\x1aOrderExecutionReportStatus\x12\'\n#EXECUTION_REPORT_STATUS_UNSPECIFIED\x10\x00\x12 \n\x1c\x45XECUTION_REPORT_STATUS_FILL\x10\x01\x12$\n EXECUTION_REPORT_STATUS_REJECTED\x10\x02\x12%\n!EXECUTION_REPORT_STATUS_CANCELLED\x10\x03\x12\x1f\n\x1b\x45XECUTION_REPORT_STATUS_NEW\x10\x04\x12)\n%EXECUTION_REPORT_STATUS_PARTIALLYFILL\x10\x05*\x88\x01\n\x0fTimeInForceType\x12\x1d\n\x19TIME_IN_FORCE_UNSPECIFIED\x10\x00\x12\x15\n\x11TIME_IN_FORCE_DAY\x10\x01\x12\x1f\n\x1bTIME_IN_FORCE_FILL_AND_KILL\x10\x02\x12\x1e\n\x1aTIME_IN_FORCE_FILL_OR_KILL\x10\x03\x32\xb9\x02\n\x13OrdersStreamService\x12\x89\x01\n\x0cTradesStream\x12:.tinkoff.public.invest.api.contract.v1.TradesStreamRequest\x1a;.tinkoff.public.invest.api.contract.v1.TradesStreamResponse0\x01\x12\x95\x01\n\x10OrderStateStream\x12>.tinkoff.public.invest.api.contract.v1.OrderStateStreamRequest\x1a?.tinkoff.public.invest.api.contract.v1.OrderStateStreamResponse0\x01\x32\xaf\x07\n\rOrdersService\x12~\n\tPostOrder\x12\x37.tinkoff.public.invest.api.contract.v1.PostOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x84\x01\n\x0b\x43\x61ncelOrder\x12\x39.tinkoff.public.invest.api.contract.v1.CancelOrderRequest\x1a:.tinkoff.public.invest.api.contract.v1.CancelOrderResponse\x12\x7f\n\rGetOrderState\x12;.tinkoff.public.invest.api.contract.v1.GetOrderStateRequest\x1a\x31.tinkoff.public.invest.api.contract.v1.OrderState\x12~\n\tGetOrders\x12\x37.tinkoff.public.invest.api.contract.v1.GetOrdersRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.GetOrdersResponse\x12\x84\x01\n\x0cReplaceOrder\x12:.tinkoff.public.invest.api.contract.v1.ReplaceOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x81\x01\n\nGetMaxLots\x12\x38.tinkoff.public.invest.api.contract.v1.GetMaxLotsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponse\x12\x8a\x01\n\rGetOrderPrice\x12;.tinkoff.public.invest.api.contract.v1.GetOrderPriceRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetOrderPriceResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tinkoff.invest.grpc.orders_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034ru.tinkoff.piapi.contract.v1P\001Z\014./;investapi\242\002\005TIAPI\252\002\024Tinkoff.InvestApi.V1\312\002\021Tinkoff\\Invest\\V1'
@@ -61,22 +61,22 @@
   _REPLACEORDERREQUEST.fields_by_name['idempotency_key']._serialized_options = b'\342A\001\002'
   _REPLACEORDERREQUEST.fields_by_name['quantity']._options = None
   _REPLACEORDERREQUEST.fields_by_name['quantity']._serialized_options = b'\342A\001\002'
   _GETMAXLOTSREQUEST.fields_by_name['account_id']._options = None
   _GETMAXLOTSREQUEST.fields_by_name['account_id']._serialized_options = b'\342A\001\002'
   _GETMAXLOTSREQUEST.fields_by_name['instrument_id']._options = None
   _GETMAXLOTSREQUEST.fields_by_name['instrument_id']._serialized_options = b'\342A\001\002'
-  _globals['_ORDERDIRECTION']._serialized_start=6651
-  _globals['_ORDERDIRECTION']._serialized_end=6751
-  _globals['_ORDERTYPE']._serialized_start=6753
-  _globals['_ORDERTYPE']._serialized_end=6863
-  _globals['_ORDEREXECUTIONREPORTSTATUS']._serialized_start=6866
-  _globals['_ORDEREXECUTIONREPORTSTATUS']._serialized_end=7122
-  _globals['_TIMEINFORCETYPE']._serialized_start=7125
-  _globals['_TIMEINFORCETYPE']._serialized_end=7261
+  _globals['_ORDERDIRECTION']._serialized_start=9380
+  _globals['_ORDERDIRECTION']._serialized_end=9480
+  _globals['_ORDERTYPE']._serialized_start=9482
+  _globals['_ORDERTYPE']._serialized_end=9592
+  _globals['_ORDEREXECUTIONREPORTSTATUS']._serialized_start=9595
+  _globals['_ORDEREXECUTIONREPORTSTATUS']._serialized_end=9851
+  _globals['_TIMEINFORCETYPE']._serialized_start=9854
+  _globals['_TIMEINFORCETYPE']._serialized_end=9990
   _globals['_TRADESSTREAMREQUEST']._serialized_start=195
   _globals['_TRADESSTREAMREQUEST']._serialized_end=234
   _globals['_TRADESSTREAMRESPONSE']._serialized_start=237
   _globals['_TRADESSTREAMRESPONSE']._serialized_end=407
   _globals['_ORDERTRADES']._serialized_start=410
   _globals['_ORDERTRADES']._serialized_end=688
   _globals['_ORDERTRADE']._serialized_start=691
@@ -113,12 +113,28 @@
   _globals['_GETORDERPRICEREQUEST']._serialized_end=5651
   _globals['_GETORDERPRICERESPONSE']._serialized_start=5654
   _globals['_GETORDERPRICERESPONSE']._serialized_end=6649
   _globals['_GETORDERPRICERESPONSE_EXTRABOND']._serialized_start=6375
   _globals['_GETORDERPRICERESPONSE_EXTRABOND']._serialized_end=6539
   _globals['_GETORDERPRICERESPONSE_EXTRAFUTURE']._serialized_start=6541
   _globals['_GETORDERPRICERESPONSE_EXTRAFUTURE']._serialized_end=6629
-  _globals['_ORDERSSTREAMSERVICE']._serialized_start=7264
-  _globals['_ORDERSSTREAMSERVICE']._serialized_end=7425
-  _globals['_ORDERSSERVICE']._serialized_start=7428
-  _globals['_ORDERSSERVICE']._serialized_end=8371
+  _globals['_ORDERSTATESTREAMREQUEST']._serialized_start=6651
+  _globals['_ORDERSTATESTREAMREQUEST']._serialized_end=6748
+  _globals['_ORDERSTATESTREAMRESPONSE']._serialized_start=6751
+  _globals['_ORDERSTATESTREAMRESPONSE']._serialized_end=9378
+  _globals['_ORDERSTATESTREAMRESPONSE_SUBSCRIPTIONRESPONSE']._serialized_start=7050
+  _globals['_ORDERSTATESTREAMRESPONSE_SUBSCRIPTIONRESPONSE']._serialized_end=7543
+  _globals['_ORDERSTATESTREAMRESPONSE_SUBSCRIPTIONRESPONSE_ERRORDETAIL']._serialized_start=7371
+  _globals['_ORDERSTATESTREAMRESPONSE_SUBSCRIPTIONRESPONSE_ERRORDETAIL']._serialized_end=7415
+  _globals['_ORDERSTATESTREAMRESPONSE_SUBSCRIPTIONRESPONSE_SUBSCRIPTIONSTATUS']._serialized_start=7417
+  _globals['_ORDERSTATESTREAMRESPONSE_SUBSCRIPTIONRESPONSE_SUBSCRIPTIONSTATUS']._serialized_end=7533
+  _globals['_ORDERSTATESTREAMRESPONSE_ORDERSTATE']._serialized_start=7546
+  _globals['_ORDERSTATESTREAMRESPONSE_ORDERSTATE']._serialized_end=8911
+  _globals['_ORDERSTATESTREAMRESPONSE_MARKERTYPE']._serialized_start=8914
+  _globals['_ORDERSTATESTREAMRESPONSE_MARKERTYPE']._serialized_end=9089
+  _globals['_ORDERSTATESTREAMRESPONSE_STATUSCAUSEINFO']._serialized_start=9092
+  _globals['_ORDERSTATESTREAMRESPONSE_STATUSCAUSEINFO']._serialized_end=9367
+  _globals['_ORDERSSTREAMSERVICE']._serialized_start=9993
+  _globals['_ORDERSSTREAMSERVICE']._serialized_end=10306
+  _globals['_ORDERSSERVICE']._serialized_start=10309
+  _globals['_ORDERSSERVICE']._serialized_end=11252
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/orders_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -117,15 +117,16 @@
     TIME_IN_FORCE_DAY: _TimeInForceType.ValueType  # 1
     """Заявка действует до конца торгового дня. Значение по умолчанию"""
     TIME_IN_FORCE_FILL_AND_KILL: _TimeInForceType.ValueType  # 2
     """Если в момент выставления возможно исполнение заявки(в т.ч. частичное), заявка будет исполнена или отменена сразу после выставления"""
     TIME_IN_FORCE_FILL_OR_KILL: _TimeInForceType.ValueType  # 3
     """Если в момент выставления возможно полное исполнение заявки, заявка будет исполнена или отменена сразу после выставления, недоступно для срочного рынка и торговли по выходным"""
 
-class TimeInForceType(_TimeInForceType, metaclass=_TimeInForceTypeEnumTypeWrapper): ...
+class TimeInForceType(_TimeInForceType, metaclass=_TimeInForceTypeEnumTypeWrapper):
+    """Алгоритм исполнения заявки"""
 
 TIME_IN_FORCE_UNSPECIFIED: TimeInForceType.ValueType  # 0
 """Значение не определено см. TIME_IN_FORCE_DAY"""
 TIME_IN_FORCE_DAY: TimeInForceType.ValueType  # 1
 """Заявка действует до конца торгового дня. Значение по умолчанию"""
 TIME_IN_FORCE_FILL_AND_KILL: TimeInForceType.ValueType  # 2
 """Если в момент выставления возможно исполнение заявки(в т.ч. частичное), заявка будет исполнена или отменена сразу после выставления"""
@@ -815,14 +816,16 @@
     def HasField(self, field_name: typing_extensions.Literal["buy_limits", b"buy_limits", "buy_margin_limits", b"buy_margin_limits", "sell_limits", b"sell_limits", "sell_margin_limits", b"sell_margin_limits"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["buy_limits", b"buy_limits", "buy_margin_limits", b"buy_margin_limits", "currency", b"currency", "sell_limits", b"sell_limits", "sell_margin_limits", b"sell_margin_limits"]) -> None: ...
 
 global___GetMaxLotsResponse = GetMaxLotsResponse
 
 @typing_extensions.final
 class GetOrderPriceRequest(google.protobuf.message.Message):
+    """Запрос получения предварительной стоимости заявки"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCOUNT_ID_FIELD_NUMBER: builtins.int
     INSTRUMENT_ID_FIELD_NUMBER: builtins.int
     PRICE_FIELD_NUMBER: builtins.int
     DIRECTION_FIELD_NUMBER: builtins.int
     QUANTITY_FIELD_NUMBER: builtins.int
@@ -849,14 +852,16 @@
     def HasField(self, field_name: typing_extensions.Literal["price", b"price"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["account_id", b"account_id", "direction", b"direction", "instrument_id", b"instrument_id", "price", b"price", "quantity", b"quantity"]) -> None: ...
 
 global___GetOrderPriceRequest = GetOrderPriceRequest
 
 @typing_extensions.final
 class GetOrderPriceResponse(google.protobuf.message.Message):
+    """Предварительная стоимость заявки"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ExtraBond(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ACI_VALUE_FIELD_NUMBER: builtins.int
@@ -941,7 +946,359 @@
         extra_future: global___GetOrderPriceResponse.ExtraFuture | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["deal_commission", b"deal_commission", "executed_commission", b"executed_commission", "executed_commission_rub", b"executed_commission_rub", "extra_bond", b"extra_bond", "extra_future", b"extra_future", "initial_order_amount", b"initial_order_amount", "instrument_extra", b"instrument_extra", "service_commission", b"service_commission", "total_order_amount", b"total_order_amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["deal_commission", b"deal_commission", "executed_commission", b"executed_commission", "executed_commission_rub", b"executed_commission_rub", "extra_bond", b"extra_bond", "extra_future", b"extra_future", "initial_order_amount", b"initial_order_amount", "instrument_extra", b"instrument_extra", "lots_requested", b"lots_requested", "service_commission", b"service_commission", "total_order_amount", b"total_order_amount"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["instrument_extra", b"instrument_extra"]) -> typing_extensions.Literal["extra_bond", "extra_future"] | None: ...
 
 global___GetOrderPriceResponse = GetOrderPriceResponse
+
+@typing_extensions.final
+class OrderStateStreamRequest(google.protobuf.message.Message):
+    """Запрос установки стрим-соединения торговых поручений"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ACCOUNTS_FIELD_NUMBER: builtins.int
+    PING_DELAY_MILLIS_FIELD_NUMBER: builtins.int
+    @property
+    def accounts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Идентификаторы счетов."""
+    ping_delay_millis: builtins.int
+    """Задержка пинг сообщений milliseconds 1000-120000, default 120000"""
+    def __init__(
+        self,
+        *,
+        accounts: collections.abc.Iterable[builtins.str] | None = ...,
+        ping_delay_millis: builtins.int | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_ping_delay_millis", b"_ping_delay_millis", "ping_delay_millis", b"ping_delay_millis"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_ping_delay_millis", b"_ping_delay_millis", "accounts", b"accounts", "ping_delay_millis", b"ping_delay_millis"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_ping_delay_millis", b"_ping_delay_millis"]) -> typing_extensions.Literal["ping_delay_millis"] | None: ...
+
+global___OrderStateStreamRequest = OrderStateStreamRequest
+
+@typing_extensions.final
+class OrderStateStreamResponse(google.protobuf.message.Message):
+    """Информация по заявкам"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _MarkerType:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _MarkerTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[OrderStateStreamResponse._MarkerType.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        MARKER_UNKNOWN: OrderStateStreamResponse._MarkerType.ValueType  # 0
+        """не определено"""
+        MARKER_BROKER: OrderStateStreamResponse._MarkerType.ValueType  # 1
+        """сделки брокера"""
+        MARKER_CHAT: OrderStateStreamResponse._MarkerType.ValueType  # 2
+        """исполнение поручение, полученного от клиента через каналы связи"""
+        MARKER_PAPER: OrderStateStreamResponse._MarkerType.ValueType  # 3
+        """исполнение поручение, полученного от клиента в бумажной форме"""
+        MARKER_MARGIN: OrderStateStreamResponse._MarkerType.ValueType  # 4
+        """принудительное закрытие позиций"""
+        MARKER_TKBNM: OrderStateStreamResponse._MarkerType.ValueType  # 5
+        """сделки по управлению ликвидностью"""
+        MARKER_SHORT: OrderStateStreamResponse._MarkerType.ValueType  # 6
+        """сделки РЕПО по привлечению у клиентов бумаг"""
+        MARKER_SPECMM: OrderStateStreamResponse._MarkerType.ValueType  # 7
+        """перенос временно непокрытых позиций"""
+        MARKER_PO: OrderStateStreamResponse._MarkerType.ValueType  # 8
+
+    class MarkerType(_MarkerType, metaclass=_MarkerTypeEnumTypeWrapper):
+        """Маркер"""
+
+    MARKER_UNKNOWN: OrderStateStreamResponse.MarkerType.ValueType  # 0
+    """не определено"""
+    MARKER_BROKER: OrderStateStreamResponse.MarkerType.ValueType  # 1
+    """сделки брокера"""
+    MARKER_CHAT: OrderStateStreamResponse.MarkerType.ValueType  # 2
+    """исполнение поручение, полученного от клиента через каналы связи"""
+    MARKER_PAPER: OrderStateStreamResponse.MarkerType.ValueType  # 3
+    """исполнение поручение, полученного от клиента в бумажной форме"""
+    MARKER_MARGIN: OrderStateStreamResponse.MarkerType.ValueType  # 4
+    """принудительное закрытие позиций"""
+    MARKER_TKBNM: OrderStateStreamResponse.MarkerType.ValueType  # 5
+    """сделки по управлению ликвидностью"""
+    MARKER_SHORT: OrderStateStreamResponse.MarkerType.ValueType  # 6
+    """сделки РЕПО по привлечению у клиентов бумаг"""
+    MARKER_SPECMM: OrderStateStreamResponse.MarkerType.ValueType  # 7
+    """перенос временно непокрытых позиций"""
+    MARKER_PO: OrderStateStreamResponse.MarkerType.ValueType  # 8
+
+    class _StatusCauseInfo:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _StatusCauseInfoEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[OrderStateStreamResponse._StatusCauseInfo.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        CAUSE_UNSPECIFIED: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 0
+        """Не определено"""
+        CAUSE_CANCELLED_BY_CLIENT: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 15
+        """Отменено клиентом"""
+        CAUSE_CANCELLED_BY_EXCHANGE: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 1
+        """Отменено биржей"""
+        CAUSE_CANCELLED_NOT_ENOUGH_POSITION: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 2
+        """Заявка не выставлена из-за нехватки средств"""
+        CAUSE_CANCELLED_BY_CLIENT_BLOCK: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 3
+        """Отменено из-за блокировки клиента"""
+        CAUSE_REJECTED_BY_BROKER: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 4
+        """Отклонено брокером"""
+        CAUSE_REJECTED_BY_EXCHANGE: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 5
+        """Отклонено биржей"""
+        CAUSE_CANCELLED_BY_BROKER: OrderStateStreamResponse._StatusCauseInfo.ValueType  # 6
+        """Отменено брокером"""
+
+    class StatusCauseInfo(_StatusCauseInfo, metaclass=_StatusCauseInfoEnumTypeWrapper):
+        """Дополнительная информация по статусу заявки"""
+
+    CAUSE_UNSPECIFIED: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 0
+    """Не определено"""
+    CAUSE_CANCELLED_BY_CLIENT: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 15
+    """Отменено клиентом"""
+    CAUSE_CANCELLED_BY_EXCHANGE: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 1
+    """Отменено биржей"""
+    CAUSE_CANCELLED_NOT_ENOUGH_POSITION: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 2
+    """Заявка не выставлена из-за нехватки средств"""
+    CAUSE_CANCELLED_BY_CLIENT_BLOCK: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 3
+    """Отменено из-за блокировки клиента"""
+    CAUSE_REJECTED_BY_BROKER: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 4
+    """Отклонено брокером"""
+    CAUSE_REJECTED_BY_EXCHANGE: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 5
+    """Отклонено биржей"""
+    CAUSE_CANCELLED_BY_BROKER: OrderStateStreamResponse.StatusCauseInfo.ValueType  # 6
+    """Отменено брокером"""
+
+    @typing_extensions.final
+    class SubscriptionResponse(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        class _SubscriptionStatus:
+            ValueType = typing.NewType("ValueType", builtins.int)
+            V: typing_extensions.TypeAlias = ValueType
+
+        class _SubscriptionStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[OrderStateStreamResponse.SubscriptionResponse._SubscriptionStatus.ValueType], builtins.type):
+            DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+            SUBSCRIPTION_STATUS_UNSPECIFIED: OrderStateStreamResponse.SubscriptionResponse._SubscriptionStatus.ValueType  # 0
+            """Статус подписки не определен."""
+            SUBSCRIPTION_STATUS_OK: OrderStateStreamResponse.SubscriptionResponse._SubscriptionStatus.ValueType  # 1
+            """Подписка успешно установлена."""
+            SUBSCRIPTION_STATUS_ERROR: OrderStateStreamResponse.SubscriptionResponse._SubscriptionStatus.ValueType  # 13
+            """Ошибка подписки"""
+
+        class SubscriptionStatus(_SubscriptionStatus, metaclass=_SubscriptionStatusEnumTypeWrapper): ...
+        SUBSCRIPTION_STATUS_UNSPECIFIED: OrderStateStreamResponse.SubscriptionResponse.SubscriptionStatus.ValueType  # 0
+        """Статус подписки не определен."""
+        SUBSCRIPTION_STATUS_OK: OrderStateStreamResponse.SubscriptionResponse.SubscriptionStatus.ValueType  # 1
+        """Подписка успешно установлена."""
+        SUBSCRIPTION_STATUS_ERROR: OrderStateStreamResponse.SubscriptionResponse.SubscriptionStatus.ValueType  # 13
+        """Ошибка подписки"""
+
+        @typing_extensions.final
+        class ErrorDetail(google.protobuf.message.Message):
+            DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+            CODE_FIELD_NUMBER: builtins.int
+            MESSAGE_FIELD_NUMBER: builtins.int
+            code: builtins.str
+            """Код ошибки."""
+            message: builtins.str
+            """Описание ошибки."""
+            def __init__(
+                self,
+                *,
+                code: builtins.str = ...,
+                message: builtins.str = ...,
+            ) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "message", b"message"]) -> None: ...
+
+        TRACKING_ID_FIELD_NUMBER: builtins.int
+        STATUS_FIELD_NUMBER: builtins.int
+        STREAM_ID_FIELD_NUMBER: builtins.int
+        ACCOUNTS_FIELD_NUMBER: builtins.int
+        ERROR_FIELD_NUMBER: builtins.int
+        tracking_id: builtins.str
+        """Уникальный идентификатор запроса, подробнее: [tracking_id](https://russianinvestments.github.io/investAPI/grpc#tracking-id)."""
+        status: global___OrderStateStreamResponse.SubscriptionResponse.SubscriptionStatus.ValueType
+        """Статус подписки."""
+        stream_id: builtins.str
+        """Идентификатор открытого соединения"""
+        @property
+        def accounts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+            """Идентификаторы счетов."""
+        @property
+        def error(self) -> global___OrderStateStreamResponse.SubscriptionResponse.ErrorDetail: ...
+        def __init__(
+            self,
+            *,
+            tracking_id: builtins.str = ...,
+            status: global___OrderStateStreamResponse.SubscriptionResponse.SubscriptionStatus.ValueType = ...,
+            stream_id: builtins.str = ...,
+            accounts: collections.abc.Iterable[builtins.str] | None = ...,
+            error: global___OrderStateStreamResponse.SubscriptionResponse.ErrorDetail | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["_error", b"_error", "error", b"error"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["_error", b"_error", "accounts", b"accounts", "error", b"error", "status", b"status", "stream_id", b"stream_id", "tracking_id", b"tracking_id"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["_error", b"_error"]) -> typing_extensions.Literal["error"] | None: ...
+
+    @typing_extensions.final
+    class OrderState(google.protobuf.message.Message):
+        """Заявка"""
+
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        ORDER_ID_FIELD_NUMBER: builtins.int
+        ORDER_REQUEST_ID_FIELD_NUMBER: builtins.int
+        CLIENT_CODE_FIELD_NUMBER: builtins.int
+        CREATED_AT_FIELD_NUMBER: builtins.int
+        EXECUTION_REPORT_STATUS_FIELD_NUMBER: builtins.int
+        STATUS_INFO_FIELD_NUMBER: builtins.int
+        TICKER_FIELD_NUMBER: builtins.int
+        CLASS_CODE_FIELD_NUMBER: builtins.int
+        LOT_SIZE_FIELD_NUMBER: builtins.int
+        DIRECTION_FIELD_NUMBER: builtins.int
+        TIME_IN_FORCE_FIELD_NUMBER: builtins.int
+        ORDER_TYPE_FIELD_NUMBER: builtins.int
+        ACCOUNT_ID_FIELD_NUMBER: builtins.int
+        INITIAL_ORDER_PRICE_FIELD_NUMBER: builtins.int
+        ORDER_PRICE_FIELD_NUMBER: builtins.int
+        AMOUNT_FIELD_NUMBER: builtins.int
+        EXECUTED_ORDER_PRICE_FIELD_NUMBER: builtins.int
+        CURRENCY_FIELD_NUMBER: builtins.int
+        LOTS_REQUESTED_FIELD_NUMBER: builtins.int
+        LOTS_EXECUTED_FIELD_NUMBER: builtins.int
+        LOTS_LEFT_FIELD_NUMBER: builtins.int
+        LOTS_CANCELLED_FIELD_NUMBER: builtins.int
+        MARKER_FIELD_NUMBER: builtins.int
+        TRADES_FIELD_NUMBER: builtins.int
+        COMPLETION_TIME_FIELD_NUMBER: builtins.int
+        EXCHANGE_FIELD_NUMBER: builtins.int
+        INSTRUMENT_UID_FIELD_NUMBER: builtins.int
+        order_id: builtins.str
+        """Биржевой идентификатор заявки"""
+        order_request_id: builtins.str
+        """Идентификатор ключа идемпотентности, переданный клиентом, в формате UID. Максимальная длина 36 символов."""
+        client_code: builtins.str
+        """Код клиента на бирже"""
+        @property
+        def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp:
+            """Дата создания заявки"""
+        execution_report_status: global___OrderExecutionReportStatus.ValueType
+        """Статус заявки"""
+        status_info: global___OrderStateStreamResponse.StatusCauseInfo.ValueType
+        """Дополнительная информация по статусу"""
+        ticker: builtins.str
+        """Тикер инструмента"""
+        class_code: builtins.str
+        """Класс-код (секция торгов)"""
+        lot_size: builtins.int
+        """Лотность инструмента заявки"""
+        direction: global___OrderDirection.ValueType
+        """Направление заявки"""
+        time_in_force: global___TimeInForceType.ValueType
+        """Алгоритм исполнения поручения"""
+        order_type: global___OrderType.ValueType
+        """Тип заявки"""
+        account_id: builtins.str
+        """Номер счета"""
+        @property
+        def initial_order_price(self) -> tinkoff.invest.grpc.common_pb2.MoneyValue:
+            """Начальная цена заявки"""
+        @property
+        def order_price(self) -> tinkoff.invest.grpc.common_pb2.MoneyValue:
+            """Цена выставления заявки"""
+        @property
+        def amount(self) -> tinkoff.invest.grpc.common_pb2.MoneyValue:
+            """Предрассчитанная стоимость полной заявки"""
+        @property
+        def executed_order_price(self) -> tinkoff.invest.grpc.common_pb2.MoneyValue:
+            """Исполненная средняя цена одного инструмента в заявке"""
+        currency: builtins.str
+        """Валюта исполнения"""
+        lots_requested: builtins.int
+        """Запрошено лотов"""
+        lots_executed: builtins.int
+        """Исполнено лотов"""
+        lots_left: builtins.int
+        """Число неисполненных лотов по заявке"""
+        lots_cancelled: builtins.int
+        """Отмененные лоты"""
+        marker: global___OrderStateStreamResponse.MarkerType.ValueType
+        """Спецсимвол"""
+        @property
+        def trades(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OrderTrade]:
+            """	Список сделок"""
+        @property
+        def completion_time(self) -> google.protobuf.timestamp_pb2.Timestamp:
+            """Время исполнения заявки"""
+        exchange: builtins.str
+        """Код биржи"""
+        instrument_uid: builtins.str
+        """UID идентификатор инструмента"""
+        def __init__(
+            self,
+            *,
+            order_id: builtins.str = ...,
+            order_request_id: builtins.str | None = ...,
+            client_code: builtins.str = ...,
+            created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+            execution_report_status: global___OrderExecutionReportStatus.ValueType = ...,
+            status_info: global___OrderStateStreamResponse.StatusCauseInfo.ValueType | None = ...,
+            ticker: builtins.str = ...,
+            class_code: builtins.str = ...,
+            lot_size: builtins.int = ...,
+            direction: global___OrderDirection.ValueType = ...,
+            time_in_force: global___TimeInForceType.ValueType = ...,
+            order_type: global___OrderType.ValueType = ...,
+            account_id: builtins.str = ...,
+            initial_order_price: tinkoff.invest.grpc.common_pb2.MoneyValue | None = ...,
+            order_price: tinkoff.invest.grpc.common_pb2.MoneyValue | None = ...,
+            amount: tinkoff.invest.grpc.common_pb2.MoneyValue | None = ...,
+            executed_order_price: tinkoff.invest.grpc.common_pb2.MoneyValue | None = ...,
+            currency: builtins.str = ...,
+            lots_requested: builtins.int = ...,
+            lots_executed: builtins.int = ...,
+            lots_left: builtins.int = ...,
+            lots_cancelled: builtins.int = ...,
+            marker: global___OrderStateStreamResponse.MarkerType.ValueType | None = ...,
+            trades: collections.abc.Iterable[global___OrderTrade] | None = ...,
+            completion_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+            exchange: builtins.str = ...,
+            instrument_uid: builtins.str = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["_amount", b"_amount", "_marker", b"_marker", "_order_request_id", b"_order_request_id", "_status_info", b"_status_info", "amount", b"amount", "completion_time", b"completion_time", "created_at", b"created_at", "executed_order_price", b"executed_order_price", "initial_order_price", b"initial_order_price", "marker", b"marker", "order_price", b"order_price", "order_request_id", b"order_request_id", "status_info", b"status_info"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["_amount", b"_amount", "_marker", b"_marker", "_order_request_id", b"_order_request_id", "_status_info", b"_status_info", "account_id", b"account_id", "amount", b"amount", "class_code", b"class_code", "client_code", b"client_code", "completion_time", b"completion_time", "created_at", b"created_at", "currency", b"currency", "direction", b"direction", "exchange", b"exchange", "executed_order_price", b"executed_order_price", "execution_report_status", b"execution_report_status", "initial_order_price", b"initial_order_price", "instrument_uid", b"instrument_uid", "lot_size", b"lot_size", "lots_cancelled", b"lots_cancelled", "lots_executed", b"lots_executed", "lots_left", b"lots_left", "lots_requested", b"lots_requested", "marker", b"marker", "order_id", b"order_id", "order_price", b"order_price", "order_request_id", b"order_request_id", "order_type", b"order_type", "status_info", b"status_info", "ticker", b"ticker", "time_in_force", b"time_in_force", "trades", b"trades"]) -> None: ...
+        @typing.overload
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["_amount", b"_amount"]) -> typing_extensions.Literal["amount"] | None: ...
+        @typing.overload
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["_marker", b"_marker"]) -> typing_extensions.Literal["marker"] | None: ...
+        @typing.overload
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["_order_request_id", b"_order_request_id"]) -> typing_extensions.Literal["order_request_id"] | None: ...
+        @typing.overload
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["_status_info", b"_status_info"]) -> typing_extensions.Literal["status_info"] | None: ...
+
+    ORDER_STATE_FIELD_NUMBER: builtins.int
+    PING_FIELD_NUMBER: builtins.int
+    SUBSCRIPTION_FIELD_NUMBER: builtins.int
+    @property
+    def order_state(self) -> global___OrderStateStreamResponse.OrderState:
+        """Информация об исполнении торгового поручения."""
+    @property
+    def ping(self) -> tinkoff.invest.grpc.common_pb2.Ping:
+        """Проверка активности стрима."""
+    @property
+    def subscription(self) -> global___OrderStateStreamResponse.SubscriptionResponse:
+        """Ответ на запрос на подписку."""
+    def __init__(
+        self,
+        *,
+        order_state: global___OrderStateStreamResponse.OrderState | None = ...,
+        ping: tinkoff.invest.grpc.common_pb2.Ping | None = ...,
+        subscription: global___OrderStateStreamResponse.SubscriptionResponse | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["order_state", b"order_state", "payload", b"payload", "ping", b"ping", "subscription", b"subscription"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["order_state", b"order_state", "payload", b"payload", "ping", b"ping", "subscription", b"subscription"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["payload", b"payload"]) -> typing_extensions.Literal["order_state", "ping", "subscription"] | None: ...
+
+global___OrderStateStreamResponse = OrderStateStreamResponse
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/orders_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/orders_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,51 @@
             channel: A grpc.Channel.
         """
         self.TradesStream = channel.unary_stream(
                 '/tinkoff.public.invest.api.contract.v1.OrdersStreamService/TradesStream',
                 request_serializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.TradesStreamRequest.SerializeToString,
                 response_deserializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.TradesStreamResponse.FromString,
                 )
+        self.OrderStateStream = channel.unary_stream(
+                '/tinkoff.public.invest.api.contract.v1.OrdersStreamService/OrderStateStream',
+                request_serializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.OrderStateStreamRequest.SerializeToString,
+                response_deserializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.OrderStateStreamResponse.FromString,
+                )
 
 
 class OrdersStreamServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def TradesStream(self, request, context):
         """Stream сделок пользователя
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def OrderStateStream(self, request, context):
+        """Stream поручений пользователя
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_OrdersStreamServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'TradesStream': grpc.unary_stream_rpc_method_handler(
                     servicer.TradesStream,
                     request_deserializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.TradesStreamRequest.FromString,
                     response_serializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.TradesStreamResponse.SerializeToString,
             ),
+            'OrderStateStream': grpc.unary_stream_rpc_method_handler(
+                    servicer.OrderStateStream,
+                    request_deserializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.OrderStateStreamRequest.FromString,
+                    response_serializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.OrderStateStreamResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'tinkoff.public.invest.api.contract.v1.OrdersStreamService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -64,14 +81,31 @@
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/tinkoff.public.invest.api.contract.v1.OrdersStreamService/TradesStream',
             tinkoff_dot_invest_dot_grpc_dot_orders__pb2.TradesStreamRequest.SerializeToString,
             tinkoff_dot_invest_dot_grpc_dot_orders__pb2.TradesStreamResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def OrderStateStream(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/tinkoff.public.invest.api.contract.v1.OrdersStreamService/OrderStateStream',
+            tinkoff_dot_invest_dot_grpc_dot_orders__pb2.OrderStateStreamRequest.SerializeToString,
+            tinkoff_dot_invest_dot_grpc_dot_orders__pb2.OrderStateStreamResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class OrdersServiceStub(object):
     """Сервис предназначен для работы с торговыми поручениями:</br> **1**.
     выставление;</br> **2**. отмена;</br> **3**. получение статуса;</br> **4**.
     расчёт полной стоимости;</br> **5**. получение списка заявок.
     """
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/sandbox_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     orders_pb2 as tinkoff_dot_invest_dot_grpc_dot_orders__pb2,
     users_pb2 as tinkoff_dot_invest_dot_grpc_dot_users__pb2,
 )
 from tinkoff.invest.grpc.google.api import (
     field_behavior_pb2 as tinkoff_dot_invest_dot_grpc_dot_google_dot_api_dot_field__behavior__pb2,
 )
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!tinkoff/invest/grpc/sandbox.proto\x12%tinkoff.public.invest.api.contract.v1\x1a tinkoff/invest/grpc/common.proto\x1a tinkoff/invest/grpc/orders.proto\x1a$tinkoff/invest/grpc/operations.proto\x1a\x1ftinkoff/invest/grpc/users.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"7\n\x19OpenSandboxAccountRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_name\"0\n\x1aOpenSandboxAccountResponse\x12\x12\n\naccount_id\x18\x01 \x01(\t\"6\n\x1a\x43loseSandboxAccountRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"\x1d\n\x1b\x43loseSandboxAccountResponse\"x\n\x13SandboxPayInRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12G\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValueB\x04\xe2\x41\x01\x02\"Z\n\x14SandboxPayInResponse\x12\x42\n\x07\x62\x61lance\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue2\x82\x10\n\x0eSandboxService\x12\x99\x01\n\x12OpenSandboxAccount\x12@.tinkoff.public.invest.api.contract.v1.OpenSandboxAccountRequest\x1a\x41.tinkoff.public.invest.api.contract.v1.OpenSandboxAccountResponse\x12\x8b\x01\n\x12GetSandboxAccounts\x12\x39.tinkoff.public.invest.api.contract.v1.GetAccountsRequest\x1a:.tinkoff.public.invest.api.contract.v1.GetAccountsResponse\x12\x9c\x01\n\x13\x43loseSandboxAccount\x12\x41.tinkoff.public.invest.api.contract.v1.CloseSandboxAccountRequest\x1a\x42.tinkoff.public.invest.api.contract.v1.CloseSandboxAccountResponse\x12\x85\x01\n\x10PostSandboxOrder\x12\x37.tinkoff.public.invest.api.contract.v1.PostOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x8b\x01\n\x13ReplaceSandboxOrder\x12:.tinkoff.public.invest.api.contract.v1.ReplaceOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x85\x01\n\x10GetSandboxOrders\x12\x37.tinkoff.public.invest.api.contract.v1.GetOrdersRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.GetOrdersResponse\x12\x8b\x01\n\x12\x43\x61ncelSandboxOrder\x12\x39.tinkoff.public.invest.api.contract.v1.CancelOrderRequest\x1a:.tinkoff.public.invest.api.contract.v1.CancelOrderResponse\x12\x86\x01\n\x14GetSandboxOrderState\x12;.tinkoff.public.invest.api.contract.v1.GetOrderStateRequest\x1a\x31.tinkoff.public.invest.api.contract.v1.OrderState\x12\x88\x01\n\x13GetSandboxPositions\x12\x37.tinkoff.public.invest.api.contract.v1.PositionsRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PositionsResponse\x12\x8b\x01\n\x14GetSandboxOperations\x12\x38.tinkoff.public.invest.api.contract.v1.OperationsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.OperationsResponse\x12\xa9\x01\n\x1cGetSandboxOperationsByCursor\x12\x43.tinkoff.public.invest.api.contract.v1.GetOperationsByCursorRequest\x1a\x44.tinkoff.public.invest.api.contract.v1.GetOperationsByCursorResponse\x12\x88\x01\n\x13GetSandboxPortfolio\x12\x37.tinkoff.public.invest.api.contract.v1.PortfolioRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PortfolioResponse\x12\x87\x01\n\x0cSandboxPayIn\x12:.tinkoff.public.invest.api.contract.v1.SandboxPayInRequest\x1a;.tinkoff.public.invest.api.contract.v1.SandboxPayInResponse\x12\x97\x01\n\x18GetSandboxWithdrawLimits\x12<.tinkoff.public.invest.api.contract.v1.WithdrawLimitsRequest\x1a=.tinkoff.public.invest.api.contract.v1.WithdrawLimitsResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!tinkoff/invest/grpc/sandbox.proto\x12%tinkoff.public.invest.api.contract.v1\x1a tinkoff/invest/grpc/common.proto\x1a tinkoff/invest/grpc/orders.proto\x1a$tinkoff/invest/grpc/operations.proto\x1a\x1ftinkoff/invest/grpc/users.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\"7\n\x19OpenSandboxAccountRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_name\"0\n\x1aOpenSandboxAccountResponse\x12\x12\n\naccount_id\x18\x01 \x01(\t\"6\n\x1a\x43loseSandboxAccountRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\"\x1d\n\x1b\x43loseSandboxAccountResponse\"x\n\x13SandboxPayInRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12G\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValueB\x04\xe2\x41\x01\x02\"Z\n\x14SandboxPayInResponse\x12\x42\n\x07\x62\x61lance\x18\x01 \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue2\x8d\x11\n\x0eSandboxService\x12\x99\x01\n\x12OpenSandboxAccount\x12@.tinkoff.public.invest.api.contract.v1.OpenSandboxAccountRequest\x1a\x41.tinkoff.public.invest.api.contract.v1.OpenSandboxAccountResponse\x12\x8b\x01\n\x12GetSandboxAccounts\x12\x39.tinkoff.public.invest.api.contract.v1.GetAccountsRequest\x1a:.tinkoff.public.invest.api.contract.v1.GetAccountsResponse\x12\x9c\x01\n\x13\x43loseSandboxAccount\x12\x41.tinkoff.public.invest.api.contract.v1.CloseSandboxAccountRequest\x1a\x42.tinkoff.public.invest.api.contract.v1.CloseSandboxAccountResponse\x12\x85\x01\n\x10PostSandboxOrder\x12\x37.tinkoff.public.invest.api.contract.v1.PostOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x8b\x01\n\x13ReplaceSandboxOrder\x12:.tinkoff.public.invest.api.contract.v1.ReplaceOrderRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PostOrderResponse\x12\x85\x01\n\x10GetSandboxOrders\x12\x37.tinkoff.public.invest.api.contract.v1.GetOrdersRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.GetOrdersResponse\x12\x8b\x01\n\x12\x43\x61ncelSandboxOrder\x12\x39.tinkoff.public.invest.api.contract.v1.CancelOrderRequest\x1a:.tinkoff.public.invest.api.contract.v1.CancelOrderResponse\x12\x86\x01\n\x14GetSandboxOrderState\x12;.tinkoff.public.invest.api.contract.v1.GetOrderStateRequest\x1a\x31.tinkoff.public.invest.api.contract.v1.OrderState\x12\x88\x01\n\x13GetSandboxPositions\x12\x37.tinkoff.public.invest.api.contract.v1.PositionsRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PositionsResponse\x12\x8b\x01\n\x14GetSandboxOperations\x12\x38.tinkoff.public.invest.api.contract.v1.OperationsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.OperationsResponse\x12\xa9\x01\n\x1cGetSandboxOperationsByCursor\x12\x43.tinkoff.public.invest.api.contract.v1.GetOperationsByCursorRequest\x1a\x44.tinkoff.public.invest.api.contract.v1.GetOperationsByCursorResponse\x12\x88\x01\n\x13GetSandboxPortfolio\x12\x37.tinkoff.public.invest.api.contract.v1.PortfolioRequest\x1a\x38.tinkoff.public.invest.api.contract.v1.PortfolioResponse\x12\x87\x01\n\x0cSandboxPayIn\x12:.tinkoff.public.invest.api.contract.v1.SandboxPayInRequest\x1a;.tinkoff.public.invest.api.contract.v1.SandboxPayInResponse\x12\x97\x01\n\x18GetSandboxWithdrawLimits\x12<.tinkoff.public.invest.api.contract.v1.WithdrawLimitsRequest\x1a=.tinkoff.public.invest.api.contract.v1.WithdrawLimitsResponse\x12\x88\x01\n\x11GetSandboxMaxLots\x12\x38.tinkoff.public.invest.api.contract.v1.GetMaxLotsRequest\x1a\x39.tinkoff.public.invest.api.contract.v1.GetMaxLotsResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tinkoff.invest.grpc.sandbox_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034ru.tinkoff.piapi.contract.v1P\001Z\014./;investapi\242\002\005TIAPI\252\002\024Tinkoff.InvestApi.V1\312\002\021Tinkoff\\Invest\\V1'
@@ -47,9 +47,9 @@
   _globals['_CLOSESANDBOXACCOUNTRESPONSE']._serialized_start=431
   _globals['_CLOSESANDBOXACCOUNTRESPONSE']._serialized_end=460
   _globals['_SANDBOXPAYINREQUEST']._serialized_start=462
   _globals['_SANDBOXPAYINREQUEST']._serialized_end=582
   _globals['_SANDBOXPAYINRESPONSE']._serialized_start=584
   _globals['_SANDBOXPAYINRESPONSE']._serialized_end=674
   _globals['_SANDBOXSERVICE']._serialized_start=677
-  _globals['_SANDBOXSERVICE']._serialized_end=2727
+  _globals['_SANDBOXSERVICE']._serialized_end=2866
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/sandbox_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/sandbox_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/sandbox_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     orders_pb2 as tinkoff_dot_invest_dot_grpc_dot_orders__pb2,
     sandbox_pb2 as tinkoff_dot_invest_dot_grpc_dot_sandbox__pb2,
     users_pb2 as tinkoff_dot_invest_dot_grpc_dot_users__pb2,
 )
 
 
 class SandboxServiceStub(object):
-    """Сервис для работы с песочницей TINKOFF INVEST API
+    """Методы для работы с песочницей Tinkoff Invest API
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -86,113 +86,125 @@
                 response_deserializer=tinkoff_dot_invest_dot_grpc_dot_sandbox__pb2.SandboxPayInResponse.FromString,
                 )
         self.GetSandboxWithdrawLimits = channel.unary_unary(
                 '/tinkoff.public.invest.api.contract.v1.SandboxService/GetSandboxWithdrawLimits',
                 request_serializer=tinkoff_dot_invest_dot_grpc_dot_operations__pb2.WithdrawLimitsRequest.SerializeToString,
                 response_deserializer=tinkoff_dot_invest_dot_grpc_dot_operations__pb2.WithdrawLimitsResponse.FromString,
                 )
+        self.GetSandboxMaxLots = channel.unary_unary(
+                '/tinkoff.public.invest.api.contract.v1.SandboxService/GetSandboxMaxLots',
+                request_serializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.GetMaxLotsRequest.SerializeToString,
+                response_deserializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.GetMaxLotsResponse.FromString,
+                )
 
 
 class SandboxServiceServicer(object):
-    """Сервис для работы с песочницей TINKOFF INVEST API
+    """Методы для работы с песочницей Tinkoff Invest API
     """
 
     def OpenSandboxAccount(self, request, context):
-        """Метод регистрации счёта в песочнице.
+        """Зарегистрировать счёт.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxAccounts(self, request, context):
-        """Метод получения счетов в песочнице.
+        """Получить счета.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CloseSandboxAccount(self, request, context):
-        """Метод закрытия счёта в песочнице.
+        """Закрыть счёт.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PostSandboxOrder(self, request, context):
-        """Метод выставления торгового поручения в песочнице.
+        """Выставить торговое поручение.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ReplaceSandboxOrder(self, request, context):
-        """Метод изменения выставленной заявки.
+        """Изменить выставленную заявку.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxOrders(self, request, context):
-        """Метод получения списка активных заявок по счёту в песочнице.
+        """Получить список активных заявок по счёту.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CancelSandboxOrder(self, request, context):
-        """Метод отмены торгового поручения в песочнице.
+        """Отменить торговое поручение.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxOrderState(self, request, context):
-        """Метод получения статуса заявки в песочнице. Заявки хранятся в таблице 7 дней.
+        """Поулчить статус заявки в песочнице. Заявки хранятся в таблице 7 дней.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxPositions(self, request, context):
-        """Метод получения позиций по виртуальному счёту песочницы.
+        """Получить позиции по виртуальному счёту.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxOperations(self, request, context):
-        """Метод получения операций в песочнице по номеру счёта.
+        """Получить операции по номеру счёта.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxOperationsByCursor(self, request, context):
-        """Метод получения операций в песочнице по номеру счета с пагинацией.
+        """Получить операции по номеру счёта с пагинацией.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxPortfolio(self, request, context):
-        """Метод получения портфолио в песочнице.
+        """Получить портфель.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SandboxPayIn(self, request, context):
-        """Метод пополнения счёта в песочнице.
+        """Пополнить счёт.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSandboxWithdrawLimits(self, request, context):
-        """Метод получения доступного остатка для вывода средств в песочнице.
+        """Получить доступный остаток для вывода средств.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSandboxMaxLots(self, request, context):
+        """Расчёт количества доступных для покупки/продажи лотов в песочнице.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SandboxServiceServicer_to_server(servicer, server):
@@ -263,23 +275,28 @@
                     response_serializer=tinkoff_dot_invest_dot_grpc_dot_sandbox__pb2.SandboxPayInResponse.SerializeToString,
             ),
             'GetSandboxWithdrawLimits': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSandboxWithdrawLimits,
                     request_deserializer=tinkoff_dot_invest_dot_grpc_dot_operations__pb2.WithdrawLimitsRequest.FromString,
                     response_serializer=tinkoff_dot_invest_dot_grpc_dot_operations__pb2.WithdrawLimitsResponse.SerializeToString,
             ),
+            'GetSandboxMaxLots': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSandboxMaxLots,
+                    request_deserializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.GetMaxLotsRequest.FromString,
+                    response_serializer=tinkoff_dot_invest_dot_grpc_dot_orders__pb2.GetMaxLotsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'tinkoff.public.invest.api.contract.v1.SandboxService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class SandboxService(object):
-    """Сервис для работы с песочницей TINKOFF INVEST API
+    """Методы для работы с песочницей Tinkoff Invest API
     """
 
     @staticmethod
     def OpenSandboxAccount(request,
             target,
             options=(),
             channel_credentials=None,
@@ -511,7 +528,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/tinkoff.public.invest.api.contract.v1.SandboxService/GetSandboxWithdrawLimits',
             tinkoff_dot_invest_dot_grpc_dot_operations__pb2.WithdrawLimitsRequest.SerializeToString,
             tinkoff_dot_invest_dot_grpc_dot_operations__pb2.WithdrawLimitsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSandboxMaxLots(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/tinkoff.public.invest.api.contract.v1.SandboxService/GetSandboxMaxLots',
+            tinkoff_dot_invest_dot_grpc_dot_orders__pb2.GetMaxLotsRequest.SerializeToString,
+            tinkoff_dot_invest_dot_grpc_dot_orders__pb2.GetMaxLotsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/stoporders_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from tinkoff.invest.grpc import (
     common_pb2 as tinkoff_dot_invest_dot_grpc_dot_common__pb2,
 )
 from tinkoff.invest.grpc.google.api import (
     field_behavior_pb2 as tinkoff_dot_invest_dot_grpc_dot_google_dot_api_dot_field__behavior__pb2,
 )
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tinkoff/invest/grpc/stoporders.proto\x12%tinkoff.public.invest.api.contract.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\x1a tinkoff/invest/grpc/common.proto\"\x97\n\n\x14PostStopOrderRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x16\n\x08quantity\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x01\x88\x01\x01\x12I\n\nstop_price\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x02\x88\x01\x01\x12R\n\tdirection\x18\x05 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.StopOrderDirectionB\x04\xe2\x41\x01\x02\x12\x18\n\naccount_id\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02\x12]\n\x0f\x65xpiration_type\x18\x07 \x01(\x0e\x32>.tinkoff.public.invest.api.contract.v1.StopOrderExpirationTypeB\x04\xe2\x41\x01\x02\x12S\n\x0fstop_order_type\x18\x08 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.StopOrderTypeB\x04\xe2\x41\x01\x02\x12\x34\n\x0b\x65xpire_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\n \x01(\tB\x04\xe2\x41\x01\x02\x12U\n\x13\x65xchange_order_type\x18\x0b \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.ExchangeOrderType\x12O\n\x10take_profit_type\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.TakeProfitType\x12_\n\rtrailing_data\x18\r \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.PostStopOrderRequest.TrailingData\x12\x44\n\nprice_type\x18\x0e \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceType\x12\x16\n\x08order_id\x18\x0f \x01(\tB\x04\xe2\x41\x01\x02\x1a\xb0\x02\n\x0cTrailingData\x12@\n\x06indent\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bindent_type\x18\x02 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueType\x12@\n\x06spread\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bspread_type\x18\x04 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueTypeB\x07\n\x05_figiB\x08\n\x06_priceB\r\n\x0b_stop_priceB\x0e\n\x0c_expire_date\"\x9d\x01\n\x15PostStopOrderResponse\x12\x15\n\rstop_order_id\x18\x01 \x01(\t\x12\x18\n\x10order_request_id\x18\x02 \x01(\t\x12S\n\x11response_metadata\x18\xfe\x01 \x01(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.ResponseMetadata\"\xd0\x01\n\x14GetStopOrdersRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12L\n\x06status\x18\x02 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.StopOrderStatusOption\x12(\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x02to\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"^\n\x15GetStopOrdersResponse\x12\x45\n\x0bstop_orders\x18\x01 \x03(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.StopOrder\"O\n\x16\x43\x61ncelStopOrderRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x1b\n\rstop_order_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\"C\n\x17\x43\x61ncelStopOrderResponse\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa7\n\n\tStopOrder\x12\x15\n\rstop_order_id\x18\x01 \x01(\t\x12\x16\n\x0elots_requested\x18\x02 \x01(\x03\x12\x0c\n\x04\x66igi\x18\x03 \x01(\t\x12L\n\tdirection\x18\x04 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.StopOrderDirection\x12\x10\n\x08\x63urrency\x18\x05 \x01(\t\x12H\n\norder_type\x18\x06 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.StopOrderType\x12/\n\x0b\x63reate_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x61\x63tivation_date_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x65xpiration_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x05price\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x45\n\nstop_price\x18\x0b \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x16\n\x0einstrument_uid\x18\x0c \x01(\t\x12O\n\x10take_profit_type\x18\r \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.TakeProfitType\x12T\n\rtrailing_data\x18\x0e \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.StopOrder.TrailingData\x12L\n\x06status\x18\x0f \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.StopOrderStatusOption\x1a\xfc\x03\n\x0cTrailingData\x12@\n\x06indent\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bindent_type\x18\x02 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueType\x12@\n\x06spread\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bspread_type\x18\x04 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueType\x12I\n\x06status\x18\x05 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.TrailingStopStatus\x12?\n\x05price\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12>\n\x04\x65xtr\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation*w\n\x12StopOrderDirection\x12$\n STOP_ORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18STOP_ORDER_DIRECTION_BUY\x10\x01\x12\x1d\n\x19STOP_ORDER_DIRECTION_SELL\x10\x02*\xa5\x01\n\x17StopOrderExpirationType\x12*\n&STOP_ORDER_EXPIRATION_TYPE_UNSPECIFIED\x10\x00\x12/\n+STOP_ORDER_EXPIRATION_TYPE_GOOD_TILL_CANCEL\x10\x01\x12-\n)STOP_ORDER_EXPIRATION_TYPE_GOOD_TILL_DATE\x10\x02*\x90\x01\n\rStopOrderType\x12\x1f\n\x1bSTOP_ORDER_TYPE_UNSPECIFIED\x10\x00\x12\x1f\n\x1bSTOP_ORDER_TYPE_TAKE_PROFIT\x10\x01\x12\x1d\n\x19STOP_ORDER_TYPE_STOP_LOSS\x10\x02\x12\x1e\n\x1aSTOP_ORDER_TYPE_STOP_LIMIT\x10\x03*\xd2\x01\n\x15StopOrderStatusOption\x12!\n\x1dSTOP_ORDER_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15STOP_ORDER_STATUS_ALL\x10\x01\x12\x1c\n\x18STOP_ORDER_STATUS_ACTIVE\x10\x02\x12\x1e\n\x1aSTOP_ORDER_STATUS_EXECUTED\x10\x03\x12\x1e\n\x1aSTOP_ORDER_STATUS_CANCELED\x10\x04\x12\x1d\n\x19STOP_ORDER_STATUS_EXPIRED\x10\x05*w\n\x11\x45xchangeOrderType\x12#\n\x1f\x45XCHANGE_ORDER_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45XCHANGE_ORDER_TYPE_MARKET\x10\x01\x12\x1d\n\x19\x45XCHANGE_ORDER_TYPE_LIMIT\x10\x02*o\n\x0eTakeProfitType\x12 \n\x1cTAKE_PROFIT_TYPE_UNSPECIFIED\x10\x00\x12\x1c\n\x18TAKE_PROFIT_TYPE_REGULAR\x10\x01\x12\x1d\n\x19TAKE_PROFIT_TYPE_TRAILING\x10\x02*m\n\x11TrailingValueType\x12\x1e\n\x1aTRAILING_VALUE_UNSPECIFIED\x10\x00\x12\x1b\n\x17TRAILING_VALUE_ABSOLUTE\x10\x01\x12\x1b\n\x17TRAILING_VALUE_RELATIVE\x10\x02*j\n\x12TrailingStopStatus\x12\x1d\n\x19TRAILING_STOP_UNSPECIFIED\x10\x00\x12\x18\n\x14TRAILING_STOP_ACTIVE\x10\x01\x12\x1b\n\x17TRAILING_STOP_ACTIVATED\x10\x02\x32\xc0\x03\n\x11StopOrdersService\x12\x8a\x01\n\rPostStopOrder\x12;.tinkoff.public.invest.api.contract.v1.PostStopOrderRequest\x1a<.tinkoff.public.invest.api.contract.v1.PostStopOrderResponse\x12\x8a\x01\n\rGetStopOrders\x12;.tinkoff.public.invest.api.contract.v1.GetStopOrdersRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetStopOrdersResponse\x12\x90\x01\n\x0f\x43\x61ncelStopOrder\x12=.tinkoff.public.invest.api.contract.v1.CancelStopOrderRequest\x1a>.tinkoff.public.invest.api.contract.v1.CancelStopOrderResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tinkoff/invest/grpc/stoporders.proto\x12%tinkoff.public.invest.api.contract.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x33tinkoff/invest/grpc/google/api/field_behavior.proto\x1a tinkoff/invest/grpc/common.proto\"\x97\n\n\x14PostStopOrderRequest\x12\x15\n\x04\x66igi\x18\x01 \x01(\tB\x02\x18\x01H\x00\x88\x01\x01\x12\x16\n\x08quantity\x18\x02 \x01(\x03\x42\x04\xe2\x41\x01\x02\x12\x44\n\x05price\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x01\x88\x01\x01\x12I\n\nstop_price\x18\x04 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.QuotationH\x02\x88\x01\x01\x12R\n\tdirection\x18\x05 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.StopOrderDirectionB\x04\xe2\x41\x01\x02\x12\x18\n\naccount_id\x18\x06 \x01(\tB\x04\xe2\x41\x01\x02\x12]\n\x0f\x65xpiration_type\x18\x07 \x01(\x0e\x32>.tinkoff.public.invest.api.contract.v1.StopOrderExpirationTypeB\x04\xe2\x41\x01\x02\x12S\n\x0fstop_order_type\x18\x08 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.StopOrderTypeB\x04\xe2\x41\x01\x02\x12\x34\n\x0b\x65xpire_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12\x1b\n\rinstrument_id\x18\n \x01(\tB\x04\xe2\x41\x01\x02\x12U\n\x13\x65xchange_order_type\x18\x0b \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.ExchangeOrderType\x12O\n\x10take_profit_type\x18\x0c \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.TakeProfitType\x12_\n\rtrailing_data\x18\r \x01(\x0b\x32H.tinkoff.public.invest.api.contract.v1.PostStopOrderRequest.TrailingData\x12\x44\n\nprice_type\x18\x0e \x01(\x0e\x32\x30.tinkoff.public.invest.api.contract.v1.PriceType\x12\x16\n\x08order_id\x18\x0f \x01(\tB\x04\xe2\x41\x01\x02\x1a\xb0\x02\n\x0cTrailingData\x12@\n\x06indent\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bindent_type\x18\x02 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueType\x12@\n\x06spread\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bspread_type\x18\x04 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueTypeB\x07\n\x05_figiB\x08\n\x06_priceB\r\n\x0b_stop_priceB\x0e\n\x0c_expire_date\"\x9d\x01\n\x15PostStopOrderResponse\x12\x15\n\rstop_order_id\x18\x01 \x01(\t\x12\x18\n\x10order_request_id\x18\x02 \x01(\t\x12S\n\x11response_metadata\x18\xfe\x01 \x01(\x0b\x32\x37.tinkoff.public.invest.api.contract.v1.ResponseMetadata\"\xd0\x01\n\x14GetStopOrdersRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12L\n\x06status\x18\x02 \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.StopOrderStatusOption\x12(\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x02to\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"^\n\x15GetStopOrdersResponse\x12\x45\n\x0bstop_orders\x18\x01 \x03(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.StopOrder\"O\n\x16\x43\x61ncelStopOrderRequest\x12\x18\n\naccount_id\x18\x01 \x01(\tB\x04\xe2\x41\x01\x02\x12\x1b\n\rstop_order_id\x18\x02 \x01(\tB\x04\xe2\x41\x01\x02\"C\n\x17\x43\x61ncelStopOrderResponse\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xfe\n\n\tStopOrder\x12\x15\n\rstop_order_id\x18\x01 \x01(\t\x12\x16\n\x0elots_requested\x18\x02 \x01(\x03\x12\x0c\n\x04\x66igi\x18\x03 \x01(\t\x12L\n\tdirection\x18\x04 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.StopOrderDirection\x12\x10\n\x08\x63urrency\x18\x05 \x01(\t\x12H\n\norder_type\x18\x06 \x01(\x0e\x32\x34.tinkoff.public.invest.api.contract.v1.StopOrderType\x12/\n\x0b\x63reate_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x61\x63tivation_date_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x65xpiration_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x05price\x18\n \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x45\n\nstop_price\x18\x0b \x01(\x0b\x32\x31.tinkoff.public.invest.api.contract.v1.MoneyValue\x12\x16\n\x0einstrument_uid\x18\x0c \x01(\t\x12O\n\x10take_profit_type\x18\r \x01(\x0e\x32\x35.tinkoff.public.invest.api.contract.v1.TakeProfitType\x12T\n\rtrailing_data\x18\x0e \x01(\x0b\x32=.tinkoff.public.invest.api.contract.v1.StopOrder.TrailingData\x12L\n\x06status\x18\x0f \x01(\x0e\x32<.tinkoff.public.invest.api.contract.v1.StopOrderStatusOption\x12U\n\x13\x65xchange_order_type\x18\x10 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.ExchangeOrderType\x1a\xfc\x03\n\x0cTrailingData\x12@\n\x06indent\x18\x01 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bindent_type\x18\x02 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueType\x12@\n\x06spread\x18\x03 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12M\n\x0bspread_type\x18\x04 \x01(\x0e\x32\x38.tinkoff.public.invest.api.contract.v1.TrailingValueType\x12I\n\x06status\x18\x05 \x01(\x0e\x32\x39.tinkoff.public.invest.api.contract.v1.TrailingStopStatus\x12?\n\x05price\x18\x07 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation\x12>\n\x04\x65xtr\x18\x08 \x01(\x0b\x32\x30.tinkoff.public.invest.api.contract.v1.Quotation*w\n\x12StopOrderDirection\x12$\n STOP_ORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18STOP_ORDER_DIRECTION_BUY\x10\x01\x12\x1d\n\x19STOP_ORDER_DIRECTION_SELL\x10\x02*\xa5\x01\n\x17StopOrderExpirationType\x12*\n&STOP_ORDER_EXPIRATION_TYPE_UNSPECIFIED\x10\x00\x12/\n+STOP_ORDER_EXPIRATION_TYPE_GOOD_TILL_CANCEL\x10\x01\x12-\n)STOP_ORDER_EXPIRATION_TYPE_GOOD_TILL_DATE\x10\x02*\x90\x01\n\rStopOrderType\x12\x1f\n\x1bSTOP_ORDER_TYPE_UNSPECIFIED\x10\x00\x12\x1f\n\x1bSTOP_ORDER_TYPE_TAKE_PROFIT\x10\x01\x12\x1d\n\x19STOP_ORDER_TYPE_STOP_LOSS\x10\x02\x12\x1e\n\x1aSTOP_ORDER_TYPE_STOP_LIMIT\x10\x03*\xd2\x01\n\x15StopOrderStatusOption\x12!\n\x1dSTOP_ORDER_STATUS_UNSPECIFIED\x10\x00\x12\x19\n\x15STOP_ORDER_STATUS_ALL\x10\x01\x12\x1c\n\x18STOP_ORDER_STATUS_ACTIVE\x10\x02\x12\x1e\n\x1aSTOP_ORDER_STATUS_EXECUTED\x10\x03\x12\x1e\n\x1aSTOP_ORDER_STATUS_CANCELED\x10\x04\x12\x1d\n\x19STOP_ORDER_STATUS_EXPIRED\x10\x05*w\n\x11\x45xchangeOrderType\x12#\n\x1f\x45XCHANGE_ORDER_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45XCHANGE_ORDER_TYPE_MARKET\x10\x01\x12\x1d\n\x19\x45XCHANGE_ORDER_TYPE_LIMIT\x10\x02*o\n\x0eTakeProfitType\x12 \n\x1cTAKE_PROFIT_TYPE_UNSPECIFIED\x10\x00\x12\x1c\n\x18TAKE_PROFIT_TYPE_REGULAR\x10\x01\x12\x1d\n\x19TAKE_PROFIT_TYPE_TRAILING\x10\x02*m\n\x11TrailingValueType\x12\x1e\n\x1aTRAILING_VALUE_UNSPECIFIED\x10\x00\x12\x1b\n\x17TRAILING_VALUE_ABSOLUTE\x10\x01\x12\x1b\n\x17TRAILING_VALUE_RELATIVE\x10\x02*j\n\x12TrailingStopStatus\x12\x1d\n\x19TRAILING_STOP_UNSPECIFIED\x10\x00\x12\x18\n\x14TRAILING_STOP_ACTIVE\x10\x01\x12\x1b\n\x17TRAILING_STOP_ACTIVATED\x10\x02\x32\xc0\x03\n\x11StopOrdersService\x12\x8a\x01\n\rPostStopOrder\x12;.tinkoff.public.invest.api.contract.v1.PostStopOrderRequest\x1a<.tinkoff.public.invest.api.contract.v1.PostStopOrderResponse\x12\x8a\x01\n\rGetStopOrders\x12;.tinkoff.public.invest.api.contract.v1.GetStopOrdersRequest\x1a<.tinkoff.public.invest.api.contract.v1.GetStopOrdersResponse\x12\x90\x01\n\x0f\x43\x61ncelStopOrder\x12=.tinkoff.public.invest.api.contract.v1.CancelStopOrderRequest\x1a>.tinkoff.public.invest.api.contract.v1.CancelStopOrderResponseBa\n\x1cru.tinkoff.piapi.contract.v1P\x01Z\x0c./;investapi\xa2\x02\x05TIAPI\xaa\x02\x14Tinkoff.InvestApi.V1\xca\x02\x11Tinkoff\\Invest\\V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tinkoff.invest.grpc.stoporders_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034ru.tinkoff.piapi.contract.v1P\001Z\014./;investapi\242\002\005TIAPI\252\002\024Tinkoff.InvestApi.V1\312\002\021Tinkoff\\Invest\\V1'
@@ -49,30 +49,30 @@
   _POSTSTOPORDERREQUEST.fields_by_name['order_id']._serialized_options = b'\342A\001\002'
   _GETSTOPORDERSREQUEST.fields_by_name['account_id']._options = None
   _GETSTOPORDERSREQUEST.fields_by_name['account_id']._serialized_options = b'\342A\001\002'
   _CANCELSTOPORDERREQUEST.fields_by_name['account_id']._options = None
   _CANCELSTOPORDERREQUEST.fields_by_name['account_id']._serialized_options = b'\342A\001\002'
   _CANCELSTOPORDERREQUEST.fields_by_name['stop_order_id']._options = None
   _CANCELSTOPORDERREQUEST.fields_by_name['stop_order_id']._serialized_options = b'\342A\001\002'
-  _globals['_STOPORDERDIRECTION']._serialized_start=3444
-  _globals['_STOPORDERDIRECTION']._serialized_end=3563
-  _globals['_STOPORDEREXPIRATIONTYPE']._serialized_start=3566
-  _globals['_STOPORDEREXPIRATIONTYPE']._serialized_end=3731
-  _globals['_STOPORDERTYPE']._serialized_start=3734
-  _globals['_STOPORDERTYPE']._serialized_end=3878
-  _globals['_STOPORDERSTATUSOPTION']._serialized_start=3881
-  _globals['_STOPORDERSTATUSOPTION']._serialized_end=4091
-  _globals['_EXCHANGEORDERTYPE']._serialized_start=4093
-  _globals['_EXCHANGEORDERTYPE']._serialized_end=4212
-  _globals['_TAKEPROFITTYPE']._serialized_start=4214
-  _globals['_TAKEPROFITTYPE']._serialized_end=4325
-  _globals['_TRAILINGVALUETYPE']._serialized_start=4327
-  _globals['_TRAILINGVALUETYPE']._serialized_end=4436
-  _globals['_TRAILINGSTOPSTATUS']._serialized_start=4438
-  _globals['_TRAILINGSTOPSTATUS']._serialized_end=4544
+  _globals['_STOPORDERDIRECTION']._serialized_start=3531
+  _globals['_STOPORDERDIRECTION']._serialized_end=3650
+  _globals['_STOPORDEREXPIRATIONTYPE']._serialized_start=3653
+  _globals['_STOPORDEREXPIRATIONTYPE']._serialized_end=3818
+  _globals['_STOPORDERTYPE']._serialized_start=3821
+  _globals['_STOPORDERTYPE']._serialized_end=3965
+  _globals['_STOPORDERSTATUSOPTION']._serialized_start=3968
+  _globals['_STOPORDERSTATUSOPTION']._serialized_end=4178
+  _globals['_EXCHANGEORDERTYPE']._serialized_start=4180
+  _globals['_EXCHANGEORDERTYPE']._serialized_end=4299
+  _globals['_TAKEPROFITTYPE']._serialized_start=4301
+  _globals['_TAKEPROFITTYPE']._serialized_end=4412
+  _globals['_TRAILINGVALUETYPE']._serialized_start=4414
+  _globals['_TRAILINGVALUETYPE']._serialized_end=4523
+  _globals['_TRAILINGSTOPSTATUS']._serialized_start=4525
+  _globals['_TRAILINGSTOPSTATUS']._serialized_end=4631
   _globals['_POSTSTOPORDERREQUEST']._serialized_start=200
   _globals['_POSTSTOPORDERREQUEST']._serialized_end=1503
   _globals['_POSTSTOPORDERREQUEST_TRAILINGDATA']._serialized_start=1149
   _globals['_POSTSTOPORDERREQUEST_TRAILINGDATA']._serialized_end=1453
   _globals['_POSTSTOPORDERRESPONSE']._serialized_start=1506
   _globals['_POSTSTOPORDERRESPONSE']._serialized_end=1663
   _globals['_GETSTOPORDERSREQUEST']._serialized_start=1666
@@ -80,13 +80,13 @@
   _globals['_GETSTOPORDERSRESPONSE']._serialized_start=1876
   _globals['_GETSTOPORDERSRESPONSE']._serialized_end=1970
   _globals['_CANCELSTOPORDERREQUEST']._serialized_start=1972
   _globals['_CANCELSTOPORDERREQUEST']._serialized_end=2051
   _globals['_CANCELSTOPORDERRESPONSE']._serialized_start=2053
   _globals['_CANCELSTOPORDERRESPONSE']._serialized_end=2120
   _globals['_STOPORDER']._serialized_start=2123
-  _globals['_STOPORDER']._serialized_end=3442
-  _globals['_STOPORDER_TRAILINGDATA']._serialized_start=2934
-  _globals['_STOPORDER_TRAILINGDATA']._serialized_end=3442
-  _globals['_STOPORDERSSERVICE']._serialized_start=4547
-  _globals['_STOPORDERSSERVICE']._serialized_end=4995
+  _globals['_STOPORDER']._serialized_end=3529
+  _globals['_STOPORDER_TRAILINGDATA']._serialized_start=3021
+  _globals['_STOPORDER_TRAILINGDATA']._serialized_end=3529
+  _globals['_STOPORDERSSERVICE']._serialized_start=4634
+  _globals['_STOPORDERSSERVICE']._serialized_end=5082
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/stoporders_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -522,14 +522,15 @@
     EXPIRATION_TIME_FIELD_NUMBER: builtins.int
     PRICE_FIELD_NUMBER: builtins.int
     STOP_PRICE_FIELD_NUMBER: builtins.int
     INSTRUMENT_UID_FIELD_NUMBER: builtins.int
     TAKE_PROFIT_TYPE_FIELD_NUMBER: builtins.int
     TRAILING_DATA_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
+    EXCHANGE_ORDER_TYPE_FIELD_NUMBER: builtins.int
     stop_order_id: builtins.str
     """Идентификатор-идентификатор стоп-заявки"""
     lots_requested: builtins.int
     """Запрошено лотов"""
     figi: builtins.str
     """Figi-идентификатор инструмента"""
     direction: global___StopOrderDirection.ValueType
@@ -558,14 +559,16 @@
     take_profit_type: global___TakeProfitType.ValueType
     """Подтип стоп-заявки TakeProfit"""
     @property
     def trailing_data(self) -> global___StopOrder.TrailingData:
         """Параметры трейлинг-стопа"""
     status: global___StopOrderStatusOption.ValueType
     """Статус заявки"""
+    exchange_order_type: global___ExchangeOrderType.ValueType
+    """Тип дочерней биржевой заявки для тейкпрофита"""
     def __init__(
         self,
         *,
         stop_order_id: builtins.str = ...,
         lots_requested: builtins.int = ...,
         figi: builtins.str = ...,
         direction: global___StopOrderDirection.ValueType = ...,
@@ -576,12 +579,13 @@
         expiration_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         price: tinkoff.invest.grpc.common_pb2.MoneyValue | None = ...,
         stop_price: tinkoff.invest.grpc.common_pb2.MoneyValue | None = ...,
         instrument_uid: builtins.str = ...,
         take_profit_type: global___TakeProfitType.ValueType = ...,
         trailing_data: global___StopOrder.TrailingData | None = ...,
         status: global___StopOrderStatusOption.ValueType = ...,
+        exchange_order_type: global___ExchangeOrderType.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["activation_date_time", b"activation_date_time", "create_date", b"create_date", "expiration_time", b"expiration_time", "price", b"price", "stop_price", b"stop_price", "trailing_data", b"trailing_data"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["activation_date_time", b"activation_date_time", "create_date", b"create_date", "currency", b"currency", "direction", b"direction", "expiration_time", b"expiration_time", "figi", b"figi", "instrument_uid", b"instrument_uid", "lots_requested", b"lots_requested", "order_type", b"order_type", "price", b"price", "status", b"status", "stop_order_id", b"stop_order_id", "stop_price", b"stop_price", "take_profit_type", b"take_profit_type", "trailing_data", b"trailing_data"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["activation_date_time", b"activation_date_time", "create_date", b"create_date", "currency", b"currency", "direction", b"direction", "exchange_order_type", b"exchange_order_type", "expiration_time", b"expiration_time", "figi", b"figi", "instrument_uid", b"instrument_uid", "lots_requested", b"lots_requested", "order_type", b"order_type", "price", b"price", "status", b"status", "stop_order_id", b"stop_order_id", "stop_price", b"stop_price", "take_profit_type", b"take_profit_type", "trailing_data", b"trailing_data"]) -> None: ...
 
 global___StopOrder = StopOrder
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/stoporders_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/stoporders_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/users_pb2.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/users_pb2.pyi` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/grpc/users_pb2_grpc.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/grpc/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/logging.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/logging.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/async_market_data_stream_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/market_data_stream_interface.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_interface.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/market_data_stream_manager.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/market_data_stream_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/market_data_stream/stream_managers.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/market_data_stream/stream_managers.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/mock_services.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/mock_services.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/client.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/client.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/grpc_interceptor.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/aio/retry_manager.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/aio/retry_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/base_retry_manager.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/base_retry_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/client.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/client.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/grpc_interceptor.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/retrying/sync/retry_manager.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/retrying/sync/retry_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/schemas.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,14 +419,60 @@
 
 class OrderBookType(_grpc_helpers.Enum):
     ORDERBOOK_TYPE_UNSPECIFIED = 0
     ORDERBOOK_TYPE_EXCHANGE = 1
     ORDERBOOK_TYPE_DEALER = 2
 
 
+class BondType(_grpc_helpers.Enum):
+    BOND_TYPE_UNSPECIFIED = 0
+    BOND_TYPE_REPLACED = 1
+
+
+class InstrumentExchangeType(_grpc_helpers.Enum):
+    INSTRUMENT_EXCHANGE_UNSPECIFIED = 0
+    INSTRUMENT_EXCHANGE_DEALER = 1
+
+
+class TradeSourceType(_grpc_helpers.Enum):
+    TRADE_SOURCE_UNSPECIFIED = 0
+    TRADE_SOURCE_EXCHANGE = 1
+    TRADE_SOURCE_DEALER = 2
+    TRADE_SOURCE_ALL = 3
+
+
+class OrderStateStreamSubscriptionStatus(_grpc_helpers.Enum):
+    SUBSCRIPTION_STATUS_UNSPECIFIED = 0
+    SUBSCRIPTION_STATUS_OK = 1
+    SUBSCRIPTION_STATUS_ERROR = 13
+
+
+class MarkerType(_grpc_helpers.Enum):
+    MARKER_UNKNOWN = 0
+    MARKER_BROKER = 1
+    MARKER_CHAT = 2
+    MARKER_PAPER = 3
+    MARKER_MARGIN = 4
+    MARKER_TKBNM = 5
+    MARKER_SHORT = 6
+    MARKER_SPECMM = 7
+    MARKER_PO = 8
+
+
+class StatusCauseInfo(_grpc_helpers.Enum):
+    CAUSE_UNSPECIFIED = 0
+    CAUSE_CANCELLED_BY_CLIENT = 15
+    CAUSE_CANCELLED_BY_EXCHANGE = 1
+    CAUSE_CANCELLED_NOT_ENOUGH_POSITION = 2
+    CAUSE_CANCELLED_BY_CLIENT_BLOCK = 3
+    CAUSE_REJECTED_BY_BROKER = 4
+    CAUSE_REJECTED_BY_EXCHANGE = 5
+    CAUSE_CANCELLED_BY_BROKER = 6
+
+
 @dataclass(eq=False, repr=True)
 class MoneyValue(_grpc_helpers.Message):
     currency: str = _grpc_helpers.string_field(1)
     units: int = _grpc_helpers.int64_field(2)
     nano: int = _grpc_helpers.int32_field(3)
 
 
@@ -535,14 +581,17 @@
     class_code: Optional[str] = _grpc_helpers.string_field(2)
     id: str = _grpc_helpers.string_field(3)
 
 
 @dataclass(eq=False, repr=True)
 class InstrumentsRequest(_grpc_helpers.Message):
     instrument_status: Optional["InstrumentStatus"] = _grpc_helpers.enum_field(1)
+    instrument_exchange: Optional["InstrumentExchangeType"] = _grpc_helpers.enum_field(
+        2
+    )
 
 
 @dataclass(eq=False, repr=True)
 class FilterOptionsRequest(_grpc_helpers.Message):
     basic_asset_uid: Optional[str] = _grpc_helpers.string_field(1)
     basic_asset_position_uid: Optional[str] = _grpc_helpers.string_field(2)
 
@@ -775,14 +824,15 @@
     blocked_tca_flag: bool = _grpc_helpers.bool_field(54)
     subordinated_flag: bool = _grpc_helpers.bool_field(55)
     liquidity_flag: bool = _grpc_helpers.bool_field(56)
     first_1min_candle_date: datetime = _grpc_helpers.message_field(61)
     first_1day_candle_date: datetime = _grpc_helpers.message_field(62)
     risk_level: "RiskLevel" = _grpc_helpers.enum_field(63)
     brand: "BrandData" = _grpc_helpers.message_field(64)
+    bond_type: "BondType" = _grpc_helpers.message_field(65)
 
 
 @dataclass(eq=False, repr=True)
 class Currency(_grpc_helpers.Message):  # pylint:disable=too-many-instance-attributes
     figi: str = _grpc_helpers.string_field(1)
     ticker: str = _grpc_helpers.string_field(2)
     class_code: str = _grpc_helpers.string_field(3)
@@ -851,14 +901,15 @@
     sell_available_flag: bool = _grpc_helpers.bool_field(28)
     min_price_increment: "Quotation" = _grpc_helpers.message_field(29)
     api_trade_available_flag: bool = _grpc_helpers.bool_field(30)
     uid: str = _grpc_helpers.string_field(31)
     real_exchange: "RealExchange" = _grpc_helpers.message_field(32)
     position_uid: str = _grpc_helpers.string_field(33)
     asset_uid: str = _grpc_helpers.string_field(34)
+    instrument_exchange: "InstrumentExchangeType" = _grpc_helpers.message_field(35)
     for_iis_flag: bool = _grpc_helpers.bool_field(41)
     for_qual_investor_flag: bool = _grpc_helpers.bool_field(42)
     weekend_flag: bool = _grpc_helpers.bool_field(43)
     blocked_tca_flag: bool = _grpc_helpers.bool_field(44)
     liquidity_flag: bool = _grpc_helpers.bool_field(45)
     first_1min_candle_date: datetime = _grpc_helpers.message_field(56)
     first_1day_candle_date: datetime = _grpc_helpers.message_field(57)
@@ -945,14 +996,15 @@
     share_type: "ShareType" = _grpc_helpers.enum_field(30)
     min_price_increment: "Quotation" = _grpc_helpers.message_field(31)
     api_trade_available_flag: bool = _grpc_helpers.bool_field(32)
     uid: str = _grpc_helpers.string_field(33)
     real_exchange: "RealExchange" = _grpc_helpers.message_field(34)
     position_uid: str = _grpc_helpers.string_field(35)
     asset_uid: str = _grpc_helpers.string_field(36)
+    instrument_exchange: "InstrumentExchangeType" = _grpc_helpers.message_field(37)
     for_iis_flag: bool = _grpc_helpers.bool_field(46)
     for_qual_investor_flag: bool = _grpc_helpers.bool_field(47)
     weekend_flag: bool = _grpc_helpers.bool_field(48)
     blocked_tca_flag: bool = _grpc_helpers.bool_field(49)
     liquidity_flag: bool = _grpc_helpers.bool_field(50)
     first_1min_candle_date: datetime = _grpc_helpers.message_field(56)
     first_1day_candle_date: datetime = _grpc_helpers.message_field(57)
@@ -1526,14 +1578,15 @@
     order_book_type: "OrderBookType" = _grpc_helpers.message_field(7)
 
 
 @dataclass(eq=False, repr=True)
 class SubscribeTradesRequest(_grpc_helpers.Message):
     subscription_action: "SubscriptionAction" = _grpc_helpers.enum_field(1)
     instruments: List["TradeInstrument"] = _grpc_helpers.message_field(2)
+    trade_type: "TradeSourceType" = _grpc_helpers.message_field(3)
 
 
 @dataclass(eq=False, repr=True)
 class SubscribeLastPriceRequest(_grpc_helpers.Message):
     subscription_action: "SubscriptionAction" = _grpc_helpers.message_field(1)
     instruments: List["LastPriceInstrument"] = _grpc_helpers.message_field(2)
 
@@ -1567,14 +1620,15 @@
     instrument_id: str = _grpc_helpers.string_field(2)
 
 
 @dataclass(eq=False, repr=True)
 class SubscribeTradesResponse(_grpc_helpers.Message):
     tracking_id: str = _grpc_helpers.string_field(1)
     trade_subscriptions: List["TradeSubscription"] = _grpc_helpers.message_field(2)
+    trade_type: "TradeSourceType" = _grpc_helpers.message_field(3)
 
 
 @dataclass(eq=False, repr=True)
 class TradeSubscription(_grpc_helpers.Message):
     figi: str = _grpc_helpers.string_field(1)
     subscription_status: "SubscriptionStatus" = _grpc_helpers.enum_field(2)
     instrument_uid: str = _grpc_helpers.string_field(3)
@@ -1647,14 +1701,15 @@
 class Trade(_grpc_helpers.Message):
     figi: str = _grpc_helpers.string_field(1)
     direction: "TradeDirection" = _grpc_helpers.enum_field(2)
     price: "Quotation" = _grpc_helpers.message_field(3)
     quantity: int = _grpc_helpers.int64_field(4)
     time: datetime = _grpc_helpers.message_field(5)
     instrument_uid: str = _grpc_helpers.string_field(6)
+    tradeSource: TradeSourceType = _grpc_helpers.message_field(7)
 
 
 @dataclass(eq=False, repr=True)
 class TradingStatus(_grpc_helpers.Message):
     figi: str = _grpc_helpers.string_field(1)
     trading_status: "SecurityTradingStatus" = _grpc_helpers.enum_field(2)
     time: datetime = _grpc_helpers.enum_field(3)
@@ -2350,14 +2405,15 @@
     expiration_time: datetime = _grpc_helpers.message_field(9)
     price: "MoneyValue" = _grpc_helpers.message_field(10)
     stop_price: "MoneyValue" = _grpc_helpers.message_field(11)
     instrument_uid: str = _grpc_helpers.string_field(12)
     take_profit_type: "TakeProfitType" = _grpc_helpers.message_field(13)
     trailing_data: "StopOrderTrailingData" = _grpc_helpers.message_field(14)
     status: "StopOrderStatusOption" = _grpc_helpers.message_field(15)
+    exchange_order_type: "ExchangeOrderType" = _grpc_helpers.message_field(16)
 
 
 @dataclass(eq=False, repr=True)
 class StopOrderTrailingData(_grpc_helpers.Message):
     indent: "Quotation" = _grpc_helpers.message_field(1)
     indent_type: "TrailingValueType" = _grpc_helpers.message_field(2)
     spread: "Quotation" = _grpc_helpers.message_field(3)
@@ -2911,14 +2967,77 @@
     extra_bond: "ExtraBond" = _grpc_helpers.message_field(12, group="instrument_extra")
     extra_future: "ExtraFuture" = _grpc_helpers.message_field(
         13, group="instrument_extra"
     )
 
 
 @dataclass(eq=False, repr=True)
+class OrderStateStreamRequest(_grpc_helpers.Message):
+    accounts: List[str] = _grpc_helpers.message_field(1)
+    ping_delay_millis: Optional[int] = _grpc_helpers.int32_field(15)
+
+
+@dataclass(eq=False, repr=True)
+class ErrorDetail(_grpc_helpers.Message):
+    code: str = _grpc_helpers.string_field(1)
+    message: str = _grpc_helpers.string_field(3)
+
+
+@dataclass(eq=False, repr=True)
+class SubscriptionResponse(_grpc_helpers.Message):
+    tracking_id: str = _grpc_helpers.string_field(1)
+    status: OrderStateStreamSubscriptionStatus = _grpc_helpers.message_field(2)
+    stream_id: str = _grpc_helpers.message_field(4)
+    accounts: List[str] = _grpc_helpers.message_field(5)
+    error: Optional[ErrorDetail] = _grpc_helpers.message_field(7)
+
+
+@dataclass(eq=False, repr=True)
+class OrderStateStreamOrderState(_grpc_helpers.Message):
+    order_id: str = _grpc_helpers.string_field(1)
+    order_request_id: Optional[str] = _grpc_helpers.string_field(2)
+    client_code: str = _grpc_helpers.string_field(3)
+    created_at: datetime = _grpc_helpers.message_field(4)
+    execution_report_status: OrderExecutionReportStatus = _grpc_helpers.message_field(5)
+    status_info: Optional[StatusCauseInfo] = _grpc_helpers.message_field(6)
+    ticker: str = _grpc_helpers.string_field(7)
+    class_code: str = _grpc_helpers.string_field(8)
+    lot_size: int = _grpc_helpers.int32_field(9)
+    direction: OrderDirection = _grpc_helpers.message_field(10)
+    time_in_force: TimeInForceType = _grpc_helpers.message_field(11)
+    order_type: OrderType = _grpc_helpers.message_field(12)
+    account_id: str = _grpc_helpers.string_field(13)
+    initial_order_price: MoneyValue = _grpc_helpers.message_field(22)
+    order_price: MoneyValue = _grpc_helpers.message_field(23)
+    amount: Optional[MoneyValue] = _grpc_helpers.message_field(24)
+    executed_order_price: MoneyValue = _grpc_helpers.message_field(25)
+    currency: str = _grpc_helpers.string_field(26)
+    lots_requested: int = _grpc_helpers.int64_field(27)
+    lots_executed: int = _grpc_helpers.int64_field(28)
+    lots_left: int = _grpc_helpers.int64_field(29)
+    lots_cancelled: int = _grpc_helpers.int64_field(30)
+    marker: Optional[MarkerType] = _grpc_helpers.message_field(31)
+    trades: List[OrderTrade] = _grpc_helpers.message_field(33)
+    completion_time: datetime = _grpc_helpers.message_field(35)
+    exchange: str = _grpc_helpers.string_field(36)
+    instrument_uid: str = _grpc_helpers.string_field(41)
+
+
+@dataclass(eq=False, repr=True)
+class OrderStateStreamResponse(_grpc_helpers.Message):
+    order_state: "OrderStateStreamOrderState" = _grpc_helpers.message_field(
+        1, group="payload"
+    )
+    ping: "Ping" = _grpc_helpers.message_field(2, group="payload")
+    subscription: "SubscriptionResponse" = _grpc_helpers.message_field(
+        3, group="payload"
+    )
+
+
+@dataclass(eq=False, repr=True)
 class ExtraBond(_grpc_helpers.Message):
     aci_value: "MoneyValue" = _grpc_helpers.message_field(2)
     nominal_conversion_rate: "Quotation" = _grpc_helpers.message_field(3)
 
 
 @dataclass(eq=False, repr=True)
 class ExtraFuture(_grpc_helpers.Message):
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/services.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     GetTradingStatusResponse,
     GetUserTariffRequest,
     GetUserTariffResponse,
     HistoricCandle,
     IndicativesRequest,
     IndicativesResponse,
     InstrumentClosePriceRequest,
+    InstrumentExchangeType,
     InstrumentIdType,
     InstrumentRequest,
     InstrumentResponse,
     InstrumentsRequest,
     InstrumentStatus,
     InstrumentType,
     MarketDataRequest,
@@ -144,14 +145,16 @@
     OperationsRequest,
     OperationsResponse,
     OperationState,
     OptionResponse,
     OptionsResponse,
     OrderDirection,
     OrderState,
+    OrderStateStreamRequest,
+    OrderStateStreamResponse,
     OrderType,
     Page,
     PortfolioRequest,
     PortfolioResponse,
     PortfolioStreamRequest,
     PortfolioStreamResponse,
     PositionsRequest,
@@ -321,18 +324,22 @@
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "BondBy")
         return _grpc_helpers.protobuf_to_dataclass(response, BondResponse)
 
     @handle_request_error("Bonds")
     def bonds(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> BondsResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response, call = self.stub.Bonds.with_call(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "Bonds")
@@ -357,18 +364,22 @@
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "CurrencyBy")
         return _grpc_helpers.protobuf_to_dataclass(response, CurrencyResponse)
 
     @handle_request_error("Currencies")
     def currencies(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> CurrenciesResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response, call = self.stub.Currencies.with_call(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "Currencies")
@@ -393,18 +404,22 @@
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "EtfBy")
         return _grpc_helpers.protobuf_to_dataclass(response, EtfResponse)
 
     @handle_request_error("Etfs")
     def etfs(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> EtfsResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response, call = self.stub.Etfs.with_call(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "Etfs")
@@ -429,18 +444,22 @@
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "FutureBy")
         return _grpc_helpers.protobuf_to_dataclass(response, FutureResponse)
 
     @handle_request_error("Futures")
     def futures(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> FuturesResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response, call = self.stub.Futures.with_call(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "Futures")
@@ -466,18 +485,22 @@
         )
         log_request(get_tracking_id_from_call(call), "OptionBy")
         return _grpc_helpers.protobuf_to_dataclass(response, OptionResponse)
 
     @deprecated(details="Use `Client.instruments.options_by(...)` method instead")
     @handle_request_error("Options")
     def options(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> OptionsResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response, call = self.stub.Options.with_call(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "Options")
@@ -518,18 +541,22 @@
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "ShareBy")
         return _grpc_helpers.protobuf_to_dataclass(response, ShareResponse)
 
     @handle_request_error("Shares")
     def shares(
-        self, *, instrument_status: InstrumentStatus = InstrumentStatus(0)
+        self,
+        *,
+        instrument_status: InstrumentStatus = InstrumentStatus(0),
+        instrument_exchange: InstrumentExchangeType = InstrumentExchangeType(0),
     ) -> SharesResponse:
         request = InstrumentsRequest()
         request.instrument_status = instrument_status
+        request.instrument_exchange = instrument_exchange
         response, call = self.stub.Shares.with_call(
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, instruments_pb2.InstrumentsRequest()
             ),
             metadata=self.metadata,
         )
         log_request(get_tracking_id_from_call(call), "Shares")
@@ -1260,14 +1287,28 @@
             request=_grpc_helpers.dataclass_to_protobuff(
                 request, orders_pb2.TradesStreamRequest()
             ),
             metadata=self.metadata,
         ):
             yield _grpc_helpers.protobuf_to_dataclass(response, TradesStreamResponse)
 
+    @handle_request_error_gen("OrderStateStream")
+    def order_state_stream(
+        self, *, request: OrderStateStreamRequest
+    ) -> Iterable[OrderStateStreamResponse]:
+        for response in self.stub.OrderStateStream(
+            request=_grpc_helpers.dataclass_to_protobuff(
+                request, orders_pb2.OrderStateStreamRequest()
+            ),
+            metadata=self.metadata,
+        ):
+            yield _grpc_helpers.protobuf_to_dataclass(
+                response, OrderStateStreamResponse
+            )
+
 
 class OrdersService(_grpc_helpers.Service):
     _stub_factory = orders_pb2_grpc.OrdersServiceStub
 
     @handle_request_error("PostOrder")
     def post_order(
         self,
```

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/account_manager.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/account_manager.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/errors.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/errors.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/signal.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/signal_executor_base.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/signal_executor_base.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/strategy_settings_base.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_settings_base.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/strategy_supervisor.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/strategy_supervisor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/base/trader_base.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/base/trader_base.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/plotter.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/plotter.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/signal_executor.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/signal_executor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/strategy.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/strategy_state.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/strategy_state.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/supervisor.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/supervisor.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/moving_average/trader.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/moving_average/trader.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/strategies/plotting/plotter.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/strategies/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/tinkoff/invest/utils.py` & `tinkoff_investments-0.2.0b98/tinkoff/invest/utils.py`

 * *Files identical despite different names*

### Comparing `tinkoff_investments-0.2.0b97/PKG-INFO` & `tinkoff_investments-0.2.0b98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkoff-investments
-Version: 0.2.0b97
+Version: 0.2.0b98
 Summary: Tinkoff Python SDK
 Home-page: https://github.com/RussianInvestments/invest-python
 License: Apache-2.0
 Author: Tinkoff Team
 Author-email: python@tinkoff.ru
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

