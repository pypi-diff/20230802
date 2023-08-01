# Comparing `tmp/alertmanagermeshtastic-2023.8.1.13.tar.gz` & `tmp/alertmanagermeshtastic-2023.8.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertmanagermeshtastic-2023.8.1.13.tar", last modified: Tue Aug  1 20:36:08 2023, max compression
+gzip compressed data, was "alertmanagermeshtastic-2023.8.1.14.tar", last modified: Tue Aug  1 23:21:09 2023, max compression
```

## Comparing `alertmanagermeshtastic-2023.8.1.13.tar` & `alertmanagermeshtastic-2023.8.1.14.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.755519 alertmanagermeshtastic-2023.8.1.13/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 20:36:08.755519 alertmanagermeshtastic-2023.8.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/config_example.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/config_example_docker.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-01 20:36:08.759520 alertmanagermeshtastic-2023.8.1.13/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.751520 alertmanagermeshtastic-2023.8.1.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.755519 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/meshtastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/tokencli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.755519 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:36:08.000000 alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:36:08.755519 alertmanagermeshtastic-2023.8.1.13/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_create_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_dummy_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_meshtastic_announcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_meshtastic_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 20:35:58.000000 alertmanagermeshtastic-2023.8.1.13/tests/test_token_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/config_example.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/config_example_docker.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.993284 alertmanagermeshtastic-2023.8.1.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/meshtastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/tokencli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 23:21:08.000000 alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:21:08.997284 alertmanagermeshtastic-2023.8.1.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_create_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_dummy_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_announcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 23:21:01.000000 alertmanagermeshtastic-2023.8.1.14/tests/test_token_cli.py
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/Dockerfile` & `alertmanagermeshtastic-2023.8.1.14/Dockerfile`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/LICENSE` & `alertmanagermeshtastic-2023.8.1.14/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Copyright (c) 2007-2022 Jochen Kupperschmidt
+Copyright (c) 2023 Alexander Volz
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.14/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.13
+Version: 2023.8.1.14
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
@@ -39,15 +39,15 @@
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanagermeshtastic)
 [![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
 This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
 
 > **Warning**
-> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. Also the way that the ack is checked is not optimal, so messages tend to take longer to get to the device, but are delivered for sure(maybe multiple times). If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/README.md` & `alertmanagermeshtastic-2023.8.1.14/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanagermeshtastic)
 [![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
 This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
 
 > **Warning**
-> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. Also the way that the ack is checked is not optimal, so messages tend to take longer to get to the device, but are delivered for sure(maybe multiple times). If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/setup.cfg` & `alertmanagermeshtastic-2023.8.1.14/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/cli.py` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 alertmanagermeshtastic.cli
 ~~~~~~~~~~~~~~~
 
 Command line entry point
 
-:Copyright: 2007-2022 Jochen Kupperschmidt, Alexander Volz
+:Copyright: 2007-2022 Jochen Kupperschmidt
+:Copyright: 2023 Alexander Volz
 :License: MIT, see LICENSE for details.
 """
 
 from __future__ import annotations
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 import sys
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/config.py` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 alertmanagermeshtastic.config
 ~~~~~~~~~~~~~~~~~~
 
 Configuration loading
 
-:Copyright: 2007-2022 Jochen Kupperschmidt, Alexander Volz
+:Copyright: 2007-2022 Jochen Kupperschmidt
+:Copyright: 2023 Alexander Volz
 :License: MIT, see LICENSE for details.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/http.py` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 alertmanagermeshtastic.http
 ~~~~~~~~~~~~~~~~
 
 HTTP server to receive messages
 
-:Copyright: 2007-2022 Jochen Kupperschmidt, Alexander Volz
+:Copyright: 2007-2022 Jochen Kupperschmidt
+:Copyright: 2023 Alexander Volz
 :License: MIT, see LICENSE for details.
 """
 
 from __future__ import annotations
 from http import HTTPStatus
 import logging
 import sys
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/meshtastic.py` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/meshtastic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 alertmanagermeshtastic.meshtastic
 ~~~~~~~~~~~~~~~
 
 Meshtastic connection
 
-:Copyright: 2007-2022 Jochen Kupperschmidt, Alexander Volz
+:Copyright: 2007-2022 Jochen Kupperschmidt
+:Copyright: 2023 Alexander Volz
 :License: MIT, see LICENSE for details.
 """
 
 from __future__ import annotations
 import logging
 import meshtastic, meshtastic.serial_interface
 
 from dateutil import parser
 from .config import MeshtasticConfig, MeshtasticConnection
 import time
 
+from pubsub import pub
 
 logger = logging.getLogger(__name__)
 
 
 class Announcer:
     """An announcer."""
 
@@ -41,24 +43,43 @@
         self,
         connection: MeshtasticConnection,
     ) -> None:
         self.connection = connection
 
         self.meshtasticinterface = _create_meshtasticinterface(connection)
 
+    def _onconnect(topic=pub.AUTO_TOPIC, interface=None):
+        logger.debug("\t Connected to meshtastic")
+
+    def _onconnectionlost(topic=pub.AUTO_TOPIC, interface=None):
+        del topic.meshtasticinterface
+        while True:
+            try:
+                topic.meshtasticinterface = _create_meshtasticinterface(
+                    topic.connection
+                )
+                break
+            except Exception as e:
+                logger.error(
+                    "\t Connnection to meshtastic failed with error: %s , retry in 2 seconds",
+                    e,
+                )
+                time.sleep(2)
+
     def start(self) -> None:
         """Connect to the connection, in a separate thread."""
         logger.info(
             '\t Connecting to MESHTASTIC connection %s, the node is %d and messages will be sent %d times with timeout %d before failing',
             self.connection.tty,
             self.connection.nodeid,
             self.connection.maxsendingattempts,
             self.connection.timeout,
         )
-
+        pub.subscribe(self._onconnectionlost, "meshtastic.connection.lost")
+        pub.subscribe(self._onconnect, "meshtastic.connection.established")
         # start_thread(self.meshtasticinterface.start)
 
     def announce(self, alert: str) -> None:
         """Announce a message."""
         try:
             try:
                 message = self.formatalert(alert)
@@ -97,14 +118,17 @@
                         "\t [%s][%d][%d] sending attempt %d ",
                         alert["fingerprint"],
                         alert["qn"],
                         index,
                         attempt,
                     )
                     try:
+                        while not hasattr(self, 'meshtasticinterface'):
+                            time.sleep(2)
+
                         self.meshtasticinterface.sendText(
                             str(alert["qn"])
                             + ":"
                             + str(index + 1)
                             + "/"
                             + str(total_chunks)
                             + "\n"
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/processor.py` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 alertmanagermeshtastic.processor
 ~~~~~~~~~~~~~~~~~~~~~
 
 Connect HTTP server and MESHTASTIC interface.
 
-:Copyright: 2007-2022 Jochen Kupperschmidt, Alexander Volz
+:Copyright: 2007-2022 Jochen Kupperschmidt
+:Copyright: 2023 Alexander Volz
 :License: MIT, see LICENSE for details.
 """
 
 from __future__ import annotations
 import logging
 from queue import SimpleQueue
 from typing import Any, Optional
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic/util.py` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic/util.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/PKG-INFO` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertmanagermeshtastic
-Version: 2023.8.1.13
+Version: 2023.8.1.14
 Summary: A proxy to forward messages received via HTTP to MESHTASTIC
 Home-page: https://github.com/Apfelwurm/alertmanagermeshtastic
 Author: Alexander Volz
 Author-email: github@volzit.de
 License: MIT
 Project-URL: Source code, https://github.com/Apfelwurm/alertmanagermeshtastic
 Project-URL: Changelog, https://github.com/Apfelwurm/alertmanagermeshtastic/releases
@@ -39,15 +39,15 @@
 [![github](https://img.shields.io/badge/github-repository-important.svg?logo=Github)](https://github.com/Apfelwurm/alertmanagermeshtastic)
 [![pypi](https://img.shields.io/badge/pypi-package-important.svg?logo=Pypi)](https://pypi.org/project/alertmanagermeshtastic)
 
 
 This little Adapter receives alertmanager webhooks and sends the notifications via a over serial attached Meshtastic device to the specified nodeID.
 
 > **Warning**
-> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
+> Caution: The Tests that are provided for the code in this repository are not currently updated! Also this is a quickly hacked together peace of software, that has not built any security in it at the moment. Also the way that the ack is checked is not optimal, so messages tend to take longer to get to the device, but are delivered for sure(maybe multiple times). If you have the skill and the time to contribute in any way, take a look at the [Contribution section](#contribution)
 
 ## Credits
 This is based on the work of https://github.com/homeworkprod/weitersager
 Thanks to [GUVWAF](https://github.com/GUVWAF) for the support and thanks to the whole meshtastic team for this awsome software!
 
 ##  Alertmanager configuration example
```

### Comparing `alertmanagermeshtastic-2023.8.1.13/src/alertmanagermeshtastic.egg-info/SOURCES.txt` & `alertmanagermeshtastic-2023.8.1.14/src/alertmanagermeshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/tests/test_create_announcer.py` & `alertmanagermeshtastic-2023.8.1.14/tests/test_create_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/tests/test_dummy_announcer.py` & `alertmanagermeshtastic-2023.8.1.14/tests/test_dummy_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/tests/test_load_config.py` & `alertmanagermeshtastic-2023.8.1.14/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/tests/test_meshtastic_announcer.py` & `alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_announcer.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/tests/test_meshtastic_channel.py` & `alertmanagermeshtastic-2023.8.1.14/tests/test_meshtastic_channel.py`

 * *Files identical despite different names*

### Comparing `alertmanagermeshtastic-2023.8.1.13/tests/test_token_cli.py` & `alertmanagermeshtastic-2023.8.1.14/tests/test_token_cli.py`

 * *Files identical despite different names*

