# Comparing `tmp/fake-useragent-1.2.0.tar.gz` & `tmp/fake-useragent-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake-useragent-1.2.0.tar", last modified: Wed Aug  2 00:03:38 2023, max compression
+gzip compressed data, was "fake-useragent-1.2.1.tar", last modified: Wed Aug  2 14:07:10 2023, max compression
```

## Comparing `fake-useragent-1.2.0.tar` & `fake-useragent-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/fake_useragent/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/data/browsers.json
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/src/fake_useragent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.093012 fake-useragent-1.2.0/src/fake_useragent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:03:37.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 00:03:38.000000 fake-useragent-1.2.0/src/fake_useragent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:03:38.097012 fake-useragent-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-02 00:03:27.000000 fake-useragent-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:07:10.700548 fake-useragent-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-08-02 14:07:10.700548 fake-useragent-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:07:10.700548 fake-useragent-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:07:10.696548 fake-useragent-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:07:10.696548 fake-useragent-1.2.1/src/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:07:10.696548 fake-useragent-1.2.1/src/fake_useragent/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/data/browsers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/src/fake_useragent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:07:10.696548 fake-useragent-1.2.1/src/fake_useragent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-08-02 14:07:10.000000 fake-useragent-1.2.1/src/fake_useragent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-02 14:07:10.000000 fake-useragent-1.2.1/src/fake_useragent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:07:10.000000 fake-useragent-1.2.1/src/fake_useragent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:07:10.000000 fake-useragent-1.2.1/src/fake_useragent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 14:07:10.000000 fake-useragent-1.2.1/src/fake_useragent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 14:07:10.000000 fake-useragent-1.2.1/src/fake_useragent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:07:10.700548 fake-useragent-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-02 14:06:56.000000 fake-useragent-1.2.1/tests/test_utils.py
```

### Comparing `fake-useragent-1.2.0/LICENSE` & `fake-useragent-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fake-useragent-1.2.0/PKG-INFO` & `fake-useragent-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-useragent
-Version: 1.2.0
+Version: 1.2.1
 Summary: Up-to-date simple useragent faker with real world database
 Author-email: Victor Kovtun <hellysmile@gmail.com>, Melroy van den Berg <melroy@melroy.org>
 Project-URL: Homepage, https://github.com/fake-useragent/fake-useragent
 Keywords: user,agent,user agent,useragent,fake,fake useragent,fake user agent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -208,14 +208,19 @@
 ```sh
 pip install -r requirements.txt
 ruff --select="I" --fix .
 ```
 
 ### Changelog
 
+- 1.2.1 August 2, 2023
+
+  - Small improvements in the `min_percentage` check
+  - Update all Pip package dependencies
+
 - 1.2.0 August 2, 2023
 
   - Updated browser useragent data
   - Allow filters on browser, OS and usage percentage
   - Update the cache scraper to scape the new data source for user-agent strings
   - Adapted the code to work with the new JSON data format
```

### Comparing `fake-useragent-1.2.0/README.md` & `fake-useragent-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,19 @@
 ```sh
 pip install -r requirements.txt
 ruff --select="I" --fix .
 ```
 
 ### Changelog
 
+- 1.2.1 August 2, 2023
+
+  - Small improvements in the `min_percentage` check
+  - Update all Pip package dependencies
+
 - 1.2.0 August 2, 2023
 
   - Updated browser useragent data
   - Allow filters on browser, OS and usage percentage
   - Update the cache scraper to scape the new data source for user-agent strings
   - Adapted the code to work with the new JSON data format
```

### Comparing `fake-useragent-1.2.0/pyproject.toml` & `fake-useragent-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fake-useragent"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
     {name = "Victor Kovtun", email = "hellysmile@gmail.com"},
     {name = "Melroy van den Berg", email = "melroy@melroy.org"},
 ]
 dependencies = [
     "importlib-resources >= 5.0; python_version < '3.10'",
     "importlib-metadata ~= 4.0; python_version < '3.8'",
```

### Comparing `fake-useragent-1.2.0/src/fake_useragent/data/browsers.json` & `fake-useragent-1.2.1/src/fake_useragent/data/browsers.json`

 * *Files identical despite different names*

### Comparing `fake-useragent-1.2.0/src/fake_useragent/fake.py` & `fake-useragent-1.2.1/src/fake_useragent/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,35 +74,35 @@
                 # And based on OS list
                 # And percentage is bigger then min percentage
                 # And convert the iterator back to a list
                 filtered_browsers = list(
                     filter(
                         lambda x: x["browser"] in self.browsers
                         and x["os"] in self.os
-                        and x["percent"] > self.min_percentage,
+                        and x["percent"] >= self.min_percentage,
                         self.data_browsers,
                     )
                 )
             else:
                 # Or when random isn't select, we filter the browsers array based on the 'attr' using lamba
                 # And based on OS list
                 # And percentage is bigger then min percentage
                 # And convert the iterator back to a list
                 filtered_browsers = list(
                     filter(
                         lambda x: x["browser"] == attr
                         and x["os"] in self.os
-                        and x["percent"] > self.min_percentage,
+                        and x["percent"] >= self.min_percentage,
                         self.data_browsers,
                     )
                 )
 
             # Pick a random browser user-agent from the filtered browsers
             # And return the useragent string.
-            return random.choice(filtered_browsers).get("useragent")
+            return random.choice(filtered_browsers).get("useragent")  # noqa: S311
         except (KeyError, IndexError):
             if self.fallback is None:
                 raise FakeUserAgentError(
                     f"Error occurred during getting browser: {attr}"
                 )  # noqa
             else:
                 logger.warning(
```

### Comparing `fake-useragent-1.2.0/src/fake_useragent/utils.py` & `fake-useragent-1.2.1/src/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `fake-useragent-1.2.0/src/fake_useragent.egg-info/PKG-INFO` & `fake-useragent-1.2.1/src/fake_useragent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-useragent
-Version: 1.2.0
+Version: 1.2.1
 Summary: Up-to-date simple useragent faker with real world database
 Author-email: Victor Kovtun <hellysmile@gmail.com>, Melroy van den Berg <melroy@melroy.org>
 Project-URL: Homepage, https://github.com/fake-useragent/fake-useragent
 Keywords: user,agent,user agent,useragent,fake,fake useragent,fake user agent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -208,14 +208,19 @@
 ```sh
 pip install -r requirements.txt
 ruff --select="I" --fix .
 ```
 
 ### Changelog
 
+- 1.2.1 August 2, 2023
+
+  - Small improvements in the `min_percentage` check
+  - Update all Pip package dependencies
+
 - 1.2.0 August 2, 2023
 
   - Updated browser useragent data
   - Allow filters on browser, OS and usage percentage
   - Update the cache scraper to scape the new data source for user-agent strings
   - Adapted the code to work with the new JSON data format
```

### Comparing `fake-useragent-1.2.0/src/fake_useragent.egg-info/SOURCES.txt` & `fake-useragent-1.2.1/src/fake_useragent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-useragent-1.2.0/tests/test_fake.py` & `fake-useragent-1.2.1/tests/test_fake.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,27 +8,14 @@
 class TestFake(unittest.TestCase):
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def _probe(self, ua):
-        ua.edge
-        ua.google
-        ua.chrome
-        ua.googlechrome
-        ua.google_chrome
-        ua["google chrome"]
-        ua.firefox
-        ua.ff
-        ua.safari
-        ua.random
-        ua["random"]
-
     def test_fake_init(self):
         ua = UserAgent()
 
         self.assertTrue(ua.chrome)
         self.assertIsInstance(ua.chrome, str)
         self.assertTrue(ua.edge)
         self.assertIsInstance(ua.edge, str)
@@ -37,18 +24,27 @@
         self.assertTrue(ua.firefox)
         self.assertIsInstance(ua.firefox, str)
         self.assertTrue(ua.safari)
         self.assertIsInstance(ua.safari, str)
         self.assertTrue(ua.random)
         self.assertIsInstance(ua.random, str)
 
-    def test_fake_user_agent_browsers(self):
+    def test_fake_probe_user_agent_browsers(self):
         ua = UserAgent()
-
-        self._probe(ua)
+        ua.edge  # noqa: B018
+        ua.google  # noqa: B018
+        ua.chrome  # noqa: B018
+        ua.googlechrome  # noqa: B018
+        ua.google_chrome  # noqa: B018
+        ua["google chrome"]  # noqa: B018
+        ua.firefox  # noqa: B018
+        ua.ff  # noqa: B018
+        ua.safari  # noqa: B018
+        ua.random  # noqa: B018
+        ua["random"]  # noqa: B018
 
     def test_fake_data_browser_type(self):
         ua = UserAgent()
         assert isinstance(ua.data_browsers, list)
 
     def test_fake_fallback(self):
         fallback = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
@@ -80,14 +76,14 @@
         with pytest.raises(AssertionError):
             UserAgent(safe_attrs=[66])
 
     def test_fake_safe_attrs(self):
         ua = UserAgent(safe_attrs=("__injections__",))
 
         with pytest.raises(AttributeError):
-            ua.__injections__
+            ua.__injections__  # noqa: B018
 
     def test_fake_version(self):
         assert VERSION == settings.__version__
 
     def test_fake_aliases(self):
         assert FakeUserAgent is UserAgent
```

### Comparing `fake-useragent-1.2.0/tests/test_utils.py` & `fake-useragent-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

