# Comparing `tmp/thinks_dash_components-0.4.8.tar.gz` & `tmp/thinks_dash_components-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.4.8.tar", last modified: Wed Aug  2 09:45:52 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.4.9.tar", last modified: Wed Aug  2 09:50:06 2023, max compression
```

## Comparing `thinks_dash_components-0.4.8.tar` & `thinks_dash_components-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 09:45:52.474553 thinks_dash_components-0.4.8/
--rw-rw-rw-   0        0        0        0 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.8/LICENSE
--rw-rw-rw-   0        0        0      464 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-08-02 09:45:52.474553 thinks_dash_components-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.8/README.md
--rw-rw-rw-   0        0        0     2373 2023-08-02 09:45:39.000000 thinks_dash_components-0.4.8/package.json
--rw-rw-rw-   0        0        0       42 2023-08-02 09:45:52.475551 thinks_dash_components-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 09:45:52.468569 thinks_dash_components-0.4.8/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1542 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1343 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.8/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2360 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.8/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44750 2023-08-02 09:45:50.000000 thinks_dash_components-0.4.8/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2373 2023-08-02 09:45:49.000000 thinks_dash_components-0.4.8/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   123922 2023-08-02 09:45:48.000000 thinks_dash_components-0.4.8/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-08-02 09:45:48.000000 thinks_dash_components-0.4.8/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-08-02 09:45:52.473556 thinks_dash_components-0.4.8/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-08-02 09:45:52.000000 thinks_dash_components-0.4.8/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-08-02 09:45:52.000000 thinks_dash_components-0.4.8/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 09:45:52.000000 thinks_dash_components-0.4.8/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-02 09:45:52.000000 thinks_dash_components-0.4.8/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 09:50:06.201286 thinks_dash_components-0.4.9/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0      464 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-08-02 09:50:06.200289 thinks_dash_components-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3802 2023-05-31 06:35:24.000000 thinks_dash_components-0.4.9/README.md
+-rw-rw-rw-   0        0        0     2373 2023-08-02 09:49:28.000000 thinks_dash_components-0.4.9/package.json
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:50:06.201286 thinks_dash_components-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      737 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:50:06.194306 thinks_dash_components-0.4.9/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1542 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1343 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.9/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2360 2023-05-31 06:35:25.000000 thinks_dash_components-0.4.9/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44750 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2373 2023-08-02 09:49:39.000000 thinks_dash_components-0.4.9/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   123815 2023-08-02 09:49:37.000000 thinks_dash_components-0.4.9/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-08-02 09:49:37.000000 thinks_dash_components-0.4.9/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-08-02 09:50:06.199292 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-02 09:50:06.000000 thinks_dash_components-0.4.9/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.4.8/PKG-INFO` & `thinks_dash_components-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.4.8
+Version: 0.4.9
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.8/README.md` & `thinks_dash_components-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/package.json` & `thinks_dash_components-0.4.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.9'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.8"
+    "version": "0.4.9"
 }
```

### Comparing `thinks_dash_components-0.4.8/setup.py` & `thinks_dash_components-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/Alert.py` & `thinks_dash_components-0.4.9/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.4.9/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.4.9/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.4.9/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.4.9/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.4.9/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.4.9/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/Notice.py` & `thinks_dash_components-0.4.9/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.4.9/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.4.9/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.4.9/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.4.9/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.4.9/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.4.9/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.4.9/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/__init__.py` & `thinks_dash_components-0.4.9/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.4.9/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/metadata.json` & `thinks_dash_components-0.4.9/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/package-info.json` & `thinks_dash_components-0.4.9/thinks_dash_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.9'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.8"
+    "version": "0.4.9"
 }
```

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.4.9/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 1% similar despite different names*

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
-            return a.splice(1, 0, "v0_4_8m1690969546"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_4_9m1690969775"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3823,15 +3823,15 @@
                     }
                 }
             }, {
                 key: "componentDidUpdate",
                 value: function() {
                     if (JSON.stringify(this.options) !== JSON.stringify(this.props.options)) {
                         var e = this.getOption();
-                        console.log(e), this.options = this.props.options, this.props.setProps({
+                        this.options = this.props.options, this.props.setProps({
                             value: e.value,
                             label: e.label
                         })
                     }
                     this.pos && (this.wrapRef.current.scrollTop = this.pos)
                 }
             }, {
@@ -3859,24 +3859,20 @@
             }, {
                 key: "getOption",
                 value: function() {
                     var e = this.props,
                         t = e.options,
                         r = e.value,
                         n = e.label;
-                    if (null !== r && t) {
-                        var o = t.filter((function(e) {
-                            return e.value == r
-                        }));
-                        if (o.length > 0) return console.log("result:" + o[0], "value:" + r, "label:" + n), {
-                            value: r,
-                            label: n
-                        }
-                    }
-                    return {
+                    return null !== r && t && t.filter((function(e) {
+                        return e.value == r
+                    })).length > 0 ? {
+                        value: r,
+                        label: n
+                    } : {
                         value: null,
                         label: null
                     }
                 }
             }, {
                 key: "render",
                 value: function() {
@@ -3895,15 +3891,15 @@
                             for (l.s(); !(u = l.n()).done;) {
                                 var f = u.value;
                                 c.push(h.a.createElement(at, {
                                     key: f.value,
                                     "data-value": f.value,
                                     "data-label": f.label,
                                     onClick: this.select
-                                }, h.a.createElement("span", null, f.label))), String(f.value) === String(a) && (console.log("test"), console.log("-- MOBILE DROPDOWN", "value:" + a, "label:" + s))
+                                }, h.a.createElement("span", null, f.label))), String(f.value) === String(a) && console.log("-- MOBILE DROPDOWN", "value:" + a, "label:" + s)
                             }
                         } catch (e) {
                             l.e(e)
                         } finally {
                             l.f()
                         }
                     } else c.push(h.a.createElement(at, {
```

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.4.9/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.4.8
+Version: 0.4.9
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.8/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.4.9/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

