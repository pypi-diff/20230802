# Comparing `tmp/setuptools-github-0.3.1b72.tar.gz` & `tmp/setuptools-github-0.3.1b73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.1b72.tar", last modified: Wed Aug  2 18:06:36 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.1b73.tar", last modified: Wed Aug  2 18:28:20 2023, max compression
```

## Comparing `setuptools-github-0.3.1b72.tar` & `setuptools-github-0.3.1b73.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:06:36.000000 setuptools-github-0.3.1b72/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:06:36.280653 setuptools-github-0.3.1b72/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-08-02 18:06:05.000000 setuptools-github-0.3.1b72/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.819696 setuptools-github-0.3.1b73/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:28:20.819696 setuptools-github-0.3.1b73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:28:20.819696 setuptools-github-0.3.1b73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 18:28:20.000000 setuptools-github-0.3.1b73/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:28:20.815696 setuptools-github-0.3.1b73/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-08-02 18:27:51.000000 setuptools-github-0.3.1b73/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.1b72/LICENSE` & `setuptools-github-0.3.1b73/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/PKG-INFO` & `setuptools-github-0.3.1b73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b72
+Version: 0.3.1b73
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.1b72/README.md` & `setuptools-github-0.3.1b73/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/pyproject.toml` & `setuptools-github-0.3.1b73/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/setup.py` & `setuptools-github-0.3.1b73/setup.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-import sys
 import pathlib
+import sys
 
 sys.path.insert(0, str(pathlib.Path(__file__).parent / "src"))
 from setuptools_github import tools  # noqa E402
 from setuptools import setup, find_namespace_packages  # noqa E402
 
 
 initfile = pathlib.Path(__file__).parent / "src/setuptools_github/__init__.py"
```

### Comparing `setuptools-github-0.3.1b72/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.1b73/setuptools_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.1b72
+Version: 0.3.1b73
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.1b72/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.1b73/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/src/setuptools_github/checks.py` & `setuptools-github-0.3.1b73/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/src/setuptools_github/cli.py` & `setuptools-github-0.3.1b73/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/src/setuptools_github/scm.py` & `setuptools-github-0.3.1b73/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/src/setuptools_github/script.py` & `setuptools-github-0.3.1b73/src/setuptools_github/script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/src/setuptools_github/tools.py` & `setuptools-github-0.3.1b73/src/setuptools_github/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,29 +338,30 @@
     Example:
         {'branch': 'beta/0.3.1',
          'build': 0,
          'current': '0.3.1',
          'hash': 'c9e484a*',
          'version': '0.3.1b0'}
     """
-    from jinja2 import Environment
     from argparse import Namespace
-    from urllib.parse import quote
     from functools import partial
+    from urllib.parse import quote
+
+    from jinja2 import Environment
 
     class Context(Namespace):
         def items(self):
             for name, value in self.__dict__.items():
                 if name.startswith("_"):
                     continue
                 yield (name, value)
 
     data = get_data(initfile, github_dump, abort)
     set_module_var(initfile, "__version__", data["version"])
     set_module_var(initfile, "__hash__", data["hash"])
 
-    env = Environment()
+    env = Environment(autoescape=True)
     env.filters["urlquote"] = partial(quote, safe="")
     for path in list_of_paths(paths):
         tmpl = env.from_string(path.read_text())
         path.write_text(tmpl.render(ctx=Context(**data)))
     return data
```

### Comparing `setuptools-github-0.3.1b72/tests/conftest.py` & `setuptools-github-0.3.1b73/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
+import collections
+import contextlib
 import os
-import sys
 import pathlib
 import shutil
-import contextlib
-import collections
 import subprocess
+import sys
 
 import pytest
 
 sys.path.insert(0, str(pathlib.Path(__file__).parent.parent / "src"))
 from setuptools_github import scm  # noqa F401,E402
 
 
@@ -58,15 +58,15 @@
         def run(self, args, cwd=None, load_data=True):
             cmd = [str(a) for a in [self.exe, self.script, *args]]
 
             with contextlib.ExitStack() as stack:
                 fpout = stack.enter_context((self.workdir / "stdout.txt").open("w"))
                 fperr = stack.enter_context((self.workdir / "stderr.txt").open("w"))
                 self.p = subprocess.Popen(
-                    cmd,
+                    cmd,  # noqa: S603
                     cwd=self.workdir if cwd is True else cwd,
                     stdout=fpout,
                     stderr=fperr,
                 )
                 self.p.communicate()
             out = (self.workdir / "stdout.txt").read_text()
             err = (self.workdir / "stderr.txt").read_text()
@@ -115,30 +115,31 @@
         # clone from repo
         repo2 = git_project_factory().create(clone=repo)
 
         assert repo.workdir != repo1.workdir
         assert repo.workdir != repo1.workdir
 
     """
+
     class GitRepoBase(scm.GitRepo):
-        def init(
-            self,
-            force: bool = False,
-            nobranch: bool = False
-        ) -> GitRepoBase:
+        def init(self, force: bool = False, nobranch: bool = False) -> GitRepoBase:
             from shutil import rmtree
 
             if force:
                 rmtree(self.workdir, ignore_errors=True)
             self.workdir.mkdir(parents=True, exist_ok=True if force else False)
 
             if not nobranch:
                 self(["init", "-b", "master"])
             else:
-                self(["init",])
+                self(
+                    [
+                        "init",
+                    ]
+                )
 
             self(["config", "user.name", "First Last"])
             self(["config", "user.email", "user@email"])
 
             if not nobranch:
                 self(["commit", "-m", "initial", "--allow-empty"])
             return self
@@ -172,22 +173,25 @@
                 clone.clone(self.workdir, force=force)
             else:
                 self.init(force=force, nobranch=nobranch)
             self.version(version)
             return self
 
     def id_generator(size=6):
-        from string import ascii_uppercase, digits
         from random import choice
+        from string import ascii_uppercase, digits
 
-        return "".join(choice(ascii_uppercase + digits) for _ in range(size))
+        return "".join(
+            choice(ascii_uppercase + digits) for _ in range(size)  # noqa: S311
+        )
 
     return lambda subdir="": Project(tmp_path / (subdir or id_generator()))
     # or request.node.name
 
+
 #####################
 # Main flags/config #
 #####################
 
 
 def pytest_configure(config):
     config.addinivalue_line("markers", "manual: test intented to run manually")
```

### Comparing `setuptools-github-0.3.1b72/tests/test_checks.py` & `setuptools-github-0.3.1b73/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/tests/test_cli.py` & `setuptools-github-0.3.1b73/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.1b72/tests/test_conftest.py` & `setuptools-github-0.3.1b73/tests/test_conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 def test_operation_create(git_project_factory):
     # simple git repo (only 1 .keep file and 1 .git dir)
     repo0 = git_project_factory().create()
-    assert set(f.name for f in repo0.workdir.glob("*")) == {".git"}
+    assert {f.name for f in repo0.workdir.glob("*")} == {".git"}
 
     # another repo with a "version" src/__init__.py file
     repo1 = git_project_factory().create("0.0.0")
-    assert set(f.name for f in repo1.workdir.glob("*")) == {".git", "src"}
+    assert {f.name for f in repo1.workdir.glob("*")} == {".git", "src"}
 
     # make sure they aren't the same
     assert repo0.workdir != repo1.workdir
     assert repo0.gitdir != repo1.gitdir
 
     # cloning
     repo2 = git_project_factory().create(clone=repo0)
     assert repo2.workdir != repo0.workdir
     assert repo2.gitdir != repo0.gitdir
-    assert set(f.name for f in repo2.workdir.glob("*")) == {".git"}
+    assert {f.name for f in repo2.workdir.glob("*")} == {".git"}
 
     repo3 = git_project_factory().create(clone=repo1)
     assert repo3.workdir != repo1.workdir
     assert repo3.gitdir != repo1.gitdir
-    assert set(f.name for f in repo3.workdir.glob("*")) == {".git", "src"}
+    assert {f.name for f in repo3.workdir.glob("*")} == {".git", "src"}
 
 
 def test_operation_dump(git_project_factory):
     repo = git_project_factory().create()
-    assert set(f.name for f in repo.workdir.glob("*")) == {".git"}
+    assert {f.name for f in repo.workdir.glob("*")} == {".git"}
 
     assert (
         repo.dumps(mask=True)
         == f"""\
 REPO: {repo.workdir}
  [status]
   On branch master
```

### Comparing `setuptools-github-0.3.1b72/tests/test_scm.py` & `setuptools-github-0.3.1b73/tests/test_scm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import subprocess
 
 import pytest
-
 from setuptools_github import scm
 
 
 def test_lookup(git_project_factory):
     repo = git_project_factory().create("0.0.0")
     dstdir = repo.workdir / "a" / "b" / "c"
     dstdir.mkdir(parents=True)
```

### Comparing `setuptools-github-0.3.1b72/tests/test_script.py` & `setuptools-github-0.3.1b73/tests/test_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from argparse import Namespace
+
 from setuptools_github import script
 
 
 class MyError(Exception):
     pass
```

### Comparing `setuptools-github-0.3.1b72/tests/test_tools.py` & `setuptools-github-0.3.1b73/tests/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from setuptools_github import tools
 
 # this is the output from ${{ toJson(github) }}
 GITHUB = {
     "beta": {
         "ref": "refs/heads/beta/0.0.4",
         "sha": "2169f90c22e",
```

