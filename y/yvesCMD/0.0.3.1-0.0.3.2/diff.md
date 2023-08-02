# Comparing `tmp/yvesCMD-0.0.3.1.tar.gz` & `tmp/yvesCMD-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.3.1.tar", last modified: Wed Aug  2 14:35:37 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.3.2.tar", last modified: Wed Aug  2 14:39:34 2023, max compression
```

## Comparing `yvesCMD-0.0.3.1.tar` & `yvesCMD-0.0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.362399 yvesCMD-0.0.3.1/
--rw-rw-rw-   0        0        0      205 2023-08-02 14:35:37.360405 yvesCMD-0.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.261670 yvesCMD-0.0.3.1/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.3.1/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.274634 yvesCMD-0.0.3.1/YvesCMD/src/
--rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.3.1/YvesCMD/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.340461 yvesCMD-0.0.3.1/YvesCMD/src/extensions/
--rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.3.1/YvesCMD/src/extensions/__init__.py
--rw-rw-rw-   0        0        0     1166 2023-08-02 14:28:56.000000 yvesCMD-0.0.3.1/YvesCMD/src/extensions/select.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.358411 yvesCMD-0.0.3.1/YvesCMD/src/utils/
--rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/detector.py
--rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/hooks.py
--rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/register.py
--rw-rw-rw-   0        0        0     2514 2023-08-02 13:12:42.000000 yvesCMD-0.0.3.1/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-02 14:35:37.362399 yvesCMD-0.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-08-02 14:35:32.000000 yvesCMD-0.0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.307548 yvesCMD-0.0.3.1/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      205 2023-08-02 14:35:36.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-08-02 14:35:37.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 14:35:36.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 14:35:36.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 14:39:34.605785 yvesCMD-0.0.3.2/
+-rw-rw-rw-   0        0        0      205 2023-08-02 14:39:34.604786 yvesCMD-0.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 14:39:34.520015 yvesCMD-0.0.3.2/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.3.2/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:39:34.526996 yvesCMD-0.0.3.2/YvesCMD/src/
+-rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.3.2/YvesCMD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:39:34.588830 yvesCMD-0.0.3.2/YvesCMD/src/extensions/
+-rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.3.2/YvesCMD/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1139 2023-08-02 14:39:00.000000 yvesCMD-0.0.3.2/YvesCMD/src/extensions/select.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:39:34.601795 yvesCMD-0.0.3.2/YvesCMD/src/utils/
+-rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.3.2/YvesCMD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.3.2/YvesCMD/src/utils/detector.py
+-rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.3.2/YvesCMD/src/utils/hooks.py
+-rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.3.2/YvesCMD/src/utils/register.py
+-rw-rw-rw-   0        0        0     2514 2023-08-02 13:12:42.000000 yvesCMD-0.0.3.2/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:39:34.606783 yvesCMD-0.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-08-02 14:39:31.000000 yvesCMD-0.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:39:34.565893 yvesCMD-0.0.3.2/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      205 2023-08-02 14:39:34.000000 yvesCMD-0.0.3.2/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-08-02 14:39:34.000000 yvesCMD-0.0.3.2/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:39:34.000000 yvesCMD-0.0.3.2/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 14:39:34.000000 yvesCMD-0.0.3.2/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.3.1/README.md` & `yvesCMD-0.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3.1/YvesCMD/src/extensions/select.py` & `yvesCMD-0.0.3.2/YvesCMD/src/extensions/select.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
         self.action = action
 
     def execute(self):
         self.action()
 
 
 class SelectMap:
-    select = Select()
-
     def __init__(self, *selects):
         self.selects = {select.option: select for select in selects}
 
     def print_options(self):
         for select in self.selects.values():
             print(f"[ {select.option} ] {select.description}")
 
@@ -25,15 +23,15 @@
             self.selects[option].execute()
         else:
             print("Invalid option. Please select a valid option.")
 
     def handle_select(self):
         self.print_options()
         while True:
-            user_input = input("> [ ? ] ")
+            user_input = input("[ ? ] ")
             if user_input == "exit":
                 break
             try:
                 option = int(user_input)
                 self.process_selection(option)
             except ValueError:
                 print("Invalid input. Please enter a number or 'exit' to quit.")
```

### Comparing `yvesCMD-0.0.3.1/YvesCMD/src/utils/detector.py` & `yvesCMD-0.0.3.2/YvesCMD/src/utils/detector.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3.1/YvesCMD/src/utils/hooks.py` & `yvesCMD-0.0.3.2/YvesCMD/src/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3.1/YvesCMD/src/utils/register.py` & `yvesCMD-0.0.3.2/YvesCMD/src/utils/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3.1/YvesCMD/src/yvescmd.py` & `yvesCMD-0.0.3.2/YvesCMD/src/yvescmd.py`

 * *Files identical despite different names*

