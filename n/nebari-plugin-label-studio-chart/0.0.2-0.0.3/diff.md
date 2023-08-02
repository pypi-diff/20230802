# Comparing `tmp/nebari_plugin_label_studio_chart-0.0.2.tar.gz` & `tmp/nebari_plugin_label_studio_chart-0.0.3.tar.gz`

## Comparing `nebari_plugin_label_studio_chart-0.0.2.tar` & `nebari_plugin_label_studio_chart-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/__about__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/cfg/__init__.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/main.tf
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/outputs.tf
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/variables.tf
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/versions.tf
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/chart/Chart.yaml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/chart/values.yaml
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/auth.yaml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/ingress.yaml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/.gitignore
--rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/LICENSE.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/README.md
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/__about__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/cfg/__init__.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/main.tf
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/outputs.tf
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/variables.tf
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/versions.tf
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/chart/Chart.yaml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/chart/values.yaml
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/auth.yaml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/.gitignore
+-rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/README.md
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 nebari_plugin_label_studio_chart-0.0.3/PKG-INFO
```

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/__init__.py` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/main.tf` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/outputs.tf` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/keycloak/terraform/variables.tf` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/keycloak/terraform/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/__init__.py` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/auth.yaml` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/auth.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/ingress.yaml` & `nebari_plugin_label_studio_chart-0.0.3/src/nebari_plugin_label_studio_chart/label_studio/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/LICENSE.md` & `nebari_plugin_label_studio_chart-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/README.md` & `nebari_plugin_label_studio_chart-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nebari_plugin_label_studio_chart-0.0.2/pyproject.toml` & `nebari_plugin_label_studio_chart-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -160,8 +160,8 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [project.entry-points.nebari]
-nebari-plugin-label-studio-chart = "nebari_plugin_label_studio_chart"
+nebari-plugin-label-studio-chart = "src.nebari_plugin_label_studio_chart"
```

### Comparing `nebari_plugin_label_studio_chart-0.0.2/PKG-INFO` & `nebari_plugin_label_studio_chart-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari-plugin-label-studio-chart
-Version: 0.0.2
+Version: 0.0.3
 Summary: MetroStar Onyx - Label Studio plugin for Nebari platform
 Project-URL: Documentation, https://github.com/MetroStar/nebari-label-studio#readme
 Project-URL: Issues, https://github.com/MetroStar/nebari-label-studio/issues
 Project-URL: Source, https://github.com/MetroStar/nebari-label-studio
 Author-email: Scott Blair <sblair@metrostar.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
```

