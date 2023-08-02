# Comparing `tmp/toui-3.1.0.tar.gz` & `tmp/toui-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.1.0.tar", last modified: Mon Jul 31 18:10:06 2023, max compression
+gzip compressed data, was "toui-3.2.0.tar", last modified: Wed Aug  2 10:48:01 2023, max compression
```

## Comparing `toui-3.1.0.tar` & `toui-3.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.757574 toui-3.1.0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.1.0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4263 2023-07-31 18:10:06.756574 toui-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.478056 toui-3.1.0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.1.0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.1.0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.1.0/examples/advanced_example_2_toui_with_javascript.py
--rw-rw-rw-   0        0        0     2119 2023-07-30 07:47:07.000000 toui-3.1.0/examples/advanced_example_3_toui_with_google_sign_in.py
--rw-rw-rw-   0        0        0     3663 2023-07-31 16:08:00.000000 toui-3.1.0/examples/advanced_example_4_toui_with_firebase.py
--rw-rw-rw-   0        0        0     2841 2023-07-31 18:06:31.000000 toui-3.1.0/examples/advanced_example_5_toui_with_sql_user_database.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.483569 toui-3.1.0/images/
--rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.1.0/images/icon.png
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.1.0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-07-31 18:10:06.757574 toui-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.484567 toui-3.1.0/tests/
--rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.1.0/tests/test_examples.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.746452 toui-3.1.0/toui/
--rw-rw-rw-   0        0        0      283 2023-07-31 16:05:00.000000 toui-3.1.0/toui/__init__.py
--rw-rw-rw-   0        0        0     2511 2023-07-29 20:14:41.000000 toui-3.1.0/toui/_cmd.py
--rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.1.0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.1.0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.1.0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.1.0/toui/_signals.py
--rw-rw-rw-   0        0        0    50682 2023-07-31 18:08:02.000000 toui-3.1.0/toui/apps.py
--rw-rw-rw-   0        0        0    23301 2023-07-30 11:21:47.000000 toui-3.1.0/toui/elements.py
--rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.1.0/toui/exceptions.py
--rw-rw-rw-   0        0        0    21645 2023-07-30 09:16:10.000000 toui-3.1.0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.1.0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.755721 toui-3.1.0/toui.egg-info/
--rw-rw-rw-   0        0        0     4263 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      217 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.587409 toui-3.2.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4263 2023-08-02 10:48:01.587409 toui-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.495270 toui-3.2.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.2.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.2.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.2.0/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     2119 2023-07-30 07:47:07.000000 toui-3.2.0/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3663 2023-07-31 16:08:00.000000 toui-3.2.0/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0     2806 2023-08-02 09:47:46.000000 toui-3.2.0/examples/advanced_example_5_toui_with_sql_user_database.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-08-02 09:47:39.000000 toui-3.2.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.2.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.506632 toui-3.2.0/images/
+-rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.2.0/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.2.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:48:01.588934 toui-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.510161 toui-3.2.0/tests/
+-rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.2.0/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.567290 toui-3.2.0/toui/
+-rw-rw-rw-   0        0        0      283 2023-08-02 09:40:36.000000 toui-3.2.0/toui/__init__.py
+-rw-rw-rw-   0        0        0     2511 2023-07-29 20:14:41.000000 toui-3.2.0/toui/_cmd.py
+-rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.2.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.2.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.2.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.2.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    50682 2023-07-31 18:08:02.000000 toui-3.2.0/toui/apps.py
+-rw-rw-rw-   0        0        0    25891 2023-08-02 09:51:19.000000 toui-3.2.0/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.2.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    21832 2023-08-02 09:51:30.000000 toui-3.2.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.2.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:48:01.585411 toui-3.2.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     4263 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      217 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-02 10:48:01.000000 toui-3.2.0/toui.egg-info/top_level.txt
```

### Comparing `toui-3.1.0/LICENSE` & `toui-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/PKG-INFO` & `toui-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.1.0
+Version: 3.2.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.1.0/README.md` & `toui-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/advanced_example_1_toui_blueprint.py` & `toui-3.2.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/advanced_example_2_toui_with_javascript.py` & `toui-3.2.0/examples/advanced_example_2_toui_with_javascript.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/advanced_example_3_toui_with_google_sign_in.py` & `toui-3.2.0/examples/advanced_example_3_toui_with_google_sign_in.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/advanced_example_4_toui_with_firebase.py` & `toui-3.2.0/examples/advanced_example_4_toui_with_firebase.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/advanced_example_5_toui_with_sql_user_database.py` & `toui-3.2.0/examples/advanced_example_5_toui_with_sql_user_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,14 @@
        <button id="sign-up">Sign up</button>
        <p id="output"></p>
    </body>
    </html>
 
 Python code:
 """
-import sys
-sys.path.append("..")
 import os
 from toui import Website, Page
 
 app = Website(__name__, assets_folder="assets", secret_key="some text")
 SQL_URI = f"sqlite:///{os.getcwd()}/.test.db" # Change this value to match your SQL database URI
 app.add_user_database_using_sql(SQL_URI, other_columns=["age"]) # Connects to sql database.
 main_pg = Page(html_file="assets/test8.html", url="/")
```

### Comparing `toui-3.1.0/examples/example_1_simple_website.py` & `toui-3.2.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/example_2_simple_desktop_app.py` & `toui-3.2.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/example_3_updating_page.py` & `toui-3.2.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/example_4_function_with_arg.py` & `toui-3.2.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/examples/example_5_user_variables.py` & `toui-3.2.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/images/icon.png` & `toui-3.2.0/images/icon.png`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/images/logo.png` & `toui-3.2.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/setup.py` & `toui-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui/_cmd.py` & `toui-3.2.0/toui/_cmd.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui/_helpers.py` & `toui-3.2.0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui/_javascript_templates.py` & `toui-3.2.0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui/_signals.py` & `toui-3.2.0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui/apps.py` & `toui-3.2.0/toui/apps.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui/elements.py` & `toui-3.2.0/toui/elements.py`

 * *Files 14% similar despite different names*

```diff
@@ -331,35 +331,41 @@
                     selector += ":nth-of-type(" + str(index) + ")"
 
             path.insert(0, selector)
             element = element.parent
 
         return ' > '.join(path)
 
-    def get_attr(self, name):
+    def get_attr(self, name, default=None):
         """
         Gets the value of an HTML element attribute.
 
         Parameters
         ----------
         name: str
             The name of the attribute.
 
+        default: Any, default=None
+            The value to return if the attribute does not exist.
+
         Returns
         -------
         str
          If the attribute exists.
 
-        None
-            If the attribute does not exist.
+        None, Any
+            ``None`` will be returned the attribute does not exist. However, if a `default` value is specified,
+            it will be returned instead.
 
         """
         value = self._element.attrs.get(name)
         if type(value) == list:
             value = ' '.join(value)
+        if value is None:
+            value = default
         return value
 
     @_ElementSignal()
     def set_attr(self, name, value):
         """
         Sets the value of an HTML element attribute.
 
@@ -401,55 +407,67 @@
         name: str
             The name of the attribute.
 
         """
         if self.has_attr(name):
             del self._element.attrs[name]
 
-    def get_id(self):
+    def get_id(self, default=None):
         """
         Gets the ``id`` attribute of the HTML element.
 
+        Parameters
+        ----------
+        default: Any, default=None
+            The value to return if the attribute does not exist.
+
         Returns
         -------
         str
          If the attribute exists.
 
-        None
-            If the attribute does not exist.
+        None, Any
+            Retuns ``None`` if the attribute does not exist. However, if a `default` value is specified,
+            it will be returned instead.
 
         """
-        return self.get_attr("id")
+        return self.get_attr("id", default=default)
 
     def set_id(self, value):
         """
         Sets the value of the ``id`` attribute.
 
         Parameters
         ----------
         value
             The new value of the ``id`` attribute.
 
         """
         self.set_attr("id", value)
 
-    def get_value(self):
+    def get_value(self, default=None):
         """
         Gets the ``value`` attribute of the HTML element.
 
+        Parameters
+        ----------
+        default: Any, default=None
+            The value to return if the attribute does not exist.
+
         Returns
         -------
         str
             If the attribute exists.
 
-        None
-            If the attribute does not exist.
+        None, Any
+            Retuns ``None`` if the attribute does not exist. However, if a `default` value is specified,
+            it will be returned instead.
 
         """
-        return self.get_attr("value")
+        return self.get_attr("value", default=default)
     
     def get_selected(self) -> 'Element':
         """
         Gets the selected option of the HTML element ``<select>``.
 
         This method is used for ``<select>`` elements only.
 
@@ -549,39 +567,48 @@
 
         """
         self._manage_content_functions(content)
         content = str(content)
         content = BeautifulSoup(content, features="html.parser")
         self._element.append(content)
 
-    def get_style_property(self, property):
+    def get_style_property(self, property, default=None):
         """
         Gets the value of a CSS property inside the ``style`` attribute.
 
         Parameters
         ----------
         property: str
             The name of the property
 
+        default: Any, default=None
+            The value to return if the property does not exist or the ``style`` attribute does not exist.
+
         Returns
         -------
         str
+            If the property exists.
+
+        None, Any
+            Retuns ``None`` if the property does not exist or the ``style`` attribute does not exist.
+            However, if a `default` value is specified, it will be returned instead.
 
         """
         if not self.has_attr("style"):
-            return
+            return default
         style = self.get_attr('style')
         parser = tinycss.make_parser("page3")
         declarations = parser.parse_style_attr(style)[0]
         for declaration in declarations:
             if declaration.name == property:
                 property_value = ""
                 for v in declaration.value:
                     property_value += v.as_css()
                 return property_value
+        return default
 
     def set_style_property(self, property, value):
         """
         Sets the value of a CSS property inside the ``style`` attribute.
 
         Parameters
         ----------
@@ -610,46 +637,66 @@
                 for v in declaration.value:
                     property_value += v.as_css()
             new_style += f"{property_value};"
         if not property_is_set:
             new_style += f"{property}: {value};"
         self.set_attr(name="style", value=new_style)
 
-    def get_width_property(self):
+    def get_width_property(self, default=None):
         """
         Gets the value of the CSS property `width` inside the ``style`` attribute.
 
+        Parameters
+        ----------
+        default: Any, default=None
+            The value to return if the property does not exist or the ``style`` attribute does not exist.
+
         Returns
         -------
         str
+            If the property exists.
+
+        None, Any
+            Retuns ``None`` if the property does not exist or the ``style`` attribute does not exist.
+            However, if a `default` value is specified, it will be returned instead.
 
         """
-        return self.get_style_property("width")
+        return self.get_style_property("width", default=default)
 
     def set_width_property(self, value):
         """
         Sets the value of the CSS property `width` inside the ``style`` attribute.
 
         Parameters
         ----------
         value: str
 
         """
         self.set_style_property("width", value)
 
-    def get_height_property(self):
+    def get_height_property(self, default=None):
         """
         Gets the value of the CSS property `height` inside the ``style`` attribute.
 
+        Parameters
+        ----------
+        default: Any, default=None
+            The value to return if the property does not exist or the ``style`` attribute does not exist.
+
         Returns
         -------
         str
+            If the property exists.
+
+        None, Any
+            Retuns ``None`` if the property does not exist or the ``style`` attribute does not exist.
+            However, if a `default` value is specified, it will be returned instead.
 
         """
-        return self.get_style_property("height")
+        return self.get_style_property("height", default=default)
 
     def set_height_property(self, value):
         """
         Sets the value of the CSS property `height` inside the ``style`` attribute.
 
         Parameters
         ----------
@@ -669,14 +716,19 @@
     def on(self, event, func_or_name, *func_args, quotes=True, return_itself=False):
         """
         Creates an HTML event attribute and adds a Python function to it.
 
         If you want to add JavaScript code instead of a single function, use `Element.set_attr` method
         instead.
 
+        Warning
+        -------
+        If you added a Python function, users might be able to call this function from the client-side. Choose wisely
+        the functions you add.
+
         Parameters
         ----------
         event: str
             Can be any HTML event, but without the "on" prefix.
             For example: `click`, `load`, `mouseover`, etc.
 
         func_or_name: Callable or str
@@ -747,14 +799,19 @@
     def onclick(self, func_or_name, *func_args, quotes=True, return_itself=False):
         """
         Creates the HTML event attribute ``onclick`` and adds a Python function to it.
 
         If you want to add JavaScript code instead of a single function, use `Element.set_attr` method
         instead.
 
+        Warning
+        -------
+        If you added a Python function, users might be able to call this function from the client-side. Choose wisely
+        the functions you add.
+
         Parameters
         ----------
         func_or_name: Callable or str
             The Python function to be called when the event is triggered. If the Python function
             itself is added, the function will be automatically added to the parent `Page`. However,
             if the function name is added, you need to add the Python function itself to the
             parent `Page` manually using the method `Page.add_function`.
```

### Comparing `toui-3.1.0/toui/pages.py` & `toui-3.2.0/toui/pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,19 @@
             return elements[0]
 
     @_PageSignal()
     def add_function(self, func):
         """
         Adds a function to the `Page`. This function can be called from an HTML element.
 
+        Warning
+        -------
+        If you added a Python function, users might be able to call this function from the client-side. Choose wisely
+        the functions you add.
+
         Examples
         --------
 
         Consider an HTML code that contains the following:
 
         >>> html_with_function = '<html><button onclick="printValue()">Print</button></html>'
```

### Comparing `toui-3.1.0/toui/structure.py` & `toui-3.2.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-3.1.0/toui.egg-info/PKG-INFO` & `toui-3.2.0/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.1.0
+Version: 3.2.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.1.0/toui.egg-info/SOURCES.txt` & `toui-3.2.0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

