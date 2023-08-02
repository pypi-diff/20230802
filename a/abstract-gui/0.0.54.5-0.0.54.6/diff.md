# Comparing `tmp/abstract_gui-0.0.54.5-py3-none-any.whl.zip` & `tmp/abstract_gui-0.0.54.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9862 bytes, number of entries: 7
+Zip file size: 10518 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       28 b- defN 23-Jul-31 06:21 abstract_gui/__init__.py
--rw-r--r--  2.0 unx    24775 b- defN 23-Aug-01 21:57 abstract_gui/abstract_gui.py
+-rw-r--r--  2.0 unx    28030 b- defN 23-Aug-02 00:30 abstract_gui/abstract_gui.py
 -rw-r--r--  2.0 unx     1602 b- defN 23-Jul-31 04:07 abstract_gui/main.py
--rw-r--r--  2.0 unx    10154 b- defN 23-Aug-01 22:39 abstract_gui-0.0.54.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 22:39 abstract_gui-0.0.54.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Aug-01 22:39 abstract_gui-0.0.54.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      573 b- defN 23-Aug-01 22:39 abstract_gui-0.0.54.5.dist-info/RECORD
-7 files, 37237 bytes uncompressed, 8844 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    10154 b- defN 23-Aug-02 00:31 abstract_gui-0.0.54.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 00:31 abstract_gui-0.0.54.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-02 00:31 abstract_gui-0.0.54.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      573 b- defN 23-Aug-02 00:31 abstract_gui-0.0.54.6.dist-info/RECORD
+7 files, 40492 bytes uncompressed, 9500 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: abstract_gui/abstract_gui.py
 Comment: 
 
 Filename: abstract_gui/main.py
 Comment: 
 
-Filename: abstract_gui-0.0.54.5.dist-info/METADATA
+Filename: abstract_gui-0.0.54.6.dist-info/METADATA
 Comment: 
 
-Filename: abstract_gui-0.0.54.5.dist-info/WHEEL
+Filename: abstract_gui-0.0.54.6.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_gui-0.0.54.5.dist-info/top_level.txt
+Filename: abstract_gui-0.0.54.6.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_gui-0.0.54.5.dist-info/RECORD
+Filename: abstract_gui-0.0.54.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_gui/abstract_gui.py

```diff
@@ -480,21 +480,63 @@
             window (any): The window to unregister.
         """
         win = self.search_global_windows(window)
         if win in self.get_window_names():
             del self.all_windows[win]
         elif self.is_window_object(win):
             del self.all_windows[window]
+def ensure_nested_list(obj):
+    # Check if the input object is a list
+    if not isinstance(obj, list):
+        # If it's not a list, create a new nested list containing the object
+        return [obj]
+    
+    # If it is a list, check if any of its elements are non-list objects
+    for element in obj:
+        if not isinstance(element, list):
+            # If at least one element is not a list, wrap the original list in a new list
+            return [obj]
+    
+    # If all elements are lists, return the original list
+    return obj
+def make_list_add(obj,values):
+    obj = list(obj)
+    for each in list(values):
+        obj.append(each)
+    return obj
+def if_not_window_make_window(window):
+    if isinstance(window, type(get_window())) == False:
+        if isinstance(window, dict):
+            if "layout" in window:
+                window["layout"]=ensure_nested_list(window["layout"])
+        window=get_window(args=window)
+    return window
+def while_quick(window,return_events:(list or str)=[],exit_events:(list or str)=[sg.WIN_CLOSED]):
+    exit_events = make_list_add(exit_events,[sg.WIN_CLOSED])
+    return_events = list(return_events)
+    last_values=[]
+    while True:
+        event, values = window.read()
+        if event ==sg.WIN_CLOSED:
+            window.close()
+            
+            values= None
+            break
+        elif event in return_events:
+            window.close()
+            break
+    return values     
+      
 def verify_args(args:dict=None, layout:list=None, title:str=None, event_function:str=None,exit_events:(list or str)=None):
         args = args or {}
         layout = layout or [[]]
         title = title or 'window'
         exit_events = exit_events or ["exit", "Exit", "EXIT"]
         args.setdefault("title", title)
-        args.setdefault("layout", layout)
+        args.setdefault("layout", ensure_nested_list(layout))
         args.setdefault("event_function", event_function)
         args.setdefault("exit_events", list(exit_events))
         return args
 def get_window(title=None, layout=None, args=None):
         """
         Get a PySimpleGUI window.
 
@@ -504,14 +546,76 @@
             args (dict, optional): Additional arguments for the window.
 
         Returns:
             any: A PySimpleGUI window.
         """
         args = verify_args(args=args, layout=layout, title=title)
         return get_gui_fun('Window', {**args})
+def get_browser_layout(title:str=None,type:str='Folder',args:dict={},initial_folder:str=get_current_path()):
+    """
+    Function to get a browser GUI based on the type specified.
+
+    Parameters:
+    type (str): The type of GUI window to display. Defaults to 'Folder'.
+    title (str): The title of the GUI window. Defaults to 'Directory'.
+
+    Returns:
+    dict: Returns the results of single_call function on the created GUI window.
+    """
+    if type.lower() not in 'folderdirectory':
+        type = 'File'
+    else:
+        type = 'Folder'
+    if title is None:
+        title = f'Please choose a {type.lower()}'
+    layout = [
+        [get_gui_fun('Text', {"text": title})],
+        [get_gui_fun('Input',args={"default":initial_folder,"key":"output"}), get_gui_fun(f'{type}Browse', {**args, "initial_folder": initial_folder})],
+        [get_gui_fun('OK'), get_gui_fun('Cancel')]
+    ]
+    return {"title": f'{type} Explorer', "layout": layout}
+def get_input_layout(title:str="Input Window",text:str="please enter your input",default:str=None,args:dict={}):
+    """
+    Function to get a browser GUI based on the type specified.
+
+    Parameters:
+    type (str): The type of GUI window to display. Defaults to 'Folder'.
+    title (str): The title of the GUI window. Defaults to 'Directory'.
+
+    Returns:
+    dict: Returns the results of single_call function on the created GUI window.
+    """
+    if type.lower() not in 'folderdirectory':
+        type = 'File'
+    else:
+        type = 'Folder'
+    if title is None:
+        title = f'Please choose a {type.lower()}'
+    if "default" not in args:
+        args["default"]=default
+    if "key" not in args:
+        args["key"]=key
+    if "text" in args:
+        text = args["text"]
+    layout = [
+        [get_gui_fun('Text', {"text": text})],
+        [get_gui_fun('Input',args=args)],
+        [get_gui_fun('OK'), get_gui_fun('Cancel')]
+    ]
+    return {"title":title, "layout": layout}
+def get_input(title:str="Input Window",text:str="please enter your input",default:str=None,args:dict={},exit_events:(str or list)=['Cancel'],return_events:(str or list)=['OK']):
+    window = get_window(args=get_input_layout(title=title,text=text,args=args,default=default,initial_folder=initial_folder))
+    return while_quick(window=window,exit_events=exit_events,return_events=return_events)
+def get_browser(title:str=None,type:str='Folder',args:dict={},initial_folder:str=get_current_path(),exit_events:(str or list)=['Cancel'],return_events:(str or list)=['OK']):
+    window = get_window(args=get_browser_layout(title=title,type=type,args=args,initial_folder=initial_folder))
+    results = while_quick(window=window,exit_events=exit_events,return_events=return_events)
+    if isinstance(results, dict):
+        if results['output']=='':
+            results['output'] =initial_folder
+    return results
 def out_of_bounds(upper: (int or float) = 100, lower: (int or float) = 0, obj: (int or float) = -1):
     """
     Checks if the given object is out of the specified upper and lower bounds.
 
     Args:
         upper (int or float): The upper bound.
         lower (int or float): The lower bound.
@@ -569,36 +673,13 @@
     Returns:
         callable: A callable object that invokes the PySimpleGUI function with the specified arguments when called.
     """
     return get_fun({"instance": sg, "name": name, "args": args})
 def expandable(size: tuple = (None, None),resizable:bool=True,scrollable:bool=True,auto_size_text:bool=True,expand_x:bool=True,expand_y:bool=True):
     """Returns a dictionary with window parameters for creating an expandable PySimpleGUI window."""
     return {"size": size, "resizable": resizable, "scrollable": scrollable, "auto_size_text": auto_size_text, "expand_x": expand_x, "expand_y": expand_y}
-def get_browser(title:str=None,type:str='Folder',args:dict={},initial_folder:str=get_current_path()):
-    """
-    Function to get a browser GUI based on the type specified.
-
-    Parameters:
-    type (str): The type of GUI window to display. Defaults to 'Folder'.
-    title (str): The title of the GUI window. Defaults to 'Directory'.
-
-    Returns:
-    dict: Returns the results of single_call function on the created GUI window.
-    """
-    if type.lower() not in 'folderdirectory':
-        type='File'
-    else:
-        type = 'Folder'
-    if title == None:
-        title = f'Please choose a {type.lower()}'
-    return get_gui_fun('Window',{"title":f'{type} Explorer', "layout":[[get_gui_fun('Text',{"text":title})],
-                                                                         [get_gui_fun('Input'), get_gui_fun(f'{type}Browse',{**args,"initial_folder":initial_folder})],
-                                                                         [get_gui_fun('OK'), get_gui_fun('Cancel')]]
-                                   }
-                         )
-
 def create_window_manager(script_name='default_script_name',global_var=globals()):
     bridge = WindowGlobalBridge()
     script_name = bridge.create_script_name(script_name)
     global_var[script_name] = script_name
     bridge.retrieve_global_variables(script_name, global_var)
     return WindowManager(script_name, bridge),bridge,script_name
```

## Comparing `abstract_gui-0.0.54.5.dist-info/METADATA` & `abstract_gui-0.0.54.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.54.5
+Version: 0.0.54.6
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

