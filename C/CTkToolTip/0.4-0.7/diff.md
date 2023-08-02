# Comparing `tmp/CTkToolTip-0.4.tar.gz` & `tmp/CTkToolTip-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkToolTip-0.4.tar", last modified: Tue Jun  6 07:06:48 2023, max compression
+gzip compressed data, was "CTkToolTip-0.7.tar", last modified: Wed Aug  2 08:37:11 2023, max compression
```

## Comparing `CTkToolTip-0.4.tar` & `CTkToolTip-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:06:48.886768 CTkToolTip-0.4/
-drwxrwxrwx   0        0        0        0 2023-06-06 07:06:48.871138 CTkToolTip-0.4/CTkToolTip/
--rw-rw-rw-   0        0        0      225 2023-06-06 06:59:28.000000 CTkToolTip-0.4/CTkToolTip/__init__.py
--rw-rw-rw-   0        0        0     6239 2023-05-09 13:29:08.000000 CTkToolTip-0.4/CTkToolTip/ctk_tooltip.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:06:48.886768 CTkToolTip-0.4/CTkToolTip.egg-info/
--rw-rw-rw-   0        0        0     3673 2023-06-06 07:06:48.000000 CTkToolTip-0.4/CTkToolTip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-06-06 07:06:48.000000 CTkToolTip-0.4/CTkToolTip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:06:48.000000 CTkToolTip-0.4/CTkToolTip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 07:06:48.000000 CTkToolTip-0.4/CTkToolTip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkToolTip-0.4/LICENSE
--rw-rw-rw-   0        0        0     3673 2023-06-06 07:06:48.886768 CTkToolTip-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2023-06-06 07:05:28.000000 CTkToolTip-0.4/README.md
--rw-rw-rw-   0        0        0      575 2023-06-06 07:06:48.886768 CTkToolTip-0.4/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-06-06 07:03:47.000000 CTkToolTip-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:37:11.615525 CTkToolTip-0.7/
+drwxrwxrwx   0        0        0        0 2023-08-02 08:37:11.592204 CTkToolTip-0.7/CTkToolTip/
+-rw-rw-rw-   0        0        0      225 2023-08-02 08:35:21.000000 CTkToolTip-0.7/CTkToolTip/__init__.py
+-rw-rw-rw-   0        0        0     6727 2023-08-02 08:34:35.000000 CTkToolTip-0.7/CTkToolTip/ctk_tooltip.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:37:11.615525 CTkToolTip-0.7/CTkToolTip.egg-info/
+-rw-rw-rw-   0        0        0     3673 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 08:37:11.000000 CTkToolTip-0.7/CTkToolTip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkToolTip-0.7/LICENSE
+-rw-rw-rw-   0        0        0     3673 2023-08-02 08:37:11.615525 CTkToolTip-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2023-08-01 12:14:05.000000 CTkToolTip-0.7/README.md
+-rw-rw-rw-   0        0        0      575 2023-08-02 08:37:11.622035 CTkToolTip-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-08-02 08:36:32.000000 CTkToolTip-0.7/setup.py
```

### Comparing `CTkToolTip-0.4/CTkToolTip/ctk_tooltip.py` & `CTkToolTip-0.7/CTkToolTip/ctk_tooltip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 CTkToolTip Widget
-version: 0.4
+version: 0.7
 """
 
 import time
 import sys
 import customtkinter
 from tkinter import Toplevel, Frame
 
@@ -65,23 +65,29 @@
         self.follow = follow
         self.x_offset = x_offset
         self.y_offset = y_offset
         self.corner_radius = corner_radius
         self.alpha = alpha
         self.border_width = border_width
         self.padding = padding
-        self.bg_color = bg_color
+        self.bg_color = customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"] if bg_color is None else bg_color
         self.border_color = border_color
         self.disable = False
         
         # visibility status of the ToolTip inside|outside|visible
         self.status = "outside"
         self.last_moved = 0
         self.attributes('-alpha', self.alpha)
-        
+
+        if sys.platform.startswith("win"):
+            if self.widget._apply_appearance_mode(self.bg_color)==self.transparent_color:
+                self.transparent_color = "#000001"
+                self.config(background=self.transparent_color)
+                self.attributes("-transparentcolor", self.transparent_color)
+            
         # Add the message widget inside the tooltip
         self.transparent_frame = Frame(self, bg=self.transparent_color)
         self.transparent_frame.pack(padx=0, pady=0, fill="both", expand=True)
         
         self.frame = customtkinter.CTkFrame(self.transparent_frame, bg_color=self.transparent_color, corner_radius=self.corner_radius,
                                             border_width=self.border_width, fg_color=self.bg_color, border_color=self.border_color)
         self.frame.pack(padx=0, pady=0, fill="both", expand=True)
@@ -90,16 +96,17 @@
         self.message_label.pack(fill="both", padx=self.padding[0]+self.border_width,
                                 pady=self.padding[1]+self.border_width, expand=True)
 
         if self.widget.winfo_name()!="tk":
             if self.frame.cget("fg_color")==self.widget.cget("bg_color"):
                 if not bg_color:             
                     self._top_fg_color = self.frame._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"])
-                    self.frame.configure(fg_color=self._top_fg_color)
-  
+                    if self._top_fg_color!=self.transparent_color:
+                        self.frame.configure(fg_color=self._top_fg_color)
+        
         # Add bindings to the widget without overriding the existing ones
         self.widget.bind("<Enter>", self.on_enter, add="+")
         self.widget.bind("<Leave>", self.on_leave, add="+")
         self.widget.bind("<Motion>", self.on_enter, add="+")
         self.widget.bind("<B1-Motion>", self.on_enter, add="+")
         self.widget.bind("<Destroy>", lambda _: self.hide(), add="+")
```

### Comparing `CTkToolTip-0.4/CTkToolTip.egg-info/PKG-INFO` & `CTkToolTip-0.7/CTkToolTip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkToolTip
-Version: 0.4
+Version: 0.7
 Summary: Customtkinter Tooltip widget
 Home-page: https://github.com/Akascape/CTkToolTip
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,tooltips,popup,widgets,tkinter-widgets,tooltip popup,floating window
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkToolTip-0.4/LICENSE` & `CTkToolTip-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkToolTip-0.4/PKG-INFO` & `CTkToolTip-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkToolTip
-Version: 0.4
+Version: 0.7
 Summary: Customtkinter Tooltip widget
 Home-page: https://github.com/Akascape/CTkToolTip
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,tooltips,popup,widgets,tkinter-widgets,tooltip popup,floating window
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkToolTip-0.4/README.md` & `CTkToolTip-0.7/README.md`

 * *Files identical despite different names*

### Comparing `CTkToolTip-0.4/setup.cfg` & `CTkToolTip-0.7/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 546f 6f6c 5469 700d 0a76   = CTkToolTip..v
-00000020: 6572 7369 6f6e 203d 2030 2e34 0d0a 6465  ersion = 0.4..de
+00000020: 6572 7369 6f6e 203d 2030 2e37 0d0a 6465  ersion = 0.7..de
 00000030: 7363 7269 7074 696f 6e20 3d20 4375 7374  scription = Cust
 00000040: 6f6d 746b 696e 7465 7220 546f 6f6c 7469  omtkinter Toolti
 00000050: 700d 0a6c 6f6e 675f 6465 7363 7269 7074  p..long_descript
 00000060: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
 00000070: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 00000080: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000090: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
```

### Comparing `CTkToolTip-0.4/setup.py` & `CTkToolTip-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name='CTkToolTip',
-    version='0.4',
+    version='0.7',
     description="Customtkinter Tooltip widget",
     license="Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type="text/markdown",
     author='Akash Bora',
     url="https://github.com/Akascape/CTkToolTip",
```

