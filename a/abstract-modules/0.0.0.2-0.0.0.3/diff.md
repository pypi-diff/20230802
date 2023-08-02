# Comparing `tmp/abstract_modules-0.0.0.2-py3-none-any.whl.zip` & `tmp/abstract_modules-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7679 bytes, number of entries: 8
+Zip file size: 7676 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       40 b- defN 23-Aug-02 04:34 abstract_modules/__init__.py
 -rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 04:34 abstract_modules/main.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-Aug-02 06:19 abstract_modules/module_utils.py
--rw-r--r--  2.0 unx     8762 b- defN 23-Aug-02 06:28 abstract_modules/upload_utils.py
--rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 06:44 abstract_modules-0.0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 06:44 abstract_modules-0.0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 06:44 abstract_modules-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 06:44 abstract_modules-0.0.0.2.dist-info/RECORD
-8 files, 18242 bytes uncompressed, 6473 bytes compressed:  64.5%
+-rw-r--r--  2.0 unx     8664 b- defN 23-Aug-02 06:45 abstract_modules/upload_utils.py
+-rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 06:46 abstract_modules-0.0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 06:46 abstract_modules-0.0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 06:46 abstract_modules-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 06:46 abstract_modules-0.0.0.3.dist-info/RECORD
+8 files, 18144 bytes uncompressed, 6470 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: abstract_modules/module_utils.py
 Comment: 
 
 Filename: abstract_modules/upload_utils.py
 Comment: 
 
-Filename: abstract_modules-0.0.0.2.dist-info/METADATA
+Filename: abstract_modules-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: abstract_modules-0.0.0.2.dist-info/WHEEL
+Filename: abstract_modules-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_modules-0.0.0.2.dist-info/top_level.txt
+Filename: abstract_modules-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_modules-0.0.0.2.dist-info/RECORD
+Filename: abstract_modules-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_modules/upload_utils.py

```diff
@@ -122,15 +122,15 @@
     globals()["version_current"] = current_version
     # Save the updated version in setup.py
     save_new_setup(setup_file = read_setup()['file'].replace(setup_js['version'], version_current))
 def install_module(event):
     if event == "install":
         cmd_run(f'pip install {proj_name}=={version_current} --break-system-packages')
 def install_mods_layout():
-    win=windows_mgr.get_new_window(title="install module",layout=[[get_gui_fun('Button',{'button_text':'install_module','key':'install'}),get_gui_fun('Button',{'button_text':'exit','key':'EXIT'})]],event_function='install_module',output_text="/home/john-putkey/Documents/python_projects/modules/abstract_essentials/output.txt")
+    win=windows_mgr.get_new_window(title="install module",layout=[[get_gui_fun('Button',{'button_text':'install_module','key':'install'}),get_gui_fun('Button',{'button_text':'exit','key':'EXIT'})]],event_function='install_module')
     while True:
         events = windows_mgr.while_basic(window=win)
         if events == None:
             return 
 def get_list_of_projects():
     win=windows_mgr.get_new_window(title="list_window",layout=[[get_gui_fun('Listbox',{"values":os.listdir(parent_dir),"size":(25,10),'key':'projects',"enable_events":True}),get_gui_fun('Button',{'button_text':'submit','key':'exit'})]])
     globals()['project'] = windows_mgr.while_basic(window=win)['projects'][0]
@@ -150,8 +150,7 @@
     cmd_run_sudo(cmd=build_module(),key="SUDO_PASSWORD",output_text="/home/john-putkey/Documents/python_projects/modules/abstract_essentials/output.txt")
     upload_module()
     print(f"Completed setup.py for project: {project_dir}")
     install_mods_layout()
 def upload_main(directory:str=os.getcwd()):
     get_parent_directory(directory)
     run_setup_loop()
-
```

## Comparing `abstract_modules-0.0.0.2.dist-info/METADATA` & `abstract_modules-0.0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-modules
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: abstract_modules allows you to easily upload your Python module to the Python Package Index (PyPI) using Twine. It automates several steps of the packaging and distribution process, making it easier to share your module with the Python community..
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_modules
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_modules-0.0.0.2.dist-info/RECORD` & `abstract_modules-0.0.0.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 abstract_modules/__init__.py,sha256=0LNjFqr-o-wHdm5LGqcJ2NyZGfe0l7_GunRKIl1PSvs,40
 abstract_modules/main.py,sha256=zrkeuBjXVoW_DfUx2uVV-mEWDUsnGgpwWPdkSYqhoT0,1290
 abstract_modules/module_utils.py,sha256=d9p1ayFVT1PQLX86e1L9kbwC1K6zcVwW6Yh-XueieKA,3407
-abstract_modules/upload_utils.py,sha256=jUXrPS3eR1pB12v4__NqjsddFQT292jTCribE8YGGlY,8762
-abstract_modules-0.0.0.2.dist-info/METADATA,sha256=BWtBZ3UquoQBe1L2CDdevkt6SuXRpI02ebpOSVDS9og,3950
-abstract_modules-0.0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_modules-0.0.0.2.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
-abstract_modules-0.0.0.2.dist-info/RECORD,,
+abstract_modules/upload_utils.py,sha256=PuXUr28zzr-X_ifI08YH64M9VvY2qU-KTGMBvxYV0a4,8664
+abstract_modules-0.0.0.3.dist-info/METADATA,sha256=d3a_j1yDl4Mcriqm8g7cal5WEdWsXbBa3p1v77yI1co,3950
+abstract_modules-0.0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_modules-0.0.0.3.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
+abstract_modules-0.0.0.3.dist-info/RECORD,,
```

