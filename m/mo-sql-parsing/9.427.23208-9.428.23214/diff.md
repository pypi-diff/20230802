# Comparing `tmp/mo_sql_parsing-9.427.23208-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.428.23214-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38408 bytes, number of entries: 13
+Zip file size: 38409 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2530 b- defN 23-Jul-18 01:32 mo_sql_parsing/__init__.py
 -rw-rw-rw-  2.0 fat    22382 b- defN 23-Jul-18 01:32 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10695 b- defN 23-Jul-18 01:32 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    34229 b- defN 23-Jul-27 21:40 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat    34299 b- defN 23-Aug-02 00:44 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7357 b- defN 23-Jul-22 13:56 mo_sql_parsing/types.py
 -rw-rw-rw-  2.0 fat    23118 b- defN 23-Jul-27 21:40 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2920 b- defN 23-Jul-18 01:32 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-27 21:40 mo_sql_parsing-9.427.23208.dist-info/RECORD
-13 files, 129759 bytes uncompressed, 36502 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-Aug-02 00:44 mo_sql_parsing-9.428.23214.dist-info/RECORD
+13 files, 129829 bytes uncompressed, 36503 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.427.23208.dist-info/LICENSE
+Filename: mo_sql_parsing-9.428.23214.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.427.23208.dist-info/METADATA
+Filename: mo_sql_parsing-9.428.23214.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.427.23208.dist-info/WHEEL
+Filename: mo_sql_parsing-9.428.23214.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.427.23208.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.428.23214.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.427.23208.dist-info/zip-safe
+Filename: mo_sql_parsing-9.428.23214.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.427.23208.dist-info/RECORD
+Filename: mo_sql_parsing-9.428.23214.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -346,16 +346,16 @@
         window_clause, over_clause = window(expression, identifier, sort_column)
 
         expression << (
             (
                 Literal("*")
                 | infix_notation(
                     compound,
-                    [
-                        (dynamic_accessor, 1, LEFT_ASSOC, to_offset,),
+                    ([] if sqlserver else [(dynamic_accessor, 1, LEFT_ASSOC, to_offset,)])
+                    + [
                         (simple_accessor, 1, LEFT_ASSOC, to_offset,),
                         (accessor, 1, LEFT_ASSOC, to_offset),
                         (window_clause, 1, LEFT_ASSOC, to_window_mod),
                         (assign("filter", LB + WHERE + expression + RB), 1, LEFT_ASSOC, to_window_mod,),
                     ]
                     + [
                         (
@@ -549,15 +549,19 @@
         #####################################################################
         # DML STATEMENTS
         #####################################################################
 
         # MySQL's index_type := Using + ( "BTREE" | "HASH" )
         index_type = Optional(assign("using", ident("index_type")))
 
-        index_column_names = LB + delimited_list((identifier("value") + Optional(LB + int_num("length") + RB)) / to_index_part)("columns") + RB
+        index_column_names = (
+            LB
+            + delimited_list((identifier("value") + Optional(LB + int_num("length") + RB)) / to_index_part)("columns")
+            + RB
+        )
 
         column_def_delete = assign("on delete", (keyword("cascade") | keyword("set null") | keyword("set default")),)
 
         table_def_foreign_key = FOREIGN_KEY + Optional(
             Optional(identifier("index_name"))
             + index_column_names
             + column_def_references
```

## Comparing `mo_sql_parsing-9.427.23208.dist-info/LICENSE` & `mo_sql_parsing-9.428.23214.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.427.23208.dist-info/METADATA` & `mo_sql_parsing-9.428.23214.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.427.23208
+Version: 9.428.23214
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots (==9.417.23168)
-Requires-Dist: mo-future (==7.416.23168)
-Requires-Dist: mo-imports (==7.416.23168)
-Requires-Dist: mo-parsing (==8.423.23199)
+Requires-Dist: mo-dots (==9.428.23214)
+Requires-Dist: mo-future (==7.428.23214)
+Requires-Dist: mo-imports (==7.428.23214)
+Requires-Dist: mo-parsing (==8.428.23214)
 Provides-Extra: dev
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-files ; extra == 'tests'
 Requires-Dist: mo-streams ; extra == 'tests'
 Requires-Dist: zstandard ; extra == 'tests'
```

## Comparing `mo_sql_parsing-9.427.23208.dist-info/RECORD` & `mo_sql_parsing-9.428.23214.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=ZbsunSI2YPlPkveviGXQuv_YjCmofsrVOOu6qb500gM,2530
 mo_sql_parsing/formatting.py,sha256=Nzcrs6aWLQRK0hd8QvyPZ4hMF1onIhyvE2iBrtKF-Fw,22382
 mo_sql_parsing/keywords.py,sha256=nFTOQv7VOTDI4Ud3oSJh0-II9FGH4wWXmFRwZ5R3uzk,10695
-mo_sql_parsing/sql_parser.py,sha256=S6oZUKwMvYp8LTwFp4mYnK_0g4aAa1ySg5Kb8WeTRG8,34229
+mo_sql_parsing/sql_parser.py,sha256=WSvORof2TnoekZzZm8Tm60AzEP9NCPSKMfLqFFGI6kU,34299
 mo_sql_parsing/types.py,sha256=tloEMsDgghBPm9O9MjyMLj8lUJ2ALTMdPEv3hU841HY,7357
 mo_sql_parsing/utils.py,sha256=r5EAEgGlIINl3UPN18Hk7LS4pQzeA_GLytRP-CI79aE,23118
 mo_sql_parsing/windows.py,sha256=KelC9CZopR53tb0xAPxWsbxt59ieR_kNmM37FFcMjzE,2920
-mo_sql_parsing-9.427.23208.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.427.23208.dist-info/METADATA,sha256=legbgdTQiK0Ar9zieB3Br7cBPpxiie9APN-TH9hahzQ,9345
-mo_sql_parsing-9.427.23208.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.427.23208.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.427.23208.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.427.23208.dist-info/RECORD,,
+mo_sql_parsing-9.428.23214.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.428.23214.dist-info/METADATA,sha256=ngF9Tq9yBtsh85G2gGhBImcN1Q5o5QjgLQh-fxckRUk,9345
+mo_sql_parsing-9.428.23214.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.428.23214.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.428.23214.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.428.23214.dist-info/RECORD,,
```

