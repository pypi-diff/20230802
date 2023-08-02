# Comparing `tmp/pmenu_lib-1.1.2.tar.gz` & `tmp/pmenu_lib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmenu_lib-1.1.2.tar", last modified: Wed Jul 26 17:25:29 2023, max compression
+gzip compressed data, was "pmenu_lib-1.1.3.tar", last modified: Wed Aug  2 11:09:54 2023, max compression
```

## Comparing `pmenu_lib-1.1.2.tar` & `pmenu_lib-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1070 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      716 2023-07-26 17:25:03.000000 pmenu_lib-1.1.2/README.md
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/pmenu_lib/
--rw-rw-r--   0 omega     (1000) omega     (1000)       29 2023-07-26 10:03:29.000000 pmenu_lib-1.1.2/pmenu_lib/__init__.py
--rw-rw-r--   0 omega     (1000) omega     (1000)     3755 2023-07-26 17:05:55.000000 pmenu_lib-1.1.2/pmenu_lib/pmenu_lib.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/pmenu_lib.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1070 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      195 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       10 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/top_level.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      506 2023-07-26 17:25:07.000000 pmenu_lib-1.1.2/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-08-02 11:09:54.980774 pmenu_lib-1.1.3/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1070 2023-08-02 11:09:54.980774 pmenu_lib-1.1.3/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      716 2023-07-26 17:25:03.000000 pmenu_lib-1.1.3/README.md
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-08-02 11:09:54.980774 pmenu_lib-1.1.3/pmenu_lib/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       29 2023-07-26 10:03:29.000000 pmenu_lib-1.1.3/pmenu_lib/__init__.py
+-rw-rw-r--   0 omega     (1000) omega     (1000)     3755 2023-08-02 11:07:48.000000 pmenu_lib-1.1.3/pmenu_lib/pmenu_lib.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-08-02 11:09:54.980774 pmenu_lib-1.1.3/pmenu_lib.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1070 2023-08-02 11:09:54.000000 pmenu_lib-1.1.3/pmenu_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      195 2023-08-02 11:09:54.000000 pmenu_lib-1.1.3/pmenu_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-08-02 11:09:54.000000 pmenu_lib-1.1.3/pmenu_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       10 2023-08-02 11:09:54.000000 pmenu_lib-1.1.3/pmenu_lib.egg-info/top_level.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-08-02 11:09:54.980774 pmenu_lib-1.1.3/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      506 2023-08-02 11:07:35.000000 pmenu_lib-1.1.3/setup.py
```

### Comparing `pmenu_lib-1.1.2/PKG-INFO` & `pmenu_lib-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmenu_lib
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sleek dmenu alternative written in Python and powered by curses.
 Home-page: https://github.com/Julynx/pmenu
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `pmenu_lib-1.1.2/README.md` & `pmenu_lib-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pmenu_lib-1.1.2/pmenu_lib/pmenu_lib.py` & `pmenu_lib-1.1.3/pmenu_lib/pmenu_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @file     pmenu_lib.py
 @brief    Sleek dmenu alternative written in Python and powered by curses.
-@date     26/07/2023
+@date     02/08/2023
 @author   Julio Cabria
 """
 
 
 import curses
 from contextlib import suppress
 
@@ -116,15 +116,15 @@
         row (int): The index of the row to highlight.
         query (str): The query to display.
 
     Returns:
         tuple: The start row and the max display rows.
     """
     max_rows, _ = screen.getmaxyx()
-    max_display_rows = min(max_rows - 2, len(lines))
+    max_display_rows = min(max_rows - 1, len(lines))
 
     start_row = max(0, row - max_display_rows + 1)
     end_row = min(start_row + max_display_rows, len(lines))
 
     for i, line in enumerate(lines[start_row:end_row], start=start_row):
         with suppress(curses.error):
             if i == row:
```

### Comparing `pmenu_lib-1.1.2/pmenu_lib.egg-info/PKG-INFO` & `pmenu_lib-1.1.3/pmenu_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmenu-lib
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sleek dmenu alternative written in Python and powered by curses.
 Home-page: https://github.com/Julynx/pmenu
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

