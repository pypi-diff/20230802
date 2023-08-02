# Comparing `tmp/efrem_utils-0.2.1.tar.gz` & `tmp/efrem_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.2.1.tar", max compression
+gzip compressed data, was "efrem_utils-0.2.2.tar", max compression
```

## Comparing `efrem_utils-0.2.1.tar` & `efrem_utils-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11332 2023-08-02 12:54:32.674919 efrem_utils-0.2.1/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.2.1/LICENSE
--rw-r--r--   0        0        0      361 2023-08-02 14:45:31.768880 efrem_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.2.1/README.md
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11573 2023-08-02 15:41:28.245768 efrem_utils-0.2.2/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.2.2/LICENSE
+-rw-r--r--   0        0        0      361 2023-08-02 15:41:26.866041 efrem_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-08-01 19:41:39.325507 efrem_utils-0.2.2/README.md
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 efrem_utils-0.2.2/PKG-INFO
```

### Comparing `efrem_utils-0.2.1/efrem_utils.py` & `efrem_utils-0.2.2/efrem_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,17 +128,17 @@
                 case _TestMode.normal_case:
                     # in a normal case, we just call the function with the provided arguments, and check if the result matches expectations
                     try:
                         result = function(*args, **kwargs) if kwargs else function(*args)
                         callable_expect = callable(expect)
                         expectation_passed = expect(result) if callable_expect else expect == result
                         if expectation_passed:
-                            print(f"\x1B[38;5;154mTest passed: {info} -> {result} {f'so {expect.__name__}({result}) was truthy' if callable_expect else f'== {expect}'}\x1B[0m")
+                            print(f"\x1B[38;5;154mTest passed: {info} -> {repr(result)} {f'so {expect.__name__}({repr(result)}) was truthy' if callable_expect else f'== {repr(expect)}'}\x1B[0m")
                         else:
-                            print(f"\x1B[38;5;196mTest failed: {info} -> {result} {f'so {expect.__name__}({result}) was falsy' if callable_expect else f'instead of {expect}'}\x1B[0m")
+                            print(f"\x1B[38;5;196mTest failed: {info} -> {repr(result)} {f'so {expect.__name__}({repr(result)}) was falsy' if callable_expect else f'instead of {expect}'}\x1B[0m")
                             
                     except Exception as exc:
                         # something gone wrong, because this is not an exception test, so the test basically "failed"
                         print(f"\x1B[38;5;99mTest raised an exception: {info} -> {repr(exc)}\x1B[0m")
                 
                 case _TestMode.case_test:
 
@@ -177,18 +177,18 @@
 
                     match expect.mode:
 
                         case Case._Mode.match:
 
                             if result_0 == result_1:
                                 # Match passed
-                                print(f"\x1B[38;5;154mMatch case passed: {info} == {buf_info} -> {result_0} | {result_1}\x1B[0m")
+                                print(f"\x1B[38;5;154mMatch case passed: {info} == {buf_info} -> {repr(result_0)} | {repr(result_1)}\x1B[0m")
                             else:
                                 # Match failed
-                                print(f"\x1B[38;5;196mMatch case failed: {info} -> {result_0} ; {buf_info} -> {result_1}\x1B[0m")
+                                print(f"\x1B[38;5;196mMatch case failed: {info} -> {repr(result_0)} ; {buf_info} -> {repr(result_1)}\x1B[0m")
 
                         case Case._Mode.validate:
                             
                             buf_res: Any = expect.validator(result_0, result_1)
                             buf_info: str = f"{expect.validator.__name__}({repr(result_0)}, {repr(result_1)})"
 
                             if buf_res:
@@ -199,15 +199,15 @@
                                 print(f"\x1B[38;5;196mValidation case failed: {buf_info} -> {buf_res} [is falsy]\x1B[0m")
 
 
                 case _TestMode.exception_test:
                     # in an exception test, we call the function with the provided arguments, and see if the catched expection matches the expected one.
                     try:
                         result = function(*args, **kwargs) if kwargs else function(*args)
-                        print(f"\x1B[38;5;202mException test didnt result in an exception {info} -> {result} instead of raising {repr(expect())}\x1B[0m")
+                        print(f"\x1B[38;5;202mException test didnt result in an exception {info} -> {repr(result)} instead of raising {repr(expect())}\x1B[0m")
                     except Exception as exc:
                         if type(exc) == expect:
                             print(f"\x1B[38;5;50mException test passed: {info} -> {repr(exc)}\x1B[0m")
                         else:
                             print(f"\x1B[38;5;196mException test failed: {info} -> {repr(exc)} instead of {repr(expect())}\x1B[0m")
 
         def test_cases() -> None:
@@ -220,8 +220,11 @@
                         parse_case(args=test_case[0], expect=test_case[1])
                 elif len(test_case) == 3: parse_case(args=test_case[0], kwargs=test_case[1], expect=test_case[2])
 
         test_cases()
 
         return function
     
-    return parametrized_decorator
+    return parametrized_decorator
+
+def parametrized_wrap(inputs: list[Any] | tuple[Any], outputs: list[Any] | tuple[Any]):
+    return parametrized(expected_io=[([arg], ans) for arg, ans in zip(inputs, outputs)])
```

### Comparing `efrem_utils-0.2.1/LICENSE` & `efrem_utils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.2.1/README.md` & `efrem_utils-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.2.1/PKG-INFO` & `efrem_utils-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

