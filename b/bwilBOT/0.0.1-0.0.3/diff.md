# Comparing `tmp/bwilBOT-0.0.1-py3-none-any.whl.zip` & `tmp/bwilBOT-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 42876 bytes, number of entries: 11
--rwxrwxrwx  2.0 unx    54701 b- defN 23-May-16 13:18 bwilBOT/__init__.py
+Zip file size: 42893 bytes, number of entries: 11
+-rwxrwxrwx  2.0 unx    54714 b- defN 23-Jun-01 17:50 bwilBOT/__init__.py
 -rwxrwxrwx  2.0 unx    54721 b- defN 23-May-08 19:05 elfebot/__init__.py
 -rwxrwxrwx  2.0 unx    54650 b- defN 23-Apr-12 07:29 oimbot/__init__.py
 -rwxrwxrwx  2.0 unx    54773 b- defN 23-Apr-01 08:51 oimbot/hahaha.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      620 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        8 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      532 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx      897 b- defN 23-May-16 13:19 bwilBOT-0.0.1.dist-info/RECORD
-11 files, 221051 bytes uncompressed, 41378 bytes compressed:  81.3%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      620 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      532 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      897 b- defN 23-Aug-02 09:57 bwilBOT-0.0.3.dist-info/RECORD
+11 files, 221064 bytes uncompressed, 41395 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: oimbot/__init__.py
 Comment: 
 
 Filename: oimbot/hahaha.py
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/DESCRIPTION.rst
+Filename: bwilBOT-0.0.3.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/dependency_links.txt
+Filename: bwilBOT-0.0.3.dist-info/dependency_links.txt
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/metadata.json
+Filename: bwilBOT-0.0.3.dist-info/metadata.json
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/top_level.txt
+Filename: bwilBOT-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/WHEEL
+Filename: bwilBOT-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/METADATA
+Filename: bwilBOT-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: bwilBOT-0.0.1.dist-info/RECORD
+Filename: bwilBOT-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bwilBOT/__init__.py

```diff
@@ -265,15 +265,15 @@
         self.bl_msg = ""
 
         self.added = "Patoche1961"
 
         self.bl_inv = 'Patoche1961'
         self.inv_on = "F"
 
-        self.adminx = "Patoche1961"
+        self.adminx = ["Patoche1961", "Roy0191"]
 
         self.inv_all = "T"
 
         self.skin_bl = ("")
         self.add_auto = ''
         self.number = ""
```

## Comparing `bwilBOT-0.0.1.dist-info/metadata.json` & `bwilBOT-0.0.3.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.0.3'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.0.1"
+    "version": "0.0.3"
 }
```

## Comparing `bwilBOT-0.0.1.dist-info/METADATA` & `bwilBOT-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: bwilBOT
-Version: 0.0.1
+Version: 0.0.3
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

