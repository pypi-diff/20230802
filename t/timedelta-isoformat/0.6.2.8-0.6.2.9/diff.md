# Comparing `tmp/timedelta_isoformat-0.6.2.8-py3-none-any.whl.zip` & `tmp/timedelta_isoformat-0.6.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 15922 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7635 b- defN 23-Mar-19 00:25 timedelta_isoformat/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-19 00:07 timedelta_isoformat/py.typed
--rw-r--r--  2.0 unx    32387 b- defN 23-Mar-19 00:27 timedelta_isoformat-0.6.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2350 b- defN 23-Mar-19 00:27 timedelta_isoformat-0.6.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-19 00:27 timedelta_isoformat-0.6.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Mar-19 00:27 timedelta_isoformat-0.6.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      627 b- defN 23-Mar-19 00:27 timedelta_isoformat-0.6.2.8.dist-info/RECORD
-7 files, 43111 bytes uncompressed, 14792 bytes compressed:  65.7%
+Zip file size: 15982 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7271 b- defN 23-Mar-19 09:30 timedelta_isoformat/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-19 01:05 timedelta_isoformat/py.typed
+-rw-r--r--  2.0 unx    32387 b- defN 23-Mar-19 09:41 timedelta_isoformat-0.6.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2636 b- defN 23-Mar-19 09:41 timedelta_isoformat-0.6.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-19 09:41 timedelta_isoformat-0.6.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Mar-19 09:41 timedelta_isoformat-0.6.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      627 b- defN 23-Mar-19 09:41 timedelta_isoformat-0.6.2.9.dist-info/RECORD
+7 files, 43033 bytes uncompressed, 14852 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: timedelta_isoformat/__init__.py
 Comment: 
 
 Filename: timedelta_isoformat/py.typed
 Comment: 
 
-Filename: timedelta_isoformat-0.6.2.8.dist-info/LICENSE
+Filename: timedelta_isoformat-0.6.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: timedelta_isoformat-0.6.2.8.dist-info/METADATA
+Filename: timedelta_isoformat-0.6.2.9.dist-info/METADATA
 Comment: 
 
-Filename: timedelta_isoformat-0.6.2.8.dist-info/WHEEL
+Filename: timedelta_isoformat-0.6.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: timedelta_isoformat-0.6.2.8.dist-info/top_level.txt
+Filename: timedelta_isoformat-0.6.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: timedelta_isoformat-0.6.2.8.dist-info/RECORD
+Filename: timedelta_isoformat-0.6.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## timedelta_isoformat/__init__.py

```diff
@@ -134,37 +134,24 @@
         date_segment, _, time_segment = duration[1:].partition("T")
         if date_segment:
             yield from cls._to_measurements(cls._parse_date(date_segment))
         if time_segment:
             yield from cls._to_measurements(cls._parse_time(time_segment))
 
     @staticmethod
-    def _type_check(value: str, integer_only: bool) -> bool:
-        if integer_only:
-            assert value.isdigit(), f"unable to parse '{value}' as a positive number"
-        else:
-            assert value[0:1].isdigit(), f"unable to parse '{value}' as a positive number"
-        return True
-
-    @staticmethod
-    def _bounds_check(quantity: float, limit: int | None, context: str) -> bool:
-        if limit is None:
-            assert 0 <= quantity, context + "[0..+∞)"
-        elif limit in (24, 60):
-            assert 0 <= quantity < limit, context + f"[0..{limit})"
-        else:
-            assert 0 <= quantity <= limit, context + f"[0..{limit}]"
-        return True
-
-    @staticmethod
     def _to_measurements(components: Components) -> Measurements:
         for value, unit, limit, integer_only in components:
-            assert timedelta._type_check(value, integer_only)
+            assert value.isdigit() if integer_only else value[0:1].isdigit(), f"unable to parse '{value}' as a positive number"
             quantity = float(value)
-            assert timedelta._bounds_check(quantity, limit, f"{unit} value of {value} exceeds range ")
+            if limit is None:
+                assert 0 <= quantity, f"{unit} value of {value} exceeds range [0..+∞)"
+            elif limit in (24, 60):
+                assert 0 <= quantity < limit, f"{unit} value of {value} exceeds range [0..{limit})"
+            else:
+                assert 0 <= quantity <= limit, f"{unit} value of {value} exceeds range [0..{limit}]"
             if quantity:
                 yield unit, quantity
 
     @classmethod
     def fromisoformat(cls, duration: str) -> "timedelta":
         """Parses an input string and returns a :py:class:`timedelta` result
```

## Comparing `timedelta_isoformat-0.6.2.8.dist-info/LICENSE` & `timedelta_isoformat-0.6.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `timedelta_isoformat-0.6.2.8.dist-info/METADATA` & `timedelta_isoformat-0.6.2.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedelta-isoformat
-Version: 0.6.2.8
+Version: 0.6.2.9
 Summary: Supplemental ISO8601 duration format support for datetime.timedelta
 Author-email: James Addison <jay@jp-hosting.net>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://pypi.org/project/timedelta-isoformat/
 Project-URL: Source, https://github.com/jayaddison/timedelta-isoformat.git/
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.10
@@ -45,7 +45,8 @@
 
 Some of the significant design decisions made within this library are:
 
 * Values in parsed duration strings must be zero-or-greater (``PT1H`` is considered valid; ``P-2D`` is not)
 * Empty time segments at the end of duration strings are allowed (``P1DT`` is considered valid)
 * Measurement limits are checked within date/time segments (``PT20:59:01`` is within limits; ``PT20:60:01`` is not)
 * Measurement values are parsed into floating-point values (at the time of writing, precise procedural algorithms to parse base-ten strings into integers for large inputs are not practical -- or not widely known)
+* When inputs are reliably known to be of correct type and format, assertions should be safe to remove (for example, by including the `-O command-line flag when invoking the Python interpreter <https://docs.python.org/3/using/cmdline.html#cmdoption-O>`_) to improve runtime performance
```

## Comparing `timedelta_isoformat-0.6.2.8.dist-info/RECORD` & `timedelta_isoformat-0.6.2.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-timedelta_isoformat/__init__.py,sha256=Gfky0t89F2MdMAntzFtCIvLwbUOOdjNn3iKVvYuoTpE,7635
+timedelta_isoformat/__init__.py,sha256=ulr2V_IzotuUmlqSPE-caL-ORxssxrKvMISw7tgcXHM,7271
 timedelta_isoformat/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-timedelta_isoformat-0.6.2.8.dist-info/LICENSE,sha256=zj-4LZ7oChyw5Uj5sFYOrVI3juK06Cb9lFm0rPcHXYk,32387
-timedelta_isoformat-0.6.2.8.dist-info/METADATA,sha256=fSHxIKEdd5txdKUDccYevzSA9Q58HPzFub5qF9UE5og,2350
-timedelta_isoformat-0.6.2.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-timedelta_isoformat-0.6.2.8.dist-info/top_level.txt,sha256=y8E7vilreINKjQnWSoAik7-mq5Zzqv7oDI0B5MHG67I,20
-timedelta_isoformat-0.6.2.8.dist-info/RECORD,,
+timedelta_isoformat-0.6.2.9.dist-info/LICENSE,sha256=zj-4LZ7oChyw5Uj5sFYOrVI3juK06Cb9lFm0rPcHXYk,32387
+timedelta_isoformat-0.6.2.9.dist-info/METADATA,sha256=NKh3hb_QfMhVLQHapu06cI8ceUCxDWTC5G8XtxiuaEs,2636
+timedelta_isoformat-0.6.2.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+timedelta_isoformat-0.6.2.9.dist-info/top_level.txt,sha256=y8E7vilreINKjQnWSoAik7-mq5Zzqv7oDI0B5MHG67I,20
+timedelta_isoformat-0.6.2.9.dist-info/RECORD,,
```

