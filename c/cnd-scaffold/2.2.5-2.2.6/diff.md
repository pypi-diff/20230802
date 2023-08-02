# Comparing `tmp/cnd_scaffold-2.2.5-py3-none-any.whl.zip` & `tmp/cnd_scaffold-2.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4567 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        5 b- defN 23-Jun-08 15:34 cnd_scaffold/VERSION
--rw-r--r--  2.0 unx      129 b- defN 23-Jun-08 15:34 cnd_scaffold/__init__.py
--rw-r--r--  2.0 unx      121 b- defN 23-Jun-08 15:34 cnd_scaffold/__version__.py
--rw-r--r--  2.0 unx     6767 b- defN 23-Jun-08 15:34 cnd_scaffold/cnd_scaffold.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      640 b- defN 23-Jun-08 15:34 cnd_scaffold-2.2.5.dist-info/RECORD
-8 files, 10284 bytes uncompressed, 3443 bytes compressed:  66.5%
+Zip file size: 4637 bytes, number of entries: 8
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Aug-02 17:28 cnd_scaffold/VERSION
+-rw-r--r--  2.0 unx      129 b- defN 23-Aug-02 17:28 cnd_scaffold/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Aug-02 17:28 cnd_scaffold/__version__.py
+-rw-r--r--  2.0 unx     7008 b- defN 23-Aug-02 17:28 cnd_scaffold/cnd_scaffold.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Aug-02 17:29 cnd_scaffold-2.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 17:29 cnd_scaffold-2.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-02 17:29 cnd_scaffold-2.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      640 b- defN 23-Aug-02 17:29 cnd_scaffold-2.2.6.dist-info/RECORD
+8 files, 10525 bytes uncompressed, 3513 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: cnd_scaffold/__version__.py
 Comment: 
 
 Filename: cnd_scaffold/cnd_scaffold.py
 Comment: 
 
-Filename: cnd_scaffold-2.2.5.dist-info/METADATA
+Filename: cnd_scaffold-2.2.6.dist-info/METADATA
 Comment: 
 
-Filename: cnd_scaffold-2.2.5.dist-info/WHEEL
+Filename: cnd_scaffold-2.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_scaffold-2.2.5.dist-info/top_level.txt
+Filename: cnd_scaffold-2.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_scaffold-2.2.5.dist-info/RECORD
+Filename: cnd_scaffold-2.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cnd_scaffold/VERSION

```diff
@@ -1 +1 @@
-2.2.5
+2.2.6
```

## cnd_scaffold/cnd_scaffold.py

```diff
@@ -106,22 +106,27 @@
         if step not in self.yaml_structure:
             return 0
         total = 0
         for item in self.yaml_structure[step]:
             total += len(self._load_file(item))
         return total
 
+    def replace_multi_type(self, content, search, value):
+        str_value = value if isinstance(value, list) is False else ",".join(value)
+        content = content.replace(f"%{search}%", str_value)
+        return content
+
     def _default_replace_engine(self, content, local_var={}):
         for item in local_var:
-            if isinstance(local_var[item], dict) is True:
-                for key in local_var[item]:
-                    str_to_replace = f'{item}.{key}'
-                    content = content.replace(f"%{str_to_replace}%", local_var[item][key])
-            else:
-                content = content.replace(f"%{item}%", local_var[item])
+            if isinstance(local_var[item], dict) is False:
+                content = self.replace_multi_type(content, item, local_var[item])
+                continue
+            for key in local_var[item]:
+                str_to_replace = f'{item}.{key}'
+                content = self.replace_multi_type(content, str_to_replace, local_var[item][key])
         for item in self._data_to_replace:
             if isinstance(self._data_to_replace[item], dict) is True or isinstance(self._data_to_replace[item], list) is True:
                 content = content.replace(f"%{item}%", json.dumps(self._data_to_replace[item]))
             else:
                 content = content.replace(f"%{item}%", self._data_to_replace[item])
         return content
```

## Comparing `cnd_scaffold-2.2.5.dist-info/METADATA` & `cnd_scaffold-2.2.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-scaffold
-Version: 2.2.5
+Version: 2.2.6
 Summary: Tools initiate a new project in git lab, based on a existing definition
 Home-page: https://gitlab.com/changendevops/gitopstoolkit/cnd-scaffold.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/gitopstoolkit/cnd-scaffold.git
```

## Comparing `cnd_scaffold-2.2.5.dist-info/RECORD` & `cnd_scaffold-2.2.6.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cnd_scaffold/VERSION,sha256=1w0u4F28hl3CGt8fYrJSEgtQOSXguuNSJWgD2xAnWrw,5
+cnd_scaffold/VERSION,sha256=47hT5mfrClTF-YlTMyWhfMnAvnPlcyPfjC-vwvFMQbA,5
 cnd_scaffold/__init__.py,sha256=lrHENo1vmuBxM5rDVLod1IRy4vj1VkmANGW4TJxjEzA,129
 cnd_scaffold/__version__.py,sha256=H3kvuz6COTEsEmLiRYVrEExrhU4b1hgM4hWI9_yQx0g,121
-cnd_scaffold/cnd_scaffold.py,sha256=Y0_SLIuIRNqvKGLuwkQ6hermf1mLZDYx1tSsGiYdoLQ,6767
-cnd_scaffold-2.2.5.dist-info/METADATA,sha256=y5h_cDS-pxpcbntlvRqGGSu-bINsRsrDsekg11ONVDM,2517
-cnd_scaffold-2.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cnd_scaffold-2.2.5.dist-info/top_level.txt,sha256=SSg5zF4f5c15HCseVrjsgR1pKy0NSF--6NYV7M2Q37k,13
-cnd_scaffold-2.2.5.dist-info/RECORD,,
+cnd_scaffold/cnd_scaffold.py,sha256=f5UB4ek5emvF_Z8KPp5ydTa1IQiSZCY156Gj7bfKD0c,7008
+cnd_scaffold-2.2.6.dist-info/METADATA,sha256=vw0Douz7FelGzICggGLUCUDu7vJtzlPcL_1vgRWzAEE,2517
+cnd_scaffold-2.2.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+cnd_scaffold-2.2.6.dist-info/top_level.txt,sha256=SSg5zF4f5c15HCseVrjsgR1pKy0NSF--6NYV7M2Q37k,13
+cnd_scaffold-2.2.6.dist-info/RECORD,,
```

