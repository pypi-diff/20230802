# Comparing `tmp/pycbsdk-0.1.2.tar.gz` & `tmp/pycbsdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycbsdk-0.1.2.tar", last modified: Wed Aug  2 16:20:45 2023, max compression
+gzip compressed data, was "pycbsdk-0.1.3.tar", last modified: Wed Aug  2 18:06:32 2023, max compression
```

## Comparing `pycbsdk-0.1.2.tar` & `pycbsdk-0.1.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.448256 pycbsdk-0.1.2/pycbsdk/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.448256 pycbsdk-0.1.2/pycbsdk/cbhw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34965 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/device/nsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/io/datagram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/packet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.452256 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v311.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v40.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v41.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v311.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v40.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v41.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/packet/v42.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbhw/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/cbsdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/pycbsdk/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/examples/print_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/pycbsdk/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pycbsdk/misc/net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.448256 pycbsdk-0.1.2/pycbsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 16:20:45.000000 pycbsdk-0.1.2/pycbsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.444256 pycbsdk-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/tests/cbhw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:45.456256 pycbsdk-0.1.2/tests/cbhw/packet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_spike.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-02 16:20:22.000000 pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.980615 pycbsdk-0.1.3/pycbsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.980615 pycbsdk-0.1.3/pycbsdk/cbhw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.980615 pycbsdk-0.1.3/pycbsdk/cbhw/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35008 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/device/nsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.980615 pycbsdk-0.1.3/pycbsdk/cbhw/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/io/datagram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/pycbsdk/cbhw/packet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/v311.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/v40.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/v41.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/v311.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/v40.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/v41.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/packet/v42.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbhw/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/cbsdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/pycbsdk/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/examples/print_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/pycbsdk/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pycbsdk/misc/net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.980615 pycbsdk-0.1.3/pycbsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-02 18:06:32.000000 pycbsdk-0.1.3/pycbsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-02 18:06:32.000000 pycbsdk-0.1.3/pycbsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:06:32.000000 pycbsdk-0.1.3/pycbsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 18:06:32.000000 pycbsdk-0.1.3/pycbsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 18:06:32.000000 pycbsdk-0.1.3/pycbsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 18:06:32.000000 pycbsdk-0.1.3/pycbsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-02 18:06:32.988615 pycbsdk-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.980615 pycbsdk-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/tests/cbhw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/tests/cbhw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:32.984615 pycbsdk-0.1.3/tests/cbhw/packet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/tests/cbhw/packet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_spike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-02 18:06:10.000000 pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_sysinfo.py
```

### Comparing `pycbsdk-0.1.2/LICENSE` & `pycbsdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/PKG-INFO` & `pycbsdk-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycbsdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pure Python interface to Blackrock Neurotech Cerebus devices
 Home-page: https://github.com/CerebusOSS/pycbsdk
 Author: Chadwick Boulay
 Author-email: chadwick.boulay@gmail.com
 Project-URL: Bug Tracker, https://github.com/CerebusOSS/pycbsdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pycbsdk-0.1.2/README.md` & `pycbsdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/device/base.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/device/base.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/device/nsp.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/device/nsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,15 +624,17 @@
         pkt.flags = flag
         pkt.val = val
         pkt.speed = speed
         # if 'nplay' in self._config and self._config['nplay'] is not None:
         #     pkt.fname = self._config['nplay'].fname
         self._send_packet(pkt)
 
-    def set_runlevel(self, run_level: CBRunLevel, timeout: Optional[float] = None) -> CBError:
+    def set_runlevel(
+        self, run_level: CBRunLevel, timeout: Optional[float] = None
+    ) -> CBError:
         """
         cbPKT_SYSINFO sysinfo;
         sysinfo.type     = cbPKTTYPE_SYSSETRUNLEV;
         sysinfo.runlevel = runlevel;
         sysinfo.resetque = resetque;
         sysinfo.runflags = runflags;
         """
@@ -725,16 +727,18 @@
         if not err:
             runlevel = self.get_runlevel(force_refresh=not startup_sequence)
             if not runlevel:
                 err = CBError.UNDEFINED
 
         if err:
             if err == CBError.NOREPLY:
-                logger.error("Device did not reply to startup sequence. This could be caused by a network problem "
-                             "or by a protocol mismatch.")
+                logger.error(
+                    "Device did not reply to startup sequence. This could be caused by a network problem "
+                    "or by a protocol mismatch."
+                )
             else:
                 logger.error(f"Error received during startup sequence: {err}")
             self.disconnect()
 
         return runlevel
 
     def disconnect(self):
```

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/handler.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/handler.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/io/datagram.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/io/datagram.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/abstract.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/abstract.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/common.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/common.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/factory.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/factory.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v40.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/v40.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/header/v41.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/header/v41.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/packets.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/packets.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v311.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/v311.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v40.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/v40.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v41.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/v41.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/cbhw/packet/v42.py` & `pycbsdk-0.1.3/pycbsdk/cbhw/packet/v42.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/pycbsdk/examples/print_rates.py` & `pycbsdk-0.1.3/pycbsdk/examples/print_rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,17 @@
     :param skip_startup:
     :return:
     """
     params_obj = cbsdk.create_params(**params_kwargs)
     nsp_obj = cbsdk.get_device(params_obj)
     run_level = cbsdk.connect(nsp_obj, startup_sequence=not skip_startup)
     if not run_level:
-        logger.error(f"Could not connect to device. Check params and try again: \n{params_obj}.")
+        logger.error(
+            f"Could not connect to device. Check params and try again: \n{params_obj}."
+        )
         return
     config = cbsdk.get_config(nsp_obj)
 
     # Check which channels have spiking enabled and what kind of thresholding they are using.
     #  TODO: We should have API functions to check channel capabilities instead of
     #   importing from pycbsdk.cbhw and doing bitwise testing here
     from pycbsdk.cbhw.device.nsp import CBAInpSpk
@@ -158,37 +160,56 @@
     parser.add_argument(
         "--inst_addr",
         "-i",
         type=str,
         default="",
         help="ipv4 address of device. pycbsdk will send control packets to this address. Subnet OK. "
         "Use 127.0.0.1 for use with nPlayServer (non-bcast). "
-        "The default is 0.0.0.0 (IPADDR_ANY) on Mac and Linux. On Windows, known IPs will be searched."
-        ,
+        "The default is 0.0.0.0 (IPADDR_ANY) on Mac and Linux. On Windows, known IPs will be searched.",
+    )
+    parser.add_argument(
+        "--inst_port",
+        type=int,
+        default=51002,
+        help="Network port to send control packets."
+        "Use 51002 for Gemini and 51001 for Legacy NSP.",
     )
-    parser.add_argument("--inst_port", type=int, default=51002, help="Network port to send control packets."
-                                                                     "Use 51002 for Gemini and 51001 for Legacy NSP.")
     parser.add_argument(
         "--client_addr",
         "-c",
         type=str,
         default="",
         help="ipv4 address of this machine's network adapter we will receive packets on. "
         "Defaults to INADDR_ANY. If address is provided, assumes Cerebus Subnet.",
     )
-    parser.add_argument("--client_port", "-p", type=int, default=51002, help="Network port to receive packets. This should always be 51002.")
+    parser.add_argument(
+        "--client_port",
+        "-p",
+        type=int,
+        default=51002,
+        help="Network port to receive packets. This should always be 51002.",
+    )
     parser.add_argument(
         "--recv_bufsize",
         "-b",
         type=int,
         help=f"UDP socket recv buffer size. "
         f"Default: {(8 if sys.platform == 'win32' else 6) * 1024 * 1024}.",
     )
-    parser.add_argument("--protocol", type=str, default="4.1", help="Protocol Version. 3.11, 4.0, or 4.1 supported.")
-    parser.add_argument("--skip_startup", action="store_true", help="Skip the initial handshake as well as the attempt to set the device to RUNNING.")
+    parser.add_argument(
+        "--protocol",
+        type=str,
+        default="4.1",
+        help="Protocol Version. 3.11, 4.0, or 4.1 supported.",
+    )
+    parser.add_argument(
+        "--skip_startup",
+        action="store_true",
+        help="Skip the initial handshake as well as the attempt to set the device to RUNNING.",
+    )
     parser.add_argument(
         "--debug",
         "-d",
         help="Print lots of debugging statements",
         action="store_const",
         dest="loglevel",
         const=logging.DEBUG,
```

### Comparing `pycbsdk-0.1.2/pycbsdk.egg-info/PKG-INFO` & `pycbsdk-0.1.3/pycbsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycbsdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pure Python interface to Blackrock Neurotech Cerebus devices
 Home-page: https://github.com/CerebusOSS/pycbsdk
 Author: Chadwick Boulay
 Author-email: chadwick.boulay@gmail.com
 Project-URL: Bug Tracker, https://github.com/CerebusOSS/pycbsdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pycbsdk-0.1.2/pycbsdk.egg-info/SOURCES.txt` & `pycbsdk-0.1.3/pycbsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/setup.cfg` & `pycbsdk-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_generic.py` & `pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_generic.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_header.py` & `pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_header.py`

 * *Files identical despite different names*

### Comparing `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_spike.py` & `pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_spike.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     assert pkt.nPeak == 1
     assert pkt.nValley == 2
     assert len(pkt.fPattern) == 3
     assert type(pkt.fPattern[0]) == float
 
 
 def test_pkt_spike_init_data_withwave():
-
     fPattern = struct.pack("<3f", 1.0, 2.0, 3.0)
     nPeak = struct.pack("<H", 1)
     nValley = struct.pack("<H", 2)
     NPTS = 10  # TODO: Test odd number. Last entry probably gets cut off!? Need ceil instead of //.
     wave = struct.pack(f"<{NPTS}h", *range(NPTS))
     _header = packets.CBPacketSpike().header
     _header.dlen += (
```

### Comparing `pycbsdk-0.1.2/tests/cbhw/packet/test_pkt_sysinfo.py` & `pycbsdk-0.1.3/tests/cbhw/packet/test_pkt_sysinfo.py`

 * *Files identical despite different names*

