# Comparing `tmp/fake-useragent-1.1.3.tar.gz` & `tmp/fake-useragent-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake-useragent-1.1.3.tar", last modified: Mon Mar 20 20:37:34 2023, max compression
+gzip compressed data, was "fake-useragent-1.2.0.tar", last modified: Wed Aug  2 00:03:38 2023, max compression
```

## Comparing `fake-useragent-1.1.3.tar` & `fake-useragent-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:37:34.035967 fake-useragent-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-03-20 20:37:34.035967 fake-useragent-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 20:37:34.035967 fake-useragent-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:37:34.027967 fake-useragent-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:37:34.031967 fake-useragent-1.1.3/src/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:37:34.031967 fake-useragent-1.1.3/src/fake_useragent/data/
--rw-r--r--   0 runner    (1001) docker     (123)   441951 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/data/browsers.json
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/src/fake_useragent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:37:34.031967 fake-useragent-1.1.3/src/fake_useragent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-03-20 20:37:34.000000 fake-useragent-1.1.3/src/fake_useragent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-20 20:37:34.000000 fake-useragent-1.1.3/src/fake_useragent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 20:37:34.000000 fake-useragent-1.1.3/src/fake_useragent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 20:37:33.000000 fake-useragent-1.1.3/src/fake_useragent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-20 20:37:34.000000 fake-useragent-1.1.3/src/fake_useragent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-20 20:37:34.000000 fake-useragent-1.1.3/src/fake_useragent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:37:34.035967 fake-useragent-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-03-20 20:37:22.000000 fake-useragent-1.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/fake_useragent/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/data/browsers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/fake_useragent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:03:37.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/tests/test_utils.py
```

### Comparing `fake-useragent-1.1.3/LICENSE` & `fake-useragent-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fake-useragent-1.1.3/PKG-INFO` & `fake-useragent-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-useragent
-Version: 1.1.3
+Version: 1.2.0
 Summary: Up-to-date simple useragent faker with real world database
 Author-email: Victor Kovtun <hellysmile@gmail.com>, Melroy van den Berg <melroy@melroy.org>
 Project-URL: Homepage, https://github.com/fake-useragent/fake-useragent
 Keywords: user,agent,user agent,useragent,fake,fake useragent,fake user agent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,22 +23,21 @@
 License-File: LICENSE
 License-File: AUTHORS
 
 [![Test & Deploy fake-useragent](https://github.com/fake-useragent/fake-useragent/actions/workflows/action.yml/badge.svg?branch=master)](https://github.com/fake-useragent/fake-useragent/actions/workflows/action.yml?query=branch%3Amaster)
 
 # fake-useragent
 
-Up-to-date simple useragent faker with real world database
+Up-to-date simple useragent faker with real world database.
 
 ## Features
 
-- Data is pre-downloaded from [useragentstring.com](http://useragentstring.com/) and part of the package
+- Data is pre-downloaded from [techblog.willshouse.com](https://techblog.willshouse.com/2012/01/03/most-common-user-agents/) and the data is part of the package
 - Retrieves user-agent strings locally
 - Supports Python 3.x
-- _Fallback_ to external resource ([useragentstring.com](http://useragentstring.com/)) + caching
 
 ### Installation
 
 ```sh
 pip install fake-useragent
 ```
 
@@ -46,103 +45,97 @@
 
 ```sh
 pip3 install fake-useragent
 ```
 
 ### Usage
 
+Simple usage example, see below for more examples:
+
 ```py
 from fake_useragent import UserAgent
 ua = UserAgent()
 
-ua.ie
-# Mozilla/5.0 (Windows; U; MSIE 9.0; Windows NT 9.0; en-US);
-ua.msie
-# Mozilla/5.0 (compatible; MSIE 10.0; Macintosh; Intel Mac OS X 10_7_3; Trident/6.0)'
-ua['Internet Explorer']
-# Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.2; SV1; .NET CLR 3.3.69573; WOW64; en-US)
-ua.opera
-# Opera/9.80 (X11; Linux i686; U; ru) Presto/2.8.131 Version/11.11
-ua.chrome
-# Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.2 (KHTML, like Gecko) Chrome/22.0.1216.0 Safari/537.2'
-ua.google
-# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_4) AppleWebKit/537.13 (KHTML, like Gecko) Chrome/24.0.1290.1 Safari/537.13
-ua['google chrome']
-# Mozilla/5.0 (X11; CrOS i686 2268.111.0) AppleWebKit/536.11 (KHTML, like Gecko) Chrome/20.0.1132.57 Safari/536.11
-ua.firefox
-# Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/16.0.1
-ua.ff
-# Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:15.0) Gecko/20100101 Firefox/15.0.1
-ua.safari
-# Mozilla/5.0 (iPad; CPU OS 6_0 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10A5355d Safari/8536.25
+# Get a random browser user-agent string
+print(ua.random)
 
-# and the best one, get a random browser user-agent string
-ua.random
+# Or get user-agent string from a specific browser
+print(ua.chrome)
+# Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
+print(ua.google)
+# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_4) AppleWebKit/537.13 (KHTML, like Gecko) Chrome/24.0.1290.1 Safari/537.13
+print(ua['google chrome'])
+# Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36
+print(ua.firefox)
+# Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/115.0
+print(ua.ff)
+# Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0
+print(ua.safari)
+# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.2 Safari/605.1.15
 ```
 
-### Notes
+#### Additional usage
+
+Additional features that fake-useragent now offers since v1.2.0.
 
-If you want to specify your own browser list, you can do that via the `browsers` argument (default is: `["chrome", "edge", "internet explorer", "firefox", "safari", "opera"]`).
+If you want to specify your own browser list, you can do that via the `browsers` argument (default is: `["chrome", "edge", "firefox", "safari"]`).  
+This example will only return random useragents from Edge and Chrome:
 
 ```py
 from fake_useragent import UserAgent
 ua = UserAgent(browsers=['edge', 'chrome'])
 ua.random
 ```
 
-You can add your own fallback string using the `fallback` parameter, in rare cases everything else failed:
-
-```py
-import fake_useragent
+_Note:_ Fakeuser-agent knowns about: Chrome, Edge, Firefox and Safari. Other browsers are not popular enough and aren't part of our dataset we use.
 
-ua = fake_useragent.UserAgent(fallback='your favorite Browser')
-# in case if something went wrong, one more time it is REALLY!!! rare case
-ua.random == 'your favorite Browser'
-```
+---
 
-If you will try to get unknown browser:
+If you want to specify your own operating systems, you can do that via the `os` argument (default is: `["windows", "macos", "linux"]`).  
+In this example you will only get Linux useragents back:
 
 ```py
 from fake_useragent import UserAgent
-ua = UserAgent()
-ua.unknown
-# Traceback (most recent call last):
-#   ...
-# fake_useragent.errors.FakeUserAgentError: Error occurred during getting browser: unknown
+ua = UserAgent(os='linux')
+ua.random
 ```
 
-By default `fake-useragent` will use it's local ([`browsers.json`](./fake_useragent/data/browsers.json)) data file as the data source.
+---
 
-If you don't want to use the local data, but use the external data source to retrieve the user-agents. Set `use_external_data` to `True`:
+If you want to return more popular useragent strings, you can play with the `min_percentage` argument (default is: `0.0`, meaning all useragents will match).  
+In this example you get only useragents that have a minimum usage percentage of 1.3% (or higher):
 
 ```py
 from fake_useragent import UserAgent
-ua = UserAgent(use_external_data=True)
+ua = UserAgent(min_percentage=1.3)
+ua.random
 ```
 
-As a fallback method `fake-useragent` will retrieve it's data from an external data source and stores in a cache file _or_ when you expcility set `use_external_data=True` as parameter.
-You can trigger an update to the cache file by calling `update()`:
+_Hint:_ Of-course you can **combine all those arguments** to you liking!
 
-```py
-from fake_useragent import UserAgent
-ua = UserAgent()
-ua.update()
-```
+### Notes
 
-The default location of the external resource cache file is in your os temp dir, like `/tmp`.  
-You can change the temp directory by changing `cache_path` (mainly useful together when `use_external_data` is set to True).
+You can override the fallback string using the `fallback` parameter, in very rare cases something failed:
 
 ```py
 import fake_useragent
 
-# I am strongly! recommend using a version suffix
-location = '/home/user/fake_useragent%s.json' % fake_useragent.VERSION
+ua = fake_useragent.UserAgent(fallback='your favorite Browser')
+# in case if something went wrong, one more time it is REALLY!!! rare case
+ua.random == 'your favorite Browser'
+```
 
-ua = fake_useragent.UserAgent(use_external_data=True, cache_path=location)
-ua.random
+If you will try to get unknown browser:
+
+```py
+from fake_useragent import UserAgent
+ua = UserAgent()
+print(ua.unknown)
+#Error occurred during getting browser: randm, but was suppressed with fallback.
+#Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
 ```
 
 If you need to safe some attributes from overriding them in UserAgent by `__getattr__` method
 use `safe_attrs` you can pass there attributes names.
 At least this will prevent you from raising FakeUserAgentError when attribute not found.
 
 For example, when using fake*useragent with `injections <https://github.com/tailhook/injections>`* you need to:
@@ -160,45 +153,84 @@
 
 Make sure that you using latest version!
 
 ```sh
 pip install --upgrade fake-useragent
 ```
 
-Check version via python console:
+Or if that isn't working, try to install the latest package version like this (`1.2.0` is an example, check what the [latest version is on PyPi](https://pypi.org/project/fake-useragent/#history)):
+
+```sh
+pip install fake-useragent==1.2.0
+```
+
+Check version via the Python console:
 
 ```py
 import fake_useragent
 
 print(fake_useragent.VERSION)
 ```
 
 And you are always welcome to post [issues](https://github.com/fake-useragent/fake-useragent/issues).
 
 Please do not forget to mention the version that you are using.
 
-### Developers
+### For Developers
 
-Since GitHub Actions is unable to reach useragentstring.com. We can run the script below to automatically scrape the user-agent strings from the external data source. The script will copy the [JSONlines](https://jsonlines.org/) file to the `src/fake_useragent/data` directory. Execute:
+Since GitHub Actions is unable to reach willshouse.com and has Cloudflare protection. We can run the script below to automatically scrape the user-agent strings from the external data source. The script will copy the [JSONlines](https://jsonlines.org/) file to the `src/fake_useragent/data` directory. Execute:
 
 ```sh
 ./update_data_file.sh
 ```
 
 The data JSON file is part of the Python package, see [pyproject.toml](pyproject.toml). Read more about [Data files support](https://setuptools.pypa.io/en/latest/userguide/datafiles.html).
 
-### Tests
+### Python Virtual Environment
+
+We encourage to use Python virtual environment before installing Pip packages, like so:
+
+```sh
+python -m virtualenv env
+source env/bin/activate
+```
+
+#### Tests
 
 ```sh
 pip install -r requirements.txt
 tox
 ```
 
+#### Linting
+
+To fix imports:
+
+```sh
+pip install -r requirements.txt
+ruff --select="I" --fix .
+```
+
 ### Changelog
 
+- 1.2.0 August 2, 2023
+
+  - Updated browser useragent data
+  - Allow filters on browser, OS and usage percentage
+  - Update the cache scraper to scape the new data source for user-agent strings
+  - Adapted the code to work with the new JSON data format
+
+- 1.1.3 March 20, 2023
+
+  - Update dependencies
+
+- 1.1.2 February 8, 2023
+
+  - Security fixes
+
 - 1.1.1 December 4, 2022
 
   - Remove whitespaces from user agent strings, this is a patch release
 
 - 1.1.0 November 26, 2022
 
   - Add `pkg_resource` as fallback mechanism in trying to retrieve the local JSON data file
```

### Comparing `fake-useragent-1.1.3/README.md` & `fake-useragent-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [![Test & Deploy fake-useragent](https://github.com/fake-useragent/fake-useragent/actions/workflows/action.yml/badge.svg?branch=master)](https://github.com/fake-useragent/fake-useragent/actions/workflows/action.yml?query=branch%3Amaster)
 
 # fake-useragent
 
-Up-to-date simple useragent faker with real world database
+Up-to-date simple useragent faker with real world database.
 
 ## Features
 
-- Data is pre-downloaded from [useragentstring.com](http://useragentstring.com/) and part of the package
+- Data is pre-downloaded from [techblog.willshouse.com](https://techblog.willshouse.com/2012/01/03/most-common-user-agents/) and the data is part of the package
 - Retrieves user-agent strings locally
 - Supports Python 3.x
-- _Fallback_ to external resource ([useragentstring.com](http://useragentstring.com/)) + caching
 
 ### Installation
 
 ```sh
 pip install fake-useragent
 ```
 
@@ -21,103 +20,97 @@
 
 ```sh
 pip3 install fake-useragent
 ```
 
 ### Usage
 
+Simple usage example, see below for more examples:
+
 ```py
 from fake_useragent import UserAgent
 ua = UserAgent()
 
-ua.ie
-# Mozilla/5.0 (Windows; U; MSIE 9.0; Windows NT 9.0; en-US);
-ua.msie
-# Mozilla/5.0 (compatible; MSIE 10.0; Macintosh; Intel Mac OS X 10_7_3; Trident/6.0)'
-ua['Internet Explorer']
-# Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.2; SV1; .NET CLR 3.3.69573; WOW64; en-US)
-ua.opera
-# Opera/9.80 (X11; Linux i686; U; ru) Presto/2.8.131 Version/11.11
-ua.chrome
-# Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.2 (KHTML, like Gecko) Chrome/22.0.1216.0 Safari/537.2'
-ua.google
-# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_4) AppleWebKit/537.13 (KHTML, like Gecko) Chrome/24.0.1290.1 Safari/537.13
-ua['google chrome']
-# Mozilla/5.0 (X11; CrOS i686 2268.111.0) AppleWebKit/536.11 (KHTML, like Gecko) Chrome/20.0.1132.57 Safari/536.11
-ua.firefox
-# Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/16.0.1
-ua.ff
-# Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:15.0) Gecko/20100101 Firefox/15.0.1
-ua.safari
-# Mozilla/5.0 (iPad; CPU OS 6_0 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10A5355d Safari/8536.25
+# Get a random browser user-agent string
+print(ua.random)
 
-# and the best one, get a random browser user-agent string
-ua.random
+# Or get user-agent string from a specific browser
+print(ua.chrome)
+# Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
+print(ua.google)
+# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_4) AppleWebKit/537.13 (KHTML, like Gecko) Chrome/24.0.1290.1 Safari/537.13
+print(ua['google chrome'])
+# Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36
+print(ua.firefox)
+# Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/115.0
+print(ua.ff)
+# Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0
+print(ua.safari)
+# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.2 Safari/605.1.15
 ```
 
-### Notes
+#### Additional usage
+
+Additional features that fake-useragent now offers since v1.2.0.
 
-If you want to specify your own browser list, you can do that via the `browsers` argument (default is: `["chrome", "edge", "internet explorer", "firefox", "safari", "opera"]`).
+If you want to specify your own browser list, you can do that via the `browsers` argument (default is: `["chrome", "edge", "firefox", "safari"]`).  
+This example will only return random useragents from Edge and Chrome:
 
 ```py
 from fake_useragent import UserAgent
 ua = UserAgent(browsers=['edge', 'chrome'])
 ua.random
 ```
 
-You can add your own fallback string using the `fallback` parameter, in rare cases everything else failed:
-
-```py
-import fake_useragent
+_Note:_ Fakeuser-agent knowns about: Chrome, Edge, Firefox and Safari. Other browsers are not popular enough and aren't part of our dataset we use.
 
-ua = fake_useragent.UserAgent(fallback='your favorite Browser')
-# in case if something went wrong, one more time it is REALLY!!! rare case
-ua.random == 'your favorite Browser'
-```
+---
 
-If you will try to get unknown browser:
+If you want to specify your own operating systems, you can do that via the `os` argument (default is: `["windows", "macos", "linux"]`).  
+In this example you will only get Linux useragents back:
 
 ```py
 from fake_useragent import UserAgent
-ua = UserAgent()
-ua.unknown
-# Traceback (most recent call last):
-#   ...
-# fake_useragent.errors.FakeUserAgentError: Error occurred during getting browser: unknown
+ua = UserAgent(os='linux')
+ua.random
 ```
 
-By default `fake-useragent` will use it's local ([`browsers.json`](./fake_useragent/data/browsers.json)) data file as the data source.
+---
 
-If you don't want to use the local data, but use the external data source to retrieve the user-agents. Set `use_external_data` to `True`:
+If you want to return more popular useragent strings, you can play with the `min_percentage` argument (default is: `0.0`, meaning all useragents will match).  
+In this example you get only useragents that have a minimum usage percentage of 1.3% (or higher):
 
 ```py
 from fake_useragent import UserAgent
-ua = UserAgent(use_external_data=True)
+ua = UserAgent(min_percentage=1.3)
+ua.random
 ```
 
-As a fallback method `fake-useragent` will retrieve it's data from an external data source and stores in a cache file _or_ when you expcility set `use_external_data=True` as parameter.
-You can trigger an update to the cache file by calling `update()`:
+_Hint:_ Of-course you can **combine all those arguments** to you liking!
 
-```py
-from fake_useragent import UserAgent
-ua = UserAgent()
-ua.update()
-```
+### Notes
 
-The default location of the external resource cache file is in your os temp dir, like `/tmp`.  
-You can change the temp directory by changing `cache_path` (mainly useful together when `use_external_data` is set to True).
+You can override the fallback string using the `fallback` parameter, in very rare cases something failed:
 
 ```py
 import fake_useragent
 
-# I am strongly! recommend using a version suffix
-location = '/home/user/fake_useragent%s.json' % fake_useragent.VERSION
+ua = fake_useragent.UserAgent(fallback='your favorite Browser')
+# in case if something went wrong, one more time it is REALLY!!! rare case
+ua.random == 'your favorite Browser'
+```
 
-ua = fake_useragent.UserAgent(use_external_data=True, cache_path=location)
-ua.random
+If you will try to get unknown browser:
+
+```py
+from fake_useragent import UserAgent
+ua = UserAgent()
+print(ua.unknown)
+#Error occurred during getting browser: randm, but was suppressed with fallback.
+#Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
 ```
 
 If you need to safe some attributes from overriding them in UserAgent by `__getattr__` method
 use `safe_attrs` you can pass there attributes names.
 At least this will prevent you from raising FakeUserAgentError when attribute not found.
 
 For example, when using fake*useragent with `injections <https://github.com/tailhook/injections>`* you need to:
@@ -135,45 +128,84 @@
 
 Make sure that you using latest version!
 
 ```sh
 pip install --upgrade fake-useragent
 ```
 
-Check version via python console:
+Or if that isn't working, try to install the latest package version like this (`1.2.0` is an example, check what the [latest version is on PyPi](https://pypi.org/project/fake-useragent/#history)):
+
+```sh
+pip install fake-useragent==1.2.0
+```
+
+Check version via the Python console:
 
 ```py
 import fake_useragent
 
 print(fake_useragent.VERSION)
 ```
 
 And you are always welcome to post [issues](https://github.com/fake-useragent/fake-useragent/issues).
 
 Please do not forget to mention the version that you are using.
 
-### Developers
+### For Developers
 
-Since GitHub Actions is unable to reach useragentstring.com. We can run the script below to automatically scrape the user-agent strings from the external data source. The script will copy the [JSONlines](https://jsonlines.org/) file to the `src/fake_useragent/data` directory. Execute:
+Since GitHub Actions is unable to reach willshouse.com and has Cloudflare protection. We can run the script below to automatically scrape the user-agent strings from the external data source. The script will copy the [JSONlines](https://jsonlines.org/) file to the `src/fake_useragent/data` directory. Execute:
 
 ```sh
 ./update_data_file.sh
 ```
 
 The data JSON file is part of the Python package, see [pyproject.toml](pyproject.toml). Read more about [Data files support](https://setuptools.pypa.io/en/latest/userguide/datafiles.html).
 
-### Tests
+### Python Virtual Environment
+
+We encourage to use Python virtual environment before installing Pip packages, like so:
+
+```sh
+python -m virtualenv env
+source env/bin/activate
+```
+
+#### Tests
 
 ```sh
 pip install -r requirements.txt
 tox
 ```
 
+#### Linting
+
+To fix imports:
+
+```sh
+pip install -r requirements.txt
+ruff --select="I" --fix .
+```
+
 ### Changelog
 
+- 1.2.0 August 2, 2023
+
+  - Updated browser useragent data
+  - Allow filters on browser, OS and usage percentage
+  - Update the cache scraper to scape the new data source for user-agent strings
+  - Adapted the code to work with the new JSON data format
+
+- 1.1.3 March 20, 2023
+
+  - Update dependencies
+
+- 1.1.2 February 8, 2023
+
+  - Security fixes
+
 - 1.1.1 December 4, 2022
 
   - Remove whitespaces from user agent strings, this is a patch release
 
 - 1.1.0 November 26, 2022
 
   - Add `pkg_resource` as fallback mechanism in trying to retrieve the local JSON data file
```

### Comparing `fake-useragent-1.1.3/pyproject.toml` & `fake-useragent-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fake-useragent"
-version = "1.1.3"
+version = "1.2.0"
 authors = [
     {name = "Victor Kovtun", email = "hellysmile@gmail.com"},
     {name = "Melroy van den Berg", email = "melroy@melroy.org"},
 ]
 dependencies = [
     "importlib-resources >= 5.0; python_version < '3.10'",
     "importlib-metadata ~= 4.0; python_version < '3.8'",
@@ -43,12 +43,33 @@
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/fake-useragent/fake-useragent"
 
+[tool.ruff]
+line-length = 142
+select = ["B", "C4", "C9", "E", "F", "I", "PL", "S", "SIM", "U", "W", "YTT"]
+ignore = ["B904", "C408", "PLW2901", "SIM105", "SIM108"]
+target-version = "py37"
+
+[tool.ruff.isort]
+known-first-party = ["fake_useragent"]
+
+[tool.ruff.mccabe]
+max-complexity = 13
+
+[tool.ruff.per-file-ignores]
+"src/fake_useragent/__init__.py" = ["F401"]
+"src/fake_useragent/fake.py" = ["B006", "S101"]
+"tests/*" = ["S", "SIM", "UP015"]
+
+[tool.ruff.pylint]
+max-args = 7
+max-branches = 13
+
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.package-data]
 "fake_useragent.data" = ["*.json"]
```

### Comparing `fake-useragent-1.1.3/src/fake_useragent.egg-info/PKG-INFO` & `fake-useragent-1.2.0/src/fake_useragent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-useragent
-Version: 1.1.3
+Version: 1.2.0
 Summary: Up-to-date simple useragent faker with real world database
 Author-email: Victor Kovtun <hellysmile@gmail.com>, Melroy van den Berg <melroy@melroy.org>
 Project-URL: Homepage, https://github.com/fake-useragent/fake-useragent
 Keywords: user,agent,user agent,useragent,fake,fake useragent,fake user agent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,22 +23,21 @@
 License-File: LICENSE
 License-File: AUTHORS
 
 [![Test & Deploy fake-useragent](https://github.com/fake-useragent/fake-useragent/actions/workflows/action.yml/badge.svg?branch=master)](https://github.com/fake-useragent/fake-useragent/actions/workflows/action.yml?query=branch%3Amaster)
 
 # fake-useragent
 
-Up-to-date simple useragent faker with real world database
+Up-to-date simple useragent faker with real world database.
 
 ## Features
 
-- Data is pre-downloaded from [useragentstring.com](http://useragentstring.com/) and part of the package
+- Data is pre-downloaded from [techblog.willshouse.com](https://techblog.willshouse.com/2012/01/03/most-common-user-agents/) and the data is part of the package
 - Retrieves user-agent strings locally
 - Supports Python 3.x
-- _Fallback_ to external resource ([useragentstring.com](http://useragentstring.com/)) + caching
 
 ### Installation
 
 ```sh
 pip install fake-useragent
 ```
 
@@ -46,103 +45,97 @@
 
 ```sh
 pip3 install fake-useragent
 ```
 
 ### Usage
 
+Simple usage example, see below for more examples:
+
 ```py
 from fake_useragent import UserAgent
 ua = UserAgent()
 
-ua.ie
-# Mozilla/5.0 (Windows; U; MSIE 9.0; Windows NT 9.0; en-US);
-ua.msie
-# Mozilla/5.0 (compatible; MSIE 10.0; Macintosh; Intel Mac OS X 10_7_3; Trident/6.0)'
-ua['Internet Explorer']
-# Mozilla/5.0 (compatible; MSIE 8.0; Windows NT 6.1; Trident/4.0; GTB7.4; InfoPath.2; SV1; .NET CLR 3.3.69573; WOW64; en-US)
-ua.opera
-# Opera/9.80 (X11; Linux i686; U; ru) Presto/2.8.131 Version/11.11
-ua.chrome
-# Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.2 (KHTML, like Gecko) Chrome/22.0.1216.0 Safari/537.2'
-ua.google
-# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_4) AppleWebKit/537.13 (KHTML, like Gecko) Chrome/24.0.1290.1 Safari/537.13
-ua['google chrome']
-# Mozilla/5.0 (X11; CrOS i686 2268.111.0) AppleWebKit/536.11 (KHTML, like Gecko) Chrome/20.0.1132.57 Safari/536.11
-ua.firefox
-# Mozilla/5.0 (Windows NT 6.2; Win64; x64; rv:16.0.1) Gecko/20121011 Firefox/16.0.1
-ua.ff
-# Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:15.0) Gecko/20100101 Firefox/15.0.1
-ua.safari
-# Mozilla/5.0 (iPad; CPU OS 6_0 like Mac OS X) AppleWebKit/536.26 (KHTML, like Gecko) Version/6.0 Mobile/10A5355d Safari/8536.25
+# Get a random browser user-agent string
+print(ua.random)
 
-# and the best one, get a random browser user-agent string
-ua.random
+# Or get user-agent string from a specific browser
+print(ua.chrome)
+# Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
+print(ua.google)
+# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_4) AppleWebKit/537.13 (KHTML, like Gecko) Chrome/24.0.1290.1 Safari/537.13
+print(ua['google chrome'])
+# Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36
+print(ua.firefox)
+# Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/115.0
+print(ua.ff)
+# Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0
+print(ua.safari)
+# Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.2 Safari/605.1.15
 ```
 
-### Notes
+#### Additional usage
+
+Additional features that fake-useragent now offers since v1.2.0.
 
-If you want to specify your own browser list, you can do that via the `browsers` argument (default is: `["chrome", "edge", "internet explorer", "firefox", "safari", "opera"]`).
+If you want to specify your own browser list, you can do that via the `browsers` argument (default is: `["chrome", "edge", "firefox", "safari"]`).  
+This example will only return random useragents from Edge and Chrome:
 
 ```py
 from fake_useragent import UserAgent
 ua = UserAgent(browsers=['edge', 'chrome'])
 ua.random
 ```
 
-You can add your own fallback string using the `fallback` parameter, in rare cases everything else failed:
-
-```py
-import fake_useragent
+_Note:_ Fakeuser-agent knowns about: Chrome, Edge, Firefox and Safari. Other browsers are not popular enough and aren't part of our dataset we use.
 
-ua = fake_useragent.UserAgent(fallback='your favorite Browser')
-# in case if something went wrong, one more time it is REALLY!!! rare case
-ua.random == 'your favorite Browser'
-```
+---
 
-If you will try to get unknown browser:
+If you want to specify your own operating systems, you can do that via the `os` argument (default is: `["windows", "macos", "linux"]`).  
+In this example you will only get Linux useragents back:
 
 ```py
 from fake_useragent import UserAgent
-ua = UserAgent()
-ua.unknown
-# Traceback (most recent call last):
-#   ...
-# fake_useragent.errors.FakeUserAgentError: Error occurred during getting browser: unknown
+ua = UserAgent(os='linux')
+ua.random
 ```
 
-By default `fake-useragent` will use it's local ([`browsers.json`](./fake_useragent/data/browsers.json)) data file as the data source.
+---
 
-If you don't want to use the local data, but use the external data source to retrieve the user-agents. Set `use_external_data` to `True`:
+If you want to return more popular useragent strings, you can play with the `min_percentage` argument (default is: `0.0`, meaning all useragents will match).  
+In this example you get only useragents that have a minimum usage percentage of 1.3% (or higher):
 
 ```py
 from fake_useragent import UserAgent
-ua = UserAgent(use_external_data=True)
+ua = UserAgent(min_percentage=1.3)
+ua.random
 ```
 
-As a fallback method `fake-useragent` will retrieve it's data from an external data source and stores in a cache file _or_ when you expcility set `use_external_data=True` as parameter.
-You can trigger an update to the cache file by calling `update()`:
+_Hint:_ Of-course you can **combine all those arguments** to you liking!
 
-```py
-from fake_useragent import UserAgent
-ua = UserAgent()
-ua.update()
-```
+### Notes
 
-The default location of the external resource cache file is in your os temp dir, like `/tmp`.  
-You can change the temp directory by changing `cache_path` (mainly useful together when `use_external_data` is set to True).
+You can override the fallback string using the `fallback` parameter, in very rare cases something failed:
 
 ```py
 import fake_useragent
 
-# I am strongly! recommend using a version suffix
-location = '/home/user/fake_useragent%s.json' % fake_useragent.VERSION
+ua = fake_useragent.UserAgent(fallback='your favorite Browser')
+# in case if something went wrong, one more time it is REALLY!!! rare case
+ua.random == 'your favorite Browser'
+```
 
-ua = fake_useragent.UserAgent(use_external_data=True, cache_path=location)
-ua.random
+If you will try to get unknown browser:
+
+```py
+from fake_useragent import UserAgent
+ua = UserAgent()
+print(ua.unknown)
+#Error occurred during getting browser: randm, but was suppressed with fallback.
+#Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
 ```
 
 If you need to safe some attributes from overriding them in UserAgent by `__getattr__` method
 use `safe_attrs` you can pass there attributes names.
 At least this will prevent you from raising FakeUserAgentError when attribute not found.
 
 For example, when using fake*useragent with `injections <https://github.com/tailhook/injections>`* you need to:
@@ -160,45 +153,84 @@
 
 Make sure that you using latest version!
 
 ```sh
 pip install --upgrade fake-useragent
 ```
 
-Check version via python console:
+Or if that isn't working, try to install the latest package version like this (`1.2.0` is an example, check what the [latest version is on PyPi](https://pypi.org/project/fake-useragent/#history)):
+
+```sh
+pip install fake-useragent==1.2.0
+```
+
+Check version via the Python console:
 
 ```py
 import fake_useragent
 
 print(fake_useragent.VERSION)
 ```
 
 And you are always welcome to post [issues](https://github.com/fake-useragent/fake-useragent/issues).
 
 Please do not forget to mention the version that you are using.
 
-### Developers
+### For Developers
 
-Since GitHub Actions is unable to reach useragentstring.com. We can run the script below to automatically scrape the user-agent strings from the external data source. The script will copy the [JSONlines](https://jsonlines.org/) file to the `src/fake_useragent/data` directory. Execute:
+Since GitHub Actions is unable to reach willshouse.com and has Cloudflare protection. We can run the script below to automatically scrape the user-agent strings from the external data source. The script will copy the [JSONlines](https://jsonlines.org/) file to the `src/fake_useragent/data` directory. Execute:
 
 ```sh
 ./update_data_file.sh
 ```
 
 The data JSON file is part of the Python package, see [pyproject.toml](pyproject.toml). Read more about [Data files support](https://setuptools.pypa.io/en/latest/userguide/datafiles.html).
 
-### Tests
+### Python Virtual Environment
+
+We encourage to use Python virtual environment before installing Pip packages, like so:
+
+```sh
+python -m virtualenv env
+source env/bin/activate
+```
+
+#### Tests
 
 ```sh
 pip install -r requirements.txt
 tox
 ```
 
+#### Linting
+
+To fix imports:
+
+```sh
+pip install -r requirements.txt
+ruff --select="I" --fix .
+```
+
 ### Changelog
 
+- 1.2.0 August 2, 2023
+
+  - Updated browser useragent data
+  - Allow filters on browser, OS and usage percentage
+  - Update the cache scraper to scape the new data source for user-agent strings
+  - Adapted the code to work with the new JSON data format
+
+- 1.1.3 March 20, 2023
+
+  - Update dependencies
+
+- 1.1.2 February 8, 2023
+
+  - Security fixes
+
 - 1.1.1 December 4, 2022
 
   - Remove whitespaces from user agent strings, this is a patch release
 
 - 1.1.0 November 26, 2022
 
   - Add `pkg_resource` as fallback mechanism in trying to retrieve the local JSON data file
```

### Comparing `fake-useragent-1.1.3/src/fake_useragent.egg-info/SOURCES.txt` & `fake-useragent-1.2.0/src/fake_useragent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

