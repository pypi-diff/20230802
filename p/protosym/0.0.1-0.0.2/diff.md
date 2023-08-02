# Comparing `tmp/protosym-0.0.1.tar.gz` & `tmp/protosym-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protosym-0.0.1.tar", max compression
+gzip compressed data, was "protosym-0.0.2.tar", max compression
```

## Comparing `protosym-0.0.1.tar` & `protosym-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,21 @@
--rw-r--r--   0        0        0     1539 2023-02-15 23:52:10.933499 protosym-0.0.1/LICENSE.rst
--rw-r--r--   0        0        0     2635 2023-02-15 23:52:10.933499 protosym-0.0.1/README.rst
--rw-r--r--   0        0        0     1701 2023-02-15 23:52:23.281392 protosym-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       16 2023-02-15 23:52:10.937499 protosym-0.0.1/src/protosym/__init__.py
--rw-r--r--   0        0        0      226 2023-02-15 23:52:10.937499 protosym-0.0.1/src/protosym/__main__.py
--rw-r--r--   0        0        0        0 2023-02-15 23:52:10.937499 protosym-0.0.1/src/protosym/py.typed
--rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 protosym-0.0.1/setup.py
--rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 protosym-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1534 2023-08-02 16:29:00.834274 protosym-0.0.2/LICENSE.rst
+-rw-r--r--   0        0        0     2635 2023-08-02 16:29:00.834274 protosym-0.0.2/README.rst
+-rw-r--r--   0        0        0     2425 2023-08-02 16:29:15.558488 protosym-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/__init__.py
+-rw-r--r--   0        0        0      222 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/__main__.py
+-rw-r--r--   0        0        0      118 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/__init__.py
+-rw-r--r--   0        0        0     5715 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/atom.py
+-rw-r--r--   0        0        0     4215 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/differentiate.py
+-rw-r--r--   0        0        0     8857 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/evaluate.py
+-rw-r--r--   0        0        0      384 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/exceptions.py
+-rw-r--r--   0        0        0    19352 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/sym.py
+-rw-r--r--   0        0        0    15551 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/core/tree.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/py.typed
+-rw-r--r--   0        0        0     1012 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/__init__.py
+-rw-r--r--   0        0        0      435 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/exceptions.py
+-rw-r--r--   0        0        0    17384 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/expr.py
+-rw-r--r--   0        0        0     3758 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/functions.py
+-rw-r--r--   0        0        0     8596 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/lambdification.py
+-rw-r--r--   0        0        0     6500 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/matrix.py
+-rw-r--r--   0        0        0     4332 2023-08-02 16:29:00.838274 protosym-0.0.2/src/protosym/simplecas/sympy_conversions.py
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 protosym-0.0.2/PKG-INFO
```

### Comparing `protosym-0.0.1/LICENSE.rst` & `protosym-0.0.2/LICENSE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-BSD-3-clause license
-====================
-
-Copyright (c) 2006-2023 Oscar Benjamin
-
+Copyright (c) 2023 Oscar Benjamin
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-  a. Redistributions of source code must retain the above copyright notice,
-     this list of conditions and the following disclaimer.
-  b. Redistributions in binary form must reproduce the above copyright
-     notice, this list of conditions and the following disclaimer in the
-     documentation and/or other materials provided with the distribution.
-  c. Neither the name of SymPy nor the names of its contributors
-     may be used to endorse or promote products derived from this software
-     without specific prior written permission.
+modification, are permitted provided that the following conditions are
+met:
 
+    * Redistributions of source code must retain the above copyright
+       notice, this list of conditions and the following disclaimer.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGE.
+    * Redistributions in binary form must reproduce the above
+       copyright notice, this list of conditions and the following
+       disclaimer in the documentation and/or other materials provided
+       with the distribution.
+
+    * Neither the name of the NumPy Developers nor the names of any
+       contributors may be used to endorse or promote products derived
+       from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `protosym-0.0.1/README.rst` & `protosym-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `protosym-0.0.1/pyproject.toml` & `protosym-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protosym"
-version = "0.0.1"
+version = "0.0.2"
 description = "ProtoSym"
 authors = ["Oscar Benjamin <oscar.j.benjamin@gmail.com>"]
 license = "BSD-3-clause"
 readme = "README.rst"
 homepage = "https://github.com/oscarbenjamin/protosym"
 repository = "https://github.com/oscarbenjamin/protosym"
 documentation = "https://protosym.readthedocs.io"
@@ -16,57 +16,100 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/oscarbenjamin/protosym/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
-coverage = {extras = ["toml"], version = "^7.1.0"}
+pytest = "^7.4.0"
+coverage = {extras = ["toml"], version = "^7.2.7"}
 safety = "^2.3.5"
-mypy = "^1.0.0"
-typeguard = "^2.13.3"
+mypy = "^1.4.1"
+typeguard = "^4.1.0"
 xdoctest = {extras = ["colors"], version = "^1.1.1"}
-sphinx = "^6.1.3"
+sphinx = "^6.2.1"
 sphinx-autobuild = "^2021.3.14"
-pre-commit = "^3.0.4"
-flake8 = "^6.0.0"
+pre-commit = "^3.3.3"
+flake8 = "^6.1.0"
 black = "22.12.0"
 flake8-bandit = "^4.1.1"
-flake8-bugbear = "^23.2.13"
+flake8-bugbear = "^23.7.10"
 flake8-docstrings = "^1.7.0"
 flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.3"
 darglint = "^1.8.1"
-reorder-python-imports = "^3.9.0"
+reorder-python-imports = "^3.10.0"
 pre-commit-hooks = "^4.4.0"
-sphinx-rtd-theme = "^1.2.0"
-Pygments = "^2.14.0"
-nox = "^2022.11.21"
-gitpython = "^3.1.30"
+sphinx-rtd-theme = "^1.2.2"
+Pygments = "^2.15.1"
+nox = "^2023.4.22"
+gitpython = "^3.1.32"
 py = "^1.11.0"
-setuptools = "^67.3.2"
+setuptools = "^67.8.0"
+pytest-coverage = "^0.0"
+sympy = "^1.12"
+pip-upgrader = "^1.4.15"
+flake8-type-checking = "^2.4.1"
+llvmlite = "^0.40.1"
+symengine = "^0.10.0"
+numpy = "^1.24.4"
+pytest-benchmark = "^4.0.0"
+
+
+[tool.poetry.group.utils.dependencies]
+ipython = "^8.12.2"
+jupyter = "^1.0.0"
 
 [tool.poetry.scripts]
 protosym = "protosym.__main__:main"
 
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+]
+
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["protosym"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 100
+exclude_lines = [
+    "pragma: no cover",
+    "if _TYPE_CHECKING:",
+    "@overload",
+]
 
 [tool.mypy]
 strict = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 
+[[tool.mypy.overrides]]
+module = [
+    'jinja2',
+    'llvmlite',
+    'llvmlite.binding',
+    'py',
+    'symengine',
+    'numpy',
+]
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = [
+    "sympy",
+    "sympy.core.function",
+    "rust_protosym",
+]
+follow_imports = "skip"
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `protosym-0.0.1/PKG-INFO` & `protosym-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: protosym
-Version: 0.0.1
+Version: 0.0.2
 Summary: ProtoSym
 Home-page: https://github.com/oscarbenjamin/protosym
 License: BSD-3-Clause
 Author: Oscar Benjamin
 Author-email: oscar.j.benjamin@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Project-URL: Changelog, https://github.com/oscarbenjamin/protosym/releases
 Project-URL: Documentation, https://protosym.readthedocs.io
 Project-URL: Repository, https://github.com/oscarbenjamin/protosym
 Description-Content-Type: text/x-rst
 
 ProtoSym
 ========
```

