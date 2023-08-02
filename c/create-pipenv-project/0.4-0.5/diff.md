# Comparing `tmp/create_pipenv_project-0.4.tar.gz` & `tmp/create_pipenv_project-0.5.tar.gz`

## Comparing `create_pipenv_project-0.4.tar` & `create_pipenv_project-0.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/py.typed
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/terminal.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/_main_runner.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/env
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/logging.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/mypy.ini
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/run.py
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/create_pipenv_project/user_files/run_tests.sh
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/LICENSE
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/README.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/pyproject.toml
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 create_pipenv_project-0.4/PKG-INFO
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/py.typed
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/terminal.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/.gitignore
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/__init__.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/_main_runner.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/env
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/logging.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/mypy.ini
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/create_pipenv_project/user_files/run.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/LICENSE
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/pyproject.toml
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 create_pipenv_project-0.5/PKG-INFO
```

### Comparing `create_pipenv_project-0.4/create_pipenv_project/__init__.py` & `create_pipenv_project-0.5/create_pipenv_project/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4"
+__version__ = "0.5"
 
 import os
 import shutil
 import create_pipenv_project
 from create_pipenv_project.terminal import ANSICodes as ansi, print_error
 
 
@@ -61,15 +61,14 @@
             self.git_init()
 
     def _copy_user_files(self, project_name: str) -> None:
         mapping = {
             "env": ".env",
             ".gitignore": ".",
             "run.py": ".",
-            "run_tests.sh": ".",
             "mypy.ini": ".",
             "__init__.py": project_name,
             "_main_runner.py": project_name,
             "logging.py": project_name,
         }
 
         cpp_dirpath = os.path.dirname(create_pipenv_project.__file__)
@@ -107,20 +106,22 @@
 
         os.system("pipenv install --dev --skip-lock mypy black coverage pytest")
         FileOperations.insert_text(
             "Pipfile",
             5,
             "\n[scripts]",
             'app = "python run.py"',
-            'tests = "bash ./run_tests.sh"',
+            'mypy = "mypy ."',
+            'tests = "coverage run -m pytest"',
             'format = "black ."',
+            'mypy_install_types = "mypy --install-types"',
         )
         FileOperations.insert_text(
             "Pipfile",
-            12,
+            14,
             'uvloop = {version = "*", sys_platform = "== \'linux\'"}',
         )
         os.system("pipenv install")
 
     def git_init(self) -> None:
         os.system("git init")
         os.system("git branch -m main")
```

### Comparing `create_pipenv_project-0.4/create_pipenv_project/terminal.py` & `create_pipenv_project-0.5/create_pipenv_project/terminal.py`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/create_pipenv_project/user_files/.gitignore` & `create_pipenv_project-0.5/create_pipenv_project/user_files/.gitignore`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/create_pipenv_project/user_files/_main_runner.py` & `create_pipenv_project-0.5/create_pipenv_project/user_files/_main_runner.py`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/create_pipenv_project/user_files/logging.py` & `create_pipenv_project-0.5/create_pipenv_project/user_files/logging.py`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/create_pipenv_project/user_files/mypy.ini` & `create_pipenv_project-0.5/create_pipenv_project/user_files/mypy.ini`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/.gitignore` & `create_pipenv_project-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/LICENSE` & `create_pipenv_project-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/README.md` & `create_pipenv_project-0.5/README.md`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/pyproject.toml` & `create_pipenv_project-0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `create_pipenv_project-0.4/PKG-INFO` & `create_pipenv_project-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create_pipenv_project
-Version: 0.4
+Version: 0.5
 Summary: A CLI tool for creating Python projects with Pipenv workflow.
 Project-URL: Repository, https://github.com/nietsuu/create_pipenv_project
 Author-email: Nie Tsuu <nietsuu@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: pipenv
 Description-Content-Type: text/markdown
```

