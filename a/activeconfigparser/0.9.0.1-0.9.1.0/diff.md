# Comparing `tmp/activeconfigparser-0.9.0.1.tar.gz` & `tmp/activeconfigparser-0.9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activeconfigparser-0.9.0.1.tar", max compression
+gzip compressed data, was "activeconfigparser-0.9.1.0.tar", max compression
```

## Comparing `activeconfigparser-0.9.0.1.tar` & `activeconfigparser-0.9.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    17842 2023-07-31 00:05:49.171704 activeconfigparser-0.9.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/LICENSE
--rw-r--r--   0        0        0     3565 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.1/README.md
--rw-r--r--   0        0        0     1898 2023-07-31 00:04:41.191715 activeconfigparser-0.9.0.1/pyproject.toml
--rw-r--r--   0        0        0    75261 2023-07-31 00:00:10.181760 activeconfigparser-0.9.0.1/src/activeconfigparser/ActiveConfigParser.py
--rw-r--r--   0        0        0     5186 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.1/src/activeconfigparser/HandlerParameters.py
--rw-r--r--   0        0        0     2559 2023-06-28 01:15:21.993938 activeconfigparser-0.9.0.1/src/activeconfigparser/__init__.py
--rw-r--r--   0        0        0      158 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/__init__.py
--rw-r--r--   0        0        0     4416 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/common.py
--rw-r--r--   0        0        0     3111 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser.ini
--rw-r--r--   0        0        0      373 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_badkeys.ini
--rw-r--r--   0        0        0      183 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_default.ini
--rw-r--r--   0        0        0      253 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_01.ini
--rw-r--r--   0        0        0      451 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_02.ini
--rw-r--r--   0        0        0      355 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03a.ini
--rw-r--r--   0        0        0      409 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03b.ini
--rw-r--r--   0        0        0    88870 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_ActiveConfigParser.py
--rw-r--r--   0        0        0     9706 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_HandlerParameters.py
--rw-r--r--   0        0        0     2511 2023-07-31 00:04:34.321716 activeconfigparser-0.9.0.1/src/activeconfigparser/version.py
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 activeconfigparser-0.9.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18118 2023-08-02 01:14:01.315016 activeconfigparser-0.9.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/LICENSE
+-rw-r--r--   0        0        0     3565 2023-06-29 11:02:00.401110 activeconfigparser-0.9.1.0/README.md
+-rw-r--r--   0        0        0     1898 2023-08-02 01:14:01.315016 activeconfigparser-0.9.1.0/pyproject.toml
+-rw-r--r--   0        0        0    76450 2023-08-02 01:14:01.315016 activeconfigparser-0.9.1.0/src/activeconfigparser/ActiveConfigParser.py
+-rw-r--r--   0        0        0     5186 2023-06-29 11:02:00.401110 activeconfigparser-0.9.1.0/src/activeconfigparser/HandlerParameters.py
+-rw-r--r--   0        0        0     2559 2023-06-28 01:15:21.993938 activeconfigparser-0.9.1.0/src/activeconfigparser/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/__init__.py
+-rw-r--r--   0        0        0     4416 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/common.py
+-rw-r--r--   0        0        0     3111 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini
+-rw-r--r--   0        0        0      373 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser_badkeys.ini
+-rw-r--r--   0        0        0      183 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser_default.ini
+-rw-r--r--   0        0        0      253 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_01.ini
+-rw-r--r--   0        0        0      451 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_02.ini
+-rw-r--r--   0        0        0      355 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03a.ini
+-rw-r--r--   0        0        0      409 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03b.ini
+-rw-r--r--   0        0        0    92397 2023-08-02 01:14:01.315016 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/test_ActiveConfigParser.py
+-rw-r--r--   0        0        0     9706 2023-06-26 03:08:47.049809 activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/test_HandlerParameters.py
+-rw-r--r--   0        0        0     2511 2023-08-02 01:14:01.315016 activeconfigparser-0.9.1.0/src/activeconfigparser/version.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 activeconfigparser-0.9.1.0/PKG-INFO
```

### Comparing `activeconfigparser-0.9.0.1/CHANGELOG.md` & `activeconfigparser-0.9.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 ### Deprecated
 ### Removed
 ### Fixed
 ### Internal
 ### Security
 -->
 
+## [0.9.1.0] - 2023-08-01
+### Added
+- Added method `_locate_class_method_by_regex(regex_pattern)` which returns a
+  list of tuples containing `[(func_name, <func_ref>), (func_name, <func_ref>, ...)]`
+  as a convenience method for locating methods that match a given pattern.
+
 ## [0.9.0.1] - 2023-07-31
 ### Changed
 - Minor documentation updates
 
 
 ## [0.9.0.0] - 2023-06-29
 ### Added
```

### Comparing `activeconfigparser-0.9.0.1/LICENSE` & `activeconfigparser-0.9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/README.md` & `activeconfigparser-0.9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/pyproject.toml` & `activeconfigparser-0.9.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "activeconfigparser"
 description = "A tool that extends configparser to enable enhanced processing of .ini files."
-version = "0.9.0.1"
+version = "0.9.1.0"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Utility",
     "Bash",
     "Configuration",
     "ActiveConfigParser",
```

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/ActiveConfigParser.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/ActiveConfigParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1209,14 +1209,39 @@
         output = (method_name, method_f)
 
         if output[1] == None:
             self.debug_message(5, f" -> Class method `{method_name}` was not found.") # Console
 
         return output
 
+    def _locate_class_method_by_regex(self, regex_pattern: str) -> list:
+        """Helper that locates a class method (if it exists) whose
+        name is matched by a regular expression (regex) pattern.
+
+        Args:
+            regex_pattern (str): A regular expression pattern (i.e., ``r"_handler_.*"``)
+                that will match the desired method name(s) in the current class.
+
+        Returns:
+            list: A ``list`` of ``tuples`` which contain the name and reference to the
+                method(s) located by the search in the form:
+                ``rval = [ ('_func_a', <ref to _func_a>), ('_func_b', <ref to _func_b>), ... ]``
+        """
+        self._validate_parameter(regex_pattern, (str, ), exception_class="CATASTROPHIC")
+
+        self.debug_message(5, f"Search for class methods matching regex `r'{regex_pattern}'`")
+
+        methods = []
+        for name, func in inspect.getmembers(self, inspect.ismethod):
+            if re.match(regex_pattern, name):
+                methods.append((name, func))
+        for i in methods:
+            self.debug_message(5, f" -> Class method found: `{i[0]}`")
+        return sorted(methods, key=lambda x: x[0])
+
     def _check_handler_rval(self, handler_name, handler_rval) -> 0:
         """Check the returned value from a handler.
 
         Args:
             handler_name (string): The name of the handler.
             handler_rval (int): The return value from a handler being processed.
 
@@ -1415,15 +1440,15 @@
                         self.debug_message(1, line)
                 self.debug_message(1, "")
         else:
             print(self._loginfo)
 
         return
 
-    def _validate_parameter(self, parameter, type_restriction, exception_class="CATASTROPHIC") -> int:
+    def _validate_parameter(self, parameter, type_restriction: tuple, exception_class="CATASTROPHIC") -> int:
         """Parameter validation with ExcpetionControl event on failure.
 
         Returns:
             int: 0 if typecheck succeeds. 1 if typecheck fails and the
                 ``exception_control_level`` prevented the exception from
                 being raised.
```

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/HandlerParameters.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/HandlerParameters.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/__init__.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/__init__.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/common.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/common.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser.ini` & `activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_ActiveConfigParser.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/test_ActiveConfigParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1583,14 +1583,96 @@
         #self.assertIn("handlebars-are-cool", known_operations)
         #self.assertIn("use", known_operations)
         print("----[ TEST END A  ]----------------------------------")
 
         print("OK")
         return 0
 
+    def test_ActiveConfigParser_locate_class_method_by_regex(self):
+        """
+        Test the ``_locate_class_method_by_regex()`` method
+        """
+        print("\n")
+
+        parser = ActiveConfigParser()
+        parser.inifilepath = self._filename
+        parser.debug_level = 5
+
+        print("-----[ TEST START ]--------------------------------------------------")
+        print(">>> Test case when we *do* find our method")
+        rval_actual = parser._locate_class_method_by_regex(r"_handler_.*")
+        rval_expect = [('_handler_use', parser._handler_use)]
+        self.assertEqual(
+            rval_expect, rval_actual, msg=f"_locate_class_method_by_regex failed to find _handler_use()"
+        )
+        print("OK")
+        print("-----[ TEST END   ]--------------------------------------------------\n")
+
+        print("-----[ TEST START ]--------------------------------------------------")
+        print(">>> Test case when we *don't* find our method")
+        rval_actual = parser._locate_class_method_by_regex(r"nonexistent_method")
+        rval_expect = []
+        self.assertEqual(
+            rval_expect,
+            rval_actual,
+            msg=f"_locate_class_method_by_regex should not find a match to `nonexistent_method`"
+        )
+        print("OK")
+        print("-----[ TEST END   ]--------------------------------------------------\n")
+
+        print("-----[ TEST START ]--------------------------------------------------")
+        print(">>> Test case when a non-string parameter is provided")
+        with self.assertRaises(TypeError):
+            rval_actual = parser._locate_class_method_by_regex(None)
+        print("OK")
+        print("-----[ TEST END   ]--------------------------------------------------\n")
+
+        print("OK")
+        return 0
+
+    def test_ActiveConfigParser_locate_class_method(self):
+        """
+        Test the ``_locate_class_method()`` method
+        """
+        print("\n")
+
+        parser = ActiveConfigParser()
+        parser.inifilepath = self._filename
+        parser.debug_level = 5
+
+        print("-----[ TEST START ]--------------------------------------------------")
+        print(">>> Test case when we *do* find our method")
+        rval_actual = parser._locate_class_method("_handler_use")
+        rval_expect = ('_handler_use', parser._handler_use)
+        self.assertEqual(rval_expect, rval_actual, msg=f"_locate_class_method failed to find _handler_use()")
+        print("OK")
+        print("-----[ TEST END   ]--------------------------------------------------\n")
+
+        print("-----[ TEST START ]--------------------------------------------------")
+        print(">>> Test case when we *don't* find our method")
+        rval_actual = parser._locate_class_method("nonexistent_method")
+        rval_expect = ('nonexistent_method', None)
+        self.assertEqual(
+            rval_expect,
+            rval_actual,
+            msg=f"_locate_class_method_by_regex should not find a match to `nonexistent_method`"
+        )
+        print("OK")
+        print("-----[ TEST END   ]--------------------------------------------------\n")
+
+        print("-----[ TEST START ]--------------------------------------------------")
+        print(">>> Test case when a non-string parameter is provided")
+        with self.assertRaises(TypeError):
+            rval_actual = parser._locate_class_method(None)
+        print("OK")
+        print("-----[ TEST END   ]--------------------------------------------------\n")
+
+        print("OK")
+        return 0
+
 
 
 # ===========================================================
 #   Test ActiveConfigParserDataTest
 # ===========================================================
```

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_HandlerParameters.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/unittests/test_HandlerParameters.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.1/src/activeconfigparser/version.py` & `activeconfigparser-0.9.1.0/src/activeconfigparser/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #===============================================================================
 """
 """
 
 # Note, when updating this, the docstring in ActiveConfigParser
 # and in pyproject.toml should also be updated
-__version__ = "0.9.0.1"
+__version__ = "0.9.1.0"
```

### Comparing `activeconfigparser-0.9.0.1/PKG-INFO` & `activeconfigparser-0.9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activeconfigparser
-Version: 0.9.0.1
+Version: 0.9.1.0
 Summary: A tool that extends configparser to enable enhanced processing of .ini files.
 Home-page: https://gitlab.com/semantik-software/code/python/ActiveConfigParser
 License: LICENSE
 Keywords: Utility,Bash,Configuration,ActiveConfigParser,ConfigParser
 Author: William
 Author-email: Semantik-Codeworks@outlook.com
 Maintainer: William
```

