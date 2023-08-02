# Comparing `tmp/mkdocs_gitlab-1.1.1.tar.gz` & `tmp/mkdocs_gitlab-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_gitlab-1.1.1.tar", max compression
+gzip compressed data, was "mkdocs_gitlab-1.2.0.tar", max compression
```

## Comparing `mkdocs_gitlab-1.1.1.tar` & `mkdocs_gitlab-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-07-15 16:35:41.188703 mkdocs_gitlab-1.1.1/LICENSE
--rw-r--r--   0        0        0      898 2023-07-15 16:35:41.188703 mkdocs_gitlab-1.1.1/README.md
--rw-r--r--   0        0        0       22 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/mkdocs_gitlab/__init__.py
--rw-r--r--   0        0        0     1591 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/mkdocs_gitlab/plugin.py
--rw-r--r--   0        0        0        0 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/mkdocs_gitlab/py.typed
--rw-r--r--   0        0        0     2282 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/LICENSE
+-rw-r--r--   0        0        0      954 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/__init__.py
+-rw-r--r--   0        0        0      649 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/markdown.py
+-rw-r--r--   0        0        0     1717 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/plugin.py
+-rw-r--r--   0        0        0        0 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/mkdocs_gitlab/py.typed
+-rw-r--r--   0        0        0     2412 2023-08-02 15:31:24.549138 mkdocs_gitlab-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.2.0/PKG-INFO
```

### Comparing `mkdocs_gitlab-1.1.1/LICENSE` & `mkdocs_gitlab-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.1.1/README.md` & `mkdocs_gitlab-1.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 - CI_PROJECT_TITLE
 - CI_PROJECT_DESCRIPTION
 - CI_PAGES_URL
 - CI_PROJECT_URL
 - CI_PROJECT_PATH
 
+Also the pugin deletes the `[[_TOC_]]` or `[TOC]` tag.
+
 ## Installation
 
 ### pip
 
 ```
 pip install mkdocs-gitlab
 ```
```

### Comparing `mkdocs_gitlab-1.1.1/mkdocs_gitlab/plugin.py` & `mkdocs_gitlab-1.2.0/mkdocs_gitlab/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,8 +48,11 @@
 
         config.site_name = site_config.site_name
         config.site_description = site_config.site_description
         config.site_url = site_config.site_url
         config.repo_url = site_config.repo_url
         config.repo_name = site_config.repo_name
 
+        if "mkdocs-gitlab" not in config.markdown_extensions:
+            config.markdown_extensions.append("mkdocs-gitlab")
+
         return config
```

### Comparing `mkdocs_gitlab-1.1.1/pyproject.toml` & `mkdocs_gitlab-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.1"
+version = "1.2.0"
 tag_format = "$version"
 version_files = [
     "mkdocs_gitlab/__init__.py",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "mkdocs-gitlab"
-version = "1.1.1"
+version = "1.2.0"
 description = "Use Gitlab CI variables for your docs"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/mkdocs-gitlab"
 homepage = "https://pypi.org/project/mkdocs-gitlab"
 keywords = []
 
 [tool.poetry.plugins."mkdocs.plugins"]
 "mkdocs-gitlab" = "mkdocs_gitlab.plugin:MkDocsGitlabPlugin"
 
+[tool.poetry.plugins."markdown.extensions"]
+"mkdocs-gitlab" = "mkdocs_gitlab.markdown:TOCExtension"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 mkdocs = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-mock = "^3.10.0"
 ruff = "^0.0.255"
 toml = "^0.10.2"
+types-markdown = "^3.4.2.10"
 
 [tool.poetry.group.git.dependencies]
 commitizen = "^3.5.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mkdocs_gitlab-1.1.1/PKG-INFO` & `mkdocs_gitlab-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-gitlab
-Version: 1.1.1
+Version: 1.2.0
 Summary: Use Gitlab CI variables for your docs
 Home-page: https://pypi.org/project/mkdocs-gitlab
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,16 @@
 
 - CI_PROJECT_TITLE
 - CI_PROJECT_DESCRIPTION
 - CI_PAGES_URL
 - CI_PROJECT_URL
 - CI_PROJECT_PATH
 
+Also the pugin deletes the `[[_TOC_]]` or `[TOC]` tag.
+
 ## Installation
 
 ### pip
 
 ```
 pip install mkdocs-gitlab
 ```
```

