# Comparing `tmp/plastik-0.4.3.tar.gz` & `tmp/plastik-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastik-0.4.3.tar", max compression
+gzip compressed data, was "plastik-0.5.0.tar", max compression
```

## Comparing `plastik-0.4.3.tar` & `plastik-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-26 08:32:12.863410 plastik-0.4.3/LICENSE
--rw-r--r--   0        0        0      820 2023-06-26 08:32:28.263753 plastik-0.4.3/README.md
--rw-r--r--   0        0        0     1072 2023-06-26 08:32:28.263753 plastik-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      263 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/__init__.py
--rw-r--r--   0        0        0     2852 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/axes.py
--rw-r--r--   0        0        0    11084 2023-06-26 08:32:28.263753 plastik-0.4.3/src/plastik/colors.py
--rw-r--r--   0        0        0      942 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/default.mplstyle
--rw-r--r--   0        0        0     5514 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/legends.py
--rw-r--r--   0        0        0    12220 2023-06-26 08:32:12.875410 plastik-0.4.3/src/plastik/ridge.py
--rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 plastik-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-02 08:16:31.958266 plastik-0.5.0/LICENSE
+-rw-r--r--   0        0        0      800 2023-08-02 08:16:31.958266 plastik-0.5.0/README.md
+-rw-r--r--   0        0        0     1072 2023-08-02 08:16:45.342689 plastik-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-08-02 08:16:31.982266 plastik-0.5.0/src/plastik/__init__.py
+-rw-r--r--   0        0        0     1082 2023-08-02 08:16:31.982266 plastik-0.5.0/src/plastik/axes.py
+-rw-r--r--   0        0        0    11402 2023-08-02 08:16:31.982266 plastik-0.5.0/src/plastik/colors.py
+-rw-r--r--   0        0        0     1005 2023-08-02 08:16:31.982266 plastik-0.5.0/src/plastik/default.mplstyle
+-rw-r--r--   0        0        0     5514 2023-08-02 08:16:31.982266 plastik-0.5.0/src/plastik/legends.py
+-rw-r--r--   0        0        0    12220 2023-08-02 08:16:31.982266 plastik-0.5.0/src/plastik/ridge.py
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 plastik-0.5.0/PKG-INFO
```

### Comparing `plastik-0.4.3/LICENSE` & `plastik-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plastik-0.4.3/README.md` & `plastik-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 ```
 
 ## Usage
 
 ### Functions
 
 - `dark_theme`
-- `log_tick_format`
 - `topside_legends`
 
 ### Classes
 
 - `Ridge`
 
 ### Example use
```

### Comparing `plastik-0.4.3/pyproject.toml` & `plastik-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plastik"
-version = "0.4.3"
+version = "0.5.0"
 description = "plastic surgery for plt"
 authors = ["Eirik Rolland Enger <eirroleng@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/engeir/plastik"
 repository = "https://github.com/engeir/plastik"
 documentation = "https://plastik.readthedocs.io/en/latest/"
```

### Comparing `plastik-0.4.3/src/plastik/colors.py` & `plastik-0.5.0/src/plastik/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -252,16 +252,16 @@
 
     >>> custom = viridis.copy()
     >>> for _ in range(3):
     ...     custom.append("#6543ff")
     >>> for _ in range(3):
     ...     custom.insert(0, "#2eff2e")
 
-    Plot the color_map alone. The ``figsize`` parameter exactly defines the shape of the
-    colour swatch.
+    Plot the ``color_map`` alone. The ``figsize`` parameter exactly defines the shape of
+    the colour swatch.
 
     >>> plt.figure(figsize=(10, 1), layout="constrained")
     >>> plastik.colors.make_color_swatch(plt.gca(), custom, no_ticks=False)
 
     Then, as an inset with other data.
 
     >>> plt.figure()
@@ -269,17 +269,24 @@
     >>> x0, y0, width, height = 0.52, 0.8, 0.40, 0.15
     >>> ax.scatter(
     ...     np.arange(len(custom)),
     ...     np.ones(len(custom)),
     ...     c=custom,
     ... )
     >>> ax2 = ax.inset_axes([x0, y0, width, height])
-    >>> plastik.colors.make_color_swatch(
+    >>> ax2 = plastik.colors.make_color_swatch(
     ...     ax2, custom, ratio=2 * len(custom), no_border=True
     ... )
+
+    You can make a custom label with the returned axis element's ``set_xticks`` (or
+    ``set_yticks``), where ``length`` is the length of the given ``c_bar`` list or equal
+    to the resolution.
+
+    >>> length = len(custom)
+    >>> ax2.set_xticks(list(range(length)), [f"No: {i}" for i in range(length)])
     >>> plt.show()
     """
     if isinstance(c_bar, list):
         row_col = "columns" if vertical else "rows"
         kwarg = {row_col: 1}
         pywaffle.Waffle.make_waffle(
             ax=ax,
```

### Comparing `plastik-0.4.3/src/plastik/default.mplstyle` & `plastik-0.5.0/src/plastik/default.mplstyle`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,9 @@
 xtick.top : True
 xtick.bottom : True
 ytick.left : True
 ytick.right : True
 # All ticks point inward
 xtick.direction : "in"
 ytick.direction : "in"
+# Tick formatting in log scale
+axes.formatter.min_exponent : 2
```

### Comparing `plastik-0.4.3/src/plastik/legends.py` & `plastik-0.5.0/src/plastik/legends.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.3/src/plastik/ridge.py` & `plastik-0.5.0/src/plastik/ridge.py`

 * *Files identical despite different names*

### Comparing `plastik-0.4.3/PKG-INFO` & `plastik-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastik
-Version: 0.4.3
+Version: 0.5.0
 Summary: plastic surgery for plt
 Home-page: https://github.com/engeir/plastik
 License: GPLv3
 Author: Eirik Rolland Enger
 Author-email: eirroleng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -48,15 +48,14 @@
 ```
 
 ## Usage
 
 ### Functions
 
 - `dark_theme`
-- `log_tick_format`
 - `topside_legends`
 
 ### Classes
 
 - `Ridge`
 
 ### Example use
```

