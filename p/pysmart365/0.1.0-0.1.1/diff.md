# Comparing `tmp/pysmart365-0.1.0.tar.gz` & `tmp/pysmart365-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.1.0.tar", last modified: Thu Jun 29 11:23:50 2023, max compression
+gzip compressed data, was "pysmart365-0.1.1.tar", last modified: Wed Aug  2 12:40:18 2023, max compression
```

## Comparing `pysmart365-0.1.0.tar` & `pysmart365-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 11:23:50.283623 pysmart365-0.1.0/
--rw-rw-rw-   0        0        0    35803 2023-06-02 13:24:19.000000 pysmart365-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      405 2023-06-29 11:23:50.283623 pysmart365-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-06-29 11:21:53.000000 pysmart365-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 11:23:50.257692 pysmart365-0.1.0/pysmart365/
--rw-rw-rw-   0        0        0     3102 2023-06-29 11:09:47.000000 pysmart365-0.1.0/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     2483 2023-06-29 11:13:27.000000 pysmart365-0.1.0/pysmart365/__init__.py
--rw-rw-rw-   0        0        0      633 2023-06-29 10:45:00.000000 pysmart365-0.1.0/pysmart365/modules.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:23:50.281666 pysmart365-0.1.0/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      405 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 11:23:50.000000 pysmart365-0.1.0/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 11:23:50.283623 pysmart365-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-06-29 11:15:01.000000 pysmart365-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:40:18.124909 pysmart365-0.1.1/
+-rw-rw-rw-   0        0        0    35803 2023-08-02 12:29:58.000000 pysmart365-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-08-02 12:40:18.124909 pysmart365-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-08-02 12:29:58.000000 pysmart365-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 12:40:18.097120 pysmart365-0.1.1/pysmart365/
+-rw-rw-rw-   0        0        0     3102 2023-08-02 12:29:58.000000 pysmart365-0.1.1/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     2541 2023-08-02 12:37:20.000000 pysmart365-0.1.1/pysmart365/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-08-02 12:29:58.000000 pysmart365-0.1.1/pysmart365/modules.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:40:18.121916 pysmart365-0.1.1/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-08-02 12:40:18.000000 pysmart365-0.1.1/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-08-02 12:40:18.000000 pysmart365-0.1.1/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 12:40:18.000000 pysmart365-0.1.1/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-08-02 12:40:18.000000 pysmart365-0.1.1/pysmart365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 12:40:18.000000 pysmart365-0.1.1/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 12:40:18.125906 pysmart365-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-08-02 12:37:47.000000 pysmart365-0.1.1/setup.py
```

### Comparing `pysmart365-0.1.0/LICENSE` & `pysmart365-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.1.0/README.md` & `pysmart365-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 Remember that to install the `pysmart365` module you need to install the latest python version or python versions starting from python3.
 # Last version:
 The last version is `0.1.0`
 # Documentation
 Working in progress...
 
 
-© Copyright 2023 Informatic365 - SmartSoft - MicroSoftware
+© Copyright 2023 Informatic365 - SmartSoft - MicroSoftware
```

### Comparing `pysmart365-0.1.0/pysmart365/MicroSoftware.py` & `pysmart365-0.1.1/pysmart365/MicroSoftware.py`

 * *Files identical despite different names*

### Comparing `pysmart365-0.1.0/pysmart365/__init__.py` & `pysmart365-0.1.1/pysmart365/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHOR = 'Runkang'
 COPYRIGHT = '© Copyright 2023 Informatic365 - SmartSoft - MicroSoftware'
 import subprocess
 import platform
 from customtkinter import *
 from tkinter import messagebox
 import sys
+from ttkbootstrap.dialogs import Messagebox
 
 def turn_off(time: float) -> None:
     '''
     Shutdown pc directly without gui graphics.
     '''
     if time is None or 0:
         subprocess.run(['shutdown', '-s', '-t', '0'])
@@ -48,22 +49,21 @@
     get = f'© Copyright {year} {company}'
     return get
 class close():
     def __init__(self) -> None:
         sys.exit()
 
 class wincenter():
-    def __init__(self, width, height) -> None:
-        swidth = CTk().winfo_screenwidth()
-        sheight = CTk().winfo_screenheight()
-        x = (swidth - width) // 2
-        y = (sheight - height) // 2
-        
+    def __init__(self, master, width, height) -> None:
+        swidth = master.winfo_screenwidth()
+        sheight = master.winfo_screenheight()
+        x = (swidth // 2 - width // 2)
+        y = (sheight // 2 - height // 2)
         self.set = f"{width}x{height}+{x}+{y}"
 
 class msbox():
     def showinfo(self, title, message) -> None:
-        messagebox.showinfo(title=title, message=message)
+        Messagebox.show_info(title=title, message=message)
     def showerror(self, title, message) -> None:
-        messagebox.showerror(title=title, message=message)
+        Messagebox.show_error(title=title, message=message)
     def show_warning(self, title, message):
-        messagebox.showwarning(title=title, message=message)
+        Messagebox.show_warning(title=title, message=message)
```

### Comparing `pysmart365-0.1.0/pysmart365/modules.py` & `pysmart365-0.1.1/pysmart365/modules.py`

 * *Files identical despite different names*

### Comparing `pysmart365-0.1.0/setup.py` & `pysmart365-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import *
 import webbrowser
 setup(
     author="Runkang",
     author_email="informatic3650@gmail.com",
     name="pysmart365",
     packages=['pysmart365'],
-    version='0.1.0',
+    version='0.1.1',
     long_description='''This module is to simplify the functions of MicroSoftware and SmartSoft.''',
     description='This module is to simplify the functions of MicroSoftware and SmartSoft.',
     install_requires=[
         'screeninfo',
         'pandas',
         'pyautogui',
         'pytube',
```

