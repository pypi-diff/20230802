# Comparing `tmp/pyrtlsdr-0.2.93.tar.gz` & `tmp/pyrtlsdr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtlsdr-0.2.93.tar", last modified: Mon Aug  1 22:10:37 2022, max compression
+gzip compressed data, was "pyrtlsdr-0.3.0.tar", last modified: Wed Aug  2 19:17:46 2023, max compression
```

## Comparing `pyrtlsdr-0.2.93.tar` & `pyrtlsdr-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 22:10:37.335279 pyrtlsdr-0.2.93/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-08-01 22:10:37.335279 pyrtlsdr-0.2.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6961 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/demo_waterfall.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 22:10:37.331279 pyrtlsdr-0.2.93/pyrtlsdr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-08-01 22:10:37.000000 pyrtlsdr-0.2.93/pyrtlsdr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-08-01 22:10:37.000000 pyrtlsdr-0.2.93/pyrtlsdr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 22:10:37.000000 pyrtlsdr-0.2.93/pyrtlsdr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-01 22:10:37.000000 pyrtlsdr-0.2.93/pyrtlsdr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 22:10:37.335279 pyrtlsdr-0.2.93/rtlsdr/
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/librtlsdr.py
--rw-r--r--   0 runner    (1001) docker     (121)    25992 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/rtlsdr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6385 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/rtlsdraio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 22:10:37.335279 pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9214 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7909 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/server.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-01 22:10:37.339280 pyrtlsdr-0.2.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-08-01 22:10:28.000000 pyrtlsdr-0.2.93/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/demo_waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/pyrtlsdr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-08-02 19:17:46.000000 pyrtlsdr-0.3.0/pyrtlsdr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-02 19:17:46.000000 pyrtlsdr-0.3.0/pyrtlsdr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:17:46.000000 pyrtlsdr-0.3.0/pyrtlsdr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-02 19:17:46.000000 pyrtlsdr-0.3.0/pyrtlsdr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 19:17:46.000000 pyrtlsdr-0.3.0/pyrtlsdr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/rtlsdr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/librtlsdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/rtlsdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/rtlsdraio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9214 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:17:46.468081 pyrtlsdr-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/tests/test_aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/tests/test_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-08-02 19:17:42.000000 pyrtlsdr-0.3.0/tests/testlibrtlsdr.py
```

### Comparing `pyrtlsdr-0.2.93/PKG-INFO` & `pyrtlsdr-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtlsdr
-Version: 0.2.93
+Version: 0.3.0
 Summary: A Python wrapper for librtlsdr (a driver for Realtek RTL2832U based SDR's)
 Home-page: https://github.com/pyrtlsdr/pyrtlsdr
 Author: roger
 License: GPLv3
 Project-URL: Documentation, https://pyrtlsdr.readthedocs.io/
 Project-URL: Source, https://github.com/pyrtlsdr/pyrtlsdr
 Keywords: radio librtlsdr rtlsdr sdr
@@ -14,20 +14,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Provides-Extra: lib
 
 # pyrtlsdr
 A Python wrapper for librtlsdr (a driver for Realtek RTL2832U based SDR's)
 
 [![PyPI](https://img.shields.io/pypi/v/pyrtlsdr)](https://pypi.org/project/pyrtlsdr) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/pyrtlsdr/pyrtlsdr/Python%20package) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyrtlsdr) [![Coveralls](https://img.shields.io/coveralls/github/pyrtlsdr/pyrtlsdr)](https://coveralls.io/github/pyrtlsdr/pyrtlsdr)
 
 # Description
@@ -44,19 +45,40 @@
 * Releases:
   * https://pypi.org/project/pyrtlsdr/
 * Source code and project home:
   * https://github.com/pyrtlsdr/pyrtlsdr
 * Releases for `librtlsdr`:
   * https://github.com/librtlsdr/librtlsdr/releases
 
-# Usage
+# Installation
 
 pyrtlsdr can be installed by downloading the source files and running `python setup.py install`, or using [pip](https://pip.pypa.io/en/stable/) and
 `pip install pyrtlsdr`.
 
+## Full installation (recommended)
+
+**New in version 0.3.0**
+
+On most platforms, the `librtlsdr` binaries may be also installed with the [pyrtlsdrlib](https://github.com/pyrtlsdr/pyrtlsdrlib) package.  This new feature should *drastically* simplify the installation process (especially for Windows).
+
+This can be done by installing `pyrtlsdrlib` separately (via pip) or for simplicity, both can be installed at once via:
+
+```bash
+pip install pyrtlsdr[lib]
+```
+
+If errors are encountered with the `pyrtlsdrlib` integration (during installation or package import),
+you may want to ensure you have the latest versions of both:
+
+```bash
+pip install --upgrade pyrtlsdr[lib]
+```
+
+# Usage
+
 All functions in librtlsdr are accessible via librtlsdr.py and a Pythonic interface is available in rtlsdr.py (recommended).
 Some documentation can be found in docstrings in the latter file.
 
 ## Examples
 
 ### Simple way to read and print some samples:
 
@@ -195,15 +217,19 @@
 function you need to add support for, and please send a pull request if you'd like to share your changes.
 
 # Troubleshooting
 
 * Some operating systems (Linux, OS X) seem to result in libusb buffer issues when performing small reads. Try reading 1024
 (or higher powers of two) samples at a time if you have problems.
 
-* If you're having librtlsdr import errors:
+## librtlsdr import errors
+
+First try upgrading `pyrtlsdr` and using the `pyrtlsdrlib` helper package described above.
+
+* In cases where that isn't feasible:
   * **Windows**: Make sure all the librtlsdr DLL files (librtlsdr.dll, libusb-1.0.dll) are in your system path, or the same folder
 as this README file. Also make sure you have all of *their* dependencies (e.g. libgcc_s_dw2-1.dll or possibly the Visual Studio runtime files). If rtl_sdr.exe
 works, then you should be okay. Also note that you can't mix the 64 bit version of Python with 32 bit builds of librtlsdr, and vice versa.
   * **Linux**: Make sure your LD_LIBRARY_PATH environment variable contains the directory where the librtlsdr.so.0 library is located. You can do this in a shell with (for example): `export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib`. See [this issue](https://github.com/roger-/pyrtlsdr/issues/7) for more details.
 
 # License
```

### Comparing `pyrtlsdr-0.2.93/README.md` & `pyrtlsdr-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,40 @@
 * Releases:
   * https://pypi.org/project/pyrtlsdr/
 * Source code and project home:
   * https://github.com/pyrtlsdr/pyrtlsdr
 * Releases for `librtlsdr`:
   * https://github.com/librtlsdr/librtlsdr/releases
 
-# Usage
+# Installation
 
 pyrtlsdr can be installed by downloading the source files and running `python setup.py install`, or using [pip](https://pip.pypa.io/en/stable/) and
 `pip install pyrtlsdr`.
 
+## Full installation (recommended)
+
+**New in version 0.3.0**
+
+On most platforms, the `librtlsdr` binaries may be also installed with the [pyrtlsdrlib](https://github.com/pyrtlsdr/pyrtlsdrlib) package.  This new feature should *drastically* simplify the installation process (especially for Windows).
+
+This can be done by installing `pyrtlsdrlib` separately (via pip) or for simplicity, both can be installed at once via:
+
+```bash
+pip install pyrtlsdr[lib]
+```
+
+If errors are encountered with the `pyrtlsdrlib` integration (during installation or package import),
+you may want to ensure you have the latest versions of both:
+
+```bash
+pip install --upgrade pyrtlsdr[lib]
+```
+
+# Usage
+
 All functions in librtlsdr are accessible via librtlsdr.py and a Pythonic interface is available in rtlsdr.py (recommended).
 Some documentation can be found in docstrings in the latter file.
 
 ## Examples
 
 ### Simple way to read and print some samples:
 
@@ -168,15 +189,19 @@
 function you need to add support for, and please send a pull request if you'd like to share your changes.
 
 # Troubleshooting
 
 * Some operating systems (Linux, OS X) seem to result in libusb buffer issues when performing small reads. Try reading 1024
 (or higher powers of two) samples at a time if you have problems.
 
-* If you're having librtlsdr import errors:
+## librtlsdr import errors
+
+First try upgrading `pyrtlsdr` and using the `pyrtlsdrlib` helper package described above.
+
+* In cases where that isn't feasible:
   * **Windows**: Make sure all the librtlsdr DLL files (librtlsdr.dll, libusb-1.0.dll) are in your system path, or the same folder
 as this README file. Also make sure you have all of *their* dependencies (e.g. libgcc_s_dw2-1.dll or possibly the Visual Studio runtime files). If rtl_sdr.exe
 works, then you should be okay. Also note that you can't mix the 64 bit version of Python with 32 bit builds of librtlsdr, and vice versa.
   * **Linux**: Make sure your LD_LIBRARY_PATH environment variable contains the directory where the librtlsdr.so.0 library is located. You can do this in a shell with (for example): `export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib`. See [this issue](https://github.com/roger-/pyrtlsdr/issues/7) for more details.
 
 # License
```

### Comparing `pyrtlsdr-0.2.93/demo_waterfall.py` & `pyrtlsdr-0.3.0/demo_waterfall.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/pyrtlsdr.egg-info/PKG-INFO` & `pyrtlsdr-0.3.0/pyrtlsdr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtlsdr
-Version: 0.2.93
+Version: 0.3.0
 Summary: A Python wrapper for librtlsdr (a driver for Realtek RTL2832U based SDR's)
 Home-page: https://github.com/pyrtlsdr/pyrtlsdr
 Author: roger
 License: GPLv3
 Project-URL: Documentation, https://pyrtlsdr.readthedocs.io/
 Project-URL: Source, https://github.com/pyrtlsdr/pyrtlsdr
 Keywords: radio librtlsdr rtlsdr sdr
@@ -14,20 +14,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Provides-Extra: lib
 
 # pyrtlsdr
 A Python wrapper for librtlsdr (a driver for Realtek RTL2832U based SDR's)
 
 [![PyPI](https://img.shields.io/pypi/v/pyrtlsdr)](https://pypi.org/project/pyrtlsdr) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/pyrtlsdr/pyrtlsdr/Python%20package) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyrtlsdr) [![Coveralls](https://img.shields.io/coveralls/github/pyrtlsdr/pyrtlsdr)](https://coveralls.io/github/pyrtlsdr/pyrtlsdr)
 
 # Description
@@ -44,19 +45,40 @@
 * Releases:
   * https://pypi.org/project/pyrtlsdr/
 * Source code and project home:
   * https://github.com/pyrtlsdr/pyrtlsdr
 * Releases for `librtlsdr`:
   * https://github.com/librtlsdr/librtlsdr/releases
 
-# Usage
+# Installation
 
 pyrtlsdr can be installed by downloading the source files and running `python setup.py install`, or using [pip](https://pip.pypa.io/en/stable/) and
 `pip install pyrtlsdr`.
 
+## Full installation (recommended)
+
+**New in version 0.3.0**
+
+On most platforms, the `librtlsdr` binaries may be also installed with the [pyrtlsdrlib](https://github.com/pyrtlsdr/pyrtlsdrlib) package.  This new feature should *drastically* simplify the installation process (especially for Windows).
+
+This can be done by installing `pyrtlsdrlib` separately (via pip) or for simplicity, both can be installed at once via:
+
+```bash
+pip install pyrtlsdr[lib]
+```
+
+If errors are encountered with the `pyrtlsdrlib` integration (during installation or package import),
+you may want to ensure you have the latest versions of both:
+
+```bash
+pip install --upgrade pyrtlsdr[lib]
+```
+
+# Usage
+
 All functions in librtlsdr are accessible via librtlsdr.py and a Pythonic interface is available in rtlsdr.py (recommended).
 Some documentation can be found in docstrings in the latter file.
 
 ## Examples
 
 ### Simple way to read and print some samples:
 
@@ -195,15 +217,19 @@
 function you need to add support for, and please send a pull request if you'd like to share your changes.
 
 # Troubleshooting
 
 * Some operating systems (Linux, OS X) seem to result in libusb buffer issues when performing small reads. Try reading 1024
 (or higher powers of two) samples at a time if you have problems.
 
-* If you're having librtlsdr import errors:
+## librtlsdr import errors
+
+First try upgrading `pyrtlsdr` and using the `pyrtlsdrlib` helper package described above.
+
+* In cases where that isn't feasible:
   * **Windows**: Make sure all the librtlsdr DLL files (librtlsdr.dll, libusb-1.0.dll) are in your system path, or the same folder
 as this README file. Also make sure you have all of *their* dependencies (e.g. libgcc_s_dw2-1.dll or possibly the Visual Studio runtime files). If rtl_sdr.exe
 works, then you should be okay. Also note that you can't mix the 64 bit version of Python with 32 bit builds of librtlsdr, and vice versa.
   * **Linux**: Make sure your LD_LIBRARY_PATH environment variable contains the directory where the librtlsdr.so.0 library is located. You can do this in a shell with (for example): `export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib`. See [this issue](https://github.com/roger-/pyrtlsdr/issues/7) for more details.
 
 # License
```

### Comparing `pyrtlsdr-0.2.93/rtlsdr/__init__.py` & `pyrtlsdr-0.3.0/rtlsdr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/helpers.py` & `pyrtlsdr-0.3.0/rtlsdr/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/librtlsdr.py` & `pyrtlsdr-0.3.0/rtlsdr/librtlsdr.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,25 @@
 
 
 import sys
 import os
 from ctypes import *
 from ctypes.util import find_library
 
+try:
+    import pyrtlsdrlib
+except ImportError:
+    pyrtlsdrlib = None
+
 def load_librtlsdr():
+    # If pyrtlsdrlib is intalled try its loader first
+    if pyrtlsdrlib is not None:
+        dll = pyrtlsdrlib.load_librtlsdr()
+        if dll is not None:
+            return dll
     if sys.platform == "linux" and 'LD_LIBRARY_PATH' in os.environ.keys():
         ld_library_paths = [local_path for local_path in os.environ['LD_LIBRARY_PATH'].split(':') if local_path.strip()]
         driver_files = [local_path + '/librtlsdr.so' for local_path in ld_library_paths]
     else:
         driver_files = []
     driver_files += ['librtlsdr.so', 'rtlsdr/librtlsdr.so']
     driver_files += ['rtlsdr.dll', 'librtlsdr.so', 'librtlsdr.dylib']
```

### Comparing `pyrtlsdr-0.2.93/rtlsdr/rtlsdr.py` & `pyrtlsdr-0.3.0/rtlsdr/rtlsdr.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/rtlsdraio.py` & `pyrtlsdr-0.3.0/rtlsdr/rtlsdraio.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/__init__.py` & `pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/base.py` & `pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/base.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/client.py` & `pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/client.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/rtlsdr/rtlsdrtcp/server.py` & `pyrtlsdr-0.3.0/rtlsdr/rtlsdrtcp/server.py`

 * *Files identical despite different names*

### Comparing `pyrtlsdr-0.2.93/setup.py` & `pyrtlsdr-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 import sys
 import re
 import shutil
 from setuptools import setup, find_packages
 
 PACKAGE_NAME = 'pyrtlsdr'
-VERSION = '0.2.93'
+VERSION = '0.3.0'
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__))
 IS_RTDBUILD = os.environ.get('READTHEDOCS', '').lower() == 'true'
 
 if IS_RTDBUILD:
     # copy a mocked wrapper since we can't build librtlsdr on rtfd
     def copy_mock_librtlsdr():
@@ -55,16 +55,16 @@
                  'Intended Audience :: Developers',
                  'License :: OSI Approved :: GNU General Public License (GPL)',
                  'Natural Language :: English',
                  'Operating System :: OS Independent',
                  'Programming Language :: Python :: 2',
                  'Programming Language :: Python :: 2.7',
                  'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7',
+                 'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11',
                  'Topic :: Utilities'],
     license='GPLv3',
     keywords='radio librtlsdr rtlsdr sdr',
     platforms=['any'],
     packages=find_packages(exclude=['tests*']))
```

### Comparing `pyrtlsdr-0.2.93/test.py` & `pyrtlsdr-0.3.0/test.py`

 * *Files identical despite different names*

