# Comparing `tmp/efrem_utils-0.1.4.tar.gz` & `tmp/efrem_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.1.4.tar", max compression
+gzip compressed data, was "efrem_utils-0.1.5.tar", max compression
```

## Comparing `efrem_utils-0.1.4.tar` & `efrem_utils-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4851 2023-08-01 22:38:19.152696 efrem_utils-0.1.4/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.4/LICENSE
--rw-r--r--   0        0        0      361 2023-08-01 22:33:01.973091 efrem_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.1.4/README.md
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4683 2023-08-01 22:52:36.611027 efrem_utils-0.1.5/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.5/LICENSE
+-rw-r--r--   0        0        0      361 2023-08-01 22:53:36.708740 efrem_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.1.5/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.1.5/PKG-INFO
```

### Comparing `efrem_utils-0.1.4/efrem_utils.py` & `efrem_utils-0.1.5/efrem_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,46 +60,43 @@
                     break
 
             else: # if no break happens in validation checking - return
                 return constructor(buffer)
                 
     return inner
 
+# --- #
+
 def parametrized(expected_io: list[tuple], unpack_args: bool = False): # currently undocumented, will get hands on it later
 
     def parametrized_decorator(function):
 
         def inner():
             for arg_s, expected in expected_io:
 
                 try:
 
                     if unpack_args: res = function(*arg_s)
                     else: res = function(arg_s)
-
-                    condition = expected(res) if callable(expected) else res==expected
-                    if condition: 
-                        if callable(expected):
-                            print(f"\x1B[38;5;154mCallable test passed: {expected.__name__}({function.__name__}({repr(arg_s)})) is truthy\x1B[0m")
-                        else:
-                            print(f"\x1B[38;5;154mTest passed: {function.__name__}({repr(arg_s)}) == {repr(expected)}\x1B[0m")
+                    
+                    pass_condition: bool = expected(res) if callable(expected) else res==expected
+                    if pass_condition: 
+                        if callable(expected): print(f"\x1B[38;5;154mCallable test passed: {expected.__name__}({function.__name__}({repr(arg_s)})) is truthy\x1B[0m")
+                        else: print(f"\x1B[38;5;154mTest passed: {function.__name__}({repr(arg_s)}) == {repr(expected)}\x1B[0m")
 
                     else:
-                        if callable(expected):
-                            print(f"\x1B[38;5;196mCallable test failed: {expected.__name__}({function.__name__}({repr(arg_s)})) is falsy\x1B[0m")
-                        else:
-                            print(f"\x1B[38;5;196mTest failed: {function.__name__}({repr(arg_s)}) == {repr(res)} instead of {expected}\x1B[0m")
+                        if callable(expected): print(f"\x1B[38;5;196mCallable test failed: {expected.__name__}({function.__name__}({repr(arg_s)})) is falsy\x1B[0m")
+                        else: print(f"\x1B[38;5;196mTest failed: {function.__name__}({repr(arg_s)}) == {repr(res)} instead of {expected}\x1B[0m")
 
                 except Exception as exc:
-                    exception_test = isinstance(expected(res)() if callable(expected) else expected(), Exception)
+
+                    exception_test = isinstance(expected(), Exception)
                     if exception_test:
-                        if type(exc) == expected:
-                            print(f"\x1B[38;5;154mException test passed: {function.__name__}({repr(arg_s)}) raised << {type(exc)} >>\x1B[0m")
-                        else:
-                            print(f"\x1B[38;5;129mException test failed: {function.__name__}({repr(arg_s)}) raised << {type(exc)} >> instead of << {expected}>> \x1B[0m")
+                        if type(exc) == expected: print(f"\x1B[38;5;154mException test passed: {function.__name__}({repr(arg_s)}) raised << {type(exc)} >>\x1B[0m")
+                        else: print(f"\x1B[38;5;129mException test failed: {function.__name__}({repr(arg_s)}) raised << {type(exc)} >> instead of << {expected}>> \x1B[0m")
                     else:
                         print(f"\x1B[38;5;129mTest raised an exception: {function.__name__}({repr(arg_s)}) raised << {type(exc)} >>\x1B[0m")
 
         if __name__ in ("__main__", "efrem_utils"):
             inner() # yes
 
         return function
```

### Comparing `efrem_utils-0.1.4/LICENSE` & `efrem_utils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.1.4/README.md` & `efrem_utils-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.1.4/PKG-INFO` & `efrem_utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

