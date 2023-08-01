# Comparing `tmp/auto_click_auto-0.1.0a4.tar.gz` & `tmp/auto_click_auto-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_click_auto-0.1.0a4.tar", max compression
+gzip compressed data, was "auto_click_auto-0.1.0a5.tar", max compression
```

## Comparing `auto_click_auto-0.1.0a4.tar` & `auto_click_auto-0.1.0a5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     5252 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/README.md
--rw-r--r--   0        0        0       99 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/auto_click_auto/__init__.py
--rw-r--r--   0        0        0      532 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/auto_click_auto/constants.py
--rw-r--r--   0        0        0     5325 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/core.py
--rw-r--r--   0        0        0      643 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/py.typed
--rw-r--r--   0        0        0     3037 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/utils.py
--rw-r--r--   0        0        0     1476 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     5252 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/README.md
+-rw-r--r--   0        0        0       99 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/auto_click_auto/__init__.py
+-rw-r--r--   0        0        0      532 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/auto_click_auto/constants.py
+-rw-r--r--   0        0        0     5681 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/auto_click_auto/core.py
+-rw-r--r--   0        0        0      643 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/auto_click_auto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/auto_click_auto/py.typed
+-rw-r--r--   0        0        0     3992 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/auto_click_auto/utils.py
+-rw-r--r--   0        0        0     1476 2023-08-01 22:58:45.725305 auto_click_auto-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a5/PKG-INFO
```

### Comparing `auto_click_auto-0.1.0a4/LICENSE` & `auto_click_auto-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a4/README.md` & `auto_click_auto-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a4/auto_click_auto/constants.py` & `auto_click_auto-0.1.0a5/auto_click_auto/constants.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a4/auto_click_auto/core.py` & `auto_click_auto-0.1.0a5/auto_click_auto/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 from typing import TYPE_CHECKING, Any, Callable, Optional, Set, TypeVar, Union
 
 from click import Command, Context, Parameter, option
 
 from .constants import ShellType
 from .exceptions import ShellEnvVarNotFoundError, ShellTypeNotSupportedError
-from .utils import add_shell_configuration, detect_shell
+from .utils import add_shell_configuration, create_file, detect_shell
 
 if TYPE_CHECKING:
     import typing_extensions as te
 
 R = TypeVar("R")
 T = TypeVar("T")
 _AnyCallable = Callable[..., Any]
@@ -83,14 +83,20 @@
             )
 
         elif shell == ShellType.FISH:
             completer_script_path = os.path.expanduser(
                 f"~/.config/fish/completions/{program_name}.{shell}"
             )
 
+            # bash and zsh config files are generic, so we can assume the user
+            # already has created them. fish's shell configuration file for
+            # custom completions is specific to the program name, so we will
+            # create it if it doesn't already exist.
+            create_file(file_path=completer_script_path)
+
             # Completion implementation: `eval` command in shell configuration
             eval_command = (
                 f"eval (env {click_env_var}={shell.value}_source "
                 f"{program_name})"
             )
             add_shell_configuration(
                 shell_config_file=completer_script_path,
```

### Comparing `auto_click_auto-0.1.0a4/auto_click_auto/exceptions.py` & `auto_click_auto-0.1.0a5/auto_click_auto/exceptions.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a4/auto_click_auto/utils.py` & `auto_click_auto-0.1.0a5/auto_click_auto/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,35 @@
 from auto_click_auto.exceptions import (
     ShellConfigurationFileNotFoundError,
     ShellEnvVarNotFoundError,
     ShellTypeNotSupportedError,
 )
 
 
+def create_file(file_path: str) -> None:
+    """
+    Check if the file and the directories of the given file path exist and if
+    not create them.
+
+    :param file_path: The path of the file the check and creation is done for.
+    :return: `None`
+    """
+
+    if not os.path.exists(file_path):
+        directory = os.path.dirname(file_path)
+
+        if not os.path.exists(directory):
+            # Recursive directory creation
+            os.makedirs(directory)
+
+        # Open for exclusive creation, failing if the file already exists
+        with open(file_path, 'x'):
+            pass
+
+
 def check_strings_in_file(file_path: str, search_strings: List[str]) -> bool:
     """
     Check if the given search strings are in the specified file.
 
     :param file_path: The path of the file the search is done for.
     :param search_strings: The strings that are searched for in the file.
     :return: `True`, if any of the strings are found in the file, and `False`
@@ -79,14 +100,24 @@
         print(
             "Tab autocomplete configuration already setup in "
             f"{shell_config_file}."
         )
 
 
 def detect_shell() -> ShellType:
+    """
+    Attempt to detect the shell type using the `SHELL` environment variable.
+
+    :raise ShellEnvVarNotFoundError: When the `SHELL` environment variable is
+    not set in the system.
+    :raise ShellTypeNotSupportedError: When the shell value returned from the
+    `SHELL` environment variable does not belong to one of the supported
+    shells.
+    """
+
     try:
         shell_env_var = os.environ["SHELL"]
 
     except KeyError:
         raise ShellEnvVarNotFoundError(
             "Could not infer the shell type from the 'SHELL' environment "
             "variable."
```

### Comparing `auto_click_auto-0.1.0a4/pyproject.toml` & `auto_click_auto-0.1.0a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-click-auto"
-version = "0.1.0-alpha.4"
+version = "0.1.0-alpha.5"
 description = "Automatically enable tab autocompletion for shells in Click CLI applications."
 authors = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 maintainers = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/KAUTH/auto-click-auto"
 repository = "https://github.com/KAUTH/auto-click-auto"
```

### Comparing `auto_click_auto-0.1.0a4/PKG-INFO` & `auto_click_auto-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-click-auto
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Automatically enable tab autocompletion for shells in Click CLI applications.
 Home-page: https://github.com/KAUTH/auto-click-auto
 License: MIT
 Keywords: click,autocomplete,shell
 Author: Konstantinos Papadopoulos
 Author-email: konpap1996@yahoo.com
 Maintainer: Konstantinos Papadopoulos
```

