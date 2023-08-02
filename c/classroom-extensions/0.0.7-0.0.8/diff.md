# Comparing `tmp/classroom_extensions-0.0.7.tar.gz` & `tmp/classroom_extensions-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classroom_extensions-0.0.7.tar", last modified: Tue Aug  1 22:20:34 2023, max compression
+gzip compressed data, was "classroom_extensions-0.0.8.tar", last modified: Wed Aug  2 17:39:00 2023, max compression
```

## Comparing `classroom_extensions-0.0.7.tar` & `classroom_extensions-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/classroom_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mariadb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/mongodb_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/classroom_extensions/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/classroom_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 22:20:34.000000 classroom_extensions-0.0.7/classroom_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:20:34.853248 classroom_extensions-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_plantuml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-01 22:20:25.000000 classroom_extensions-0.0.7/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:39:00.570585 classroom_extensions-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-02 17:39:00.570585 classroom_extensions-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:39:00.566585 classroom_extensions-0.0.8/classroom_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/mariadb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/mongodb_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/classroom_extensions/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:39:00.566585 classroom_extensions-0.0.8/classroom_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-02 17:39:00.000000 classroom_extensions-0.0.8/classroom_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 17:39:00.000000 classroom_extensions-0.0.8/classroom_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:39:00.000000 classroom_extensions-0.0.8/classroom_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-02 17:39:00.000000 classroom_extensions-0.0.8/classroom_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 17:39:00.000000 classroom_extensions-0.0.8/classroom_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:39:00.570585 classroom_extensions-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:39:00.570585 classroom_extensions-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/tests/test_mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/tests/test_plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-02 17:38:50.000000 classroom_extensions-0.0.8/tests/test_web.py
```

### Comparing `classroom_extensions-0.0.7/LICENSE` & `classroom_extensions-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/PKG-INFO` & `classroom_extensions-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom_extensions
-Version: 0.0.7
+Version: 0.0.8
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
```

### Comparing `classroom_extensions-0.0.7/README.rst` & `classroom_extensions-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions/mariadb.py` & `classroom_extensions-0.0.8/classroom_extensions/mariadb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions/mariadb_install.py` & `classroom_extensions-0.0.8/classroom_extensions/mariadb_install.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions/mongodb.py` & `classroom_extensions-0.0.8/classroom_extensions/mongodb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions/mongodb_install.py` & `classroom_extensions-0.0.8/classroom_extensions/mongodb_install.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions/plantuml.py` & `classroom_extensions-0.0.8/classroom_extensions/plantuml.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """ Extension that uses PlantUML to draw multiple types of diagrams """
 
 import json
 import sys
 from os.path import expanduser
 
 from IPython.core import magic_arguments
-from IPython.core.magic import magics_class, cell_magic, line_magic
+from IPython.core.magic import magics_class, cell_magic, line_magic, line_cell_magic
 from IPython.core.magics.display import DisplayMagics, display
 from IPython.display import SVG, Image
 from IPython.utils.process import arg_split
 from plantweb import render, defaults
 
 __all__ = ["load_ipython_extension", "unload_ipython_extension", "PlantUmlMagics"]
 
@@ -97,14 +97,38 @@
             print(
                 "Use --server=address to provide the address of a valid PlantUML server"
             )
 
         self._plantweb_config["format"] = args.format
         self._save_plantuml_config()
 
+    @magic_arguments.magic_arguments()
+    @plantuml_args
+    @magic_arguments.argument("--json", "-j", type=str, help="Path to the file on disk")
+    @line_cell_magic
+    def json(self, line="", cell=None) -> None:
+        """Used to create a graphical representation of a JSON file/object"""
+        args = magic_arguments.parse_argstring(self.json, line)
+
+        if args.json is not None:
+            with open(args.json, "r", encoding="UTF-8") as json_file:
+                cell = json_file.read()
+
+        cell = f"""
+                @startjson
+                {cell}
+                @endjson
+                """
+        command = ""
+        for arg, value in vars(args).items():
+            if value is not None and arg != "json":
+                command += f" --{arg}={value}"
+
+        self.plantuml(line=command, cell=cell)
+
 
 def load_ipython_extension(ipython) -> None:
     """
     To unload the extension
     Args:
         ipython: the current interactive shell
```

### Comparing `classroom_extensions-0.0.7/classroom_extensions/util.py` & `classroom_extensions-0.0.8/classroom_extensions/util.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions/web.py` & `classroom_extensions-0.0.8/classroom_extensions/web.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/classroom_extensions.egg-info/PKG-INFO` & `classroom_extensions-0.0.8/classroom_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classroom-extensions
-Version: 0.0.7
+Version: 0.0.8
 Summary: IPython extensions used for teaching
 Author-email: Marcos Dias de Assuncao <assuncao@acm.org>
 Maintainer-email: Marcos Dias de Assuncao <assuncao@acm.org>
 License: MIT
 Project-URL: Homepage, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Bug Reports, https://github.com/assuncaomarcos/classroom_extensions
 Project-URL: Say Thanks!, https://saythanks.io/to/assuncaomarcos
```

### Comparing `classroom_extensions-0.0.7/classroom_extensions.egg-info/SOURCES.txt` & `classroom_extensions-0.0.8/classroom_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/pyproject.toml` & `classroom_extensions-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/tests/test_mariadb.py` & `classroom_extensions-0.0.8/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/tests/test_mongodb.py` & `classroom_extensions-0.0.8/tests/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `classroom_extensions-0.0.7/tests/test_plantuml.py` & `classroom_extensions-0.0.8/tests/test_plantuml.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,34 @@
     database Foo5
     Foo1 -> Foo2 : To boundary
     Foo1 -> Foo3 : To control
     Foo1 -> Foo4 : To entity
     Foo1 -> Foo5 : To database
 """
 
+_SIMPLE_JSON = """
+{
+    "status": "OK",
+    "code": 200,
+    "total": 2,
+    "data": [
+        {
+            "title": "Harum cumque placeat id.",
+            "description": "Qui autem tenetur ut aut.",
+            "url": "https://placekitten.com/300/500"
+        },
+        {
+            "title": "Incidunt neque at enim fuga.",
+            "description": "Harum libero quo dolorum aut vel.",
+            "url": "https://placekitten.com/300/400"
+        }
+    ]
+}
+"""
+
 _TEST_PLANTUML_URL = "http://localhost:8080/plantuml/"
 _DEFAULT_PLANTUML_URL = "http://plantuml.com/plantuml/"
 _DEFAULT_FORMAT = "svg"
 
 
 class TestPlantUML(BaseTestCase):
     """Testcase for the PlantUML extension"""
@@ -79,14 +99,33 @@
         print("Testing PlantUML rendering SVG...")
         with self._config(server=_DEFAULT_PLANTUML_URL, out_format="svg") as magic:
             try:
                 magic.plantuml(cell=_SIMPLE_DIAGRAM)
             except Exception as exception:
                 self.fail(f"Error: {exception}")
 
+    def test_render_json(self):
+        """Tests rendering an svg"""
+        print("Testing PlantUML rendering JSON...")
+        with self._config(server=_DEFAULT_PLANTUML_URL, out_format="png") as magic:
+            try:
+                magic.json(cell=_SIMPLE_JSON)
+            except Exception as exception:
+                self.fail(f"Error: {exception}")
+
+        tmp_file = "/tmp/temp_json.json"
+        with open(tmp_file, "w", encoding="UTF-8") as json_file:
+            json_file.write(_SIMPLE_JSON)
+
+        with self._config(server=_DEFAULT_PLANTUML_URL, out_format="png") as magic:
+            try:
+                magic.json(line=f"--json={tmp_file}", cell=None)
+            except Exception as exception:
+                self.fail(f"Error: {exception}")
+
     def test_render_png(self):
         """Tests rendering a png"""
         print("Testing PlantUML rendering PNG...")
         magic = PlantUmlMagics(self.ipython)
         magic.plantuml_config(f"--server={_DEFAULT_PLANTUML_URL}")
         try:
             magic.plantuml(line="--format=png", cell=_AZURE_DIAGRAM)
```

### Comparing `classroom_extensions-0.0.7/tests/test_web.py` & `classroom_extensions-0.0.8/tests/test_web.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         def stdout_callback(data):
             nonlocal where_ls
             where_ls += data
 
         async def run_cmd():
             async with proc_manager.open_process(
                 "ls", "/usr/bin/pwd", stdout_callback=stdout_callback
-            ) :
+            ):
                 pass
 
         asyncio.run(run_cmd())
         self.assertRegex(text=where_ls, expected_regex=r"pwd")
 
     def test_node_script(self):
         """Tests executing server-side JavaScript"""
@@ -63,15 +63,15 @@
             "javascript",
             line=f"--target=disk --filename={tmp_file}",
             cell="console.log('------');\n",
         )
         self.assertEqual(path.exists(tmp_file), True)
         try:
             self.ipython.run_cell_magic(
-                "javascript", line=f"--target=disk", cell="console.log(' ');\n"
+                "javascript", line="--target=disk", cell="console.log(' ');\n"
             )
         except ValueError:
             pass
 
     def test_node_server(self):
         """Tests the creation of a Node.js server"""
         print("Testing executing Node.js server...")
@@ -144,14 +144,17 @@
         expected = "IPython shell not available.\n"
         output = self.capture_output(node_ext.load_ipython_extension, None)
         self.assertEqual(output, expected)
         output = self.capture_output(node_ext.unload_ipython_extension, None)
         self.assertEqual(output, expected)
 
     def test_http_server(self):
-        """ Tests start/stop of HTTP server """
-        self.ipython.run_line_magic("http_server", line="--action=start --bind=0.0.0.0 --port=8000 --directory=/tmp")
+        """Tests start/stop of HTTP server"""
+        self.ipython.run_line_magic(
+            "http_server",
+            line="--action=start --bind=0.0.0.0 --port=8000 --directory=/tmp",
+        )
         self.ipython.run_line_magic("http_server", line="--action=stop --port=8000")
 
 
 if __name__ == "__main__":
     unittest.main()
```

