# Comparing `tmp/idf_build_apps-1.1.0.tar.gz` & `tmp/idf_build_apps-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.1.0.tar` & `idf_build_apps-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      351 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.editorconfig
--rw-r--r--   0        0        0      123 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.gitattributes
--rw-r--r--   0        0        0      513 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      253 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-07-21 08:38:46.199686 idf_build_apps-1.1.0/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3870 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.gitignore
--rw-r--r--   0        0        0     1077 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     5793 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1882 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/LICENSE
--rw-r--r--   0        0        0     3843 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/README.md
--rw-r--r--   0        0        0       33 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/config_file.md
--rw-r--r--   0        0        0    10473 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/index.rst
--rw-r--r--   0        0        0     5962 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    27235 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/config.py
--rw-r--r--   0        0        0     2182 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6328 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/log.py
--rw-r--r--   0        0        0    30514 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6368 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     6535 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3888 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     7081 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/license_header.txt
--rw-r--r--   0        0        0     2060 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3347 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_build.py
--rw-r--r--   0        0        0    18222 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_finder.py
--rw-r--r--   0        0        0     1568 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_manifest.py
--rw-r--r--   0        0        0     3710 2023-07-21 08:38:46.203686 idf_build_apps-1.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.1.0/setup.py
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.editorconfig
+-rw-r--r--   0        0        0      123 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.gitattributes
+-rw-r--r--   0        0        0      513 2023-06-28 00:47:16.025375 idf_build_apps-1.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      253 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-04-11 02:32:02.166123 idf_build_apps-1.1.1/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3870 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1077 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-07-27 09:31:01.648238 idf_build_apps-1.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0     5854 2023-08-02 08:31:02.047278 idf_build_apps-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1882 2023-06-09 07:19:31.556959 idf_build_apps-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3843 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/README.md
+-rw-r--r--   0        0        0       33 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-07-26 03:05:43.171073 idf_build_apps-1.1.1/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-04-21 06:49:01.279494 idf_build_apps-1.1.1/docs/config_file.md
+-rw-r--r--   0        0        0    10473 2023-06-12 08:46:12.574018 idf_build_apps-1.1.1/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-04-21 06:49:01.279494 idf_build_apps-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0     5962 2023-07-26 03:06:03.004294 idf_build_apps-1.1.1/docs/manifest.md
+-rw-r--r--   0        0        0      481 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-26 04:47:25.614071 idf_build_apps-1.1.1/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    27434 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2182 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6328 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-08-02 08:40:20.313852 idf_build_apps-1.1.1/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30232 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-06-08 06:29:51.606207 idf_build_apps-1.1.1/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6368 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     6535 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3888 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7081 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-04-11 02:32:02.169456 idf_build_apps-1.1.1/license_header.txt
+-rw-r--r--   0        0        0     2060 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/tests/test_build.py
+-rw-r--r--   0        0        0    18222 2023-08-02 08:40:20.317185 idf_build_apps-1.1.1/tests/test_finder.py
+-rw-r--r--   0        0        0     1568 2023-07-26 03:09:05.713381 idf_build_apps-1.1.1/tests/test_manifest.py
+-rw-r--r--   0        0        0     3710 2023-06-09 07:19:31.560293 idf_build_apps-1.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.1.1/setup.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.1.1/PKG-INFO
```

### Comparing `idf_build_apps-1.1.0/.github/dependabot.yml` & `idf_build_apps-1.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.github/workflows/issue_comment.yml` & `idf_build_apps-1.1.1/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.github/workflows/new_issues.yml` & `idf_build_apps-1.1.1/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.github/workflows/new_prs.yml` & `idf_build_apps-1.1.1/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.1.1/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.1.1/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.gitignore` & `idf_build_apps-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/.pre-commit-config.yaml` & `idf_build_apps-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/CHANGELOG.md` & `idf_build_apps-1.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## v1.1.1 (2023-08-02)
+
+### Fix
+
+- ignore idf_size.py error
+
 ## v1.1.0 (2023-07-21)
 
 ### Feat
 
 - support esp_rom caps as keywords in the manifest file
 
 ## v1.0.4 (2023-07-20)
```

### Comparing `idf_build_apps-1.1.0/CONTRIBUTING.md` & `idf_build_apps-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/LICENSE` & `idf_build_apps-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/README.md` & `idf_build_apps-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/Makefile` & `idf_build_apps-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/_static/espressif-logo.svg` & `idf_build_apps-1.1.1/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/_static/theme_overrides.css` & `idf_build_apps-1.1.1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/conf.py` & `idf_build_apps-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/config_file.md` & `idf_build_apps-1.1.1/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/find_build.md` & `idf_build_apps-1.1.1/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/docs/manifest.md` & `idf_build_apps-1.1.1/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/app.py` & `idf_build_apps-1.1.1/idf_build_apps/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,15 @@
         manifest_rootpath=None,  # type: str | None
         modified_components=None,  # type: list[str] | str | None
         modified_files=None,  # type: list[str] | str | None
         check_app_dependencies=False,  # type: bool
     ):  # type: (...) -> bool
         pass
 
-    def write_size_json(self):
+    def _write_size_json(self):
         map_file = find_first_match('*.map', self.build_path)
         if not map_file:
             LOGGER.warning(
                 '.map file not found. Cannot write size json to file: %s',
                 self.size_json_path,
             )
             return
@@ -438,14 +438,20 @@
                     map_file,
                 ]
             ),
             check=True,
         )
         LOGGER.info('=> Generated size info to %s', self.size_json_path)
 
+    def write_size_json(self):  # type: () -> None
+        try:
+            self._write_size_json()
+        except Exception as e:
+            LOGGER.warning('Failed to generate size json: %s', e)
+
     def to_json(self):
         # keeping backward compatibility, only provide these stuffs
         return json.dumps(
             {
                 'build_system': self.BUILD_SYSTEM,
                 'app_dir': self.app_dir,
                 'work_dir': self.work_dir,
```

### Comparing `idf_build_apps-1.1.0/idf_build_apps/config.py` & `idf_build_apps-1.1.1/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/constants.py` & `idf_build_apps-1.1.1/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/finder.py` & `idf_build_apps-1.1.1/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/log.py` & `idf_build_apps-1.1.1/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/main.py` & `idf_build_apps-1.1.1/idf_build_apps/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,21 +356,15 @@
             if is_built:
                 if app.collect_app_info:
                     with open(app.collect_app_info, 'a') as fw:
                         fw.write(app.to_json() + '\n')
                     LOGGER.info('=> Recorded app info in %s', app.collect_app_info)
 
                 if app.collect_size_info and app.size_json_path:
-                    try:
-                        if not os.path.isfile(app.size_json_path):
-                            app.write_size_json()
-                    except Exception as e:
-                        LOGGER.warning('Adding size info for app %s failed:', app.name)
-                        LOGGER.warning(e)
-                    else:
+                    if os.path.isfile(app.size_json_path):
                         with open(app.collect_size_info, 'a') as fw:
                             fw.write(
                                 json.dumps(
                                     {
                                         'app_name': app.name,
                                         'config_name': app.config_name,
                                         'target': app.target,
```

### Comparing `idf_build_apps-1.1.0/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.1.1/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.1.1/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.1.1/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/idf_build_apps/utils.py` & `idf_build_apps-1.1.1/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/pyproject.toml` & `idf_build_apps-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 changelog = "https://github.com/espressif/idf-build-apps/blob/master/CHANGELOG.md"
 
 [project.scripts]
 idf-build-apps = "idf_build_apps:main.main"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.0"
+version = "1.1.1"
 tag_format = "v$version"
 version_files = [
     "idf_build_apps/__init__.py",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-s --log-cli-level DEBUG"
```

### Comparing `idf_build_apps-1.1.0/tests/conftest.py` & `idf_build_apps-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/tests/test_build.py` & `idf_build_apps-1.1.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/tests/test_finder.py` & `idf_build_apps-1.1.1/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/tests/test_manifest.py` & `idf_build_apps-1.1.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/tests/test_utils.py` & `idf_build_apps-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.1.0/setup.py` & `idf_build_apps-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.1.0',
+      version='1.1.1',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.1.0/PKG-INFO` & `idf_build_apps-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

