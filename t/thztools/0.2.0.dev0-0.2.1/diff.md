# Comparing `tmp/thztools-0.2.0.dev0.tar.gz` & `tmp/thztools-0.2.1.tar.gz`

## Comparing `thztools-0.2.0.dev0.tar` & `thztools-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.DS_Store
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.gitattributes
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/simulation-example.ipynb
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/other.xml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.vscode/settings.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/coverage_html.js
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e___init___py.html
--rw-r--r--   0        0        0    46109 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_common_py.html
--rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html
--rw-r--r--   0        0        0    87482 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_messages_py.html
--rw-r--r--   0        0        0   139772 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b___init___py.html
--rw-r--r--   0        0        0    35110 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b__util_py.html
--rw-r--r--   0        0        0   321235 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b_thztools_py.html
--rw-r--r--   0        0        0    43443 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html
--rw-r--r--   0        0        0    20570 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html
--rw-r--r--   0        0        0   107696 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html
--rw-r--r--   0        0        0    34575 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html
--rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/favicon_32.png
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/keybd_open.png
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/htmlReport/style.css
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/.DS_Store
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/__about__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/__init__.py
--rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/src/thztools/thztools.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/LICENSE
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/README.md
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 thztools-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 thztools-0.2.1/.DS_Store
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 thztools-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.2.1/simulation-example.ipynb
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/other.xml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 thztools-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 thztools-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/coverage_html.js
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e___init___py.html
+-rw-r--r--   0        0        0    46109 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_common_py.html
+-rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html
+-rw-r--r--   0        0        0    87482 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_messages_py.html
+-rw-r--r--   0        0        0   139772 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_36ede29a3be77d5b___init___py.html
+-rw-r--r--   0        0        0    35110 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_36ede29a3be77d5b__util_py.html
+-rw-r--r--   0        0        0   321235 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_36ede29a3be77d5b_thztools_py.html
+-rw-r--r--   0        0        0    43443 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html
+-rw-r--r--   0        0        0    20570 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html
+-rw-r--r--   0        0        0   107696 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html
+-rw-r--r--   0        0        0    34575 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html
+-rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/favicon_32.png
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/keybd_open.png
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 thztools-0.2.1/htmlReport/style.css
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.2.1/src/thztools/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.2.1/src/thztools/__about__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 thztools-0.2.1/src/thztools/__init__.py
+-rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 thztools-0.2.1/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 thztools-0.2.1/README.md
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 thztools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 thztools-0.2.1/PKG-INFO
```

### Comparing `thztools-0.2.0.dev0/.DS_Store` & `thztools-0.2.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/simulation-example.ipynb` & `thztools-0.2.1/simulation-example.ipynb`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/.idea/thztools.iml` & `thztools-0.2.1/.idea/thztools.iml`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.2.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/coverage_html.js` & `thztools-0.2.1/htmlReport/coverage_html.js`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e___init___py.html` & `thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e___init___py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_common_py.html` & `thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_common_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html` & `thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_messages_py.html` & `thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_messages_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html` & `thztools-0.2.1/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b___init___py.html` & `thztools-0.2.1/htmlReport/d_36ede29a3be77d5b___init___py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b__util_py.html` & `thztools-0.2.1/htmlReport/d_36ede29a3be77d5b__util_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_36ede29a3be77d5b_thztools_py.html` & `thztools-0.2.1/htmlReport/d_36ede29a3be77d5b_thztools_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html` & `thztools-0.2.1/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html` & `thztools-0.2.1/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html` & `thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html` & `thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html` & `thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html` & `thztools-0.2.1/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/favicon_32.png` & `thztools-0.2.1/htmlReport/favicon_32.png`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/index.html` & `thztools-0.2.1/htmlReport/index.html`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/keybd_closed.png` & `thztools-0.2.1/htmlReport/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/keybd_open.png` & `thztools-0.2.1/htmlReport/keybd_open.png`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/status.json` & `thztools-0.2.1/htmlReport/status.json`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/htmlReport/style.css` & `thztools-0.2.1/htmlReport/style.css`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/src/thztools/.DS_Store` & `thztools-0.2.1/src/thztools/.DS_Store`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/src/thztools/thztools.py` & `thztools-0.2.1/src/thztools/thztools.py`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/.gitignore` & `thztools-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/LICENSE` & `thztools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/README.md` & `thztools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `thztools-0.2.0.dev0/pyproject.toml` & `thztools-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "THzTools"
+name = "thztools"
 dynamic = ["version"]
 description = "Tools for terahertz time-domain spectroscopy (THz-TDS)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["terahertz", "THz", "time-domain spectroscopy", "data analysis"]
 authors = [
```

### Comparing `thztools-0.2.0.dev0/PKG-INFO` & `thztools-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: THzTools
-Version: 0.2.0.dev0
+Name: thztools
+Version: 0.2.1
 Summary: Tools for terahertz time-domain spectroscopy (THz-TDS)
 Project-URL: Documentation, https://dodge-research-group.github.io/thztools/
 Project-URL: Issues, https://github.com/dodge-research-group/thztools/issues
 Project-URL: Source, https://github.com/dodge-research-group/thztools
 Author-email: Steve Dodge <jsdodge@sfu.ca>, Santiago Higuera Quintero <s.higuera@uniandes.edu.co>, Jonathan Posada <jonathan.posada1@udea.edu.co>
 Maintainer-email: Steve Dodge <jsdodge@sfu.ca>
 License-Expression: MIT
```

