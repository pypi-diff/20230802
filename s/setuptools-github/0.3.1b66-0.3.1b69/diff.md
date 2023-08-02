# Comparing `tmp/setuptools-github-0.3.1b66.tar.gz` & `tmp/setuptools-github-0.3.1b69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.1b66.tar", last modified: Tue Aug  1 20:03:07 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.1b69.tar", last modified: Wed Aug  2 16:17:30 2023, max compression
```

## Comparing `setuptools-github-0.3.1b66.tar` & `setuptools-github-0.3.1b69.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.502533 setuptools-github-0.3.1b66/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 20:03:07.000000 setuptools-github-0.3.1b66/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:03:07.506533 setuptools-github-0.3.1b66/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-08-01 20:02:36.000000 setuptools-github-0.3.1b66/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.155953 setuptools-github-0.3.1b69/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.155953 setuptools-github-0.3.1b69/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 16:17:30.000000 setuptools-github-0.3.1b69/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:17:30.159953 setuptools-github-0.3.1b69/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-02 16:16:55.000000 setuptools-github-0.3.1b69/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.1b66/LICENSE` & `setuptools-github-0.3.1b69/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/PKG-INFO` & `setuptools-github-0.3.1b69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b66
+Version: 0.3.1b69
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg)](Coverage)
+[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/beta/0.3.1/graph/badge.svg)](Coverage)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
```

### Comparing `setuptools-github-0.3.1b66/README.md` & `setuptools-github-0.3.1b69/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg)](Coverage)
+[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/beta/0.3.1/graph/badge.svg)](Coverage)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 
 
 
@@ -167,8 +167,8 @@
 Once done, you'll need to push it the tag.
 ```bash
 git push release/N.M.O
 ```
 This will:
 - trigger a CI build that will create the project-name-N.M.O
 - Create a new wheel package under dist/
-- (on success) Send the new wheels **project-N.M.O** to [PyPI](https://pypi.org)
+- (on success) Send the new wheels **project-N.M.O** to [PyPI](https://pypi.org)
```

### Comparing `setuptools-github-0.3.1b66/pyproject.toml` & `setuptools-github-0.3.1b69/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = [ "setuptools", "setuptools-github", "wheel", "typing-extensions", ]
+requires = [ "setuptools", "setuptools-github", "wheel", "typing-extensions", "jinja2"]
 build-backend = 'setuptools.build_meta'
 
 [tool.black]
 line-length = 88
 
 
 [tool.ruff]
```

### Comparing `setuptools-github-0.3.1b66/setup.py` & `setuptools-github-0.3.1b69/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 
 sys.path.insert(0, str(pathlib.Path(__file__).parent / "src"))
 from setuptools_github import tools  # noqa E402
 from setuptools import setup, find_namespace_packages  # noqa E402
 
 
 initfile = pathlib.Path(__file__).parent / "src/setuptools_github/__init__.py"
-version = tools.update_version(initfile, os.getenv("GITHUB_DUMP"))
+readme = pathlib.Path(__file__).parent / "README.md"
+version = tools.process(initfile, os.getenv("GITHUB_DUMP"), readme)["version"]
 
 packages = find_namespace_packages(where="src")
 
 setup(
     name="setuptools-github",
     version=version,
     url="https://github.com/cav71/setuptools-github",
     packages=packages,
     package_dir={"setuptools_github": "src/setuptools_github"},
     description="supports github releases",
-    long_description=pathlib.Path("README.md").read_text(),
+    long_description=readme.read_text(),
     long_description_content_type="text/markdown",
-    install_requires=["setuptools"],
+    install_requires=[
+        "setuptools",
+        "typing-extensions",
+        "jinja2",
+    ],
     entry_points={
         "console_scripts": [
             "setuptools-github=setuptools_github.script:main",
         ],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `setuptools-github-0.3.1b66/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.1b69/setuptools_github.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b66
+Version: 0.3.1b69
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # setuptools-github
 [![PyPI version](https://img.shields.io/pypi/v/setuptools-github.svg?color=blue)](https://pypi.org/project/setuptools-github)
 [![Python versions](https://img.shields.io/pypi/pyversions/setuptools-github.svg)](https://pypi.org/project/setuptools-github)
 [![Build](https://github.com/cav71/setuptools-github/actions/workflows/master.yml/badge.svg)](https://github.com/cav71/setuptools-github/actions)
-[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/master/graph/badge.svg)](Coverage)
+[![Coverage](https://codecov.io/gh/cav71/setuptools-github/branch/beta/0.3.1/graph/badge.svg)](Coverage)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
```

### Comparing `setuptools-github-0.3.1b66/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.1b69/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/src/setuptools_github/checks.py` & `setuptools-github-0.3.1b69/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/src/setuptools_github/cli.py` & `setuptools-github-0.3.1b69/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/src/setuptools_github/scm.py` & `setuptools-github-0.3.1b69/src/setuptools_github/scm.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,17 @@
             value = mapper[tag]
             if value:
                 result[filename] = (
                     (result[filename] | value) if filename in result else value
                 )
         return result
 
+    def dirty(self) -> bool:
+        return bool(self.status(untracked_files="no"))
+
     def commit(
         self,
         paths: ListOfArgs,
         message: str,
     ) -> None:
         all_paths = to_list_of_paths(paths)
         self(["add", *all_paths])
```

### Comparing `setuptools-github-0.3.1b66/src/setuptools_github/script.py` & `setuptools-github-0.3.1b69/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/src/setuptools_github/tools.py` & `setuptools-github-0.3.1b69/src/setuptools_github/tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -83,18 +83,24 @@
     else:
         last_eol = ""
 
     result = pre + txt.replace("\n", "\n" + pre) + last_eol
     return result if result.strip() else result.strip()
 
 
-def list_of_paths(paths: str | Path | list[str | Path]) -> list[Path]:
+def list_of_paths(paths: str | Path | list[str | Path] | None) -> list[Path]:
+    if not paths:
+        return []
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
+def lstrip(txt: str, left: str) -> str:
+    return txt[len(left) :] if txt.startswith(left) else txt
+
+
 def get_module_var(
     path: Path | str, var: str = "__version__", abort=True
 ) -> str | None:
     """extract from a python module in path the module level <var> variable
 
     Args:
         path (str,Path): python module file to parse using ast (no code-execution)
@@ -131,14 +137,18 @@
                         )
                     if isinstance(subnode.value, ast.Str):
                         value = subnode.value.s
                     elif isinstance(subnode.value, ast.Num):
                         value = subnode.value.n
                     else:
                         value = subnode.value.value
+                    if target.id in self.result:
+                        raise ValidationError(
+                            f"found multiple repeated variables {target.id}"
+                        )
                     self.result[target.id] = value
             return self.generic_visit(node)
 
     v = V({var})
     path = Path(path)
     if path.exists():
         tree = ast.parse(Path(path).read_text())
@@ -158,38 +168,42 @@
         var (str): module level variable name to extract
         value (None or Any): if not None replace var in initfile
         create (bool): create path if not present
 
     Returns:
         (str, str) the (<previous-var-value|None>, <the new text>)
     """
+
+    # validate the var
+    get_module_var(path, var, abort=False)
+
     # module level var
     expr = re.compile(f"^{var}\\s*=\\s*['\\\"](?P<value>[^\\\"']*)['\\\"]")
     fixed = None
     lines = []
 
     src = Path(path)
     if not src.exists() and create:
         src.parent.mkdir(parents=True, exist_ok=True)
         src.touch()
 
     input_lines = src.read_text().split("\n")
-    for line in reversed(input_lines):
-        if fixed:
+    for line in input_lines:
+        if fixed is not None:
             lines.append(line)
             continue
         match = expr.search(line)
         if match:
             fixed = match.group("value")
             if value is not None:
                 x, y = match.span(1)
                 line = line[:x] + value + line[y:]
         lines.append(line)
-    txt = "\n".join(reversed(lines))
-    if not fixed and create:
+    txt = "\n".join(lines)
+    if (fixed is None) and create:
         if txt and txt[-1] != "\n":
             txt += "\n"
         txt += f'{var} = "{value}"'
 
     with Path(path).open("w") as fp:
         fp.write(txt)
     return fixed, txt
@@ -219,63 +233,124 @@
         newver[-2] += 1
         newver[-1] = 0
     elif mode == "micro":
         newver[-1] += 1
     return ".".join(str(v) for v in newver)
 
 
-def update_version(
+def get_data(
     initfile: str | Path, github_dump: str | None = None, abort: bool = True
-) -> str | None:
+) -> dict[str, str | None]:
     """extracts version information from github_dump and updates initfile in-place
 
     Args:
         initfile (str, Path): path to the __init__.py file with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
-        str: the new version for the package
+        dict[str,str|None]: a dict with the current config
     """
+    result = {
+        "version": get_module_var(initfile, "__version__"),
+        "current": get_module_var(initfile, "__version__"),
+        "branch": None,
+        "hash": None,
+        "build": None,
+    }
 
     path = Path(initfile)
     repo = scm.lookup(path)
 
     if not (repo or github_dump):
         if abort:
             raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")
-        return get_module_var(path, "__version__")
+        return result
 
     if not github_dump and repo:
         gdata = {
             "ref": repo.head.name,
             "sha": repo.head.target.hex[:7],
             "run_number": 0,
         }
-        dirty = bool(repo.status())
+        dirty = repo.dirty()
     else:
         gdata = json.loads(github_dump) if isinstance(github_dump, str) else github_dump
         dirty = False
 
-    version = current = get_module_var(path, "__version__")
-
     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$")
     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
 
+    result["branch"] = lstrip(gdata["ref"], "refs/heads/")
+    result["hash"] = gdata["sha"] + ("*" if dirty else "")
+    result["build"] = gdata["run_number"]
+
+    current = result["current"]
     if match := expr.search(gdata["ref"]):
         # setuptools double calls the update_version,
         # this fixes the issue
         match1 = expr1.search(current or "")
         if not match1:
             raise InvalidVersionError(f"cannot parse current version '{current}'")
         if match1.group("version") != match.group("version"):
             raise InvalidVersionError(
                 f"building package for {current} from '{gdata['ref']}' "
                 f"branch ({match.groupdict()} mismatch {match1.groupdict()})"
             )
         if match.group("what") == "beta":
-            version = f"{match1.group('version')}b{gdata['run_number']}"
+            result["version"] = f"{match1.group('version')}b{gdata['run_number']}"
+    return result
+
 
-    short = gdata["sha"] + ("*" if dirty else "")
+def update_version(
+    initfile: str | Path, github_dump: str | None = None, abort: bool = True
+) -> str | None:
+    """extracts version information from github_dump and updates initfile in-place
+
+    Args:
+        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        github_dump (str): the os.getenv("GITHUB_DUMP") value
+
+    Returns:
+        str: the new version for the package
+    """
+
+    data = get_data(initfile, github_dump, abort)
+    set_module_var(initfile, "__version__", data["version"])
+    set_module_var(initfile, "__hash__", data["hash"])
+    return data["version"]
+
+
+def process(
+    initfile: str | Path,
+    github_dump: str | None = None,
+    paths: str | Path | list[str | Path] | None = None,
+    abort: bool = True,
+) -> dict[str, str | None]:
+    """get version from github_dump and updates initfile/paths
+
+    Args:
+        paths (str, Path): path(s) to files jinja2 processeable
+        initfile (str, Path): path to the __init__.py file with a __version__ variable
+        github_dump (str): the os.getenv("GITHUB_DUMP") value
+
+    Returns:
+        str: the new version for the package
+    """
+    from jinja2 import Environment
+    from argparse import Namespace
+
+    class Context(Namespace):
+        def items(self):
+            for name, value in self.__dict__.items():
+                if name.startswith("_"):
+                    continue
+                yield (name, value)
 
-    set_module_var(path, "__version__", version)
-    set_module_var(path, "__hash__", short)
-    return version
+    data = get_data(initfile, github_dump, abort)
+    set_module_var(initfile, "__version__", data["version"])
+    set_module_var(initfile, "__hash__", data["hash"])
+
+    env = Environment()
+    for path in list_of_paths(paths):
+        tmpl = env.from_string(path.read_text())
+        path.write_text(tmpl.render(ctx=Context(**data)))
+    return data
```

### Comparing `setuptools-github-0.3.1b66/tests/conftest.py` & `setuptools-github-0.3.1b69/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/tests/test_checks.py` & `setuptools-github-0.3.1b69/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/tests/test_cli.py` & `setuptools-github-0.3.1b69/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/tests/test_conftest.py` & `setuptools-github-0.3.1b69/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/tests/test_scm.py` & `setuptools-github-0.3.1b69/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/tests/test_script.py` & `setuptools-github-0.3.1b69/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b66/tests/test_tools.py` & `setuptools-github-0.3.1b69/tests/test_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -125,14 +125,18 @@
     assert tools.list_of_paths("hello") == [Path("hello")]
     assert tools.list_of_paths(["hello", Path("world")]) == [
         Path("hello"),
         Path("world"),
     ]
 
 
+def test_lstrip():
+    assert tools.lstrip("/a/b/c/d/e", "/a/b") == "/c/d/e"
+
+
 def test_get_module_var(tmp_path):
     "pulls variables from a file"
     path = tmp_path / "in0.txt"
     path.write_text(
         """
 # a test file
 A = 12
@@ -142,14 +146,26 @@
 """
     )
     assert 12 == tools.get_module_var(path, "A")
     assert "hello" == tools.get_module_var(path, "C")
     pytest.raises(tools.ValidationError, tools.get_module_var, path, "B")
     pytest.raises(tools.MissingVariableError, tools.get_module_var, path, "X1")
 
+    path.write_text(
+        """
+# a test file
+A = 12
+B = 3+5
+C = "hello"
+C = "hello2"
+# end of test
+"""
+    )
+    pytest.raises(tools.ValidationError, tools.get_module_var, path, "C")
+
 
 def test_set_module_var(tmp_path):
     "handles set_module_var cases"
     path = tmp_path / "in2.txt"
 
     path.write_text(
         """
@@ -191,14 +207,26 @@
 # a fist comment line
 __hash__ = "9.10.11"
 # end of test
 __version__ = "6.7.8"
 """.rstrip()
     )
 
+    version, txt = tools.set_module_var(path, "__version__", "9.10.11")
+    assert version == "6.7.8"
+    assert (
+        txt.rstrip()
+        == """
+# a fist comment line
+__hash__ = "9.10.11"
+# end of test
+__version__ = "9.10.11"
+""".rstrip()
+    )
+
 
 def test_set_module_var_empty_file(tmp_path):
     "check if the set_module_var will create a bew file"
     path = tmp_path / "in1.txt"
 
     assert not path.exists()
     tools.set_module_var(path, "__version__", "1.2.3")
@@ -304,7 +332,50 @@
 
     assert (
         tools.update_version(repo.initfile, GITHUB["release"], abort=False) == "0.0.3"
     )
     assert tools.get_module_var(repo.initfile) == "0.0.3"
     assert tools.get_module_var(repo.initfile, "__hash__") == "5547365c82"
     repo.revert(repo.initfile)
+
+
+def test_process(git_project_factory):
+    def write_tfile(tfile):
+        tfile.write_text("""
+{% for k, v in ctx.items() | sort -%}
+Key[{{k}}] = {{v}}
+{% endfor %}
+""")
+        return tfile
+
+    repo = git_project_factory().create("1.2.3")
+
+    # tfile won't appear in the repo.status() because is untracked
+    tfile = write_tfile(repo.workdir / "test.txt")
+
+    data = tools.process(repo.initfile, None, tfile)
+
+    assert data["hash"][-1] != "*"
+
+    assert tfile.read_text() == f"""
+Key[branch] = master
+Key[build] = 0
+Key[current] = 1.2.3
+Key[hash] = {data['hash']}
+Key[version] = 1.2.3
+"""
+
+    # clean and switch to new branch
+    repo.revert(repo.initfile)
+    write_tfile(tfile)
+    repo.branch("beta/1.2.3", "master")
+
+    data = tools.process(repo.initfile, None, tfile)
+    assert data["hash"][-1] != "*"
+
+    assert tfile.read_text() == f"""
+Key[branch] = beta/1.2.3
+Key[build] = 0
+Key[current] = 1.2.3
+Key[hash] = {data['hash']}
+Key[version] = 1.2.3b0
+"""
```

