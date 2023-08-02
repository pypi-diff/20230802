# Comparing `tmp/browser-history-0.3.2.tar.gz` & `tmp/browser-history-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browser-history-0.3.2.tar", last modified: Thu Dec 16 15:09:34 2021, max compression
+gzip compressed data, was "browser-history-0.3.3.tar", last modified: Wed Aug  2 18:01:18 2023, max compression
```

## Comparing `browser-history-0.3.2.tar` & `browser-history-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 samyak    (1000) samyak    (1000)        0 2021-12-16 15:09:34.866088 browser-history-0.3.2/
--rw-r--r--   0 samyak    (1000) samyak    (1000)    11345 2021-12-16 13:54:54.000000 browser-history-0.3.2/LICENSE
--rw-rw-r--   0 samyak    (1000) samyak    (1000)     5656 2021-12-16 15:09:34.866088 browser-history-0.3.2/PKG-INFO
--rw-rw-r--   0 samyak    (1000) samyak    (1000)     4025 2021-12-16 14:59:23.000000 browser-history-0.3.2/README.md
-drwxrwxr-x   0 samyak    (1000) samyak    (1000)        0 2021-12-16 15:09:34.865088 browser-history-0.3.2/browser_history/
--rw-r--r--   0 samyak    (1000) samyak    (1000)     1999 2021-12-16 13:59:55.000000 browser-history-0.3.2/browser_history/__init__.py
--rw-r--r--   0 samyak    (1000) samyak    (1000)     6374 2021-12-16 13:59:55.000000 browser-history-0.3.2/browser_history/browsers.py
--rw-rw-r--   0 samyak    (1000) samyak    (1000)     8553 2021-12-16 14:59:23.000000 browser-history-0.3.2/browser_history/cli.py
--rw-r--r--   0 samyak    (1000) samyak    (1000)    25147 2021-12-16 13:59:55.000000 browser-history-0.3.2/browser_history/generic.py
--rw-r--r--   0 samyak    (1000) samyak    (1000)     6580 2021-12-16 13:59:55.000000 browser-history-0.3.2/browser_history/utils.py
-drwxrwxr-x   0 samyak    (1000) samyak    (1000)        0 2021-12-16 15:09:34.866088 browser-history-0.3.2/browser_history.egg-info/
--rw-rw-r--   0 samyak    (1000) samyak    (1000)     5656 2021-12-16 15:09:34.000000 browser-history-0.3.2/browser_history.egg-info/PKG-INFO
--rw-rw-r--   0 samyak    (1000) samyak    (1000)      399 2021-12-16 15:09:34.000000 browser-history-0.3.2/browser_history.egg-info/SOURCES.txt
--rw-rw-r--   0 samyak    (1000) samyak    (1000)        1 2021-12-16 15:09:34.000000 browser-history-0.3.2/browser_history.egg-info/dependency_links.txt
--rw-rw-r--   0 samyak    (1000) samyak    (1000)       62 2021-12-16 15:09:34.000000 browser-history-0.3.2/browser_history.egg-info/entry_points.txt
--rw-rw-r--   0 samyak    (1000) samyak    (1000)       16 2021-12-16 15:09:34.000000 browser-history-0.3.2/browser_history.egg-info/top_level.txt
--rw-rw-r--   0 samyak    (1000) samyak    (1000)        1 2021-12-16 14:45:58.000000 browser-history-0.3.2/browser_history.egg-info/zip-safe
--rw-rw-r--   0 samyak    (1000) samyak    (1000)     1334 2021-12-16 15:09:34.867088 browser-history-0.3.2/setup.cfg
--rw-r--r--   0 samyak    (1000) samyak    (1000)      865 2021-12-16 13:59:55.000000 browser-history-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:01:18.115404 browser-history-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-02 18:01:04.000000 browser-history-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-02 18:01:18.115404 browser-history-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-08-02 18:01:04.000000 browser-history-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:01:18.115404 browser-history-0.3.3/browser_history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-02 18:01:04.000000 browser-history-0.3.3/browser_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-08-02 18:01:04.000000 browser-history-0.3.3/browser_history/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-08-02 18:01:04.000000 browser-history-0.3.3/browser_history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-08-02 18:01:04.000000 browser-history-0.3.3/browser_history/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-08-02 18:01:04.000000 browser-history-0.3.3/browser_history/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:01:18.115404 browser-history-0.3.3/browser_history.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-08-02 18:01:18.000000 browser-history-0.3.3/browser_history.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-02 18:01:18.000000 browser-history-0.3.3/browser_history.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:01:18.000000 browser-history-0.3.3/browser_history.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 18:01:18.000000 browser-history-0.3.3/browser_history.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 18:01:18.000000 browser-history-0.3.3/browser_history.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:01:18.000000 browser-history-0.3.3/browser_history.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-02 18:01:18.115404 browser-history-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 18:01:04.000000 browser-history-0.3.3/setup.py
```

### Comparing `browser-history-0.3.2/LICENSE` & `browser-history-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `browser-history-0.3.2/PKG-INFO` & `browser-history-0.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 Metadata-Version: 2.1
 Name: browser-history
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python module to extract browser history
 Home-page: https://github.com/browser-history/browser-history
 Author: Samyak Sarnayak
 Author-email: samyak201@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://browser-history.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/browser-history/browser-history/
 Project-URL: Tracker, https://github.com/browser-history/browser-history/issues
-Description: <p align="center" width="100%">
-            <img width="33%" src="./logo.png">
-        </p>
-        
-        <h1 align="center"> browser-history</h1>
-        
-        ![tests](https://github.com/browser-history/browser-history/workflows/tests/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/browser-history/badge/?version=latest)](https://browser-history.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/browser-history.svg)](https://badge.fury.io/py/browser-history)
-        [![codecov](https://codecov.io/gh/browser-history/browser-history/branch/master/graph/badge.svg)](https://codecov.io/gh/browser-history/browser-history)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/64c86a28b0d7d387ce72/maintainability)](https://codeclimate.com/github/browser-history/browser-history/maintainability)
-        
-        ``browser-history`` is a simple, zero-dependencies, developer-friendly python
-        package to retrieve (almost) any browser's history on (almost) any platform.
-        
-        
-        ## Features
-        
-         - Supports most **popular browsers**. See [this](https://browser-history.readthedocs.io/en/latest/browsers.html) for a full list.
-         - Supports all major platforms - **Windows, Mac and Linux**.
-         - A **command-line tool**: simply run `browser-history --help` from your terminal.
-         - **History**: browsing history with exact timestamp and URL.
-         - **Bookmarks**: browser bookmarks with timestamp, URL, title and folder.
-         - Lightweight: the entire package is less than 20kB in size and has no dependencies other than python 3.6+.
-         - Developer friendly: you can add support for new browsers or add a new feature very easily.
-         - Default browser: can automatically determine the default browser on Windows and Linux (`browser-history -b default`).
-         - Fully open source: this project is developed and maintained by the [`browser-history` organization](https://github.com/browser-history) (previously maintained by [PESOS](https://github.com/pesos)) and will always be open source (with the Apache 2.0 License).
-        
-        # Quick Start
-        
-        ## Installation
-        
-        To install the latest release:
-        
-        ```
-        pip install browser-history
-        ```
-        
-        To install from the master branch (warning: development version. Things could break)
-        
-        ```
-        pip install git+https://github.com/browser-history/browser-history.git
-        ```
-        
-        ## Usage
-        
-        ### History
-        
-        To get history from all installed browsers:
-        ```python
-        from browser_history import get_history
-        
-        outputs = get_history()
-        
-        # his is a list of (datetime.datetime, url) tuples
-        his = outputs.histories
-        ```
-        
-        If you want history from a specific browser:
-        ```python
-        from browser_history.browsers import Firefox
-        
-        f = Firefox()
-        outputs = f.fetch_history()
-        
-        # his is a list of (datetime.datetime, url) tuples
-        his = outputs.histories
-        ```
-        
-         - `Firefox` in the above snippet can be replaced with any of the [supported browsers](https://browser-history.readthedocs.io/en/latest/browsers.html).
-        
-        ### Bookmarks
-        
-        WARNING: Experimental feature. Although this has been confirmed to work on multiple (Firefox and Chromium based) browsers
-        on all platforms, it is not covered by tests and has not been used as much as the history feature.
-        
-        To get bookmarks from all installed browsers:
-        ```python
-        from browser_history import get_bookmarks
-        
-        outputs = get_bookmarks()
-        
-        # bms is a list of (datetime.datetime, url, title, folder) tuples
-        bms = outputs.bookmarks
-        ```
-        
-        To get bookmarks from a specific browser:
-        ```python
-        from browser_history.browsers import Firefox
-        
-        f = Firefox()
-        outputs = f.fetch_bookmarks()
-        
-        # bms is a list of (datetime.datetime, url, title, folder) tuples
-        bms = outputs.bookmarks
-        ```
-        
-        Check out the [documentation](https://browser-history.readthedocs.io/en/latest/) for more details.
-        
-        # Supported Browsers
-        
-        Read the [documentation](https://browser-history.readthedocs.io/en/latest/browsers.html)
-        
-        # Credits
-        
-        Logo designed with :heart: by [XA](https://github.com/XAMES3).
-        
-        # License
-        
-        Licensed under the [Apache License, Version 2.0 (the "License")](LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center" width="100%">
+    <img width="33%" src="https://github.com/browser-history/browser-history/blob/master/logo.png?raw=true">
+</p>
+
+<h1 align="center"> browser-history</h1>
+
+![tests](https://github.com/browser-history/browser-history/workflows/tests/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/browser-history/badge/?version=latest)](https://browser-history.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/browser-history.svg)](https://badge.fury.io/py/browser-history)
+[![codecov](https://codecov.io/gh/browser-history/browser-history/branch/master/graph/badge.svg)](https://codecov.io/gh/browser-history/browser-history)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Maintainability](https://api.codeclimate.com/v1/badges/64c86a28b0d7d387ce72/maintainability)](https://codeclimate.com/github/browser-history/browser-history/maintainability)
+
+``browser-history`` is a simple, zero-dependencies, developer-friendly python
+package to retrieve (almost) any browser's history on (almost) any platform.
+
+
+## Features
+
+ - Supports most **popular browsers**. See [this](https://browser-history.readthedocs.io/en/latest/browsers.html) for a full list.
+ - Supports all major platforms - **Windows, Mac and Linux**.
+ - A **command-line tool**: simply run `browser-history --help` from your terminal.
+ - **History**: browsing history with exact timestamp and URL.
+ - **Bookmarks**: browser bookmarks with timestamp, URL, title and folder.
+ - Lightweight: the entire package is less than 20kB in size and has no dependencies other than python 3.7+.
+ - Developer friendly: you can add support for new browsers or add a new feature very easily.
+ - Default browser: can automatically determine the default browser on Windows and Linux (`browser-history -b default`).
+ - Fully open source: this project is developed and maintained by the [`browser-history` organization](https://github.com/browser-history) (previously maintained by [PESOS](https://github.com/pesos)) and will always be open source (with the Apache 2.0 License).
+
+# Quick Start
+
+## Installation
+
+To install the latest release:
+
+```
+pip install browser-history
+```
+
+To install from the master branch (warning: development version. Things could break)
+
+```
+pip install git+https://github.com/browser-history/browser-history.git
+```
+
+## Usage
+
+### History
+
+To get history from all installed browsers:
+```python
+from browser_history import get_history
+
+outputs = get_history()
+
+# his is a list of (datetime.datetime, url) tuples
+his = outputs.histories
+```
+
+If you want history from a specific browser:
+```python
+from browser_history.browsers import Firefox
+
+f = Firefox()
+outputs = f.fetch_history()
+
+# his is a list of (datetime.datetime, url) tuples
+his = outputs.histories
+```
+
+ - `Firefox` in the above snippet can be replaced with any of the [supported browsers](https://browser-history.readthedocs.io/en/latest/browsers.html).
+
+### Bookmarks
+
+WARNING: Experimental feature. Although this has been confirmed to work on multiple (Firefox and Chromium based) browsers
+on all platforms, it is not covered by tests and has not been used as much as the history feature.
+
+To get bookmarks from all installed browsers:
+```python
+from browser_history import get_bookmarks
+
+outputs = get_bookmarks()
+
+# bms is a list of (datetime.datetime, url, title, folder) tuples
+bms = outputs.bookmarks
+```
+
+To get bookmarks from a specific browser:
+```python
+from browser_history.browsers import Firefox
+
+f = Firefox()
+outputs = f.fetch_bookmarks()
+
+# bms is a list of (datetime.datetime, url, title, folder) tuples
+bms = outputs.bookmarks
+```
+
+Check out the [documentation](https://browser-history.readthedocs.io/en/latest/) for more details.
+
+# Supported Browsers
+
+Read the [documentation](https://browser-history.readthedocs.io/en/latest/browsers.html)
+
+# Credits
+
+Logo designed with :heart: by [XA](https://github.com/XAMES3).
+
+# License
+
+Licensed under the [Apache License, Version 2.0 (the "License")](LICENSE)
```

### Comparing `browser-history-0.3.2/README.md` & `browser-history-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center" width="100%">
-    <img width="33%" src="./logo.png">
+    <img width="33%" src="https://github.com/browser-history/browser-history/blob/master/logo.png?raw=true">
 </p>
 
 <h1 align="center"> browser-history</h1>
 
 ![tests](https://github.com/browser-history/browser-history/workflows/tests/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/browser-history/badge/?version=latest)](https://browser-history.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/browser-history.svg)](https://badge.fury.io/py/browser-history)
@@ -18,15 +18,15 @@
 ## Features
 
  - Supports most **popular browsers**. See [this](https://browser-history.readthedocs.io/en/latest/browsers.html) for a full list.
  - Supports all major platforms - **Windows, Mac and Linux**.
  - A **command-line tool**: simply run `browser-history --help` from your terminal.
  - **History**: browsing history with exact timestamp and URL.
  - **Bookmarks**: browser bookmarks with timestamp, URL, title and folder.
- - Lightweight: the entire package is less than 20kB in size and has no dependencies other than python 3.6+.
+ - Lightweight: the entire package is less than 20kB in size and has no dependencies other than python 3.7+.
  - Developer friendly: you can add support for new browsers or add a new feature very easily.
  - Default browser: can automatically determine the default browser on Windows and Linux (`browser-history -b default`).
  - Fully open source: this project is developed and maintained by the [`browser-history` organization](https://github.com/browser-history) (previously maintained by [PESOS](https://github.com/pesos)) and will always be open source (with the Apache 2.0 License).
 
 # Quick Start
 
 ## Installation
```

### Comparing `browser-history-0.3.2/browser_history/__init__.py` & `browser-history-0.3.3/browser_history/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from . import browsers, generic, utils  # noqa: F401
 
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 
 def get_history():
     """This method is used to obtain browser histories of all available and
     supported browsers for the system platform.
 
     :return: Object of class :py:class:`browser_history.generic.Outputs` with
```

### Comparing `browser-history-0.3.2/browser_history/browsers.py` & `browser-history-0.3.3/browser_history/browsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
                 ),
                 url,
                 title,
                 folder,
             )
             for d, url, title, folder in cursor.fetchall()
         ]
+        conn.close()
         return date_bookmarks
 
 
 class LibreWolf(Firefox):
     """LibreWolf Browser
 
     Supported platforms:
```

### Comparing `browser-history-0.3.2/browser_history/cli.py` & `browser-history-0.3.3/browser_history/cli.py`

 * *Files identical despite different names*

### Comparing `browser-history-0.3.2/browser_history/generic.py` & `browser-history-0.3.3/browser_history/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         with tempfile.TemporaryDirectory() as tmpdirname:
             for bookmarks_path in bookmarks_paths:
                 if not os.path.exists(bookmarks_path):
                     continue
                 copied_bookmark_path = shutil.copy2(
                     bookmarks_path.absolute(), tmpdirname
                 )
-                date_bookmarks = self.bookmarks_parser(copied_bookmark_path)
+                date_bookmarks = self.bookmarks_parser(copied_bookmark_path)  # pylint: disable=assignment-from-no-return
                 output_object.bookmarks.extend(date_bookmarks)
             if sort:
                 output_object.bookmarks.sort(reverse=desc)
         return output_object
 
     @classmethod
     def is_supported(cls):
@@ -636,14 +636,14 @@
                     break
                 else:
                     bookmarks_list = _deeper(
                         bookmarks_json[node], folder, bookmarks_list
                     )
             return bookmarks_list
 
-        with open(bookmark_path) as b_p:
+        with open(bookmark_path, "rb") as b_p:
             b_m = json.load(b_p)
             bookmarks_list = []
             for root in b_m["roots"]:
                 if isinstance(b_m["roots"][root], dict):
                     bookmarks_list = _deeper(b_m["roots"][root], root, bookmarks_list)
         return bookmarks_list
```

### Comparing `browser-history-0.3.2/browser_history/utils.py` & `browser-history-0.3.3/browser_history/utils.py`

 * *Files identical despite different names*

### Comparing `browser-history-0.3.2/browser_history.egg-info/PKG-INFO` & `browser-history-0.3.3/browser_history.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 Metadata-Version: 2.1
 Name: browser-history
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python module to extract browser history
 Home-page: https://github.com/browser-history/browser-history
 Author: Samyak Sarnayak
 Author-email: samyak201@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://browser-history.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/browser-history/browser-history/
 Project-URL: Tracker, https://github.com/browser-history/browser-history/issues
-Description: <p align="center" width="100%">
-            <img width="33%" src="./logo.png">
-        </p>
-        
-        <h1 align="center"> browser-history</h1>
-        
-        ![tests](https://github.com/browser-history/browser-history/workflows/tests/badge.svg)
-        [![Documentation Status](https://readthedocs.org/projects/browser-history/badge/?version=latest)](https://browser-history.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI version](https://badge.fury.io/py/browser-history.svg)](https://badge.fury.io/py/browser-history)
-        [![codecov](https://codecov.io/gh/browser-history/browser-history/branch/master/graph/badge.svg)](https://codecov.io/gh/browser-history/browser-history)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/64c86a28b0d7d387ce72/maintainability)](https://codeclimate.com/github/browser-history/browser-history/maintainability)
-        
-        ``browser-history`` is a simple, zero-dependencies, developer-friendly python
-        package to retrieve (almost) any browser's history on (almost) any platform.
-        
-        
-        ## Features
-        
-         - Supports most **popular browsers**. See [this](https://browser-history.readthedocs.io/en/latest/browsers.html) for a full list.
-         - Supports all major platforms - **Windows, Mac and Linux**.
-         - A **command-line tool**: simply run `browser-history --help` from your terminal.
-         - **History**: browsing history with exact timestamp and URL.
-         - **Bookmarks**: browser bookmarks with timestamp, URL, title and folder.
-         - Lightweight: the entire package is less than 20kB in size and has no dependencies other than python 3.6+.
-         - Developer friendly: you can add support for new browsers or add a new feature very easily.
-         - Default browser: can automatically determine the default browser on Windows and Linux (`browser-history -b default`).
-         - Fully open source: this project is developed and maintained by the [`browser-history` organization](https://github.com/browser-history) (previously maintained by [PESOS](https://github.com/pesos)) and will always be open source (with the Apache 2.0 License).
-        
-        # Quick Start
-        
-        ## Installation
-        
-        To install the latest release:
-        
-        ```
-        pip install browser-history
-        ```
-        
-        To install from the master branch (warning: development version. Things could break)
-        
-        ```
-        pip install git+https://github.com/browser-history/browser-history.git
-        ```
-        
-        ## Usage
-        
-        ### History
-        
-        To get history from all installed browsers:
-        ```python
-        from browser_history import get_history
-        
-        outputs = get_history()
-        
-        # his is a list of (datetime.datetime, url) tuples
-        his = outputs.histories
-        ```
-        
-        If you want history from a specific browser:
-        ```python
-        from browser_history.browsers import Firefox
-        
-        f = Firefox()
-        outputs = f.fetch_history()
-        
-        # his is a list of (datetime.datetime, url) tuples
-        his = outputs.histories
-        ```
-        
-         - `Firefox` in the above snippet can be replaced with any of the [supported browsers](https://browser-history.readthedocs.io/en/latest/browsers.html).
-        
-        ### Bookmarks
-        
-        WARNING: Experimental feature. Although this has been confirmed to work on multiple (Firefox and Chromium based) browsers
-        on all platforms, it is not covered by tests and has not been used as much as the history feature.
-        
-        To get bookmarks from all installed browsers:
-        ```python
-        from browser_history import get_bookmarks
-        
-        outputs = get_bookmarks()
-        
-        # bms is a list of (datetime.datetime, url, title, folder) tuples
-        bms = outputs.bookmarks
-        ```
-        
-        To get bookmarks from a specific browser:
-        ```python
-        from browser_history.browsers import Firefox
-        
-        f = Firefox()
-        outputs = f.fetch_bookmarks()
-        
-        # bms is a list of (datetime.datetime, url, title, folder) tuples
-        bms = outputs.bookmarks
-        ```
-        
-        Check out the [documentation](https://browser-history.readthedocs.io/en/latest/) for more details.
-        
-        # Supported Browsers
-        
-        Read the [documentation](https://browser-history.readthedocs.io/en/latest/browsers.html)
-        
-        # Credits
-        
-        Logo designed with :heart: by [XA](https://github.com/XAMES3).
-        
-        # License
-        
-        Licensed under the [Apache License, Version 2.0 (the "License")](LICENSE)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center" width="100%">
+    <img width="33%" src="https://github.com/browser-history/browser-history/blob/master/logo.png?raw=true">
+</p>
+
+<h1 align="center"> browser-history</h1>
+
+![tests](https://github.com/browser-history/browser-history/workflows/tests/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/browser-history/badge/?version=latest)](https://browser-history.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/browser-history.svg)](https://badge.fury.io/py/browser-history)
+[![codecov](https://codecov.io/gh/browser-history/browser-history/branch/master/graph/badge.svg)](https://codecov.io/gh/browser-history/browser-history)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Maintainability](https://api.codeclimate.com/v1/badges/64c86a28b0d7d387ce72/maintainability)](https://codeclimate.com/github/browser-history/browser-history/maintainability)
+
+``browser-history`` is a simple, zero-dependencies, developer-friendly python
+package to retrieve (almost) any browser's history on (almost) any platform.
+
+
+## Features
+
+ - Supports most **popular browsers**. See [this](https://browser-history.readthedocs.io/en/latest/browsers.html) for a full list.
+ - Supports all major platforms - **Windows, Mac and Linux**.
+ - A **command-line tool**: simply run `browser-history --help` from your terminal.
+ - **History**: browsing history with exact timestamp and URL.
+ - **Bookmarks**: browser bookmarks with timestamp, URL, title and folder.
+ - Lightweight: the entire package is less than 20kB in size and has no dependencies other than python 3.7+.
+ - Developer friendly: you can add support for new browsers or add a new feature very easily.
+ - Default browser: can automatically determine the default browser on Windows and Linux (`browser-history -b default`).
+ - Fully open source: this project is developed and maintained by the [`browser-history` organization](https://github.com/browser-history) (previously maintained by [PESOS](https://github.com/pesos)) and will always be open source (with the Apache 2.0 License).
+
+# Quick Start
+
+## Installation
+
+To install the latest release:
+
+```
+pip install browser-history
+```
+
+To install from the master branch (warning: development version. Things could break)
+
+```
+pip install git+https://github.com/browser-history/browser-history.git
+```
+
+## Usage
+
+### History
+
+To get history from all installed browsers:
+```python
+from browser_history import get_history
+
+outputs = get_history()
+
+# his is a list of (datetime.datetime, url) tuples
+his = outputs.histories
+```
+
+If you want history from a specific browser:
+```python
+from browser_history.browsers import Firefox
+
+f = Firefox()
+outputs = f.fetch_history()
+
+# his is a list of (datetime.datetime, url) tuples
+his = outputs.histories
+```
+
+ - `Firefox` in the above snippet can be replaced with any of the [supported browsers](https://browser-history.readthedocs.io/en/latest/browsers.html).
+
+### Bookmarks
+
+WARNING: Experimental feature. Although this has been confirmed to work on multiple (Firefox and Chromium based) browsers
+on all platforms, it is not covered by tests and has not been used as much as the history feature.
+
+To get bookmarks from all installed browsers:
+```python
+from browser_history import get_bookmarks
+
+outputs = get_bookmarks()
+
+# bms is a list of (datetime.datetime, url, title, folder) tuples
+bms = outputs.bookmarks
+```
+
+To get bookmarks from a specific browser:
+```python
+from browser_history.browsers import Firefox
+
+f = Firefox()
+outputs = f.fetch_bookmarks()
+
+# bms is a list of (datetime.datetime, url, title, folder) tuples
+bms = outputs.bookmarks
+```
+
+Check out the [documentation](https://browser-history.readthedocs.io/en/latest/) for more details.
+
+# Supported Browsers
+
+Read the [documentation](https://browser-history.readthedocs.io/en/latest/browsers.html)
+
+# Credits
+
+Logo designed with :heart: by [XA](https://github.com/XAMES3).
+
+# License
+
+Licensed under the [Apache License, Version 2.0 (the "License")](LICENSE)
```

### Comparing `browser-history-0.3.2/setup.cfg` & `browser-history-0.3.3/setup.cfg`

 * *Files identical despite different names*

