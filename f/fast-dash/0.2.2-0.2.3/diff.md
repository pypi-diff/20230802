# Comparing `tmp/fast_dash-0.2.2.tar.gz` & `tmp/fast_dash-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dash-0.2.2.tar", max compression
+gzip compressed data, was "fast_dash-0.2.3.tar", max compression
```

## Comparing `fast_dash-0.2.2.tar` & `fast_dash-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-07-26 23:53:13.759936 fast_dash-0.2.2/LICENSE
--rw-r--r--   0        0        0     3824 2023-07-26 23:53:13.759936 fast_dash-0.2.2/README.md
--rw-r--r--   0        0        0    34285 2023-07-26 23:53:13.803936 fast_dash-0.2.2/fast_dash/Components.py
--rw-r--r--   0        0        0      655 2023-07-26 23:53:13.803936 fast_dash-0.2.2/fast_dash/__init__.py
--rw-r--r--   0        0        0    24457 2023-07-26 23:53:13.807936 fast_dash-0.2.2/fast_dash/assets/favicon.ico
--rw-r--r--   0        0        0    17282 2023-07-26 23:53:13.807936 fast_dash-0.2.2/fast_dash/fast_dash.py
--rw-r--r--   0        0        0     7667 2023-07-26 23:53:13.807936 fast_dash-0.2.2/fast_dash/utils.py
--rw-r--r--   0        0        0     2325 2023-07-26 23:53:13.807936 fast_dash-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       39 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      314 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     3538 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/examples.py
--rw-r--r--   0        0        0     2709 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/test_examples.py
--rw-r--r--   0        0        0     6261 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/test_fast_dash.py
--rw-r--r--   0        0        0    21632 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/test_fast_dash_autodetect.py
--rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 fast_dash-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-01 23:16:06.350666 fast_dash-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4946 2023-08-01 23:16:06.350666 fast_dash-0.2.3/README.md
+-rw-r--r--   0        0        0    35310 2023-08-01 23:16:06.398667 fast_dash-0.2.3/fast_dash/Components.py
+-rw-r--r--   0        0        0      678 2023-08-01 23:16:06.398667 fast_dash-0.2.3/fast_dash/__init__.py
+-rw-r--r--   0        0        0    24457 2023-08-01 23:16:06.398667 fast_dash-0.2.3/fast_dash/assets/favicon.ico
+-rw-r--r--   0        0        0    17381 2023-08-01 23:16:06.398667 fast_dash-0.2.3/fast_dash/fast_dash.py
+-rw-r--r--   0        0        0    10746 2023-08-01 23:16:06.398667 fast_dash-0.2.3/fast_dash/utils.py
+-rw-r--r--   0        0        0     2325 2023-08-01 23:16:06.398667 fast_dash-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-08-01 23:16:06.398667 fast_dash-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      314 2023-08-01 23:16:06.398667 fast_dash-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     3538 2023-08-01 23:16:06.398667 fast_dash-0.2.3/tests/examples.py
+-rw-r--r--   0        0        0     2709 2023-08-01 23:16:06.398667 fast_dash-0.2.3/tests/test_examples.py
+-rw-r--r--   0        0        0     6261 2023-08-01 23:16:06.398667 fast_dash-0.2.3/tests/test_fast_dash.py
+-rw-r--r--   0        0        0    23644 2023-08-01 23:16:06.398667 fast_dash-0.2.3/tests/test_fast_dash_autodetect.py
+-rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 fast_dash-0.2.3/PKG-INFO
```

### Comparing `fast_dash-0.2.2/LICENSE` & `fast_dash-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.2/README.md` & `fast_dash-0.2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ```python
 from fast_dash import fastdash
 
 @fastdash
 def text_to_text_function(input_text):
     return input_text
 
-# * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
+# * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
 ```
 
 And just like that (🪄), we have a completely functional interactive app!
 
 Output:
 ![Simple example](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20text%20to%20text.png)
 ---
@@ -70,37 +70,69 @@
 
 ```python
 from fast_dash import fastdash
 
 @fastdash
 def display_selected_text_and_number(text: str, number: int) -> str:
     "Simply display the selected text and number"
+
     processed_text = f'Selected text is {text} and the number is {number}.'
+    
     return processed_text
 
-# * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
+# * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
 ```
 
 Output:
 ![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20example%202.png)
 
 And with just a few more lines, we can add a title icon, subheader and other social branding details.
 
 ---
 
+Output components can be arranged using a mosaic layout (ASCII art), inspired from Matplotlib's `subplot_mosaic` feature.
+
+```python
+from fast_dash import fastdash, UploadImage, Graph
+import matplotlib.pyplot as plt
+
+mosaic = """
+AB
+AC
+"""
+
+@fastdash(mosaic=mosaic, theme="BOOTSTRAP")
+def multiple_output_components(start_date: datetime.date, # Adds a date component
+                            upload_image: UploadImage, # Adds an upload component
+                            fips: str = [List of FIPs]) # Adds a single select dropdown
+                            -> (Graph, plt.Figure, plt.Figure): 
+                            # Output components are a Plotly graph, and two figure components
+
+    "Fast Dash allows using mosaic arrays to arrange output components"
+
+    choropleth_map = ...
+    histogram = ...
+    radar_chart = ...
+    
+    return chloropleth_map, histogram, radar_chart
+
+# * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
+```
+![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.2.3/Multiple%20components%20using%20mosaic.png)
+
 ## About
 
 Read different ways to build Fast Dash apps and additional details by navigating to the [project documentation](https://docs.fastdash.app/).
 
 ### Key features
 
-- Launch an app by adding a decorator only.
-- Use multiple input and output components simultaneously.
-- Flask-based backend allows easy scalability and customizability.
-- Build fast, share and iterate.
+- Deploy an app just by adding a decorator
+- Components are inferred from function type hints. Allows using Dash components as type hints.
+- Use multiple input and output components simultaneously
+- Build fast, share and iterate
 
 ## Community
 
 Fast Dash is built using [Plotly Dash](https://github.com/plotly/dash) and it's completely open-source.
 
 ## Citation
 Please cite Fast Dash it if you use it in your work.
```

### Comparing `fast_dash-0.2.2/fast_dash/Components.py` & `fast_dash-0.2.3/fast_dash/Components.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import numpy as np
 import PIL
 import plotly.graph_objs as go
 from dash import Input, Output, State, dcc, html
 from dash_iconify import DashIconify
 from PIL import ImageFile
 
-from .utils import Fastify, _pil_to_b64
+from .utils import Fastify, _pil_to_b64, _get_default_property
 
 
 class BaseLayout:
     def __init__(
         self,
         mosaic=None,
         inputs=None,
@@ -689,14 +689,22 @@
         FastComponent: Component that can be used to represent the given input.
     """
 
     # If hint has the attribute "component_property", it indicates that hint is a FastComponent, return it
     if hasattr(hint, "component_property"):
         return hint
 
+    # Elif the component is a Dash component, use the specified component_property
+    # If one isn't specified, get the default component_property
+    # If not even that assign it the component_property "value" and return the FastComponent.
+    elif isinstance(type(hint), dash.development.base_component.ComponentMeta):
+        default_component_property = _get_default_property(type(hint))
+
+        return Fastify(component=hint, component_property=default_component_property)
+
     # If hint is not type, assume that the user specified an object. Change it to type
     if not isinstance(hint, type):
         hint = type(hint)
 
     _hint_type = _map_types_to_readable_names.get(hint)
     _default_value_type = _map_types_to_readable_names.get(type(default_value))
 
@@ -949,14 +957,24 @@
     return component
 
 
 def _get_output_components(_hint_type):
     if hasattr(_hint_type, "component_property"):
         return _hint_type
 
+    # Elif the component is a Dash component, use the specified component_property
+    # If one isn't specified, get the default component_property
+    # If not even that assign it the component_property "value" and return the FastComponent.
+    elif isinstance(type(_hint_type), dash.development.base_component.ComponentMeta):
+        default_component_property = _get_default_property(type(_hint_type))
+
+        return Fastify(
+            component=_hint_type, component_property=default_component_property
+        )
+
     # If hint is not type, assume that the user specified an object. Change it to type
     if not isinstance(_hint_type, type):
         _hint_type = type(_hint_type)
 
     if issubclass(_hint_type, PIL.ImageFile.ImageFile):
         component = Image
```

### Comparing `fast_dash-0.2.2/fast_dash/__init__.py` & `fast_dash-0.2.3/fast_dash/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Fast Dash."""
 
 __author__ = """Kedar Dabhadkar"""
 __email__ = "kedar@fastdash.app"
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from fast_dash.Components import (
     Graph,
     Image,
     Slider,
     Text,
     TextArea,
@@ -14,14 +14,15 @@
     UploadImage,
     acknowledge_image_component,
     dbc,
     dcc,
     dmc,
     html,
 )
+import dash
 from fast_dash.fast_dash import FastDash, fastdash
 from fast_dash.utils import Fastify
 
 __all__ = [
     "FastDash",
     "fastdash",
     "Fastify",
@@ -33,8 +34,9 @@
     "UploadImage",
     "Image",
     "Graph",
     "dcc",
     "dbc",
     "dmc",
     "html",
+    "dash"
 ]
```

### Comparing `fast_dash-0.2.2/fast_dash/assets/favicon.ico` & `fast_dash-0.2.3/fast_dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.2/fast_dash/fast_dash.py` & `fast_dash-0.2.3/fast_dash/fast_dash.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,20 +169,22 @@
         self.theme = theme or "JOURNAL"
         self.minimal = minimal
 
         # Assign IDs to components
         self.inputs_with_ids = _assign_ids_to_inputs(self.inputs, self.callback_fn)
         self.outputs_with_ids = _assign_ids_to_outputs(self.outputs)
         self.ack_mask = [
-            True if input_.ack is not None else False for input_ in self.inputs_with_ids
+            False if (not hasattr(input_, "ack") or (input_.ack is None)) else True
+            for input_ in self.inputs_with_ids
         ]
 
         # Default state of outputs
         self.output_state_default = [
-            output_.placeholder for output_ in self.outputs_with_ids
+            output_.placeholder if hasattr(output_, "placeholder") else None
+            for output_ in self.outputs_with_ids
         ]
 
         # Define Flask server
         server = flask.Flask(__name__)
         external_stylesheets = [
             theme_mapper(self.theme),
             "https://use.fontawesome.com/releases/v5.9.0/css/all.css",
```

### Comparing `fast_dash-0.2.2/pyproject.toml` & `fast_dash-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "fast_dash"
-version = "0.2.2"
+version = "0.2.3"
 homepage = "https://github.com/dkedar7/fast_dash"
 description = "Build Machine Learning prototypes web applications lightning fast."
 authors = ["Kedar Dabhadkar <kedar@fastdash.app>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `fast_dash-0.2.2/tests/examples.py` & `fast_dash-0.2.3/tests/examples.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.2/tests/test_examples.py` & `fast_dash-0.2.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.2/tests/test_fast_dash.py` & `fast_dash-0.2.3/tests/test_fast_dash.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.2/tests/test_fast_dash_autodetect.py` & `fast_dash-0.2.3/tests/test_fast_dash_autodetect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 """Tests for `fast_dash` package."""
 # pylint: disable=redefined-outer-name
 
-from fast_dash import FastDash, dcc, dbc, html
+from fast_dash import FastDash, dcc, dbc, dmc, html
 from fast_dash.Components import Text, Slider, UploadImage
 from fast_dash.utils import _pil_to_b64
 
 import time
 import datetime
 
 
@@ -15,15 +15,14 @@
     "Converts text to text"
     return input_text
 
 
 def simple_number_to_number(input_: Slider):
     return input_
 
-
 def simple_image_to_image(input_: UploadImage):
     return UploadImage
 
 
 def simple_text_to_multiple_text_function(input_text):
     return input_text, input_text
 
@@ -685,7 +684,73 @@
     output_component = app.outputs[0]
 
     assert (
         output_component.__doc__ == html.Img.__doc__
         and hasattr(output_component, "component_property")
         and output_component.component_property == "src"
     )
+
+
+def test_fdco015_input_is_dash_component(dash_duo):
+    "When the input hint type is a Dash component"
+
+    # Component property is specified
+    component = dmc.Text()
+    component.component_property = "children"
+
+    def simple_text_to_text(text: component):
+        return "Some markdown text"
+
+    app = FastDash(callback_fn=simple_text_to_text)
+    input_component = app.inputs[0]
+
+    assert (
+        input_component.__doc__ == dmc.Text.__doc__
+        and hasattr(input_component, "component_property")
+        and input_component.component_property == "children"
+    )
+
+    # Component property is not specified
+    def simple_text_to_text(text: dmc.Text()):
+        return "Some markdown text"
+
+    app = FastDash(callback_fn=simple_text_to_text)
+    input_component = app.inputs[0]
+
+    assert (
+        input_component.__doc__ == dmc.Text.__doc__
+        and hasattr(input_component, "component_property")
+        and input_component.component_property == "children"
+    )
+
+
+def test_fdco016_output_is_dash_component(dash_duo):
+    "When the output hint type is a Dash component"
+
+    # Component property is specified
+    component = dcc.Markdown()
+    component.component_property = "children"
+
+    def simple_text_to_text(text) -> component:
+        return "Some markdown text"
+
+    app = FastDash(callback_fn=simple_text_to_text)
+    output_component = app.outputs[0]
+
+    assert (
+        output_component.__doc__ == dcc.Markdown.__doc__
+        and hasattr(output_component, "component_property")
+        and output_component.component_property == "children"
+    )
+
+    # Component property is not specified
+    def simple_text_to_text(text) -> dcc.Markdown():
+        return "Some markdown text"
+
+    app = FastDash(callback_fn=simple_text_to_text)
+    output_component = app.outputs[0]
+
+    assert (
+        output_component.__doc__ == dcc.Markdown.__doc__
+        and hasattr(output_component, "component_property")
+        and output_component.component_property == "children"
+    )
```

### Comparing `fast_dash-0.2.2/PKG-INFO` & `fast_dash-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-dash
-Version: 0.2.2
+Version: 0.2.3
 Summary: Build Machine Learning prototypes web applications lightning fast.
 Home-page: https://github.com/dkedar7/fast_dash
 License: MIT
 Author: Kedar Dabhadkar
 Author-email: kedar@fastdash.app
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -84,15 +84,15 @@
 ```python
 from fast_dash import fastdash
 
 @fastdash
 def text_to_text_function(input_text):
     return input_text
 
-# * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
+# * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
 ```
 
 And just like that (🪄), we have a completely functional interactive app!
 
 Output:
 ![Simple example](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20text%20to%20text.png)
 ---
@@ -103,37 +103,69 @@
 
 ```python
 from fast_dash import fastdash
 
 @fastdash
 def display_selected_text_and_number(text: str, number: int) -> str:
     "Simply display the selected text and number"
+
     processed_text = f'Selected text is {text} and the number is {number}.'
+    
     return processed_text
 
-# * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
+# * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
 ```
 
 Output:
 ![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.2.1/Simple%20example%202.png)
 
 And with just a few more lines, we can add a title icon, subheader and other social branding details.
 
 ---
 
+Output components can be arranged using a mosaic layout (ASCII art), inspired from Matplotlib's `subplot_mosaic` feature.
+
+```python
+from fast_dash import fastdash, UploadImage, Graph
+import matplotlib.pyplot as plt
+
+mosaic = """
+AB
+AC
+"""
+
+@fastdash(mosaic=mosaic, theme="BOOTSTRAP")
+def multiple_output_components(start_date: datetime.date, # Adds a date component
+                            upload_image: UploadImage, # Adds an upload component
+                            fips: str = [List of FIPs]) # Adds a single select dropdown
+                            -> (Graph, plt.Figure, plt.Figure): 
+                            # Output components are a Plotly graph, and two figure components
+
+    "Fast Dash allows using mosaic arrays to arrange output components"
+
+    choropleth_map = ...
+    histogram = ...
+    radar_chart = ...
+    
+    return chloropleth_map, histogram, radar_chart
+
+# * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
+```
+![Simple example with multiple inputs](https://storage.googleapis.com/fast_dash/0.2.3/Multiple%20components%20using%20mosaic.png)
+
 ## About
 
 Read different ways to build Fast Dash apps and additional details by navigating to the [project documentation](https://docs.fastdash.app/).
 
 ### Key features
 
-- Launch an app by adding a decorator only.
-- Use multiple input and output components simultaneously.
-- Flask-based backend allows easy scalability and customizability.
-- Build fast, share and iterate.
+- Deploy an app just by adding a decorator
+- Components are inferred from function type hints. Allows using Dash components as type hints.
+- Use multiple input and output components simultaneously
+- Build fast, share and iterate
 
 ## Community
 
 Fast Dash is built using [Plotly Dash](https://github.com/plotly/dash) and it's completely open-source.
 
 ## Citation
 Please cite Fast Dash it if you use it in your work.
```

