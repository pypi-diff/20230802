# Comparing `tmp/abstract_gui-0.0.54.82-py3-none-any.whl.zip` & `tmp/abstract_gui-0.0.54.83-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10530 bytes, number of entries: 7
+Zip file size: 10662 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       28 b- defN 23-Jul-31 06:21 abstract_gui/__init__.py
--rw-r--r--  2.0 unx    28030 b- defN 23-Aug-02 00:30 abstract_gui/abstract_gui.py
+-rw-r--r--  2.0 unx    28715 b- defN 23-Aug-02 03:28 abstract_gui/abstract_gui.py
 -rw-r--r--  2.0 unx     1602 b- defN 23-Jul-31 04:07 abstract_gui/main.py
--rw-r--r--  2.0 unx    10155 b- defN 23-Aug-02 00:43 abstract_gui-0.0.54.82.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 00:43 abstract_gui-0.0.54.82.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Aug-02 00:43 abstract_gui-0.0.54.82.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      577 b- defN 23-Aug-02 00:43 abstract_gui-0.0.54.82.dist-info/RECORD
-7 files, 40497 bytes uncompressed, 9504 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx    10155 b- defN 23-Aug-02 03:32 abstract_gui-0.0.54.83.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 03:32 abstract_gui-0.0.54.83.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-02 03:32 abstract_gui-0.0.54.83.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      577 b- defN 23-Aug-02 03:32 abstract_gui-0.0.54.83.dist-info/RECORD
+7 files, 41182 bytes uncompressed, 9636 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: abstract_gui/abstract_gui.py
 Comment: 
 
 Filename: abstract_gui/main.py
 Comment: 
 
-Filename: abstract_gui-0.0.54.82.dist-info/METADATA
+Filename: abstract_gui-0.0.54.83.dist-info/METADATA
 Comment: 
 
-Filename: abstract_gui-0.0.54.82.dist-info/WHEEL
+Filename: abstract_gui-0.0.54.83.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_gui-0.0.54.82.dist-info/top_level.txt
+Filename: abstract_gui-0.0.54.83.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_gui-0.0.54.82.dist-info/RECORD
+Filename: abstract_gui-0.0.54.83.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_gui/abstract_gui.py

```diff
@@ -506,29 +506,30 @@
 def if_not_window_make_window(window):
     if isinstance(window, type(get_window())) == False:
         if isinstance(window, dict):
             if "layout" in window:
                 window["layout"]=ensure_nested_list(window["layout"])
         window=get_window(args=window)
     return window
-def while_quick(window,return_events:(list or str)=[],exit_events:(list or str)=[sg.WIN_CLOSED]):
+def while_quick(window,return_events:(list or str)=[],exit_events:(list or str)=[sg.WIN_CLOSED],event_return=False):
     exit_events = make_list_add(exit_events,[sg.WIN_CLOSED])
     return_events = list(return_events)
     last_values=[]
     while True:
         event, values = window.read()
         if event ==sg.WIN_CLOSED:
             window.close()
-            
             values= None
             break
         elif event in return_events:
             window.close()
             break
-    return values     
+    if event_return == True:
+        return event
+    return values  
       
 def verify_args(args:dict=None, layout:list=None, title:str=None, event_function:str=None,exit_events:(list or str)=None):
         args = args or {}
         layout = layout or [[]]
         title = title or 'window'
         exit_events = exit_events or ["exit", "Exit", "EXIT"]
         args.setdefault("title", title)
@@ -569,14 +570,20 @@
         title = f'Please choose a {type.lower()}'
     layout = [
         [get_gui_fun('Text', {"text": title})],
         [get_gui_fun('Input',args={"default":initial_folder,"key":"output"}), get_gui_fun(f'{type}Browse', {**args, "initial_folder": initial_folder})],
         [get_gui_fun('OK'), get_gui_fun('Cancel')]
     ]
     return {"title": f'{type} Explorer', "layout": layout}
+def get_yes_no_layout(title:str="Answer Window",text:str="would you lie to proceed?",args:dict={}):
+    layout = [
+        [get_gui_fun('Text', {"text": text})],
+        [sg.Button('Yes'), sg.Button('No')]
+    ]
+    return {"title":title, "layout": layout,**args}
 def get_input_layout(title:str="Input Window",text:str="please enter your input",default:str=None,args:dict={}):
     """
     Function to get a browser GUI based on the type specified.
 
     Parameters:
     type (str): The type of GUI window to display. Defaults to 'Folder'.
     title (str): The title of the GUI window. Defaults to 'Directory'.
@@ -598,14 +605,17 @@
         text = args["text"]
     layout = [
         [get_gui_fun('Text', {"text": text})],
         [get_gui_fun('Input',args=args)],
         [get_gui_fun('OK'), get_gui_fun('Cancel')]
     ]
     return {"title":title, "layout": layout}
+def get_yes_no(title:str="Answer Window",text:str="would you lie to proceed?",args:dict={},exit_events:(str or list)=[],return_events:(str or list)=["Yes","No"],event_return=True):
+    window = get_window(args=get_yes_no_layout(title=title,text=text))
+    return while_quick(window=window,exit_events=exit_events,return_events=return_events,event_return=event_return)
 def get_input(title:str="Input Window",text:str="please enter your input",default:str=None,args:dict={},exit_events:(str or list)=['Cancel'],return_events:(str or list)=['OK']):
     window = get_window(args=get_input_layout(title=title,text=text,args=args,default=default,initial_folder=initial_folder))
     return while_quick(window=window,exit_events=exit_events,return_events=return_events)
 def get_browser(title:str=None,type:str='Folder',args:dict={},initial_folder:str=get_current_path(),exit_events:(str or list)=['Cancel'],return_events:(str or list)=['OK']):
     window = get_window(args=get_browser_layout(title=title,type=type,args=args,initial_folder=initial_folder))
     results = while_quick(window=window,exit_events=exit_events,return_events=return_events)
     if isinstance(results, dict):
```

## Comparing `abstract_gui-0.0.54.82.dist-info/METADATA` & `abstract_gui-0.0.54.83.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.54.82
+Version: 0.0.54.83
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_gui-0.0.54.82.dist-info/RECORD` & `abstract_gui-0.0.54.83.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 abstract_gui/__init__.py,sha256=D-StaJ4AjH9dHP_QOd6gr4JBYGgyX8iFOTJ9gj5tiuM,28
-abstract_gui/abstract_gui.py,sha256=Nmwng5TTqSbYdMjyr71LsBKqeaiyOi_x8NOYNqhm4dY,28030
+abstract_gui/abstract_gui.py,sha256=TAEtJVwhfZ3LCDWSAhYUoP_ADw497Xz6y1vGnvI3quk,28715
 abstract_gui/main.py,sha256=-5vBXHVdAuN_poGzYwcGvp1MUhUUg18z_crcDaIXWl4,1602
-abstract_gui-0.0.54.82.dist-info/METADATA,sha256=qQSxgXPU0Rppik9F7hIMNdz1TfaqzSYgtbGL9thJFkc,10155
-abstract_gui-0.0.54.82.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_gui-0.0.54.82.dist-info/top_level.txt,sha256=_lse2PkXkIfgtYuAn73RTk--wVrV_nWJ7Dn-2wK0F0E,13
-abstract_gui-0.0.54.82.dist-info/RECORD,,
+abstract_gui-0.0.54.83.dist-info/METADATA,sha256=YGqLq-H8giHEJfoxK9nNUtBSZ1UilxjB0zdg-LBS-60,10155
+abstract_gui-0.0.54.83.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_gui-0.0.54.83.dist-info/top_level.txt,sha256=_lse2PkXkIfgtYuAn73RTk--wVrV_nWJ7Dn-2wK0F0E,13
+abstract_gui-0.0.54.83.dist-info/RECORD,,
```

