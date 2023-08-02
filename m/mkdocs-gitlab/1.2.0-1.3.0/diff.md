# Comparing `tmp/mkdocs_gitlab-1.2.0.tar.gz` & `tmp/mkdocs_gitlab-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_gitlab-1.2.0.tar", max compression
+gzip compressed data, was "mkdocs_gitlab-1.3.0.tar", max compression
```

## Comparing `mkdocs_gitlab-1.2.0.tar` & `mkdocs_gitlab-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/LICENSE
--rw-r--r--   0        0        0      954 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/README.md
--rw-r--r--   0        0        0       22 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/__init__.py
--rw-r--r--   0        0        0      649 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/markdown.py
--rw-r--r--   0        0        0     1717 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/plugin.py
--rw-r--r--   0        0        0        0 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/py.typed
--rw-r--r--   0        0        0     2412 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/LICENSE
+-rw-r--r--   0        0        0      947 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/mkdocs_gitlab/__init__.py
+-rw-r--r--   0        0        0      649 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/mkdocs_gitlab/markdown.py
+-rw-r--r--   0        0        0     1703 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/mkdocs_gitlab/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/mkdocs_gitlab/py.typed
+-rw-r--r--   0        0        0     2514 2023-08-02 18:49:49.941602 mkdocs_gitlab-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.3.0/PKG-INFO
```

### Comparing `mkdocs_gitlab-1.2.0/LICENSE` & `mkdocs_gitlab-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.2.0/README.md` & `mkdocs_gitlab-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## Usage
 
 ```yaml
 site_name: Title
 
 plugins:
-- mkdocs-gitlab
+- gitlab
 
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
```

### Comparing `mkdocs_gitlab-1.2.0/mkdocs_gitlab/markdown.py` & `mkdocs_gitlab-1.3.0/mkdocs_gitlab/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.2.0/mkdocs_gitlab/plugin.py` & `mkdocs_gitlab-1.3.0/mkdocs_gitlab/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,11 +48,11 @@
 
         config.site_name = site_config.site_name
         config.site_description = site_config.site_description
         config.site_url = site_config.site_url
         config.repo_url = site_config.repo_url
         config.repo_name = site_config.repo_name
 
-        if "mkdocs-gitlab" not in config.markdown_extensions:
-            config.markdown_extensions.append("mkdocs-gitlab")
+        if "gitlab" not in config.markdown_extensions:
+            config.markdown_extensions.append("gitlab")
 
         return config
```

### Comparing `mkdocs_gitlab-1.2.0/pyproject.toml` & `mkdocs_gitlab-1.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.0"
+version = "1.3.0"
 tag_format = "$version"
 version_files = [
     "mkdocs_gitlab/__init__.py",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "mkdocs-gitlab"
-version = "1.2.0"
+version = "1.3.0"
 description = "Use Gitlab CI variables for your docs"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/mkdocs-gitlab"
 homepage = "https://pypi.org/project/mkdocs-gitlab"
 keywords = []
 
 [tool.poetry.plugins."mkdocs.plugins"]
 "mkdocs-gitlab" = "mkdocs_gitlab.plugin:MkDocsGitlabPlugin"
+"gitlab" = "mkdocs_gitlab.plugin:MkDocsGitlabPlugin"
 
 [tool.poetry.plugins."markdown.extensions"]
 "mkdocs-gitlab" = "mkdocs_gitlab.markdown:TOCExtension"
+"gitlab" = "mkdocs_gitlab.markdown:TOCExtension"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 mkdocs = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
```

### Comparing `mkdocs_gitlab-1.2.0/PKG-INFO` & `mkdocs_gitlab-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-gitlab
-Version: 1.2.0
+Version: 1.3.0
 Summary: Use Gitlab CI variables for your docs
 Home-page: https://pypi.org/project/mkdocs-gitlab
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,15 +44,15 @@
 
 ## Usage
 
 ```yaml
 site_name: Title
 
 plugins:
-- mkdocs-gitlab
+- gitlab
 
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
```

