# Comparing `tmp/mazikeen-1.2.6.tar.gz` & `tmp/mazikeen-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazikeen-1.2.6.tar", last modified: Sat Jan 22 23:21:06 2022, max compression
+gzip compressed data, was "mazikeen-1.2.7.tar", last modified: Tue Aug  1 23:56:49 2023, max compression
```

## Comparing `mazikeen-1.2.6.tar` & `mazikeen-1.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 23:21:06.711841 mazikeen-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-01-22 23:20:53.000000 mazikeen-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-01-22 23:21:06.711841 mazikeen-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-01-22 23:20:53.000000 mazikeen-1.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 23:21:06.707841 mazikeen-1.2.6/mazikeen/
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/ConsolePrinter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/DiffBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorDiffBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorException.py
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorLooper.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorMakedirs.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorRmdir.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorRunBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/GeneratorUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4256 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/Loopers.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/MakedirsBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/RmdirBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)     8916 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/RunBlock.py
--rw-r--r--   0 runner    (1001) docker     (121)     6706 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/ScriptDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/ScriptReader.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/SignalHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     8071 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/Utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9512 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-22 23:20:53.000000 mazikeen-1.2.6/mazikeen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 23:21:06.711841 mazikeen-1.2.6/mazikeen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-01-22 23:21:06.000000 mazikeen-1.2.6/mazikeen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-01-22 23:21:06.000000 mazikeen-1.2.6/mazikeen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-22 23:21:06.000000 mazikeen-1.2.6/mazikeen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-01-22 23:21:06.000000 mazikeen-1.2.6/mazikeen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-01-22 23:21:06.000000 mazikeen-1.2.6/mazikeen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-22 23:21:06.000000 mazikeen-1.2.6/mazikeen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-22 23:21:06.711841 mazikeen-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-01-22 23:20:53.000000 mazikeen-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:56:49.470538 mazikeen-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 23:56:39.000000 mazikeen-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 23:56:49.470538 mazikeen-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 23:56:39.000000 mazikeen-1.2.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:56:49.470538 mazikeen-1.2.7/mazikeen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/ConsolePrinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/DiffBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorDiffBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorException.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorLooper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorMakedirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorRmdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorRunBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/GeneratorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/Loopers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/MakedirsBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/RmdirBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/RunBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/ScriptDataProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/ScriptReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/SignalHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 23:56:39.000000 mazikeen-1.2.7/mazikeen/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:56:49.470538 mazikeen-1.2.7/mazikeen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 23:56:49.000000 mazikeen-1.2.7/mazikeen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:56:49.470538 mazikeen-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-01 23:56:39.000000 mazikeen-1.2.7/setup.py
```

### Comparing `mazikeen-1.2.6/LICENSE` & `mazikeen-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/PKG-INFO` & `mazikeen-1.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazikeen
-Version: 1.2.6
+Version: 1.2.7
 Summary: Test enviroment for CLI application
 Home-page: https://github.com/hanniballar/mazikeen
 Author: Neaga Septimiu
 Author-email: neagas@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/hanniballar/mazikeen/issues
 Description: `mazikeen` is a test framework for command line applications.
```

### Comparing `mazikeen-1.2.6/README.rst` & `mazikeen-1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/ConsolePrinter.py` & `mazikeen-1.2.7/mazikeen/ConsolePrinter.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/DiffBlock.py` & `mazikeen-1.2.7/mazikeen/DiffBlock.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/GeneratorDiffBlock.py` & `mazikeen-1.2.7/mazikeen/GeneratorDiffBlock.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/GeneratorLooper.py` & `mazikeen-1.2.7/mazikeen/GeneratorLooper.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/GeneratorRunBlock.py` & `mazikeen-1.2.7/mazikeen/GeneratorRunBlock.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/GeneratorUtils.py` & `mazikeen-1.2.7/mazikeen/GeneratorUtils.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/Loopers.py` & `mazikeen-1.2.7/mazikeen/Loopers.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/RunBlock.py` & `mazikeen-1.2.7/mazikeen/RunBlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.exitcode = exitcode
         self.shell = shell
         
     def run(self, workingDir = ".", variables = {}, printer = Printer()):
 
         printer.verbose("Run:", self.cmd)
         replCmd = replaceVariables(self.cmd, variables)
-        printer.verbose("cwd:", os.getcwd())
+        printer.verbose("cwd:", os.path.abspath(workingDir))
         printer.verbose("call:", replCmd)
         cmdNArgs = shlex.split(replCmd)
 
         if self.shell == "powershell": return self.__run_powershell(replCmd, workingDir, variables, printer)
         elif self.shell == "cmd": return self.__run_cmd(replCmd, workingDir, variables, printer)
         elif self.shell == "sh": return self.__run_sh(replCmd, workingDir, variables, printer)
         elif self.shell == "python": return self.__run_pythonX(replCmd, "python", workingDir, variables, printer)
```

### Comparing `mazikeen-1.2.6/mazikeen/ScriptDataProcessor.py` & `mazikeen-1.2.7/mazikeen/ScriptDataProcessor.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/ScriptReader.py` & `mazikeen-1.2.7/mazikeen/ScriptReader.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/SignalHandler.py` & `mazikeen-1.2.7/mazikeen/SignalHandler.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/Utils.py` & `mazikeen-1.2.7/mazikeen/Utils.py`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/mazikeen/__main__.py` & `mazikeen-1.2.7/mazikeen/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from mazikeen.GeneratorLooper import generateSerialBlock, generateParallelBlock
 from mazikeen.Loopers import Serial, Parallel
 from mazikeen.ConsolePrinter import Printer, BufferedPrinter
 from mazikeen.version import __version__
 from mazikeen.Utils import ensure_dir
 from mazikeen.ScriptDataProcessor import processScriptData
 
-def getScriptFiles(dir, scriptName, maxLevel=2):
+def getScriptFiles(dir, scriptName, maxLevel=-1):
     curLevel = 0
     curLevelDirs = [Path(dir)]
     scriptFiles = []
-    while(curLevelDirs and (curLevel <= maxLevel)):
+    while(curLevelDirs and (curLevel != maxLevel)):
         nextLevelDir = []
         for curDir in curLevelDirs:
             tmpNextLevelDir = []
             dirContent = os.listdir(curDir)
             for curFile in map(lambda path: Path(curDir).joinpath(path),dirContent): 
                 if curFile.is_dir(): 
                     tmpNextLevelDir.append(curFile)
```

### Comparing `mazikeen-1.2.6/mazikeen.egg-info/PKG-INFO` & `mazikeen-1.2.7/mazikeen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazikeen
-Version: 1.2.6
+Version: 1.2.7
 Summary: Test enviroment for CLI application
 Home-page: https://github.com/hanniballar/mazikeen
 Author: Neaga Septimiu
 Author-email: neagas@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/hanniballar/mazikeen/issues
 Description: `mazikeen` is a test framework for command line applications.
```

### Comparing `mazikeen-1.2.6/mazikeen.egg-info/SOURCES.txt` & `mazikeen-1.2.7/mazikeen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mazikeen-1.2.6/setup.py` & `mazikeen-1.2.7/setup.py`

 * *Files identical despite different names*

