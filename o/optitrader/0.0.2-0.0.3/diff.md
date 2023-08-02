# Comparing `tmp/optitrader-0.0.2.tar.gz` & `tmp/optitrader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optitrader-0.0.2.tar", max compression
+gzip compressed data, was "optitrader-0.0.3.tar", max compression
```

## Comparing `optitrader-0.0.2.tar` & `optitrader-0.0.3.tar`

### file list

```diff
@@ -1,67 +1,62 @@
--rw-r--r--   0        0        0     1073 2023-06-21 14:21:29.622704 optitrader-0.0.2/LICENSE
--rw-r--r--   0        0        0     8319 2023-07-31 22:37:33.181726 optitrader-0.0.2/README.md
--rw-r--r--   0        0        0     6611 2023-07-31 22:50:32.353355 optitrader-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      218 2023-07-31 22:31:29.394400 optitrader-0.0.2/src/optitrader/__init__.py
--rw-r--r--   0        0        0     2239 2023-07-31 22:25:43.134379 optitrader-0.0.2/src/optitrader/api.py
--rw-r--r--   0        0        0       87 2023-07-31 22:16:35.718200 optitrader-0.0.2/src/optitrader/app/1_🏠_Home.py
--rw-r--r--   0        0        0      177 2023-07-31 22:16:39.107123 optitrader-0.0.2/src/optitrader/app/__init__.py
--rw-r--r--   0        0        0      248 2023-07-31 22:25:56.769513 optitrader-0.0.2/src/optitrader/app/__pycache__/1_🏠_Home.cpython-310.pyc
--rw-r--r--   0        0        0      389 2023-07-31 22:16:25.132083 optitrader-0.0.2/src/optitrader/app/about.py
--rw-r--r--   0        0        0      518 2023-07-31 22:16:25.132046 optitrader-0.0.2/src/optitrader/app/account.py
--rw-r--r--   0        0        0     1187 2023-07-31 22:16:24.915829 optitrader-0.0.2/src/optitrader/app/backtester.py
--rw-r--r--   0        0        0     3575 2023-07-31 22:25:43.108796 optitrader-0.0.2/src/optitrader/app/explore.py
--rw-r--r--   0        0        0     1305 2023-07-31 22:25:43.071331 optitrader-0.0.2/src/optitrader/app/home.py
--rw-r--r--   0        0        0     1129 2023-07-31 22:16:22.689395 optitrader-0.0.2/src/optitrader/app/page.py
--rw-r--r--   0        0        0      105 2023-07-31 22:16:37.550338 optitrader-0.0.2/src/optitrader/app/pages/2_📈_Backtester.py
--rw-r--r--   0        0        0       96 2023-07-31 22:16:32.677118 optitrader-0.0.2/src/optitrader/app/pages/3_🗺️_Explore.py
--rw-r--r--   0        0        0       96 2023-07-31 22:16:35.747188 optitrader-0.0.2/src/optitrader/app/pages/4_💼_Account.py
--rw-r--r--   0        0        0       90 2023-07-31 22:16:25.026663 optitrader-0.0.2/src/optitrader/app/pages/5_👨🏻‍💻_About.py
--rw-r--r--   0        0        0       12 2023-07-31 19:38:53.710765 optitrader-0.0.2/src/optitrader/app/pages/__init__.py
--rw-r--r--   0        0        0      272 2023-07-31 22:25:57.146093 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/2_📈_Backtester.cpython-310.pyc
--rw-r--r--   0        0        0      266 2023-07-31 22:25:57.157579 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/3_🗺️_Explore.cpython-310.pyc
--rw-r--r--   0        0        0      263 2023-07-31 22:26:01.281761 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/4_💼_Account.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-07-31 22:26:05.045788 optitrader-0.0.2/src/optitrader/app/pages/__pycache__/5_👨🏻‍💻_About.cpython-310.pyc
--rw-r--r--   0        0        0    24191 2023-07-31 22:36:35.174592 optitrader-0.0.2/src/optitrader/app/session_manager.py
--rw-r--r--   0        0        0    24190 2023-07-31 22:36:33.537641 optitrader-0.0.2/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp
--rw-r--r--   0        0        0     2621 2023-07-31 22:32:06.810228 optitrader-0.0.2/src/optitrader/backtester.py
--rw-r--r--   0        0        0      469 2023-07-31 22:16:21.845724 optitrader-0.0.2/src/optitrader/cli.py
--rw-r--r--   0        0        0     1542 2023-07-31 19:38:53.752242 optitrader-0.0.2/src/optitrader/config.py
--rw-r--r--   0        0        0      422 2023-07-31 22:16:38.897012 optitrader-0.0.2/src/optitrader/enums/__init__.py
--rw-r--r--   0        0        0      228 2023-07-31 22:16:29.794921 optitrader-0.0.2/src/optitrader/enums/backtester.py
--rw-r--r--   0        0        0      736 2023-07-31 19:38:53.803876 optitrader-0.0.2/src/optitrader/enums/iterable.py
--rw-r--r--   0        0        0     1712 2023-07-31 22:16:37.049303 optitrader-0.0.2/src/optitrader/enums/market.py
--rw-r--r--   0        0        0      860 2023-07-31 22:16:24.915822 optitrader-0.0.2/src/optitrader/enums/optimization.py
--rw-r--r--   0        0        0     6667 2023-07-31 22:28:44.554563 optitrader-0.0.2/src/optitrader/main.py
--rw-r--r--   0        0        0      231 2023-07-31 22:16:29.990535 optitrader-0.0.2/src/optitrader/market/__init__.py
--rw-r--r--   0        0        0     8461 2023-07-31 22:25:43.150556 optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py
--rw-r--r--   0        0        0     8460 2023-07-31 22:16:38.373315 optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp
--rw-r--r--   0        0        0      768 2023-07-31 22:25:43.113539 optitrader-0.0.2/src/optitrader/market/base_data_provider.py
--rw-r--r--   0        0        0       12 2023-07-31 19:38:53.914363 optitrader-0.0.2/src/optitrader/market/db/__init__.py
--rw-r--r--   0        0        0     5339 2023-07-31 22:25:43.129931 optitrader-0.0.2/src/optitrader/market/db/database.py
--rw-r--r--   0        0        0     5338 2023-07-31 22:16:37.469729 optitrader-0.0.2/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp
--rw-r--r--   0        0        0     1935 2023-07-31 19:38:53.949530 optitrader-0.0.2/src/optitrader/market/db/models.py
--rw-r--r--   0        0        0       12 2023-07-31 19:38:53.965858 optitrader-0.0.2/src/optitrader/market/db/scripts/__init__.py
--rw-r--r--   0        0        0      743 2023-07-31 22:16:40.153937 optitrader-0.0.2/src/optitrader/market/db/scripts/add_asset.py
--rw-r--r--   0        0        0     1311 2023-07-31 22:25:43.054031 optitrader-0.0.2/src/optitrader/market/db/scripts/create_assets_table.py
--rw-r--r--   0        0        0      733 2023-07-31 22:16:35.747150 optitrader-0.0.2/src/optitrader/market/db/scripts/update_number_of_shares.py
--rw-r--r--   0        0        0     2830 2023-07-31 22:25:43.025856 optitrader-0.0.2/src/optitrader/market/finnhub_market_data.py
--rw-r--r--   0        0        0     3473 2023-07-31 22:25:42.994845 optitrader-0.0.2/src/optitrader/market/investment_universe.py
--rw-r--r--   0        0        0    14240 2023-07-31 22:25:42.966510 optitrader-0.0.2/src/optitrader/market/market_data.py
--rw-r--r--   0        0        0    14239 2023-07-31 22:16:39.723467 optitrader-0.0.2/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp
--rw-r--r--   0        0        0     3330 2023-07-31 22:25:42.927223 optitrader-0.0.2/src/optitrader/market/news.py
--rw-r--r--   0        0        0     4446 2023-07-31 22:25:42.888846 optitrader-0.0.2/src/optitrader/market/trading.py
--rw-r--r--   0        0        0     6381 2023-07-31 22:25:43.077120 optitrader-0.0.2/src/optitrader/market/yahoo_market_data.py
--rw-r--r--   0        0        0      270 2023-07-31 22:16:37.288605 optitrader-0.0.2/src/optitrader/models/__init__.py
--rw-r--r--   0        0        0     2112 2023-07-31 22:25:43.027353 optitrader-0.0.2/src/optitrader/models/asset.py
--rw-r--r--   0        0        0      243 2023-07-31 19:38:54.162170 optitrader-0.0.2/src/optitrader/models/base.py
--rw-r--r--   0        0        0     1962 2023-07-31 22:16:44.855769 optitrader-0.0.2/src/optitrader/models/optimization.py
--rw-r--r--   0        0        0     1962 2023-07-31 22:16:38.241893 optitrader-0.0.2/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp
--rw-r--r--   0        0        0       12 2023-07-31 19:38:54.193302 optitrader-0.0.2/src/optitrader/optimization/__init__.py
--rw-r--r--   0        0        0     7861 2023-07-31 22:25:42.975155 optitrader-0.0.2/src/optitrader/optimization/constraints.py
--rw-r--r--   0        0        0    12717 2023-07-31 22:25:42.953925 optitrader-0.0.2/src/optitrader/optimization/objectives.py
--rw-r--r--   0        0        0     6440 2023-07-31 22:25:42.902512 optitrader-0.0.2/src/optitrader/optimization/solver.py
--rw-r--r--   0        0        0     6510 2023-07-31 22:25:42.870039 optitrader-0.0.2/src/optitrader/portfolio.py
--rw-r--r--   0        0        0        0 2023-07-31 19:38:54.245739 optitrader-0.0.2/src/optitrader/py.typed
--rw-r--r--   0        0        0      203 2023-07-31 22:16:39.107081 optitrader-0.0.2/src/optitrader/utils/__init__.py
--rw-r--r--   0        0        0      953 2023-07-31 19:38:54.294727 optitrader-0.0.2/src/optitrader/utils/utils.py
--rw-r--r--   0        0        0     9610 1970-01-01 00:00:00.000000 optitrader-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-02 15:23:56.882993 optitrader-0.0.3/LICENSE
+-rw-r--r--   0        0        0     8749 2023-08-02 15:23:56.882993 optitrader-0.0.3/README.md
+-rw-r--r--   0        0        0     6611 2023-08-02 15:23:56.906993 optitrader-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/__init__.py
+-rw-r--r--   0        0        0     2239 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/api.py
+-rw-r--r--   0        0        0       87 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/1_🏠_Home.py
+-rw-r--r--   0        0        0      177 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/__init__.py
+-rw-r--r--   0        0        0      389 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/about.py
+-rw-r--r--   0        0        0      518 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/account.py
+-rw-r--r--   0        0        0     1187 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/backtester.py
+-rw-r--r--   0        0        0     3575 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/explore.py
+-rw-r--r--   0        0        0     1305 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/home.py
+-rw-r--r--   0        0        0     1129 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/page.py
+-rw-r--r--   0        0        0      105 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/2_📈_Backtester.py
+-rw-r--r--   0        0        0       96 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/3_🗺️_Explore.py
+-rw-r--r--   0        0        0       96 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/4_💼_Account.py
+-rw-r--r--   0        0        0       90 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/5_👨🏻‍💻_About.py
+-rw-r--r--   0        0        0       12 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/__init__.py
+-rw-r--r--   0        0        0    24191 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/session_manager.py
+-rw-r--r--   0        0        0    24190 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp
+-rw-r--r--   0        0        0     2621 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/backtester.py
+-rw-r--r--   0        0        0      469 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/cli.py
+-rw-r--r--   0        0        0     1556 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/config.py
+-rw-r--r--   0        0        0      422 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/backtester.py
+-rw-r--r--   0        0        0      736 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/iterable.py
+-rw-r--r--   0        0        0     1712 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/market.py
+-rw-r--r--   0        0        0      860 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/optimization.py
+-rw-r--r--   0        0        0     7356 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/main.py
+-rw-r--r--   0        0        0      231 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/__init__.py
+-rw-r--r--   0        0        0     8461 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py
+-rw-r--r--   0        0        0     8460 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp
+-rw-r--r--   0        0        0      768 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/base_data_provider.py
+-rw-r--r--   0        0        0       12 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/__init__.py
+-rw-r--r--   0        0        0     5339 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/database.py
+-rw-r--r--   0        0        0     5338 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp
+-rw-r--r--   0        0        0     1935 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/models.py
+-rw-r--r--   0        0        0       12 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/add_asset.py
+-rw-r--r--   0        0        0     1311 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/create_assets_table.py
+-rw-r--r--   0        0        0      733 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/update_number_of_shares.py
+-rw-r--r--   0        0        0     2830 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/finnhub_market_data.py
+-rw-r--r--   0        0        0     3473 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/investment_universe.py
+-rw-r--r--   0        0        0    14305 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/market_data.py
+-rw-r--r--   0        0        0    14239 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp
+-rw-r--r--   0        0        0     3330 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/news.py
+-rw-r--r--   0        0        0     4446 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/trading.py
+-rw-r--r--   0        0        0     6381 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/market/yahoo_market_data.py
+-rw-r--r--   0        0        0      270 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/__init__.py
+-rw-r--r--   0        0        0     2112 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/asset.py
+-rw-r--r--   0        0        0      243 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/base.py
+-rw-r--r--   0        0        0     1962 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/optimization.py
+-rw-r--r--   0        0        0     1962 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp
+-rw-r--r--   0        0        0       12 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/__init__.py
+-rw-r--r--   0        0        0     7861 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/constraints.py
+-rw-r--r--   0        0        0    12717 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/objectives.py
+-rw-r--r--   0        0        0     6440 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/solver.py
+-rw-r--r--   0        0        0     6510 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/portfolio.py
+-rw-r--r--   0        0        0        0 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/py.typed
+-rw-r--r--   0        0        0      203 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/utils/__init__.py
+-rw-r--r--   0        0        0      953 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/utils/utils.py
+-rw-r--r--   0        0        0    10040 1970-01-01 00:00:00.000000 optitrader-0.0.3/PKG-INFO
```

### Comparing `optitrader-0.0.2/LICENSE` & `optitrader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/README.md` & `optitrader-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+<div align="center">
+
+<h1> Optitrader </h1>
+
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://optitrader.streamlit.app/)
+[![Streamlit](https://img.shields.io/badge/Streamlit-1.24.0-FF4B4B.svg?style=flat&logo=Streamlit&logoColor=white)](https://streamlit.io)
+
 ![Build](https://github.com/Ale-Cas/optitrader/actions/workflows/test.yml/badge.svg)
 [![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![codecov](https://codecov.io/github/Ale-Cas/optitrader/branch/master/graph/badge.svg?token=F0COJXH0IJ)](https://codecov.io/github/Ale-Cas/optitrader)
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/Ale-Cas/optitrader)
-[![Streamlit](https://img.shields.io/badge/Streamlit-1.24.0-FF4B4B.svg?style=flat&logo=Streamlit&logoColor=white)](https://streamlit.io)
+
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Pydantic v1](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v1.json)](https://pydantic.dev)
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 [![FastAPI](https://img.shields.io/badge/FastAPI-0.63.0-009688.svg?style=flat&logo=FastAPI&logoColor=white)](https://fastapi.tiangolo.com)
+</div>
 
+Optitrader is an open-source Python package designed for portfolio optimization, quantitative finance, and algorithmic trading. It empowers users with a wide array of tools to effortlessly construct personalized portfolios, thoroughly analyze optimization outcomes, and seamlessly execute trades using [Alpaca's Trading API](https://alpaca.markets/docs/trading/).
 
-# optitrader
-
-## Description 
-
-optitrader is an open-source Python package for portfolio optimization and quantitative finance applications. 
-It is meant to provide a comprehensive suite of tools to easily build a custom portfolio, analyze the optimization results and it also supports the trade execution by leveraging [Alpaca's Trading API](https://alpaca.markets/docs/trading/).
+Accessible through an intuitive web-based [Streamlit](https://streamlit.io/) dashboard hosted at https://optitrader.streamlit.app, Optitrader enables users to interact with its rich features and harness the potential of portfolio optimization and algorithmic trade execution.
 
 ## Using
 
 _Python package_: to add and install this package as a dependency of your project, run `poetry add optitrader`.
 
 _Python CLI_: to view this app's CLI commands once it's installed, run `optitrader --help`.
 
@@ -59,15 +63,15 @@
         }
 )
 ```
 and you can use the available methods of the [Portfolio class](src/optitrader/portfolio.py), such as `pie_plot`:
 ```python
 optimal_ptf.pie_plot()
 ```
-![pie plot result](https://github.com/Ale-Cas/optitrader/assets/64859146/d369bdbf-f4dd-44b5-b8d8-8156604caec6)
+![pieplot](https://github.com/Ale-Cas/optitrader/assets/64859146/3728507d-8f5d-472e-8131-129e2d54c211)
 
 
 
 ## Contributing
 
 This project has been boostrapped using [this cookiecutter template](https://github.com/radix-ai/poetry-cookiecutter).
```

### Comparing `optitrader-0.0.2/pyproject.toml` & `optitrader-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "optitrader"
-version = "0.0.2"
+version = "0.0.3"
 description = "Optitrader is an opne-source Python package for portfolio optimization. "
 authors = ["Alessio Castrica <castricaalessio@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Ale-Cas/optitrader"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
```

### Comparing `optitrader-0.0.2/src/optitrader/api.py` & `optitrader-0.0.3/src/optitrader/api.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/account.py` & `optitrader-0.0.3/src/optitrader/app/account.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/backtester.py` & `optitrader-0.0.3/src/optitrader/app/backtester.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/explore.py` & `optitrader-0.0.3/src/optitrader/app/explore.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/home.py` & `optitrader-0.0.3/src/optitrader/app/home.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/page.py` & `optitrader-0.0.3/src/optitrader/app/page.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/session_manager.py` & `optitrader-0.0.3/src/optitrader/app/session_manager.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp` & `optitrader-0.0.3/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/backtester.py` & `optitrader-0.0.3/src/optitrader/backtester.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/config.py` & `optitrader-0.0.3/src/optitrader/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # ALPACA SETTINGS
     ALPACA_TRADING_API_KEY: str | None = None
     ALPACA_TRADING_API_SECRET: str | None = None
     ALPACA_BROKER_API_KEY: str | None = None
     ALPACA_BROKER_API_SECRET: str | None = None
 
     # FINNHUB
-    FINHUB_API_KEY: str
+    FINHUB_API_KEY: str | None = None
 
     # OPTIMIZATION SETTINGS
     # this means that if the portfolio's weights sum to 0.99 instead of 1 is accepted
     SUM_WEIGHTS_TOLERANCE: float = 1e-2
 
     # DB SETTINGS
     DB_URI_MARKET: str = "sqlite:///market.db"  # prod
```

### Comparing `optitrader-0.0.2/src/optitrader/enums/iterable.py` & `optitrader-0.0.3/src/optitrader/enums/iterable.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/enums/market.py` & `optitrader-0.0.3/src/optitrader/enums/market.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/enums/optimization.py` & `optitrader-0.0.3/src/optitrader/enums/optimization.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/main.py` & `optitrader-0.0.3/src/optitrader/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Main module for the optitrader class implementation."""
 
 import pandas as pd
 
+from optitrader.config import SETTINGS
 from optitrader.enums import UniverseName
 from optitrader.enums.market import BalanceSheetItem, CashFlowItem, IncomeStatementItem
 from optitrader.enums.optimization import ObjectiveName
 from optitrader.market import InvestmentUniverse, MarketData
 from optitrader.optimization.constraints import (
     NoShortSellConstraint,
     NumberOfAssetsConstraint,
@@ -38,14 +39,18 @@
     def __init__(
         self,
         objectives: list[PortfolioObjective],
         universe_name: UniverseName | None = None,
         tickers: tuple[str, ...] | None = None,
         constraints: list[PortfolioConstraint] | None = None,
         market_data: MarketData | None = None,
+        trading_key: str | None = SETTINGS.ALPACA_TRADING_API_KEY,
+        trading_secret: str | None = SETTINGS.ALPACA_TRADING_API_SECRET,
+        broker_key: str | None = SETTINGS.ALPACA_BROKER_API_KEY,
+        broker_secret: str | None = SETTINGS.ALPACA_BROKER_API_SECRET,
     ) -> None:
         """
         Initialize optitrader instance.
 
         Parameters
         ----------
         `objectives`: list[PortfolioObjective]
@@ -59,15 +64,23 @@
         `market_data`: MarketData | None = None
             The market data instance to get the data from,
             you can pass your own with your API keys and preferred data provider.
         """
         self.investment_universe = InvestmentUniverse(tickers=tickers, name=universe_name)
         self.objectives = objectives
         self.constraints = constraints or [SumToOneConstraint(), NoShortSellConstraint()]
-        self.market_data = market_data or MarketData()
+        assert (
+            market_data or (trading_key and trading_secret) or (broker_key and broker_secret)
+        ), "You must pass either a MarketData instance, the Trading API keys or Broker API keys."
+        self.market_data = market_data or MarketData(
+            trading_key=trading_key,
+            trading_secret=trading_secret,
+            broker_key=broker_key,
+            broker_secret=broker_secret,
+        )
 
     def add_constraint(self, constraint: PortfolioConstraint) -> None:
         """Add a constraint."""
         self.constraints.append(constraint)
 
     def add_objective(self, objective: PortfolioObjective) -> None:
         """Add an objective."""
```

### Comparing `optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py` & `optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp` & `optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/base_data_provider.py` & `optitrader-0.0.3/src/optitrader/market/base_data_provider.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/db/database.py` & `optitrader-0.0.3/src/optitrader/market/db/database.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp` & `optitrader-0.0.3/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/db/models.py` & `optitrader-0.0.3/src/optitrader/market/db/models.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/db/scripts/add_asset.py` & `optitrader-0.0.3/src/optitrader/market/db/scripts/add_asset.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/db/scripts/create_assets_table.py` & `optitrader-0.0.3/src/optitrader/market/db/scripts/create_assets_table.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/db/scripts/update_number_of_shares.py` & `optitrader-0.0.3/src/optitrader/market/db/scripts/update_number_of_shares.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/finnhub_market_data.py` & `optitrader-0.0.3/src/optitrader/market/finnhub_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/investment_universe.py` & `optitrader-0.0.3/src/optitrader/market/investment_universe.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/market_data.py` & `optitrader-0.0.3/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import asyncio
 import logging
 import time
 from functools import lru_cache
 
 import finnhub
 import pandas as pd
-
 from optitrader.config import SETTINGS
 from optitrader.enums import BarsField, DataProvider
 from optitrader.enums.market import BalanceSheetItem, CashFlowItem, IncomeStatementItem
 from optitrader.market.alpaca_market_data import AlpacaMarketData, Asset
 from optitrader.market.base_data_provider import BaseDataProvider
 from optitrader.market.db.database import MarketDB
 from optitrader.market.finnhub_market_data import FinnhubClient
```

### Comparing `optitrader-0.0.2/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp` & `optitrader-0.0.3/src/optitrader/market/market_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import logging
 import time
 from functools import lru_cache
 
 import finnhub
 import pandas as pd
+
 from optitrader.config import SETTINGS
 from optitrader.enums import BarsField, DataProvider
 from optitrader.enums.market import BalanceSheetItem, CashFlowItem, IncomeStatementItem
 from optitrader.market.alpaca_market_data import AlpacaMarketData, Asset
 from optitrader.market.base_data_provider import BaseDataProvider
 from optitrader.market.db.database import MarketDB
 from optitrader.market.finnhub_market_data import FinnhubClient
@@ -41,15 +42,15 @@
         self.__alpaca_client = AlpacaMarketData(
             trading_key=trading_key,
             trading_secret=trading_secret,
             broker_key=broker_key,
             broker_secret=broker_secret,
         )
         self.__yahoo_client = YahooMarketData()
-        self.__finnhub = FinnhubClient()
+        self.__finnhub = FinnhubClient() if SETTINGS.FINHUB_API_KEY else None
         provider_mapping: dict[DataProvider, BaseDataProvider] = {
             DataProvider.ALPACA: self.__alpaca_client,
             DataProvider.YAHOO: self.__yahoo_client,
         }
         self.__provider_client = provider_mapping[data_provider]
         self.use_db = use_db
         if self.use_db:
@@ -162,15 +163,15 @@
         Returns
         -------
         `asset`
             AssetModel data model.
         """
         duplicate_fields = set(_YahooFinnhubCommon.__fields__.keys())
         apca_asset = self.__alpaca_client.get_alpaca_asset(ticker)
-        finnhub_asset = self.__finnhub.get_asset_profile(ticker)
+        finnhub_asset = self.__finnhub.get_asset_profile(ticker) if self.__finnhub else None
         yahoo_asset = self.__yahoo_client.get_yahoo_asset(ticker)
         return AssetModel(
             **apca_asset.dict(exclude_none=True),
             **yahoo_asset.dict(
                 exclude=duplicate_fields,
                 exclude_none=True,
             )
```

### Comparing `optitrader-0.0.2/src/optitrader/market/news.py` & `optitrader-0.0.3/src/optitrader/market/news.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/trading.py` & `optitrader-0.0.3/src/optitrader/market/trading.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/market/yahoo_market_data.py` & `optitrader-0.0.3/src/optitrader/market/yahoo_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/models/asset.py` & `optitrader-0.0.3/src/optitrader/models/asset.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/models/optimization.py` & `optitrader-0.0.3/src/optitrader/models/optimization.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp` & `optitrader-0.0.3/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/optimization/constraints.py` & `optitrader-0.0.3/src/optitrader/optimization/constraints.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/optimization/objectives.py` & `optitrader-0.0.3/src/optitrader/optimization/objectives.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/optimization/solver.py` & `optitrader-0.0.3/src/optitrader/optimization/solver.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/portfolio.py` & `optitrader-0.0.3/src/optitrader/portfolio.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/src/optitrader/utils/utils.py` & `optitrader-0.0.3/src/optitrader/utils/utils.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.2/PKG-INFO` & `optitrader-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optitrader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Optitrader is an opne-source Python package for portfolio optimization. 
 Home-page: https://github.com/Ale-Cas/optitrader
 Author: Alessio Castrica
 Author-email: castricaalessio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -27,32 +27,36 @@
 Requires-Dist: typer[all] (>=0.9.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Requires-Dist: yahooquery (>=2.3.1,<3.0.0)
 Project-URL: Repository, https://github.com/Ale-Cas/optitrader
 Description-Content-Type: text/markdown
 
+<div align="center">
+
+<h1> Optitrader </h1>
+
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://optitrader.streamlit.app/)
+[![Streamlit](https://img.shields.io/badge/Streamlit-1.24.0-FF4B4B.svg?style=flat&logo=Streamlit&logoColor=white)](https://streamlit.io)
+
 ![Build](https://github.com/Ale-Cas/optitrader/actions/workflows/test.yml/badge.svg)
 [![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![codecov](https://codecov.io/github/Ale-Cas/optitrader/branch/master/graph/badge.svg?token=F0COJXH0IJ)](https://codecov.io/github/Ale-Cas/optitrader)
 [![Open in Dev Containers](https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/Ale-Cas/optitrader)
-[![Streamlit](https://img.shields.io/badge/Streamlit-1.24.0-FF4B4B.svg?style=flat&logo=Streamlit&logoColor=white)](https://streamlit.io)
+
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Pydantic v1](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v1.json)](https://pydantic.dev)
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 [![FastAPI](https://img.shields.io/badge/FastAPI-0.63.0-009688.svg?style=flat&logo=FastAPI&logoColor=white)](https://fastapi.tiangolo.com)
+</div>
 
+Optitrader is an open-source Python package designed for portfolio optimization, quantitative finance, and algorithmic trading. It empowers users with a wide array of tools to effortlessly construct personalized portfolios, thoroughly analyze optimization outcomes, and seamlessly execute trades using [Alpaca's Trading API](https://alpaca.markets/docs/trading/).
 
-# optitrader
-
-## Description 
-
-optitrader is an open-source Python package for portfolio optimization and quantitative finance applications. 
-It is meant to provide a comprehensive suite of tools to easily build a custom portfolio, analyze the optimization results and it also supports the trade execution by leveraging [Alpaca's Trading API](https://alpaca.markets/docs/trading/).
+Accessible through an intuitive web-based [Streamlit](https://streamlit.io/) dashboard hosted at https://optitrader.streamlit.app, Optitrader enables users to interact with its rich features and harness the potential of portfolio optimization and algorithmic trade execution.
 
 ## Using
 
 _Python package_: to add and install this package as a dependency of your project, run `poetry add optitrader`.
 
 _Python CLI_: to view this app's CLI commands once it's installed, run `optitrader --help`.
 
@@ -92,15 +96,15 @@
         }
 )
 ```
 and you can use the available methods of the [Portfolio class](src/optitrader/portfolio.py), such as `pie_plot`:
 ```python
 optimal_ptf.pie_plot()
 ```
-![pie plot result](https://github.com/Ale-Cas/optitrader/assets/64859146/d369bdbf-f4dd-44b5-b8d8-8156604caec6)
+![pieplot](https://github.com/Ale-Cas/optitrader/assets/64859146/3728507d-8f5d-472e-8131-129e2d54c211)
 
 
 
 ## Contributing
 
 This project has been boostrapped using [this cookiecutter template](https://github.com/radix-ai/poetry-cookiecutter).
```

