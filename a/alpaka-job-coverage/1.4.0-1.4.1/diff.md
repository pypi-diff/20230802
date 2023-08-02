# Comparing `tmp/alpaka-job-coverage-1.4.0.tar.gz` & `tmp/alpaka-job-coverage-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.4.0.tar", last modified: Tue Aug  1 10:25:32 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.4.1.tar", last modified: Wed Aug  2 11:12:32 2023, max compression
```

## Comparing `alpaka-job-coverage-1.4.0.tar` & `alpaka-job-coverage-1.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.847143 alpaka-job-coverage-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:25:32.847143 alpaka-job-coverage-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.835143 alpaka-job-coverage-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12111 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 10:25:32.000000 alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:25:32.843143 alpaka-job-coverage-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 10:25:13.000000 alpaka-job-coverage-1.4.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.557951 alpaka-job-coverage-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.561951 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12111 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.561951 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 11:12:32.000000 alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:12:32.565951 alpaka-job-coverage-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 11:12:15.000000 alpaka-job-coverage-1.4.1/version.txt
```

### Comparing `alpaka-job-coverage-1.4.0/LICENSE` & `alpaka-job-coverage-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/PKG-INFO` & `alpaka-job-coverage-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.4.0
+Version: 1.4.1
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.4.0/README.md` & `alpaka-job-coverage-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/setup.py` & `alpaka-job-coverage-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,16 +84,19 @@
     if row_check_name(row, DEVICE_COMPILER, "==", NVCC):
         cuda_sdk_version = 0
         cuda_host_compiler_version = 1
 
         # set the and lowest highest supported gcc version for nvcc
         if row_check_name(row, HOST_COMPILER, "==", GCC):
             combinations = [
+                # it needs to be defined the CUDA SDK version, which supports
+                # a new gcc version the first time
+                # the latest CUDA SDK, also if it supports no new gcc version
                 # (maximum_CUDA_SDK_version, "maximum_gcc_version")
-                ("12.1", "12"),
+                ("12.2", "12"),
                 ("12.0", "12"),
                 ("11.4", "11"),
                 ("11.1", "10"),
                 ("11.0", "9"),
                 ("10.1", "8"),
                 ("10.0", "7"),
             ]
@@ -140,15 +143,19 @@
                 reason(
                     output,
                     "clang as host compiler is disabled for nvcc-11.3 to 11.5",
                 )
                 return False
 
             combinations = [
+                # it needs to be defined the CUDA SDK version, which supports
+                # a new clang version the first time
+                # the latest CUDA SDK, also if it supports no new clang version
                 # (maximum_CUDA_SDK_version, "maximum_clang_version")
+                ("12.2", "15"),
                 ("12.1", "15"),
                 ("12.0", "14"),
                 ("11.6", "13"),
                 ("11.4", "12"),
                 ("11.2", "11"),
                 ("11.1", "10"),
                 ("11.0", "9"),
```

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         parsed_nvcc_version = pk_version.parse(row[param_map[DEVICE_COMPILER]][VERSION])
 
         # definition of the tuple values: if the nvcc version of the first
         # tuple is older than the cxx standard of the second value, it is not supported
         nvcc_cxx_versions = [
             ("11.0", 17),  # NVCC versions older than 11.0 does not support C++ 17
             ("12.0", 20),  # NVCC versions older than 12.0 does not support C++ 20
-            ("12.2", 23),  # NVCC 12.2 is not released yet, therefore we need to
+            ("12.3", 23),  # NVCC 12.3 is not released yet, therefore we need to
             # expect that it could support C++23
         ]
         for nvcc_version, cxx_version in nvcc_cxx_versions:
             if (
                 parsed_nvcc_version < pk_version.parse(nvcc_version)
                 and int(row[param_map[CXX_STANDARD]][VERSION]) >= cxx_version
             ):
```

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -313,45 +313,14 @@
             new_job_list.insert(0, job)
         else:
             new_job_list.append(job)
 
     return new_job_list
 
 
-@typechecked
-def is_supported_sw_version(name: str, version: str, verbose=True) -> bool:
-    def warning_text(text: str):
-        return "\033[1;33mWARNING: " + text + "\033[0m"
-
-    support_versions: Dict[str, Tuple[str, str]] = {
-        GCC: ("5", "13"),
-        CLANG: ("6.0", "15"),
-        NVCC: ("10.0", "12.1"),
-        HIPCC: ("4.3", "5.1"),
-        CMAKE: ("3.18", "3.22"),
-        BOOST: ("1.66.0", "1.78.0"),
-        CXX_STANDARD: ("14", "20"),
-    }
-
-    if name not in support_versions:
-        if verbose:
-            print(warning_text(f"{name} is an unknown software"))
-        return False
-    else:
-        parsed_version = pk_version.parse(version)
-        if parsed_version < pk_version.parse(
-            support_versions[name][0]
-        ) or parsed_version > pk_version.parse(support_versions[name][1]):
-            if verbose:
-                print(warning_text(f"{name} {version} is not supported"))
-            return False
-
-    return True
-
-
 def reason(output: Optional[Union[io.StringIO, io.TextIOWrapper]], msg: str):
     """Write the message to output if it is not None. This function is used
     in filter functions to print additional information about filter decisions.
 
     Args:
         output (Optional[Union[io.StringIO, io.TextIOWrapper]]): IO object.
         Can be io.StringIO, sys.stdout sys.stderr
```

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/validate.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/validate.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage/versions.py` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage/versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # This dict contains all software version, which we handle we the filter rules.
 # Not every software version results in a case in the filter rules. For example
 # we have no case, where a combination with a specific Boost version needs to be
 # disabled (date: 26.7.2023). Maybe in future, a Boost specific case will be
 # added.
 versions: Dict[str, List[str]] = {
-    GCC: ["6", "7", "8", "9", "10", "11", "12"],
+    GCC: ["6", "7", "8", "9", "10", "11", "12", "13"],
     CLANG: ["6", "7", "8", "9", "10", "11", "12", "13", "14", "15", "16"],
     NVCC: [
         "10.0",
         "10.1",
         "10.2",
         "11.0",
         "11.1",
@@ -23,14 +23,15 @@
         "11.4",
         "11.5",
         "11.6",
         "11.7",
         "11.8",
         "12.0",
         "12.1",
+        "12.2",
     ],
     HIPCC: ["5.0", "5.1", "5.2", "5.3", "5.4", "5.5"],
     UBUNTU: ["18.04", "20.04"],
     CMAKE: ["3.18", "3.19", "3.20", "3.21", "3.22", "3.23", "3.24", "3.25", "3.26"],
     BOOST: [
         "1.74.0",
         "1.75.0",
```

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.4.0
+Version: 1.4.1
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.4.0/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.4.1/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/tests/test_compiler_names.py` & `alpaka-job-coverage-1.4.1/tests/test_compiler_names.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.4.1/tests/test_cuda_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,14 +368,16 @@
             ("11.7", "12", False),
             ("11.8", "11", True),
             ("11.8", "12", False),
             ("12.0", "12", True),
             ("12.0", "13", False),
             ("12.1", "12", True),
             ("12.1", "13", False),
+            ("12.2", "12", True),
+            ("12.2", "13", False),
         ]
 
         for nvcc_version, gcc_version, expected_value in expected_results:
             self.assertEqual(
                 compiler_version_filter_typed(
                     [(NVCC, nvcc_version), (GCC, gcc_version)]
                 ),
@@ -448,14 +450,16 @@
             ("11.7", "14", False),
             ("11.8", "13", True),
             ("11.8", "14", False),
             ("12.0", "14", True),
             ("12.0", "15", False),
             ("12.1", "15", True),
             ("12.1", "16", False),
+            ("12.2", "15", True),
+            ("12.2", "16", False),
         ]
 
         for nvcc_version, clang_version, expected_value in expected_results:
             self.assertEqual(
                 compiler_version_filter_typed(
                     [(NVCC, nvcc_version), (CLANG, clang_version)]
                 ),
@@ -509,18 +513,18 @@
         manual_version_test(self, NVCC, [], ["12.2, 45.0"])
 
         for nvcc_version, max_cxx in [
             ("11.0", 17),
             ("11.2", 17),
             ("11.8", 17),
             ("12.0", 20),
-            ("12.1", 20),
+            ("12.2", 20),
             # not released version
             # therefore they should support all C++ versions
-            ("12.2", 32),
+            ("12.3", 32),
             ("45.0", 32),
         ]:
             for cxx_version in [11, 14, 17, 20, 23, 26, 29, 32]:
                 comb = [(NVCC, nvcc_version), (CXX_STANDARD, str(cxx_version))]
                 if cxx_version <= max_cxx:
                     self.assertTrue(
                         software_dependency_filter_typed(comb),
```

### Comparing `alpaka-job-coverage-1.4.0/tests/test_hipcc.py` & `alpaka-job-coverage-1.4.1/tests/test_hipcc.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/tests/test_single_rules.py` & `alpaka-job-coverage-1.4.1/tests/test_single_rules.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/tests/test_util.py` & `alpaka-job-coverage-1.4.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.4.0/tests/test_versions.py` & `alpaka-job-coverage-1.4.1/tests/test_versions.py`

 * *Files identical despite different names*

