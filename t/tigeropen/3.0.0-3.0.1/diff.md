# Comparing `tmp/tigeropen-3.0.0.tar.gz` & `tmp/tigeropen-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-3.0.0.tar", last modified: Thu Jun  8 06:17:55 2023, max compression
+gzip compressed data, was "tigeropen-3.0.1.tar", last modified: Wed Jun 21 08:37:36 2023, max compression
```

## Comparing `tigeropen-3.0.0.tar` & `tigeropen-3.0.1.tar`

### file list

```diff
@@ -1,208 +1,215 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.028241 tigeropen-3.0.0/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.0.0/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-08 06:17:55.028116 tigeropen-3.0.0/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.0.0/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-3.0.0/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-08 06:17:55.028282 tigeropen-3.0.0/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-3.0.0/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:54.998125 tigeropen-3.0.0/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-08 06:17:42.000000 tigeropen-3.0.0/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.000279 tigeropen-3.0.0/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.002478 tigeropen-3.0.0/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4706 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.0.0/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.004207 tigeropen-3.0.0/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-3.0.0/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-3.0.0/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.0.0/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005147 tigeropen-3.0.0/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005406 tigeropen-3.0.0/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    10346 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005535 tigeropen-3.0.0/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005663 tigeropen-3.0.0/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005927 tigeropen-3.0.0/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.006843 tigeropen-3.0.0/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.0.0/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.0.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.007446 tigeropen-3.0.0/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.008769 tigeropen-3.0.0/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-3.0.0/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.015342 tigeropen-3.0.0/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-3.0.0/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-3.0.0/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    15009 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8077 2023-06-08 06:17:42.000000 tigeropen-3.0.0/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.015596 tigeropen-3.0.0/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.017521 tigeropen-3.0.0/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    77148 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.017770 tigeropen-3.0.0/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.023294 tigeropen-3.0.0/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.0.0/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.0.0/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.0.0/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-3.0.0/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-3.0.0/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-3.0.0/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.023583 tigeropen-3.0.0/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.025094 tigeropen-3.0.0/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-3.0.0/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.025531 tigeropen-3.0.0/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.027877 tigeropen-3.0.0/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     7277 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4759 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:54.999044 tigeropen-3.0.0/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7392 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.710766 tigeropen-3.0.1/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.0.1/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-21 08:37:36.710644 tigeropen-3.0.1/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.0.1/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-3.0.1/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-21 08:37:36.710808 tigeropen-3.0.1/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-3.0.1/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.676767 tigeropen-3.0.1/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.679105 tigeropen-3.0.1/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.681128 tigeropen-3.0.1/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     5080 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.0.1/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3037 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.683318 tigeropen-3.0.1/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-3.0.1/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-3.0.1/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.0.1/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.684438 tigeropen-3.0.1/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.684798 tigeropen-3.0.1/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11145 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.684938 tigeropen-3.0.1/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.685068 tigeropen-3.0.1/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.685323 tigeropen-3.0.1/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.686249 tigeropen-3.0.1/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.0.1/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.0.1/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.686938 tigeropen-3.0.1/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.688196 tigeropen-3.0.1/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-3.0.1/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.697724 tigeropen-3.0.1/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1238 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/OptionTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2473 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/OptionTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3823 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/OptionTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-3.0.1/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1008 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3832 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3637 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4814 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1855 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      765 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2104 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1551 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/StockTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1631 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/StockTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1720 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/StockTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-3.0.1/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9068 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    17538 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9122 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    28235 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.698082 tigeropen-3.0.1/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.699907 tigeropen-3.0.1/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    77859 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.700307 tigeropen-3.0.1/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    34187 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.706461 tigeropen-3.0.1/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.0.1/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.0.1/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.0.1/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      706 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/kline_quota_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-3.0.1/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-3.0.1/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-3.0.1/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.706749 tigeropen-3.0.1/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.708066 tigeropen-3.0.1/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2704 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.708375 tigeropen-3.0.1/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.710415 tigeropen-3.0.1/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7367 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6199 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.678084 tigeropen-3.0.1/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7672 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-3.0.0/PKG-INFO` & `tigeropen-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.0.0
+Version: 3.0.1
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.0.0/README.md` & `tigeropen-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/setup.py` & `tigeropen-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/__init__.py` & `tigeropen-3.0.1/tigeropen/common/consts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -211,7 +211,22 @@
     VERTICAL = 'VERTICAL'
     STRADDLE = 'STRADDLE'
     STRANGLE = 'STRANGLE'
     CALENDAR = 'CALENDAR'
     DIAGONAL = 'DIAGONAL'
     SYNTHETIC = 'SYNTHETIC'
     CUSTOM = 'CUSTOM'
+
+class StockRankingIndicator(Enum):
+    ChangeRate = "changeRate"
+    ChangeRate5Min = "changeRate5Min"
+    TurnoverRate = "turnoverRate"
+    Amount = "amount"  # trade amount
+    Volume = "volume"  # trade volume
+    Amplitude = "amplitude"
+
+class OptionRankingIndicator(Enum):
+    BigOrder = "bigOrder"
+    Volume = "volume"
+    Amount = "amount"
+    OpenInt = "openInt"
+
```

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/filter_fields.py` & `tigeropen-3.0.1/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-3.0.1/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/params.py` & `tigeropen-3.0.1/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/push_types.py` & `tigeropen-3.0.1/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/quote_keys.py` & `tigeropen-3.0.1/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/service_types.py` & `tigeropen-3.0.1/tigeropen/common/consts/service_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 GET_QUOTE_PERMISSION = "get_quote_permission"
 TRADING_CALENDAR = "trading_calendar"
 STOCK_BROKER = "stock_broker"  # 港股股票实时经纪队列
 CAPITAL_DISTRIBUTION = "capital_distribution"  # 股票当日资金分布
 CAPITAL_FLOW = "capital_flow"  # 股票资金流向
 WARRANT_FILTER = "warrant_filter"
 WARRANT_REAL_TIME_QUOTE = "warrant_real_time_quote"
+KLINE_QUOTA = "kline_quota"  # 历史k线额度
 
 # 期权行情
 OPTION_EXPIRATION = "option_expiration"
 OPTION_CHAIN = "option_chain"
 OPTION_BRIEF = "option_brief"
 OPTION_KLINE = "option_kline"
 OPTION_TRADE_TICK = "option_trade_tick"
```

### Comparing `tigeropen-3.0.0/tigeropen/common/consts/tick_constants.py` & `tigeropen-3.0.1/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/model.py` & `tigeropen-3.0.1/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/request.py` & `tigeropen-3.0.1/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/response.py` & `tigeropen-3.0.1/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/common_utils.py` & `tigeropen-3.0.1/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/contract_utils.py` & `tigeropen-3.0.1/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/order_utils.py` & `tigeropen-3.0.1/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/price_util.py` & `tigeropen-3.0.1/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/signature_utils.py` & `tigeropen-3.0.1/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/string_utils.py` & `tigeropen-3.0.1/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/tick_util.py` & `tigeropen-3.0.1/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/common/util/web_utils.py` & `tigeropen-3.0.1/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/examples/client_config.py` & `tigeropen-3.0.1/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/examples/nasdaq100.py` & `tigeropen-3.0.1/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-3.0.1/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/examples/push_client_demo.py` & `tigeropen-3.0.1/tigeropen/examples/push_client_demo.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 @author: gaoan
 """
 import time
 # from tigeropen.common.consts import QuoteKeyType
 import pandas as pd
 
+from tigeropen.common.consts import StockRankingIndicator, OptionRankingIndicator
 from tigeropen.push.pb.AssetData_pb2 import AssetData
+from tigeropen.push.pb.OptionTopData_pb2 import OptionTopData
 from tigeropen.push.pb.OrderStatusData_pb2 import OrderStatusData
 from tigeropen.push.pb.OrderTransactionData_pb2 import OrderTransactionData
 from tigeropen.push.pb.PositionData_pb2 import PositionData
 from tigeropen.push.pb.QuoteBBOData_pb2 import QuoteBBOData
 from tigeropen.push.pb.QuoteBasicData_pb2 import QuoteBasicData
 from tigeropen.push.pb.QuoteDepthData_pb2 import QuoteDepthData
+from tigeropen.push.pb.StockTopData_pb2 import StockTopData
 from tigeropen.push.pb.TradeTickData_pb2 import TradeTickData
 from tigeropen.push.pb.trade_tick import TradeTick
 from tigeropen.push.push_client import PushClient
 from tigeropen.examples.client_config import get_client_config
 
 
 def query_subscribed_callback(data):
@@ -157,14 +160,19 @@
     """逐笔成交回调
     example:
     TradeTick<{'symbol': '00700', 'sec_type': 'STK', 'quote_level': 'hkStockQuoteLv2', 'timestamp': 1685602618145, 'ticks': [TradeTickItem<{'tick_type': '+', 'price': 316.6, 'volume': 100, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602617046, 'sn': 42055}>, TradeTickItem<{'tick_type': '-', 'price': 316.4, 'volume': 600, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602617639, 'sn': 42056}>, TradeTickItem<{'tick_type': '-', 'price': 316.4, 'volume': 200, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602617639, 'sn': 42057}>]}>
     TradeTick<{'symbol': 'CLmain', 'sec_type': 'FUT', 'quote_level': '', 'timestamp': 1685602618153, 'ticks': [TradeTickItem<{'tick_type': None, 'price': 68.7, 'volume': 1, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602616000, 'sn': 109150}>, TradeTickItem<{'tick_type': None, 'price': 68.7, 'volume': 1, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602616000, 'sn': 109151}>]}>
     """
     print(frame)
 
+def on_stock_top_changed(frame: StockTopData):
+    print(f'stock top changed: {frame}')
+
+def on_option_top_changed(frame: OptionTopData):
+    print(f'option top changed: {frame}')
 
 def on_order_changed(frame: OrderStatusData):
     """订单回调
     {"id":"28875370355884032","account":"736845","symbol":"CL","identifier":"CL2312","multiplier":1000,
     "action":"BUY","market":"US","currency":"USD","segment":"C","secType":"FUT","orderType":"LMT",
     "isLong":true,"totalQuantity":"1","filledQuantity":"1","avgFillPrice":77.76,"limitPrice":77.76,
     "status":"Filled","outsideRth":true,"name":"WTI原油2312","source":"android","commissionAndFee":4.0,
@@ -308,14 +316,20 @@
     # 订单执行明细回调
     push_client.transaction_changed = on_transaction_changed
     # 资产变动回调
     push_client.asset_changed = on_asset_changed
     # 持仓变动回调
     push_client.position_changed = on_position_changed
 
+    # 股票榜单回调
+    push_client.stock_top_changed = on_stock_top_changed
+    # 期权榜单回调
+    push_client.option_top_changed = on_option_top_changed
+
+
     # 订阅成功与否的回调
     push_client.subscribe_callback = subscribe_callback
     # 退订成功与否的回调
     push_client.unsubscribe_callback = unsubscribe_callback
 
     # 错误信息回调
     push_client.error_callback = error_callback
@@ -344,9 +358,14 @@
     # 订阅订单执行明细
     push_client.subscribe_transaction()
     # 订阅持仓变动
     push_client.subscribe_position()
     # 查询已订阅的 symbol
     push_client.query_subscribed_quote()
 
+    # 订阅股票榜单数据
+    push_client.subscribe_stock_top("HK", [StockRankingIndicator.Amount, StockRankingIndicator.ChangeRate])
+    # 订阅期权榜单数据
+    push_client.subscribe_option_top("US", [OptionRankingIndicator.Amount])
+
     time.sleep(600)
     push_client.disconnect()
```

### Comparing `tigeropen-3.0.0/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-3.0.1/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/examples/quote_client_demo.py` & `tigeropen-3.0.1/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/examples/trade_client_demo.py` & `tigeropen-3.0.1/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/request/model.py` & `tigeropen-3.0.1/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-3.0.1/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-3.0.1/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-3.0.1/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-3.0.1/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-3.0.1/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/fundamental/response/industry_response.py` & `tigeropen-3.0.1/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/__init__.py` & `tigeropen-3.0.1/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/network/connect.py` & `tigeropen-3.0.1/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/network/exception.py` & `tigeropen-3.0.1/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/network/listener.py` & `tigeropen-3.0.1/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/network/protocal.py` & `tigeropen-3.0.1/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/network/transport.py` & `tigeropen-3.0.1/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/network/utils.py` & `tigeropen-3.0.1/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/AssetData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/PositionData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/PushData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/PushData.proto`

 * *Files 26% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 import public "tigeropen/push/pb/OrderStatusData.proto";
 import public "tigeropen/push/pb/PositionData.proto";
 import public "tigeropen/push/pb/AssetData.proto";
 import public "tigeropen/push/pb/QuoteData.proto";
 import public "tigeropen/push/pb/QuoteDepthData.proto";
 import public "tigeropen/push/pb/TradeTickData.proto";
 import public "tigeropen/push/pb/OrderTransactionData.proto";
+import public "tigeropen/push/pb/StockTopData.proto";
+import public "tigeropen/push/pb/OptionTopData.proto";
 
 package tigeropen.push.pb;
 
 message PushData {
   SocketCommon.DataType dataType = 1;
   oneof body {
     QuoteData quoteData = 2;
     QuoteDepthData quoteDepthData = 3;
     TradeTickData tradeTickData = 4;
     PositionData positionData = 5;
     AssetData assetData = 6;
     OrderStatusData orderStatusData = 7;
     OrderTransactionData orderTransactionData = 8;
+    StockTopData stockTopData = 9;
+    OptionTopData optionTopData = 10;
   }
 }
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,27 +15,31 @@
 from tigeropen.push.pb import OrderStatusData_pb2 as tigeropen_dot_push_dot_pb_dot_OrderStatusData__pb2
 from tigeropen.push.pb import PositionData_pb2 as tigeropen_dot_push_dot_pb_dot_PositionData__pb2
 from tigeropen.push.pb import AssetData_pb2 as tigeropen_dot_push_dot_pb_dot_AssetData__pb2
 from tigeropen.push.pb import QuoteData_pb2 as tigeropen_dot_push_dot_pb_dot_QuoteData__pb2
 from tigeropen.push.pb import QuoteDepthData_pb2 as tigeropen_dot_push_dot_pb_dot_QuoteDepthData__pb2
 from tigeropen.push.pb import TradeTickData_pb2 as tigeropen_dot_push_dot_pb_dot_TradeTickData__pb2
 from tigeropen.push.pb import OrderTransactionData_pb2 as tigeropen_dot_push_dot_pb_dot_OrderTransactionData__pb2
+from tigeropen.push.pb import StockTopData_pb2 as tigeropen_dot_push_dot_pb_dot_StockTopData__pb2
+from tigeropen.push.pb import OptionTopData_pb2 as tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2
 
 from tigeropen.push.pb.SocketCommon_pb2 import *
 from tigeropen.push.pb.OrderStatusData_pb2 import *
 from tigeropen.push.pb.PositionData_pb2 import *
 from tigeropen.push.pb.AssetData_pb2 import *
 from tigeropen.push.pb.QuoteData_pb2 import *
 from tigeropen.push.pb.QuoteDepthData_pb2 import *
 from tigeropen.push.pb.TradeTickData_pb2 import *
 from tigeropen.push.pb.OrderTransactionData_pb2 import *
+from tigeropen.push.pb.StockTopData_pb2 import *
+from tigeropen.push.pb.OptionTopData_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tigeropen/push/pb/PushData.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\x1a\'tigeropen/push/pb/OrderStatusData.proto\x1a$tigeropen/push/pb/PositionData.proto\x1a!tigeropen/push/pb/AssetData.proto\x1a!tigeropen/push/pb/QuoteData.proto\x1a&tigeropen/push/pb/QuoteDepthData.proto\x1a%tigeropen/push/pb/TradeTickData.proto\x1a,tigeropen/push/pb/OrderTransactionData.proto\"\xed\x03\n\x08PushData\x12:\n\x08\x64\x61taType\x18\x01 \x01(\x0e\x32(.tigeropen.push.pb.SocketCommon.DataType\x12\x31\n\tquoteData\x18\x02 \x01(\x0b\x32\x1c.tigeropen.push.pb.QuoteDataH\x00\x12;\n\x0equoteDepthData\x18\x03 \x01(\x0b\x32!.tigeropen.push.pb.QuoteDepthDataH\x00\x12\x39\n\rtradeTickData\x18\x04 \x01(\x0b\x32 .tigeropen.push.pb.TradeTickDataH\x00\x12\x37\n\x0cpositionData\x18\x05 \x01(\x0b\x32\x1f.tigeropen.push.pb.PositionDataH\x00\x12\x31\n\tassetData\x18\x06 \x01(\x0b\x32\x1c.tigeropen.push.pb.AssetDataH\x00\x12=\n\x0forderStatusData\x18\x07 \x01(\x0b\x32\".tigeropen.push.pb.OrderStatusDataH\x00\x12G\n\x14orderTransactionData\x18\x08 \x01(\x0b\x32\'.tigeropen.push.pb.OrderTransactionDataH\x00\x42\x06\n\x04\x62odyP\x00P\x01P\x02P\x03P\x04P\x05P\x06P\x07\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tigeropen/push/pb/PushData.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\x1a\'tigeropen/push/pb/OrderStatusData.proto\x1a$tigeropen/push/pb/PositionData.proto\x1a!tigeropen/push/pb/AssetData.proto\x1a!tigeropen/push/pb/QuoteData.proto\x1a&tigeropen/push/pb/QuoteDepthData.proto\x1a%tigeropen/push/pb/TradeTickData.proto\x1a,tigeropen/push/pb/OrderTransactionData.proto\x1a$tigeropen/push/pb/StockTopData.proto\x1a%tigeropen/push/pb/OptionTopData.proto\"\xe1\x04\n\x08PushData\x12:\n\x08\x64\x61taType\x18\x01 \x01(\x0e\x32(.tigeropen.push.pb.SocketCommon.DataType\x12\x31\n\tquoteData\x18\x02 \x01(\x0b\x32\x1c.tigeropen.push.pb.QuoteDataH\x00\x12;\n\x0equoteDepthData\x18\x03 \x01(\x0b\x32!.tigeropen.push.pb.QuoteDepthDataH\x00\x12\x39\n\rtradeTickData\x18\x04 \x01(\x0b\x32 .tigeropen.push.pb.TradeTickDataH\x00\x12\x37\n\x0cpositionData\x18\x05 \x01(\x0b\x32\x1f.tigeropen.push.pb.PositionDataH\x00\x12\x31\n\tassetData\x18\x06 \x01(\x0b\x32\x1c.tigeropen.push.pb.AssetDataH\x00\x12=\n\x0forderStatusData\x18\x07 \x01(\x0b\x32\".tigeropen.push.pb.OrderStatusDataH\x00\x12G\n\x14orderTransactionData\x18\x08 \x01(\x0b\x32\'.tigeropen.push.pb.OrderTransactionDataH\x00\x12\x37\n\x0cstockTopData\x18\t \x01(\x0b\x32\x1f.tigeropen.push.pb.StockTopDataH\x00\x12\x39\n\roptionTopData\x18\n \x01(\x0b\x32 .tigeropen.push.pb.OptionTopDataH\x00\x42\x06\n\x04\x62odyP\x00P\x01P\x02P\x03P\x04P\x05P\x06P\x07P\x08P\tb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.PushData_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _PUSHDATA._serialized_start=368
-  _PUSHDATA._serialized_end=861
+  _PUSHDATA._serialized_start=445
+  _PUSHDATA._serialized_end=1054
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,40 +2,48 @@
 from tigeropen.push.pb import OrderStatusData_pb2 as _OrderStatusData_pb2
 from tigeropen.push.pb import PositionData_pb2 as _PositionData_pb2
 from tigeropen.push.pb import AssetData_pb2 as _AssetData_pb2
 from tigeropen.push.pb import QuoteData_pb2 as _QuoteData_pb2
 from tigeropen.push.pb import QuoteDepthData_pb2 as _QuoteDepthData_pb2
 from tigeropen.push.pb import TradeTickData_pb2 as _TradeTickData_pb2
 from tigeropen.push.pb import OrderTransactionData_pb2 as _OrderTransactionData_pb2
+from tigeropen.push.pb import StockTopData_pb2 as _StockTopData_pb2
+from tigeropen.push.pb import OptionTopData_pb2 as _OptionTopData_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
 from tigeropen.push.pb.OrderStatusData_pb2 import OrderStatusData
 from tigeropen.push.pb.PositionData_pb2 import PositionData
 from tigeropen.push.pb.AssetData_pb2 import AssetData
 from tigeropen.push.pb.QuoteData_pb2 import QuoteData
 from tigeropen.push.pb.QuoteDepthData_pb2 import QuoteDepthData
 from tigeropen.push.pb.TradeTickData_pb2 import TradeTickData
 from tigeropen.push.pb.OrderTransactionData_pb2 import OrderTransactionData
+from tigeropen.push.pb.StockTopData_pb2 import StockTopData
+from tigeropen.push.pb.OptionTopData_pb2 import OptionTopData
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PushData(_message.Message):
-    __slots__ = ["assetData", "dataType", "orderStatusData", "orderTransactionData", "positionData", "quoteData", "quoteDepthData", "tradeTickData"]
+    __slots__ = ["assetData", "dataType", "optionTopData", "orderStatusData", "orderTransactionData", "positionData", "quoteData", "quoteDepthData", "stockTopData", "tradeTickData"]
     ASSETDATA_FIELD_NUMBER: _ClassVar[int]
     DATATYPE_FIELD_NUMBER: _ClassVar[int]
+    OPTIONTOPDATA_FIELD_NUMBER: _ClassVar[int]
     ORDERSTATUSDATA_FIELD_NUMBER: _ClassVar[int]
     ORDERTRANSACTIONDATA_FIELD_NUMBER: _ClassVar[int]
     POSITIONDATA_FIELD_NUMBER: _ClassVar[int]
     QUOTEDATA_FIELD_NUMBER: _ClassVar[int]
     QUOTEDEPTHDATA_FIELD_NUMBER: _ClassVar[int]
+    STOCKTOPDATA_FIELD_NUMBER: _ClassVar[int]
     TRADETICKDATA_FIELD_NUMBER: _ClassVar[int]
     assetData: _AssetData_pb2.AssetData
     dataType: _SocketCommon_pb2.SocketCommon.DataType
+    optionTopData: _OptionTopData_pb2.OptionTopData
     orderStatusData: _OrderStatusData_pb2.OrderStatusData
     orderTransactionData: _OrderTransactionData_pb2.OrderTransactionData
     positionData: _PositionData_pb2.PositionData
     quoteData: _QuoteData_pb2.QuoteData
     quoteDepthData: _QuoteDepthData_pb2.QuoteDepthData
+    stockTopData: _StockTopData_pb2.StockTopData
     tradeTickData: _TradeTickData_pb2.TradeTickData
-    def __init__(self, dataType: _Optional[_Union[_SocketCommon_pb2.SocketCommon.DataType, str]] = ..., quoteData: _Optional[_Union[_QuoteData_pb2.QuoteData, _Mapping]] = ..., quoteDepthData: _Optional[_Union[_QuoteDepthData_pb2.QuoteDepthData, _Mapping]] = ..., tradeTickData: _Optional[_Union[_TradeTickData_pb2.TradeTickData, _Mapping]] = ..., positionData: _Optional[_Union[_PositionData_pb2.PositionData, _Mapping]] = ..., assetData: _Optional[_Union[_AssetData_pb2.AssetData, _Mapping]] = ..., orderStatusData: _Optional[_Union[_OrderStatusData_pb2.OrderStatusData, _Mapping]] = ..., orderTransactionData: _Optional[_Union[_OrderTransactionData_pb2.OrderTransactionData, _Mapping]] = ...) -> None: ...
+    def __init__(self, dataType: _Optional[_Union[_SocketCommon_pb2.SocketCommon.DataType, str]] = ..., quoteData: _Optional[_Union[_QuoteData_pb2.QuoteData, _Mapping]] = ..., quoteDepthData: _Optional[_Union[_QuoteDepthData_pb2.QuoteDepthData, _Mapping]] = ..., tradeTickData: _Optional[_Union[_TradeTickData_pb2.TradeTickData, _Mapping]] = ..., positionData: _Optional[_Union[_PositionData_pb2.PositionData, _Mapping]] = ..., assetData: _Optional[_Union[_AssetData_pb2.AssetData, _Mapping]] = ..., orderStatusData: _Optional[_Union[_OrderStatusData_pb2.OrderStatusData, _Mapping]] = ..., orderTransactionData: _Optional[_Union[_OrderTransactionData_pb2.OrderTransactionData, _Mapping]] = ..., stockTopData: _Optional[_Union[_StockTopData_pb2.StockTopData, _Mapping]] = ..., optionTopData: _Optional[_Union[_OptionTopData_pb2.OptionTopData, _Mapping]] = ...) -> None: ...
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/Request.proto` & `tigeropen-3.0.1/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,22 @@
   tigeropen_dot_push_dot_pb_dot_TradeTickData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_TradeTickData__pb2
 except AttributeError:
   tigeropen_dot_push_dot_pb_dot_TradeTickData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.TradeTickData_pb2
 try:
   tigeropen_dot_push_dot_pb_dot_OrderTransactionData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_OrderTransactionData__pb2
 except AttributeError:
   tigeropen_dot_push_dot_pb_dot_OrderTransactionData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.OrderTransactionData_pb2
+try:
+  tigeropen_dot_push_dot_pb_dot_StockTopData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_StockTopData__pb2
+except AttributeError:
+  tigeropen_dot_push_dot_pb_dot_StockTopData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.StockTopData_pb2
+try:
+  tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2
+except AttributeError:
+  tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.OptionTopData_pb2
 
 from tigeropen.push.pb.SocketCommon_pb2 import *
 from tigeropen.push.pb.PushData_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tigeropen/push/pb/Response.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\x1a tigeropen/push/pb/PushData.proto\"\xcb\x01\n\x08Response\x12\x38\n\x07\x63ommand\x18\x01 \x01(\x0e\x32\'.tigeropen.push.pb.SocketCommon.Command\x12\x0f\n\x02id\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04\x63ode\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12\x10\n\x03msg\x18\x04 \x01(\tH\x02\x88\x01\x01\x12.\n\x04\x62ody\x18\x05 \x01(\x0b\x32\x1b.tigeropen.push.pb.PushDataH\x03\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_codeB\x06\n\x04_msgB\x07\n\x05_bodyP\x00P\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from tigeropen.push.pb import OrderStatusData_pb2 as _OrderStatusData_pb2
 from tigeropen.push.pb import PositionData_pb2 as _PositionData_pb2
 from tigeropen.push.pb import AssetData_pb2 as _AssetData_pb2
 from tigeropen.push.pb import QuoteData_pb2 as _QuoteData_pb2
 from tigeropen.push.pb import QuoteDepthData_pb2 as _QuoteDepthData_pb2
 from tigeropen.push.pb import TradeTickData_pb2 as _TradeTickData_pb2
 from tigeropen.push.pb import OrderTransactionData_pb2 as _OrderTransactionData_pb2
+from tigeropen.push.pb import StockTopData_pb2 as _StockTopData_pb2
+from tigeropen.push.pb import OptionTopData_pb2 as _OptionTopData_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
 from tigeropen.push.pb.PushData_pb2 import PushData
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-3.0.1/tigeropen/push/pb/SocketCommon.proto`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     Future = 3;
     QuoteDepth = 4;
     TradeTick = 5;
     Asset = 6;
     Position = 7;
     OrderStatus = 8;
     OrderTransaction = 9;
+    StockTop = 10;
+    OptionTop = 11;
   }
 
   enum QuoteType {
     None = 0;
     BASIC = 1; // basic quote data
     BBO = 2; // best bid and offer(include fields: askSize,askPrice,bidSize,bizePrice)
     ALL = 3; // include BASIC AND BBO
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tigeropen/push/pb/SocketCommon.proto\x12\x11tigeropen.push.pb\"\xf4\x02\n\x0cSocketCommon\"\x93\x01\n\x07\x43ommand\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07\x43ONNECT\x10\x01\x12\r\n\tCONNECTED\x10\x02\x12\x08\n\x04SEND\x10\x03\x12\r\n\tSUBSCRIBE\x10\x04\x12\x0f\n\x0bUNSUBSCRIBE\x10\x05\x12\x0e\n\nDISCONNECT\x10\x06\x12\x0b\n\x07MESSAGE\x10\x07\x12\r\n\tHEARTBEAT\x10\x08\x12\t\n\x05\x45RROR\x10\t\"\x99\x01\n\x08\x44\x61taType\x12\x0b\n\x07Unknown\x10\x00\x12\t\n\x05Quote\x10\x01\x12\n\n\x06Option\x10\x02\x12\n\n\x06\x46uture\x10\x03\x12\x0e\n\nQuoteDepth\x10\x04\x12\r\n\tTradeTick\x10\x05\x12\t\n\x05\x41sset\x10\x06\x12\x0c\n\x08Position\x10\x07\x12\x0f\n\x0bOrderStatus\x10\x08\x12\x14\n\x10OrderTransaction\x10\t\"2\n\tQuoteType\x12\x08\n\x04None\x10\x00\x12\t\n\x05\x42\x41SIC\x10\x01\x12\x07\n\x03\x42\x42O\x10\x02\x12\x07\n\x03\x41LL\x10\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tigeropen/push/pb/SocketCommon.proto\x12\x11tigeropen.push.pb\"\x91\x03\n\x0cSocketCommon\"\x93\x01\n\x07\x43ommand\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07\x43ONNECT\x10\x01\x12\r\n\tCONNECTED\x10\x02\x12\x08\n\x04SEND\x10\x03\x12\r\n\tSUBSCRIBE\x10\x04\x12\x0f\n\x0bUNSUBSCRIBE\x10\x05\x12\x0e\n\nDISCONNECT\x10\x06\x12\x0b\n\x07MESSAGE\x10\x07\x12\r\n\tHEARTBEAT\x10\x08\x12\t\n\x05\x45RROR\x10\t\"\xb6\x01\n\x08\x44\x61taType\x12\x0b\n\x07Unknown\x10\x00\x12\t\n\x05Quote\x10\x01\x12\n\n\x06Option\x10\x02\x12\n\n\x06\x46uture\x10\x03\x12\x0e\n\nQuoteDepth\x10\x04\x12\r\n\tTradeTick\x10\x05\x12\t\n\x05\x41sset\x10\x06\x12\x0c\n\x08Position\x10\x07\x12\x0f\n\x0bOrderStatus\x10\x08\x12\x14\n\x10OrderTransaction\x10\t\x12\x0c\n\x08StockTop\x10\n\x12\r\n\tOptionTop\x10\x0b\"2\n\tQuoteType\x12\x08\n\x04None\x10\x00\x12\t\n\x05\x42\x41SIC\x10\x01\x12\x07\n\x03\x42\x42O\x10\x02\x12\x07\n\x03\x41LL\x10\x03\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.SocketCommon_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _SOCKETCOMMON._serialized_start=60
-  _SOCKETCOMMON._serialized_end=432
+  _SOCKETCOMMON._serialized_end=461
   _SOCKETCOMMON_COMMAND._serialized_start=77
   _SOCKETCOMMON_COMMAND._serialized_end=224
   _SOCKETCOMMON_DATATYPE._serialized_start=227
-  _SOCKETCOMMON_DATATYPE._serialized_end=380
-  _SOCKETCOMMON_QUOTETYPE._serialized_start=382
-  _SOCKETCOMMON_QUOTETYPE._serialized_end=432
+  _SOCKETCOMMON_DATATYPE._serialized_end=409
+  _SOCKETCOMMON_QUOTETYPE._serialized_start=411
+  _SOCKETCOMMON_QUOTETYPE._serialized_end=461
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,21 @@
     DISCONNECT: SocketCommon.Command
     ERROR: SocketCommon.Command
     Future: SocketCommon.DataType
     HEARTBEAT: SocketCommon.Command
     MESSAGE: SocketCommon.Command
     None: SocketCommon.QuoteType
     Option: SocketCommon.DataType
+    OptionTop: SocketCommon.DataType
     OrderStatus: SocketCommon.DataType
     OrderTransaction: SocketCommon.DataType
     Position: SocketCommon.DataType
     Quote: SocketCommon.DataType
     QuoteDepth: SocketCommon.DataType
     SEND: SocketCommon.Command
     SUBSCRIBE: SocketCommon.Command
+    StockTop: SocketCommon.DataType
     TradeTick: SocketCommon.DataType
     UNKNOWN: SocketCommon.Command
     UNSUBSCRIBE: SocketCommon.Command
     Unknown: SocketCommon.DataType
     def __init__(self) -> None: ...
```

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-3.0.1/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/trade_tick.py` & `tigeropen-3.0.1/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/push/pb/util.py` & `tigeropen-3.0.1/tigeropen/push/pb/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,20 +95,20 @@
     def build_subscribe_query_message(cls):
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.SEND
         request.id = cls.increment()
         return request
 
     @classmethod
-    def build_subscribe_quote_message(cls, symbols, data_type=SocketCommon_pb2.SocketCommon.Quote):
-        return cls.build_quote_message(data_type, symbols, SocketCommon_pb2.SocketCommon.SUBSCRIBE)
+    def build_subscribe_quote_message(cls, symbols, data_type=SocketCommon_pb2.SocketCommon.Quote, market=None):
+        return cls.build_quote_message(data_type, symbols, SocketCommon_pb2.SocketCommon.SUBSCRIBE, market=market)
 
     @classmethod
-    def build_unsubscribe_quote_message(cls, symbols, data_type=SocketCommon_pb2.SocketCommon.Quote):
-        return cls.build_quote_message(data_type, symbols, SocketCommon_pb2.SocketCommon.UNSUBSCRIBE)
+    def build_unsubscribe_quote_message(cls, symbols, data_type=SocketCommon_pb2.SocketCommon.Quote, market=None):
+        return cls.build_quote_message(data_type, symbols, SocketCommon_pb2.SocketCommon.UNSUBSCRIBE, market=market)
 
     @classmethod
     def build_subscribe_tick_quote_message(cls, symbols):
         return cls.build_quote_message(SocketCommon_pb2.SocketCommon.TradeTick, symbols, SocketCommon_pb2.SocketCommon.SUBSCRIBE)
 
     @classmethod
     def build_unsubscribe_tick_quote_message(cls, symbols):
@@ -127,23 +127,25 @@
         return cls.build_market_quote_message(market, SocketCommon_pb2.SocketCommon.SUBSCRIBE)
 
     @classmethod
     def build_unsubscribe_market_message(cls, market):
         return cls.build_market_quote_message(market, SocketCommon_pb2.SocketCommon.UNSUBSCRIBE)
 
     @classmethod
-    def build_quote_message(cls, data_type, symbols, command):
+    def build_quote_message(cls, data_type, symbols, command, market=None):
         request = Request_pb2.Request()
         request.command = command
         request.id = cls.increment()
 
         sub = Request_pb2.Request.Subscribe()
         sub.dataType = data_type
         if symbols:
             sub.symbols = ','.join(symbols) if isinstance(symbols, list) else symbols
+        if market:
+            sub.market = market
         request.subscribe.CopyFrom(sub)
         return request
 
     @classmethod
     def build_market_quote_message(cls, market, command):
         request = Request_pb2.Request()
         request.command = command
```

### Comparing `tigeropen-3.0.0/tigeropen/push/protobuf_push_client.py` & `tigeropen-3.0.1/tigeropen/push/protobuf_push_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # @Date    : 2023/2/17
 # @Author  : sukai
 import logging
 import sys
 from itertools import accumulate, zip_longest
 
 from tigeropen.common.consts.push_types import ResponseType
-from tigeropen.common.util.signature_utils import sign_with_rsa, read_private_key
+from tigeropen.common.util.common_utils import get_enum_value
+from tigeropen.common.util.signature_utils import sign_with_rsa
 from tigeropen.common.util.tick_util import get_part_code, get_part_code_name, get_trade_condition_map, \
     get_trade_condition
 from tigeropen.push import _patch_ssl
 from tigeropen.push.network.connect import PushConnection
 from tigeropen.push.network.exception import ConnectFailedException
 from tigeropen.push.network.listener import ConnectionListener
 from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
@@ -41,14 +42,16 @@
         self.quote_bbo_changed = None
         self.quote_depth_changed = None
         self.tick_changed = None
         self.asset_changed = None
         self.position_changed = None
         self.order_changed = None
         self.transaction_changed = None
+        self.stock_top_changed = None
+        self.option_top_changed = None
         self.connect_callback = None
         self.disconnect_callback = None
         self.subscribe_callback = None
         self.unsubscribe_callback = None
         self.error_callback = None
         self._connection_timeout = connection_timeout
         self._heartbeats = heartbeats
@@ -152,14 +155,20 @@
                     self.transaction_changed(frame.body.orderTransactionData)
             elif frame.body.dataType == SocketCommon.DataType.Asset:
                 if self.asset_changed:
                     self.asset_changed(frame.body.assetData)
             elif frame.body.dataType == SocketCommon.DataType.Position:
                 if self.position_changed:
                     self.position_changed(frame.body.positionData)
+            elif frame.body.dataType == SocketCommon.DataType.StockTop:
+                if self.stock_top_changed:
+                    self.stock_top_changed(frame.body.stockTopData)
+            elif frame.body.dataType == SocketCommon.DataType.OptionTop:
+                if self.option_top_changed:
+                    self.option_top_changed(frame.body.optionTopData)
             else:
                 self.logger.warning(f'unhandled frame: {frame}')
 
     def subscribe_asset(self, account=None):
         """
         订阅账户资产更新
         :return:
@@ -264,14 +273,64 @@
         订阅期货行情
         :param symbols: symbol列表
         :return:
         """
         req = ProtoMessageUtil.build_subscribe_quote_message(symbols, data_type=SocketCommon.Future)
         self._connection.send_frame(req)
 
+    def subscribe_stock_top(self, market, indicators):
+        """
+        订阅股票榜单行情
+        :param market: 市场
+        :param indicators: indicator列表
+        :return:
+        """
+        indicator_names = []
+        if indicators:
+            indicator_names = [get_enum_value(indicator) for indicator in indicators]
+        req = ProtoMessageUtil.build_subscribe_quote_message(symbols=indicator_names, data_type=SocketCommon.StockTop,
+                                                             market=market)
+        self._connection.send_frame(req)
+
+    def unsubscribe_stock_top(self, market, indicators):
+        """
+        退订股票榜单行情
+        :param market: 市场
+        :param indicators: indicator列表
+        :return:
+        """
+        indicator_names = []
+        if indicators:
+            indicator_names = [get_enum_value(indicator) for indicator in indicators]
+        req = ProtoMessageUtil.build_unsubscribe_quote_message(symbols=indicator_names, data_type=SocketCommon.StockTop,
+                                                               market=market)
+        self._connection.send_frame(req)
+
+    def subscribe_option_top(self, market, indicators):
+        """
+        订阅期权榜单行情
+        :param market: 市场
+        :param indicators: indicator列表
+        :return:
+        """
+        req = ProtoMessageUtil.build_subscribe_quote_message(symbols=indicators, data_type=SocketCommon.OptionTop,
+                                                             market=market)
+        self._connection.send_frame(req)
+
+    def unsubscribe_option_top(self, market, indicators):
+        """
+        退订期权榜单行情
+        :param market: 市场
+        :param indicators: indicator列表
+        :return:
+        """
+        req = ProtoMessageUtil.build_unsubscribe_quote_message(symbols=indicators, data_type=SocketCommon.OptionTop,
+                                                               market=market)
+        self._connection.send_frame(req)
+
     def query_subscribed_quote(self):
         """
         查询已订阅行情的合约
         :return:
         """
         req = ProtoMessageUtil.build_subscribe_query_message()
         self._connection.send_frame(req)
```

### Comparing `tigeropen-3.0.0/tigeropen/push/push_client.py` & `tigeropen-3.0.1/tigeropen/push/push_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/30
 
 @author: gaoan
 """
-
+from tigeropen.common.util.common_utils import get_enum_value
 from tigeropen.push.protobuf_push_client import ProtobufPushClient
 from tigeropen.push.stomp_push_client import StompPushClient
 
 
 class PushClient:
     def __init__(self, host, port, use_ssl=True, connection_timeout=120, heartbeats=(30 * 1000, 30 * 1000),
                  use_protobuf=True):
@@ -75,14 +75,30 @@
         return self.client.tick_changed
 
     @tick_changed.setter
     def tick_changed(self, value):
         self.client.tick_changed = value
 
     @property
+    def stock_top_changed(self):
+        return self.client.stock_top_changed
+
+    @stock_top_changed.setter
+    def stock_top_changed(self, value):
+        self.client.stock_top_changed = value
+
+    @property
+    def option_top_changed(self):
+        return self.client.option_top_changed
+
+    @option_top_changed.setter
+    def option_top_changed(self, value):
+        self.client.option_top_changed = value
+
+    @property
     def asset_changed(self):
         return self.client.asset_changed
 
     @asset_changed.setter
     def asset_changed(self, value):
         self.client.asset_changed = value
 
@@ -293,8 +309,19 @@
         """
         self.client.unsubscribe_depth_quote(symbols=symbols)
 
     def subscribe_market(self, market):
         self.client.subscribe_market(market)
 
     def unsubscribe_market(self, market):
-        self.client.unsubscribe_market(market)
+        self.client.unsubscribe_market(market)
+
+    def subscribe_stock_top(self, market, indicators=None):
+        self.client.subscribe_stock_top(get_enum_value(market), indicators)
+
+    def unsubscribe_stock_top(self, market, indicators=None):
+        self.client.unsubscribe_stock_top(get_enum_value(market), indicators)
+    def subscribe_option_top(self, market, indicators=None):
+        self.client.subscribe_option_top(get_enum_value(market), indicators)
+
+    def unsubscribe_option_top(self, market, indicators=None):
+        self.client.unsubscribe_option_top(get_enum_value(market), indicators)
```

### Comparing `tigeropen-3.0.0/tigeropen/push/stomp_push_client.py` & `tigeropen-3.0.1/tigeropen/push/stomp_push_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 
         self.subscribed_symbols = None
         self.query_subscribed_callback = None
         self.quote_changed = None
         self.quote_bbo_changed = None
         self.quote_depth_changed = None
         self.tick_changed = None
+        self.stock_top_changed = None
+        self.option_top_changed = None
         self.asset_changed = None
         self.position_changed = None
         self.order_changed = None
         self.transaction_changed = None
         self.connect_callback = None
         self.disconnect_callback = None
         self.subscribe_callback = None
@@ -461,14 +463,26 @@
 
     def subscribe_market(self, market):
         raise NotImplementedError('Only protobuf support subscribe market')
 
     def unsubscribe_market(self, market):
         raise NotImplementedError('Only protobuf support unsubscribe market')
 
+    def subscribe_stock_top(self, market, indicators):
+        raise NotImplementedError('Only protobuf support subscribe stock top')
+
+    def unsubscribe_stock_top(self, market, indicators):
+        raise NotImplementedError('Only protobuf support unsubscribe stock top')
+
+    def subscribe_option_top(self, market, indicators):
+        raise NotImplementedError('Only protobuf support subscribe option top')
+
+    def unsubscribe_option_top(self, market, indicators):
+        raise NotImplementedError('Only protobuf support unsubscribe option top')
+
     def _handle_trade_subscribe(self, destination, subscription, account=None, extra_headers=None):
         if extra_headers is None:
             extra_headers = dict()
         if account is not None:
             extra_headers['account'] = account
         return self._handle_subscribe(destination=destination, subscription=subscription, extra_headers=extra_headers)
```

### Comparing `tigeropen-3.0.0/tigeropen/quote/domain/filter.py` & `tigeropen-3.0.1/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/domain/quote_brief.py` & `tigeropen-3.0.1/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/domain/stock_broker.py` & `tigeropen-3.0.1/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/quote_client.py` & `tigeropen-3.0.1/tigeropen/quote/quote_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 from tigeropen.common.consts import Market, QuoteRight, BarPeriod, OPEN_API_SERVICE_VERSION_V3, \
     OPEN_API_SERVICE_VERSION_V1
 from tigeropen.common.consts import THREAD_LOCAL, SecurityType, CorporateActionType, IndustryLevel
 from tigeropen.common.consts.filter_fields import FieldBelongType
 from tigeropen.common.consts.service_types import GRAB_QUOTE_PERMISSION, QUOTE_DELAY, GET_QUOTE_PERMISSION, \
     HISTORY_TIMELINE, FUTURE_CONTRACT_BY_CONTRACT_CODE, TRADING_CALENDAR, FUTURE_CONTRACTS, MARKET_SCANNER, \
-    STOCK_BROKER, CAPITAL_FLOW, CAPITAL_DISTRIBUTION, WARRANT_REAL_TIME_QUOTE, WARRANT_FILTER, MARKET_SCANNER_TAGS
+    STOCK_BROKER, CAPITAL_FLOW, CAPITAL_DISTRIBUTION, WARRANT_REAL_TIME_QUOTE, WARRANT_FILTER, MARKET_SCANNER_TAGS, \
+    KLINE_QUOTA
 from tigeropen.common.consts.service_types import MARKET_STATE, ALL_SYMBOLS, ALL_SYMBOL_NAMES, BRIEF, \
     TIMELINE, KLINE, TRADE_TICK, OPTION_EXPIRATION, OPTION_CHAIN, FUTURE_EXCHANGE, OPTION_BRIEF, \
     OPTION_KLINE, OPTION_TRADE_TICK, FUTURE_KLINE, FUTURE_TICK, FUTURE_CONTRACT_BY_EXCHANGE_CODE, \
     FUTURE_TRADING_DATE, QUOTE_SHORTABLE_STOCKS, FUTURE_REAL_TIME_QUOTE, \
     FUTURE_CURRENT_CONTRACT, QUOTE_REAL_TIME, QUOTE_STOCK_TRADE, FINANCIAL_DAILY, FINANCIAL_REPORT, CORPORATE_ACTION, \
     QUOTE_DEPTH, INDUSTRY_LIST, INDUSTRY_STOCKS, STOCK_INDUSTRY, STOCK_DETAIL
 from tigeropen.common.exceptions import ApiException
@@ -36,23 +37,24 @@
 from tigeropen.fundamental.response.financial_report_response import FinancialReportResponse
 from tigeropen.fundamental.response.industry_response import IndustryListResponse, IndustryStocksResponse, \
     StockIndustryResponse
 from tigeropen.quote.domain.filter import OptionFilter
 from tigeropen.quote.request.model import MarketParams, MultipleQuoteParams, MultipleContractParams, \
     FutureQuoteParams, FutureExchangeParams, FutureContractParams, FutureTradingTimeParams, SingleContractParams, \
     SingleOptionQuoteParams, DepthQuoteParams, OptionChainParams, TradingCalendarParams, MarketScannerParams, \
-    StockBrokerParams, CapitalParams, WarrantFilterParams
+    StockBrokerParams, CapitalParams, WarrantFilterParams, KlineQuotaParams
 from tigeropen.quote.response.capital_distribution_response import CapitalDistributionResponse
 from tigeropen.quote.response.capital_flow_response import CapitalFlowResponse
 from tigeropen.quote.response.future_briefs_response import FutureBriefsResponse
 from tigeropen.quote.response.future_contract_response import FutureContractResponse
 from tigeropen.quote.response.future_exchange_response import FutureExchangeResponse
 from tigeropen.quote.response.future_quote_bar_response import FutureQuoteBarResponse
 from tigeropen.quote.response.future_quote_ticks_response import FutureTradeTickResponse
 from tigeropen.quote.response.future_trading_times_response import FutureTradingTimesResponse
+from tigeropen.quote.response.kline_quota_response import KlineQuotaResponse
 from tigeropen.quote.response.market_status_response import MarketStatusResponse
 from tigeropen.quote.response.option_briefs_response import OptionBriefsResponse
 from tigeropen.quote.response.option_chains_response import OptionChainsResponse
 from tigeropen.quote.response.option_expirations_response import OptionExpirationsResponse
 from tigeropen.quote.response.option_quote_bar_response import OptionQuoteBarResponse
 from tigeropen.quote.response.option_quote_ticks_response import OptionTradeTickResponse
 from tigeropen.quote.response.quote_bar_response import QuoteBarResponse
@@ -1629,8 +1631,22 @@
         response_content = self.__fetch_data(request)
         if response_content:
             response = WarrantFilterResponse()
             response.parse_response_content(response_content)
             if response.is_success():
                 return response.result
             else:
-                raise ApiException(response.code, response.message)
+                raise ApiException(response.code, response.message)
+
+    def get_kline_quota(self, with_details=False):
+        params = KlineQuotaParams()
+        params.lang = get_enum_value(self._lang)
+        params.with_details = with_details
+        request = OpenApiRequest(KLINE_QUOTA, biz_model=params)
+        response_content = self.__fetch_data(request)
+        if response_content:
+            response = KlineQuotaResponse()
+            response.parse_response_content(response_content)
+            if response.is_success():
+                return response.result
+            else:
+                raise ApiException(response.code, response.message)
```

### Comparing `tigeropen-3.0.0/tigeropen/quote/request/model.py` & `tigeropen-3.0.1/tigeropen/quote/request/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1348,8 +1348,27 @@
             params['volume'] = self.convert_range_param(self.volume)
         if self.premium:
             params['premium'] = self.convert_range_param(self.premium)
         if self.outstanding_ratio:
             params['outstanding_ratio'] = self.convert_range_param(self.outstanding_ratio)
         if self.implied_volatility:
             params['implied_volatility'] = self.convert_range_param(self.implied_volatility)
-        return params
+        return params
+
+class KlineQuotaParams(BaseParams):
+    def __init__(self):
+        super().__init__()
+        self._with_details = False
+
+    @property
+    def with_details(self):
+        return self._with_details
+
+    @with_details.setter
+    def with_details(self, value):
+        self._with_details = value
+
+    def to_openapi_dict(self):
+        params = super().to_openapi_dict()
+        if self.with_details is not None:
+            params['with_details'] = self.with_details
+        return params
```

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/future_contract_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/market_status_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/option_chains_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/stock_details_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/symbols_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-3.0.1/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/tiger_open_client.py` & `tigeropen-3.0.1/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/tiger_open_config.py` & `tigeropen-3.0.1/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/domain/account.py` & `tigeropen-3.0.1/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/domain/contract.py` & `tigeropen-3.0.1/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/domain/order.py` & `tigeropen-3.0.1/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/domain/position.py` & `tigeropen-3.0.1/tigeropen/trade/domain/position.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,40 @@
 
 @author: gaoan
 """
 
 
 class Position:
     def __init__(self, account, contract, quantity=0, average_cost=None, market_price=None, market_value=None,
-                 realized_pnl=None, unrealized_pnl=None, saleable=None, position_scale=None):
+                 realized_pnl=None, unrealized_pnl=None, saleable=None, position_scale=None, **kwargs):
         """
         - account: 对应的账户ID
         - contract: 合约对象
         - quantity: 合约数量
         - average_cost: 含佣金的平均成本
         - market_price: 市价
         - market_value: 市值
         - realized_pnl: 已实现盈亏
         - unrealized_pnl: 未实现盈亏
         """
         self.account = account
         self.contract = contract
         self.quantity = quantity
         self.average_cost = average_cost
+        self.average_cost_by_average = kwargs.get('average_cost_by_average', None)
         self.market_price = market_price
         self.market_value = market_value
         self.realized_pnl = realized_pnl
+        self.realized_pnl_by_average = kwargs.get('realized_pnl_by_average', None)
         self.unrealized_pnl = unrealized_pnl
+        self.unrealized_pnl_by_average = kwargs.get('unrealized_pnl_by_average', None)
         self.saleable = saleable
         self.position_scale = position_scale
+        self.unrealized_pnl_percent = kwargs.get('unrealized_pnl_percent', None)
+        self.unrealized_pnl_percent_by_average = kwargs.get('unrealized_pnl_percent_by_average', None)
     
     def __repr__(self):
         template = "contract: {contract}, quantity: {quantity}, average_cost: {average_cost}, " \
                    "market_price: {market_price}"
         return template.format(
             contract=self.contract,
             quantity=self.quantity,
```

### Comparing `tigeropen-3.0.0/tigeropen/trade/domain/prime_account.py` & `tigeropen-3.0.1/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/request/model.py` & `tigeropen-3.0.1/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/__init__.py` & `tigeropen-3.0.1/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/account_profile_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/assets_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/contracts_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/forex_order_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/order_id_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/order_preview_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/orders_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/orders_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,19 @@
         origin_symbol = contract_fields.get('origin_symbol')
         local_symbol = contract_fields.get('local_symbol')
         expiry = contract_fields.get('expiry')
         strike = contract_fields.get('strike')
         put_call = contract_fields.get('right')
         multiplier = contract_fields.get('multiplier')
         identifier = contract_fields.get('identifier')
+        market = contract_fields.get('market')
         contract = Contract(symbol, currency, contract_id=contract_id, sec_type=sec_type, exchange=exchange,
                             origin_symbol=origin_symbol, local_symbol=local_symbol, expiry=expiry,
-                            strike=strike, put_call=put_call, multiplier=multiplier, identifier=identifier)
+                            strike=strike, put_call=put_call, multiplier=multiplier, identifier=identifier,
+                            market=market)
         account = order_fields.get('account')
         action = order_fields.get('action')
         order_type = order_fields.get('order_type')
         quantity = order_fields.get('quantity')
         limit_price = order_fields.get('limit_price')
         aux_price = order_fields.get('aux_price')
         trail_stop_price = order_fields.get('trail_stop_price')
```

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/response/transactions_response.py` & `tigeropen-3.0.1/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen/trade/trade_client.py` & `tigeropen-3.0.1/tigeropen/trade/trade_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.0/tigeropen.egg-info/PKG-INFO` & `tigeropen-3.0.1/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.0.0
+Version: 3.0.1
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.0.0/tigeropen.egg-info/SOURCES.txt` & `tigeropen-3.0.1/tigeropen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 tigeropen/push/network/listener.py
 tigeropen/push/network/protocal.py
 tigeropen/push/network/transport.py
 tigeropen/push/network/utils.py
 tigeropen/push/pb/AssetData.proto
 tigeropen/push/pb/AssetData_pb2.py
 tigeropen/push/pb/AssetData_pb2.pyi
+tigeropen/push/pb/OptionTopData.proto
+tigeropen/push/pb/OptionTopData_pb2.py
+tigeropen/push/pb/OptionTopData_pb2.pyi
 tigeropen/push/pb/OrderStatusData.proto
 tigeropen/push/pb/OrderStatusData_pb2.py
 tigeropen/push/pb/OrderStatusData_pb2.pyi
 tigeropen/push/pb/OrderTransactionData.proto
 tigeropen/push/pb/OrderTransactionData_pb2.py
 tigeropen/push/pb/OrderTransactionData_pb2.pyi
 tigeropen/push/pb/PositionData.proto
@@ -98,14 +101,17 @@
 tigeropen/push/pb/Request_pb2.pyi
 tigeropen/push/pb/Response.proto
 tigeropen/push/pb/Response_pb2.py
 tigeropen/push/pb/Response_pb2.pyi
 tigeropen/push/pb/SocketCommon.proto
 tigeropen/push/pb/SocketCommon_pb2.py
 tigeropen/push/pb/SocketCommon_pb2.pyi
+tigeropen/push/pb/StockTopData.proto
+tigeropen/push/pb/StockTopData_pb2.py
+tigeropen/push/pb/StockTopData_pb2.pyi
 tigeropen/push/pb/TradeTickData.proto
 tigeropen/push/pb/TradeTickData_pb2.py
 tigeropen/push/pb/TradeTickData_pb2.pyi
 tigeropen/push/pb/__init__.py
 tigeropen/push/pb/readme.md
 tigeropen/push/pb/trade_tick.py
 tigeropen/push/pb/util.py
@@ -127,14 +133,15 @@
 tigeropen/quote/response/capital_flow_response.py
 tigeropen/quote/response/future_briefs_response.py
 tigeropen/quote/response/future_contract_response.py
 tigeropen/quote/response/future_exchange_response.py
 tigeropen/quote/response/future_quote_bar_response.py
 tigeropen/quote/response/future_quote_ticks_response.py
 tigeropen/quote/response/future_trading_times_response.py
+tigeropen/quote/response/kline_quota_response.py
 tigeropen/quote/response/market_scanner_response.py
 tigeropen/quote/response/market_status_response.py
 tigeropen/quote/response/option_briefs_response.py
 tigeropen/quote/response/option_chains_response.py
 tigeropen/quote/response/option_expirations_response.py
 tigeropen/quote/response/option_quote_bar_response.py
 tigeropen/quote/response/option_quote_ticks_response.py
```

