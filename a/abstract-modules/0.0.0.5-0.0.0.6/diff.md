# Comparing `tmp/abstract_modules-0.0.0.5-py3-none-any.whl.zip` & `tmp/abstract_modules-0.0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 7740 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       40 b- defN 23-Aug-02 04:34 abstract_modules/__init__.py
 -rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 04:34 abstract_modules/main.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-Aug-02 06:19 abstract_modules/module_utils.py
--rw-r--r--  2.0 unx     9022 b- defN 23-Aug-02 07:12 abstract_modules/upload_utils.py
--rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 07:12 abstract_modules-0.0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 07:12 abstract_modules-0.0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 07:12 abstract_modules-0.0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 07:12 abstract_modules-0.0.0.5.dist-info/RECORD
-8 files, 18502 bytes uncompressed, 6534 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     9040 b- defN 23-Aug-02 07:14 abstract_modules/upload_utils.py
+-rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 07:14 abstract_modules-0.0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 07:14 abstract_modules-0.0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 07:14 abstract_modules-0.0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 07:14 abstract_modules-0.0.0.6.dist-info/RECORD
+8 files, 18520 bytes uncompressed, 6534 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: abstract_modules/module_utils.py
 Comment: 
 
 Filename: abstract_modules/upload_utils.py
 Comment: 
 
-Filename: abstract_modules-0.0.0.5.dist-info/METADATA
+Filename: abstract_modules-0.0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: abstract_modules-0.0.0.5.dist-info/WHEEL
+Filename: abstract_modules-0.0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_modules-0.0.0.5.dist-info/top_level.txt
+Filename: abstract_modules-0.0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_modules-0.0.0.5.dist-info/RECORD
+Filename: abstract_modules-0.0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_modules/upload_utils.py

```diff
@@ -70,15 +70,15 @@
     Organize the list of version numbers from highest to lowest.
     :param version_list: A list of version numbers to organize.
     :return: A new list of version numbers sorted from highest to lowest.
     """
     sorted_versions = sorted(version_list, key=lambda x: list(map(int, x.split('.'))), reverse=True)
     return sorted_versions
 
-def get_distributions_from_packages(version_numbers):
+def get_distributions_from_packages(setup_js,version_numbers):
     if os.path.isdir('dist'):
         dist_list = os.listdir('dist')
         for dist in dist_list:
             rest = dist[len(setup_js['name'] + '-'):]
             version = ''
             while len(rest) > 0 and rest[0] in '0123456789.':
                 version += rest[0]
@@ -99,15 +99,15 @@
     version_numbers = organize_versions_from_high_to_low(version_numbers)
     if version_numbers[0] != current_version:
         version_number_highest = False
         text = text + f" Your version number {current_version} is lower than the highest version number {version_numbers[0]}."
     return text,version_number_highest
 def get_distributions(setup_js):
    
-    version_numbers = get_distributions_from_packages([])
+    version_numbers = get_distributions_from_packages(setup_js,[])
     installed_versions = get_installed_versions(setup_js['name'])
     for version in installed_versions:
         version_number = version.split('=')[-1]
         if version_number not in version_numbers:
             version_numbers.append(version_number)
     new_version = setup_js['version']
```

## Comparing `abstract_modules-0.0.0.5.dist-info/METADATA` & `abstract_modules-0.0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-modules
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: abstract_modules allows you to easily upload your Python module to the Python Package Index (PyPI) using Twine. It automates several steps of the packaging and distribution process, making it easier to share your module with the Python community..
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_modules
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `abstract_modules-0.0.0.5.dist-info/RECORD` & `abstract_modules-0.0.0.6.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 abstract_modules/__init__.py,sha256=0LNjFqr-o-wHdm5LGqcJ2NyZGfe0l7_GunRKIl1PSvs,40
 abstract_modules/main.py,sha256=zrkeuBjXVoW_DfUx2uVV-mEWDUsnGgpwWPdkSYqhoT0,1290
 abstract_modules/module_utils.py,sha256=d9p1ayFVT1PQLX86e1L9kbwC1K6zcVwW6Yh-XueieKA,3407
-abstract_modules/upload_utils.py,sha256=vDjHdgKml_-4FX_raTl8KjV-Ok45pKn_74pTw6vW-bA,9022
-abstract_modules-0.0.0.5.dist-info/METADATA,sha256=6bwzesQK94j8sN51IUPzpvRXEfic-2CtcqgER-p6k-E,3950
-abstract_modules-0.0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_modules-0.0.0.5.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
-abstract_modules-0.0.0.5.dist-info/RECORD,,
+abstract_modules/upload_utils.py,sha256=S3OibAqUb_1TFYXNw45pFpwCMEax0M3FJnRiS6mfkeE,9040
+abstract_modules-0.0.0.6.dist-info/METADATA,sha256=M_F66Ehv0iGfh7-zrURhmxfTabL0i7oSG2OpfDYnQTg,3950
+abstract_modules-0.0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_modules-0.0.0.6.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
+abstract_modules-0.0.0.6.dist-info/RECORD,,
```

