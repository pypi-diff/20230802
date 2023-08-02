# Comparing `tmp/hyfi_absa-0.1.0.tar.gz` & `tmp/hyfi_absa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_absa-0.1.0.tar", max compression
+gzip compressed data, was "hyfi_absa-0.2.0.tar", max compression
```

## Comparing `hyfi_absa-0.1.0.tar` & `hyfi_absa-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,29 @@
--rw-r--r--   0        0        0     1071 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/LICENSE
--rw-r--r--   0        0        0     2600 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/README.md
--rw-r--r--   0        0        0     2927 2023-07-30 06:35:12.977532 hyfi_absa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      181 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/src/hyabsa/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/src/hyabsa/__init__.py
--rw-r--r--   0        0        0       22 2023-07-30 06:35:12.937531 hyfi_absa-0.1.0/src/hyabsa/_version.py
--rw-r--r--   0        0        0        0 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/src/hyabsa/conf/__init__.py
--rw-r--r--   0        0        0      234 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/src/hyabsa/conf/about/hyabsa.yaml
--rw-r--r--   0        0        0        0 2023-07-30 06:34:47.881223 hyfi_absa-0.1.0/src/hyabsa/py.typed
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 hyfi_absa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-02 12:23:49.380314 hyfi_absa-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2598 2023-08-02 12:23:49.380314 hyfi_absa-0.2.0/README.md
+-rw-r--r--   0        0        0     2965 2023-08-02 12:24:15.216351 hyfi_absa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/__cli__.py
+-rw-r--r--   0        0        0      473 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-02 12:24:15.176351 hyfi_absa-0.2.0/src/hyabsa/_version.py
+-rw-r--r--   0        0        0      157 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/__init__.py
+-rw-r--r--   0        0        0      641 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/absa.py
+-rw-r--r--   0        0        0     1458 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/base.py
+-rw-r--r--   0        0        0      900 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/agents/results.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/__init__.py
+-rw-r--r--   0        0        0      234 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/about/hyabsa.yaml
+-rw-r--r--   0        0        0      158 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/agent/__init__.yaml
+-rw-r--r--   0        0        0      158 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/agent/absa.yaml
+-rw-r--r--   0        0        0       51 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/gpt35.yaml
+-rw-r--r--   0        0        0       80 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/gpt4.yaml
+-rw-r--r--   0        0        0      111 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/llm/openai.yaml
+-rw-r--r--   0        0        0       64 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/prompts/__init__.yaml
+-rw-r--r--   0        0        0     2975 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/prompts/default.yaml
+-rw-r--r--   0        0        0      319 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/conf/runner/absa.yaml
+-rw-r--r--   0        0        0      108 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/contexts/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/llms/__init__.py
+-rw-r--r--   0        0        0     2949 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/llms/openai.py
+-rw-r--r--   0        0        0      744 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/py.typed
+-rw-r--r--   0        0        0       62 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/runners/__init__.py
+-rw-r--r--   0        0        0     2560 2023-08-02 12:23:49.384314 hyfi_absa-0.2.0/src/hyabsa/runners/absa.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 hyfi_absa-0.2.0/PKG-INFO
```

### Comparing `hyfi_absa-0.1.0/LICENSE` & `hyfi_absa-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.1.0/README.md` & `hyfi_absa-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
-[codecov-image]: https://codecov.io/gh/entelecheia/hyfi-absa/branch/main/graph/badge.svg?token=[REPLACE_ME]
+[codecov-image]: https://codecov.io/gh/entelecheia/hyfi-absa/branch/main/graph/badge.svg?token=BC2f1ooCPI
 [codecov-url]: https://codecov.io/gh/entelecheia/hyfi-absa
 [pypi-image]: https://img.shields.io/pypi/v/hyfi-absa
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi-absa
 [license-url]: https://github.com/entelecheia/hyfi-absa/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi-absa?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi-absa
 [release-url]: https://github.com/entelecheia/hyfi-absa/releases
```

### Comparing `hyfi_absa-0.1.0/pyproject.toml` & `hyfi_absa-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "hyfi-absa"
-version = "0.1.0"
+version = "0.2.0"
 description = "HyFI-ABSA is a Python package developed as a plugin for the Hydra Fast Interface (HyFI)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-absa.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-absa"
 readme = "README.md"
 packages = [{ include = "hyabsa", from = "src" }]
 
 [tool.poetry.scripts]
 hyabsa = 'hyabsa.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.12.5"
+hyfi = "^1.17.0"
+backoff = "^2.2.1"
+openai = "^0.27.8"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_absa-0.1.0/PKG-INFO` & `hyfi_absa-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: hyfi-absa
-Version: 0.1.0
+Version: 0.2.0
 Summary: HyFI-ABSA is a Python package developed as a plugin for the Hydra Fast Interface (HyFI).
 Home-page: https://hyfi-absa.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.12.5,<2.0.0)
+Requires-Dist: hyfi (>=1.17.0,<2.0.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-absa
 Description-Content-Type: text/markdown
 
 # HyFI-ABSA
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![codecov][codecov-image]][codecov-url]
 [![jupyter-book-image]][docs-url]
 
 <!-- Links: -->
-[codecov-image]: https://codecov.io/gh/entelecheia/hyfi-absa/branch/main/graph/badge.svg?token=[REPLACE_ME]
+[codecov-image]: https://codecov.io/gh/entelecheia/hyfi-absa/branch/main/graph/badge.svg?token=BC2f1ooCPI
 [codecov-url]: https://codecov.io/gh/entelecheia/hyfi-absa
 [pypi-image]: https://img.shields.io/pypi/v/hyfi-absa
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi-absa
 [license-url]: https://github.com/entelecheia/hyfi-absa/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi-absa?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi-absa
 [release-url]: https://github.com/entelecheia/hyfi-absa/releases
```

