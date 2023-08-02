# Comparing `tmp/pycbsdk-0.1.0.tar.gz` & `tmp/pycbsdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycbsdk-0.1.0.tar", last modified: Tue Aug  1 18:50:40 2023, max compression
+gzip compressed data, was "pycbsdk-0.1.2.tar", last modified: Wed Aug  2 16:20:45 2023, max compression
```

## Comparing `pycbsdk-0.1.0.tar` & `pycbsdk-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.462952 pycbsdk-0.1.0/pycbsdk/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.462952 pycbsdk-0.1.0/pycbsdk/cbhw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.462952 pycbsdk-0.1.0/pycbsdk/cbhw/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34165 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/device/nsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.462952 pycbsdk-0.1.0/pycbsdk/cbhw/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/io/datagram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/pycbsdk/cbhw/packet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/v311.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/v40.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/v41.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/v311.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/v40.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/v41.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/packet/v42.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbhw/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/cbsdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/pycbsdk/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pycbsdk/examples/print_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.462952 pycbsdk-0.1.0/pycbsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-01 18:50:40.000000 pycbsdk-0.1.0/pycbsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-01 18:50:40.000000 pycbsdk-0.1.0/pycbsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:50:40.000000 pycbsdk-0.1.0/pycbsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 18:50:40.000000 pycbsdk-0.1.0/pycbsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 18:50:40.000000 pycbsdk-0.1.0/pycbsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 18:50:40.000000 pycbsdk-0.1.0/pycbsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.462952 pycbsdk-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/tests/cbhw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/tests/cbhw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:40.466951 pycbsdk-0.1.0/tests/cbhw/packet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/tests/cbhw/packet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_spike.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-01 18:50:17.000000 pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.448256 pycbsdk-0.1.2/pycbsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.448256 pycbsdk-0.1.2/pycbsdk/cbhw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34965 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/device/nsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/io/datagram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/packet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v40.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v41.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v311.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v40.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v41.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v42.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbsdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/pycbsdk/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/examples/print_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/pycbsdk/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/misc/net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.448256 pycbsdk-0.1.2/pycbsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.444256 pycbsdk-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/tests/cbhw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/tests/cbhw/packet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_spike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_sysinfo.py
```

### Comparing `pycbsdk-0.1.0/LICENSE` & `pycbsdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/PKG-INFO` & `pycbsdk-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: pycbsdk
-Version: 0.1.0
-Summary: Pure Python interface to Blackrock Neurotech Cerebus devices
-Home-page: https://github.com/CerebusOSS/pycbsdk
-Author: Chadwick Boulay
-Author-email: chadwick.boulay@gmail.com
-Project-URL: Bug Tracker, https://github.com/CerebusOSS/pycbsdk/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
+[![PyPI version](https://badge.fury.io/py/pycbsdk.svg)](https://badge.fury.io/py/pycbsdk)
 
 # pycbsdk
 
 Pure Python package for communicating with Blackrock Cerebus devices
 
 ## Quick Start
 
@@ -29,16 +15,16 @@
 Then in python
 
 ```Python
 from pycbsdk import cbsdk
 
 
 params_obj = cbsdk.create_params()
-nsp_obj = cbsdk.get_device(params_obj)
-err = cbsdk.connect(nsp_obj)
+nsp_obj = cbsdk.get_device(params_obj)  # NSPDevice instance. This will be the first argument to most API calls. 
+err = cbsdk.connect(nsp_obj)  # Bind sockets, change device run state, and get device config.
 config = cbsdk.get_config(nsp_obj)
 print(config)
 ```
 
 You may also try the provided test script with `python -m pycbsdk.examples.print_rates` or via the shortcut: `pycbsdk_print_rates`.
 
 ## Introduction
@@ -47,32 +33,39 @@
 
 `pycbsdk`'s API design is intended to mimic that of a C-library. Indeed, a primary goal of this library is to help prototype libraries in other languages. After all, Python is a poor choice to handle high throughput data without some compiled language underneath doing all the heavy lifting.
 
 However, it's pretty useful as is! And so far it has been good-enough for some quick test scripts, and it even drops fewer packets than CereLink. So, please use it, and contribute! We are more than happy to see the API expand to support more features, or even to have an additional "pythonic" API.
 
 ## Design
 
+Upon initialization, the `NSPDevice` instance configures its sockets (but no connection yet), it allocates memory for its mirror of the device state, and it registers callbacks to monitor config state.
+
 When the connection to the device is established, two threads are created and started:
 * `CerebusDatagramThread`
   * Retrieves datagrams using `asyncio`
   * Slices into generic packets
   * Casts packets into their native type
   * Enqueues packets for the PacketHandlerThread
 * `PacketHandlerThread`
   * Updates device state (e.g., mirrors device time)
   * Calls registered callbacks depending on the packet type.
 
-The device also registers some of its own internal callbacks to monitor config state.
+`connect()` has `startup_sequence=True` by default. This will cause the SDK to attempt to put the device into a running state. Otherwise, it'll stay in its original run state.
 
-The client can use API functions to:
-* Get / Set config -- these might simply grab the internal state or they might warrant a roundtrip communication to the device.
-  * The latter may hold back the return value until the reply packet has been received and can therefore be slow. Try to call `get_config` with `force_refresh=True` sparingly.
+After the connection is established, the client can use API functions to:
+* Get / Set config
+  * `set_config` and `set_channel_config` do not do anything yet
+  * `set_channel_spk_config` and `set_channel_config_by_packet` do things and are blocking.
+  * `get_config` is non-blocking by default and will simply read the local mirror of the config. However, if `force_refresh=True` is passed as a kwarg, then this function will block and wait for a reply from the device. Use this sparingly.
 * Register a callback to receive data as soon as it appears on the handler thread.
   
 This and more should appear in the documentation at some point in the future...
 
 ## Limitations
 
 * This library takes exclusive control over the UDP socket on port 51002 and thus cannot be used with Central, nor any other instance of `pycbsdk`. You only get one instance of `pycbsdk` _or_ Central per machine.
+  * [CereLink](https://github.com/CerebusOSS/CereLink)'s cerebus.cbpy uses shared memory and therefore can work in parallel to Central or other cbpy instances.
 * The API is still very sparse and limited in functionality.
 * For now, Python still has the GIL. This means that despite using threading, if your callback functions are slow and hold up the PacketHandlerThread, this could hold up datagram retrieval and ultimately cause packets to be dropped.
-  * A possible solution is for your callbacks to simply enqueue the data for a longer-running process to handle.
+  * Callbacks may enqueue the data for a longer-running `multiprocessing` process to handle.
+  * Switch to [No GIL Python](https://peps.python.org/pep-0703/) as soon as it is available.
+  * Use pycbsdk to prototype an application in a language that uses real parallelism.
```

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/device/base.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/device/base.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/device/nsp.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/device/nsp.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     CBChannelType,
     CBPacketType,
     CBNPlayMode,
     CBNPlayFlag,
     CBSpecialChan,
 )
 from pycbsdk.cbhw.params import Params
+from pycbsdk.cbhw.consts import CBError
 
 
 __all__ = ["SpikeEvent", "NSPDevice", "CBRunLevel"]
 
 
 # globals
 logger = logging.getLogger(__name__)
@@ -623,15 +624,15 @@
         pkt.flags = flag
         pkt.val = val
         pkt.speed = speed
         # if 'nplay' in self._config and self._config['nplay'] is not None:
         #     pkt.fname = self._config['nplay'].fname
         self._send_packet(pkt)
 
-    def set_runlevel(self, run_level: CBRunLevel, timeout: Optional[float] = None):
+    def set_runlevel(self, run_level: CBRunLevel, timeout: Optional[float] = None) -> CBError:
         """
         cbPKT_SYSINFO sysinfo;
         sysinfo.type     = cbPKTTYPE_SYSSETRUNLEV;
         sysinfo.runlevel = runlevel;
         sysinfo.resetque = resetque;
         sysinfo.runflags = runflags;
         """
@@ -643,20 +644,24 @@
         if run_level == CBRunLevel.HARDRESET:
             event = self._config_events["runlevel_standby"]
         elif run_level == CBRunLevel.RESET:
             event = self._config_events["runlevel_running"]
         else:
             event = self._config_events["sysrep"]
         logger.debug(f"Attempting to set runlevel to {run_level}")
-        if not self._send_packet(pkt, event=event, timeout=timeout):
-            logger.warning(f"Did not receive SYSREPRUNLEV in expected timeout.")
+        succ = self._send_packet(pkt, event=event, timeout=timeout)
+        if not succ:
+            logger.warning("Did not receive SYSREPRUNLEV in expected timeout.")
+            return CBError.NOREPLY
+        else:
+            return CBError.NONE
 
     def get_runlevel(self, force_refresh=False) -> CBRunLevel:
         if force_refresh:
-            self.set_runlevel(CBRunLevel.RUNNING, timeout=0.5)
+            err = self.set_runlevel(CBRunLevel.RUNNING, timeout=0.5)
         return self._config["runlevel"]
 
     def set_transport(
         self, transport: str, value: bool, timeout: Optional[float] = None
     ):
         pkt = self.packet_factory.make_packet(
             None,
@@ -705,57 +710,74 @@
         )
 
         self._pkt_handler_thread.start()
         self._io_thread.start()
         # _io_thread.start() returns immediately but takes a few moments until its send_q is created.
         time.sleep(0.5)
 
+        err = CBError.NONE
+        runlevel = 0
+
         # Startup sequence runs in a short-lived async chain.
         #  It relies on both the sender and receiver working.
         if startup_sequence:
-            self._startup_sequence()
+            err = self._startup_sequence()
 
-        return self.get_runlevel(force_refresh=not startup_sequence)
+        if not err:
+            runlevel = self.get_runlevel(force_refresh=not startup_sequence)
+            if not runlevel:
+                err = CBError.UNDEFINED
+
+        if err:
+            if err == CBError.NOREPLY:
+                logger.error("Device did not reply to startup sequence. This could be caused by a network problem "
+                             "or by a protocol mismatch.")
+            else:
+                logger.error(f"Error received during startup sequence: {err}")
+            self.disconnect()
+
+        return runlevel
 
     def disconnect(self):
         # TODO: Terminate IO
         self._io_thread.stop()
         self._pkt_handler_thread.stop()
 
         self._io_thread.join()
         self._pkt_handler_thread.join()
 
         del self._receiver_queue
         self._receiver_queue = None
 
         logger.info("Disconnected successfully.")
 
-    def _startup_sequence(self):
-        self.set_runlevel(CBRunLevel.RUNNING, timeout=0.45)
+    def _startup_sequence(self) -> CBError:
+        err = self.set_runlevel(CBRunLevel.RUNNING, timeout=0.45)
+        if err != CBError.NONE:
+            return err
 
         if self._config["runlevel"] != CBRunLevel.RUNNING:
             # After a cold boot, the system is probably in runlevel 10 (startup)
             # Central does not attempt to reset until 500 msec after the initial runlevel check.
             # We will receive 2 runlevel packets. 20 to acknowledge the hard reset, the 30 when it's in standby.
-            self.set_runlevel(
+            err = self.set_runlevel(
                 CBRunLevel.HARDRESET, timeout=0.45
             )  # Doesn't return until standby is received.
 
         # Central waits another 0.5 seconds before requesting the config, even if already running.
         # We don't do that here.
 
         logger.debug("Attempting to get_config")
         _cfg = self.get_config(timeout=2.0)
 
         if self._config["runlevel"] != CBRunLevel.RUNNING:
             # Central waits a full second between the reqconfigall and reset
             # We will receive 2 runlevel packets. 40 to acknowledge the reset, and 50 when it's running.
-            self.set_runlevel(
-                CBRunLevel.RESET
-            )  # Doesn't return until RUNNING is received.
+            err = self.set_runlevel(CBRunLevel.RESET)
+            # Note: no timeout! Will block until RUNNING is received.
 
             # time.sleep(0.1)  # Give it enough time to finish starting up.
 
         if self._config["nplay"] is not None:
             # 1. (skip) mode=CBNPlayMode.PATH, fname=folder_path.
             # 2. mode=CBNPlayMode.NONE, speed=1, fname=filename. These are the default settings.
             self.set_nplay_state()
@@ -764,14 +786,16 @@
             self.set_nplay_state(val=0, mode=CBNPlayMode.PAUSE)
             time.sleep(0.1)
             # 4. mode=CBNPlayMode.SINGLE, val=0, speed=0??
             self.set_nplay_state(val=0, mode=CBNPlayMode.SINGLE, speed=0)
             time.sleep(0.1)
             # set unpause
 
+        return CBError.NONE
+
     def _send_packet(
         self, pkt, event: Optional[threading.Event] = None, timeout=0.005
     ) -> bool:
         """
         Touch-up packet and enqueue for sender thread.
         Called by configure and _startup_sequence.
         """
```

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/handler.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/handler.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/io/datagram.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/io/datagram.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/abstract.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/abstract.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/common.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/common.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/factory.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/factory.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/v40.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v40.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/header/v41.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v41.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/packets.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/packets.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/v311.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v311.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/v40.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v40.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/v41.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v41.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/packet/v42.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v42.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/pycbsdk/cbhw/params.py` & `pycbsdk-0.1.2/pycbsdk/cbhw/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,19 @@
         self._inst_addr = ""
         self._inst_port = 51001
         self._client_addr = ""
         self._client_port = 51002
         self._recv_bufsize = (8 if sys.platform == "win32" else 6) * 1024 * 1024
         self._protocol = "4.1"
 
+    def __str__(self):
+        return f"From Adapter {self._client_addr}:{self._client_port}\n" \
+               f"To Device {self._inst_addr}:{self._inst_port}\n" \
+               f"Using Protocol {self._protocol} and socket buffer size {self._recv_bufsize}"
+
     @property
     def inst_addr(self) -> str:
         return self._inst_addr
 
     @inst_addr.setter
     def inst_addr(self, value: str):
         self._inst_addr = value
```

### Comparing `pycbsdk-0.1.0/pycbsdk/examples/print_rates.py` & `pycbsdk-0.1.2/pycbsdk/examples/print_rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,18 @@
     - run the async chain
     - on the main thread, render the internal state (print the min-max mean+/-std of the rates every 0.5 seconds).
     :param skip_startup:
     :return:
     """
     params_obj = cbsdk.create_params(**params_kwargs)
     nsp_obj = cbsdk.get_device(params_obj)
-    _ = cbsdk.connect(nsp_obj, startup_sequence=not skip_startup)
+    run_level = cbsdk.connect(nsp_obj, startup_sequence=not skip_startup)
+    if not run_level:
+        logger.error(f"Could not connect to device. Check params and try again: \n{params_obj}.")
+        return
     config = cbsdk.get_config(nsp_obj)
 
     # Check which channels have spiking enabled and what kind of thresholding they are using.
     #  TODO: We should have API functions to check channel capabilities instead of
     #   importing from pycbsdk.cbhw and doing bitwise testing here
     from pycbsdk.cbhw.device.nsp import CBAInpSpk
     from pycbsdk.cbhw.packet.common import CBChannelType
@@ -153,37 +156,39 @@
     # --inst_addr=192.168.137.255 --client_addr=192.168.137.199
     parser = argparse.ArgumentParser(description="Consume data from (emulated) NSP.")
     parser.add_argument(
         "--inst_addr",
         "-i",
         type=str,
         default="",
-        help="ipv4 address to send control packets. Can use subnet. "
-        "Will broadcast if not on Cerebus Subnet."
-        "Use 127.0.0.1 if using with nPlayServer in non-bcast.",
+        help="ipv4 address of device. pycbsdk will send control packets to this address. Subnet OK. "
+        "Use 127.0.0.1 for use with nPlayServer (non-bcast). "
+        "The default is 0.0.0.0 (IPADDR_ANY) on Mac and Linux. On Windows, known IPs will be searched."
+        ,
     )
-    parser.add_argument("--inst_port", type=int, default=51001)
+    parser.add_argument("--inst_port", type=int, default=51002, help="Network port to send control packets."
+                                                                     "Use 51002 for Gemini and 51001 for Legacy NSP.")
     parser.add_argument(
         "--client_addr",
         "-c",
         type=str,
         default="",
-        help="ipv4 address of the adapter we will receive packets on. "
+        help="ipv4 address of this machine's network adapter we will receive packets on. "
         "Defaults to INADDR_ANY. If address is provided, assumes Cerebus Subnet.",
     )
-    parser.add_argument("--client_port", "-p", type=int, default=51002)
+    parser.add_argument("--client_port", "-p", type=int, default=51002, help="Network port to receive packets. This should always be 51002.")
     parser.add_argument(
         "--recv_bufsize",
         "-b",
         type=int,
         help=f"UDP socket recv buffer size. "
         f"Default: {(8 if sys.platform == 'win32' else 6) * 1024 * 1024}.",
     )
-    parser.add_argument("--protocol", type=str, default="4.1")
-    parser.add_argument("--skip_startup", action="store_true")
+    parser.add_argument("--protocol", type=str, default="4.1", help="Protocol Version. 3.11, 4.0, or 4.1 supported.")
+    parser.add_argument("--skip_startup", action="store_true", help="Skip the initial handshake as well as the attempt to set the device to RUNNING.")
     parser.add_argument(
         "--debug",
         "-d",
         help="Print lots of debugging statements",
         action="store_const",
         dest="loglevel",
         const=logging.DEBUG,
```

### Comparing `pycbsdk-0.1.0/pycbsdk.egg-info/PKG-INFO` & `pycbsdk-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pycbsdk
-Version: 0.1.0
+Version: 0.1.2
 Summary: Pure Python interface to Blackrock Neurotech Cerebus devices
 Home-page: https://github.com/CerebusOSS/pycbsdk
 Author: Chadwick Boulay
 Author-email: chadwick.boulay@gmail.com
 Project-URL: Bug Tracker, https://github.com/CerebusOSS/pycbsdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/pycbsdk.svg)](https://badge.fury.io/py/pycbsdk)
+
 # pycbsdk
 
 Pure Python package for communicating with Blackrock Cerebus devices
 
 ## Quick Start
 
 From a shell...
@@ -29,16 +31,16 @@
 Then in python
 
 ```Python
 from pycbsdk import cbsdk
 
 
 params_obj = cbsdk.create_params()
-nsp_obj = cbsdk.get_device(params_obj)
-err = cbsdk.connect(nsp_obj)
+nsp_obj = cbsdk.get_device(params_obj)  # NSPDevice instance. This will be the first argument to most API calls. 
+err = cbsdk.connect(nsp_obj)  # Bind sockets, change device run state, and get device config.
 config = cbsdk.get_config(nsp_obj)
 print(config)
 ```
 
 You may also try the provided test script with `python -m pycbsdk.examples.print_rates` or via the shortcut: `pycbsdk_print_rates`.
 
 ## Introduction
@@ -47,32 +49,39 @@
 
 `pycbsdk`'s API design is intended to mimic that of a C-library. Indeed, a primary goal of this library is to help prototype libraries in other languages. After all, Python is a poor choice to handle high throughput data without some compiled language underneath doing all the heavy lifting.
 
 However, it's pretty useful as is! And so far it has been good-enough for some quick test scripts, and it even drops fewer packets than CereLink. So, please use it, and contribute! We are more than happy to see the API expand to support more features, or even to have an additional "pythonic" API.
 
 ## Design
 
+Upon initialization, the `NSPDevice` instance configures its sockets (but no connection yet), it allocates memory for its mirror of the device state, and it registers callbacks to monitor config state.
+
 When the connection to the device is established, two threads are created and started:
 * `CerebusDatagramThread`
   * Retrieves datagrams using `asyncio`
   * Slices into generic packets
   * Casts packets into their native type
   * Enqueues packets for the PacketHandlerThread
 * `PacketHandlerThread`
   * Updates device state (e.g., mirrors device time)
   * Calls registered callbacks depending on the packet type.
 
-The device also registers some of its own internal callbacks to monitor config state.
+`connect()` has `startup_sequence=True` by default. This will cause the SDK to attempt to put the device into a running state. Otherwise, it'll stay in its original run state.
 
-The client can use API functions to:
-* Get / Set config -- these might simply grab the internal state or they might warrant a roundtrip communication to the device.
-  * The latter may hold back the return value until the reply packet has been received and can therefore be slow. Try to call `get_config` with `force_refresh=True` sparingly.
+After the connection is established, the client can use API functions to:
+* Get / Set config
+  * `set_config` and `set_channel_config` do not do anything yet
+  * `set_channel_spk_config` and `set_channel_config_by_packet` do things and are blocking.
+  * `get_config` is non-blocking by default and will simply read the local mirror of the config. However, if `force_refresh=True` is passed as a kwarg, then this function will block and wait for a reply from the device. Use this sparingly.
 * Register a callback to receive data as soon as it appears on the handler thread.
   
 This and more should appear in the documentation at some point in the future...
 
 ## Limitations
 
 * This library takes exclusive control over the UDP socket on port 51002 and thus cannot be used with Central, nor any other instance of `pycbsdk`. You only get one instance of `pycbsdk` _or_ Central per machine.
+  * [CereLink](https://github.com/CerebusOSS/CereLink)'s cerebus.cbpy uses shared memory and therefore can work in parallel to Central or other cbpy instances.
 * The API is still very sparse and limited in functionality.
 * For now, Python still has the GIL. This means that despite using threading, if your callback functions are slow and hold up the PacketHandlerThread, this could hold up datagram retrieval and ultimately cause packets to be dropped.
-  * A possible solution is for your callbacks to simply enqueue the data for a longer-running process to handle.
+  * Callbacks may enqueue the data for a longer-running `multiprocessing` process to handle.
+  * Switch to [No GIL Python](https://peps.python.org/pep-0703/) as soon as it is available.
+  * Use pycbsdk to prototype an application in a language that uses real parallelism.
```

### Comparing `pycbsdk-0.1.0/pycbsdk.egg-info/SOURCES.txt` & `pycbsdk-0.1.2/pycbsdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pycbsdk.egg-info/SOURCES.txt
 pycbsdk.egg-info/dependency_links.txt
 pycbsdk.egg-info/entry_points.txt
 pycbsdk.egg-info/requires.txt
 pycbsdk.egg-info/top_level.txt
 pycbsdk/cbhw/__init__.py
 pycbsdk/cbhw/config.py
+pycbsdk/cbhw/consts.py
 pycbsdk/cbhw/handler.py
 pycbsdk/cbhw/params.py
 pycbsdk/cbhw/device/__init__.py
 pycbsdk/cbhw/device/base.py
 pycbsdk/cbhw/device/nsp.py
 pycbsdk/cbhw/io/__init__.py
 pycbsdk/cbhw/io/base.py
@@ -32,13 +33,15 @@
 pycbsdk/cbhw/packet/v42.py
 pycbsdk/cbhw/packet/header/__init__.py
 pycbsdk/cbhw/packet/header/v311.py
 pycbsdk/cbhw/packet/header/v40.py
 pycbsdk/cbhw/packet/header/v41.py
 pycbsdk/examples/__init__.py
 pycbsdk/examples/print_rates.py
+pycbsdk/misc/__init__.py
+pycbsdk/misc/net.py
 tests/cbhw/__init__.py
 tests/cbhw/packet/__init__.py
 tests/cbhw/packet/test_pkt_generic.py
 tests/cbhw/packet/test_pkt_header.py
 tests/cbhw/packet/test_pkt_spike.py
 tests/cbhw/packet/test_pkt_sysinfo.py
```

### Comparing `pycbsdk-0.1.0/setup.cfg` & `pycbsdk-0.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 [options]
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy
 	aenum
+	ifaddr
 
 [options.extras_require]
 tests = pytest
 
 [options.packages.find]
 exclude = tests
```

### Comparing `pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_generic.py` & `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_generic.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_header.py` & `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_header.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_spike.py` & `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_spike.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.0/tests/cbhw/packet/test_pkt_sysinfo.py` & `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_sysinfo.py`

 * *Files identical despite different names*

