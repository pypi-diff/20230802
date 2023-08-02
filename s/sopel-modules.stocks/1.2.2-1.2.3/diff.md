# Comparing `tmp/sopel_modules.stocks-1.2.2.tar.gz` & `tmp/sopel_modules.stocks-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules.stocks-1.2.2.tar", last modified: Sat Jul 22 01:33:56 2023, max compression
+gzip compressed data, was "sopel_modules.stocks-1.2.3.tar", last modified: Wed Aug  2 18:28:10 2023, max compression
```

## Comparing `sopel_modules.stocks-1.2.2.tar` & `sopel_modules.stocks-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/NEWS
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules/stocks/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/alphavantage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/iexcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/sopel_modules/stocks/stocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-22 01:33:56.000000 sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:33:56.377245 sopel_modules.stocks-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-22 01:33:45.000000 sopel_modules.stocks-1.2.2/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/sopel_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/sopel_modules/stocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/stocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/alphavantage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/finnhub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/iexcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/sopel_modules/stocks/stocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-02 18:28:10.000000 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-02 18:28:10.000000 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:28:10.000000 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 18:28:10.000000 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 18:28:10.000000 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 18:28:10.000000 sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:10.977637 sopel_modules.stocks-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:27:57.000000 sopel_modules.stocks-1.2.3/tests/requirements.txt
```

### Comparing `sopel_modules.stocks-1.2.2/LICENSE` & `sopel_modules.stocks-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sopel_modules.stocks-1.2.2/PKG-INFO` & `sopel_modules.stocks-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel_modules.stocks
-Version: 1.2.2
+Version: 1.2.3
 Summary: Sopel Stocks Plugin
 Home-page: http://github.com/rustybower/sopel-stocks
 Author: Rusty Bower
 Author-email: rusty@rustybower.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -37,21 +37,22 @@
 ## Configuring
 You can automatically configure this plugin using the `sopel configure --plugins` command.
 
 However, if you want or need to configure this plugin manually, you will need to define the following in `~/.sopel/default.cfg`
 
     [stocks]
     api_key = API_KEY
-    provider = alphavantage (or iexcloud)
+    provider = finnhub (or alphavantage/iexcloud)
 
 ## Requirements
 #### API Key (from 1 of the following providers)
 
     https://www.alphavantage.co/support/#api-key
     https://iexcloud.io/console/tokens
+    https://finnhub.io/dashboard (recommended)
 
 #### Python Requirements
 
     requests
     sopel
 
 ## Usage
```

### Comparing `sopel_modules.stocks-1.2.2/README.md` & `sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: sopel-modules.stocks
+Version: 1.2.3
+Summary: Sopel Stocks Plugin
+Home-page: http://github.com/rustybower/sopel-stocks
+Author: Rusty Bower
+Author-email: rusty@rustybower.com
+License: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Python Tests](https://github.com/sopel-irc/sopel-stocks/actions/workflows/python-tests.yml/badge.svg?branch=master)](https://github.com/sopel-irc/sopel-stocks/actions/workflows/python-tests.yml)
 [![PyPI version](https://badge.fury.io/py/sopel-modules.stocks.svg)](https://badge.fury.io/py/sopel-modules.stocks)
 [![Total alerts](https://img.shields.io/lgtm/alerts/g/sopel-irc/sopel-stocks.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sopel-irc/sopel-stocks/alerts/)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/sopel-irc/sopel-stocks.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sopel-irc/sopel-stocks/context:python)
 
 **Maintainer:** [@RustyBower](https://github.com/rustybower)
 
@@ -26,21 +37,22 @@
 ## Configuring
 You can automatically configure this plugin using the `sopel configure --plugins` command.
 
 However, if you want or need to configure this plugin manually, you will need to define the following in `~/.sopel/default.cfg`
 
     [stocks]
     api_key = API_KEY
-    provider = alphavantage (or iexcloud)
+    provider = finnhub (or alphavantage/iexcloud)
 
 ## Requirements
 #### API Key (from 1 of the following providers)
 
     https://www.alphavantage.co/support/#api-key
     https://iexcloud.io/console/tokens
+    https://finnhub.io/dashboard (recommended)
 
 #### Python Requirements
 
     requests
     sopel
 
 ## Usage
@@ -48,7 +60,9 @@
     .stock msft
     <sopel> MSFT $123.37 1.6 (1.31%)⬆
 
     .stock aapl amzn goog
     <sopel> AAPL $150.83 -2.51 (-1.64%)⬇
     <sopel> AMZN $97.06 -5.38 (-5.25%)⬇
     <sopel> GOOG $90.445 -4.215 (-4.45%)⬇
+
+
```

### Comparing `sopel_modules.stocks-1.2.2/setup.py` & `sopel_modules.stocks-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 with open('tests/requirements.txt') as dev_requirements_file:
     dev_requirements = [req for req in dev_requirements_file.readlines()]
 
 
 setup(
     name='sopel_modules.stocks',
-    version='1.2.2',
+    version='1.2.3',
     description='Sopel Stocks Plugin',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',  # This is important!
     author='Rusty Bower',
     author_email='rusty@rustybower.com',
     url='http://github.com/rustybower/sopel-stocks',
     packages=find_packages('.'),
```

### Comparing `sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/alphavantage.py` & `sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/alphavantage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding=utf-8
 import requests
 
 
 def alphavantage(bot, symbol):
     r = requests.get(
-        "https://www.alphavantage.co/query?function=TIME_SERIES_INTRADAY&symbol={symbol}&apikey={api_key}".format(
+        "https://www.alphavantage.co/query?function=TIME_SERIES_DAILY&symbol={symbol}&apikey={api_key}".format(
             symbol=symbol, api_key=bot.config.stocks.api_key
         )
     )
 
     if not r.json():
         raise Exception("An error occurred.")
```

### Comparing `sopel_modules.stocks-1.2.2/sopel_modules/stocks/providers/iexcloud.py` & `sopel_modules.stocks-1.2.3/sopel_modules/stocks/providers/iexcloud.py`

 * *Files identical despite different names*

### Comparing `sopel_modules.stocks-1.2.2/sopel_modules/stocks/stocks.py` & `sopel_modules.stocks-1.2.3/sopel_modules/stocks/stocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from sopel.config.types import NO_DEFAULT, ChoiceAttribute, StaticSection, ValidatedAttribute
 from sopel.formatting import color, colors
 from sopel.logger import get_logger
 from sopel.module import commands, example
 
 from .providers.alphavantage import alphavantage
 from .providers.iexcloud import iexcloud
+from .providers.finnhub import finnhub
 
 logger = get_logger(__name__)
 
 
 STOCK_PROVIDERS = [
     'alphavantage',
     'iexcloud',
+    'finnhub',
 ]
 
 
 # Define our sopel stocks configuration
 class StocksSection(StaticSection):
     provider = ChoiceAttribute(
         'provider',
@@ -53,14 +55,17 @@
 def get_price(bot, symbol):
     # Alphavantage
     if bot.config.stocks.provider == 'alphavantage':
         return alphavantage(bot, symbol)
     # IEX Cloud
     elif bot.config.stocks.provider == 'iexcloud':
         return iexcloud(bot, symbol)
+    # IEX Cloud
+    elif bot.config.stocks.provider == 'finnhub':
+        return finnhub(bot, symbol)
     # Unsupported Provider
     else:
         raise Exception('Error: Unsupported Provider')
 
 
 @commands('stock')
 @example('.stock msft')
```

### Comparing `sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/PKG-INFO` & `sopel_modules.stocks-1.2.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: sopel-modules.stocks
-Version: 1.2.2
-Summary: Sopel Stocks Plugin
-Home-page: http://github.com/rustybower/sopel-stocks
-Author: Rusty Bower
-Author-email: rusty@rustybower.com
-License: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python Tests](https://github.com/sopel-irc/sopel-stocks/actions/workflows/python-tests.yml/badge.svg?branch=master)](https://github.com/sopel-irc/sopel-stocks/actions/workflows/python-tests.yml)
 [![PyPI version](https://badge.fury.io/py/sopel-modules.stocks.svg)](https://badge.fury.io/py/sopel-modules.stocks)
 [![Total alerts](https://img.shields.io/lgtm/alerts/g/sopel-irc/sopel-stocks.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sopel-irc/sopel-stocks/alerts/)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/sopel-irc/sopel-stocks.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/sopel-irc/sopel-stocks/context:python)
 
 **Maintainer:** [@RustyBower](https://github.com/rustybower)
 
@@ -37,21 +26,22 @@
 ## Configuring
 You can automatically configure this plugin using the `sopel configure --plugins` command.
 
 However, if you want or need to configure this plugin manually, you will need to define the following in `~/.sopel/default.cfg`
 
     [stocks]
     api_key = API_KEY
-    provider = alphavantage (or iexcloud)
+    provider = finnhub (or alphavantage/iexcloud)
 
 ## Requirements
 #### API Key (from 1 of the following providers)
 
     https://www.alphavantage.co/support/#api-key
     https://iexcloud.io/console/tokens
+    https://finnhub.io/dashboard (recommended)
 
 #### Python Requirements
 
     requests
     sopel
 
 ## Usage
@@ -59,9 +49,7 @@
     .stock msft
     <sopel> MSFT $123.37 1.6 (1.31%)⬆
 
     .stock aapl amzn goog
     <sopel> AAPL $150.83 -2.51 (-1.64%)⬇
     <sopel> AMZN $97.06 -5.38 (-5.25%)⬇
     <sopel> GOOG $90.445 -4.215 (-4.45%)⬇
-
-
```

### Comparing `sopel_modules.stocks-1.2.2/sopel_modules.stocks.egg-info/SOURCES.txt` & `sopel_modules.stocks-1.2.3/sopel_modules.stocks.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 sopel_modules.stocks.egg-info/namespace_packages.txt
 sopel_modules.stocks.egg-info/requires.txt
 sopel_modules.stocks.egg-info/top_level.txt
 sopel_modules/stocks/__init__.py
 sopel_modules/stocks/stocks.py
 sopel_modules/stocks/providers/__init__.py
 sopel_modules/stocks/providers/alphavantage.py
+sopel_modules/stocks/providers/finnhub.py
 sopel_modules/stocks/providers/iexcloud.py
 tests/requirements.txt
```

