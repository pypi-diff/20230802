# Comparing `tmp/abstract_gui-0.0.54.3-py3-none-any.whl.zip` & `tmp/abstract_gui-0.0.54.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9903 bytes, number of entries: 7
+Zip file size: 9861 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       28 b- defN 23-Jul-31 06:21 abstract_gui/__init__.py
--rw-r--r--  2.0 unx    24985 b- defN 23-Aug-01 21:55 abstract_gui/abstract_gui.py
+-rw-r--r--  2.0 unx    24775 b- defN 23-Aug-01 21:57 abstract_gui/abstract_gui.py
 -rw-r--r--  2.0 unx     1602 b- defN 23-Jul-31 04:07 abstract_gui/main.py
--rw-r--r--  2.0 unx    10154 b- defN 23-Aug-01 21:55 abstract_gui-0.0.54.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 21:55 abstract_gui-0.0.54.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Aug-01 21:55 abstract_gui-0.0.54.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      573 b- defN 23-Aug-01 21:55 abstract_gui-0.0.54.3.dist-info/RECORD
-7 files, 37447 bytes uncompressed, 8885 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx    10154 b- defN 23-Aug-01 21:58 abstract_gui-0.0.54.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 21:58 abstract_gui-0.0.54.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-01 21:58 abstract_gui-0.0.54.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      573 b- defN 23-Aug-01 21:58 abstract_gui-0.0.54.4.dist-info/RECORD
+7 files, 37237 bytes uncompressed, 8843 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: abstract_gui/abstract_gui.py
 Comment: 
 
 Filename: abstract_gui/main.py
 Comment: 
 
-Filename: abstract_gui-0.0.54.3.dist-info/METADATA
+Filename: abstract_gui-0.0.54.4.dist-info/METADATA
 Comment: 
 
-Filename: abstract_gui-0.0.54.3.dist-info/WHEEL
+Filename: abstract_gui-0.0.54.4.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_gui-0.0.54.3.dist-info/top_level.txt
+Filename: abstract_gui-0.0.54.4.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_gui-0.0.54.3.dist-info/RECORD
+Filename: abstract_gui-0.0.54.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_gui/abstract_gui.py

```diff
@@ -580,27 +580,25 @@
     Parameters:
     type (str): The type of GUI window to display. Defaults to 'Folder'.
     title (str): The title of the GUI window. Defaults to 'Directory'.
 
     Returns:
     dict: Returns the results of single_call function on the created GUI window.
     """
-    if 'script_name' not in globals():
-        windows_mgr,bridge,script_name=create_window_manager(script_name='default_script_name',global_var=globals())
     if type.lower() not in 'folderdirectory':
         type='File'
     else:
         type = 'Folder'
     if title == None:
         title = f'Please choose a {type.lower()}'
-    window = get_gui_fun('Window',{"title":f'{type} Explorer', "layout":[[get_gui_fun('Text',{"text":title})],
+    return get_gui_fun('Window',{"title":f'{type} Explorer', "layout":[[get_gui_fun('Text',{"text":title})],
                                                                          [get_gui_fun('Input'), get_gui_fun(f'{type}Browse',{**args,"initial_folder":initial_folder})],
                                                                          [get_gui_fun('OK'), get_gui_fun('Cancel')]]
                                    }
                          )
-    return windows_mgr.while_basic(window)['Browse']
+
 def create_window_manager(script_name='default_script_name',global_var=globals()):
     bridge = WindowGlobalBridge()
     script_name = bridge.create_script_name(script_name)
     global_var[script_name] = script_name
     bridge.retrieve_global_variables(script_name, global_var)
     return WindowManager(script_name, bridge),bridge,script_name
```

## Comparing `abstract_gui-0.0.54.3.dist-info/METADATA` & `abstract_gui-0.0.54.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.54.3
+Version: 0.0.54.4
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_gui-0.0.54.3.dist-info/RECORD` & `abstract_gui-0.0.54.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 abstract_gui/__init__.py,sha256=D-StaJ4AjH9dHP_QOd6gr4JBYGgyX8iFOTJ9gj5tiuM,28
-abstract_gui/abstract_gui.py,sha256=5uKbCbuYSx0PJ_xNILi46X6RBjWknIEEmR5Jq_UooCc,24985
+abstract_gui/abstract_gui.py,sha256=RLEQ2YDEJvbl6xi-CdXlgIdmzmaB6XlZvug35MkMFQI,24775
 abstract_gui/main.py,sha256=-5vBXHVdAuN_poGzYwcGvp1MUhUUg18z_crcDaIXWl4,1602
-abstract_gui-0.0.54.3.dist-info/METADATA,sha256=Sd33wEwIEqPGP_H_bj2NBqE3ZtJXfKtlTQeKe8St8PM,10154
-abstract_gui-0.0.54.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_gui-0.0.54.3.dist-info/top_level.txt,sha256=_lse2PkXkIfgtYuAn73RTk--wVrV_nWJ7Dn-2wK0F0E,13
-abstract_gui-0.0.54.3.dist-info/RECORD,,
+abstract_gui-0.0.54.4.dist-info/METADATA,sha256=A-GPTybERJ_R3TpTAFX1l1gMxsEtEUIL1sgVVgcopCU,10154
+abstract_gui-0.0.54.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_gui-0.0.54.4.dist-info/top_level.txt,sha256=_lse2PkXkIfgtYuAn73RTk--wVrV_nWJ7Dn-2wK0F0E,13
+abstract_gui-0.0.54.4.dist-info/RECORD,,
```

