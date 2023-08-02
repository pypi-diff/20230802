# Comparing `tmp/SOMcreator-1.1.8.tar.gz` & `tmp/SOMcreator-1.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.8.tar", last modified: Tue Aug  1 15:29:36 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.8.2.tar", last modified: Wed Aug  2 07:02:08 2023, max compression
```

## Comparing `SOMcreator-1.1.8.tar` & `SOMcreator-1.1.8.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.344247 SOMcreator-1.1.8/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1554 2023-08-01 15:29:36.344247 SOMcreator-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.8/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 15:29:36.344247 SOMcreator-1.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.154034 SOMcreator-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.183826 SOMcreator-1.1.8/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.251649 SOMcreator-1.1.8/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.8/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.263422 SOMcreator-1.1.8/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.294165 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      154 2023-08-01 15:29:19.000000 SOMcreator-1.1.8/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    24554 2023-08-01 15:26:46.000000 SOMcreator-1.1.8/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.8/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.343251 SOMcreator-1.1.8/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9397 2023-08-01 15:25:56.000000 SOMcreator-1.1.8/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.8/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:29:36.217166 SOMcreator-1.1.8/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1554 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 15:29:36.000000 SOMcreator-1.1.8/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.936198 SOMcreator-1.1.8.2/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.8.2/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1556 2023-08-02 07:02:08.935963 SOMcreator-1.1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.8.2/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:02:08.936198 SOMcreator-1.1.8.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.706434 SOMcreator-1.1.8.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.740712 SOMcreator-1.1.8.2/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.814039 SOMcreator-1.1.8.2/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.829525 SOMcreator-1.1.8.2/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.873396 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      156 2023-08-02 07:01:42.000000 SOMcreator-1.1.8.2/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    24588 2023-08-01 15:38:40.000000 SOMcreator-1.1.8.2/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.2/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.934473 SOMcreator-1.1.8.2/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22074 2023-08-02 06:22:43.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0     9397 2023-08-01 15:25:56.000000 SOMcreator-1.1.8.2/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.765737 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1556 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.8/LICENSE` & `SOMcreator-1.1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/PKG-INFO` & `SOMcreator-1.1.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.8
+Version: 1.1.8.2
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.8/pyproject.toml` & `SOMcreator-1.1.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.8.2/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.8.2/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.8.2/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/classes.py` & `SOMcreator-1.1.8.2/src/SOMcreator/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -743,15 +743,16 @@
         self._parent: Aggregation | None = None
         self._parent_connection = parent_connection
         self.object.add_aggregation(self)
 
     def delete(self) -> None:
         super(Aggregation, self).delete()
         self.object.remove_aggregation(self)
-        self.parent.children.remove(self)
+        if not self.is_root:
+            self.parent.children.remove(self)
         for child in self.children:
             child.parent = None
 
     @property
     def parent_connection(self):
         return self._parent_connection
```

### Comparing `SOMcreator-1.1.8/src/SOMcreator/constants.py` & `SOMcreator-1.1.8.2/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.8.2/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.8.2/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.8.2/src/SOMcreator/external_software/desite.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,19 +165,14 @@
                     ident_property_set = f"{ident_property_set}:"
 
                 cdata_code = template.render(psets=property_sets, object=obj, ident=ident_name,
                                              ident_pset=ident_property_set, constants=constants)
                 xml_code.text = cdata_code
                 handle_rule(xml_checkrun, "UniquePattern")
 
-                for script in obj.scripts:
-                    xml_rule_script = handle_rule_script(xml_attribute_rule_list, name=script.name)
-                    xml_code = handle_code(xml_rule_script)
-                    xml_code.text = script.code
-
                 xml_object_dict[xml_checkrun] = obj
 
             if parent_node.children:
                 create_container(parent_xml_container, parent_node)
             else:
                 create_object(parent_xml_container, parent_node)
```

### Comparing `SOMcreator-1.1.8/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.8.2/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.8.2/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.8.2/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.8.2/src/SOMcreator/filehandling.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.8.2/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.8.2/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.8
+Version: 1.1.8.2
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.8/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.8.2/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

