# Comparing `tmp/zeroconf-0.71.4.tar.gz` & `tmp/zeroconf-0.71.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.71.4.tar", max compression
+gzip compressed data, was "zeroconf-0.71.5.tar", max compression
```

## Comparing `zeroconf-0.71.4.tar` & `zeroconf-0.71.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    56117 2023-07-24 16:13:08.265268 zeroconf-0.71.4/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-07-24 16:13:07.129202 zeroconf-0.71.4/COPYING
--rw-r--r--   0        0        0     4407 2023-07-24 16:13:07.129202 zeroconf-0.71.4/README.rst
--rw-r--r--   0        0        0     1060 2023-07-24 16:13:07.129202 zeroconf-0.71.4/build_ext.py
--rw-r--r--   0        0        0     6770 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/Makefile
--rw-r--r--   0        0        0      234 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/conf.py
--rw-r--r--   0        0        0      991 2023-07-24 16:13:07.129202 zeroconf-0.71.4/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-07-24 16:13:08.365274 zeroconf-0.71.4/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-07-24 16:13:08.281269 zeroconf-0.71.4/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      897 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0    10040 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39600 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2119 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18270 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    24697 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2661 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14353 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     2317 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17896 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2419 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    23045 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    27841 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3999 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4515 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-07-24 16:13:07.133203 zeroconf-0.71.4/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-07-24 16:13:07.133203 zeroconf-0.71.4/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-07-24 16:13:07.133203 zeroconf-0.71.4/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/__init__.py
--rw-r--r--   0        0        0    42949 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_browser.py
--rw-r--r--   0        0        0    47563 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_registry.py
--rw-r--r--   0        0        0     4681 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/services/test_types.py
--rw-r--r--   0        0        0    44525 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_cache.py
--rw-r--r--   0        0        0    32599 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_dns.py
--rw-r--r--   0        0        0     5021 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_exceptions.py
--rw-r--r--   0        0        0    67411 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-07-24 16:13:07.137203 zeroconf-0.71.4/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.71.4/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.71.4/PKG-INFO
+-rw-r--r--   0        0        0    56391 2023-08-02 00:43:33.296290 zeroconf-0.71.5/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-08-02 00:43:32.492277 zeroconf-0.71.5/COPYING
+-rw-r--r--   0        0        0     4407 2023-08-02 00:43:32.492277 zeroconf-0.71.5/README.rst
+-rw-r--r--   0        0        0     1060 2023-08-02 00:43:32.492277 zeroconf-0.71.5/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-08-02 00:43:32.492277 zeroconf-0.71.5/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-08-02 00:43:32.492277 zeroconf-0.71.5/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-08-02 00:43:32.492277 zeroconf-0.71.5/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-08-02 00:43:32.492277 zeroconf-0.71.5/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-08-02 00:43:33.376291 zeroconf-0.71.5/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-08-02 00:43:33.308290 zeroconf-0.71.5/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10040 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39600 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2119 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18270 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24697 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14353 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     2317 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17896 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2419 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    23045 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    28130 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3999 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-08-02 00:43:32.496277 zeroconf-0.71.5/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-08-02 00:43:32.496277 zeroconf-0.71.5/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-08-02 00:43:32.496277 zeroconf-0.71.5/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-08-02 00:43:32.496277 zeroconf-0.71.5/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-08-02 00:43:32.496277 zeroconf-0.71.5/tests/services/test_browser.py
+-rw-r--r--   0        0        0    49788 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4677 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_cache.py
+-rw-r--r--   0        0        0    32599 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-08-02 00:43:32.500277 zeroconf-0.71.5/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.71.5/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.71.5/PKG-INFO
```

### Comparing `zeroconf-0.71.4/CHANGELOG.md` & `zeroconf-0.71.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.71.5 (2023-08-02)
+
+### Fix
+
+* Improve performance of ServiceInfo.async_request ([#1205](https://github.com/python-zeroconf/python-zeroconf/issues/1205)) ([`8019a73`](https://github.com/python-zeroconf/python-zeroconf/commit/8019a73c952f2fc4c88d849aab970fafedb316d8))
+
 ## v0.71.4 (2023-07-24)
 
 ### Fix
 
 * Cleanup naming from previous refactoring in ServiceInfo ([#1202](https://github.com/python-zeroconf/python-zeroconf/issues/1202)) ([`b272d75`](https://github.com/python-zeroconf/python-zeroconf/commit/b272d75abd982f3be1f4b20f683cac38011cc6f4))
 
 ## v0.71.3 (2023-07-23)
```

### Comparing `zeroconf-0.71.4/COPYING` & `zeroconf-0.71.5/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/README.rst` & `zeroconf-0.71.5/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/build_ext.py` & `zeroconf-0.71.5/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/docs/Makefile` & `zeroconf-0.71.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/docs/conf.py` & `zeroconf-0.71.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/docs/index.rst` & `zeroconf-0.71.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/pyproject.toml` & `zeroconf-0.71.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.71.4"
+version = "0.71.5"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.71.4/src/zeroconf/__init__.py` & `zeroconf-0.71.5/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.71.4'
+__version__ = '0.71.5'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.71.4/src/zeroconf/_cache.pxd` & `zeroconf-0.71.5/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_cache.py` & `zeroconf-0.71.5/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_core.py` & `zeroconf-0.71.5/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_dns.pxd` & `zeroconf-0.71.5/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_dns.py` & `zeroconf-0.71.5/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_exceptions.py` & `zeroconf-0.71.5/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_handlers.py` & `zeroconf-0.71.5/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_history.py` & `zeroconf-0.71.5/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_logger.py` & `zeroconf-0.71.5/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.71.5/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.71.5/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.71.5/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.71.5/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.71.5/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_services/__init__.py` & `zeroconf-0.71.5/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_services/browser.py` & `zeroconf-0.71.5/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_services/info.py` & `zeroconf-0.71.5/src/zeroconf/_services/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,15 @@
     DNSService,
     DNSText,
 )
 from .._exceptions import BadTypeInNameException
 from .._logger import log
 from .._protocol.outgoing import DNSOutgoing
 from .._updates import RecordUpdate, RecordUpdateListener
-from .._utils.asyncio import (
-    get_running_loop,
-    run_coro_with_timeout,
-    wait_event_or_timeout,
-)
+from .._utils.asyncio import get_running_loop, run_coro_with_timeout
 from .._utils.name import service_type_name
 from .._utils.net import IPVersion, _encode_address
 from .._utils.time import current_time_millis, millis_to_seconds
 from ..const import (
     _ADDRESS_RECORD_TYPES,
     _CLASS_IN,
     _CLASS_UNIQUE,
@@ -127,14 +123,15 @@
         "priority",
         "server",
         "server_key",
         "_properties",
         "host_ttl",
         "other_ttl",
         "interface_index",
+        "_new_records_futures",
     )
 
     def __init__(
         self,
         type_: str,
         name: str,
         port: Optional[int] = None,
@@ -173,15 +170,15 @@
         if isinstance(properties, bytes):
             self._set_text(properties)
         else:
             self._set_properties(properties)
         self.host_ttl = host_ttl
         self.other_ttl = other_ttl
         self.interface_index = interface_index
-        self._notify_event: Optional[asyncio.Event] = None
+        self._new_records_futures: List[asyncio.Future] = []
 
     @property
     def name(self) -> str:
         """The name of the service."""
         return self._name
 
     @name.setter
@@ -231,17 +228,22 @@
         bytes and the values are either bytes, if there was a value, even empty, or `None`, if there
         was none. No further decoding is attempted. The type returned is `Dict[bytes, Optional[bytes]]`.
         """
         return self._properties
 
     async def async_wait(self, timeout: float) -> None:
         """Calling task waits for a given number of milliseconds or until notified."""
-        if self._notify_event is None:
-            self._notify_event = asyncio.Event()
-        await wait_event_or_timeout(self._notify_event, timeout=millis_to_seconds(timeout))
+        loop = asyncio.get_running_loop()
+        future = loop.create_future()
+        self._new_records_futures.append(future)
+        handle = loop.call_later(millis_to_seconds(timeout), future.set_result, None)
+        try:
+            await future
+        finally:
+            handle.cancel()
 
     def addresses_by_version(self, version: IPVersion) -> List[bytes]:
         """List addresses matching IP version.
 
         Addresses are guaranteed to be returned in LIFO (last in, first out)
         order with IPv4 addresses first and IPv6 addresses second.
 
@@ -405,17 +407,19 @@
             self._process_record_threadsafe(zc, record, now)
 
     def async_update_records(self, zc: 'Zeroconf', now: float, records: List[RecordUpdate]) -> None:
         """Updates service information from a DNS record.
 
         This method will be run in the event loop.
         """
-        if self._process_records_threadsafe(zc, now, records) and self._notify_event:
-            self._notify_event.set()
-            self._notify_event.clear()
+        if self._process_records_threadsafe(zc, now, records) and self._new_records_futures:
+            for future in self._new_records_futures:
+                if not future.done():
+                    future.set_result(None)
+            self._new_records_futures.clear()
 
     def _process_records_threadsafe(self, zc: 'Zeroconf', now: float, records: List[RecordUpdate]) -> bool:
         """Thread safe record updating.
 
         Returns True if new records were added.
         """
         updated: bool = False
@@ -587,20 +591,21 @@
 
         This function is for backwards compatibility.
         """
         if self.server is None:
             self.server = self.name
             self.server_key = self.server.lower()
 
-    def load_from_cache(self, zc: 'Zeroconf') -> bool:
+    def load_from_cache(self, zc: 'Zeroconf', now: Optional[float] = None) -> bool:
         """Populate the service info from the cache.
 
         This method is designed to be threadsafe.
         """
-        now = current_time_millis()
+        if not now:
+            now = current_time_millis()
         original_server_key = self.server_key
         cached_srv_record = zc.cache.get_by_details(self.name, _TYPE_SRV, _CLASS_IN)
         if cached_srv_record:
             self._process_record_threadsafe(zc, cached_srv_record, now)
         cached_txt_record = zc.cache.get_by_details(self.name, _TYPE_TXT, _CLASS_IN)
         if cached_txt_record:
             self._process_record_threadsafe(zc, cached_txt_record, now)
@@ -660,34 +665,36 @@
         Passing addr and port is optional, and will default to the
         mDNS multicast address and port. This is useful for directing
         requests to a specific host that may be able to respond across
         subnets.
         """
         if not zc.started:
             await zc.async_wait_for_start()
-        if self.load_from_cache(zc):
+
+        now = current_time_millis()
+
+        if self.load_from_cache(zc, now):
             return True
 
         first_request = True
-        now = current_time_millis()
         delay = _LISTENER_TIME
         next_ = now
         last = now + timeout
         try:
             zc.async_add_listener(self, None)
             while not self._is_complete:
                 if last <= now:
                     return False
                 if next_ <= now:
                     out = self.generate_request_query(
                         zc, now, question_type or DNSQuestionType.QU if first_request else DNSQuestionType.QM
                     )
                     first_request = False
                     if not out.questions:
-                        return self.load_from_cache(zc)
+                        return self.load_from_cache(zc, now)
                     zc.async_send(out, addr, port)
                     next_ = now + delay
                     delay *= 2
                     next_ += random.randint(*_AVOID_SYNC_DELAY_RANDOM_INTERVAL)
 
                 await self.async_wait(min(next_, last) - now)
                 now = current_time_millis()
```

### Comparing `zeroconf-0.71.4/src/zeroconf/_services/registry.py` & `zeroconf-0.71.5/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_services/types.py` & `zeroconf-0.71.5/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_updates.py` & `zeroconf-0.71.5/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_utils/__init__.py` & `zeroconf-0.71.5/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.71.5/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_utils/name.py` & `zeroconf-0.71.5/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_utils/net.py` & `zeroconf-0.71.5/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/_utils/time.py` & `zeroconf-0.71.5/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/asyncio.py` & `zeroconf-0.71.5/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/src/zeroconf/const.py` & `zeroconf-0.71.5/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/__init__.py` & `zeroconf-0.71.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/conftest.py` & `zeroconf-0.71.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/services/__init__.py` & `zeroconf-0.71.5/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/services/test_browser.py` & `zeroconf-0.71.5/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/services/test_info.py` & `zeroconf-0.71.5/tests/services/test_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import Iterable, List, Optional
 from unittest.mock import patch
 
 import pytest
 
 import zeroconf as r
 from zeroconf import DNSAddress, const
+from zeroconf._services import info
 from zeroconf._services.info import ServiceInfo
 from zeroconf._utils.net import IPVersion
 from zeroconf.asyncio import AsyncZeroconf
 
 from .. import _inject_response, has_working_ipv6
 
 log = logging.getLogger('zeroconf')
@@ -1423,7 +1424,79 @@
     aiozc.zeroconf.handle_response(r.DNSIncoming(generated.packets()[0]))
 
     info = ServiceInfo(type_, registration_name)
     await info.async_request(aiozc.zeroconf, timeout=200)
     assert info.addresses_by_version(IPVersion.V4Only) == [b'\x7f\x00\x00\x02']
 
     await aiozc.async_close()
+
+
+@pytest.mark.asyncio
+@patch.object(info, "_LISTENER_TIME", 10000000)
+async def test_release_wait_when_new_recorded_added_concurrency():
+    """Test that concurrent async_request returns as soon as new matching records are added to the cache."""
+    type_ = "_http._tcp.local."
+    registration_name = "multiareccon.%s" % type_
+    desc = {'path': '/~paulsm/'}
+    aiozc = AsyncZeroconf(interfaces=['127.0.0.1'])
+    host = "multahostcon.local."
+    await aiozc.zeroconf.async_wait_for_start()
+
+    # New kwarg way
+    info = ServiceInfo(type_, registration_name, 80, 0, 0, desc, host)
+    tasks = [asyncio.create_task(info.async_request(aiozc.zeroconf, timeout=200000)) for _ in range(10)]
+    await asyncio.sleep(0.1)
+    for task in tasks:
+        assert not task.done()
+    generated = r.DNSOutgoing(const._FLAGS_QR_RESPONSE)
+    generated.add_answer_at_time(
+        r.DNSNsec(
+            registration_name,
+            const._TYPE_NSEC,
+            const._CLASS_IN | const._CLASS_UNIQUE,
+            const._DNS_OTHER_TTL,
+            registration_name,
+            [const._TYPE_AAAA],
+        ),
+        0,
+    )
+    generated.add_answer_at_time(
+        r.DNSService(
+            registration_name,
+            const._TYPE_SRV,
+            const._CLASS_IN | const._CLASS_UNIQUE,
+            10000,
+            0,
+            0,
+            80,
+            host,
+        ),
+        0,
+    )
+    generated.add_answer_at_time(
+        r.DNSAddress(
+            host,
+            const._TYPE_A,
+            const._CLASS_IN,
+            10000,
+            b'\x7f\x00\x00\x01',
+        ),
+        0,
+    )
+    generated.add_answer_at_time(
+        r.DNSText(
+            registration_name,
+            const._TYPE_TXT,
+            const._CLASS_IN | const._CLASS_UNIQUE,
+            10000,
+            b'\x04ff=0\x04ci=2\x04sf=0\x0bsh=6fLM5A==',
+        ),
+        0,
+    )
+    await asyncio.sleep(0)
+    for task in tasks:
+        assert not task.done()
+    aiozc.zeroconf.handle_response(r.DNSIncoming(generated.packets()[0]))
+    _, pending = await asyncio.wait(tasks, timeout=2)
+    assert not pending
+    assert info.addresses == [b'\x7f\x00\x00\x01']
+    await aiozc.async_close()
```

### Comparing `zeroconf-0.71.4/tests/services/test_registry.py` & `zeroconf-0.71.5/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/services/test_types.py` & `zeroconf-0.71.5/tests/services/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         0,
         desc,
         "ash-2.local.",
         addresses=[socket.inet_aton("10.0.1.2")],
     )
     zeroconf_registrar.registry.async_add(info)
     try:
-
         service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
         assert type_ in service_types
         _clear_cache(zeroconf_registrar)
         service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
         assert type_ in service_types
 
     finally:
@@ -77,15 +76,14 @@
         0,
         desc,
         "ash-2.local.",
         addresses=[socket.inet_pton(socket.AF_INET6, addr)],
     )
     zeroconf_registrar.registry.async_add(info)
     try:
-
         service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
         assert type_ in service_types
         _clear_cache(zeroconf_registrar)
         service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
         assert type_ in service_types
 
     finally:
@@ -110,15 +108,14 @@
         0,
         desc,
         "ash-2.local.",
         addresses=[socket.inet_pton(socket.AF_INET6, addr)],
     )
     zeroconf_registrar.registry.async_add(info)
     try:
-
         service_types = ZeroconfServiceTypes.find(ip_version=r.IPVersion.V6Only, timeout=2)
         assert type_ in service_types
         _clear_cache(zeroconf_registrar)
         service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
         assert type_ in service_types
 
     finally:
@@ -143,15 +140,14 @@
         0,
         desc,
         "ash-2.local.",
         addresses=[socket.inet_aton("10.0.1.2")],
     )
     zeroconf_registrar.registry.async_add(info)
     try:
-
         service_types = ZeroconfServiceTypes.find(interfaces=['127.0.0.1'], timeout=2)
         assert discovery_type in service_types
         _clear_cache(zeroconf_registrar)
         service_types = ZeroconfServiceTypes.find(zc=zeroconf_registrar, timeout=2)
         assert discovery_type in service_types
 
     finally:
```

### Comparing `zeroconf-0.71.4/tests/test_asyncio.py` & `zeroconf-0.71.5/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_cache.py` & `zeroconf-0.71.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_core.py` & `zeroconf-0.71.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_dns.py` & `zeroconf-0.71.5/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_exceptions.py` & `zeroconf-0.71.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_handlers.py` & `zeroconf-0.71.5/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_history.py` & `zeroconf-0.71.5/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_init.py` & `zeroconf-0.71.5/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_logger.py` & `zeroconf-0.71.5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_protocol.py` & `zeroconf-0.71.5/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_services.py` & `zeroconf-0.71.5/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/test_updates.py` & `zeroconf-0.71.5/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/utils/__init__.py` & `zeroconf-0.71.5/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/utils/test_asyncio.py` & `zeroconf-0.71.5/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/utils/test_name.py` & `zeroconf-0.71.5/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/tests/utils/test_net.py` & `zeroconf-0.71.5/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.71.4/setup.py` & `zeroconf-0.71.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.71.4',
+    'version': '0.71.5',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.71.4/PKG-INFO` & `zeroconf-0.71.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.71.4
+Version: 0.71.5
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

