# Comparing `tmp/frontrunner-sdk-0.3.0.tar.gz` & `tmp/frontrunner-sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontrunner-sdk-0.3.0.tar", last modified: Mon Jul 31 19:13:05 2023, max compression
+gzip compressed data, was "frontrunner-sdk-0.4.0.tar", last modified: Wed Aug  2 19:38:20 2023, max compression
```

## Comparing `frontrunner-sdk-0.3.0.tar` & `frontrunner-sdk-0.4.0.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.700608 frontrunner-sdk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-31 19:13:05.700608 frontrunner-sdk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.692608 frontrunner-sdk-0.3.0/frontrunner_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.692608 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/denom_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/injective_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/injective_faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/injective_light_client_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/clients/openapi_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.692608 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/find_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_leagues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_sport_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_sport_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_sports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/cancel_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/create_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/create_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_account_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_order_books.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/config/chained.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/config/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/config/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/config/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/facades/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/facades/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/facades/frontrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/facades/injective.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/facades/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/paginators.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/logging/log_external_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/logging/log_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.696608 frontrunner-sdk-0.3.0/frontrunner_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/models/cancel_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/models/denom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/models/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.692608 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.700608 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.700608 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.700608 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/league.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:05.692608 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:13:05.700608 frontrunner-sdk-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-31 19:13:05.000000 frontrunner-sdk-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/denom_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/injective_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/injective_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/injective_light_client_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/clients/openapi_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/find_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_leagues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_sport_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_sport_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_sports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/cancel_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/create_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/create_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/fund_subaccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_account_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_order_books.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/config/chained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/config/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/config/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/config/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/facades/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/facades/frontrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/facades/injective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/facades/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/logging/log_external_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/logging/log_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/models/cancel_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/models/denom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/models/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.331939 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/league.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/frontrunner_sdk/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:38:20.335939 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 19:38:20.000000 frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:38:20.339939 frontrunner-sdk-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-08-02 19:38:19.000000 frontrunner-sdk-0.4.0/setup.py
```

### Comparing `frontrunner-sdk-0.3.0/PKG-INFO` & `frontrunner-sdk-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontrunner-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Frontrunner SDK
 Home-page: https://github.com/GetFrontrunner/frontrunner-sdk
 Author: Frontrunner
 Author-email: support@getfrontrunner.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `frontrunner-sdk-0.3.0/backend_shim.py` & `frontrunner-sdk-0.4.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/clients/denom_factory.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/clients/denom_factory.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/clients/injective_chain.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/clients/injective_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pyinjective.transaction import Transaction
 
 from frontrunner_sdk.exceptions import FrontrunnerInjectiveException
 from frontrunner_sdk.helpers.paginators import injective_paginated_list
 from frontrunner_sdk.logging.log_external_exceptions import log_external_exceptions # NOQA
 from frontrunner_sdk.models.cancel_order import CancelOrder
 from frontrunner_sdk.models.order import Order
+from frontrunner_sdk.models.wallet import Subaccount
 from frontrunner_sdk.models.wallet import Wallet
 
 logger = logging.getLogger(__name__)
 
 
 class InjectiveChain:
 
@@ -56,16 +57,16 @@
     signing_document = transaction.get_sign_doc(wallet.public_key)
     signature = wallet.private_key.sign(signing_document.SerializeToString())
     return transaction.get_tx_data(signature, wallet.public_key)
 
   def _estimate_fee(self, simulation: SimulationResponse) -> Tuple[int, List[Coin]]:
     limit = int(simulation.gas_info.gas_used) + self.ADDITIONAL_GAS_FEE
     amount = self.GAS_PRICE * limit
-    fee = [self.composer.Coin(amount=str(amount), denom=self.network.fee_denom)]
-    return (limit, fee)
+    fee = [self.composer.Coin(amount=amount, denom=self.network.fee_denom)]
+    return limit, fee
 
   def _injective_order(self, wallet: Wallet, order: Order) -> Message:
     return self.composer.BinaryOptionsOrder(
       market_id=order.market_id,
       quantity=order.quantity,
       price=order.price,
 
@@ -75,25 +76,25 @@
       # [sell, short] => [is_buy = True, is_reduce_only = True]
       is_buy=((order.direction == "buy") == (order.side == "long")),
       is_reduce_only=(order.direction == "sell"),
 
       # TODO allow different fee recipient address
       fee_recipient=wallet.injective_address,
 
-      # use default subaccount; can revisit this later
-      subaccount_id=wallet.subaccount_address(),
+      # uses default subaccount if not set explicitly on the order
+      subaccount_id=wallet.subaccount_address(order.subaccount_index),
 
       # We need to specify a placeholder denom because one isn't hardcoded for
       # our ephemeral markets.
       denom=self.DENOM,
     )
 
-  def _injective_order_cancel(self, wallet: Wallet, market_id: str, order_hash: str):
+  def _injective_order_cancel(self, wallet: Wallet, market_id: str, order_hash: str, subaccount_index: int):
     return self.composer.OrderData(
-      market_id=market_id, subaccount_id=wallet.subaccount_address(), order_hash=order_hash
+      market_id=market_id, subaccount_id=wallet.subaccount_address(subaccount_index), order_hash=order_hash
     )
 
   async def _simulate_transaction(self, wallet: Wallet, sequence: int, messages: List[Message]) -> SimulationResponse:
     transaction = self._sign_transaction(
       wallet,
       Transaction(
         msgs=messages,
@@ -169,19 +170,19 @@
   async def _execute_transaction(self, wallet: Wallet, messages: List[Message]) -> TxResponse:
     sequence = wallet.get_and_increment_sequence()
     simulation = await self._simulate_transaction(wallet, sequence, messages)
     gas, fee = self._estimate_fee(simulation)
     return await self._send_transaction(wallet, sequence, messages, gas, fee)
 
   @log_external_exceptions(__name__)
-  async def get_all_open_orders(self, wallet: Wallet) -> Iterable[DerivativeLimitOrder]:
+  async def get_all_open_orders(self, subaccount: Subaccount) -> Iterable[DerivativeLimitOrder]:
     return await injective_paginated_list(
       self.client.get_derivative_subaccount_orders,
       "orders",
-      wallet.subaccount_address(),
+      subaccount.subaccount_id,
     )
 
   @log_external_exceptions(__name__)
   async def create_orders(
     self,
     wallet: Wallet,
     orders: Iterable[Order],
@@ -195,29 +196,43 @@
 
     return await self._execute_transaction(wallet, [batch_message])
 
   @log_external_exceptions(__name__)
   async def cancel_all_orders_for_markets(
     self,
     wallet: Wallet,
+    subaccount: Subaccount,
     injective_market_ids: Set[str],
   ) -> TxResponse:
     batch_message = self.composer.MsgBatchUpdateOrders(
       wallet.injective_address,
-      subaccount_id=wallet.subaccount_address(),
+      subaccount_id=subaccount.subaccount_id,
       binary_options_market_ids_to_cancel_all=injective_market_ids,
     )
 
     return await self._execute_transaction(wallet, [batch_message])
 
   @log_external_exceptions(__name__)
   async def cancel_orders(self, wallet: Wallet, orders: Iterable[CancelOrder]) -> TxResponse:
     order_messages = [
-      self._injective_order_cancel(wallet, order.market_id, order.order_hash) for order in orders if order.order_hash
+      self._injective_order_cancel(wallet, order.market_id, order.order_hash, order.subaccount_index)
+      for order in orders
+      if order.order_hash
     ]
 
     batch_message = self.composer.MsgBatchUpdateOrders(
       wallet.injective_address,
       binary_options_orders_to_cancel=order_messages,
     )
 
     return await self._execute_transaction(wallet, [batch_message])
+
+  @log_external_exceptions(__name__)
+  async def fund_subaccount(self, wallet: Wallet, subaccount_id: str, amount: int, denom: str) -> TxResponse:
+    message = self.composer.MsgDeposit(
+      wallet.injective_address,
+      subaccount_id=subaccount_id,
+      amount=amount,
+      denom=denom,
+    )
+
+    return await self._execute_transaction(wallet, [message])
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/clients/injective_faucet.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/clients/injective_faucet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/clients/injective_light_client_daemon.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/clients/injective_light_client_daemon.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/clients/openapi_client.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/base.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/find_markets.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/find_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_leagues.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_leagues.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_markets.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_props.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_props.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_sport_entities.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_sport_entities.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_sport_events.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_sport_events.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/frontrunner/get_sports.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/frontrunner/get_sports.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/cancel_orders.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/cancel_orders.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativeLimitOrder # NOQA
 
 from frontrunner_sdk.commands.base import FrontrunnerOperation
 from frontrunner_sdk.exceptions import FrontrunnerArgumentException
 from frontrunner_sdk.ioc import FrontrunnerIoC
 from frontrunner_sdk.logging.log_operation import log_operation
+from frontrunner_sdk.models import Subaccount
 from frontrunner_sdk.models.cancel_order import CancelOrder
 
 
 @dataclass
 class CancelAllOrdersRequest:
-  pass
+  subaccount_index: int = 0
 
 
 @dataclass
 class CancelAllOrdersResponse:
   orders: Iterable[DerivativeLimitOrder]
   transaction: Optional[str] = None
 
@@ -29,23 +30,24 @@
 
   def validate(self, deps: FrontrunnerIoC) -> None:
     pass
 
   @log_operation(__name__)
   async def execute(self, deps: FrontrunnerIoC) -> CancelAllOrdersResponse:
     wallet = await deps.wallet()
+    subaccount = Subaccount.from_wallet_and_index(wallet, self.request.subaccount_index)
 
-    open_orders = await deps.injective_chain.get_all_open_orders(wallet)
+    open_orders = await deps.injective_chain.get_all_open_orders(subaccount)
 
     if not open_orders:
       return CancelAllOrdersResponse(orders=[])
 
     injective_market_ids = {order.market_id for order in open_orders}
 
-    response = await deps.injective_chain.cancel_all_orders_for_markets(wallet, injective_market_ids)
+    response = await deps.injective_chain.cancel_all_orders_for_markets(wallet, subaccount, injective_market_ids)
 
     return CancelAllOrdersResponse(
       transaction=response.txhash,
       orders=open_orders,
     )
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/create_orders.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/create_orders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from collections import defaultdict
 from dataclasses import dataclass
 from typing import List
 
 from frontrunner_sdk.commands.base import FrontrunnerOperation
 from frontrunner_sdk.exceptions import FrontrunnerArgumentException
 from frontrunner_sdk.ioc import FrontrunnerIoC
 from frontrunner_sdk.logging.log_operation import log_operation
 from frontrunner_sdk.models.order import Order
+from frontrunner_sdk.models.order import OrderType
 
 
 @dataclass
 class CreateOrdersRequest:
   orders: List[Order]
 
 
@@ -23,19 +25,30 @@
   def __init__(self, request: CreateOrdersRequest):
     super().__init__(request)
 
   def validate(self, deps: FrontrunnerIoC) -> None:
     if not len(self.request.orders):
       raise FrontrunnerArgumentException("Orders cannot be empty")
 
+    orders_by_subaccount_and_market: dict = defaultdict(lambda: defaultdict(list))
     for order in self.request.orders:
       if order.quantity <= 0:
         raise FrontrunnerArgumentException("Order quantity must be > 0", order=order)
 
       if order.price <= 0 or 1 <= order.price:
         raise FrontrunnerArgumentException("Order price must be within between 0 and 1 exclusive", order=order)
 
+      orders_for_subaccount_and_market = orders_by_subaccount_and_market[order.subaccount_index][order.market_id]
+      order_types = set([
+        OrderType.from_direction_and_side(order.direction, order.side) for order in orders_for_subaccount_and_market
+      ])
+      if OrderType.BUY_LONG in order_types and OrderType.BUY_SHORT in order_types:
+        raise FrontrunnerArgumentException(
+          f"Cannot place both short and long orders in market {order.market_id} from a single subaccount"
+        )
+      orders_by_subaccount_and_market[order.subaccount_index][order.market_id] += [order]
+
   @log_operation(__name__)
   async def execute(self, deps: FrontrunnerIoC) -> CreateOrdersResponse:
     response = await deps.injective_chain.create_orders(await deps.wallet(), self.request.orders)
 
     return CreateOrdersResponse(transaction=response.txhash)
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/create_wallet.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/create_wallet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_account_portfolio.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_account_portfolio.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_order_books.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_order_books.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_orders.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_trades.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,86 @@
 from dataclasses import dataclass
-from datetime import datetime
+from typing import Any
+from typing import AsyncIterator
+from typing import Dict
+from typing import Iterable
 from typing import List
 from typing import Literal
 from typing import Optional
-from typing import Sequence
 
-from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativeLimitOrder # NOQA
-from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativeOrderHistory # NOQA
+from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativeTrade # NOQA
 
 from frontrunner_sdk.commands.base import FrontrunnerOperation
-from frontrunner_sdk.helpers.paginators import injective_paginated_list
-from frontrunner_sdk.helpers.validation import validate_mutually_exclusive
-from frontrunner_sdk.helpers.validation import validate_start_time_end_time
+from frontrunner_sdk.exceptions import FrontrunnerArgumentException
+from frontrunner_sdk.helpers.streams import injective_stream
+from frontrunner_sdk.helpers.validation import validate_all_mutually_exclusive
 from frontrunner_sdk.ioc import FrontrunnerIoC
 from frontrunner_sdk.logging.log_operation import log_operation
-from frontrunner_sdk.models import InjectiveOrderExecutionType
-from frontrunner_sdk.models import InjectiveOrderState
-from frontrunner_sdk.models import InjectiveOrderType
-from frontrunner_sdk.models import OrderHistory
+from frontrunner_sdk.models import Subaccount
 
 
 @dataclass
-class GetOrdersRequest:
-  # internal fields
-  mine: Optional[bool] = None
-  # passthrough fields
-  market_ids: Optional[List[str]] = None
-  subaccount_id: Optional[str] = None
+class StreamTradesRequest:
+  market_ids: Iterable[str]
+  mine: bool
   direction: Optional[Literal["buy", "sell"]] = None
-  is_conditional: Optional[bool] = None
-  order_types: Optional[List[InjectiveOrderType]] = None
-  state: Optional[InjectiveOrderState] = None
-  execution_types: Optional[List[InjectiveOrderExecutionType]] = None
-  start_time: Optional[datetime] = None
-  end_time: Optional[datetime] = None
+  side: Optional[Literal["maker", "taker"]] = None
+  # internal fields
+  subaccount: Optional[Subaccount] = None
+  subaccount_index: Optional[int] = None
+  subaccounts: Optional[List[Subaccount]] = None
+  subaccount_indexes: Optional[List[int]] = None
 
 
 @dataclass
-class GetOrdersResponse:
-  orders: Sequence[OrderHistory]
+class StreamTradesResponse:
+  trades: AsyncIterator[DerivativeTrade]
 
 
-class GetOrdersOperation(FrontrunnerOperation[GetOrdersRequest, GetOrdersResponse]):
+class StreamTradesOperation(FrontrunnerOperation[StreamTradesRequest, StreamTradesResponse]):
 
-  def __init__(self, request: GetOrdersRequest):
+  MUTUALLY_EXCLUSIVE_PARAMS = ["subaccount", "subaccount_index", "subaccounts", "subaccount_indexes"]
+  MUTUALLY_EXCLUSIVE_PARAMS_MINE = ["mine", "subaccount"]
+  MUTUALLY_EXCLUSIVE_PARAMS_MINE_PLURAL = ["mine", "subaccounts"]
+
+  def __init__(self, request: StreamTradesRequest):
     super().__init__(request)
 
   def validate(self, deps: FrontrunnerIoC) -> None:
-    validate_mutually_exclusive("mine", self.request.mine, "subaccount_id", self.request.subaccount_id)
-    validate_start_time_end_time(self.request.start_time, self.request.end_time)
+    if not self.request.market_ids:
+      raise FrontrunnerArgumentException("At least one market id is required")
+
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS_MINE)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS_MINE_PLURAL)
 
   @log_operation(__name__)
-  async def execute(self, deps: FrontrunnerIoC) -> GetOrdersResponse:
-    request = self.request_as_kwargs()
-    request.pop("mine", None)
+  async def execute(self, deps: FrontrunnerIoC) -> StreamTradesResponse:
+    request: Dict[str, Any] = {
+      "market_ids": list(self.request.market_ids),
+    }
 
-    if self.request.mine:
+    if (self.request.mine and not self.request.subaccount_indexes) or self.request.subaccount_index is not None:
       wallet = await deps.wallet()
-      request["subaccount_id"] = wallet.subaccount_address()
-    if self.request.is_conditional is not None:
-      request["is_conditional"] = str(self.request.is_conditional).lower()
-
-    if self.request.start_time:
-      request["start_time"] = int(self.request.start_time.timestamp())
-
-    if self.request.end_time:
-      request["end_time"] = int(self.request.end_time.timestamp())
-
-    injective_orders: Sequence[DerivativeOrderHistory] = await injective_paginated_list(
-      deps.injective_client.get_historical_derivative_orders,
-      "orders",
-      # Force market_id=None since we use optional market_ids param instead
-      # TODO: remove workaround once Injective SDK has market_id as optional
-      None,
-      **request,
-    )
+      request["subaccount_id"] = wallet.subaccount_address(self.request.subaccount_index or 0)
 
-    orders = OrderHistory._from_injective_derivative_order_histories(injective_orders)
+    if self.request.subaccount:
+      request["subaccount_id"] = self.request.subaccount.subaccount_id
 
-    return GetOrdersResponse(orders=orders)
+    if self.request.subaccount_indexes:
+      wallet = await deps.wallet()
+      request["subaccount_ids"] = [wallet.subaccount_address(index) for index in self.request.subaccount_indexes]
+
+    if self.request.subaccounts:
+      request["subaccount_ids"] = [subaccount.subaccount_id for subaccount in self.request.subaccounts]
+
+    if self.request.direction:
+      request["direction"] = self.request.direction
+
+    if self.request.side:
+      request["execution_side"] = self.request.side
+
+    trades: AsyncIterator[DerivativeTrade] = await injective_stream(
+      deps.injective_client.stream_derivative_trades,
+      **request,
+    )
+    return StreamTradesResponse(trades)
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/get_positions.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/get_positions.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,51 +8,63 @@
 from typing import Sequence
 
 from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativePosition # NOQA
 
 from frontrunner_sdk.commands.base import FrontrunnerOperation
 from frontrunner_sdk.exceptions import FrontrunnerArgumentException
 from frontrunner_sdk.helpers.paginators import injective_paginated_list
+from frontrunner_sdk.helpers.validation import validate_all_mutually_exclusive
 from frontrunner_sdk.helpers.validation import validate_start_time_end_time
 from frontrunner_sdk.ioc import FrontrunnerIoC
 from frontrunner_sdk.logging.log_operation import log_operation
+from frontrunner_sdk.models import Subaccount
 
 
 @dataclass
 class GetPositionsRequest:
   mine: bool = False
+  subaccount: Optional[Subaccount] = None
+  subaccount_index: Optional[int] = None
   market_ids: Optional[Iterable[str]] = None
   direction: Optional[Literal["buy", "sell"]] = None
   start_time: Optional[datetime] = None
   end_time: Optional[datetime] = None
 
 
 @dataclass
 class GetPositionsResponse:
   positions: Sequence[DerivativePosition]
 
 
 class GetPositionsOperation(FrontrunnerOperation[GetPositionsRequest, GetPositionsResponse]):
 
+  MUTUALLY_EXCLUSIVE_PARAMS = ["subaccount", "subaccount_index"]
+  MUTUALLY_EXCLUSIVE_PARAMS_MINE = ["mine", "subaccount"]
+
   def __init__(self, request: GetPositionsRequest):
     super().__init__(request)
 
   def validate(self, deps: FrontrunnerIoC) -> None:
     if not self.request.mine and not self.request.market_ids:
       raise FrontrunnerArgumentException("Either mine must be True, or at least one market id must be provided")
 
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS_MINE)
     validate_start_time_end_time(self.request.start_time, self.request.end_time)
 
   @log_operation(__name__)
   async def execute(self, deps: FrontrunnerIoC) -> GetPositionsResponse:
     request: Dict[str, Any] = {}
 
-    if self.request.mine:
+    if self.request.mine or self.request.subaccount_index is not None:
       wallet = await deps.wallet()
-      request["subaccount_id"] = wallet.subaccount_address()
+      request["subaccount_id"] = wallet.subaccount_address(self.request.subaccount_index or 0)
+
+    if self.request.subaccount:
+      request["subaccount_id"] = self.request.subaccount.subaccount_id
 
     if self.request.market_ids:
       request["market_ids"] = list(self.request.market_ids)
 
     if self.request.start_time:
       request["start_time"] = int(self.request.start_time.timestamp())
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_markets.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_orders.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_orders.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,60 +6,74 @@
 
 from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativeLimitOrder # NOQA
 from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativeOrderHistory # NOQA
 
 from frontrunner_sdk.commands.base import FrontrunnerOperation
 from frontrunner_sdk.exceptions import FrontrunnerArgumentException
 from frontrunner_sdk.helpers.streams import injective_stream
-from frontrunner_sdk.helpers.validation import validate_mutually_exclusive
+from frontrunner_sdk.helpers.validation import validate_all_mutually_exclusive
 from frontrunner_sdk.ioc import FrontrunnerIoC
 from frontrunner_sdk.logging.log_operation import log_operation
 from frontrunner_sdk.models import InjectiveOrderExecutionType
 from frontrunner_sdk.models import InjectiveOrderState
 from frontrunner_sdk.models import InjectiveOrderType
 from frontrunner_sdk.models import OrderHistory
+from frontrunner_sdk.models import Subaccount
 
 
 @dataclass
 class StreamOrdersRequest:
-  # internal fields
+  # internal required fields
   mine: bool
-  # passthrough fields
+  # passthrough required fields
   market_id: str
+  # internal fields
+  subaccount: Optional[Subaccount] = None
+  subaccount_index: Optional[int] = None
+  # passthrough fields
   direction: Optional[Literal["buy", "sell"]] = None
   subaccount_id: Optional[str] = None
   order_types: Optional[List[InjectiveOrderType]] = None
   state: Optional[InjectiveOrderState] = None
   execution_types: Optional[List[InjectiveOrderExecutionType]] = None
 
 
 @dataclass
 class StreamOrdersResponse:
   orders: AsyncIterator[OrderHistory]
 
 
 class StreamOrdersOperation(FrontrunnerOperation[StreamOrdersRequest, StreamOrdersResponse]):
 
+  MUTUALLY_EXCLUSIVE_PARAMS = ["subaccount_id", "subaccount", "subaccount_index"]
+  MUTUALLY_EXCLUSIVE_PARAMS_MINE = ["mine", "subaccount_id", "subaccount"]
+
   def __init__(self, request: StreamOrdersRequest):
     super().__init__(request)
 
   def validate(self, deps: FrontrunnerIoC) -> None:
     if not self.request.market_id:
       raise FrontrunnerArgumentException("'market_id' is required")
 
-    validate_mutually_exclusive("mine", self.request.mine, "subaccount_id", self.request.subaccount_id)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS_MINE)
 
   @log_operation(__name__)
   async def execute(self, deps: FrontrunnerIoC) -> StreamOrdersResponse:
     request = self.request_as_kwargs()
     request.pop("mine", None)
+    request.pop("subaccount", None)
+    request.pop("subaccount_index", None)
 
-    if self.request.mine:
+    if self.request.mine or self.request.subaccount_index is not None:
       wallet = await deps.wallet()
-      request["subaccount_id"] = wallet.subaccount_address()
+      request["subaccount_id"] = wallet.subaccount_address(self.request.subaccount_index or 0)
+
+    if self.request.subaccount:
+      request["subaccount_id"] = self.request.subaccount.subaccount_id
 
     injective_orders: AsyncIterator[DerivativeOrderHistory] = await injective_stream(
       deps.injective_client.stream_historical_derivative_orders,
       **request,
     )
     orders: AsyncIterator[OrderHistory] = OrderHistory._from_async_iterator(injective_orders)
     return StreamOrdersResponse(orders)
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/commands/injective/stream_positions.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/commands/injective/stream_positions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 from dataclasses import dataclass
 from typing import AsyncIterator
 from typing import Iterable
+from typing import List
 from typing import Optional
 
 from pyinjective.proto.exchange.injective_derivative_exchange_rpc_pb2 import DerivativePosition # NOQA
 
 from frontrunner_sdk.commands.base import FrontrunnerOperation
 from frontrunner_sdk.helpers.streams import injective_stream
-from frontrunner_sdk.helpers.validation import validate_mutually_exclusive
+from frontrunner_sdk.helpers.validation import validate_all_mutually_exclusive
 from frontrunner_sdk.ioc import FrontrunnerIoC
 from frontrunner_sdk.logging.log_operation import log_operation
+from frontrunner_sdk.models import Subaccount
 
 
 @dataclass
 class StreamPositionsRequest:
-  # internal fields
+  # internal required fields
   mine: bool
-  # passthrough fields
+  # passthrough required fields
   market_ids: Optional[Iterable[str]] = None
   subaccount_ids: Optional[Iterable[str]] = None
+  # internal optional fields
+  subaccounts: Optional[List[Subaccount]] = None
+  subaccount_indexes: Optional[List[int]] = None
 
 
 @dataclass
 class StreamPositionsResponse:
   positions: AsyncIterator[DerivativePosition]
 
 
 class StreamPositionsOperation(FrontrunnerOperation[StreamPositionsRequest, StreamPositionsResponse]):
 
+  MUTUALLY_EXCLUSIVE_PARAMS = ["subaccounts", "subaccount_indexes"]
+  MUTUALLY_EXCLUSIVE_PARAMS_MINE = ["mine", "subaccount_ids", "subaccounts"]
+
   def __init__(self, request: StreamPositionsRequest):
     super().__init__(request)
 
   def validate(self, deps: FrontrunnerIoC) -> None:
-    validate_mutually_exclusive("mine", self.request.mine, "subaccount_ids", self.request.subaccount_ids)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS)
+    validate_all_mutually_exclusive(self.request, self.MUTUALLY_EXCLUSIVE_PARAMS_MINE)
 
   @log_operation(__name__)
   async def execute(self, deps: FrontrunnerIoC) -> StreamPositionsResponse:
     request = self.request_as_kwargs()
     request.pop("mine", None)
+    request.pop("subaccounts", None)
+    request.pop("subaccount_indexes", None)
 
     if self.request.mine:
       wallet = await deps.wallet()
       request["subaccount_ids"] = [wallet.subaccount_address()]
 
+    if self.request.subaccount_indexes:
+      wallet = await deps.wallet()
+      request["subaccount_ids"] = [wallet.subaccount_address(index) for index in self.request.subaccount_indexes]
+
+    if self.request.subaccounts:
+      request["subaccount_ids"] = [subaccount.subaccount_id for subaccount in self.request.subaccounts]
+
     positions: AsyncIterator[DerivativePosition] = await injective_stream(
       deps.injective_client.stream_derivative_positions,
       **request,
     )
     return StreamPositionsResponse(positions)
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/config/__init__.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/config/base.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/config/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/config/chained.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/config/chained.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/config/conditional.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/config/conditional.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/config/environment_variable.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/config/environment_variable.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/config/static.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/config/static.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/exceptions/__init__.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/facades/base.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/facades/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/facades/frontrunner.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/facades/frontrunner.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/facades/injective.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/facades/injective.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from frontrunner_sdk.commands.injective.cancel_orders import CancelOrdersResponse # NOQA
 from frontrunner_sdk.commands.injective.create_orders import CreateOrdersOperation # NOQA
 from frontrunner_sdk.commands.injective.create_orders import CreateOrdersRequest # NOQA
 from frontrunner_sdk.commands.injective.create_orders import CreateOrdersResponse # NOQA
 from frontrunner_sdk.commands.injective.create_wallet import CreateWalletOperation # NOQA
 from frontrunner_sdk.commands.injective.create_wallet import CreateWalletRequest # NOQA
 from frontrunner_sdk.commands.injective.create_wallet import CreateWalletResponse # NOQA
+from frontrunner_sdk.commands.injective.fund_subaccount import FundSubaccountOperation # NOQA
+from frontrunner_sdk.commands.injective.fund_subaccount import FundSubaccountRequest # NOQA
+from frontrunner_sdk.commands.injective.fund_subaccount import FundSubaccountResponse # NOQA
 from frontrunner_sdk.commands.injective.fund_wallet_from_faucet import FundWalletFromFaucetOperation # NOQA
 from frontrunner_sdk.commands.injective.fund_wallet_from_faucet import FundWalletFromFaucetRequest # NOQA
 from frontrunner_sdk.commands.injective.fund_wallet_from_faucet import FundWalletFromFaucetResponse # NOQA
 from frontrunner_sdk.commands.injective.get_account_portfolio import GetAccountPortfolioOperation # NOQA
 from frontrunner_sdk.commands.injective.get_account_portfolio import GetAccountPortfolioRequest # NOQA
 from frontrunner_sdk.commands.injective.get_account_portfolio import GetAccountPortfolioResponse # NOQA
 from frontrunner_sdk.commands.injective.get_order_books import GetOrderBooksOperation # NOQA
@@ -45,14 +48,15 @@
 from frontrunner_sdk.commands.injective.stream_positions import StreamPositionsResponse # NOQA
 from frontrunner_sdk.commands.injective.stream_trades import StreamTradesOperation # NOQA
 from frontrunner_sdk.commands.injective.stream_trades import StreamTradesRequest # NOQA
 from frontrunner_sdk.commands.injective.stream_trades import StreamTradesResponse # NOQA
 from frontrunner_sdk.facades.base import FrontrunnerFacadeMixin # NOQA
 from frontrunner_sdk.helpers.parameters import as_request_args
 from frontrunner_sdk.ioc import FrontrunnerIoC
+from frontrunner_sdk.models import Subaccount
 from frontrunner_sdk.models.cancel_order import CancelOrder
 from frontrunner_sdk.models.order import InjectiveOrderExecutionType
 from frontrunner_sdk.models.order import InjectiveOrderState
 from frontrunner_sdk.models.order import InjectiveOrderType
 from frontrunner_sdk.models.order import Order
 from frontrunner_sdk.sync import SyncMixin
 
@@ -62,24 +66,34 @@
   def __init__(self, deps: FrontrunnerIoC):
     self.deps = deps
 
   async def create_wallet(self, fund_and_initialize: bool = True) -> CreateWalletResponse:
     request = CreateWalletRequest(fund_and_initialize=fund_and_initialize)
     return await self._run_operation(CreateWalletOperation, self.deps, request)
 
+  async def fund_subaccount(
+    self,
+    amount: int,
+    denom: str,
+    subaccount_index: Optional[int] = None,
+    subaccount: Optional[Subaccount] = None,
+  ) -> FundSubaccountResponse:
+    request = FundSubaccountRequest(amount, denom, subaccount=subaccount, subaccount_index=subaccount_index)
+    return await self._run_operation(FundSubaccountOperation, self.deps, request)
+
   async def fund_wallet_from_faucet(self) -> FundWalletFromFaucetResponse:
     request = FundWalletFromFaucetRequest()
     return await self._run_operation(FundWalletFromFaucetOperation, self.deps, request)
 
   async def create_orders(self, orders: List[Order]) -> CreateOrdersResponse:
     request = CreateOrdersRequest(orders=orders)
     return await self._run_operation(CreateOrdersOperation, self.deps, request)
 
-  async def cancel_all_orders(self) -> CancelAllOrdersResponse:
-    request = CancelAllOrdersRequest()
+  async def cancel_all_orders(self, subaccount_index: int = 0) -> CancelAllOrdersResponse:
+    request = CancelAllOrdersRequest(subaccount_index=subaccount_index)
     return await self._run_operation(CancelAllOrdersOperation, self.deps, request)
 
   async def cancel_orders(self, orders: Iterable[CancelOrder]) -> CancelOrdersResponse:
     request = CancelOrdersRequest(orders=orders)
     return await self._run_operation(CancelOrdersOperation, self.deps, request)
 
   async def get_account_portfolio(self) -> GetAccountPortfolioResponse:
@@ -91,14 +105,16 @@
     return await self._run_operation(GetOrderBooksOperation, self.deps, request)
 
   async def get_orders(
     self,
     mine: Optional[bool] = None,
     market_ids: Optional[List[str]] = None,
     subaccount_id: Optional[str] = None,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     is_conditional: Optional[bool] = None,
     order_types: Optional[List[InjectiveOrderType]] = None,
     state: Optional[InjectiveOrderState] = None,
     execution_types: Optional[List[InjectiveOrderExecutionType]] = None,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
@@ -106,27 +122,33 @@
     kwargs = as_request_args(locals())
     request = GetOrdersRequest(**kwargs)
     return await self._run_operation(GetOrdersOperation, self.deps, request)
 
   async def get_positions(
     self,
     mine: bool = False,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
     market_ids: Optional[Iterable[str]] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
   ) -> GetPositionsResponse:
     kwargs = as_request_args(locals())
     request = GetPositionsRequest(**kwargs)
     return await self._run_operation(GetPositionsOperation, self.deps, request)
 
   async def get_trades(
     self,
     market_ids: Iterable[str],
     mine: bool = False,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
+    subaccounts: Optional[List[Subaccount]] = None,
+    subaccount_indexes: Optional[List[int]] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     side: Optional[Literal["maker", "taker"]] = None,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
   ) -> GetTradesResponse:
     kwargs = as_request_args(locals())
     request = GetTradesRequest(**kwargs)
@@ -151,14 +173,16 @@
     request = StreamMarketsRequest(**kwargs)
     return await self._run_operation(StreamMarketsOperation, self.deps, request)
 
   async def stream_orders(
     self,
     market_id: str,
     mine: bool = False,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     subaccount_id: Optional[str] = None,
     order_types: Optional[List[str]] = None,
     state: Optional[str] = None,
     execution_types: Optional[str] = None,
   ) -> StreamOrdersResponse:
     kwargs = as_request_args(locals())
@@ -166,14 +190,16 @@
     return await self._run_operation(StreamOrdersOperation, self.deps, request)
 
   async def stream_positions(
     self,
     mine: bool = False,
     market_ids: Optional[List[str]] = None,
     subaccount_ids: Optional[List[str]] = None,
+    subaccounts: Optional[List[Subaccount]] = None,
+    subaccount_indexes: Optional[List[int]] = None,
   ) -> StreamPositionsResponse:
     kwargs = as_request_args(locals())
     request = StreamPositionsRequest(**kwargs)
     return await self._run_operation(StreamPositionsOperation, self.deps, request)
 
 
 class InjectiveFacade(SyncMixin):
@@ -186,16 +212,16 @@
 
   def fund_wallet_from_faucet(self) -> FundWalletFromFaucetResponse:
     return self._synchronously(self.impl.fund_wallet_from_faucet)
 
   def create_orders(self, orders: Iterable[Order]) -> CreateOrdersResponse:
     return self._synchronously(self.impl.create_orders, orders)
 
-  def cancel_all_orders(self) -> CancelAllOrdersResponse:
-    return self._synchronously(self.impl.cancel_all_orders)
+  def cancel_all_orders(self, subaccount_index: int = 0) -> CancelAllOrdersResponse:
+    return self._synchronously(self.impl.cancel_all_orders, subaccount_index)
 
   def cancel_orders(self, orders: Iterable[CancelOrder]) -> CancelOrdersResponse:
     return self._synchronously(self.impl.cancel_orders, orders)
 
   def get_account_portfolio(self) -> GetAccountPortfolioResponse:
     return self._synchronously(self.impl.get_account_portfolio)
 
@@ -203,40 +229,48 @@
     return self._synchronously(self.impl.get_order_books, market_ids)
 
   def get_orders(
     self,
     mine: Optional[bool] = None,
     market_ids: Optional[List[str]] = None,
     subaccount_id: Optional[str] = None,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     is_conditional: Optional[bool] = None,
     order_types: Optional[List[InjectiveOrderType]] = None,
     state: Optional[InjectiveOrderState] = None,
     execution_types: Optional[List[InjectiveOrderExecutionType]] = None,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
   ) -> GetOrdersResponse:
     kwargs = as_request_args(locals())
     return self._synchronously(self.impl.get_orders, **kwargs)
 
   def get_positions(
     self,
     mine: bool = False,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
     market_ids: Optional[Iterable[str]] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
   ) -> GetPositionsResponse:
     kwargs = as_request_args(locals())
     return self._synchronously(self.impl.get_positions, **kwargs)
 
   def get_trades(
     self,
     market_ids: Iterable[str],
     mine: bool = False,
+    subaccount: Optional[Subaccount] = None,
+    subaccount_index: Optional[int] = None,
+    subaccounts: Optional[List[Subaccount]] = None,
+    subaccount_indexes: Optional[List[int]] = None,
     direction: Optional[Literal["buy", "sell"]] = None,
     side: Optional[Literal["maker", "taker"]] = None,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
   ) -> GetTradesResponse:
     kwargs = as_request_args(locals())
     return self._synchronously(self.impl.get_trades, **kwargs)
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/facades/utilities.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/facades/utilities.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/paginators.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/paginators.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/streams.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/streams.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/helpers/validation.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/helpers/validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from datetime import datetime
 from typing import Any
+from typing import List
 from typing import Optional
 
 from frontrunner_sdk.exceptions import FrontrunnerArgumentException
 
 
 def validate_mutually_exclusive(name1: str, val1: Optional[Any], name2: str, val2: Optional[Any]):
   if val1 is not None and val2 is not None:
     kwargs = {name1: val1, name2: val2}
     raise FrontrunnerArgumentException(f"'{name1}' and '{name2}' are mutually exclusive", **kwargs)
 
 
+def validate_all_mutually_exclusive(request: object, names: List[str]):
+  num_mutually_exclusive_params = sum(getattr(request, prop) is not None for prop in names)
+  if num_mutually_exclusive_params > 1:
+    raise FrontrunnerArgumentException(f"These request params are mutually exclusive: {names}")
+
+
 def validate_start_time_end_time(start_time: Optional[datetime], end_time: Optional[datetime]):
   now = datetime.now()
 
   if start_time and start_time > now:
     raise FrontrunnerArgumentException(
       "Start time cannot be in the future",
       now=now,
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/ioc.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/ioc.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/logging/log_external_exceptions.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/logging/log_external_exceptions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/logging/log_operation.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/logging/log_operation.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/models/currency.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/models/currency.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/models/order.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/models/order.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,35 +19,56 @@
 
 class OrderType(Enum):
   BUY_LONG = 0
   BUY_SHORT = 1
   SELL_LONG = 2
   SELL_SHORT = 3
 
+  @classmethod
+  def from_injective_params(cls, direction: str, is_reduce_only: bool):
+    if direction == "buy" and not is_reduce_only:
+      return cls.BUY_LONG
+    elif direction == "sell" and not is_reduce_only:
+      return cls.BUY_SHORT
+    elif direction == "buy" and is_reduce_only:
+      return cls.SELL_SHORT
+    elif direction == "sell" and is_reduce_only:
+      return cls.SELL_LONG
+    else:
+      raise FrontrunnerInjectiveException(
+        "Unable to compute Frontrunner order type",
+        direction=direction,
+        is_reduce_only=is_reduce_only,
+      )
+
+  @classmethod
+  def from_direction_and_side(cls, direction: str, side: str):
+    if direction == "buy" and side == "long":
+      return cls.BUY_LONG
+    elif direction == "buy" and side == "short":
+      return cls.BUY_SHORT
+    elif direction == "sell" and side == "short":
+      return cls.SELL_SHORT
+    elif direction == "sell" and side == "long":
+      return cls.SELL_LONG
+    else:
+      raise FrontrunnerInjectiveException(
+        "Unable to compute Frontrunner order type",
+        direction=direction,
+        side=side,
+      )
+
 
 @dataclass
 class OrderHistory:
   order: DerivativeOrderHistory
 
   @property
   def order_type(self):
-    if self.order.direction == "buy" and not self.order.is_reduce_only:
-      return OrderType.BUY_LONG
-    elif self.order.direction == "sell" and not self.order.is_reduce_only:
-      return OrderType.BUY_SHORT
-    elif self.order.direction == "buy" and self.order.is_reduce_only:
-      return OrderType.SELL_SHORT
-    elif self.order.direction == "sell" and self.order.is_reduce_only:
-      return OrderType.SELL_LONG
-    else:
-      raise FrontrunnerInjectiveException(
-        "Unable to compute Frontrunner order type",
-        direction=self.order.direction,
-        is_reduce_only=self.order.is_reduce_only,
-      )
+    return OrderType.from_injective_params(self.order.direction, self.order.is_reduce_only)
 
   def __repr__(self):
     # Custom repr is required to pick up added @property
     return f"{self.__class__.__qualname__}(order={self.order},order_type={self.order_type})"
 
   @classmethod
   def _from_injective_derivative_order_histories(cls: Type[T], orders: Sequence[DerivativeOrderHistory]) -> Sequence[T]:
@@ -62,23 +83,24 @@
 @dataclass
 class Order:
   direction: Literal["buy", "sell"]
   side: Literal["long", "short"]
   market_id: str
   quantity: int
   price: float
+  subaccount_index: int
 
   @classmethod
-  def buy_long(clz, market_id: str, quantity: int, price: float) -> "Order":
-    return clz("buy", "long", market_id, quantity, price)
+  def buy_long(clz, market_id: str, quantity: int, price: float, subaccount_index: int = 0) -> "Order":
+    return clz("buy", "long", market_id, quantity, price, subaccount_index)
 
   @classmethod
-  def buy_short(clz, market_id: str, quantity: int, price: float) -> "Order":
-    return clz("buy", "short", market_id, quantity, price)
+  def buy_short(clz, market_id: str, quantity: int, price: float, subaccount_index: int = 0) -> "Order":
+    return clz("buy", "short", market_id, quantity, price, subaccount_index)
 
   @classmethod
-  def sell_long(clz, market_id: str, quantity: int, price: float) -> "Order":
-    return clz("sell", "long", market_id, quantity, price)
+  def sell_long(clz, market_id: str, quantity: int, price: float, subaccount_index: int = 0) -> "Order":
+    return clz("sell", "long", market_id, quantity, price, subaccount_index)
 
   @classmethod
-  def sell_short(clz, market_id: str, quantity: int, price: float) -> "Order":
-    return clz("sell", "short", market_id, quantity, price)
+  def sell_short(clz, market_id: str, quantity: int, price: float, subaccount_index: int = 0) -> "Order":
+    return clz("sell", "short", market_id, quantity, price, subaccount_index)
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/__init__.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/api_client.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/api_client.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/configuration.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/configuration.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/error.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/error.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/league.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/league.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/market.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/market.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/openapi/frontrunner_api/rest.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/openapi/frontrunner_api/rest.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk/sdk.py` & `frontrunner-sdk-0.4.0/frontrunner_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/PKG-INFO` & `frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontrunner-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Frontrunner SDK
 Home-page: https://github.com/GetFrontrunner/frontrunner-sdk
 Author: Frontrunner
 Author-email: support@getfrontrunner.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `frontrunner-sdk-0.3.0/frontrunner_sdk.egg-info/SOURCES.txt` & `frontrunner-sdk-0.4.0/frontrunner_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 frontrunner_sdk/commands/frontrunner/get_sport_entities.py
 frontrunner_sdk/commands/frontrunner/get_sport_events.py
 frontrunner_sdk/commands/frontrunner/get_sports.py
 frontrunner_sdk/commands/injective/__init__.py
 frontrunner_sdk/commands/injective/cancel_orders.py
 frontrunner_sdk/commands/injective/create_orders.py
 frontrunner_sdk/commands/injective/create_wallet.py
+frontrunner_sdk/commands/injective/fund_subaccount.py
 frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
 frontrunner_sdk/commands/injective/get_account_portfolio.py
 frontrunner_sdk/commands/injective/get_order_books.py
 frontrunner_sdk/commands/injective/get_orders.py
 frontrunner_sdk/commands/injective/get_positions.py
 frontrunner_sdk/commands/injective/get_trades.py
 frontrunner_sdk/commands/injective/stream_markets.py
```

### Comparing `frontrunner-sdk-0.3.0/setup.py` & `frontrunner-sdk-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,9 +215,9 @@
         'frontrunner_sdk.models',
         'frontrunner_sdk.openapi.frontrunner_api',
         'frontrunner_sdk.openapi.frontrunner_api.api',
         'frontrunner_sdk.openapi.frontrunner_api.models',
     ),
     'python_requires': '>=3.9,<3.11',
     'url': 'https://github.com/GetFrontrunner/frontrunner-sdk',
-    'version': '0.3.0',
+    'version': '0.4.0',
 })
```

