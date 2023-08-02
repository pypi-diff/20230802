# Comparing `tmp/yvesCMD-0.0.4.tar.gz` & `tmp/yvesCMD-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.4.tar", last modified: Wed Aug  2 15:24:26 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.5.tar", last modified: Wed Aug  2 15:27:17 2023, max compression
```

## Comparing `yvesCMD-0.0.4.tar` & `yvesCMD-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:24:26.454098 yvesCMD-0.0.4/
--rw-rw-rw-   0        0        0      203 2023-08-02 15:24:26.451106 yvesCMD-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 15:24:26.375308 yvesCMD-0.0.4/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.4/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:24:26.380295 yvesCMD-0.0.4/YvesCMD/src/
--rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.4/YvesCMD/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:24:26.433154 yvesCMD-0.0.4/YvesCMD/src/extensions/
--rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.4/YvesCMD/src/extensions/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-08-02 15:22:58.000000 yvesCMD-0.0.4/YvesCMD/src/extensions/select.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:24:26.447117 yvesCMD-0.0.4/YvesCMD/src/utils/
--rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.4/YvesCMD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.4/YvesCMD/src/utils/detector.py
--rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.4/YvesCMD/src/utils/hooks.py
--rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.4/YvesCMD/src/utils/register.py
--rw-rw-rw-   0        0        0     2518 2023-08-02 15:11:19.000000 yvesCMD-0.0.4/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-02 15:24:26.454098 yvesCMD-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-08-02 15:24:08.000000 yvesCMD-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:24:26.412330 yvesCMD-0.0.4/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      203 2023-08-02 15:24:26.000000 yvesCMD-0.0.4/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-08-02 15:24:26.000000 yvesCMD-0.0.4/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:24:26.000000 yvesCMD-0.0.4/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 15:24:26.000000 yvesCMD-0.0.4/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 15:27:17.654905 yvesCMD-0.0.5/
+-rw-rw-rw-   0        0        0      203 2023-08-02 15:27:17.652909 yvesCMD-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 15:27:17.583098 yvesCMD-0.0.5/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.5/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:27:17.590079 yvesCMD-0.0.5/YvesCMD/src/
+-rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.5/YvesCMD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:27:17.637951 yvesCMD-0.0.5/YvesCMD/src/extensions/
+-rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.5/YvesCMD/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1350 2023-08-02 15:26:11.000000 yvesCMD-0.0.5/YvesCMD/src/extensions/select.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:27:17.650915 yvesCMD-0.0.5/YvesCMD/src/utils/
+-rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.5/YvesCMD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.5/YvesCMD/src/utils/detector.py
+-rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.5/YvesCMD/src/utils/hooks.py
+-rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.5/YvesCMD/src/utils/register.py
+-rw-rw-rw-   0        0        0     2518 2023-08-02 15:11:19.000000 yvesCMD-0.0.5/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:27:17.654905 yvesCMD-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-08-02 15:27:05.000000 yvesCMD-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:27:17.619998 yvesCMD-0.0.5/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-08-02 15:27:17.000000 yvesCMD-0.0.5/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-08-02 15:27:17.000000 yvesCMD-0.0.5/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:27:17.000000 yvesCMD-0.0.5/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 15:27:17.000000 yvesCMD-0.0.5/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.4/README.md` & `yvesCMD-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.4/YvesCMD/src/extensions/select.py` & `yvesCMD-0.0.5/YvesCMD/src/extensions/select.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self.action = action
 
     def execute(self):
         self.action()
 
 
 class SelectMap:
-    select_promt: str = "[ ? ] "
+    select_promt: str = "[ ? ]"
     invalid_opt: str = "Invalid option. Please select a valid option."
     select_exit: str = "exit"
     valueErrorExcept: str = f"Invalid input. Please enter a number or exit-command to quit."
     
     def __init__(self, *selects):
         self.selects = {select.option: select for select in selects}
 
@@ -25,15 +25,15 @@
 
     def process_selection(self, option):
         if option in self.selects:
             self.selects[option].execute()
         else:
             print(self.invalid_opt)
 
-    def run(self):
+    def handle_select(self):
         self.print_options()
         while True:
             user_input = input(self.select_promt)
             if user_input == self.select_exit:
                 break
             try:
                 option = int(user_input)
```

### Comparing `yvesCMD-0.0.4/YvesCMD/src/utils/detector.py` & `yvesCMD-0.0.5/YvesCMD/src/utils/detector.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.4/YvesCMD/src/utils/hooks.py` & `yvesCMD-0.0.5/YvesCMD/src/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.4/YvesCMD/src/utils/register.py` & `yvesCMD-0.0.5/YvesCMD/src/utils/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.4/YvesCMD/src/yvescmd.py` & `yvesCMD-0.0.5/YvesCMD/src/yvescmd.py`

 * *Files identical despite different names*

