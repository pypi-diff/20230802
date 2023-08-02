# Comparing `tmp/dtsh-0.1.0a6.tar.gz` & `tmp/dtsh-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtsh-0.1.0a6.tar", last modified: Thu Apr 27 04:55:44 2023, max compression
+gzip compressed data, was "dtsh-0.1.0b1.tar", last modified: Wed Aug  2 09:58:17 2023, max compression
```

## Comparing `dtsh-0.1.0a6.tar` & `dtsh-0.1.0b1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/
--rw-r--r--   0 chris     (1000) chris     (1000)    11357 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     2580 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     1589 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/README.rst
--rw-r--r--   0 chris     (1000) chris     (1000)       81 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/setup.cfg
--rw-r--r--   0 chris     (1000) chris     (1000)     6619 2023-04-27 04:21:52.000000 dtsh-0.1.0a6/setup.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.920066 dtsh-0.1.0a6/src/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.921066 dtsh-0.1.0a6/src/devicetree/
--rw-r--r--   0 chris     (1000) chris     (1000)      115 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    73804 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/dtlib.py
--rw-r--r--   0 chris     (1000) chris     (1000)   110651 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/edtlib.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5815 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/devicetree/grutils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.923066 dtsh-0.1.0a6/src/dtsh/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/src/dtsh/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4895 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/autocomp.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4277 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_alias.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4003 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_cat.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1676 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_cd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4445 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_chosen.py
--rw-r--r--   0 chris     (1000) chris     (1000)    24126 2023-04-27 04:05:16.000000 dtsh-0.1.0a6/src/dtsh/builtin_find.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10044 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_ls.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4755 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_man.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1104 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_pwd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5637 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_tree.py
--rw-r--r--   0 chris     (1000) chris     (1000)    15188 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/builtin_uname.py
--rw-r--r--   0 chris     (1000) chris     (1000)      643 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/src/dtsh/cli.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3914 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/config.py
--rw-r--r--   0 chris     (1000) chris     (1000)    52057 2023-04-27 04:21:39.000000 dtsh-0.1.0a6/src/dtsh/dtsh.py
--rw-r--r--   0 chris     (1000) chris     (1000)    22997 2023-04-27 04:14:38.000000 dtsh-0.1.0a6/src/dtsh/man.py
--rw-r--r--   0 chris     (1000) chris     (1000)      989 2023-04-27 02:02:51.000000 dtsh-0.1.0a6/src/dtsh/rl.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13355 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/session.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3351 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/shell.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8540 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/systools.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3595 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/term.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2576 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/src/dtsh/theme
--rw-r--r--   0 chris     (1000) chris     (1000)    60671 2023-04-26 23:55:06.000000 dtsh-0.1.0a6/src/dtsh/tui.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/src/dtsh.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     2580 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      879 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      149 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       16 2023-04-27 04:55:44.000000 dtsh-0.1.0a6/src/dtsh.egg-info/top_level.txt
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-04-27 04:55:44.924066 dtsh-0.1.0a6/tests/
--rw-r--r--   0 chris     (1000) chris     (1000)     3702 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/tests/test_autocomp.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13172 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/tests/test_dtsh.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1887 2023-04-22 16:49:35.000000 dtsh-0.1.0a6/tests/test_shell.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-08-02 09:58:17.278093 dtsh-0.1.0b1/
+-rw-r--r--   0 chris     (1000) chris     (1000)    11357 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     2579 2023-08-02 09:58:17.278093 dtsh-0.1.0b1/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1589 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/README.rst
+-rw-r--r--   0 chris     (1000) chris     (1000)       81 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-08-02 09:58:17.278093 dtsh-0.1.0b1/setup.cfg
+-rw-r--r--   0 chris     (1000) chris     (1000)     6618 2023-08-02 09:38:03.000000 dtsh-0.1.0b1/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-08-02 09:58:17.273093 dtsh-0.1.0b1/src/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-08-02 09:58:17.275093 dtsh-0.1.0b1/src/devicetree/
+-rw-r--r--   0 chris     (1000) chris     (1000)      115 2023-08-02 03:46:26.000000 dtsh-0.1.0b1/src/devicetree/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1227 2023-08-02 09:38:03.000000 dtsh-0.1.0b1/src/devicetree/_private.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    75929 2023-08-02 09:38:03.000000 dtsh-0.1.0b1/src/devicetree/dtlib.py
+-rw-r--r--   0 chris     (1000) chris     (1000)   117550 2023-08-02 09:38:03.000000 dtsh-0.1.0b1/src/devicetree/edtlib.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5815 2023-08-02 03:46:26.000000 dtsh-0.1.0b1/src/devicetree/grutils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-08-02 09:58:17.277093 dtsh-0.1.0b1/src/dtsh/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4895 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/autocomp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4277 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_alias.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4003 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_cat.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1676 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_cd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4445 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_chosen.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    24126 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_find.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10044 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_ls.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4755 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_man.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1104 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_pwd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5637 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_tree.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    15188 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/builtin_uname.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      643 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/cli.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3914 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/config.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    52057 2023-08-02 09:38:03.000000 dtsh-0.1.0b1/src/dtsh/dtsh.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    22997 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/man.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      989 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/rl.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13355 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/session.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3351 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/shell.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     8540 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/systools.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3595 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/term.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2576 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/theme
+-rw-r--r--   0 chris     (1000) chris     (1000)    60671 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/src/dtsh/tui.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-08-02 09:58:17.277093 dtsh-0.1.0b1/src/dtsh.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     2579 2023-08-02 09:58:17.000000 dtsh-0.1.0b1/src/dtsh.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      906 2023-08-02 09:58:17.000000 dtsh-0.1.0b1/src/dtsh.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2023-08-02 09:58:17.000000 dtsh-0.1.0b1/src/dtsh.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2023-08-02 09:58:17.000000 dtsh-0.1.0b1/src/dtsh.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      149 2023-08-02 09:58:17.000000 dtsh-0.1.0b1/src/dtsh.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       16 2023-08-02 09:58:17.000000 dtsh-0.1.0b1/src/dtsh.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2023-08-02 09:58:17.278093 dtsh-0.1.0b1/tests/
+-rw-r--r--   0 chris     (1000) chris     (1000)     3702 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/tests/test_autocomp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13172 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/tests/test_dtsh.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1887 2023-05-16 12:34:38.000000 dtsh-0.1.0b1/tests/test_shell.py
```

### Comparing `dtsh-0.1.0a6/LICENSE` & `dtsh-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/PKG-INFO` & `dtsh-0.1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dtsh
-Version: 0.1.0a6
+Version: 0.1.0b1
 Summary: Shell-like interface with Zephyr devicetree and bindings
 Home-page: https://github.com/dottspina/dtsh
 Author: Chris Duf
 Author-email: chris@openmarl.org
 License: Apache License version 2.0
 Project-URL: Bug Reports, https://github.com/dottspina/dtsh/issues
 Project-URL: Source, https://github.com/dottspina/dtsh
 Keywords: devicetree,zephyr,dts,embedded
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dtsh-0.1.0a6/README.rst` & `dtsh-0.1.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/setup.py` & `dtsh-0.1.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
     #
     # See also: https://peps.python.org/pep-0440/
     #
-    version="0.1.0a6",
+    version="0.1.0b1",
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     #
     description="Shell-like interface with Zephyr devicetree and bindings",
 
@@ -66,15 +66,15 @@
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     #
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Embedded Systems",
         # Pick your license as you wish
         "License :: OSI Approved :: Apache Software License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
```

### Comparing `dtsh-0.1.0a6/src/devicetree/dtlib.py` & `dtsh-0.1.0b1/src/devicetree/dtlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import errno
 import os
 import re
 import string
 import sys
 import textwrap
 from typing import Any, Dict, Iterable, List, \
-    NamedTuple, NoReturn, Optional, Set, Tuple, Union
+    NamedTuple, NoReturn, Optional, Set, Tuple, TYPE_CHECKING, Union
 
 # NOTE: tests/test_dtlib.py is the test suite for this library.
 
 class DTError(Exception):
     "Exception raised for devicetree-related errors"
 
 class Node:
@@ -86,15 +86,15 @@
 
     def __init__(self, name: str, parent: Optional['Node'], dt: 'DT'):
         """
         Node constructor. Not meant to be called directly by clients.
         """
         # Remember to update DT.__deepcopy__() if you change this.
 
-        self.name = name
+        self._name = name
         self.props: Dict[str, 'Property'] = {}
         self.nodes: Dict[str, 'Node'] = {}
         self.labels: List[str] = []
         self.parent = parent
         self.dt = dt
 
         self._omit_if_no_ref = False
@@ -105,27 +105,38 @@
         if not name == "/":
             for char in name:
                 if char not in _nodename_chars:
                     dt._parse_error(f"{self.path}: bad character '{char}' "
                                     "in node name")
 
     @property
+    def name(self) -> str:
+        """
+        See the class documentation.
+        """
+        # Converted to a property to discourage renaming -- that has to be done
+        # via DT.move_node.
+        return self._name
+
+    @property
     def unit_addr(self) -> str:
         """
         See the class documentation.
         """
         return self.name.partition("@")[2]
 
     @property
     def path(self) -> str:
         """
         See the class documentation.
         """
         node_names = []
 
+        # This dynamic computation is required to be able to move
+        # nodes in the DT class.
         cur = self
         while cur.parent:
             node_names.append(cur.name)
             cur = cur.parent
 
         return "/" + "/".join(reversed(node_names))
 
@@ -306,15 +317,15 @@
         # _MarkerType.LABEL, for a label on/within data. Node paths
         # and phandles need to be patched in after parsing.
         self._markers: List[List] = []
 
     @property
     def type(self) -> Type:
         """
-        See the class docstring.
+        See the class documentation.
         """
         # Data labels (e.g. 'foo = label: <3>') are irrelevant, so filter them
         # out
         types = [marker[1] for marker in self._markers
                  if marker[1] != _MarkerType.LABEL]
 
         if not types:
@@ -750,14 +761,16 @@
         self.memreserves: List[Tuple[Set[str], int, int]] = []
         self.filename = filename
 
         self._force = force
 
         if filename is not None:
             self._parse_file(filename, include_path)
+        else:
+            self._include_path: List[str] = []
 
     @property
     def root(self) -> Node:
         """
         See the class documentation.
         """
         # This is necessary because mypy can't tell that we never
@@ -800,22 +813,69 @@
             _err(f"no alias '{alias}' found -- did you forget the leading "
                  "'/' in the node path?")
 
         return _root_and_path_to_node(self.alias2node[alias], rest, path)
 
     def has_node(self, path: str) -> bool:
         """
-        Returns True if the path or alias 'path' exists. See Node.get_node().
+        Returns True if the path or alias 'path' exists. See DT.get_node().
         """
         try:
             self.get_node(path)
             return True
         except DTError:
             return False
 
+    def move_node(self, node: Node, new_path: str):
+        """
+        Move a node 'node' to a new path 'new_path'. The entire subtree
+        rooted at 'node' is moved along with it.
+
+        You cannot move the root node or provide a 'new_path' value
+        where a node already exists. This method raises an exception
+        in both cases.
+
+        As a restriction on the current implementation, the parent node
+        of the new path must exist.
+        """
+        if node is self.root:
+            _err("the root node can't be moved")
+
+        if self.has_node(new_path):
+            _err(f"can't move '{node.path}' to '{new_path}': "
+                 'destination node exists')
+
+        if not new_path.startswith('/'):
+            _err(f"path '{new_path}' doesn't start with '/'")
+
+        for component in new_path.split('/'):
+            for char in component:
+                if char not in _nodename_chars:
+                    _err(f"new path '{new_path}': bad character '{char}'")
+
+        old_name = node.name
+        old_path = node.path
+
+        new_parent_path, _, new_name = new_path.rpartition('/')
+        if new_parent_path == '':
+            # '/foo'.rpartition('/') is ('', '/', 'foo').
+            new_parent_path = '/'
+        if not self.has_node(new_parent_path):
+            _err(f"can't move '{old_path}' to '{new_path}': "
+                 f"parent node '{new_parent_path}' doesn't exist")
+        new_parent = self.get_node(new_parent_path)
+        if TYPE_CHECKING:
+            assert new_parent is not None
+            assert node.parent is not None
+
+        del node.parent.nodes[old_name]
+        node._name = new_name
+        node.parent = new_parent
+        new_parent.nodes[new_name] = node
+
     def node_iter(self) -> Iterable[Node]:
         """
         Returns a generator for iterating over all nodes in the devicetree.
 
         For example, this will print the name of each node that has a property
         called 'foo':
 
@@ -948,15 +1008,15 @@
 
         return ret
 
     #
     # Parsing
     #
 
-    def _parse_file(self, filename, include_path):
+    def _parse_file(self, filename: str, include_path: Iterable[str]):
         self._include_path = list(include_path)
 
         with open(filename, encoding="utf-8") as f:
             self._file_contents = f.read()
 
         self._tok_i = self._tok_end_i = 0
         self._filestack: List[_FileStackElt] = []
@@ -1037,15 +1097,15 @@
                 else:
                     label = None
 
                 try:
                     node = self._ref2node(tok.val)
                 except DTError as e:
                     self._parse_error(e)
-                node = self._parse_node(node)
+                self._parse_node(node)
 
                 if label:
                     _append_no_dup(node.labels, label)
 
             elif tok.id == _T.DEL_NODE:
                 self._next_ref2node()._del()
                 self._expect_token(";")
@@ -1059,16 +1119,15 @@
                     self._parse_error("no root node defined")
                 return
 
             else:
                 self._parse_error("expected '/' or label reference (&foo)")
 
     def _parse_node(self, node):
-        # Parses the '{ ... };' part of 'node-name { ... };'. Returns the new
-        # Node.
+        # Parses the '{ ... };' part of 'node-name { ... };'.
 
         # We need to track which child nodes were defined in this set
         # of curly braces in order to reject duplicate node names.
         current_child_names = set()
 
         self._expect_token("{")
         while True:
@@ -1129,15 +1188,15 @@
                 if tok2.id != _T.PROPNODENAME:
                     self._parse_error("expected property name")
                 node.props.pop(tok2.val, None)
                 self._expect_token(";")
 
             elif tok.val == "}":
                 self._expect_token(";")
-                return node
+                return
 
             else:
                 self._parse_error("expected node name, property name, or '}'")
 
     def _parse_propnode_labels(self):
         # _parse_node() helpers for parsing labels and /omit-if-no-ref/s before
         # nodes and properties. Returns a (<label list>, <omit-if-no-ref bool>)
@@ -1972,15 +2031,15 @@
         _err(f"{data!r} is {len(data)} bytes long, "
              f"expected a length that's a a multiple of {length}")
 
     return [int.from_bytes(data[i:i + length], "big", signed=signed)
             for i in range(0, len(data), length)]
 
 #
-# Public constants
+# Private helpers
 #
 
 def _check_is_bytes(data):
     if not isinstance(data, bytes):
         _err(f"'{data}' has type '{type(data).__name__}', expected 'bytes'")
 
 def _check_length_positive(length):
```

### Comparing `dtsh-0.1.0a6/src/devicetree/edtlib.py` & `dtsh-0.1.0b1/src/devicetree/edtlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,485 +65,791 @@
 #   APIs, and "doc comments" for internal functions.
 #
 #   @properties are documented in the class docstring, as if they were
 #   variables. See the existing @properties for a template.
 
 from collections import defaultdict
 from copy import deepcopy
+from dataclasses import dataclass
+from typing import Any, Callable, Dict, Iterable, List, NoReturn, \
+    Optional, Set, TYPE_CHECKING, Tuple, Union
 import logging
 import os
 import re
 
 import yaml
 try:
     # Use the C LibYAML parser if available, rather than the Python parser.
     # This makes e.g. gen_defines.py more than twice as fast.
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader     # type: ignore
 
 from devicetree.dtlib import DT, DTError, to_num, to_nums, Type
+from devicetree.dtlib import Node as dtlib_Node
+from devicetree.dtlib import Property as dtlib_Property
 from devicetree.grutils import Graph
-
+from devicetree._private import _slice_helper
 
 #
 # Public classes
 #
 
 
-class EDT:
+class Binding:
     """
-    Represents a devicetree augmented with information from bindings.
+    Represents a parsed binding.
 
-    These attributes are available on EDT objects:
+    These attributes are available on Binding objects:
 
-    nodes:
-      A list of Node objects for the nodes that appear in the devicetree
+    path:
+      The absolute path to the file defining the binding.
 
-    compat2nodes:
-      A collections.defaultdict that maps each 'compatible' string that appears
-      on some Node to a list of Nodes with that compatible.
+    description:
+      The free-form description of the binding, or None.
 
-    compat2okay:
-      Like compat2nodes, but just for nodes with status 'okay'.
+    compatible:
+      The compatible string the binding matches.
 
-    compat2vendor:
-      A collections.defaultdict that maps each 'compatible' string that appears
-      on some Node to a vendor name parsed from vendor_prefixes.
+      This may be None. For example, it's None when the Binding is inferred
+      from node properties. It can also be None for Binding objects created
+      using 'child-binding:' with no compatible.
 
-    compat2model:
-      A collections.defaultdict that maps each 'compatible' string that appears
-      on some Node to a model name parsed from that compatible.
+    prop2specs:
+      A dict mapping property names to PropertySpec objects
+      describing those properties' values.
 
-    label2node:
-      A dict that maps a node label to the node with that label.
+    specifier2cells:
+      A dict that maps specifier space names (like "gpio",
+      "clock", "pwm", etc.) to lists of cell names.
 
-    dep_ord2node:
-      A dict that maps an ordinal to the node with that dependency ordinal.
+      For example, if the binding YAML contains 'pin' and 'flags' cell names
+      for the 'gpio' specifier space, like this:
 
-    chosen_nodes:
-      A dict that maps the properties defined on the devicetree's /chosen
-      node to their values. 'chosen' is indexed by property name (a string),
-      and values are converted to Node objects. Note that properties of the
-      /chosen node which can't be converted to a Node are not included in
-      the value.
+          gpio-cells:
+          - pin
+          - flags
 
-    dts_path:
-      The .dts path passed to __init__()
+      Then the Binding object will have a 'specifier2cells' attribute mapping
+      "gpio" to ["pin", "flags"]. A missing key should be interpreted as zero
+      cells.
 
-    dts_source:
-      The final DTS source code of the loaded devicetree after merging nodes
-      and processing /delete-node/ and /delete-property/, as a string
+    raw:
+      The binding as an object parsed from YAML.
 
-    bindings_dirs:
-      The bindings directory paths passed to __init__()
+    bus:
+      If nodes with this binding's 'compatible' describe a bus, a string
+      describing the bus type (like "i2c") or a list describing supported
+      protocols (like ["i3c", "i2c"]). None otherwise.
 
-    scc_order:
-      A list of lists of Nodes. All elements of each list
-      depend on each other, and the Nodes in any list do not depend
-      on any Node in a subsequent list. Each list defines a Strongly
-      Connected Component (SCC) of the graph.
+      Note that this is the raw value from the binding where it can be
+      a string or a list. Use "buses" instead unless you need the raw
+      value, where "buses" is always a list.
 
-      For an acyclic graph each list will be a singleton. Cycles
-      will be represented by lists with multiple nodes. Cycles are
-      not expected to be present in devicetree graphs.
+    buses:
+      Deprived property from 'bus' where 'buses' is a list of bus(es),
+      for example, ["i2c"] or ["i3c", "i2c"]. Or an empty list if there is
+      no 'bus:' in this binding.
 
-    The standard library's pickle module can be used to marshal and
-    unmarshal EDT objects.
+    on_bus:
+      If nodes with this binding's 'compatible' appear on a bus, a string
+      describing the bus type (like "i2c"). None otherwise.
+
+    child_binding:
+      If this binding describes the properties of child nodes, then
+      this is a Binding object for those children; it is None otherwise.
+      A Binding object's 'child_binding.child_binding' is not None if there
+      are multiple levels of 'child-binding' descriptions in the binding.
     """
-    def __init__(self, dts, bindings_dirs,
-                 warn_reg_unit_address_mismatch=True,
-                 default_prop_types=True,
-                 support_fixed_partitions_on_any_bus=True,
-                 infer_binding_for_paths=None,
-                 vendor_prefixes=None,
-                 werror=False):
-        """EDT constructor.
 
-        dts:
-          Path to devicetree .dts file
+    def __init__(self, path: Optional[str], fname2path: Dict[str, str],
+                 raw: Any = None, require_compatible: bool = True,
+                 require_description: bool = True):
+        """
+        Binding constructor.
 
-        bindings_dirs:
-          List of paths to directories containing bindings, in YAML format.
-          These directories are recursively searched for .yaml files.
+        path:
+          Path to binding YAML file. May be None.
 
-        warn_reg_unit_address_mismatch (default: True):
-          If True, a warning is logged if a node has a 'reg' property where
-          the address of the first entry does not match the unit address of the
-          node
+        fname2path:
+          Map from include files to their absolute paths. Must
+          not be None, but may be empty.
 
-        default_prop_types (default: True):
-          If True, default property types will be used when a node has no
-          bindings.
+        raw:
+          Optional raw content in the binding.
+          This does not have to have any "include:" lines resolved.
+          May be left out, in which case 'path' is opened and read.
+          This can be used to resolve child bindings, for example.
 
-        support_fixed_partitions_on_any_bus (default True):
-          If True, set the Node.bus for 'fixed-partitions' compatible nodes
-          to None.  This allows 'fixed-partitions' binding to match regardless
-          of the bus the 'fixed-partition' is under.
+        require_compatible:
+          If True, it is an error if the binding does not contain a
+          "compatible:" line. If False, a missing "compatible:" is
+          not an error. Either way, "compatible:" must be a string
+          if it is present in the binding.
 
-        infer_binding_for_paths (default: None):
-          An iterable of devicetree paths identifying nodes for which bindings
-          should be inferred from the node content.  (Child nodes are not
-          processed.)  Pass none if no nodes should support inferred bindings.
+        require_description:
+          If True, it is an error if the binding does not contain a
+          "description:" line. If False, a missing "description:" is
+          not an error. Either way, "description:" must be a string
+          if it is present in the binding.
+        """
+        self.path: Optional[str] = path
+        self._fname2path: Dict[str, str] = fname2path
 
-        vendor_prefixes (default: None):
-          A dict mapping vendor prefixes in compatible properties to their
-          descriptions. If given, compatibles in the form "manufacturer,device"
-          for which "manufacturer" is neither a key in the dict nor a specially
-          exempt set of grandfathered-in cases will cause warnings.
+        if raw is None:
+            if path is None:
+                _err("you must provide either a 'path' or a 'raw' argument")
+            with open(path, encoding="utf-8") as f:
+                raw = yaml.load(f, Loader=_BindingLoader)
 
-        werror (default: False):
-          If True, some edtlib specific warnings become errors. This currently
-          errors out if 'dts' has any deprecated properties set, or an unknown
-          vendor prefix is used.
-        """
-        self._warn_reg_unit_address_mismatch = warn_reg_unit_address_mismatch
-        self._default_prop_types = default_prop_types
-        self._fixed_partitions_no_bus = support_fixed_partitions_on_any_bus
-        self._infer_binding_for_paths = set(infer_binding_for_paths or [])
-        self._werror = bool(werror)
-        self._vendor_prefixes = vendor_prefixes or {}
+        # Merge any included files into self.raw. This also pulls in
+        # inherited child binding definitions, so it has to be done
+        # before initializing those.
+        self.raw: dict = self._merge_includes(raw, self.path)
 
-        self.dts_path = dts
-        self.bindings_dirs = bindings_dirs
+        # Recursively initialize any child bindings. These don't
+        # require a 'compatible' or 'description' to be well defined,
+        # but they must be dicts.
+        if "child-binding" in raw:
+            if not isinstance(raw["child-binding"], dict):
+                _err(f"malformed 'child-binding:' in {self.path}, "
+                     "expected a binding (dictionary with keys/values)")
+            self.child_binding: Optional['Binding'] = Binding(
+                path, fname2path,
+                raw=raw["child-binding"],
+                require_compatible=False,
+                require_description=False)
+        else:
+            self.child_binding = None
 
-        try:
-            self._dt = DT(dts)
-        except DTError as e:
-            raise EDTError(e) from e
-        _check_dt(self._dt)
+        # Make sure this is a well defined object.
+        self._check(require_compatible, require_description)
 
-        self._init_compat2binding()
-        self._init_nodes()
-        self._init_graph()
-        self._init_luts()
+        # Initialize look up tables.
+        self.prop2specs: Dict[str, 'PropertySpec'] = {}
+        for prop_name in self.raw.get("properties", {}).keys():
+            self.prop2specs[prop_name] = PropertySpec(prop_name, self)
+        self.specifier2cells: Dict[str, List[str]] = {}
+        for key, val in self.raw.items():
+            if key.endswith("-cells"):
+                self.specifier2cells[key[:-len("-cells")]] = val
 
-        self._check()
+    def __repr__(self) -> str:
+        if self.compatible:
+            compat = f" for compatible '{self.compatible}'"
+        else:
+            compat = ""
+        basename = os.path.basename(self.path or "")
+        return f"<Binding {basename}" + compat + ">"
 
-    def get_node(self, path):
-        """
-        Returns the Node at the DT path or alias 'path'. Raises EDTError if the
-        path or alias doesn't exist.
-        """
-        try:
-            return self._node2enode[self._dt.get_node(path)]
-        except DTError as e:
-            _err(e)
+    @property
+    def description(self) -> Optional[str]:
+        "See the class docstring"
+        return self.raw.get('description')
 
     @property
-    def chosen_nodes(self):
-        ret = {}
+    def compatible(self) -> Optional[str]:
+        "See the class docstring"
+        return self.raw.get('compatible')
 
-        try:
-            chosen = self._dt.get_node("/chosen")
-        except DTError:
-            return ret
+    @property
+    def bus(self) -> Union[None, str, List[str]]:
+        "See the class docstring"
+        return self.raw.get('bus')
 
-        for name, prop in chosen.props.items():
-            try:
-                node = prop.to_path()
-            except DTError:
-                # DTS value is not phandle or string, or path doesn't exist
-                continue
+    @property
+    def buses(self) -> List[str]:
+        "See the class docstring"
+        if self.raw.get('bus') is not None:
+            return self._buses
+        else:
+            return []
 
-            ret[name] = self._node2enode[node]
+    @property
+    def on_bus(self) -> Optional[str]:
+        "See the class docstring"
+        return self.raw.get('on-bus')
 
-        return ret
+    def _merge_includes(self, raw: dict, binding_path: Optional[str]) -> dict:
+        # Constructor helper. Merges included files in
+        # 'raw["include"]' into 'raw' using 'self._include_paths' as a
+        # source of include files, removing the "include" key while
+        # doing so.
+        #
+        # This treats 'binding_path' as the binding file being built up
+        # and uses it for error messages.
 
-    def chosen_node(self, name):
-        """
-        Returns the Node pointed at by the property named 'name' in /chosen, or
-        None if the property is missing
-        """
-        return self.chosen_nodes.get(name)
+        if "include" not in raw:
+            return raw
+
+        include = raw.pop("include")
+
+        # First, merge the included files together. If more than one included
+        # file has a 'required:' for a particular property, OR the values
+        # together, so that 'required: true' wins.
+
+        merged: Dict[str, Any] = {}
+
+        if isinstance(include, str):
+            # Simple scalar string case
+            _merge_props(merged, self._load_raw(include), None, binding_path,
+                         False)
+        elif isinstance(include, list):
+            # List of strings and maps. These types may be intermixed.
+            for elem in include:
+                if isinstance(elem, str):
+                    _merge_props(merged, self._load_raw(elem), None,
+                                 binding_path, False)
+                elif isinstance(elem, dict):
+                    name = elem.pop('name', None)
+                    allowlist = elem.pop('property-allowlist', None)
+                    blocklist = elem.pop('property-blocklist', None)
+                    child_filter = elem.pop('child-binding', None)
+
+                    if elem:
+                        # We've popped out all the valid keys.
+                        _err(f"'include:' in {binding_path} should not have "
+                             f"these unexpected contents: {elem}")
+
+                    _check_include_dict(name, allowlist, blocklist,
+                                        child_filter, binding_path)
+
+                    contents = self._load_raw(name)
+
+                    _filter_properties(contents, allowlist, blocklist,
+                                       child_filter, binding_path)
+                    _merge_props(merged, contents, None, binding_path, False)
+                else:
+                    _err(f"all elements in 'include:' in {binding_path} "
+                         "should be either strings or maps with a 'name' key "
+                         "and optional 'property-allowlist' or "
+                         f"'property-blocklist' keys, but got: {elem}")
+        else:
+            # Invalid item.
+            _err(f"'include:' in {binding_path} "
+                 f"should be a string or list, but has type {type(include)}")
+
+        # Next, merge the merged included files into 'raw'. Error out if
+        # 'raw' has 'required: false' while the merged included files have
+        # 'required: true'.
+
+        _merge_props(raw, merged, None, binding_path, check_required=True)
+
+        return raw
+
+    def _load_raw(self, fname: str) -> dict:
+        # Returns the contents of the binding given by 'fname' after merging
+        # any bindings it lists in 'include:' into it. 'fname' is just the
+        # basename of the file, so we check that there aren't multiple
+        # candidates.
+
+        path = self._fname2path.get(fname)
+
+        if not path:
+            _err(f"'{fname}' not found")
+
+        with open(path, encoding="utf-8") as f:
+            contents = yaml.load(f, Loader=_BindingLoader)
+            if not isinstance(contents, dict):
+                _err(f'{path}: invalid contents, expected a mapping')
+
+        return self._merge_includes(contents, path)
+
+    def _check(self, require_compatible: bool, require_description: bool):
+        # Does sanity checking on the binding.
+
+        raw = self.raw
+
+        if "compatible" in raw:
+            compatible = raw["compatible"]
+            if not isinstance(compatible, str):
+                _err(f"malformed 'compatible: {compatible}' "
+                     f"field in {self.path} - "
+                     f"should be a string, not {type(compatible).__name__}")
+        elif require_compatible:
+            _err(f"missing 'compatible' in {self.path}")
+
+        if "description" in raw:
+            description = raw["description"]
+            if not isinstance(description, str) or not description:
+                _err(f"malformed or empty 'description' in {self.path}")
+        elif require_description:
+            _err(f"missing 'description' in {self.path}")
+
+        # Allowed top-level keys. The 'include' key should have been
+        # removed by _load_raw() already.
+        ok_top = {"description", "compatible", "bus", "on-bus",
+                  "properties", "child-binding"}
+
+        # Descriptive errors for legacy bindings.
+        legacy_errors = {
+            "#cells": "expected *-cells syntax",
+            "child": "use 'bus: <bus>' instead",
+            "child-bus": "use 'bus: <bus>' instead",
+            "parent": "use 'on-bus: <bus>' instead",
+            "parent-bus": "use 'on-bus: <bus>' instead",
+            "sub-node": "use 'child-binding' instead",
+            "title": "use 'description' instead",
+        }
+
+        for key in raw:
+            if key in legacy_errors:
+                _err(f"legacy '{key}:' in {self.path}, {legacy_errors[key]}")
+
+            if key not in ok_top and not key.endswith("-cells"):
+                _err(f"unknown key '{key}' in {self.path}, "
+                     "expected one of {', '.join(ok_top)}, or *-cells")
+
+        if "bus" in raw:
+            bus = raw["bus"]
+            if not isinstance(bus, str) and \
+               (not isinstance(bus, list) and \
+                not all(isinstance(elem, str) for elem in bus)):
+                _err(f"malformed 'bus:' value in {self.path}, "
+                     "expected string or list of strings")
+
+            if isinstance(bus, list):
+                self._buses = bus
+            else:
+                # Convert bus into a list
+                self._buses = [bus]
+
+        if "on-bus" in raw and \
+           not isinstance(raw["on-bus"], str):
+            _err(f"malformed 'on-bus:' value in {self.path}, "
+                 "expected string")
+
+        self._check_properties()
+
+        for key, val in raw.items():
+            if key.endswith("-cells"):
+                if not isinstance(val, list) or \
+                   not all(isinstance(elem, str) for elem in val):
+                    _err(f"malformed '{key}:' in {self.path}, "
+                         "expected a list of strings")
+
+    def _check_properties(self) -> None:
+        # _check() helper for checking the contents of 'properties:'.
+
+        raw = self.raw
+
+        if "properties" not in raw:
+            return
+
+        ok_prop_keys = {"description", "type", "required",
+                        "enum", "const", "default", "deprecated",
+                        "specifier-space"}
+
+        for prop_name, options in raw["properties"].items():
+            for key in options:
+                if key not in ok_prop_keys:
+                    _err(f"unknown setting '{key}' in "
+                         f"'properties: {prop_name}: ...' in {self.path}, "
+                         f"expected one of {', '.join(ok_prop_keys)}")
+
+            _check_prop_by_type(prop_name, options, self.path)
+
+            for true_false_opt in ["required", "deprecated"]:
+                if true_false_opt in options:
+                    option = options[true_false_opt]
+                    if not isinstance(option, bool):
+                        _err(f"malformed '{true_false_opt}:' setting '{option}' "
+                             f"for '{prop_name}' in 'properties' in {self.path}, "
+                             "expected true/false")
+
+            if options.get("deprecated") and options.get("required"):
+                _err(f"'{prop_name}' in 'properties' in {self.path} should not "
+                      "have both 'deprecated' and 'required' set")
+
+            if "description" in options and \
+               not isinstance(options["description"], str):
+                _err("missing, malformed, or empty 'description' for "
+                     f"'{prop_name}' in 'properties' in {self.path}")
+
+            if "enum" in options and not isinstance(options["enum"], list):
+                _err(f"enum in {self.path} for property '{prop_name}' "
+                     "is not a list")
+
+
+class PropertySpec:
+    """
+    Represents a "property specification", i.e. the description of a
+    property provided by a binding file, like its type and description.
+
+    These attributes are available on PropertySpec objects:
+
+    binding:
+      The Binding object which defined this property.
+
+    name:
+      The property's name.
+
+    path:
+      The file where this property was defined. In case a binding includes
+      other bindings, this is the file where the property was last modified.
+
+    type:
+      The type of the property as a string, as given in the binding.
+
+    description:
+      The free-form description of the property as a string, or None.
+
+    enum:
+      A list of values the property may take as given in the binding, or None.
+
+    enum_tokenizable:
+      True if enum is not None and all the values in it are tokenizable;
+      False otherwise.
+
+      A property must have string type and an "enum:" in its binding to be
+      tokenizable. Additionally, the "enum:" values must be unique after
+      converting all non-alphanumeric characters to underscores (so "foo bar"
+      and "foo_bar" in the same "enum:" would not be tokenizable).
+
+    enum_upper_tokenizable:
+      Like 'enum_tokenizable', with the additional restriction that the
+      "enum:" values must be unique after uppercasing and converting
+      non-alphanumeric characters to underscores.
+
+    const:
+      The property's constant value as given in the binding, or None.
+
+    default:
+      The property's default value as given in the binding, or None.
+
+    deprecated:
+      True if the property is deprecated; False otherwise.
+
+    required:
+      True if the property is marked required; False otherwise.
+
+    specifier_space:
+      The specifier space for the property as given in the binding, or None.
+    """
+
+    def __init__(self, name: str, binding: Binding):
+        self.binding: Binding = binding
+        self.name: str = name
+        self._raw: Dict[str, Any] = self.binding.raw["properties"][name]
+
+    def __repr__(self) -> str:
+        return f"<PropertySpec {self.name} type '{self.type}'>"
 
     @property
-    def dts_source(self):
-        return f"{self._dt}"
+    def path(self) -> Optional[str]:
+        "See the class docstring"
+        return self.binding.path
 
-    def __repr__(self):
-        return f"<EDT for '{self.dts_path}', binding directories " \
-            f"'{self.bindings_dirs}'>"
+    @property
+    def type(self) -> str:
+        "See the class docstring"
+        return self._raw["type"]
 
     @property
-    def scc_order(self):
-        try:
-            return self._graph.scc_order()
-        except Exception as e:
-            raise EDTError(e)
+    def description(self) -> Optional[str]:
+        "See the class docstring"
+        return self._raw.get("description")
 
-    def _init_graph(self):
-        # Constructs a graph of dependencies between Node instances,
-        # which is usable for computing a partial order over the dependencies.
-        # The algorithm supports detecting dependency loops.
-        #
-        # Actually computing the SCC order is lazily deferred to the
-        # first time the scc_order property is read.
+    @property
+    def enum(self) -> Optional[list]:
+        "See the class docstring"
+        return self._raw.get("enum")
 
-        self._graph = Graph()
+    @property
+    def enum_tokenizable(self) -> bool:
+        "See the class docstring"
+        if not hasattr(self, '_enum_tokenizable'):
+            if self.type != 'string' or self.enum is None:
+                self._enum_tokenizable = False
+            else:
+                # Saving _as_tokens here lets us reuse it in
+                # enum_upper_tokenizable.
+                self._as_tokens = [re.sub(_NOT_ALPHANUM_OR_UNDERSCORE,
+                                          '_', value)
+                                   for value in self.enum]
+                self._enum_tokenizable = (len(self._as_tokens) ==
+                                          len(set(self._as_tokens)))
 
-        for node in self.nodes:
-            # A Node always depends on its parent.
-            for child in node.children.values():
-                self._graph.add_edge(child, node)
+        return self._enum_tokenizable
 
-            # A Node depends on any Nodes present in 'phandle',
-            # 'phandles', or 'phandle-array' property values.
-            for prop in node.props.values():
-                if prop.type == 'phandle':
-                    self._graph.add_edge(node, prop.val)
-                elif prop.type == 'phandles':
-                    for phandle_node in prop.val:
-                        self._graph.add_edge(node, phandle_node)
-                elif prop.type == 'phandle-array':
-                    for cd in prop.val:
-                        if cd is None:
-                            continue
-                        self._graph.add_edge(node, cd.controller)
+    @property
+    def enum_upper_tokenizable(self) -> bool:
+        "See the class docstring"
+        if not hasattr(self, '_enum_upper_tokenizable'):
+            if not self.enum_tokenizable:
+                self._enum_upper_tokenizable = False
+            else:
+                self._enum_upper_tokenizable = \
+                    (len(self._as_tokens) ==
+                     len(set(x.upper() for x in self._as_tokens)))
+        return self._enum_upper_tokenizable
 
-            # A Node depends on whatever supports the interrupts it
-            # generates.
-            for intr in node.interrupts:
-                self._graph.add_edge(node, intr.controller)
+    @property
+    def const(self) -> Union[None, int, List[int], str, List[str]]:
+        "See the class docstring"
+        return self._raw.get("const")
 
-    def _init_compat2binding(self):
-        # Creates self._compat2binding, a dictionary that maps
-        # (<compatible>, <bus>) tuples (both strings) to Binding objects.
-        #
-        # The Binding objects are created from YAML files discovered
-        # in self.bindings_dirs as needed.
-        #
-        # For example, self._compat2binding["company,dev", "can"]
-        # contains the Binding for the 'company,dev' device, when it
-        # appears on the CAN bus.
-        #
-        # For bindings that don't specify a bus, <bus> is None, so that e.g.
-        # self._compat2binding["company,notonbus", None] is the Binding.
-        #
-        # Only bindings for 'compatible' strings that appear in the devicetree
-        # are loaded.
+    @property
+    def default(self) -> Union[None, int, List[int], str, List[str]]:
+        "See the class docstring"
+        return self._raw.get("default")
 
-        dt_compats = _dt_compats(self._dt)
-        # Searches for any 'compatible' string mentioned in the devicetree
-        # files, with a regex
-        dt_compats_search = re.compile(
-            "|".join(re.escape(compat) for compat in dt_compats)
-        ).search
+    @property
+    def required(self) -> bool:
+        "See the class docstring"
+        return self._raw.get("required", False)
 
-        self._binding_paths = _binding_paths(self.bindings_dirs)
-        self._binding_fname2path = {os.path.basename(path): path
-                                    for path in self._binding_paths}
+    @property
+    def deprecated(self) -> bool:
+        "See the class docstring"
+        return self._raw.get("deprecated", False)
 
-        self._compat2binding = {}
-        for binding_path in self._binding_paths:
-            with open(binding_path, encoding="utf-8") as f:
-                contents = f.read()
+    @property
+    def specifier_space(self) -> Optional[str]:
+        "See the class docstring"
+        return self._raw.get("specifier-space")
 
-            # As an optimization, skip parsing files that don't contain any of
-            # the .dts 'compatible' strings, which should be reasonably safe
-            if not dt_compats_search(contents):
-                continue
+PropertyValType = Union[int, str,
+                        List[int], List[str],
+                        'Node', List['Node'],
+                        List[Optional['ControllerAndData']],
+                        bytes, None]
 
-            # Load the binding and check that it actually matches one of the
-            # compatibles. Might get false positives above due to comments and
-            # stuff.
 
-            try:
-                # Parsed PyYAML output (Python lists/dictionaries/strings/etc.,
-                # representing the file)
-                raw = yaml.load(contents, Loader=_BindingLoader)
-            except yaml.YAMLError as e:
-                _err(
-                        f"'{binding_path}' appears in binding directories "
-                        f"but isn't valid YAML: {e}")
-                continue
+@dataclass
+class Property:
+    """
+    Represents a property on a Node, as set in its DT node and with
+    additional info from the 'properties:' section of the binding.
 
-            # Convert the raw data to a Binding object, erroring out
-            # if necessary.
-            binding = self._binding(raw, binding_path, dt_compats)
+    Only properties mentioned in 'properties:' get created. Properties of type
+    'compound' currently do not get Property instances, as it's not clear
+    what to generate for them.
 
-            # Register the binding in self._compat2binding, along with
-            # any child bindings that have their own compatibles.
-            while binding is not None:
-                if binding.compatible:
-                    self._register_binding(binding)
-                binding = binding.child_binding
+    These attributes are available on Property objects. Several are
+    just convenience accessors for attributes on the PropertySpec object
+    accessible via the 'spec' attribute.
 
-    def _binding(self, raw, binding_path, dt_compats):
-        # Convert a 'raw' binding from YAML to a Binding object and return it.
-        #
-        # Error out if the raw data looks like an invalid binding.
-        #
-        # Return None if the file doesn't contain a binding or the
-        # binding's compatible isn't in dt_compats.
+    These attributes are available on Property objects:
 
-        # Get the 'compatible:' string.
-        if raw is None or "compatible" not in raw:
-            # Empty file, binding fragment, spurious file, etc.
-            return None
+    spec:
+      The PropertySpec object which specifies this property.
 
-        compatible = raw["compatible"]
+    val:
+      The value of the property, with the format determined by spec.type,
+      which comes from the 'type:' string in the binding.
 
-        if compatible not in dt_compats:
-            # Not a compatible we care about.
-            return None
+        - For 'type: int/array/string/string-array', 'val' is what you'd expect
+          (a Python integer or string, or a list of them)
 
-        # Initialize and return the Binding object.
-        return Binding(binding_path, self._binding_fname2path, raw=raw)
+        - For 'type: phandle' and 'type: path', 'val' is the pointed-to Node
+          instance
 
-    def _register_binding(self, binding):
-        # Do not allow two different bindings to have the same
-        # 'compatible:'/'on-bus:' combo
-        old_binding = self._compat2binding.get((binding.compatible,
-                                                binding.on_bus))
-        if old_binding:
-            msg = (f"both {old_binding.path} and {binding.path} have "
-                   f"'compatible: {binding.compatible}'")
-            if binding.on_bus is not None:
-                msg += f" and 'on-bus: {binding.on_bus}'"
-            _err(msg)
+        - For 'type: phandles', 'val' is a list of the pointed-to Node
+          instances
 
-        # Register the binding.
-        self._compat2binding[binding.compatible, binding.on_bus] = binding
+        - For 'type: phandle-array', 'val' is a list of ControllerAndData
+          instances. See the documentation for that class.
 
-    def _init_nodes(self):
-        # Creates a list of edtlib.Node objects from the dtlib.Node objects, in
-        # self.nodes
+    node:
+      The Node instance the property is on
 
-        # Maps each dtlib.Node to its corresponding edtlib.Node
-        self._node2enode = {}
+    name:
+      Convenience for spec.name.
 
-        self.nodes = []
+    description:
+      Convenience for spec.description with leading and trailing whitespace
+      (including newlines) removed. May be None.
 
-        for dt_node in self._dt.node_iter():
-            # Warning: We depend on parent Nodes being created before their
-            # children. This is guaranteed by node_iter().
-            node = Node()
-            node.edt = self
-            node._node = dt_node
-            if "compatible" in node._node.props:
-                node.compats = node._node.props["compatible"].to_strings()
-            else:
-                node.compats = []
-            node.bus_node = node._bus_node(self._fixed_partitions_no_bus)
-            node._init_binding()
-            node._init_regs()
-            node._init_ranges()
+    type:
+      Convenience for spec.type.
 
-            self.nodes.append(node)
-            self._node2enode[dt_node] = node
+    val_as_token:
+      The value of the property as a token, i.e. with non-alphanumeric
+      characters replaced with underscores. This is only safe to access
+      if 'spec.enum_tokenizable' returns True.
 
-        for node in self.nodes:
-            # These depend on all Node objects having been created, because
-            # they (either always or sometimes) reference other nodes, so we
-            # run them separately
-            node._init_props(default_prop_types=self._default_prop_types,
-                             err_on_deprecated=self._werror)
-            node._init_interrupts()
-            node._init_pinctrls()
+    enum_index:
+      The index of 'val' in 'spec.enum' (which comes from the 'enum:' list
+      in the binding), or None if spec.enum is None.
+    """
 
-        if self._warn_reg_unit_address_mismatch:
-            # This warning matches the simple_bus_reg warning in dtc
-            for node in self.nodes:
-                if node.regs and node.regs[0].addr != node.unit_addr:
-                    _LOG.warning("unit address and first address in 'reg' "
-                                 f"(0x{node.regs[0].addr:x}) don't match for "
-                                 f"{node.path}")
+    spec: PropertySpec
+    val: PropertyValType
+    node: 'Node'
 
-    def _init_luts(self):
-        # Initialize node lookup tables (LUTs).
+    @property
+    def name(self) -> str:
+        "See the class docstring"
+        return self.spec.name
 
-        self.label2node = {}
-        self.dep_ord2node = {}
-        self.compat2nodes = defaultdict(list)
-        self.compat2okay = defaultdict(list)
-        self.compat2vendor = defaultdict(str)
-        self.compat2model = defaultdict(str)
+    @property
+    def description(self) -> Optional[str]:
+        "See the class docstring"
+        return self.spec.description.strip() if self.spec.description else None
 
-        for node in self.nodes:
-            for label in node.labels:
-                self.label2node[label] = node
+    @property
+    def type(self) -> str:
+        "See the class docstring"
+        return self.spec.type
 
-            for compat in node.compats:
-                self.compat2nodes[compat].append(node)
+    @property
+    def val_as_token(self) -> str:
+        "See the class docstring"
+        assert isinstance(self.val, str)
+        return str_as_token(self.val)
 
-                if node.status == "okay":
-                    self.compat2okay[compat].append(node)
+    @property
+    def enum_index(self) -> Optional[int]:
+        "See the class docstring"
+        enum = self.spec.enum
+        return enum.index(self.val) if enum else None
 
-                if compat in self.compat2vendor:
-                    continue
 
-                # The regular expression comes from dt-schema.
-                compat_re = r'^[a-zA-Z][a-zA-Z0-9,+\-._]+$'
-                if not re.match(compat_re, compat):
-                    _err(f"node '{node.path}' compatible '{compat}' "
-                         'must match this regular expression: '
-                         f"'{compat_re}'")
+@dataclass
+class Register:
+    """
+    Represents a register on a node.
 
-                if ',' in compat and self._vendor_prefixes:
-                    vendor, model = compat.split(',', 1)
-                    if vendor in self._vendor_prefixes:
-                        self.compat2vendor[compat] = self._vendor_prefixes[vendor]
-                        self.compat2model[compat] = model
+    These attributes are available on Register objects:
 
-                    # As an exception, the root node can have whatever
-                    # compatibles it wants. Other nodes get checked.
-                    elif node.path != '/' and \
-                       vendor not in _VENDOR_PREFIX_ALLOWED:
-                        if self._werror:
-                            handler_fn = _err
-                        else:
-                            handler_fn = _LOG.warning
-                        handler_fn(
-                            f"node '{node.path}' compatible '{compat}' "
-                            f"has unknown vendor prefix '{vendor}'")
+    node:
+      The Node instance this register is from
 
+    name:
+      The name of the register as given in the 'reg-names' property, or None if
+      there is no 'reg-names' property
 
-        for nodeset in self.scc_order:
-            node = nodeset[0]
-            self.dep_ord2node[node.dep_ordinal] = node
+    addr:
+      The starting address of the register, in the parent address space, or None
+      if #address-cells is zero. Any 'ranges' properties are taken into account.
 
-    def _check(self):
-        # Tree-wide checks and warnings.
+    size:
+      The length of the register in bytes
+    """
 
-        for binding in self._compat2binding.values():
-            for spec in binding.prop2specs.values():
-                if not spec.enum or spec.type != 'string':
-                    continue
+    node: 'Node'
+    name: Optional[str]
+    addr: Optional[int]
+    size: Optional[int]
 
-                if not spec.enum_tokenizable:
-                    _LOG.warning(
-                        f"compatible '{binding.compatible}' "
-                        f"in binding '{binding.path}' has non-tokenizable enum "
-                        f"for property '{spec.name}': " +
-                        ', '.join(repr(x) for x in spec.enum))
-                elif not spec.enum_upper_tokenizable:
-                    _LOG.warning(
-                        f"compatible '{binding.compatible}' "
-                        f"in binding '{binding.path}' has enum for property "
-                        f"'{spec.name}' that is only tokenizable "
-                        'in lowercase: ' +
-                        ', '.join(repr(x) for x in spec.enum))
 
-        # Validate the contents of compatible properties.
-        for node in self.nodes:
-            if 'compatible' not in node.props:
-                continue
+@dataclass
+class Range:
+    """
+    Represents a translation range on a node as described by the 'ranges' property.
 
-            compatibles = node.props['compatible'].val
+    These attributes are available on Range objects:
 
-            # _check() runs after _init_compat2binding() has called
-            # _dt_compats(), which already converted every compatible
-            # property to a list of strings. So we know 'compatibles'
-            # is a list, but add an assert for future-proofing.
-            assert isinstance(compatibles, list)
+    node:
+      The Node instance this range is from
 
-            for compat in compatibles:
-                # This is also just for future-proofing.
-                assert isinstance(compat, str)
+    child_bus_cells:
+      The number of cells used to describe a child bus address.
+
+    child_bus_addr:
+      A physical address within the child bus address space, or None if the
+      child's #address-cells equals 0.
+
+    parent_bus_cells:
+      The number of cells used to describe a parent bus address.
+
+    parent_bus_addr:
+      A physical address within the parent bus address space, or None if the
+      parent's #address-cells equals 0.
+
+    length_cells:
+      The number of cells used to describe the size of range in
+      the child's address space.
+
+    length:
+      The size of the range in the child address space, or None if the
+      child's #size-cells equals 0.
+    """
+    node: 'Node'
+    child_bus_cells: int
+    child_bus_addr: Optional[int]
+    parent_bus_cells: int
+    parent_bus_addr: Optional[int]
+    length_cells: int
+    length: Optional[int]
+
+
+@dataclass
+class ControllerAndData:
+    """
+    Represents an entry in an 'interrupts' or 'type: phandle-array' property
+    value, e.g. <&ctrl-1 4 0> in
+
+        cs-gpios = <&ctrl-1 4 0 &ctrl-2 3 4>;
+
+    These attributes are available on ControllerAndData objects:
+
+    node:
+      The Node instance the property appears on
+
+    controller:
+      The Node instance for the controller (e.g. the controller the interrupt
+      gets sent to for interrupts)
+
+    data:
+      A dictionary that maps names from the *-cells key in the binding for the
+      controller to data values, e.g. {"pin": 4, "flags": 0} for the example
+      above.
+
+      'interrupts = <1 2>' might give {"irq": 1, "level": 2}.
+
+    name:
+      The name of the entry as given in
+      'interrupt-names'/'gpio-names'/'pwm-names'/etc., or None if there is no
+      *-names property
+
+    basename:
+      Basename for the controller when supporting named cells
+    """
+    node: 'Node'
+    controller: 'Node'
+    data: dict
+    name: Optional[str]
+    basename: Optional[str]
+
+
+@dataclass
+class PinCtrl:
+    """
+    Represents a pin control configuration for a set of pins on a device,
+    e.g. pinctrl-0 or pinctrl-1.
+
+    These attributes are available on PinCtrl objects:
+
+    node:
+      The Node instance the pinctrl-* property is on
+
+    name:
+      The name of the configuration, as given in pinctrl-names, or None if
+      there is no pinctrl-names property
+
+    name_as_token:
+      Like 'name', but with non-alphanumeric characters converted to underscores.
+
+    conf_nodes:
+      A list of Node instances for the pin configuration nodes, e.g.
+      the nodes pointed at by &state_1 and &state_2 in
+
+          pinctrl-0 = <&state_1 &state_2>;
+    """
+
+    node: 'Node'
+    name: Optional[str]
+    conf_nodes: List['Node']
+
+    @property
+    def name_as_token(self):
+        "See the class docstring"
+        return str_as_token(self.name) if self.name is not None else None
 
 
 class Node:
     """
     Represents a devicetree node, augmented with information from bindings, and
     with some interpretation of devicetree properties. There's a one-to-one
     correspondence between devicetree nodes and Nodes.
@@ -619,15 +925,15 @@
       binding
 
     compats:
       A list of 'compatible' strings for the node, in the same order that
       they're listed in the .dts file
 
     ranges:
-      A list if Range objects extracted from the node's ranges property.
+      A list of Range objects extracted from the node's ranges property.
       The list is empty if the node does not have a range property.
 
     regs:
       A list of Register objects for the node's registers
 
     props:
       A dict that maps property names to Property objects.
@@ -673,21 +979,46 @@
       Documentation/devicetree/bindings/spi/spi-controller.yaml in the Linux kernel.
 
     gpio_hogs:
       A list of ControllerAndData objects for the GPIOs hogged by the node. The
       list is empty if the node does not hog any GPIOs. Only relevant for GPIO hog
       nodes.
     """
+
+    def __init__(self,
+                 dt_node: dtlib_Node,
+                 edt: 'EDT',
+                 compats: List[str]):
+        '''
+        For internal use only; not meant to be used outside edtlib itself.
+        '''
+        # Public, some of which are initialized properly later:
+        self.edt: 'EDT' = edt
+        self.dep_ordinal: int = -1
+        self.matching_compat: Optional[str] = None
+        self.binding_path: Optional[str] = None
+        self.compats: List[str] = compats
+        self.ranges: List[Range] = []
+        self.regs: List[Register] = []
+        self.props: Dict[str, Property] = {}
+        self.interrupts: List[ControllerAndData] = []
+        self.pinctrls: List[PinCtrl] = []
+        self.bus_node: Optional['Node'] = None
+
+        # Private, don't touch outside the class:
+        self._node: dtlib_Node = dt_node
+        self._binding: Optional[Binding] = None
+
     @property
-    def name(self):
+    def name(self) -> str:
         "See the class docstring"
         return self._node.name
 
     @property
-    def unit_addr(self):
+    def unit_addr(self) -> Optional[int]:
         "See the class docstring"
 
         # TODO: Return a plain string here later, like dtlib.Node.unit_addr?
 
         if "@" not in self.name:
             return None
 
@@ -695,159 +1026,171 @@
             addr = int(self.name.split("@", 1)[1], 16)
         except ValueError:
             _err(f"{self!r} has non-hex unit address")
 
         return _translate(addr, self._node)
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         "See the class docstring."
         if self._binding:
             return self._binding.description
         return None
 
     @property
-    def path(self):
+    def path(self) ->  str:
         "See the class docstring"
         return self._node.path
 
     @property
-    def label(self):
+    def label(self) -> Optional[str]:
         "See the class docstring"
         if "label" in self._node.props:
             return self._node.props["label"].to_string()
         return None
 
     @property
-    def labels(self):
+    def labels(self) -> List[str]:
         "See the class docstring"
         return self._node.labels
 
     @property
-    def parent(self):
+    def parent(self) -> Optional['Node']:
         "See the class docstring"
-        return self.edt._node2enode.get(self._node.parent)
+        return self.edt._node2enode.get(self._node.parent) # type: ignore
 
     @property
-    def children(self):
+    def children(self) -> Dict[str, 'Node']:
         "See the class docstring"
         # Could be initialized statically too to preserve identity, but not
         # sure if needed. Parent nodes being initialized before their children
         # would need to be kept in mind.
         return {name: self.edt._node2enode[node]
                 for name, node in self._node.nodes.items()}
 
-    def child_index(self, node):
+    def child_index(self, node) -> int:
         """Get the index of *node* in self.children.
         Raises KeyError if the argument is not a child of this node.
         """
         if not hasattr(self, '_child2index'):
             # Defer initialization of this lookup table until this
             # method is callable to handle parents needing to be
             # initialized before their chidlren. By the time we
             # return from __init__, 'self.children' is callable.
-            self._child2index = {}
-            for index, child in enumerate(self.children.values()):
-                self._child2index[child] = index
+            self._child2index: Dict[str, int] = {}
+            for index, child_path in enumerate(child.path for child in
+                                               self.children.values()):
+                self._child2index[child_path] = index
 
-        return self._child2index[node]
+        return self._child2index[node.path]
 
     @property
-    def required_by(self):
+    def required_by(self) -> List['Node']:
         "See the class docstring"
         return self.edt._graph.required_by(self)
 
     @property
-    def depends_on(self):
+    def depends_on(self) -> List['Node']:
         "See the class docstring"
         return self.edt._graph.depends_on(self)
 
     @property
-    def status(self):
+    def status(self) -> str:
         "See the class docstring"
         status = self._node.props.get("status")
 
         if status is None:
             as_string = "okay"
         else:
             as_string = status.to_string()
 
         if as_string == "ok":
             as_string = "okay"
 
         return as_string
 
     @property
-    def read_only(self):
+    def read_only(self) -> bool:
         "See the class docstring"
         return "read-only" in self._node.props
 
     @property
-    def aliases(self):
+    def aliases(self) -> List[str]:
         "See the class docstring"
         return [alias for alias, node in self._node.dt.alias2node.items()
                 if node is self._node]
 
     @property
-    def buses(self):
+    def buses(self) -> List[str]:
         "See the class docstring"
         if self._binding:
             return self._binding.buses
         return []
 
     @property
-    def on_buses(self):
+    def on_buses(self) -> List[str]:
         "See the class docstring"
         bus_node = self.bus_node
         return bus_node.buses if bus_node else []
 
     @property
-    def flash_controller(self):
+    def flash_controller(self) -> 'Node':
         "See the class docstring"
 
         # The node path might be something like
         # /flash-controller@4001E000/flash@0/partitions/partition@fc000. We go
         # up two levels to get the flash and check its compat. The flash
         # controller might be the flash itself (for cases like NOR flashes).
         # For the case of 'soc-nv-flash', we assume the controller is the
         # parent of the flash node.
 
         if not self.parent or not self.parent.parent:
             _err(f"flash partition {self!r} lacks parent or grandparent node")
 
         controller = self.parent.parent
         if controller.matching_compat == "soc-nv-flash":
+            if controller.parent is None:
+                _err(f"flash controller '{controller.path}' cannot be the root node")
             return controller.parent
         return controller
 
     @property
-    def spi_cs_gpio(self):
+    def spi_cs_gpio(self) -> Optional[ControllerAndData]:
         "See the class docstring"
 
         if not ("spi" in self.on_buses
+                and self.bus_node
                 and "cs-gpios" in self.bus_node.props):
             return None
 
         if not self.regs:
             _err(f"{self!r} needs a 'reg' property, to look up the "
                  "chip select index for SPI")
 
         parent_cs_lst = self.bus_node.props["cs-gpios"].val
+        if TYPE_CHECKING:
+            assert isinstance(parent_cs_lst, list)
 
         # cs-gpios is indexed by the unit address
         cs_index = self.regs[0].addr
+        if TYPE_CHECKING:
+            assert isinstance(cs_index, int)
+
         if cs_index >= len(parent_cs_lst):
             _err(f"index from 'regs' in {self!r} ({cs_index}) "
                  "is >= number of cs-gpios in "
                  f"{self.bus_node!r} ({len(parent_cs_lst)})")
 
-        return parent_cs_lst[cs_index]
+        ret = parent_cs_lst[cs_index]
+        if TYPE_CHECKING:
+            assert isinstance(ret, ControllerAndData)
+        return ret
 
     @property
-    def gpio_hogs(self):
+    def gpio_hogs(self) -> List[ControllerAndData]:
         "See the class docstring"
 
         if "gpio-hog" not in self.props:
             return []
 
         if not self.parent or not "gpio-controller" in self.parent.props:
             _err(f"GPIO hog {self!r} lacks parent GPIO controller node")
@@ -856,33 +1199,30 @@
             _err(f"GPIO hog {self!r} parent node lacks #gpio-cells")
 
         n_cells = self.parent._node.props["#gpio-cells"].to_num()
         res = []
 
         for item in _slice(self._node, "gpios", 4*n_cells,
                            f"4*(<#gpio-cells> (= {n_cells})"):
-            entry = ControllerAndData()
-            entry.node = self
-            entry.controller = self.parent
-            entry.data = self._named_cells(entry.controller, item, "gpio")
-            entry.basename = "gpio"
-            entry.name = None
-
-            res.append(entry)
+            controller = self.parent
+            res.append(ControllerAndData(
+                node=self, controller=controller,
+                data=self._named_cells(controller, item, "gpio"),
+                name=None, basename="gpio"))
 
         return res
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self.binding_path:
             binding = "binding " + self.binding_path
         else:
             binding = "no binding"
         return f"<Node {self.path} in '{self.edt.dts_path}', {binding}>"
 
-    def _init_binding(self):
+    def _init_binding(self) -> None:
         # Initializes Node.matching_compat, Node._binding, and
         # Node.binding_path.
         #
         # Node._binding holds the data from the node's binding file, in the
         # format returned by PyYAML (plain Python lists, dicts, etc.), or None
         # if the node has no binding.
 
@@ -932,27 +1272,27 @@
                 self.matching_compat = self._binding.compatible
 
                 return
 
         # No binding found
         self._binding = self.binding_path = self.matching_compat = None
 
-    def _binding_from_properties(self):
+    def _binding_from_properties(self) -> None:
         # Sets up a Binding object synthesized from the properties in the node.
 
         if self.compats:
             _err(f"compatible in node with inferred binding: {self.path}")
 
         # Synthesize a 'raw' binding as if it had been parsed from YAML.
-        raw = {
+        raw: Dict[str, Any] = {
             'description': 'Inferred binding from properties, via edtlib.',
             'properties': {},
         }
         for name, prop in self._node.props.items():
-            pp = {}
+            pp: Dict[str, str] = {}
             if prop.type == Type.EMPTY:
                 pp["type"] = "boolean"
             elif prop.type == Type.BYTES:
                 pp["type"] = "uint8-array"
             elif prop.type == Type.NUM:
                 pp["type"] = "int"
             elif prop.type == Type.NUMS:
@@ -976,15 +1316,15 @@
 
         # Set up Node state.
         self.binding_path = None
         self.matching_compat = None
         self.compats = []
         self._binding = Binding(None, {}, raw=raw, require_compatible=False)
 
-    def _binding_from_parent(self):
+    def _binding_from_parent(self) -> Optional[Binding]:
         # Returns the binding from 'child-binding:' in the parent node's
         # binding.
 
         if not self.parent:
             return None
 
         pbinding = self.parent._binding
@@ -992,15 +1332,16 @@
             return None
 
         if pbinding.child_binding:
             return pbinding.child_binding
 
         return None
 
-    def _bus_node(self, support_fixed_partitions_on_any_bus = True):
+    def _bus_node(self, support_fixed_partitions_on_any_bus: bool = True
+                  ) -> Optional['Node']:
         # Returns the value for self.bus_node. Relies on parent nodes being
         # initialized before their children.
 
         if not self.parent:
             # This is the root node
             return None
 
@@ -1015,15 +1356,16 @@
         if self.parent.buses:
             # The parent node is a bus node
             return self.parent
 
         # Same bus node as parent (possibly None)
         return self.parent.bus_node
 
-    def _init_props(self, default_prop_types=False, err_on_deprecated=False):
+    def _init_props(self, default_prop_types: bool = False,
+                    err_on_deprecated: bool = False) -> None:
         # Creates self.props. See the class docstring. Also checks that all
         # properties on the node are declared in its binding.
 
         self.props = {}
 
         node = self._node
         if self._binding:
@@ -1041,15 +1383,16 @@
                 if name not in _DEFAULT_PROP_SPECS:
                     continue
                 prop_spec = _DEFAULT_PROP_SPECS[name]
                 val = self._prop_val(name, prop_spec.type, False, False, None,
                                      None, err_on_deprecated)
                 self.props[name] = Property(prop_spec, val, self)
 
-    def _init_prop(self, prop_spec, err_on_deprecated):
+    def _init_prop(self, prop_spec: PropertySpec,
+                   err_on_deprecated: bool) -> None:
         # _init_props() helper for initializing a single property.
         # 'prop_spec' is a PropertySpec object from the node's binding.
 
         name = prop_spec.name
         prop_type = prop_spec.type
         if not prop_type:
             _err(f"'{name}' in {self.binding_path} lacks 'type'")
@@ -1079,16 +1422,19 @@
         # Skip properties that start with '#', like '#size-cells', and mapping
         # properties like 'gpio-map'/'interrupt-map'
         if name[0] == "#" or name.endswith("-map"):
             return
 
         self.props[name] = Property(prop_spec, val, self)
 
-    def _prop_val(self, name, prop_type, deprecated, required, default,
-                  specifier_space, err_on_deprecated):
+    def _prop_val(self, name: str, prop_type: str,
+                  deprecated: bool, required: bool,
+                  default: PropertyValType,
+                  specifier_space: Optional[str],
+                  err_on_deprecated: bool) -> PropertyValType:
         # _init_prop() helper for getting the property's value
         #
         # name:
         #   Property name from binding
         #
         # prop_type:
         #   Property type from binding (a string like "int")
@@ -1127,15 +1473,15 @@
 
             if default is not None:
                 # YAML doesn't have a native format for byte arrays. We need to
                 # convert those from an array like [0x12, 0x34, ...]. The
                 # format has already been checked in
                 # _check_prop_by_type().
                 if prop_type == "uint8-array":
-                    return bytes(default)
+                    return bytes(default) # type: ignore
                 return default
 
             return False if prop_type == "boolean" else None
 
         if prop_type == "boolean":
             if prop.type != Type.EMPTY:
                 _err("'{0}' in {1!r} is defined with 'type: boolean' in {2}, "
@@ -1183,52 +1529,55 @@
         # value is valid is done in _check_prop_by_type().
         #
         # 'compound' is a dummy type for properties that don't fit any of the
         # patterns above, so that we can require all entries in 'properties:'
         # to have a 'type: ...'. No Property object is created for it.
         return None
 
-    def _check_undeclared_props(self):
+    def _check_undeclared_props(self) -> None:
         # Checks that all properties are declared in the binding
 
         for prop_name in self._node.props:
             # Allow a few special properties to not be declared in the binding
             if prop_name.endswith("-controller") or \
                prop_name.startswith("#") or \
                prop_name.startswith("pinctrl-") or \
                prop_name in {
                    "compatible", "status", "ranges", "phandle",
                    "interrupt-parent", "interrupts-extended", "device_type"}:
                 continue
 
+            if TYPE_CHECKING:
+                assert self._binding
+
             if prop_name not in self._binding.prop2specs:
                 _err(f"'{prop_name}' appears in {self._node.path} in "
                      f"{self.edt.dts_path}, but is not declared in "
                      f"'properties:' in {self.binding_path}")
 
-    def _init_ranges(self):
+    def _init_ranges(self) -> None:
         # Initializes self.ranges
         node = self._node
 
         self.ranges = []
 
         if "ranges" not in node.props:
             return
 
-        child_address_cells = node.props.get("#address-cells")
+        raw_child_address_cells = node.props.get("#address-cells")
         parent_address_cells = _address_cells(node)
-        if child_address_cells is None:
+        if raw_child_address_cells is None:
             child_address_cells = 2 # Default value per DT spec.
         else:
-            child_address_cells = child_address_cells.to_num()
-        child_size_cells = node.props.get("#size-cells")
-        if child_size_cells is None:
+            child_address_cells = raw_child_address_cells.to_num()
+        raw_child_size_cells = node.props.get("#size-cells")
+        if raw_child_size_cells is None:
             child_size_cells = 1 # Default value per DT spec.
         else:
-            child_size_cells = child_size_cells.to_num()
+            child_size_cells = raw_child_size_cells.to_num()
 
         # Number of cells for one translation 3-tuple in 'ranges'
         entry_cells = child_address_cells + parent_address_cells + child_size_cells
 
         if entry_cells == 0:
             if len(node.props["ranges"].value) == 0:
                 return
@@ -1240,37 +1589,38 @@
 
         for raw_range in _slice(node, "ranges", 4*entry_cells,
                                 f"4*(<#address-cells> (= {child_address_cells}) + "
                                 "<#address-cells for parent> "
                                 f"(= {parent_address_cells}) + "
                                 f"<#size-cells> (= {child_size_cells}))"):
 
-            range = Range()
-            range.node = self
-            range.child_bus_cells = child_address_cells
+            child_bus_cells = child_address_cells
             if child_address_cells == 0:
-                range.child_bus_addr = None
+                child_bus_addr = None
             else:
-                range.child_bus_addr = to_num(raw_range[:4*child_address_cells])
-            range.parent_bus_cells = parent_address_cells
+                child_bus_addr = to_num(raw_range[:4*child_address_cells])
+            parent_bus_cells = parent_address_cells
             if parent_address_cells == 0:
-                range.parent_bus_addr = None
+                parent_bus_addr = None
             else:
-                range.parent_bus_addr = to_num(raw_range[(4*child_address_cells):\
-                                            (4*child_address_cells + 4*parent_address_cells)])
-            range.length_cells = child_size_cells
+                parent_bus_addr = to_num(
+                    raw_range[(4*child_address_cells):
+                              (4*child_address_cells + 4*parent_address_cells)])
+            length_cells = child_size_cells
             if child_size_cells == 0:
-                range.length = None
+                length = None
             else:
-                range.length = to_num(raw_range[(4*child_address_cells + \
-                                                    4*parent_address_cells):])
+                length = to_num(
+                    raw_range[(4*child_address_cells + 4*parent_address_cells):])
 
-            self.ranges.append(range)
+            self.ranges.append(Range(self, child_bus_cells, child_bus_addr,
+                                     parent_bus_cells, parent_bus_addr,
+                                     length_cells, length))
 
-    def _init_regs(self):
+    def _init_regs(self) -> None:
         # Initializes self.regs
 
         node = self._node
 
         self.regs = []
 
         if "reg" not in node.props:
@@ -1278,34 +1628,33 @@
 
         address_cells = _address_cells(node)
         size_cells = _size_cells(node)
 
         for raw_reg in _slice(node, "reg", 4*(address_cells + size_cells),
                               f"4*(<#address-cells> (= {address_cells}) + "
                               f"<#size-cells> (= {size_cells}))"):
-            reg = Register()
-            reg.node = self
             if address_cells == 0:
-                reg.addr = None
+                addr = None
             else:
-                reg.addr = _translate(to_num(raw_reg[:4*address_cells]), node)
+                addr = _translate(to_num(raw_reg[:4*address_cells]), node)
             if size_cells == 0:
-                reg.size = None
+                size = None
             else:
-                reg.size = to_num(raw_reg[4*address_cells:])
-            if size_cells != 0 and reg.size == 0:
+                size = to_num(raw_reg[4*address_cells:])
+            if size_cells != 0 and size == 0:
                 _err(f"zero-sized 'reg' in {self._node!r} seems meaningless "
                      "(maybe you want a size of one or #size-cells = 0 "
                      "instead)")
 
-            self.regs.append(reg)
+            # We'll fix up the name when we're done.
+            self.regs.append(Register(self, None, addr, size))
 
         _add_names(node, "reg", self.regs)
 
-    def _init_pinctrls(self):
+    def _init_pinctrls(self) -> None:
         # Initializes self.pinctrls from any pinctrl-<index> properties
 
         node = self._node
 
         # pinctrl-<index> properties
         pinctrl_props = [prop for name, prop in node.props.items()
                          if re.match("pinctrl-[0-9]+", name)]
@@ -1316,42 +1665,45 @@
         for i, prop in enumerate(pinctrl_props):
             if prop.name != "pinctrl-" + str(i):
                 _err(f"missing 'pinctrl-{i}' property on {node!r} "
                      "- indices should be contiguous and start from zero")
 
         self.pinctrls = []
         for prop in pinctrl_props:
-            pinctrl = PinCtrl()
-            pinctrl.node = self
-            pinctrl.conf_nodes = [
-                self.edt._node2enode[node] for node in prop.to_nodes()
-            ]
-            self.pinctrls.append(pinctrl)
+            # We'll fix up the names below.
+            self.pinctrls.append(PinCtrl(
+                node=self,
+                name=None,
+                conf_nodes=[self.edt._node2enode[node]
+                            for node in prop.to_nodes()]))
 
         _add_names(node, "pinctrl", self.pinctrls)
 
-    def _init_interrupts(self):
+    def _init_interrupts(self) -> None:
         # Initializes self.interrupts
 
         node = self._node
 
         self.interrupts = []
 
         for controller_node, data in _interrupts(node):
-            interrupt = ControllerAndData()
-            interrupt.node = self
-            interrupt.controller = self.edt._node2enode[controller_node]
-            interrupt.data = self._named_cells(interrupt.controller, data,
-                                               "interrupt")
-
-            self.interrupts.append(interrupt)
+            # We'll fix up the names below.
+            controller = self.edt._node2enode[controller_node]
+            self.interrupts.append(ControllerAndData(
+                node=self, controller=controller,
+                data=self._named_cells(controller, data, "interrupt"),
+                name=None, basename=None))
 
         _add_names(node, "interrupt", self.interrupts)
 
-    def _standard_phandle_val_list(self, prop, specifier_space):
+    def _standard_phandle_val_list(
+            self,
+            prop: dtlib_Property,
+            specifier_space: Optional[str]
+    ) -> List[Optional[ControllerAndData]]:
         # Parses a property like
         #
         #     <prop.name> = <phandle cell phandle cell ...>;
         #
         # where each phandle points to a controller node that has a
         #
         #     #<specifier_space>-cells = <size>;
@@ -1393,50 +1745,54 @@
                 # #foo-gpio-cells
                 specifier_space = "gpio"
             else:
                 # Strip -s. We've already checked that property names end in -s
                 # if there is no specifier space in _check_prop_by_type().
                 specifier_space = prop.name[:-1]
 
-        res = []
+        res: List[Optional[ControllerAndData]] = []
 
         for item in _phandle_val_list(prop, specifier_space):
             if item is None:
                 res.append(None)
                 continue
 
             controller_node, data = item
             mapped_controller, mapped_data = \
                 _map_phandle_array_entry(prop.node, controller_node, data,
                                          specifier_space)
 
-            entry = ControllerAndData()
-            entry.node = self
-            entry.controller = self.edt._node2enode[mapped_controller]
-            entry.basename = specifier_space
-            entry.data = self._named_cells(entry.controller, mapped_data,
-                                           specifier_space)
-
-            res.append(entry)
+            controller = self.edt._node2enode[mapped_controller]
+            # We'll fix up the names below.
+            res.append(ControllerAndData(
+                node=self, controller=controller,
+                data=self._named_cells(controller, mapped_data,
+                                       specifier_space),
+                name=None, basename=specifier_space))
 
         _add_names(self._node, specifier_space, res)
 
         return res
 
-    def _named_cells(self, controller, data, basename):
+    def _named_cells(
+            self,
+            controller: 'Node',
+            data: bytes,
+            basename: str
+    ) -> Dict[str, int]:
         # Returns a dictionary that maps <basename>-cells names given in the
         # binding for 'controller' to cell values. 'data' is the raw data, as a
         # byte array.
 
         if not controller._binding:
             _err(f"{basename} controller {controller._node!r} "
                  f"for {self._node!r} lacks binding")
 
         if basename in controller._binding.specifier2cells:
-            cell_names = controller._binding.specifier2cells[basename]
+            cell_names: List[str] = controller._binding.specifier2cells[basename]
         else:
             # Treat no *-cells in the binding the same as an empty *-cells, so
             # that bindings don't have to have e.g. an empty 'clock-cells:' for
             # '#clock-cells = <0>'.
             cell_names = []
 
         data_list = to_nums(data)
@@ -1444,649 +1800,514 @@
             _err(f"unexpected '{basename}-cells:' length in binding for "
                  f"{controller._node!r} - {len(cell_names)} "
                  f"instead of {len(data_list)}")
 
         return dict(zip(cell_names, data_list))
 
 
-class Range:
-    """
-    Represents a translation range on a node as described by the 'ranges' property.
-
-    These attributes are available on Range objects:
-
-    node:
-      The Node instance this range is from
-
-    child_bus_cells:
-      Is the number of cells (4-bytes wide words) describing the child bus address.
-
-    child_bus_addr:
-      Is a physical address within the child bus address space, or None if the
-      child address-cells is equal 0.
-
-    parent_bus_cells:
-      Is the number of cells (4-bytes wide words) describing the parent bus address.
-
-    parent_bus_addr:
-      Is a physical address within the parent bus address space, or None if the
-      parent address-cells is equal 0.
-
-    length_cells:
-      Is the number of cells (4-bytes wide words) describing the size of range in
-      the child address space.
-
-    length:
-      Specifies the size of the range in the child address space, or None if the
-      child size-cells is equal 0.
-    """
-    def __repr__(self):
-        fields = []
-
-        if self.child_bus_cells is not None:
-            fields.append("child-bus-cells: " + hex(self.child_bus_cells))
-        if self.child_bus_addr is not None:
-            fields.append("child-bus-addr: " + hex(self.child_bus_addr))
-        if self.parent_bus_cells is not None:
-            fields.append("parent-bus-cells: " + hex(self.parent_bus_cells))
-        if self.parent_bus_addr is not None:
-            fields.append("parent-bus-addr: " + hex(self.parent_bus_addr))
-        if self.length_cells is not None:
-            fields.append("length-cells " + hex(self.length_cells))
-        if self.length is not None:
-            fields.append("length " + hex(self.length))
-
-        return "<Range, {}>".format(", ".join(fields))
-
-class Register:
-    """
-    Represents a register on a node.
-
-    These attributes are available on Register objects:
-
-    node:
-      The Node instance this register is from
-
-    name:
-      The name of the register as given in the 'reg-names' property, or None if
-      there is no 'reg-names' property
-
-    addr:
-      The starting address of the register, in the parent address space, or None
-      if #address-cells is zero. Any 'ranges' properties are taken into account.
-
-    size:
-      The length of the register in bytes
-    """
-    def __repr__(self):
-        fields = []
-
-        if self.name is not None:
-            fields.append("name: " + self.name)
-        if self.addr is not None:
-            fields.append("addr: " + hex(self.addr))
-        if self.size is not None:
-            fields.append("size: " + hex(self.size))
-
-        return "<Register, {}>".format(", ".join(fields))
-
-
-class ControllerAndData:
-    """
-    Represents an entry in an 'interrupts' or 'type: phandle-array' property
-    value, e.g. <&ctrl-1 4 0> in
-
-        cs-gpios = <&ctrl-1 4 0 &ctrl-2 3 4>;
-
-    These attributes are available on ControllerAndData objects:
-
-    node:
-      The Node instance the property appears on
-
-    controller:
-      The Node instance for the controller (e.g. the controller the interrupt
-      gets sent to for interrupts)
-
-    data:
-      A dictionary that maps names from the *-cells key in the binding for the
-      controller to data values, e.g. {"pin": 4, "flags": 0} for the example
-      above.
-
-      'interrupts = <1 2>' might give {"irq": 1, "level": 2}.
-
-    name:
-      The name of the entry as given in
-      'interrupt-names'/'gpio-names'/'pwm-names'/etc., or None if there is no
-      *-names property
-
-    basename:
-      Basename for the controller when supporting named cells
+class EDT:
     """
-    def __repr__(self):
-        fields = []
-
-        if self.name is not None:
-            fields.append("name: " + self.name)
-
-        fields.append(f"controller: {self.controller}")
-        fields.append(f"data: {self.data}")
-
-        return "<ControllerAndData, {}>".format(", ".join(fields))
+    Represents a devicetree augmented with information from bindings.
 
+    These attributes are available on EDT objects:
 
-class PinCtrl:
-    """
-    Represents a pin control configuration for a set of pins on a device,
-    e.g. pinctrl-0 or pinctrl-1.
+    nodes:
+      A list of Node objects for the nodes that appear in the devicetree
 
-    These attributes are available on PinCtrl objects:
+    compat2nodes:
+      A collections.defaultdict that maps each 'compatible' string that appears
+      on some Node to a list of Nodes with that compatible.
 
-    node:
-      The Node instance the pinctrl-* property is on
+    compat2okay:
+      Like compat2nodes, but just for nodes with status 'okay'.
 
-    name:
-      The name of the configuration, as given in pinctrl-names, or None if
-      there is no pinctrl-names property
+    compat2vendor:
+      A collections.defaultdict that maps each 'compatible' string that appears
+      on some Node to a vendor name parsed from vendor_prefixes.
 
-    name_as_token:
-      Like 'name', but with non-alphanumeric characters converted to underscores.
+    compat2model:
+      A collections.defaultdict that maps each 'compatible' string that appears
+      on some Node to a model name parsed from that compatible.
 
-    conf_nodes:
-      A list of Node instances for the pin configuration nodes, e.g.
-      the nodes pointed at by &state_1 and &state_2 in
+    label2node:
+      A dict that maps a node label to the node with that label.
 
-          pinctrl-0 = <&state_1 &state_2>;
-    """
+    dep_ord2node:
+      A dict that maps an ordinal to the node with that dependency ordinal.
 
-    @property
-    def name_as_token(self):
-        "See the class docstring"
-        return str_as_token(self.name) if self.name is not None else None
+    chosen_nodes:
+      A dict that maps the properties defined on the devicetree's /chosen
+      node to their values. 'chosen' is indexed by property name (a string),
+      and values are converted to Node objects. Note that properties of the
+      /chosen node which can't be converted to a Node are not included in
+      the value.
 
-    def __repr__(self):
-        fields = []
+    dts_path:
+      The .dts path passed to __init__()
 
-        if self.name is not None:
-            fields.append("name: " + self.name)
+    dts_source:
+      The final DTS source code of the loaded devicetree after merging nodes
+      and processing /delete-node/ and /delete-property/, as a string
 
-        fields.append("configuration nodes: " + str(self.conf_nodes))
+    bindings_dirs:
+      The bindings directory paths passed to __init__()
 
-        return "<PinCtrl, {}>".format(", ".join(fields))
+    scc_order:
+      A list of lists of Nodes. All elements of each list
+      depend on each other, and the Nodes in any list do not depend
+      on any Node in a subsequent list. Each list defines a Strongly
+      Connected Component (SCC) of the graph.
 
+      For an acyclic graph each list will be a singleton. Cycles
+      will be represented by lists with multiple nodes. Cycles are
+      not expected to be present in devicetree graphs.
 
-class Property:
+    The standard library's pickle module can be used to marshal and
+    unmarshal EDT objects.
     """
-    Represents a property on a Node, as set in its DT node and with
-    additional info from the 'properties:' section of the binding.
-
-    Only properties mentioned in 'properties:' get created. Properties of type
-    'compound' currently do not get Property instances, as it's not clear
-    what to generate for them.
-
-    These attributes are available on Property objects. Several are
-    just convenience accessors for attributes on the PropertySpec object
-    accessible via the 'spec' attribute.
-
-    These attributes are available on Property objects:
-
-    node:
-      The Node instance the property is on
-
-    spec:
-      The PropertySpec object which specifies this property.
 
-    name:
-      Convenience for spec.name.
-
-    description:
-      Convenience for spec.description with leading and trailing whitespace
-      (including newlines) removed. May be None.
+    def __init__(self,
+                 dts: Optional[str],
+                 bindings_dirs: List[str],
+                 warn_reg_unit_address_mismatch: bool = True,
+                 default_prop_types: bool = True,
+                 support_fixed_partitions_on_any_bus: bool = True,
+                 infer_binding_for_paths: Optional[Iterable[str]] = None,
+                 vendor_prefixes: Optional[Dict[str, str]] = None,
+                 werror: bool = False):
+        """EDT constructor.
 
-    type:
-      Convenience for spec.type.
+        dts:
+          Path to devicetree .dts file. Passing None for this value
+          is only for internal use; do not do that outside of edtlib.
 
-    val:
-      The value of the property, with the format determined by spec.type,
-      which comes from the 'type:' string in the binding.
+        bindings_dirs:
+          List of paths to directories containing bindings, in YAML format.
+          These directories are recursively searched for .yaml files.
 
-        - For 'type: int/array/string/string-array', 'val' is what you'd expect
-          (a Python integer or string, or a list of them)
+        warn_reg_unit_address_mismatch (default: True):
+          If True, a warning is logged if a node has a 'reg' property where
+          the address of the first entry does not match the unit address of the
+          node
 
-        - For 'type: phandle' and 'type: path', 'val' is the pointed-to Node
-          instance
+        default_prop_types (default: True):
+          If True, default property types will be used when a node has no
+          bindings.
 
-        - For 'type: phandles', 'val' is a list of the pointed-to Node
-          instances
+        support_fixed_partitions_on_any_bus (default True):
+          If True, set the Node.bus for 'fixed-partitions' compatible nodes
+          to None.  This allows 'fixed-partitions' binding to match regardless
+          of the bus the 'fixed-partition' is under.
 
-        - For 'type: phandle-array', 'val' is a list of ControllerAndData
-          instances. See the documentation for that class.
+        infer_binding_for_paths (default: None):
+          An iterable of devicetree paths identifying nodes for which bindings
+          should be inferred from the node content.  (Child nodes are not
+          processed.)  Pass none if no nodes should support inferred bindings.
 
-    val_as_token:
-      The value of the property as a token, i.e. with non-alphanumeric
-      characters replaced with underscores. This is only safe to access
-      if self.enum_tokenizable returns True.
+        vendor_prefixes (default: None):
+          A dict mapping vendor prefixes in compatible properties to their
+          descriptions. If given, compatibles in the form "manufacturer,device"
+          for which "manufacturer" is neither a key in the dict nor a specially
+          exempt set of grandfathered-in cases will cause warnings.
 
-    enum_index:
-      The index of 'val' in 'spec.enum' (which comes from the 'enum:' list
-      in the binding), or None if spec.enum is None.
-    """
+        werror (default: False):
+          If True, some edtlib specific warnings become errors. This currently
+          errors out if 'dts' has any deprecated properties set, or an unknown
+          vendor prefix is used.
+        """
+        # All instance attributes should be initialized here.
+        # This makes it easy to keep track of them, which makes
+        # implementing __deepcopy__() easier.
+        # If you change this, make sure to update __deepcopy__() too,
+        # and update the tests for that method.
+
+        # Public attributes (the rest are properties)
+        self.nodes: List[Node] = []
+        self.compat2nodes: Dict[str, List[Node]] = defaultdict(list)
+        self.compat2okay: Dict[str, List[Node]] = defaultdict(list)
+        self.compat2vendor: Dict[str, str] = defaultdict(str)
+        self.compat2model: Dict[str, str]  = defaultdict(str)
+        self.label2node: Dict[str, Node] = {}
+        self.dep_ord2node: Dict[int, Node] = {}
+        self.dts_path: str = dts # type: ignore
+        self.bindings_dirs: List[str] = list(bindings_dirs)
+
+        # Saved kwarg values for internal use
+        self._warn_reg_unit_address_mismatch: bool = warn_reg_unit_address_mismatch
+        self._default_prop_types: bool = default_prop_types
+        self._fixed_partitions_no_bus: bool = support_fixed_partitions_on_any_bus
+        self._infer_binding_for_paths: Set[str] = set(infer_binding_for_paths or [])
+        self._vendor_prefixes: Dict[str, str] = vendor_prefixes or {}
+        self._werror: bool = bool(werror)
+
+        # Other internal state
+        self._compat2binding: Dict[Tuple[str, Optional[str]], Binding] = {}
+        self._graph: Graph = Graph()
+        self._binding_paths: List[str] = _binding_paths(self.bindings_dirs)
+        self._binding_fname2path: Dict[str, str] = {
+            os.path.basename(path): path
+            for path in self._binding_paths
+        }
+        self._node2enode: Dict[dtlib_Node, Node] = {}
 
-    def __init__(self, spec, val, node):
-        self.val = val
-        self.spec = spec
-        self.node = node
+        if dts is not None:
+            try:
+                self._dt = DT(dts)
+            except DTError as e:
+                raise EDTError(e) from e
+            self._finish_init()
 
-    @property
-    def name(self):
-        "See the class docstring"
-        return self.spec.name
+    def _finish_init(self) -> None:
+        # This helper exists to make the __deepcopy__() implementation
+        # easier to keep in sync with __init__().
+        _check_dt(self._dt)
 
-    @property
-    def description(self):
-        "See the class docstring"
-        return self.spec.description.strip() if self.spec.description else None
+        self._init_compat2binding()
+        self._init_nodes()
+        self._init_graph()
+        self._init_luts()
 
-    @property
-    def type(self):
-        "See the class docstring"
-        return self.spec.type
+        self._check()
 
-    @property
-    def val_as_token(self):
-        "See the class docstring"
-        return str_as_token(self.val)
+    def get_node(self, path: str) -> Node:
+        """
+        Returns the Node at the DT path or alias 'path'. Raises EDTError if the
+        path or alias doesn't exist.
+        """
+        try:
+            return self._node2enode[self._dt.get_node(path)]
+        except DTError as e:
+            _err(e)
 
     @property
-    def enum_index(self):
-        "See the class docstring"
-        enum = self.spec.enum
-        return enum.index(self.val) if enum else None
-
-    def __repr__(self):
-        fields = ["name: " + self.name,
-                  # repr() to deal with lists
-                  "type: " + self.type,
-                  "value: " + repr(self.val)]
-
-        if self.enum_index is not None:
-            fields.append(f"enum index: {self.enum_index}")
-
-        return "<Property, {}>".format(", ".join(fields))
-
-
-class Binding:
-    """
-    Represents a parsed binding.
-
-    These attributes are available on Binding objects:
-
-    path:
-      The absolute path to the file defining the binding.
-
-    description:
-      The free-form description of the binding, or None.
-
-    compatible:
-      The compatible string the binding matches.
-
-      This may be None. For example, it's None when the Binding is inferred
-      from node properties. It can also be None for Binding objects created
-      using 'child-binding:' with no compatible.
-
-    prop2specs:
-      A dict mapping property names to PropertySpec objects
-      describing those properties' values.
-
-    specifier2cells:
-      A dict that maps specifier space names (like "gpio",
-      "clock", "pwm", etc.) to lists of cell names.
-
-      For example, if the binding YAML contains 'pin' and 'flags' cell names
-      for the 'gpio' specifier space, like this:
-
-          gpio-cells:
-          - pin
-          - flags
-
-      Then the Binding object will have a 'specifier2cells' attribute mapping
-      "gpio" to ["pin", "flags"]. A missing key should be interpreted as zero
-      cells.
-
-    raw:
-      The binding as an object parsed from YAML.
+    def chosen_nodes(self) -> Dict[str, Node]:
+        ret: Dict[str, Node] = {}
 
-    bus:
-      If nodes with this binding's 'compatible' describe a bus, a string
-      describing the bus type (like "i2c") or a list describing supported
-      protocols (like ["i3c", "i2c"]). None otherwise.
-
-      Note that this is the raw value from the binding where it can be
-      a string or a list. Use "buses" instead unless you need the raw
-      value, where "buses" is always a list.
+        try:
+            chosen = self._dt.get_node("/chosen")
+        except DTError:
+            return ret
 
-    buses:
-      Deprived property from 'bus' where 'buses' is a list of bus(es),
-      for example, ["i2c"] or ["i3c", "i2c"]. Or an empty list if there is
-      no 'bus:' in this binding.
+        for name, prop in chosen.props.items():
+            try:
+                node = prop.to_path()
+            except DTError:
+                # DTS value is not phandle or string, or path doesn't exist
+                continue
 
-    on_bus:
-      If nodes with this binding's 'compatible' appear on a bus, a string
-      describing the bus type (like "i2c"). None otherwise.
+            ret[name] = self._node2enode[node]
 
-    child_binding:
-      If this binding describes the properties of child nodes, then
-      this is a Binding object for those children; it is None otherwise.
-      A Binding object's 'child_binding.child_binding' is not None if there
-      are multiple levels of 'child-binding' descriptions in the binding.
-    """
+        return ret
 
-    def __init__(self, path, fname2path, raw=None,
-                 require_compatible=True, require_description=True):
+    def chosen_node(self, name: str) -> Optional[Node]:
         """
-        Binding constructor.
-
-        path:
-          Path to binding YAML file. May be None.
-
-        fname2path:
-          Map from include files to their absolute paths. Must
-          not be None, but may be empty.
-
-        raw:
-          Optional raw content in the binding.
-          This does not have to have any "include:" lines resolved.
-          May be left out, in which case 'path' is opened and read.
-          This can be used to resolve child bindings, for example.
-
-        require_compatible:
-          If True, it is an error if the binding does not contain a
-          "compatible:" line. If False, a missing "compatible:" is
-          not an error. Either way, "compatible:" must be a string
-          if it is present in the binding.
-
-        require_description:
-          If True, it is an error if the binding does not contain a
-          "description:" line. If False, a missing "description:" is
-          not an error. Either way, "description:" must be a string
-          if it is present in the binding.
+        Returns the Node pointed at by the property named 'name' in /chosen, or
+        None if the property is missing
         """
-        self.path = path
-        self._fname2path = fname2path
-
-        if raw is None:
-            with open(path, encoding="utf-8") as f:
-                raw = yaml.load(f, Loader=_BindingLoader)
-
-        # Merge any included files into self.raw. This also pulls in
-        # inherited child binding definitions, so it has to be done
-        # before initializing those.
-        self.raw = self._merge_includes(raw, self.path)
-
-        # Recursively initialize any child bindings. These don't
-        # require a 'compatible' or 'description' to be well defined,
-        # but they must be dicts.
-        if "child-binding" in raw:
-            if not isinstance(raw["child-binding"], dict):
-                _err(f"malformed 'child-binding:' in {self.path}, "
-                     "expected a binding (dictionary with keys/values)")
-            self.child_binding = Binding(path, fname2path,
-                                         raw=raw["child-binding"],
-                                         require_compatible=False,
-                                         require_description=False)
-        else:
-            self.child_binding = None
-
-        # Make sure this is a well defined object.
-        self._check(require_compatible, require_description)
-
-        # Initialize look up tables.
-        self.prop2specs = {}
-        for prop_name in self.raw.get("properties", {}).keys():
-            self.prop2specs[prop_name] = PropertySpec(prop_name, self)
-        self.specifier2cells = {}
-        for key, val in self.raw.items():
-            if key.endswith("-cells"):
-                self.specifier2cells[key[:-len("-cells")]] = val
-
-    def __repr__(self):
-        if self.compatible:
-            compat = f" for compatible '{self.compatible}'"
-        else:
-            compat = ""
-        basename = os.path.basename(self.path or "")
-        return f"<Binding {basename}" + compat + ">"
+        return self.chosen_nodes.get(name)
 
     @property
-    def description(self):
-        "See the class docstring"
-        return self.raw.get('description')
+    def dts_source(self) -> str:
+        return f"{self._dt}"
 
-    @property
-    def compatible(self):
-        "See the class docstring"
-        return self.raw.get('compatible')
+    def __repr__(self) -> str:
+        return f"<EDT for '{self.dts_path}', binding directories " \
+            f"'{self.bindings_dirs}'>"
 
-    @property
-    def bus(self):
-        "See the class docstring"
-        return self.raw.get('bus')
+    def __deepcopy__(self, memo) -> 'EDT':
+        """
+        Implements support for the standard library copy.deepcopy()
+        function on EDT instances.
+        """
 
-    @property
-    def buses(self):
-        "See the class docstring"
-        if self.raw.get('bus') is not None:
-            return self._buses
-        else:
-            return []
+        ret = EDT(
+            None,
+            self.bindings_dirs,
+            warn_reg_unit_address_mismatch=self._warn_reg_unit_address_mismatch,
+            default_prop_types=self._default_prop_types,
+            support_fixed_partitions_on_any_bus=self._fixed_partitions_no_bus,
+            infer_binding_for_paths=set(self._infer_binding_for_paths),
+            vendor_prefixes=dict(self._vendor_prefixes),
+            werror=self._werror
+        )
+        ret.dts_path = self.dts_path
+        ret._dt = deepcopy(self._dt, memo)
+        ret._finish_init()
+        return ret
 
     @property
-    def on_bus(self):
-        "See the class docstring"
-        return self.raw.get('on-bus')
+    def scc_order(self) -> List[List[Node]]:
+        try:
+            return self._graph.scc_order()
+        except Exception as e:
+            raise EDTError(e)
 
-    def _merge_includes(self, raw, binding_path):
-        # Constructor helper. Merges included files in
-        # 'raw["include"]' into 'raw' using 'self._include_paths' as a
-        # source of include files, removing the "include" key while
-        # doing so.
+    def _init_graph(self) -> None:
+        # Constructs a graph of dependencies between Node instances,
+        # which is usable for computing a partial order over the dependencies.
+        # The algorithm supports detecting dependency loops.
         #
-        # This treats 'binding_path' as the binding file being built up
-        # and uses it for error messages.
+        # Actually computing the SCC order is lazily deferred to the
+        # first time the scc_order property is read.
 
-        if "include" not in raw:
-            return raw
+        for node in self.nodes:
+            # A Node always depends on its parent.
+            for child in node.children.values():
+                self._graph.add_edge(child, node)
 
-        include = raw.pop("include")
+            # A Node depends on any Nodes present in 'phandle',
+            # 'phandles', or 'phandle-array' property values.
+            for prop in node.props.values():
+                if prop.type == 'phandle':
+                    self._graph.add_edge(node, prop.val)
+                elif prop.type == 'phandles':
+                    if TYPE_CHECKING:
+                        assert isinstance(prop.val, list)
+                    for phandle_node in prop.val:
+                        self._graph.add_edge(node, phandle_node)
+                elif prop.type == 'phandle-array':
+                    if TYPE_CHECKING:
+                        assert isinstance(prop.val, list)
+                    for cd in prop.val:
+                        if cd is None:
+                            continue
+                        if TYPE_CHECKING:
+                            assert isinstance(cd, ControllerAndData)
+                        self._graph.add_edge(node, cd.controller)
 
-        # First, merge the included files together. If more than one included
-        # file has a 'required:' for a particular property, OR the values
-        # together, so that 'required: true' wins.
+            # A Node depends on whatever supports the interrupts it
+            # generates.
+            for intr in node.interrupts:
+                self._graph.add_edge(node, intr.controller)
 
-        merged = {}
+    def _init_compat2binding(self) -> None:
+        # Creates self._compat2binding, a dictionary that maps
+        # (<compatible>, <bus>) tuples (both strings) to Binding objects.
+        #
+        # The Binding objects are created from YAML files discovered
+        # in self.bindings_dirs as needed.
+        #
+        # For example, self._compat2binding["company,dev", "can"]
+        # contains the Binding for the 'company,dev' device, when it
+        # appears on the CAN bus.
+        #
+        # For bindings that don't specify a bus, <bus> is None, so that e.g.
+        # self._compat2binding["company,notonbus", None] is the Binding.
+        #
+        # Only bindings for 'compatible' strings that appear in the devicetree
+        # are loaded.
 
-        if isinstance(include, str):
-            # Simple scalar string case
-            _merge_props(merged, self._load_raw(include), None, binding_path,
-                         False)
-        elif isinstance(include, list):
-            # List of strings and maps. These types may be intermixed.
-            for elem in include:
-                if isinstance(elem, str):
-                    _merge_props(merged, self._load_raw(elem), None,
-                                 binding_path, False)
-                elif isinstance(elem, dict):
-                    name = elem.pop('name', None)
-                    allowlist = elem.pop('property-allowlist', None)
-                    blocklist = elem.pop('property-blocklist', None)
-                    child_filter = elem.pop('child-binding', None)
+        dt_compats = _dt_compats(self._dt)
+        # Searches for any 'compatible' string mentioned in the devicetree
+        # files, with a regex
+        dt_compats_search = re.compile(
+            "|".join(re.escape(compat) for compat in dt_compats)
+        ).search
 
-                    if elem:
-                        # We've popped out all the valid keys.
-                        _err(f"'include:' in {binding_path} should not have "
-                             f"these unexpected contents: {elem}")
+        for binding_path in self._binding_paths:
+            with open(binding_path, encoding="utf-8") as f:
+                contents = f.read()
 
-                    _check_include_dict(name, allowlist, blocklist,
-                                        child_filter, binding_path)
+            # As an optimization, skip parsing files that don't contain any of
+            # the .dts 'compatible' strings, which should be reasonably safe
+            if not dt_compats_search(contents):
+                continue
 
-                    contents = self._load_raw(name)
+            # Load the binding and check that it actually matches one of the
+            # compatibles. Might get false positives above due to comments and
+            # stuff.
 
-                    _filter_properties(contents, allowlist, blocklist,
-                                       child_filter, binding_path)
-                    _merge_props(merged, contents, None, binding_path, False)
-                else:
-                    _err(f"all elements in 'include:' in {binding_path} "
-                         "should be either strings or maps with a 'name' key "
-                         "and optional 'property-allowlist' or "
-                         f"'property-blocklist' keys, but got: {elem}")
-        else:
-            # Invalid item.
-            _err(f"'include:' in {binding_path} "
-                 f"should be a string or list, but has type {type(include)}")
+            try:
+                # Parsed PyYAML output (Python lists/dictionaries/strings/etc.,
+                # representing the file)
+                raw = yaml.load(contents, Loader=_BindingLoader)
+            except yaml.YAMLError as e:
+                _err(
+                        f"'{binding_path}' appears in binding directories "
+                        f"but isn't valid YAML: {e}")
+                continue
 
-        # Next, merge the merged included files into 'raw'. Error out if
-        # 'raw' has 'required: false' while the merged included files have
-        # 'required: true'.
+            # Convert the raw data to a Binding object, erroring out
+            # if necessary.
+            binding = self._binding(raw, binding_path, dt_compats)
 
-        _merge_props(raw, merged, None, binding_path, check_required=True)
+            # Register the binding in self._compat2binding, along with
+            # any child bindings that have their own compatibles.
+            while binding is not None:
+                if binding.compatible:
+                    self._register_binding(binding)
+                binding = binding.child_binding
 
-        return raw
+    def _binding(self,
+                 raw: Optional[dict],
+                 binding_path: str,
+                 dt_compats: Set[str]) -> Optional[Binding]:
+        # Convert a 'raw' binding from YAML to a Binding object and return it.
+        #
+        # Error out if the raw data looks like an invalid binding.
+        #
+        # Return None if the file doesn't contain a binding or the
+        # binding's compatible isn't in dt_compats.
 
-    def _load_raw(self, fname):
-        # Returns the contents of the binding given by 'fname' after merging
-        # any bindings it lists in 'include:' into it. 'fname' is just the
-        # basename of the file, so we check that there aren't multiple
-        # candidates.
+        # Get the 'compatible:' string.
+        if raw is None or "compatible" not in raw:
+            # Empty file, binding fragment, spurious file, etc.
+            return None
 
-        path = self._fname2path.get(fname)
+        compatible = raw["compatible"]
 
-        if not path:
-            _err(f"'{fname}' not found")
+        if compatible not in dt_compats:
+            # Not a compatible we care about.
+            return None
 
-        with open(path, encoding="utf-8") as f:
-            contents = yaml.load(f, Loader=_BindingLoader)
+        # Initialize and return the Binding object.
+        return Binding(binding_path, self._binding_fname2path, raw=raw)
 
-        return self._merge_includes(contents, path)
+    def _register_binding(self, binding: Binding) -> None:
+        # Do not allow two different bindings to have the same
+        # 'compatible:'/'on-bus:' combo
+        if TYPE_CHECKING:
+            assert binding.compatible
+        old_binding = self._compat2binding.get((binding.compatible,
+                                                binding.on_bus))
+        if old_binding:
+            msg = (f"both {old_binding.path} and {binding.path} have "
+                   f"'compatible: {binding.compatible}'")
+            if binding.on_bus is not None:
+                msg += f" and 'on-bus: {binding.on_bus}'"
+            _err(msg)
 
-    def _check(self, require_compatible, require_description):
-        # Does sanity checking on the binding.
+        # Register the binding.
+        self._compat2binding[binding.compatible, binding.on_bus] = binding
 
-        raw = self.raw
+    def _init_nodes(self) -> None:
+        # Creates a list of edtlib.Node objects from the dtlib.Node objects, in
+        # self.nodes
 
-        if "compatible" in raw:
-            compatible = raw["compatible"]
-            if not isinstance(compatible, str):
-                _err(f"malformed 'compatible: {compatible}' "
-                     f"field in {self.path} - "
-                     f"should be a string, not {type(compatible).__name__}")
-        elif require_compatible:
-            _err(f"missing 'compatible' in {self.path}")
+        for dt_node in self._dt.node_iter():
+            # Warning: We depend on parent Nodes being created before their
+            # children. This is guaranteed by node_iter().
+            if "compatible" in dt_node.props:
+                compats = dt_node.props["compatible"].to_strings()
+            else:
+                compats = []
+            node = Node(dt_node, self, compats)
+            node.bus_node = node._bus_node(self._fixed_partitions_no_bus)
+            node._init_binding()
+            node._init_regs()
+            node._init_ranges()
 
-        if "description" in raw:
-            description = raw["description"]
-            if not isinstance(description, str) or not description:
-                _err(f"malformed or empty 'description' in {self.path}")
-        elif require_description:
-            _err(f"missing 'description' in {self.path}")
+            self.nodes.append(node)
+            self._node2enode[dt_node] = node
 
-        # Allowed top-level keys. The 'include' key should have been
-        # removed by _load_raw() already.
-        ok_top = {"description", "compatible", "bus", "on-bus",
-                  "properties", "child-binding"}
+        for node in self.nodes:
+            # These depend on all Node objects having been created, because
+            # they (either always or sometimes) reference other nodes, so we
+            # run them separately
+            node._init_props(default_prop_types=self._default_prop_types,
+                             err_on_deprecated=self._werror)
+            node._init_interrupts()
+            node._init_pinctrls()
 
-        # Descriptive errors for legacy bindings.
-        legacy_errors = {
-            "#cells": "expected *-cells syntax",
-            "child": "use 'bus: <bus>' instead",
-            "child-bus": "use 'bus: <bus>' instead",
-            "parent": "use 'on-bus: <bus>' instead",
-            "parent-bus": "use 'on-bus: <bus>' instead",
-            "sub-node": "use 'child-binding' instead",
-            "title": "use 'description' instead",
-        }
+        if self._warn_reg_unit_address_mismatch:
+            # This warning matches the simple_bus_reg warning in dtc
+            for node in self.nodes:
+                if node.regs and node.regs[0].addr != node.unit_addr:
+                    _LOG.warning("unit address and first address in 'reg' "
+                                 f"(0x{node.regs[0].addr:x}) don't match for "
+                                 f"{node.path}")
 
-        for key in raw:
-            if key in legacy_errors:
-                _err(f"legacy '{key}:' in {self.path}, {legacy_errors[key]}")
+    def _init_luts(self) -> None:
+        # Initialize node lookup tables (LUTs).
 
-            if key not in ok_top and not key.endswith("-cells"):
-                _err(f"unknown key '{key}' in {self.path}, "
-                     "expected one of {', '.join(ok_top)}, or *-cells")
+        for node in self.nodes:
+            for label in node.labels:
+                self.label2node[label] = node
 
-        if "bus" in raw:
-            bus = raw["bus"]
-            if not isinstance(bus, str) and \
-               (not isinstance(bus, list) and \
-                not all(isinstance(elem, str) for elem in bus)):
-                _err(f"malformed 'bus:' value in {self.path}, "
-                     "expected string or list of strings")
+            for compat in node.compats:
+                self.compat2nodes[compat].append(node)
 
-            if isinstance(bus, list):
-                self._buses = bus
-            else:
-                # Convert bus into a list
-                self._buses = [bus]
+                if node.status == "okay":
+                    self.compat2okay[compat].append(node)
 
-        if "on-bus" in raw and \
-           not isinstance(raw["on-bus"], str):
-            _err(f"malformed 'on-bus:' value in {self.path}, "
-                 "expected string")
+                if compat in self.compat2vendor:
+                    continue
 
-        self._check_properties()
+                # The regular expression comes from dt-schema.
+                compat_re = r'^[a-zA-Z][a-zA-Z0-9,+\-._]+$'
+                if not re.match(compat_re, compat):
+                    _err(f"node '{node.path}' compatible '{compat}' "
+                         'must match this regular expression: '
+                         f"'{compat_re}'")
 
-        for key, val in raw.items():
-            if key.endswith("-cells"):
-                if not isinstance(val, list) or \
-                   not all(isinstance(elem, str) for elem in val):
-                    _err(f"malformed '{key}:' in {self.path}, "
-                         "expected a list of strings")
+                if ',' in compat and self._vendor_prefixes:
+                    vendor, model = compat.split(',', 1)
+                    if vendor in self._vendor_prefixes:
+                        self.compat2vendor[compat] = self._vendor_prefixes[vendor]
+                        self.compat2model[compat] = model
 
-    def _check_properties(self):
-        # _check() helper for checking the contents of 'properties:'.
+                    # As an exception, the root node can have whatever
+                    # compatibles it wants. Other nodes get checked.
+                    elif node.path != '/' and \
+                       vendor not in _VENDOR_PREFIX_ALLOWED:
+                        if self._werror:
+                            handler_fn: Any = _err
+                        else:
+                            handler_fn = _LOG.warning
+                        handler_fn(
+                            f"node '{node.path}' compatible '{compat}' "
+                            f"has unknown vendor prefix '{vendor}'")
 
-        raw = self.raw
 
-        if "properties" not in raw:
-            return
+        for nodeset in self.scc_order:
+            node = nodeset[0]
+            self.dep_ord2node[node.dep_ordinal] = node
 
-        ok_prop_keys = {"description", "type", "required",
-                        "enum", "const", "default", "deprecated",
-                        "specifier-space"}
+    def _check(self) -> None:
+        # Tree-wide checks and warnings.
 
-        for prop_name, options in raw["properties"].items():
-            for key in options:
-                if key not in ok_prop_keys:
-                    _err(f"unknown setting '{key}' in "
-                         f"'properties: {prop_name}: ...' in {self.path}, "
-                         f"expected one of {', '.join(ok_prop_keys)}")
+        for binding in self._compat2binding.values():
+            for spec in binding.prop2specs.values():
+                if not spec.enum or spec.type != 'string':
+                    continue
 
-            _check_prop_by_type(prop_name, options, self.path)
+                if not spec.enum_tokenizable:
+                    _LOG.warning(
+                        f"compatible '{binding.compatible}' "
+                        f"in binding '{binding.path}' has non-tokenizable enum "
+                        f"for property '{spec.name}': " +
+                        ', '.join(repr(x) for x in spec.enum))
+                elif not spec.enum_upper_tokenizable:
+                    _LOG.warning(
+                        f"compatible '{binding.compatible}' "
+                        f"in binding '{binding.path}' has enum for property "
+                        f"'{spec.name}' that is only tokenizable "
+                        'in lowercase: ' +
+                        ', '.join(repr(x) for x in spec.enum))
 
-            for true_false_opt in ["required", "deprecated"]:
-                if true_false_opt in options:
-                    option = options[true_false_opt]
-                    if not isinstance(option, bool):
-                        _err(f"malformed '{true_false_opt}:' setting '{option}' "
-                             f"for '{prop_name}' in 'properties' in {self.path}, "
-                             "expected true/false")
+        # Validate the contents of compatible properties.
+        for node in self.nodes:
+            if 'compatible' not in node.props:
+                continue
 
-            if options.get("deprecated") and options.get("required"):
-                _err(f"'{prop_name}' in 'properties' in {self.path} should not "
-                      "have both 'deprecated' and 'required' set")
+            compatibles = node.props['compatible'].val
 
-            if "description" in options and \
-               not isinstance(options["description"], str):
-                _err("missing, malformed, or empty 'description' for "
-                     f"'{prop_name}' in 'properties' in {self.path}")
+            # _check() runs after _init_compat2binding() has called
+            # _dt_compats(), which already converted every compatible
+            # property to a list of strings. So we know 'compatibles'
+            # is a list, but add an assert for future-proofing.
+            assert isinstance(compatibles, list)
 
-            if "enum" in options and not isinstance(options["enum"], list):
-                _err(f"enum in {self.path} for property '{prop_name}' "
-                     "is not a list")
+            for compat in compatibles:
+                # This is also just for future-proofing.
+                assert isinstance(compat, str)
 
 
-def bindings_from_paths(yaml_paths, ignore_errors=False):
+def bindings_from_paths(yaml_paths: List[str],
+                        ignore_errors: bool = False) -> List[Binding]:
     """
     Get a list of Binding objects from the yaml files 'yaml_paths'.
 
     If 'ignore_errors' is True, YAML files that cause an EDTError when
     loaded are ignored. (No other exception types are silenced.)
     """
 
@@ -2098,166 +2319,28 @@
         except EDTError:
             if ignore_errors:
                 continue
             raise
 
     return ret
 
-class PropertySpec:
-    """
-    Represents a "property specification", i.e. the description of a
-    property provided by a binding file, like its type and description.
-
-    These attributes are available on PropertySpec objects:
-
-    binding:
-      The Binding object which defined this property.
-
-    name:
-      The property's name.
-
-    path:
-      The file where this property was defined. In case a binding includes
-      other bindings, this is the file where the property was last modified.
-
-    type:
-      The type of the property as a string, as given in the binding.
-
-    description:
-      The free-form description of the property as a string, or None.
-
-    enum:
-      A list of values the property may take as given in the binding, or None.
-
-    enum_tokenizable:
-      True if enum is not None and all the values in it are tokenizable;
-      False otherwise.
-
-      A property must have string type and an "enum:" in its binding to be
-      tokenizable. Additionally, the "enum:" values must be unique after
-      converting all non-alphanumeric characters to underscores (so "foo bar"
-      and "foo_bar" in the same "enum:" would not be tokenizable).
-
-    enum_upper_tokenizable:
-      Like 'enum_tokenizable', with the additional restriction that the
-      "enum:" values must be unique after uppercasing and converting
-      non-alphanumeric characters to underscores.
-
-    const:
-      The property's constant value as given in the binding, or None.
-
-    default:
-      The property's default value as given in the binding, or None.
-
-    deprecated:
-      True if the property is deprecated; False otherwise.
-
-    required:
-      True if the property is marked required; False otherwise.
-
-    specifier_space:
-      The specifier space for the property as given in the binding, or None.
-    """
-
-    def __init__(self, name, binding):
-        self.binding = binding
-        self.name = name
-        self._raw = self.binding.raw["properties"][name]
-
-    def __repr__(self):
-        return f"<PropertySpec {self.name} type '{self.type}'>"
-
-    @property
-    def path(self):
-        "See the class docstring"
-        return self.binding.path
-
-    @property
-    def type(self):
-        "See the class docstring"
-        return self._raw["type"]
-
-    @property
-    def description(self):
-        "See the class docstring"
-        return self._raw.get("description")
-
-    @property
-    def enum(self):
-        "See the class docstring"
-        return self._raw.get("enum")
-
-    @property
-    def enum_tokenizable(self):
-        "See the class docstring"
-        if not hasattr(self, '_enum_tokenizable'):
-            if self.type != 'string' or self.enum is None:
-                self._enum_tokenizable = False
-            else:
-                # Saving _as_tokens here lets us reuse it in
-                # enum_upper_tokenizable.
-                self._as_tokens = [re.sub(_NOT_ALPHANUM_OR_UNDERSCORE,
-                                          '_', value)
-                                   for value in self.enum]
-                self._enum_tokenizable = (len(self._as_tokens) ==
-                                          len(set(self._as_tokens)))
-
-        return self._enum_tokenizable
-
-    @property
-    def enum_upper_tokenizable(self):
-        "See the class docstring"
-        if not hasattr(self, '_enum_upper_tokenizable'):
-            if not self.enum_tokenizable:
-                self._enum_upper_tokenizable = False
-            else:
-                self._enum_upper_tokenizable = \
-                    (len(self._as_tokens) ==
-                     len(set(x.upper() for x in self._as_tokens)))
-        return self._enum_upper_tokenizable
-
-    @property
-    def const(self):
-        "See the class docstring"
-        return self._raw.get("const")
-
-    @property
-    def default(self):
-        "See the class docstring"
-        return self._raw.get("default")
-
-    @property
-    def required(self):
-        "See the class docstring"
-        return self._raw.get("required", False)
-
-    @property
-    def deprecated(self):
-        "See the class docstring"
-        return self._raw.get("deprecated", False)
-
-    @property
-    def specifier_space(self):
-        "See the class docstring"
-        return self._raw.get("specifier-space")
-
 
 class EDTError(Exception):
     "Exception raised for devicetree- and binding-related errors"
 
 #
 # Public global functions
 #
 
 
-def load_vendor_prefixes_txt(vendor_prefixes):
+def load_vendor_prefixes_txt(vendor_prefixes: str) -> Dict[str, str]:
     """Load a vendor-prefixes.txt file and return a dict
     representation mapping a vendor prefix to the vendor name.
     """
-    vnd2vendor = {}
+    vnd2vendor: Dict[str, str] = {}
     with open(vendor_prefixes, 'r', encoding='utf-8') as f:
         for line in f:
             line = line.strip()
 
             if not line or line.startswith('#'):
                 # Comment or empty line.
                 continue
@@ -2271,25 +2354,25 @@
     return vnd2vendor
 
 #
 # Private global functions
 #
 
 
-def _dt_compats(dt):
+def _dt_compats(dt: DT) -> Set[str]:
     # Returns a set() with all 'compatible' strings in the devicetree
     # represented by dt (a dtlib.DT instance)
 
     return {compat
             for node in dt.node_iter()
                 if "compatible" in node.props
                     for compat in node.props["compatible"].to_strings()}
 
 
-def _binding_paths(bindings_dirs):
+def _binding_paths(bindings_dirs: List[str]) -> List[str]:
     # Returns a list with the paths to all bindings (.yaml files) in
     # 'bindings_dirs'
 
     binding_paths = []
 
     for bindings_dir in bindings_dirs:
         for root, _, filenames in os.walk(bindings_dir):
@@ -2302,16 +2385,19 @@
 
 def _binding_inc_error(msg):
     # Helper for reporting errors in the !include implementation
 
     raise yaml.constructor.ConstructorError(None, None, "error: " + msg)
 
 
-def _check_include_dict(name, allowlist, blocklist, child_filter,
-                        binding_path):
+def _check_include_dict(name: Optional[str],
+                        allowlist: Optional[List[str]],
+                        blocklist: Optional[List[str]],
+                        child_filter: Optional[dict],
+                        binding_path: Optional[str]) -> None:
     # Check that an 'include:' named 'name' with property-allowlist
     # 'allowlist', property-blocklist 'blocklist', and
     # child-binding filter 'child_filter' has valid structure.
 
     if name is None:
         _err(f"'include:' element in {binding_path} "
              "should have a 'name' key")
@@ -2319,17 +2405,20 @@
     if allowlist is not None and blocklist is not None:
         _err(f"'include:' of file '{name}' in {binding_path} "
              "should not specify both 'property-allowlist:' "
              "and 'property-blocklist:'")
 
     while child_filter is not None:
         child_copy = deepcopy(child_filter)
-        child_allowlist = child_copy.pop('property-allowlist', None)
-        child_blocklist = child_copy.pop('property-blocklist', None)
-        next_child_filter = child_copy.pop('child-binding', None)
+        child_allowlist: Optional[List[str]] = \
+            child_copy.pop('property-allowlist', None)
+        child_blocklist: Optional[List[str]] = \
+            child_copy.pop('property-blocklist', None)
+        next_child_filter: Optional[dict] = \
+            child_copy.pop('child-binding', None)
 
         if child_copy:
             # We've popped out all the valid keys.
             _err(f"'include:' of file '{name}' in {binding_path} "
                  "should not have these unexpected contents in a "
                  f"'child-binding': {child_copy}")
 
@@ -2337,16 +2426,19 @@
             _err(f"'include:' of file '{name}' in {binding_path} "
                  "should not specify both 'property-allowlist:' and "
                  "'property-blocklist:' in a 'child-binding:'")
 
         child_filter = next_child_filter
 
 
-def _filter_properties(raw, allowlist, blocklist, child_filter,
-                       binding_path):
+def _filter_properties(raw: dict,
+                       allowlist: Optional[List[str]],
+                       blocklist: Optional[List[str]],
+                       child_filter: Optional[dict],
+                       binding_path: Optional[str]) -> None:
     # Destructively modifies 'raw["properties"]' and
     # 'raw["child-binding"]', if they exist, according to
     # 'allowlist', 'blocklist', and 'child_filter'.
 
     props = raw.get('properties')
     _filter_properties_helper(props, allowlist, blocklist, binding_path)
 
@@ -2356,44 +2448,54 @@
                                   child_filter.get('property-allowlist'),
                                   child_filter.get('property-blocklist'),
                                   binding_path)
         child_filter = child_filter.get('child-binding')
         child_binding = child_binding.get('child-binding')
 
 
-def _filter_properties_helper(props, allowlist, blocklist, binding_path):
+def _filter_properties_helper(props: Optional[dict],
+                              allowlist: Optional[List[str]],
+                              blocklist: Optional[List[str]],
+                              binding_path: Optional[str]) -> None:
     if props is None or (allowlist is None and blocklist is None):
         return
 
     _check_prop_filter('property-allowlist', allowlist, binding_path)
     _check_prop_filter('property-blocklist', blocklist, binding_path)
 
     if allowlist is not None:
         allowset = set(allowlist)
         to_del = [prop for prop in props if prop not in allowset]
     else:
+        if TYPE_CHECKING:
+            assert blocklist
         blockset = set(blocklist)
         to_del = [prop for prop in props if prop in blockset]
 
     for prop in to_del:
         del props[prop]
 
 
-def _check_prop_filter(name, value, binding_path):
+def _check_prop_filter(name: str, value: Optional[List[str]],
+                       binding_path: Optional[str]) -> None:
     # Ensure an include: ... property-allowlist or property-blocklist
     # is a list.
 
     if value is None:
         return
 
     if not isinstance(value, list):
         _err(f"'{name}' value {value} in {binding_path} should be a list")
 
 
-def _merge_props(to_dict, from_dict, parent, binding_path, check_required):
+def _merge_props(to_dict: dict,
+                 from_dict: dict,
+                 parent: Optional[str],
+                 binding_path: Optional[str],
+                 check_required: bool = False):
     # Recursively merges 'from_dict' into 'to_dict', to implement 'include:'.
     #
     # If 'from_dict' and 'to_dict' contain a 'required:' key for the same
     # property, then the values are ORed together.
     #
     # If 'check_required' is True, then an error is raised if 'from_dict' has
     # 'required: true' while 'to_dict' has 'required: false'. This prevents
@@ -2427,15 +2529,16 @@
                 _err(f"malformed 'required:' setting for '{parent}' in "
                      f"'properties' in {binding_path}, expected true/false")
 
             # 'required: true' takes precedence
             to_dict["required"] = to_dict["required"] or from_dict["required"]
 
 
-def _bad_overwrite(to_dict, from_dict, prop, check_required):
+def _bad_overwrite(to_dict: dict, from_dict: dict, prop: str,
+                   check_required: bool) -> bool:
     # _merge_props() helper. Returns True in cases where it's bad that
     # to_dict[prop] takes precedence over from_dict[prop].
 
     if to_dict[prop] == from_dict[prop]:
         return False
 
     # These are overridden deliberately
@@ -2461,15 +2564,17 @@
     if isinstance(node, yaml.SequenceNode):
         # !include [foo.yaml, bar.yaml]
         return loader.construct_sequence(node)
 
     _binding_inc_error("unrecognised node type in !include statement")
 
 
-def _check_prop_by_type(prop_name, options, binding_path):
+def _check_prop_by_type(prop_name: str,
+                        options: dict,
+                        binding_path: Optional[str]) -> None:
     # Binding._check_properties() helper. Checks 'type:', 'default:',
     # 'const:' and # 'specifier-space:' for the property named 'prop_name'
 
     prop_type = options.get("type")
     default = options.get("default")
     const = options.get("const")
 
@@ -2492,14 +2597,16 @@
 
     if prop_type == "phandle-array":
         if not prop_name.endswith("s") and not "specifier-space" in options:
             _err(f"'{prop_name}' in 'properties:' in {binding_path} "
                  f"has type 'phandle-array' and its name does not end in 's', "
                  f"but no 'specifier-space' was provided.")
 
+    # If you change const_types, be sure to update the type annotation
+    # for PropertySpec.const.
     const_types = {"int", "array", "uint8-array", "string", "string-array"}
     if const and prop_type not in const_types:
         _err(f"const in {binding_path} for property '{prop_name}' "
              f"has type '{prop_type}', expected one of " +
              ", ".join(const_types))
 
     # Check default
@@ -2509,16 +2616,18 @@
 
     if prop_type in {"boolean", "compound", "phandle", "phandles",
                      "phandle-array", "path"}:
         _err("'default:' can't be combined with "
              f"'type: {prop_type}' for '{prop_name}' in "
              f"'properties:' in {binding_path}")
 
-    def ok_default():
-        # Returns True if 'default' is an okay default for the property's type
+    def ok_default() -> bool:
+        # Returns True if 'default' is an okay default for the property's type.
+        # If you change this, be sure to update the type annotation for
+        # PropertySpec.default.
 
         if prop_type == "int" and isinstance(default, int) or \
            prop_type == "string" and isinstance(default, str):
             return True
 
         # array, uint8-array, or string-array
 
@@ -2538,21 +2647,18 @@
 
     if not ok_default():
         _err(f"'default: {default}' is invalid for '{prop_name}' "
              f"in 'properties:' in {binding_path}, "
              f"which has type {prop_type}")
 
 
-def _translate(addr, node):
+def _translate(addr: int, node: dtlib_Node) -> int:
     # Recursively translates 'addr' on 'node' to the address space(s) of its
     # parent(s), by looking at 'ranges' properties. Returns the translated
     # address.
-    #
-    # node:
-    #   dtlib.Node instance
 
     if not node.parent or "ranges" not in node.parent.props:
         # No translation
         return addr
 
     if not node.parent.props["ranges"].value:
         # DT spec.: "If the property is defined with an <empty> value, it
@@ -2589,19 +2695,19 @@
             # translate it and return the result.
             return _translate(parent_addr + addr - child_addr, node.parent)
 
     # 'addr' is not within range of any translation in 'ranges'
     return addr
 
 
-def _add_names(node, names_ident, objs):
+def _add_names(node: dtlib_Node, names_ident: str, objs: Any) -> None:
     # Helper for registering names from <foo>-names properties.
     #
     # node:
-    #   edtlib.Node instance
+    #   Node which has a property that might need named elements.
     #
     # names-ident:
     #   The <foo> part of <foo>-names, e.g. "reg" for "reg-names"
     #
     # objs:
     #   list of objects whose .name field should be set
 
@@ -2620,41 +2726,48 @@
             obj.name = name
     else:
         for obj in objs:
             if obj is not None:
                 obj.name = None
 
 
-def _interrupt_parent(node):
+def _interrupt_parent(start_node: dtlib_Node) -> dtlib_Node:
     # Returns the node pointed at by the closest 'interrupt-parent', searching
     # the parents of 'node'. As of writing, this behavior isn't specified in
     # the DT spec., but seems to match what some .dts files except.
 
-    start_node = node
+    node: Optional[dtlib_Node] = start_node
 
     while node:
         if "interrupt-parent" in node.props:
             return node.props["interrupt-parent"].to_node()
         node = node.parent
 
     _err(f"{start_node!r} has an 'interrupts' property, but neither the node "
          f"nor any of its parents has an 'interrupt-parent' property")
 
 
-def _interrupts(node):
+def _interrupts(node: dtlib_Node) -> List[Tuple[dtlib_Node, bytes]]:
     # Returns a list of (<controller>, <data>) tuples, with one tuple per
     # interrupt generated by 'node'. <controller> is the destination of the
     # interrupt (possibly after mapping through an 'interrupt-map'), and <data>
     # the data associated with the interrupt (as a 'bytes' object).
 
     # Takes precedence over 'interrupts' if both are present
     if "interrupts-extended" in node.props:
         prop = node.props["interrupts-extended"]
-        return [_map_interrupt(node, iparent, spec)
-                for iparent, spec in _phandle_val_list(prop, "interrupt")]
+
+        ret: List[Tuple[dtlib_Node, bytes]] = []
+        for entry in _phandle_val_list(prop, "interrupt"):
+            if entry is None:
+                _err(f"node '{node.path}' interrupts-extended property "
+                     "has an empty element")
+            iparent, spec = entry
+            ret.append(_map_interrupt(node, iparent, spec))
+        return ret
 
     if "interrupts" in node.props:
         # Treat 'interrupts' as a special case of 'interrupts-extended', with
         # the same interrupt parent for all interrupts
 
         iparent = _interrupt_parent(node)
         interrupt_cells = _interrupt_cells(iparent)
@@ -2662,15 +2775,19 @@
         return [_map_interrupt(node, iparent, raw)
                 for raw in _slice(node, "interrupts", 4*interrupt_cells,
                                   "4*<#interrupt-cells>")]
 
     return []
 
 
-def _map_interrupt(child, parent, child_spec):
+def _map_interrupt(
+        child: dtlib_Node,
+        parent: dtlib_Node,
+        child_spec: bytes
+) -> Tuple[dtlib_Node, bytes]:
     # Translates an interrupt headed from 'child' to 'parent' with data
     # 'child_spec' through any 'interrupt-map' properties. Returns a
     # (<controller>, <data>) tuple with the final destination after mapping.
 
     if "interrupt-controller" in parent.props:
         return (parent, child_spec)
 
@@ -2694,15 +2811,20 @@
         "interrupt", child, parent, _raw_unit_addr(child) + child_spec,
         spec_len_fn, require_controller=True)
 
     # Strip the parent unit address part, if any
     return (parent, raw_spec[4*own_address_cells(parent):])
 
 
-def _map_phandle_array_entry(child, parent, child_spec, basename):
+def _map_phandle_array_entry(
+        child: dtlib_Node,
+        parent: dtlib_Node,
+        child_spec: bytes,
+        basename: str
+) -> Tuple[dtlib_Node, bytes]:
     # Returns a (<controller>, <data>) tuple with the final destination after
     # mapping through any '<basename>-map' (e.g. gpio-map) properties. See
     # _map_interrupt().
 
     def spec_len_fn(node):
         prop_name = f"#{basename}-cells"
         if prop_name not in node.props:
@@ -2711,15 +2833,22 @@
         return node.props[prop_name].to_num()
 
     # Do not require <prefix>-controller for anything but interrupts for now
     return _map(basename, child, parent, child_spec, spec_len_fn,
                 require_controller=False)
 
 
-def _map(prefix, child, parent, child_spec, spec_len_fn, require_controller):
+def _map(
+        prefix: str,
+        child: dtlib_Node,
+        parent: dtlib_Node,
+        child_spec: bytes,
+        spec_len_fn: Callable[[dtlib_Node], int],
+        require_controller: bool
+) -> Tuple[dtlib_Node, bytes]:
     # Common code for mapping through <prefix>-map properties, e.g.
     # interrupt-map and gpio-map.
     #
     # prefix:
     #   The prefix, e.g. "interrupt" or "gpio"
     #
     # child:
@@ -2781,19 +2910,24 @@
             parent_spec = _pass_thru(
                 prefix, child, parent, child_spec, parent_spec)
 
             # Found match. Recursively map and return it.
             return _map(prefix, parent, map_parent, parent_spec, spec_len_fn,
                         require_controller)
 
-    _err(f"child specifier for {child!r} ({child_spec}) "
+    _err(f"child specifier for {child!r} ({child_spec!r}) "
          f"does not appear in {map_prop!r}")
 
 
-def _mask(prefix, child, parent, child_spec):
+def _mask(
+        prefix: str,
+        child: dtlib_Node,
+        parent: dtlib_Node,
+        child_spec: bytes
+) -> bytes:
     # Common code for handling <prefix>-mask properties, e.g. interrupt-mask.
     # See _map() for the parameters.
 
     mask_prop = parent.props.get(prefix + "-map-mask")
     if not mask_prop:
         # No mask
         return child_spec
@@ -2802,15 +2936,21 @@
     if len(mask) != len(child_spec):
         _err(f"{child!r}: expected '{prefix}-mask' in {parent!r} "
              f"to be {len(child_spec)} bytes, is {len(mask)} bytes")
 
     return _and(child_spec, mask)
 
 
-def _pass_thru(prefix, child, parent, child_spec, parent_spec):
+def _pass_thru(
+        prefix: str,
+        child: dtlib_Node,
+        parent: dtlib_Node,
+        child_spec: bytes,
+        parent_spec: bytes
+) -> bytes:
     # Common code for handling <prefix>-map-thru properties, e.g.
     # interrupt-pass-thru.
     #
     # parent_spec:
     #   The parent data from the matched entry in the <prefix>-map property
     #
     # See _map() for the other parameters.
@@ -2828,15 +2968,15 @@
     res = _or(_and(child_spec, pass_thru),
               _and(parent_spec, _not(pass_thru)))
 
     # Truncate to length of parent spec.
     return res[-len(parent_spec):]
 
 
-def _raw_unit_addr(node):
+def _raw_unit_addr(node: dtlib_Node) -> bytes:
     # _map_interrupt() helper. Returns the unit address (derived from 'reg' and
     # #address-cells) as a raw 'bytes'
 
     if 'reg' not in node.props:
         _err(f"{node!r} lacks 'reg' property "
              "(needed for 'interrupt-map' unit address lookup)")
 
@@ -2845,62 +2985,63 @@
     if len(node.props['reg'].value) < addr_len:
         _err(f"{node!r} has too short 'reg' property "
              "(while doing 'interrupt-map' unit address lookup)")
 
     return node.props['reg'].value[:addr_len]
 
 
-def _and(b1, b2):
+def _and(b1: bytes, b2: bytes) -> bytes:
     # Returns the bitwise AND of the two 'bytes' objects b1 and b2. Pads
     # with ones on the left if the lengths are not equal.
 
     # Pad on the left, to equal length
     maxlen = max(len(b1), len(b2))
     return bytes(x & y for x, y in zip(b1.rjust(maxlen, b'\xff'),
                                        b2.rjust(maxlen, b'\xff')))
 
 
-def _or(b1, b2):
+def _or(b1: bytes, b2: bytes) -> bytes:
     # Returns the bitwise OR of the two 'bytes' objects b1 and b2. Pads with
     # zeros on the left if the lengths are not equal.
 
     # Pad on the left, to equal length
     maxlen = max(len(b1), len(b2))
     return bytes(x | y for x, y in zip(b1.rjust(maxlen, b'\x00'),
                                        b2.rjust(maxlen, b'\x00')))
 
 
-def _not(b):
+def _not(b: bytes) -> bytes:
     # Returns the bitwise not of the 'bytes' object 'b'
 
     # ANDing with 0xFF avoids negative numbers
     return bytes(~x & 0xFF for x in b)
 
 
-def _phandle_val_list(prop, n_cells_name):
+def _phandle_val_list(
+        prop: dtlib_Property,
+        n_cells_name: str
+) -> List[Optional[Tuple[dtlib_Node, bytes]]]:
     # Parses a '<phandle> <value> <phandle> <value> ...' value. The number of
     # cells that make up each <value> is derived from the node pointed at by
     # the preceding <phandle>.
     #
     # prop:
     #   dtlib.Property with value to parse
     #
     # n_cells_name:
     #   The <name> part of the #<name>-cells property to look for on the nodes
     #   the phandles point to, e.g. "gpio" for #gpio-cells.
     #
-    # Returns a list[Optional[tuple]].
-    #
-    # Each tuple in the list is a (<node>, <value>) pair, where <node>
+    # Each tuple in the return value is a (<node>, <value>) pair, where <node>
     # is the node pointed at by <phandle>. If <phandle> does not refer
     # to a node, the entire list element is None.
 
     full_n_cells_name = f"#{n_cells_name}-cells"
 
-    res = []
+    res: List[Optional[Tuple[dtlib_Node, bytes]]] = []
 
     raw = prop.value
     while raw:
         if len(raw) < 4:
             # Not enough room for phandle
             _err("bad value for " + repr(prop))
         phandle = to_num(raw[:4])
@@ -2922,58 +3063,53 @@
 
         res.append((node, raw[:4*n_cells]))
         raw = raw[4*n_cells:]
 
     return res
 
 
-def _address_cells(node):
+def _address_cells(node: dtlib_Node) -> int:
     # Returns the #address-cells setting for 'node', giving the number of <u32>
     # cells used to encode the address in the 'reg' property
+    if TYPE_CHECKING:
+        assert node.parent
 
     if "#address-cells" in node.parent.props:
         return node.parent.props["#address-cells"].to_num()
     return 2  # Default value per DT spec.
 
 
-def _size_cells(node):
+def _size_cells(node: dtlib_Node) -> int:
     # Returns the #size-cells setting for 'node', giving the number of <u32>
     # cells used to encode the size in the 'reg' property
+    if TYPE_CHECKING:
+        assert node.parent
 
     if "#size-cells" in node.parent.props:
         return node.parent.props["#size-cells"].to_num()
     return 1  # Default value per DT spec.
 
 
-def _interrupt_cells(node):
+def _interrupt_cells(node: dtlib_Node) -> int:
     # Returns the #interrupt-cells property value on 'node', erroring out if
     # 'node' has no #interrupt-cells property
 
     if "#interrupt-cells" not in node.props:
         _err(f"{node!r} lacks #interrupt-cells")
     return node.props["#interrupt-cells"].to_num()
 
 
-def _slice(node, prop_name, size, size_hint):
-    # Splits node.props[prop_name].value into 'size'-sized chunks, returning a
-    # list of chunks. Raises EDTError if the length of the property is not
-    # evenly divisible by 'size'. 'size_hint' is a string shown on errors that
-    # gives a hint on how 'size' was calculated.
-
-    raw = node.props[prop_name].value
-    if len(raw) % size:
-        _err(f"'{prop_name}' property in {node!r} has length {len(raw)}, "
-             f"which is not evenly divisible by {size} (= {size_hint}). "
-             "Note that #*-cells properties come either from the parent node or "
-             "from the controller (in the case of 'interrupts').")
-
-    return [raw[i:i + size] for i in range(0, len(raw), size)]
+def _slice(node: dtlib_Node,
+           prop_name: str,
+           size: int,
+           size_hint: str) -> List[bytes]:
+    return _slice_helper(node, prop_name, size, size_hint, EDTError)
 
 
-def _check_dt(dt):
+def _check_dt(dt: DT) -> None:
     # Does devicetree sanity checks. dtlib is meant to be general and
     # anything-goes except for very special properties like phandle, but in
     # edtlib we can be pickier.
 
     # Check that 'status' has one of the values given in the devicetree spec.
 
     # Accept "ok" for backwards compatibility
@@ -2997,25 +3133,25 @@
         if ranges_prop:
             if ranges_prop.type not in (Type.EMPTY, Type.NUMS):
                 _err(f"expected 'ranges = < ... >;' in {node.path} in "
                      f"{node.dt.filename}, not '{ranges_prop}' "
                      "(see the devicetree specification)")
 
 
-def _err(msg):
+def _err(msg) -> NoReturn:
     raise EDTError(msg)
 
 # Logging object
 _LOG = logging.getLogger(__name__)
 
 # Regular expression for non-alphanumeric-or-underscore characters.
 _NOT_ALPHANUM_OR_UNDERSCORE = re.compile(r'\W', re.ASCII)
 
 
-def str_as_token(val):
+def str_as_token(val: str) -> str:
     """Return a canonical representation of a string as a C token.
 
     This converts special characters in 'val' to underscores, and
     returns the result."""
 
     return re.sub(_NOT_ALPHANUM_OR_UNDERSCORE, '_', val)
 
@@ -3033,56 +3169,58 @@
 # "Default" binding for properties which are defined by the spec.
 #
 # Zephyr: do not change the _DEFAULT_PROP_TYPES keys without
 # updating the documentation for the DT_PROP() macro in
 # include/devicetree.h.
 #
 
-_DEFAULT_PROP_TYPES = {
+_DEFAULT_PROP_TYPES: Dict[str, str] = {
     "compatible": "string-array",
     "status": "string",
     "reg": "array",
     "reg-names": "string-array",
     "label": "string",
     "interrupts": "array",
     "interrupts-extended": "compound",
     "interrupt-names": "string-array",
     "interrupt-controller": "boolean",
 }
 
-_STATUS_ENUM = "ok okay disabled reserved fail fail-sss".split()
+_STATUS_ENUM: List[str] = "ok okay disabled reserved fail fail-sss".split()
 
-def _raw_default_property_for(name):
-    ret = {
+def _raw_default_property_for(
+        name: str
+) -> Dict[str, Union[str, bool, List[str]]]:
+    ret: Dict[str, Union[str, bool, List[str]]] = {
         'type': _DEFAULT_PROP_TYPES[name],
         'required': False,
     }
     if name == 'status':
         ret['enum'] = _STATUS_ENUM
     return ret
 
-_DEFAULT_PROP_BINDING = Binding(
+_DEFAULT_PROP_BINDING: Binding = Binding(
     None, {},
     raw={
         'properties': {
             name: _raw_default_property_for(name)
             for name in _DEFAULT_PROP_TYPES
         },
     },
     require_compatible=False, require_description=False,
 )
 
-_DEFAULT_PROP_SPECS = {
+_DEFAULT_PROP_SPECS: Dict[str, PropertySpec] = {
     name: PropertySpec(name, _DEFAULT_PROP_BINDING)
     for name in _DEFAULT_PROP_TYPES
 }
 
 # A set of vendor prefixes which are grandfathered in by Linux,
 # and therefore by us as well.
-_VENDOR_PREFIX_ALLOWED = set([
+_VENDOR_PREFIX_ALLOWED: Set[str] = set([
     "at25", "bm", "devbus", "dmacap", "dsa",
     "exynos", "fsia", "fsib", "gpio-fan", "gpio-key", "gpio", "gpmc",
     "hdmi", "i2c-gpio", "keypad", "m25p", "max8952", "max8997",
     "max8998", "mpmc", "pinctrl-single", "#pinctrl-single", "PowerPC",
     "pl022", "pxa-mmc", "rcar_sound", "rotary-encoder", "s5m8767",
     "sdhci", "simple-audio-card", "st-plgpio", "st-spics", "ts",
 ])
```

### Comparing `dtsh-0.1.0a6/src/devicetree/grutils.py` & `dtsh-0.1.0b1/src/devicetree/grutils.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/autocomp.py` & `dtsh-0.1.0b1/src/dtsh/autocomp.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_alias.py` & `dtsh-0.1.0b1/src/dtsh/builtin_alias.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_cat.py` & `dtsh-0.1.0b1/src/dtsh/builtin_cat.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_cd.py` & `dtsh-0.1.0b1/src/dtsh/builtin_cd.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_chosen.py` & `dtsh-0.1.0b1/src/dtsh/builtin_chosen.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_find.py` & `dtsh-0.1.0b1/src/dtsh/builtin_find.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_ls.py` & `dtsh-0.1.0b1/src/dtsh/builtin_ls.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_man.py` & `dtsh-0.1.0b1/src/dtsh/builtin_man.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_pwd.py` & `dtsh-0.1.0b1/src/dtsh/builtin_pwd.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_tree.py` & `dtsh-0.1.0b1/src/dtsh/builtin_tree.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/builtin_uname.py` & `dtsh-0.1.0b1/src/dtsh/builtin_uname.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/cli.py` & `dtsh-0.1.0b1/src/dtsh/cli.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/config.py` & `dtsh-0.1.0b1/src/dtsh/config.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/dtsh.py` & `dtsh-0.1.0b1/src/dtsh/dtsh.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,15 @@
     """Shell-like interface to a devicetree.
 
     The global metaphor is:
     - a filesystem-like view of the devicetree model
     - a command string interface to POSIX-like shell commands (aka built-ins)
     """
 
-    API_VERSION = '0.1.0a6'
+    API_VERSION = '0.1.0b1'
     """API version for the dtsh module.
 
     Should match 'version' in setup.py.
     """
 
     # Devicetree model (edtlib).
     _edt: EDT
```

### Comparing `dtsh-0.1.0a6/src/dtsh/man.py` & `dtsh-0.1.0b1/src/dtsh/man.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/rl.py` & `dtsh-0.1.0b1/src/dtsh/rl.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/session.py` & `dtsh-0.1.0b1/src/dtsh/session.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/shell.py` & `dtsh-0.1.0b1/src/dtsh/shell.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/systools.py` & `dtsh-0.1.0b1/src/dtsh/systools.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/term.py` & `dtsh-0.1.0b1/src/dtsh/term.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/theme` & `dtsh-0.1.0b1/src/dtsh/theme`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh/tui.py` & `dtsh-0.1.0b1/src/dtsh/tui.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/src/dtsh.egg-info/PKG-INFO` & `dtsh-0.1.0b1/src/dtsh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dtsh
-Version: 0.1.0a6
+Version: 0.1.0b1
 Summary: Shell-like interface with Zephyr devicetree and bindings
 Home-page: https://github.com/dottspina/dtsh
 Author: Chris Duf
 Author-email: chris@openmarl.org
 License: Apache License version 2.0
 Project-URL: Bug Reports, https://github.com/dottspina/dtsh/issues
 Project-URL: Source, https://github.com/dottspina/dtsh
 Keywords: devicetree,zephyr,dts,embedded
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dtsh-0.1.0a6/src/dtsh.egg-info/SOURCES.txt` & `dtsh-0.1.0b1/src/dtsh.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.py
 src/devicetree/__init__.py
+src/devicetree/_private.py
 src/devicetree/dtlib.py
 src/devicetree/edtlib.py
 src/devicetree/grutils.py
 src/dtsh/__init__.py
 src/dtsh/autocomp.py
 src/dtsh/builtin_alias.py
 src/dtsh/builtin_cat.py
```

### Comparing `dtsh-0.1.0a6/tests/test_autocomp.py` & `dtsh-0.1.0b1/tests/test_autocomp.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/tests/test_dtsh.py` & `dtsh-0.1.0b1/tests/test_dtsh.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.1.0a6/tests/test_shell.py` & `dtsh-0.1.0b1/tests/test_shell.py`

 * *Files identical despite different names*

