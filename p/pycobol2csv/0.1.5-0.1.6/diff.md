# Comparing `tmp/pycobol2csv-0.1.5-py3-none-any.whl.zip` & `tmp/pycobol2csv-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8071 bytes, number of entries: 7
+Zip file size: 8068 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       52 b- defN 21-Sep-15 00:40 pycobol2csv/__init__.py
--rw-rw-rw-  2.0 fat    19023 b- defN 23-Aug-01 05:33 pycobol2csv/convert.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      564 b- defN 23-Aug-01 05:41 pycobol2csv-0.1.5.dist-info/RECORD
-7 files, 23097 bytes uncompressed, 7069 bytes compressed:  69.4%
+-rw-rw-rw-  2.0 fat    19023 b- defN 23-Aug-02 05:01 pycobol2csv/convert.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Aug-02 05:04 pycobol2csv-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Aug-02 05:04 pycobol2csv-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 05:04 pycobol2csv-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-02 05:04 pycobol2csv-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      564 b- defN 23-Aug-02 05:04 pycobol2csv-0.1.6.dist-info/RECORD
+7 files, 23097 bytes uncompressed, 7066 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycobol2csv/__init__.py
 Comment: 
 
 Filename: pycobol2csv/convert.py
 Comment: 
 
-Filename: pycobol2csv-0.1.5.dist-info/LICENSE
+Filename: pycobol2csv-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: pycobol2csv-0.1.5.dist-info/METADATA
+Filename: pycobol2csv-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: pycobol2csv-0.1.5.dist-info/WHEEL
+Filename: pycobol2csv-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: pycobol2csv-0.1.5.dist-info/top_level.txt
+Filename: pycobol2csv-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pycobol2csv-0.1.5.dist-info/RECORD
+Filename: pycobol2csv-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycobol2csv/convert.py

```diff
@@ -13,16 +13,16 @@
 class CobolPatterns:
     opt_pattern_format = "({})?"
     row_pattern_base = r"^(?P<level>\d{2})\s+(?P<name>\S+)"
     row_pattern_occurs = r"\s+OCCURS (?P<occurs>\d+) TIMES"
     row_pattern_indexed_by = r"\s+INDEXED BY\s(?P<indexed_by>\S+)"
     # row_pattern_redefines = r"\s+REDEFINES\s(?P<redefines>\S+)"
     row_pattern_redefines = r"\s+REDEFINES\s+(?P<redefines>\S+)"
-    # row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)"
-    row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)\s*\S+"
+    row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)"
+    # row_pattern_pic = r"\s+PIC\s+(?P<pic>\S+)\s*\S+"
     row_pattern_end = r"\.$"
     row_pattern = re.compile(
         row_pattern_base
         + opt_pattern_format.format(row_pattern_redefines)
         + opt_pattern_format.format(row_pattern_occurs)
         + opt_pattern_format.format(row_pattern_indexed_by)
         + opt_pattern_format.format(row_pattern_pic)
```

## Comparing `pycobol2csv-0.1.5.dist-info/LICENSE` & `pycobol2csv-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycobol2csv-0.1.5.dist-info/METADATA` & `pycobol2csv-0.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobol2csv
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library to convert COBOL ebcdic file to CSV format
 Home-page: https://github.com/jasonli-lijie/pycobol2csv
 Author: Jason Li
 Author-email: niomobileapp@gmail.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Project-URL: Bug Tracker, https://github.com/jasonli-lijie/pycobol2csv/issues
```

## Comparing `pycobol2csv-0.1.5.dist-info/RECORD` & `pycobol2csv-0.1.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pycobol2csv/__init__.py,sha256=q_ngSSKPu6OI2yQM0kHOOIU1tJkrSHwilFYszju4ZAc,52
-pycobol2csv/convert.py,sha256=oAecOxcb4hFkgzDuw7JKETfSXTAA9lc6_pqf3NpPuYg,19023
-pycobol2csv-0.1.5.dist-info/LICENSE,sha256=gpfrbvkPCMPpkAd1Hj5QOiDUlc3YiekPESzqUOnrAXc,1086
-pycobol2csv-0.1.5.dist-info/METADATA,sha256=U1x9k0AWNmh9JNDwsk3f7mP-VHmDcvxFYaV11g9Jp5g,2268
-pycobol2csv-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pycobol2csv-0.1.5.dist-info/top_level.txt,sha256=7vXJihqVTBYjcbl6skF7mXGZeB8VZfPBuFavaMCxtGk,12
-pycobol2csv-0.1.5.dist-info/RECORD,,
+pycobol2csv/convert.py,sha256=gEk5ByTZK7onjmKbB9Oga38cR5P1_dE9jOE9j7k_gzs,19023
+pycobol2csv-0.1.6.dist-info/LICENSE,sha256=gpfrbvkPCMPpkAd1Hj5QOiDUlc3YiekPESzqUOnrAXc,1086
+pycobol2csv-0.1.6.dist-info/METADATA,sha256=HvboIpAeLYl8IjuqXP5gPKMCWHFM8fciHdjH3oM-uVM,2268
+pycobol2csv-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pycobol2csv-0.1.6.dist-info/top_level.txt,sha256=7vXJihqVTBYjcbl6skF7mXGZeB8VZfPBuFavaMCxtGk,12
+pycobol2csv-0.1.6.dist-info/RECORD,,
```

