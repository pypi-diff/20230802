# Comparing `tmp/pssepath-0.2.1.tar.gz` & `tmp/pssepath-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pssepath-0.2.1.tar", last modified: Mon Jan 25 23:54:15 2021, max compression
+gzip compressed data, was "pssepath-0.2.2.tar", last modified: Wed Aug  2 03:43:34 2023, max compression
```

## Comparing `pssepath-0.2.1.tar` & `pssepath-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-01-25 23:54:15.819294 pssepath-0.2.1/
--rw-r--r--   0 dan        (501) staff       (20)       27 2020-03-03 09:08:24.000000 pssepath-0.2.1/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)     7786 2021-01-25 23:54:15.818602 pssepath-0.2.1/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     5302 2020-03-03 11:56:41.000000 pssepath-0.2.1/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-01-25 23:54:15.802393 pssepath-0.2.1/pssepath/
--rw-r--r--   0 dan        (501) staff       (20)      150 2020-03-03 07:00:37.000000 pssepath-0.2.1/pssepath/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)       63 2021-01-25 23:50:59.000000 pssepath-0.2.1/pssepath/__version__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-01-25 23:54:15.815766 pssepath-0.2.1/pssepath/compat/
--rw-r--r--   0 dan        (501) staff       (20)      614 2020-03-02 23:15:50.000000 pssepath-0.2.1/pssepath/compat/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)       88 2020-03-02 23:15:50.000000 pssepath-0.2.1/pssepath/compat/_compat2.py
--rw-r--r--   0 dan        (501) staff       (20)       85 2020-03-02 23:15:50.000000 pssepath-0.2.1/pssepath/compat/_compat3.py
--rw-r--r--   0 dan        (501) staff       (20)    21808 2020-03-03 08:08:51.000000 pssepath-0.2.1/pssepath/core.py
--rw-r--r--   0 dan        (501) staff       (20)     3954 2021-01-25 23:49:00.000000 pssepath-0.2.1/pssepath/helpers.py
--rw-r--r--   0 dan        (501) staff       (20)      602 2020-03-03 07:01:37.000000 pssepath-0.2.1/pssepath/pssepathinfo.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-01-25 23:54:15.807488 pssepath-0.2.1/pssepath.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     7786 2021-01-25 23:54:15.000000 pssepath-0.2.1/pssepath.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      349 2021-01-25 23:54:15.000000 pssepath-0.2.1/pssepath.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2021-01-25 23:54:15.000000 pssepath-0.2.1/pssepath.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        9 2021-01-25 23:54:15.000000 pssepath-0.2.1/pssepath.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)       38 2021-01-25 23:54:15.819479 pssepath-0.2.1/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     3525 2020-03-03 09:23:40.000000 pssepath-0.2.1/setup.py
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.280082 pssepath-0.2.2/
+-rw-r--r--   0 danielhillier   (501) staff       (20)     1072 2023-08-02 03:12:39.000000 pssepath-0.2.2/LICENSE
+-rw-r--r--   0 danielhillier   (501) staff       (20)       27 2023-08-02 03:12:39.000000 pssepath-0.2.2/MANIFEST.in
+-rw-r--r--   0 danielhillier   (501) staff       (20)     6339 2023-08-02 03:43:34.279946 pssepath-0.2.2/PKG-INFO
+-rw-r--r--   0 danielhillier   (501) staff       (20)     5312 2023-08-02 03:12:39.000000 pssepath-0.2.2/README.md
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.279009 pssepath-0.2.2/pssepath/
+-rw-r--r--   0 danielhillier   (501) staff       (20)      150 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/__init__.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)       63 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/__version__.py
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.279776 pssepath-0.2.2/pssepath/compat/
+-rw-r--r--   0 danielhillier   (501) staff       (20)      614 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/compat/__init__.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)       88 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/compat/_compat2.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)       85 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/compat/_compat3.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)    22791 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/core.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)     3954 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/helpers.py
+-rw-r--r--   0 danielhillier   (501) staff       (20)      602 2023-08-02 03:12:39.000000 pssepath-0.2.2/pssepath/pssepathinfo.py
+drwxr-xr-x   0 danielhillier   (501) staff       (20)        0 2023-08-02 03:43:34.279414 pssepath-0.2.2/pssepath.egg-info/
+-rw-r--r--   0 danielhillier   (501) staff       (20)     6339 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/PKG-INFO
+-rw-r--r--   0 danielhillier   (501) staff       (20)      357 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/SOURCES.txt
+-rw-r--r--   0 danielhillier   (501) staff       (20)        1 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/dependency_links.txt
+-rw-r--r--   0 danielhillier   (501) staff       (20)        9 2023-08-02 03:43:34.000000 pssepath-0.2.2/pssepath.egg-info/top_level.txt
+-rw-r--r--   0 danielhillier   (501) staff       (20)       38 2023-08-02 03:43:34.280115 pssepath-0.2.2/setup.cfg
+-rw-r--r--   0 danielhillier   (501) staff       (20)     3525 2023-08-02 03:12:39.000000 pssepath-0.2.2/setup.py
```

### Comparing `pssepath-0.2.1/PKG-INFO` & `pssepath-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,199 +1,16 @@
 Metadata-Version: 2.1
 Name: pssepath
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simplified PSSe python importing
 Home-page: https://github.com/danifus/pssepath
 Author: Daniel Hillier
 Author-email: daniel.hillier@gmail.com
 License: MIT
-Description: 
-        pssepath - Easy PSSE Python coding
-        ====================================
-        
-        *author*: whit. (whit.com.au)
-        
-        `pssepath` simplifies the code required to setup the Python environment necessary
-        to use the PSSE API. Using `pssepath` all you have to do is::
-        
-        ```python
-            import pssepath
-            pssepath.add_pssepath()
-        
-            import psspy
-        ```
-        
-        Tested and works on:
-        
-        - PSSE 32
-        - PSSE 33
-        - PSSE 34
-        
-        Supports 32 and 64 bit windows (and provides warnings when using mismatched 64
-        bit python when PSSE requires 32 bit python).
-        
-        Using this module makes the PSSE system files available for use while avoiding
-        making modifications to system paths or hardcoding the location of the PSSE
-        system folders. This makes PSSE easy to use.
-        
-        Without `pssepath`, you have to do something like this::
-        
-        ```python
-            import os
-            import sys
-        
-            PSSE_LOCATION = r"C:\Program Files\PTI\PSSE32\PSSBIN"
-            sys.path.append(PSSE_LOCATION)
-            os.environ['PATH'] = os.environ['PATH'] + ';' +  PSSE_LOCATION
-        
-            import psspy
-        ```
-        
-        Furthermore, by including `pssepath` with any scripts you distribute, others will
-        be able to use your code without having to edit your code to suit their
-        varying install paths (such as different versions of PSSE).
-        
-        It can also provide information about which version of Python to use with a
-        particular install of PSSE to avoid `ImportError: Bad magic number...`.
-        
-        Installation
-        -------------
-        
-        `pip install pssepath`
-        
-        or copy the `pssepath` code directory (the dir that contains `core.py`) to your
-        project's root directory.
-        
-        
-        Usage
-        ------
-        `pssepath` provides 3 methods for setting up the PSSE paths:
-        
-        
-        - `pssepath.add_pssepath()`
-        
-            Adds the most recent version of PSSE that works with the currently
-            running version of Python.
-        
-        - `pssepath.add_pssepath(<version>)`
-        
-            Adds the requested version of PSSE. Remember that specifying a version
-            number may make your code less portable if you or your colleagues ever use a
-            different version.  `pssepath.add_pssepath(33)`
-        
-        - `pssepath.select_pssepath()`
-        
-            Produces a menu of all the PSSE and Python installs on your system,
-            along with the required version of Python.
-        
-        If you have set up your system to have the PSSE system files on the system path
-        at all times, `pssepath` will only use these files.
-        
-        For information about the PSSE versions installed on your system, either:
-        
-        - execute the pssepath.py file from windows; or
-        - run `python -m pssepath.pssepathinfo` You may have to specify the python
-          install path: ie. `c:\Python25\python -m pssepath.pssepathinfo` or `py.exe
-          -2.5 -m pssepath.pssepathinfo`
-        
-        This will provide you with a summary similar to the following::
-        
-        ```
-        Found the following versions of PSSE installed:
-        
-            1. PSSE version 32
-                Requires Python 2.5-32bit (Current running Python)
-            2. PSSE version XX
-                Requires Python 2.X-32bit (Installed)
-            3. PSSE version XX
-                Requires Python 2.X-32bit
-        
-        Found the following Python installations:
-          2.5-32bit (currently running):
-            PythonCore: C:\Python25\
-          3.7-64bit:
-            PythonCore: C:\Users\dan\AppData\Local\Programs\Python\Python37\
-        ```
-        
-        The status next to the Python version indicates the installation status of the
-        required Python for the particular PSSE install.
-        
-        - `Current running Python`
-        
-            indicates the Python version used to invoke the script
-            (`c:\Python25\python.exe` if invoked as `c:\Python25\python.exe -m pssepath`) is
-            appropriate for that version of PSSE.
-        
-        - `Installed`
-        
-          indicates that a Python version different to the one used to invoke the
-          script is required for that PSSE version, but that it is already installed
-          on your system.
-        
-        `<nothing>`
-        
-          The absence of a status means that a different version of Python is
-          required to run that version of PSSE and it is not installed on your
-          system. As Python comes bundled with PSSE, this status is unlikely.
-        
-        Ensuring you use the correct version of Python for the version of PSSE you are
-        running will avoid seeing `ImportError: Bad magic number...` ever again.
-        
-        License
-        --------
-        This program is released under the very permissive MIT license. You may freely
-        use it for commercial purposes, without needing to provide modified source.
-        
-        Read the LICENSE file for more information.
-        
-        Tips on managing multiple Python versions
-        -------------------------------------------
-        I like to use batch files that point to a specific python version.  For
-        example::
-        
-        ```shell
-        $ more C:\bin\python25.bat
-        @C:\Python25\python.exe %*
-        ```
-        
-        Where the PATH includes `c:\bin`.  Now you can run python scripts with the
-        command::
-        
-        ```shell
-        python25 myscript.py args
-        ```
-        
-        instead of:
-        
-        ```shell
-        c:\Python25\python.exe myscript.py args
-        ```
-        
-        Contributers
-        --------------
-        Discussion about this module was conducted at the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>) involving the following members:
-        
-        - Daniel Hillier
-        - JervisW
-        - Chip Webber
-        
-        Improvements or suggestions
-        -----------------------------
-        Visit the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>)
-        
-        See also:
-        
-        - github: https://github.com/danifus/pssepath
-        - contact: daniel@whit.com.au
-        
-        For any other questions about Python and PSSE, feel free to raise them on the
-        [Python for PSSE Forum](https://psspy.org>)
-        
 Keywords: psse extension utility pssepath
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.5
 Classifier: Programming Language :: Python :: 2.6
@@ -202,7 +19,191 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+pssepath - Easy PSSE Python coding
+====================================
+
+*author*: whit. (whit.com.au)
+
+`pssepath` simplifies the code required to setup the Python environment necessary
+to use the PSSE API. Using `pssepath` all you have to do is::
+
+```python
+    import pssepath
+    pssepath.add_pssepath()
+
+    import psspy
+```
+
+Tested and works on:
+
+- PSSE 32
+- PSSE 33
+- PSSE 34
+- PSSE 35
+
+Supports 32 and 64 bit windows (and provides warnings when using mismatched 64
+bit python when PSSE requires 32 bit python).
+
+Using this module makes the PSSE system files available for use while avoiding
+making modifications to system paths or hardcoding the location of the PSSE
+system folders. This makes PSSE easy to use.
+
+Without `pssepath`, you have to do something like this::
+
+```python
+    import os
+    import sys
+
+    PSSE_LOCATION = r"C:\Program Files\PTI\PSSE32\PSSBIN"
+    sys.path.append(PSSE_LOCATION)
+    os.environ['PATH'] = os.environ['PATH'] + ';' +  PSSE_LOCATION
+
+    import psspy
+```
+
+Furthermore, by including `pssepath` with any scripts you distribute, others will
+be able to use your code without having to edit your code to suit their
+varying install paths (such as different versions of PSSE).
+
+It can also provide information about which version of Python to use with a
+particular install of PSSE to avoid `ImportError: Bad magic number...`.
+
+Installation
+-------------
+
+`pip install pssepath`
+
+or copy the `pssepath` code directory (the dir that contains `core.py`) to your
+project's root directory.
+
+
+Usage
+------
+`pssepath` provides 3 methods for setting up the PSSE paths:
+
+
+- `pssepath.add_pssepath()`
+
+    Adds the most recent version of PSSE that works with the currently
+    running version of Python.
+
+- `pssepath.add_pssepath(<version>)`
+
+    Adds the requested version of PSSE. Remember that specifying a version
+    number may make your code less portable if you or your colleagues ever use a
+    different version.  `pssepath.add_pssepath(33)`
+
+- `pssepath.select_pssepath()`
+
+    Produces a menu of all the PSSE and Python installs on your system,
+    along with the required version of Python.
+
+If you have set up your system to have the PSSE system files on the system path
+at all times, `pssepath` will only use these files.
+
+For information about the PSSE versions installed on your system, either:
+
+- execute the pssepath.py file from windows; or
+- run `python -m pssepath.pssepathinfo` You may have to specify the python
+  install path: ie. `c:\Python25\python -m pssepath.pssepathinfo` or `py.exe
+  -2.5 -m pssepath.pssepathinfo`
+
+This will provide you with a summary similar to the following::
+
+```
+Found the following versions of PSSE installed:
+
+    1. PSSE version 32
+        Requires Python 2.5-32bit (Current running Python)
+    2. PSSE version XX
+        Requires Python 2.X-32bit (Installed)
+    3. PSSE version XX
+        Requires Python 2.X-32bit
+
+Found the following Python installations:
+  2.5-32bit (currently running):
+    PythonCore: C:\Python25\
+  3.7-64bit:
+    PythonCore: C:\Users\dan\AppData\Local\Programs\Python\Python37\
+```
+
+The status next to the Python version indicates the installation status of the
+required Python for the particular PSSE install.
+
+- `Current running Python`
+
+    indicates the Python version used to invoke the script
+    (`c:\Python25\python.exe` if invoked as `c:\Python25\python.exe -m pssepath`) is
+    appropriate for that version of PSSE.
+
+- `Installed`
+
+  indicates that a Python version different to the one used to invoke the
+  script is required for that PSSE version, but that it is already installed
+  on your system.
+
+`<nothing>`
+
+  The absence of a status means that a different version of Python is
+  required to run that version of PSSE and it is not installed on your
+  system. As Python comes bundled with PSSE, this status is unlikely.
+
+Ensuring you use the correct version of Python for the version of PSSE you are
+running will avoid seeing `ImportError: Bad magic number...` ever again.
+
+License
+--------
+This program is released under the very permissive MIT license. You may freely
+use it for commercial purposes, without needing to provide modified source.
+
+Read the LICENSE file for more information.
+
+Tips on managing multiple Python versions
+-------------------------------------------
+I like to use batch files that point to a specific python version.  For
+example::
+
+```shell
+$ more C:\bin\python25.bat
+@C:\Python25\python.exe %*
+```
+
+Where the PATH includes `c:\bin`.  Now you can run python scripts with the
+command::
+
+```shell
+python25 myscript.py args
+```
+
+instead of:
+
+```shell
+c:\Python25\python.exe myscript.py args
+```
+
+Contributers
+--------------
+Discussion about this module was conducted at the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>) involving the following members:
+
+- Daniel Hillier
+- JervisW
+- Chip Webber
+
+Improvements or suggestions
+-----------------------------
+Visit the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>)
+
+See also:
+
+- github: https://github.com/danifus/pssepath
+- contact: daniel@whit.com.au
+
+For any other questions about Python and PSSE, feel free to raise them on the
+[Python for PSSE Forum](https://psspy.org>)
```

### Comparing `pssepath-0.2.1/README.md` & `pssepath-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ```
 
 Tested and works on:
 
 - PSSE 32
 - PSSE 33
 - PSSE 34
+- PSSE 35
 
 Supports 32 and 64 bit windows (and provides warnings when using mismatched 64
 bit python when PSSE requires 32 bit python).
 
 Using this module makes the PSSE system files available for use while avoiding
 making modifications to system paths or hardcoding the location of the PSSE
 system folders. This makes PSSE easy to use.
```

### Comparing `pssepath-0.2.1/pssepath/compat/__init__.py` & `pssepath-0.2.2/pssepath/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.1/pssepath/core.py` & `pssepath-0.2.2/pssepath/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,27 +129,47 @@
 
     if psse_ver >= 34:
         # Also add the PSSBIN dir
         pssebin_dir = os.path.join(os.path.dirname(psse_path), "PSSBIN")
         sys.path.insert(0, pssebin_dir)
         os.environ["PATH"] = pssebin_dir + ";" + os.environ["PATH"]
 
+    if int(psse_ver) == 35:
+        # PSSE 35 appears to require you to run the psse35 import, 
+        # otherwise psspy fails to initialise
+        import psse35
+
 
 def search_pssbin_reg_key(pti_key):
     pssbin_paths = {}
     for sub_key in helpers.enum_reg_keys(pti_key):
         try:
+            # First, try the v34 registry format of PTI\PSSE 34\Product Paths
             with open_hkey_ctxmg(pti_key, sub_key + "\\Product Paths") as ver_key:
                 # Version num is the last 2 digits of the subkey
                 version_num = int(sub_key[-2:])
                 pssbin_paths[version_num] = helpers.get_reg_value(
                     ver_key, "PsseExePath"
                 )
         except WindowsError:
             pass
+
+        # Next, try the v35 registry format of PTI\PSSE 35\5\Product Paths (for 35.5)
+        with open_hkey_ctxmg(pti_key, sub_key) as ver_key:
+            for point_ver_key in helpers.enum_reg_keys(ver_key):
+                try:
+                    # Version num is the last 2 digits of the subkey (35) plus the point version (.5)
+                    with open_hkey_ctxmg(ver_key, point_ver_key + "\\Product Paths") as point_ver_hkey:
+                        version_num = float(sub_key[-2:] + "." + point_ver_key)
+                        pssbin_paths[version_num] = helpers.get_reg_value(
+                            point_ver_hkey, "PsseExePath"
+                        )
+                except WindowsError:
+                    pass
+
     return pssbin_paths
 
 
 @helpers.memoize
 def get_pssbin_paths_dict():
     pssbin_paths = {}
     if helpers.is_win64():
@@ -326,15 +346,15 @@
     installed_py_vers = get_installed_py_vers()
     for i, (psse_ver, pyver) in options.items():
         python_str = "Requires Python%s" % ("-".join(pyver),)
         if pyver == running_py_ver:
             python_str += " (Current running Python)"
         elif running_py_ver in installed_py_vers:
             python_str += " (Installed, not current running version.)"
-        simple_print("  %i. PSSE Version %d\n      %s" % (i, psse_ver, python_str))
+        simple_print("  %i. PSSE Version %s\n      %s" % (i, psse_ver, python_str))
     return options
 
 
 def print_python_selection():
     python_by_paths = get_pythons_by_location()
     python_paths = {}
     for path, vals in python_by_paths.items():
```

### Comparing `pssepath-0.2.1/pssepath/helpers.py` & `pssepath-0.2.2/pssepath/helpers.py`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.1/pssepath/pssepathinfo.py` & `pssepath-0.2.2/pssepath/pssepathinfo.py`

 * *Files identical despite different names*

### Comparing `pssepath-0.2.1/pssepath.egg-info/PKG-INFO` & `pssepath-0.2.2/pssepath.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,199 +1,16 @@
 Metadata-Version: 2.1
 Name: pssepath
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simplified PSSe python importing
 Home-page: https://github.com/danifus/pssepath
 Author: Daniel Hillier
 Author-email: daniel.hillier@gmail.com
 License: MIT
-Description: 
-        pssepath - Easy PSSE Python coding
-        ====================================
-        
-        *author*: whit. (whit.com.au)
-        
-        `pssepath` simplifies the code required to setup the Python environment necessary
-        to use the PSSE API. Using `pssepath` all you have to do is::
-        
-        ```python
-            import pssepath
-            pssepath.add_pssepath()
-        
-            import psspy
-        ```
-        
-        Tested and works on:
-        
-        - PSSE 32
-        - PSSE 33
-        - PSSE 34
-        
-        Supports 32 and 64 bit windows (and provides warnings when using mismatched 64
-        bit python when PSSE requires 32 bit python).
-        
-        Using this module makes the PSSE system files available for use while avoiding
-        making modifications to system paths or hardcoding the location of the PSSE
-        system folders. This makes PSSE easy to use.
-        
-        Without `pssepath`, you have to do something like this::
-        
-        ```python
-            import os
-            import sys
-        
-            PSSE_LOCATION = r"C:\Program Files\PTI\PSSE32\PSSBIN"
-            sys.path.append(PSSE_LOCATION)
-            os.environ['PATH'] = os.environ['PATH'] + ';' +  PSSE_LOCATION
-        
-            import psspy
-        ```
-        
-        Furthermore, by including `pssepath` with any scripts you distribute, others will
-        be able to use your code without having to edit your code to suit their
-        varying install paths (such as different versions of PSSE).
-        
-        It can also provide information about which version of Python to use with a
-        particular install of PSSE to avoid `ImportError: Bad magic number...`.
-        
-        Installation
-        -------------
-        
-        `pip install pssepath`
-        
-        or copy the `pssepath` code directory (the dir that contains `core.py`) to your
-        project's root directory.
-        
-        
-        Usage
-        ------
-        `pssepath` provides 3 methods for setting up the PSSE paths:
-        
-        
-        - `pssepath.add_pssepath()`
-        
-            Adds the most recent version of PSSE that works with the currently
-            running version of Python.
-        
-        - `pssepath.add_pssepath(<version>)`
-        
-            Adds the requested version of PSSE. Remember that specifying a version
-            number may make your code less portable if you or your colleagues ever use a
-            different version.  `pssepath.add_pssepath(33)`
-        
-        - `pssepath.select_pssepath()`
-        
-            Produces a menu of all the PSSE and Python installs on your system,
-            along with the required version of Python.
-        
-        If you have set up your system to have the PSSE system files on the system path
-        at all times, `pssepath` will only use these files.
-        
-        For information about the PSSE versions installed on your system, either:
-        
-        - execute the pssepath.py file from windows; or
-        - run `python -m pssepath.pssepathinfo` You may have to specify the python
-          install path: ie. `c:\Python25\python -m pssepath.pssepathinfo` or `py.exe
-          -2.5 -m pssepath.pssepathinfo`
-        
-        This will provide you with a summary similar to the following::
-        
-        ```
-        Found the following versions of PSSE installed:
-        
-            1. PSSE version 32
-                Requires Python 2.5-32bit (Current running Python)
-            2. PSSE version XX
-                Requires Python 2.X-32bit (Installed)
-            3. PSSE version XX
-                Requires Python 2.X-32bit
-        
-        Found the following Python installations:
-          2.5-32bit (currently running):
-            PythonCore: C:\Python25\
-          3.7-64bit:
-            PythonCore: C:\Users\dan\AppData\Local\Programs\Python\Python37\
-        ```
-        
-        The status next to the Python version indicates the installation status of the
-        required Python for the particular PSSE install.
-        
-        - `Current running Python`
-        
-            indicates the Python version used to invoke the script
-            (`c:\Python25\python.exe` if invoked as `c:\Python25\python.exe -m pssepath`) is
-            appropriate for that version of PSSE.
-        
-        - `Installed`
-        
-          indicates that a Python version different to the one used to invoke the
-          script is required for that PSSE version, but that it is already installed
-          on your system.
-        
-        `<nothing>`
-        
-          The absence of a status means that a different version of Python is
-          required to run that version of PSSE and it is not installed on your
-          system. As Python comes bundled with PSSE, this status is unlikely.
-        
-        Ensuring you use the correct version of Python for the version of PSSE you are
-        running will avoid seeing `ImportError: Bad magic number...` ever again.
-        
-        License
-        --------
-        This program is released under the very permissive MIT license. You may freely
-        use it for commercial purposes, without needing to provide modified source.
-        
-        Read the LICENSE file for more information.
-        
-        Tips on managing multiple Python versions
-        -------------------------------------------
-        I like to use batch files that point to a specific python version.  For
-        example::
-        
-        ```shell
-        $ more C:\bin\python25.bat
-        @C:\Python25\python.exe %*
-        ```
-        
-        Where the PATH includes `c:\bin`.  Now you can run python scripts with the
-        command::
-        
-        ```shell
-        python25 myscript.py args
-        ```
-        
-        instead of:
-        
-        ```shell
-        c:\Python25\python.exe myscript.py args
-        ```
-        
-        Contributers
-        --------------
-        Discussion about this module was conducted at the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>) involving the following members:
-        
-        - Daniel Hillier
-        - JervisW
-        - Chip Webber
-        
-        Improvements or suggestions
-        -----------------------------
-        Visit the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>)
-        
-        See also:
-        
-        - github: https://github.com/danifus/pssepath
-        - contact: daniel@whit.com.au
-        
-        For any other questions about Python and PSSE, feel free to raise them on the
-        [Python for PSSE Forum](https://psspy.org>)
-        
 Keywords: psse extension utility pssepath
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.5
 Classifier: Programming Language :: Python :: 2.6
@@ -202,7 +19,191 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+pssepath - Easy PSSE Python coding
+====================================
+
+*author*: whit. (whit.com.au)
+
+`pssepath` simplifies the code required to setup the Python environment necessary
+to use the PSSE API. Using `pssepath` all you have to do is::
+
+```python
+    import pssepath
+    pssepath.add_pssepath()
+
+    import psspy
+```
+
+Tested and works on:
+
+- PSSE 32
+- PSSE 33
+- PSSE 34
+- PSSE 35
+
+Supports 32 and 64 bit windows (and provides warnings when using mismatched 64
+bit python when PSSE requires 32 bit python).
+
+Using this module makes the PSSE system files available for use while avoiding
+making modifications to system paths or hardcoding the location of the PSSE
+system folders. This makes PSSE easy to use.
+
+Without `pssepath`, you have to do something like this::
+
+```python
+    import os
+    import sys
+
+    PSSE_LOCATION = r"C:\Program Files\PTI\PSSE32\PSSBIN"
+    sys.path.append(PSSE_LOCATION)
+    os.environ['PATH'] = os.environ['PATH'] + ';' +  PSSE_LOCATION
+
+    import psspy
+```
+
+Furthermore, by including `pssepath` with any scripts you distribute, others will
+be able to use your code without having to edit your code to suit their
+varying install paths (such as different versions of PSSE).
+
+It can also provide information about which version of Python to use with a
+particular install of PSSE to avoid `ImportError: Bad magic number...`.
+
+Installation
+-------------
+
+`pip install pssepath`
+
+or copy the `pssepath` code directory (the dir that contains `core.py`) to your
+project's root directory.
+
+
+Usage
+------
+`pssepath` provides 3 methods for setting up the PSSE paths:
+
+
+- `pssepath.add_pssepath()`
+
+    Adds the most recent version of PSSE that works with the currently
+    running version of Python.
+
+- `pssepath.add_pssepath(<version>)`
+
+    Adds the requested version of PSSE. Remember that specifying a version
+    number may make your code less portable if you or your colleagues ever use a
+    different version.  `pssepath.add_pssepath(33)`
+
+- `pssepath.select_pssepath()`
+
+    Produces a menu of all the PSSE and Python installs on your system,
+    along with the required version of Python.
+
+If you have set up your system to have the PSSE system files on the system path
+at all times, `pssepath` will only use these files.
+
+For information about the PSSE versions installed on your system, either:
+
+- execute the pssepath.py file from windows; or
+- run `python -m pssepath.pssepathinfo` You may have to specify the python
+  install path: ie. `c:\Python25\python -m pssepath.pssepathinfo` or `py.exe
+  -2.5 -m pssepath.pssepathinfo`
+
+This will provide you with a summary similar to the following::
+
+```
+Found the following versions of PSSE installed:
+
+    1. PSSE version 32
+        Requires Python 2.5-32bit (Current running Python)
+    2. PSSE version XX
+        Requires Python 2.X-32bit (Installed)
+    3. PSSE version XX
+        Requires Python 2.X-32bit
+
+Found the following Python installations:
+  2.5-32bit (currently running):
+    PythonCore: C:\Python25\
+  3.7-64bit:
+    PythonCore: C:\Users\dan\AppData\Local\Programs\Python\Python37\
+```
+
+The status next to the Python version indicates the installation status of the
+required Python for the particular PSSE install.
+
+- `Current running Python`
+
+    indicates the Python version used to invoke the script
+    (`c:\Python25\python.exe` if invoked as `c:\Python25\python.exe -m pssepath`) is
+    appropriate for that version of PSSE.
+
+- `Installed`
+
+  indicates that a Python version different to the one used to invoke the
+  script is required for that PSSE version, but that it is already installed
+  on your system.
+
+`<nothing>`
+
+  The absence of a status means that a different version of Python is
+  required to run that version of PSSE and it is not installed on your
+  system. As Python comes bundled with PSSE, this status is unlikely.
+
+Ensuring you use the correct version of Python for the version of PSSE you are
+running will avoid seeing `ImportError: Bad magic number...` ever again.
+
+License
+--------
+This program is released under the very permissive MIT license. You may freely
+use it for commercial purposes, without needing to provide modified source.
+
+Read the LICENSE file for more information.
+
+Tips on managing multiple Python versions
+-------------------------------------------
+I like to use batch files that point to a specific python version.  For
+example::
+
+```shell
+$ more C:\bin\python25.bat
+@C:\Python25\python.exe %*
+```
+
+Where the PATH includes `c:\bin`.  Now you can run python scripts with the
+command::
+
+```shell
+python25 myscript.py args
+```
+
+instead of:
+
+```shell
+c:\Python25\python.exe myscript.py args
+```
+
+Contributers
+--------------
+Discussion about this module was conducted at the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>) involving the following members:
+
+- Daniel Hillier
+- JervisW
+- Chip Webber
+
+Improvements or suggestions
+-----------------------------
+Visit the [Python for PSSE Forum](https://psspy.org/psse-help-forum/question/3/how-do-i-import-the-psspy-module-in-a-python>)
+
+See also:
+
+- github: https://github.com/danifus/pssepath
+- contact: daniel@whit.com.au
+
+For any other questions about Python and PSSE, feel free to raise them on the
+[Python for PSSE Forum](https://psspy.org>)
```

### Comparing `pssepath-0.2.1/setup.py` & `pssepath-0.2.2/setup.py`

 * *Files identical despite different names*

