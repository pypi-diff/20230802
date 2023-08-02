# Comparing `tmp/thinks_dash_components-0.4.5.tar.gz` & `tmp/thinks_dash_components-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.4.5.tar", last modified: Wed Aug  2 09:09:56 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.4.6.tar", last modified: Wed Aug  2 09:17:16 2023, max compression
```

## Comparing `thinks_dash_components-0.4.5.tar` & `thinks_dash_components-0.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 09:09:56.809927 thinks_dash_components-0.4.5/
--rw-rw-rw-   0        0        0        0 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.5/LICENSE
--rw-rw-rw-   0        0        0      464 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-08-02 09:09:56.808930 thinks_dash_components-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.5/README.md
--rw-rw-rw-   0        0        0     2373 2023-08-02 09:05:32.000000 thinks_dash_components-0.4.5/package.json
--rw-rw-rw-   0        0        0       42 2023-08-02 09:09:56.809927 thinks_dash_components-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 09:09:56.802947 thinks_dash_components-0.4.5/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1542 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1343 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.5/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2360 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.5/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44750 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2373 2023-08-02 09:05:47.000000 thinks_dash_components-0.4.5/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   123815 2023-08-02 09:05:45.000000 thinks_dash_components-0.4.5/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-08-02 09:05:45.000000 thinks_dash_components-0.4.5/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-08-02 09:09:56.807932 thinks_dash_components-0.4.5/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-08-02 09:09:56.000000 thinks_dash_components-0.4.5/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-08-02 09:09:56.000000 thinks_dash_components-0.4.5/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 09:09:56.000000 thinks_dash_components-0.4.5/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-02 09:09:56.000000 thinks_dash_components-0.4.5/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 09:17:16.338034 thinks_dash_components-0.4.6/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-08-02 09:17:16.338034 thinks_dash_components-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3802 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.6/README.md
+-rw-rw-rw-   0        0        0     2373 2023-08-02 09:17:00.000000 thinks_dash_components-0.4.6/package.json
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:17:16.338034 thinks_dash_components-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:17:16.332049 thinks_dash_components-0.4.6/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1542 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1343 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.6/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2360 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.6/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44750 2023-08-02 09:17:12.000000 thinks_dash_components-0.4.6/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2373 2023-08-02 09:17:11.000000 thinks_dash_components-0.4.6/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   123884 2023-08-02 09:17:10.000000 thinks_dash_components-0.4.6/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-08-02 09:17:10.000000 thinks_dash_components-0.4.6/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-08-02 09:17:16.336039 thinks_dash_components-0.4.6/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-08-02 09:17:16.000000 thinks_dash_components-0.4.6/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-08-02 09:17:16.000000 thinks_dash_components-0.4.6/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:17:16.000000 thinks_dash_components-0.4.6/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-02 09:17:16.000000 thinks_dash_components-0.4.6/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.4.5/PKG-INFO` & `thinks_dash_components-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.4.5
+Version: 0.4.6
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.5/README.md` & `thinks_dash_components-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/package.json` & `thinks_dash_components-0.4.6/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.6'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.5"
+    "version": "0.4.6"
 }
```

### Comparing `thinks_dash_components-0.4.5/setup.py` & `thinks_dash_components-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/Alert.py` & `thinks_dash_components-0.4.6/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.4.6/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.4.6/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.4.6/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.4.6/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.4.6/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.4.6/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/Notice.py` & `thinks_dash_components-0.4.6/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.4.6/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.4.6/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.4.6/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.4.6/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.4.6/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.4.6/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.4.6/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/__init__.py` & `thinks_dash_components-0.4.6/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.4.6/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/metadata.json` & `thinks_dash_components-0.4.6/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/package-info.json` & `thinks_dash_components-0.4.6/thinks_dash_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.6'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.5"
+    "version": "0.4.6"
 }
```

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.4.6/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 r = i(e);
             if (!t) return r;
             var n = r.split("/"),
                 a = n.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_4_5m1690967143"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_4_6m1690967828"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3859,20 +3859,24 @@
             }, {
                 key: "getOption",
                 value: function() {
                     var e = this.props,
                         t = e.options,
                         r = e.value,
                         n = e.label;
-                    return null !== r && t && t.filter((function(e) {
-                        return e.value == r
-                    })).length > 0 ? {
-                        value: r,
-                        label: n
-                    } : {
+                    if (null !== r && t) {
+                        var o = t.filter((function(e) {
+                            return e.value == r
+                        }));
+                        if (o.length > 0) return console.log("result:", o[0], "value:", r, "label", n), {
+                            value: r,
+                            label: n
+                        }
+                    }
+                    return {
                         value: null,
                         label: null
                     }
                 }
             }, {
                 key: "render",
                 value: function() {
```

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.4.6/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.4.5
+Version: 0.4.6
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.5/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.4.6/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

