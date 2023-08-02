# Comparing `tmp/cook-build-0.4.0.tar.gz` & `tmp/cook-build-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook-build-0.4.0.tar", last modified: Tue Jul 25 19:51:39 2023, max compression
+gzip compressed data, was "cook-build-0.4.1.tar", last modified: Wed Aug  2 17:56:14 2023, max compression
```

## Comparing `cook-build-0.4.0.tar` & `cook-build-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:51:39.420446 cook-build-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-25 19:51:03.000000 cook-build-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-25 19:51:39.420446 cook-build-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-25 19:51:03.000000 cook-build-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:51:39.420446 cook-build-0.4.0/cook/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-25 19:51:03.000000 cook-build-0.4.0/cook/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:51:39.420446 cook-build-0.4.0/cook_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-25 19:51:39.000000 cook-build-0.4.0/cook_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-25 19:51:39.000000 cook-build-0.4.0/cook_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:51:39.000000 cook-build-0.4.0/cook_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 19:51:39.000000 cook-build-0.4.0/cook_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:51:39.000000 cook-build-0.4.0/cook_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 19:51:39.000000 cook-build-0.4.0/cook_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-25 19:51:39.424446 cook-build-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 19:51:03.000000 cook-build-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:51:39.420446 cook-build-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 19:51:03.000000 cook-build-0.4.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:14.224237 cook-build-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-02 17:55:42.000000 cook-build-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 17:56:14.224237 cook-build-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-02 17:55:42.000000 cook-build-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:14.220237 cook-build-0.4.1/cook/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-02 17:55:42.000000 cook-build-0.4.1/cook/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:14.220237 cook-build-0.4.1/cook_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 17:56:14.000000 cook-build-0.4.1/cook_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-02 17:56:14.000000 cook-build-0.4.1/cook_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:56:14.000000 cook-build-0.4.1/cook_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 17:56:14.000000 cook-build-0.4.1/cook_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 17:56:14.000000 cook-build-0.4.1/cook_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 17:56:14.000000 cook-build-0.4.1/cook_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 17:56:14.224237 cook-build-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 17:55:42.000000 cook-build-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:56:14.224237 cook-build-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 17:55:42.000000 cook-build-0.4.1/tests/test_util.py
```

### Comparing `cook-build-0.4.0/LICENSE` & `cook-build-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/PKG-INFO` & `cook-build-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook-build
-Version: 0.4.0
+Version: 0.4.1
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 🧑‍🍳 Cook
 ==========
```

### Comparing `cook-build-0.4.0/README.rst` & `cook-build-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/cook/__main__.py` & `cook-build-0.4.1/cook/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 from pathlib import Path
 import re
 import sqlite3
 import sys
 import textwrap
 from typing import Iterable, List, Optional
+
 from .contexts import create_target_directories, normalize_action, normalize_dependencies
 from .controller import Controller, QUERIES
 from .manager import Manager
 from .task import Task
 from .util import FailedTaskError, format_datetime, format_timedelta
 
 
@@ -29,114 +30,114 @@
         else:
             *patterns, last = patterns
             message = "found no tasks matching patterns " + ", ".join(patterns) \
                 + (", or " if len(patterns) > 1 else " or ") + last
         super().__init__(message)
 
 
-def discover_tasks(tasks: Iterable[Task], patterns: Iterable[re.Pattern], use_re: bool) \
-        -> List[Task]:
-    """
-    Discover tasks based on regular expressions.
-    """
-    if not patterns:
-        return list(tasks)
-    tasks = [task for task in tasks if any(
-        re.match(pat, task.name) if use_re else fnmatch.fnmatch(task.name, pat) for pat in patterns
-    )]
-    if not tasks:
-        raise NoMatchingTaskError(patterns)
-    return tasks
+class Args:
+    tasks: Iterable[re.Pattern]
+    re: bool
+    all: bool
 
 
 class Command:
     """
     Abstract base class for commands.
     """
     NAME: Optional[str] = None
 
-    def __init__(self) -> None:
-        pass
-
     def configure_parser(self, parser: argparse.ArgumentParser) -> None:
-        raise NotImplementedError
+        parser.add_argument("--re", "-r", action="store_true",
+                            help="use regular expressions for pattern matching instead of glob")
+        parser.add_argument("--all", "-a", action="store_true",
+                            help="include tasks starting with `_` prefix")
+        parser.add_argument("tasks", nargs="*",
+                            help="task or tasks to execute as regular expressions")
 
     def execute(self, controller: Controller, args: argparse.Namespace) -> None:
         raise NotImplementedError
 
+    def discover_tasks(self, controller: Controller, args: Args) -> List[Task]:
+        if not args.tasks:
+            return list(controller.dependencies)
 
-class ExecArgs(argparse.Namespace):
-    tasks: Iterable[re.Pattern]
-    re: bool
+        tasks: List[Task] = []
+        task: Task
+        for task in controller.dependencies:
+            match = any(re.match(pattern, task.name) for pattern in args.tasks) if args.re else \
+                any(fnmatch.fnmatch(task.name, pattern) for pattern in args.tasks)
+            match = match and (args.all or not task.name.startswith("_"))
+            if match:
+                tasks.append(task)
+        if not tasks:
+            raise NoMatchingTaskError(args.tasks)
+        return tasks
+
+
+class ExecArgs(Args):
     jobs: int
 
 
 class ExecCommand(Command):
     """
     Execute one or more tasks.
     """
     NAME = "exec"
 
     def configure_parser(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("--re", "-r", action="store_true",
-                            help="use regular expressions for pattern matching instead of glob")
         parser.add_argument("--jobs", "-j", help="number of concurrent jobs", type=int, default=1)
-        parser.add_argument("tasks", nargs="+",
-                            help="task or tasks to execute as regular expressions")
+        super().configure_parser(parser)
 
     def execute(self, controller: Controller, args: ExecArgs) -> None:
-        tasks = discover_tasks(controller.dependencies, args.tasks, args.re)
+        tasks = self.discover_tasks(controller, args)
         controller.execute(tasks, num_concurrent=args.jobs)
 
 
-class LsArgs(argparse.Namespace):
-    tasks: Iterable[re.Pattern]
-    all: bool
-    re: bool
+class LsArgs(Args):
+    stale: bool
+    current: bool
 
 
 class LsCommand(Command):
     """
     List tasks.
     """
     NAME = "ls"
 
     def configure_parser(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("--all", "-a", action="store_true",
-                            help="include tasks starting with `_` prefix")
-        parser.add_argument("--re", "-r", action="store_true",
-                            help="use regular expressions for pattern matching instead of glob")
-        parser.add_argument("tasks", nargs="*",
-                            help="task or tasks to execute as regular expressions")
+        parser.add_argument("--stale", "-s", action="store_true", help="only show stale tasks")
+        parser.add_argument("--current", "-c", action="store_true", help="only show current tasks")
+        super().configure_parser(parser)
 
     def execute(self, controller: Controller, args: LsArgs) -> None:
-        tasks = discover_tasks(controller.dependencies, args.tasks, args.re)
-        if not args.all:
-            tasks = [task for task in tasks if not task.name.startswith("_")]
-        print("\n".join(map(str, tasks)))
-
-
-class InfoArgs(argparse.Namespace):
-    pass
+        tasks = self.discover_tasks(controller, args)
+        tasks = [task.format(colorama.Fore.YELLOW if is_stale else colorama.Fore.GREEN)
+                 for is_stale, task in zip(controller.is_stale(tasks), tasks)]
+        print("\n".join(tasks))
+
+    def discover_tasks(self, controller: Controller, args: LsArgs) -> List[Task]:
+        if args.current and args.stale:
+            raise ValueError("only one of `--stale` and `--current` may be given at the same time")
+        tasks = super().discover_tasks(controller, args)
+        if args.stale:
+            return [task for stale, task in zip(controller.is_stale(tasks), tasks) if stale]
+        elif args.current:
+            return [task for stale, task in zip(controller.is_stale(tasks), tasks) if not stale]
+        return tasks
 
 
-class InfoCommand(Command):
+class InfoCommand(LsCommand):
     """
     Display information about one or more tasks.
     """
     NAME = "info"
 
-    def configure_parser(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("--re", "-r", action="store_true",
-                            help="use regular expressions for pattern matching instead of glob")
-        parser.add_argument("tasks", nargs="*",
-                            help="task or tasks to execute as regular expressions")
-
-    def execute(self, controller: Controller, args: InfoArgs) -> None:
-        tasks = discover_tasks(controller.dependencies, args.tasks, args.re)
+    def execute(self, controller: Controller, args: LsArgs) -> None:
+        tasks = self.discover_tasks(controller, args)
         stales = controller.is_stale(tasks)
 
         stale_string = f"{colorama.Fore.YELLOW}stale{colorama.Fore.RESET}"
         current_string = f"{colorama.Fore.GREEN}current{colorama.Fore.RESET}"
         indent = "    "
 
         task: Task
@@ -153,15 +154,26 @@
             for key, value in zip(["completed", "failed"], last):
                 if value is None:
                     parts.append(f"last {key}: -")
                     continue
                 parts.append(f"last {key}: {format_timedelta(datetime.now() - value)} ago "
                              f"({format_datetime(value)})")
             # Show dependencies and targets.
-            for key, value in [("dependencies", task.dependencies), ("targets", task.targets)]:
+            task_dependencies = list(sorted(controller.dependencies.successors(task),
+                                            key=lambda t: t.name))
+            task_dependencies = [
+                dep.format(colorama.Fore.YELLOW if is_stale else colorama.Fore.GREEN)
+                for is_stale, dep in zip(controller.is_stale(task_dependencies), task_dependencies)
+            ]
+            items = [
+                ("dependencies", task.dependencies),
+                ("targets", task.targets),
+                ("task_dependencies", task_dependencies),
+            ]
+            for key, value in items:
                 value = "\n".join(map(str, value))
                 if value:
                     parts.append(f"{key}:\n{textwrap.indent(value, indent)}")
                 else:
                     parts.append(f"{key}: -")
             parts.append(f"action: {task.action if task.action else '-'}")
 
@@ -176,37 +188,35 @@
 
 class ResetCommand(Command):
     """
     Reset the status of one or more tasks.
     """
     NAME = "reset"
 
-    def configure_parser(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("--re", "-r", action="store_true",
-                            help="use regular expressions for pattern matching instead of glob")
-        parser.add_argument("tasks", nargs="*",
-                            help="task or tasks to execute as regular expressions")
-
     def execute(self, controller: Controller, args: ResetArgs) -> None:
-        controller.reset(*discover_tasks(controller.dependencies, args.tasks, args.re))
+        tasks = self.discover_tasks(controller, args)
+        controller.reset(*tasks)
 
 
 class Formatter(logging.Formatter):
     COLOR_BY_LEVEL = {
         "DEBUG": colorama.Fore.MAGENTA,
         "INFO": colorama.Fore.BLUE,
         "WARNING": colorama.Fore.YELLOW,
         "ERROR": colorama.Fore.RED,
         "CRITICAL": colorama.Fore.WHITE + colorama.Back.RED,
     }
     RESET = colorama.Fore.RESET + colorama.Back.RESET
 
     def format(self, record: logging.LogRecord) -> str:
         color = self.COLOR_BY_LEVEL[record.levelname]
-        return f"{color}{record.levelname}{self.RESET}: {record.getMessage()}"
+        formatted = f"{color}{record.levelname}{self.RESET}: {record.getMessage()}"
+        if record.exc_info:
+            formatted = f"{formatted}\n{self.formatException(record.exc_info)}"
+        return formatted
 
 
 def __main__(cli_args: Optional[List[str]] = None) -> None:
     parser = argparse.ArgumentParser("cook")
     parser.add_argument("--recipe", help="file containing declarative recipe for tasks",
                         default="recipe.py", type=Path)
     parser.add_argument("--module", "-m", help="module containing declarative recipe for tasks")
@@ -247,19 +257,19 @@
                 spec = importlib.util.spec_from_file_location("recipe", args.recipe)
                 recipe = importlib.util.module_from_spec(spec)
                 spec.loader.exec_module(recipe)
             else:  # pragma: no cover
                 raise ValueError("recipe file or module must be specified; default recipe.py not "
                                  "found")
         except:  # noqa: E722
-            LOGGER.fatal("failed to load recipe")
+            LOGGER.fatal("failed to load recipe", exc_info=sys.exc_info())
             sys.exit(1)
 
     with sqlite3.connect(args.db, detect_types=sqlite3.PARSE_DECLTYPES) as connection:
-        connection.execute(QUERIES["schema"])
+        connection.executescript(QUERIES["schema"])
         controller = Controller(manager.resolve_dependencies(), connection)
         command: Command = args.command
         try:
             command.execute(controller, args)
         except KeyboardInterrupt:  # pragma: no cover
             LOGGER.warning("interrupted by user")
         except NoMatchingTaskError as ex:
```

### Comparing `cook-build-0.4.0/cook/actions.py` & `cook-build-0.4.1/cook/actions.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/cook/contexts.py` & `cook-build-0.4.1/cook/contexts.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/cook/controller.py` & `cook-build-0.4.1/cook/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,45 +3,64 @@
 import logging
 import networkx as nx
 from pathlib import Path
 from queue import Empty, Queue
 from sqlite3 import Connection
 import sys
 import threading
-import time
 from typing import Dict, List, Optional, Sequence, Set, Tuple, TYPE_CHECKING, Union
 from . import util
 
 if TYPE_CHECKING:
     from .task import Task
 
 
 LOGGER = logging.getLogger(__name__)
 QUERIES = {
     "schema": """
+    -- Information about the status of tasks.
     CREATE TABLE IF NOT EXISTS "tasks" (
         "name" TEXT PRIMARY KEY,
         "digest" TEXT NOT NULL,
         "last_completed" TIMESTAMP,
         "last_failed" TIMESTAMP
-    )
+    );
+
+    -- Information about files so we can cache digests.
+    CREATE TABLE IF NOT EXISTS "files" (
+        "name" TEXT PRIMARY KEY,
+        "digest" TEXT NOT NULL,
+        "last_digested" TIMESTAMP NOT NULL
+    );
     """,
-    "select": """
-        SELECT "digest" FROM "files" WHERE "name" = :name
+    "select_task": """
+        SELECT "digest"
+        FROM "files"
+        WHERE "name" = :name
     """,
-    "upsert_completed": """
+    "upsert_task_completed": """
         INSERT INTO "tasks" ("name", "digest", "last_completed")
         VALUES (:name, :digest, :last_completed)
-        ON CONFLICT("name") DO UPDATE SET "digest" = :digest, last_completed = :last_completed
+        ON CONFLICT ("name") DO UPDATE SET "digest" = :digest, last_completed = :last_completed
     """,
-    "upsert_failed": """
+    "upsert_task_failed": """
         INSERT INTO "tasks" ("name", "digest", "last_failed")
         VALUES (:name, '__failed__', :last_failed)
-        ON CONFLICT("name") DO UPDATE SET "digest" = '__failed__', last_failed = :last_failed
+        ON CONFLICT ("name") DO UPDATE SET "digest" = '__failed__', last_failed = :last_failed
+    """,
+    "upsert_file": """
+        INSERT INTO "files" ("name", "digest", "last_digested")
+        VALUES (:name, :digest, :last_digested)
+        ON CONFLICT ("name") DO UPDATE SET "digest" = :digest, last_digested = :last_digested
     """,
+    "select_file": """
+        SELECT "digest", "last_digested"
+        FROM "files"
+        WHERE "name" = :name AND last_digested > :last_modified
+    """
 }
 
 
 class Controller:
     """
     Controller to manage dependencies and execute tasks.
     """
@@ -50,45 +69,58 @@
         self.connection = connection
         self._digest_cache: Dict[Path, Tuple[float, bytes]] = {}
 
     def resolve_stale_tasks(self, tasks: Optional[List["Task"]] = None) -> Set["Task"]:
         self.is_stale(tasks or list(self.dependencies))
         return {node for node, data in self.dependencies.nodes(True) if data.get("is_stale")}
 
-    def _evaluate_path_digest(self, path: Path) -> bytes:
-        """
-        Evaluate the digest of a file.
-        """
-        path = Path(path).resolve()
-        cached = self._digest_cache.get(path)
-        if cached:
-            digested, digest = cached
-            if path.stat().st_mtime < digested:
-                return digest
-        digest = util.evaluate_digest(path)
-        self._digest_cache[path] = (time.time(), digest)
-        return digest
-
-    def _evaluate_task_hexdigest(self, task: "Task") -> bytes:
+    def _evaluate_task_hexdigest(self, task: "Task") -> str:
         """
         Evaluate the digest of a task by combining the digest of all its dependencies.
         """
         dependencies = []
         for dependency in task.dependencies:
             dependency = Path(dependency).resolve()
             if not dependency.is_file():
                 LOGGER.debug("dependency %s of %s is missing", dependency, task)
                 return None
             dependencies.append(dependency)
 
         hasher = hashlib.sha1()
         for dependency in sorted(dependencies):
-            hasher.update(util.evaluate_digest(dependency))
+            hasher.update(bytearray.fromhex(self._evaluate_path_hexdigest(dependency)))
         return hasher.hexdigest()
 
+    def _evaluate_path_hexdigest(self, path: Union[Path, str]) -> str:
+        """
+        Get the digest of a file.
+        """
+        # Try to return the cached digest.
+        path = Path(path)
+        stat = path.stat()
+        name = str(path.resolve())
+        params = {
+            "name": name,
+            "last_modified": datetime.fromtimestamp(stat.st_mtime)
+        }
+        digest = self.connection.execute(QUERIES["select_file"], params).fetchone()
+        if digest:
+            return digest[0]
+
+        # Evaluate a new digest and cache it.
+        digest = util.evaluate_hexdigest(path)
+        params = {
+            "name": name,
+            "last_digested": datetime.now(),
+            "digest": digest,
+        }
+        self.connection.execute(QUERIES["upsert_file"], params)
+        self.connection.commit()
+        return digest
+
     def is_stale(self, task: Union["Task", Sequence["Task"]]) -> Union[bool, List[bool]]:
         """
         Determine if one or more tasks are stale.
 
         Args:
             task: Task or tasks to check.
 
@@ -169,18 +201,18 @@
         stop = util.StopEvent(interval)
         for i in range(num_concurrent):
             thread = threading.Thread(target=self._target, name=f"cook-thread-{i}",
                                       args=(stop, input_queue, output_queue), daemon=True)
             thread.start()
             threads.append(thread)
 
-        # Create a copy of the dependency graph and filter it to remove all non-stale tasks.
-        dependencies: nx.DiGraph = self.dependencies.copy()
-        not_stale = [node for node, data in dependencies.nodes.data() if not data.get("is_stale")]
-        dependencies.remove_nodes_from(not_stale)
+        # Get the subgraph of stale nodes.
+        stale_nodes = [node for node, data in self.dependencies.nodes.data() if
+                       data.get("is_stale")]
+        dependencies: nx.DiGraph = self.dependencies.subgraph(stale_nodes).copy()
 
         # Initialize the input queue with leaf nodes.
         for node, out_degree in dependencies.out_degree():
             if out_degree == 0:
                 input_queue.put(node)
 
         try:
@@ -202,15 +234,15 @@
                 task, exc_info = item
                 if exc_info:
                     # Update the status in the database.
                     params = {
                         "name": task.name,
                         "last_failed": datetime.now(),
                     }
-                    self.connection.execute(QUERIES["upsert_failed"], params)
+                    self.connection.execute(QUERIES["upsert_task_failed"], params)
                     self.connection.commit()
                     raise util.FailedTaskError(task=task) from exc_info[1]
 
                 # Add tasks that are now leaf nodes to the tree.
                 predecessors = list(dependencies.predecessors(task))
                 dependencies.remove_node(task)
                 self.dependencies.add_node(task, is_stale=False)
@@ -227,15 +259,15 @@
 
                 # Update the status in the database.
                 params = {
                     "name": task.name,
                     "digest": self._evaluate_task_hexdigest(task),
                     "last_completed": datetime.now(),
                 }
-                self.connection.execute(QUERIES["upsert_completed"], params)
+                self.connection.execute(QUERIES["upsert_task_completed"], params)
                 self.connection.commit()
         finally:
             # Set the stop event and add "None" to the queue so the workers stop waiting.
             LOGGER.debug("set stop event for threads: %s", [thread.name for thread in threads])
             stop.set()
             for thread in threads:
                 input_queue.put(None)
@@ -276,12 +308,15 @@
                 output_queue.put((task, sys.exc_info()))
 
         # Put anything on the queue in case the parent is waiting.
         LOGGER.debug(f"exiting thread `{threading.current_thread().name}`")
         output_queue.put(None)
 
     def reset(self, *tasks: "Task") -> None:
-        params = [{"name": task.name for task in tasks}]
-        self.connection.executemany("UPDATE tasks SET digest = '__reset__' WHERE name = :name",
-                                    params)
+        # TODO: add tests for resetting.
+        params = [{"name": task.name} for task in tasks]
+        cursor = self.connection.executemany(
+            "UPDATE tasks SET digest = '__reset__' WHERE name = :name", params
+        )
         self.connection.commit()
-        LOGGER.info("reset %d %s", len(tasks), "task" if len(tasks) == 1 else "tasks")
+        n_reset = cursor.rowcount
+        LOGGER.info("reset %d %s", n_reset, "task" if n_reset == 1 else "tasks")
```

### Comparing `cook-build-0.4.0/cook/manager.py` & `cook-build-0.4.1/cook/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,18 +56,18 @@
             task = task_.Task(name, **kwargs)
             for context in reversed(self.contexts):
                 task = context.apply(task)
                 if task is None:
                     raise ValueError(f"{context} did not return a task")
             self.tasks[name] = task
             return task
-        except Exception as ex:
+        except:  # noqa: 722
             filename, lineno = util.get_location()
-            LOGGER.error("failed to create task with name '%s' at %s:%d: %s", name, filename,
-                         lineno, ex)
+            LOGGER.exception("failed to create task with name '%s' at %s:%d", name, filename,
+                             lineno)
             raise
 
     def resolve_dependencies(self) -> nx.DiGraph:
         """
         Resolve dependencies between tasks.
 
         Returns:
@@ -77,14 +77,17 @@
         task_by_target: Dict[Path, "Task"] = {}
         tasks_by_file_dependency: Dict[Path, List["Task"]] = {}
         dependencies: Dict["Task", Set["Task"]] = {}
         for task in self.tasks.values():
             if task.task_dependencies:
                 dependencies[task] = set(task.task_dependencies)
             for path in task.targets:
+                if path.is_symlink():
+                    LOGGER.warning("target %s of %s is a symlink which may lead to unexpected "
+                                   "behavior", path, task)
                 path = path.resolve()
                 if (other := task_by_target.get(path)):
                     raise ValueError(f"tasks {task} and {other} both have target {path}")
                 task_by_target[path] = task
             for path in task.dependencies:
                 path = path.resolve()
                 tasks_by_file_dependency.setdefault(path, set()).add(task)
```

### Comparing `cook-build-0.4.0/cook/task.py` & `cook-build-0.4.1/cook/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import colorama
 from pathlib import Path
 import threading
 from typing import List, Optional, Tuple, TYPE_CHECKING
 from . import util
 
 
 if TYPE_CHECKING:
@@ -34,10 +35,16 @@
     def execute(self, stop: Optional[threading.Event] = None) -> None:
         if self.action:
             self.action.execute(self, stop)
 
     def __hash__(self) -> int:
         return hash(self.name)
 
-    def __repr__(self) -> str:
+    def format(self, color: str = None) -> str:
+        name = self.name
+        if color:
+            name = f"{color}{name}{colorama.Fore.RESET}"
         filename, lineno = self.location
-        return f"<task `{self.name}` @ {filename}:{lineno}>"
+        return f"<task `{name}` @ {filename}:{lineno}>"
+
+    def __repr__(self) -> str:
+        return self.format()
```

### Comparing `cook-build-0.4.0/cook/util.py` & `cook-build-0.4.1/cook/util.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/cook_build.egg-info/PKG-INFO` & `cook-build-0.4.1/cook_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook-build
-Version: 0.4.0
+Version: 0.4.1
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 🧑‍🍳 Cook
 ==========
```

### Comparing `cook-build-0.4.0/cook_build.egg-info/SOURCES.txt` & `cook-build-0.4.1/cook_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/setup.py` & `cook-build-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     .replace(":class:", ":code:") \
     .replace(".. toctree::", "..") \
     .replace(".. sh::", "..")
 
 
 setup(
     name="cook-build",
-    version="0.4.0",
+    version="0.4.1",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     python_requires=">=3.8",
     install_requires=[
         "colorama",
         "networkx",
     ],
```

### Comparing `cook-build-0.4.0/tests/test_actions.py` & `cook-build-0.4.1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/tests/test_contexts.py` & `cook-build-0.4.1/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.4.0/tests/test_controller.py` & `cook-build-0.4.1/tests/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,21 +45,21 @@
 
     # Up to date entry in the database.
     params = {
         "name": "foo",
         "digest": "80d4129af3d5366c3fcd26c498e143d9a199f7c4",
         "last_completed": None,
     }
-    conn.execute(QUERIES["upsert_completed"], params)
+    conn.execute(QUERIES["upsert_task_completed"], params)
     c = Controller(m.resolve_dependencies(), conn)
     assert not c.is_stale(task)
 
     # Wrong digest in the database.
     params = {"name": "foo", "digest": "-", "last_completed": None}
-    conn.execute(QUERIES["upsert_completed"], params)
+    conn.execute(QUERIES["upsert_task_completed"], params)
     c = Controller(m.resolve_dependencies(), conn)
     assert c.is_stale(task)
 
 
 def test_controller_missing_input(m: Manager, conn: Connection) -> None:
     with normalize_dependencies():
         m.create_task("input", targets=["input.txt"], action=FunctionAction(touch))
@@ -69,15 +69,15 @@
     # Create the output.
     Path("output.txt").write_text("output.txt")
     params = {
         "name": "output",
         "digest": "80d4129af3d5366c3fcd26c498e143d9a199f7c4",
         "last_completed": None,
     }
-    conn.execute(QUERIES["upsert_completed"], params)
+    conn.execute(QUERIES["upsert_task_completed"], params)
     c = Controller(m.resolve_dependencies(), conn)
     assert c.is_stale(output) is True
 
 
 def test_controller(m: Manager, conn: Connection) -> None:
     for filename in ["input1.txt", "input2.txt", "intermediate.txt", "output1.txt"]:
         Path(filename).write_text(filename)
@@ -155,17 +155,17 @@
         c.execute(task, num_concurrent=num_tasks)
     assert timer.duration < 2 * delay
 
 
 def test_digest_cache(m: Manager, conn: Connection, tmp_wd: Path) -> None:
     c = Controller(m.resolve_dependencies(), conn)
     shutil.copy(__file__, tmp_wd / "foo")
-    with patch("cook.util.evaluate_digest") as evaluate_digest:
-        c._evaluate_path_digest("foo")
-        c._evaluate_path_digest("foo")
+    with patch("cook.util.evaluate_digest", return_value=b"aaaa") as evaluate_digest:
+        c._evaluate_path_hexdigest("foo")
+        c._evaluate_path_hexdigest("foo")
     evaluate_digest.assert_called_once()
 
 
 def test_skip_if_no_stale_tasks(m: Manager, conn: Connection, tmp_wd: Path) -> None:
     c = Controller(m, conn)
     c.execute([])
```

### Comparing `cook-build-0.4.0/tests/test_main.py` & `cook-build-0.4.1/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from cook.__main__ import __main__, Formatter
 import logging
 from pathlib import Path
 import pytest
 import shutil
+import sys
 from typing import List
 
 
 RECIPES = Path(__file__).parent / "recipes"
 
 
 def test_blah_recipe_run(tmp_wd: Path) -> None:
@@ -19,15 +20,15 @@
     (["--re", r"^\w{3}\w?$"], ["link", "run"]),
     (["run"], ["run"]),
 ])
 def test_blah_recipe_ls(patterns: str, expected: List[str], capsys: pytest.CaptureFixture) -> None:
     __main__(["--recipe", str(RECIPES / "blah.py"), "ls", *patterns])
     out, _ = capsys.readouterr()
     for task in expected:
-        assert f"<task `{task}` @ " in out
+        assert f"<task `{task}` @ " in pytest.shared.strip_colors(out)
 
 
 def test_blah_recipe_info(tmp_wd: Path, capsys: pytest.CaptureFixture) -> None:
     __main__(["--recipe", str(RECIPES / "blah.py"), "info", "link"])
     stdout, _ = capsys.readouterr()
     assert "status: stale" in pytest.shared.strip_colors(stdout)
 
@@ -36,14 +37,32 @@
     stdout, _ = capsys.readouterr()
     assert "status: current" in pytest.shared.strip_colors(stdout)
 
     __main__(["--recipe", str(RECIPES / "blah.py"), "info", "run"])
     stdout, _ = capsys.readouterr()
     assert "targets: -" in pytest.shared.strip_colors(stdout)
 
+    # Check filtering based on stale/current status.
+    __main__(["--recipe", str(RECIPES / "blah.py"), "info", "--stale"])
+    stdout, _ = capsys.readouterr()
+    assert "status: current" not in pytest.shared.strip_colors(stdout)
+
+    __main__(["--recipe", str(RECIPES / "blah.py"), "info", "--current"])
+    stdout, _ = capsys.readouterr()
+    assert "status: stale" not in pytest.shared.strip_colors(stdout)
+
+    __main__(["--recipe", str(RECIPES / "blah.py"), "info"])
+    stdout, _ = capsys.readouterr()
+    stdout = pytest.shared.strip_colors(stdout)
+    assert "status: stale" in stdout and "status: current" in stdout
+
+    # Check only one can be given.
+    with pytest.raises(ValueError, match="may be given at the same time"):
+        __main__(["--recipe", str(RECIPES / "blah.py"), "info", "--current", "--stale"])
+
 
 def test_blah_recipe_reset(tmp_wd: Path) -> None:
     __main__(["--recipe", str(RECIPES / "blah.py"), "reset", "link"])
 
 
 def test_simple_dag_run(tmp_wd: Path) -> None:
     __main__(["--recipe", str(RECIPES / "simple_dag.py"), "exec", "3-1"])
@@ -70,16 +89,22 @@
 def test_bad_recipe(caplog: pytest.LogCaptureFixture) -> None:
     with pytest.raises(SystemExit), caplog.at_level("ERROR"):
         __main__(["--recipe", str(RECIPES / "bad.py"), "exec", "false"])
     assert "failed to execute" in caplog.text
 
 
 def test_custom_formatter() -> None:
+    try:
+        raise ValueError("terrible error")
+    except ValueError:
+        exc_info = sys.exc_info()
     formatter = Formatter()
-    record = logging.LogRecord("a", logging.ERROR, "b", 2, "foo", None, None)
-    assert isinstance(formatter.format(record), str)
+    record = logging.LogRecord("a", logging.ERROR, "b", 2, "foo", None, exc_info=exc_info)
+    formatted = formatter.format(record)
+    assert isinstance(formatted, str)
+    assert "terrible error" in formatted
 
 
 def test_terrible_recipe(caplog: pytest.LogCaptureFixture) -> None:
     with pytest.raises(SystemExit), caplog.at_level("CRITICAL"):
         __main__(["--recipe", str(RECIPES / "terrible.not-py"), "ls"])
     assert "failed to load recipe" in caplog.text
```

### Comparing `cook-build-0.4.0/tests/test_manager.py` & `cook-build-0.4.1/tests/test_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from cook import Manager
 from cook.contexts import create_group, normalize_dependencies
 from cook.util import CookError
+import logging
 from pathlib import Path
 import pytest
 
 
 def test_resolve_dependencies(m: Manager) -> None:
     Path("input1.txt").write_text("input1.txt")
     Path("input2.txt").write_text("input2.txt")
@@ -42,14 +43,31 @@
 def test_conflicting_targets(m: Manager) -> None:
     m.create_task("foo", targets=["bar"])
     m.create_task("baz", targets=["bar"])
     with pytest.raises(ValueError, match="both have target"):
         m.resolve_dependencies()
 
 
+def test_symlink_targets(m: Manager, caplog: pytest.LogCaptureFixture, tmp_wd: Path) -> None:
+    file2 = Path("file2")
+    file1 = Path("file1")
+    m.create_task("task1", targets=[file1])
+    m.create_task("task2", targets=[file2])
+    file2.symlink_to("file3")
+
+    with caplog.at_level(logging.WARNING):
+        m.resolve_dependencies()
+    assert "is a symlink" in caplog.messages[0]
+
+    file2.unlink()
+    file2.symlink_to(file1)
+    with pytest.raises(ValueError, match="both have target"):
+        m.resolve_dependencies()
+
+
 def test_same_name(m: Manager) -> None:
     m.create_task("foo")
     with pytest.raises(ValueError, match="task with name 'foo' already exists"):
         m.create_task("foo")
 
 
 def test_get_manager_instance() -> None:
```

### Comparing `cook-build-0.4.0/tests/test_util.py` & `cook-build-0.4.1/tests/test_util.py`

 * *Files identical despite different names*

