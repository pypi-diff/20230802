# Comparing `tmp/cmdhelper-0.3.0.tar.gz` & `tmp/cmdhelper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmdhelper-0.3.0.tar", last modified: Mon Oct  3 05:00:04 2022, max compression
+gzip compressed data, was "dist/cmdhelper-0.3.1.tar", last modified: Wed Aug  2 00:02:17 2023, max compression
```

## Comparing `cmdhelper-0.3.0.tar` & `cmdhelper-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/
--rw-r--r--   0 jb        (1000) users      (100)     1090 2015-05-18 05:30:53.000000 cmdhelper-0.3.0/LICENSE
--rw-r--r--   0 jb        (1000) users      (100)       22 2015-05-20 00:44:40.000000 cmdhelper-0.3.0/MANIFEST.in
--rw-r--r--   0 jb        (1000) users      (100)     4611 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/PKG-INFO
--rw-r--r--   0 jb        (1000) users      (100)     3221 2016-04-26 21:04:59.000000 cmdhelper-0.3.0/README.rst
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/cmdhelper.egg-info/
--rw-r--r--   0 jb        (1000) users      (100)     4611 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/cmdhelper.egg-info/PKG-INFO
--rw-r--r--   0 jb        (1000) users      (100)      244 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/cmdhelper.egg-info/SOURCES.txt
--rw-r--r--   0 jb        (1000) users      (100)        1 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/cmdhelper.egg-info/dependency_links.txt
--rw-r--r--   0 jb        (1000) users      (100)       46 2016-06-02 05:08:29.000000 cmdhelper-0.3.0/cmdhelper.egg-info/pbr.json
--rw-r--r--   0 jb        (1000) users      (100)        7 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/cmdhelper.egg-info/requires.txt
--rw-r--r--   0 jb        (1000) users      (100)       10 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/cmdhelper.egg-info/top_level.txt
--rwxr-xr-x   0 jb        (1000) users      (100)    30832 2022-10-03 01:51:47.000000 cmdhelper-0.3.0/cmdhelper.py
--rw-r--r--   0 jb        (1000) users      (100)       38 2022-10-03 05:00:04.000000 cmdhelper-0.3.0/setup.cfg
--rw-r--r--   0 jb        (1000) users      (100)     1032 2022-10-03 01:56:21.000000 cmdhelper-0.3.0/setup.py
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/
+-rw-r--r--   0 jb        (1000) users      (100)     1090 2023-08-01 23:54:39.000000 cmdhelper-0.3.1/LICENSE
+-rw-r--r--   0 jb        (1000) users      (100)       22 2015-05-20 00:44:40.000000 cmdhelper-0.3.1/MANIFEST.in
+-rw-r--r--   0 jb        (1000) users      (100)     4611 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/PKG-INFO
+-rw-r--r--   0 jb        (1000) users      (100)     3221 2016-04-26 21:04:59.000000 cmdhelper-0.3.1/README.rst
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/cmdhelper.egg-info/
+-rw-r--r--   0 jb        (1000) users      (100)     4611 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/cmdhelper.egg-info/PKG-INFO
+-rw-r--r--   0 jb        (1000) users      (100)      244 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/cmdhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 jb        (1000) users      (100)        1 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/cmdhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 jb        (1000) users      (100)       46 2016-06-02 05:08:29.000000 cmdhelper-0.3.1/cmdhelper.egg-info/pbr.json
+-rw-r--r--   0 jb        (1000) users      (100)        7 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/cmdhelper.egg-info/requires.txt
+-rw-r--r--   0 jb        (1000) users      (100)       10 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/cmdhelper.egg-info/top_level.txt
+-rwxr-xr-x   0 jb        (1000) users      (100)    31965 2023-08-01 23:04:19.000000 cmdhelper-0.3.1/cmdhelper.py
+-rw-r--r--   0 jb        (1000) users      (100)       38 2023-08-02 00:02:17.000000 cmdhelper-0.3.1/setup.cfg
+-rw-r--r--   0 jb        (1000) users      (100)     1032 2023-08-01 23:04:19.000000 cmdhelper-0.3.1/setup.py
```

### Comparing `cmdhelper-0.3.0/LICENSE` & `cmdhelper-0.3.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2014-2015 Juerg Beringer (juerg.beringer@gmail.com)
+Copyright (c) 2014-2023 Juerg Beringer (juerg.beringer@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cmdhelper-0.3.0/PKG-INFO` & `cmdhelper-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cmdhelper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python utility for writing command line scripts with consistent look and feel.
 Home-page: https://github.com/juergberinger/cmdhelper
 Author: Juerg Beringer
 Author-email: juerg.beringer@gmail.com
 License: MIT
 Description: cmdhelper
         =========
```

### Comparing `cmdhelper-0.3.0/README.rst` & `cmdhelper-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `cmdhelper-0.3.0/cmdhelper.egg-info/PKG-INFO` & `cmdhelper-0.3.1/cmdhelper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cmdhelper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python utility for writing command line scripts with consistent look and feel.
 Home-page: https://github.com/juergberinger/cmdhelper
 Author: Juerg Beringer
 Author-email: juerg.beringer@gmail.com
 License: MIT
 Description: cmdhelper
         =========
```

### Comparing `cmdhelper-0.3.0/cmdhelper.py` & `cmdhelper-0.3.1/cmdhelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Python 2/3 compatibility
 from __future__ import print_function
 from builtins import input
 from builtins import str
 from builtins import range
 
 __author__ = 'Juerg Beringer'
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 __all__ = ['CmdHelper', 'CmdError', 'cmdLine', 'handleError',
            'debug', 'warning', 'info', 'error', 'critical',
            'confirm', 'run', 'abort', 'enableHistory']
 
 import sys
 import os
@@ -139,15 +139,27 @@
         self.abortOnIOError = abortOnIOError
 
     def emit(self, record):
         """Emit a record. Unless record.terminator is set, a trailing
            newline will be written to the output stream."""
         try:
             msg = self.format(record)
-            self.stream.write(msg)
+            if sys.version_info.major == 2:
+                # Python 2 fix for UnicodeEncodeError in case of unicode characters in log messages
+                if isinstance(msg, unicode):
+                    if hasattr(self.stream, "encoding") and self.stream.encoding:
+                        # Stream should take care of encoding, but do it explicitly to prevent bug in Python 2.6 - see
+                        # https://stackoverflow.com/questions/8016236/python-unicode-handling-differences-between-print-and-sys-stdout-write
+                        self.stream.write(msg.encode(self.stream.encoding))
+                    else:
+                        self.stream.write(msg.encode(encoding))
+                else:
+                    self.stream.write(msg)
+            else:
+                self.stream.write(msg)
             terminator = getattr(record, 'terminator', '\n')
             if terminator is not None:
                 self.stream.write(terminator)
             self.flush()
         except (KeyboardInterrupt, SystemExit):
             raise
         except Exception:
@@ -307,15 +319,15 @@
             return 1 if record.levelno in self.levelList else 0
 
 
 class CmdHelper:
 
     """CmdHelper class to setup option parsing and logging.
 
-    The constructs accepts the following parameters:
+    The constructor accepts the following parameters:
 
     parseTool          Must be present, and must be either 'optparse'
                        or 'argparse' for using optparse.OptionParser
                        or argparse.ArgumentParser, respectively.
 
     version            Version info.
 
@@ -335,14 +347,16 @@
     hasInteractive     Whether to add -i option to go to an interactive
                        Python shell after script completion.
 
     hasBatch           Whether to add --batch option.
 
     hasDryRun          Whether to add --dryrun option.
 
+    hasCommit          Whether to add --commit option.
+
     logFile            Default log file.
 
     logSeparator       Default string to separate logs from different
                        invocation of the script.
 
     logTimestampFmt    Default time stamp format.
 
@@ -350,28 +364,29 @@
     by either directly calling the OptionParser or ArgumentParser
     object via CmdHelper.parser, or using the utility methods
     CmdHelper.add_option and CmdHelper.add_argument."""
 
     def __init__(self, parseTool, version=None,
                  description=None, epilog=None,
                  redirectStdOut=True, separateStdErr=True, hasLogFile=True, hasEmail=True,
-                 hasInteractive=True, hasBatch=False, hasDryRun=False,
+                 hasInteractive=True, hasBatch=False, hasDryRun=False, hasCommit=False,
                  logFile='', logSeparator=None, logTimestampFmt=None):
         if parseTool not in ('optparse', 'argparse'):
             raise ValueError('parseTool must be either "optparse" or "argparse"')
         self.parseTool = parseTool
         self.version = version
         self.description = description
         self.epilog = epilog
         self.redirectStdOut = redirectStdOut
         self.separateStdErr = separateStdErr
         self.hasLogFile = hasLogFile
         self.hasInteractive = hasInteractive
         self.hasBatch = hasBatch
         self.hasDryRun = hasDryRun
+        self.hasCommit = hasCommit
         self.logFile = logFile
         self.logSeparator = logSeparator
         self.logTimestampFmt = logTimestampFmt
 
         self.historyPath = "~/.cmdhelper_history"   # default history path, set to None to disable history
         self.consoleHandler = None
         self.errorHandler = None
@@ -399,14 +414,18 @@
         self.add_option('', '--debug', dest='debug',
                         action='store_true', default=False,
                         help='debugging output')
         if hasDryRun:
             self.add_option('', '--dryrun', dest='dryrun',
                             action='store_true', default=False,
                             help='only show what would be done without --dryrun')
+        if hasCommit:
+            self.add_option('', '--commit', dest='commit',
+                            action='store_true', default=False,
+                            help='commit changes rather than showing only what would be done')
         if hasBatch:
             self.add_option('', '--batch', dest='batch',
                             action='store_true', default=False,
                             help='batch mode (skips confirmations)')
         if hasLogFile:
             self.add_option('', '--noscreen', dest='noscreen',
                             action='store_true', default=False,
```

### Comparing `cmdhelper-0.3.0/setup.py` & `cmdhelper-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def read(fname):
     """Return contents of file with name fname."""
     with open(fname, 'r') as f:
         return f.read()
 
 setup(
     name = 'cmdhelper',
-    version = '0.3.0',
+    version = '0.3.1',
     description = 'Python utility for writing command line scripts with consistent look and feel.',
     long_description = read('README.rst'),
     url = 'https://github.com/juergberinger/cmdhelper',
     license = 'MIT',
     author = 'Juerg Beringer',
     author_email = 'juerg.beringer@gmail.com',
     py_modules = ['cmdhelper'],
```

