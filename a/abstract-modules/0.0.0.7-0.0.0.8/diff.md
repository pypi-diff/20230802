# Comparing `tmp/abstract_modules-0.0.0.7-py3-none-any.whl.zip` & `tmp/abstract_modules-0.0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7732 bytes, number of entries: 8
+Zip file size: 7737 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       40 b- defN 23-Aug-02 04:34 abstract_modules/__init__.py
 -rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 04:34 abstract_modules/main.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-Aug-02 06:19 abstract_modules/module_utils.py
--rw-r--r--  2.0 unx     8990 b- defN 23-Aug-02 07:16 abstract_modules/upload_utils.py
--rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 07:16 abstract_modules-0.0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 07:16 abstract_modules-0.0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 07:16 abstract_modules-0.0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 07:16 abstract_modules-0.0.0.7.dist-info/RECORD
-8 files, 18470 bytes uncompressed, 6526 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     8994 b- defN 23-Aug-02 07:18 abstract_modules/upload_utils.py
+-rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 07:19 abstract_modules-0.0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 07:19 abstract_modules-0.0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 07:19 abstract_modules-0.0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 07:19 abstract_modules-0.0.0.8.dist-info/RECORD
+8 files, 18474 bytes uncompressed, 6531 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: abstract_modules/module_utils.py
 Comment: 
 
 Filename: abstract_modules/upload_utils.py
 Comment: 
 
-Filename: abstract_modules-0.0.0.7.dist-info/METADATA
+Filename: abstract_modules-0.0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: abstract_modules-0.0.0.7.dist-info/WHEEL
+Filename: abstract_modules-0.0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_modules-0.0.0.7.dist-info/top_level.txt
+Filename: abstract_modules-0.0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_modules-0.0.0.7.dist-info/RECORD
+Filename: abstract_modules-0.0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_modules/upload_utils.py

```diff
@@ -108,15 +108,15 @@
     for version in installed_versions:
         version_number = version.split('=')[-1]
         if version_number not in version_numbers:
             version_numbers.append(version_number)
     new_version = setup_js['version']
     
     while get_version_text(new_version,version_numbers)[1] !=True:
-        text = get_version_text(new_version,version_numbers)+' please enter a new version number'
+        text = get_version_text(new_version,version_numbers)[0] +' please enter a new version number'
         layout = [
             [get_gui_fun("T", {"text": text})],
             [get_gui_fun('Input', {"default_text": organize_versions_from_high_to_low(version_numbers)[0], "key": "version_number"})],
             [sg.Button("OK")]
         ]
         new_version = windows_mgr.while_basic(windows_mgr.get_new_window(title='Version number', args={"layout": layout},exit_events=["OK", "Override"]))["version_number"]
         setup_file = setup_file.replace(current_version, new_version)
```

## Comparing `abstract_modules-0.0.0.7.dist-info/METADATA` & `abstract_modules-0.0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-modules
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: abstract_modules allows you to easily upload your Python module to the Python Package Index (PyPI) using Twine. It automates several steps of the packaging and distribution process, making it easier to share your module with the Python community..
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_modules
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_modules-0.0.0.7.dist-info/RECORD` & `abstract_modules-0.0.0.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 abstract_modules/__init__.py,sha256=0LNjFqr-o-wHdm5LGqcJ2NyZGfe0l7_GunRKIl1PSvs,40
 abstract_modules/main.py,sha256=zrkeuBjXVoW_DfUx2uVV-mEWDUsnGgpwWPdkSYqhoT0,1290
 abstract_modules/module_utils.py,sha256=d9p1ayFVT1PQLX86e1L9kbwC1K6zcVwW6Yh-XueieKA,3407
-abstract_modules/upload_utils.py,sha256=AxxqEwfZaxzPJM53e1reAu50KgvIun6iV7req6YtK5s,8990
-abstract_modules-0.0.0.7.dist-info/METADATA,sha256=lIn5FMj8d5mq6vZ-dTHmjxhrTPsFstnml2H3pKVnffM,3950
-abstract_modules-0.0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_modules-0.0.0.7.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
-abstract_modules-0.0.0.7.dist-info/RECORD,,
+abstract_modules/upload_utils.py,sha256=hmaSTeAqJvFt-22JJZTFkbcH45ZVEIXfWQ_ep7MU174,8994
+abstract_modules-0.0.0.8.dist-info/METADATA,sha256=ULKqQUW9htu5xgnxrJt8cfHDFkMXvvVuUVJvRBO87Bs,3950
+abstract_modules-0.0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_modules-0.0.0.8.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
+abstract_modules-0.0.0.8.dist-info/RECORD,,
```

