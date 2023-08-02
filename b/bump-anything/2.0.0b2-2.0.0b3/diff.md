# Comparing `tmp/bump-anything-2.0.0b2.tar.gz` & `tmp/bump-anything-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-anything-2.0.0b2.tar", last modified: Wed Aug  2 02:21:56 2023, max compression
+gzip compressed data, was "bump-anything-2.0.0b3.tar", last modified: Wed Aug  2 02:27:23 2023, max compression
```

## Comparing `bump-anything-2.0.0b2.tar` & `bump-anything-2.0.0b3.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/bump_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/file_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/git.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/bump_anything.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 02:21:56.317640 bump-anything-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:27:23.863576 bump-anything-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-08-02 02:27:23.863576 bump-anything-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:27:23.859576 bump-anything-2.0.0b3/bump_anything.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-08-02 02:27:23.000000 bump-anything-2.0.0b3/bump_anything.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-02 02:27:23.000000 bump-anything-2.0.0b3/bump_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:27:23.000000 bump-anything-2.0.0b3/bump_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 02:27:23.000000 bump-anything-2.0.0b3/bump_anything.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 02:27:23.000000 bump-anything-2.0.0b3/bump_anything.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 02:27:23.000000 bump-anything-2.0.0b3/bump_anything.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:27:23.859576 bump-anything-2.0.0b3/bumpanything/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/bumpanything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/bumpanything/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/bumpanything/file_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/bumpanything/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 02:27:23.863576 bump-anything-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:27:23.863576 bump-anything-2.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/tests/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-08-02 02:27:07.000000 bump-anything-2.0.0b3/tests/test_git.py
```

### Comparing `bump-anything-2.0.0b2/LICENSE.txt` & `bump-anything-2.0.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bump-anything-2.0.0b2/bump_anything/__main__.py` & `bump-anything-2.0.0b3/bumpanything/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,32 @@
 import os.path
 import re
 import sys
 from functools import partial
 
 import semver
 
-import bump_anything.git as git
-from bump_anything.file_result import FileResult
+import bumpanything.git as git
+from bumpanything.file_result import FileResult
 
 # The regular expression pattern used to match the version to be incremented
 # within any given file of any type
 VERSION_PATT = r"({key}\s*[=:]\s*([\"\']?)){value}(\3\s*)".format(
     key=r'(["\']?)version\2',
     value=r"(?P<version>\d+\.\d+\.\d+[a-z0-9\-\+\.]*)",
 )
 
-# The valid types of increments you could make to a semantic version
-INCREMENT_TYPES = {"major", "minor", "patch", "prerelease"}
+# The valid types of increments you could make to a semantic version, and the
+# functions they map to
+INCREMENT_TYPES = {
+    "major": semver.bump_major,
+    "minor": semver.bump_minor,
+    "patch": semver.bump_patch,
+    "prerelease": semver.bump_prerelease,
+}
 
 
 def get_auto_detectable_file_names():
     # Get the name of the project directory
     project_name = os.path.basename(os.getcwd())
     return (
         # If a Node project
@@ -40,22 +46,16 @@
         "pyproject.toml",
     )
 
 
 # Increment the major, minor, or patch part of the given version string and
 # return the incremented version
 def bump_version(version, version_specifier):
-    if version_specifier == "major":
-        return semver.bump_major(version)
-    elif version_specifier == "minor":
-        return semver.bump_minor(version)
-    elif version_specifier == "patch":
-        return semver.bump_patch(version)
-    elif version_specifier == "prerelease":
-        return semver.bump_prerelease(version)
+    if version_specifier in INCREMENT_TYPES.keys():
+        return INCREMENT_TYPES[version_specifier](version)
     else:
         # If we are not incrementing the version using one of the above
         # commands, we can assume the version specified is the explicit new
         # version to use
         return version_specifier
 
 
@@ -118,19 +118,39 @@
 
 
 def abort_if_version_mismatch(file_results):
     if len(set(result.new_version for result in file_results)) > 1:
         print(
             "Aborting commit because not all bumped versions are equal", file=sys.stderr
         )
+        sys.exit()
+
+
+def bump_version_for_files(file_paths, version_specifier):
+    file_results = []
+    for file_path in file_paths:
+        did_version_change, current_version, new_version = bump_version_for_file(
+            file_path=file_path, version_specifier=version_specifier
+        )
+        if did_version_change:
+            file_results.append(
+                FileResult(
+                    file_path=file_path,
+                    current_version=current_version,
+                    new_version=new_version,
+                )
+            )
+    return file_results
 
 
 def handle_git_operations(
     file_results, commit_message, tag_name=None, should_tag=False
 ):
+    if not git.is_in_git_repository():
+        return
     abort_if_version_mismatch(file_results)
     changed_result_paths = [result.file_path for result in file_results]
     git.add(changed_result_paths)
     print(f"Staging {', '.join(changed_result_paths)}")
     git.commit(commit_message)
     if not should_tag:
         return
@@ -139,15 +159,15 @@
         return
     print(f"Tagging commit as {tag_name}")
 
 
 def version_specifier(arg_value):
     # Strip out 'v' prefix if included in the version specifier
     arg_value = re.sub(r"^v", "", arg_value)
-    if arg_value in INCREMENT_TYPES or semver.Version.is_valid(arg_value):
+    if arg_value in INCREMENT_TYPES.keys() or semver.Version.is_valid(arg_value):
         return arg_value
     else:
         raise argparse.ArgumentTypeError(
             "invalid version specifier (must be a valid semantic version)"
         )
 
 
@@ -159,44 +179,32 @@
         metavar="file",
         nargs="*",
         type=os.path.expanduser,
         default=get_default_file_paths(),
     )
     parser.add_argument("--no-commit", "-n", action="store_true")
     parser.add_argument("--no-tag", action="store_true")
-    parser.add_argument("--commit-message", "-m")
-    parser.add_argument("--tag-name", "-t")
+    parser.add_argument(
+        "--commit-message", "-m", default="Prepare v{new_version} release"
+    )
+    parser.add_argument("--tag-name", "-t", default="v{new_version}")
     return parser.parse_args()
 
 
 def main():
     args = parse_cli_args()
-    did_any_version_change = False
-    file_results = []
-    for file_path in args.file_paths:
-        did_version_change, current_version, new_version = bump_version_for_file(
-            file_path=file_path, version_specifier=args.version_specifier
-        )
-        if did_version_change:
-            file_results.append(
-                FileResult(
-                    file_path=file_path,
-                    current_version=current_version,
-                    new_version=new_version,
-                )
-            )
-            did_any_version_change = True
-    if not did_any_version_change:
+    file_results = bump_version_for_files(args.file_paths, args.version_specifier)
+    if not file_results:
         print("No files updated")
         return
     if not args.no_commit:
         new_version = file_results[0].new_version
         handle_git_operations(
             file_results=file_results,
-            commit_message=args.commit_message or f"Prepare {new_version} release",
-            tag_name=args.tag_name or f"v{new_version}",
+            commit_message=args.commit_message.format(new_version=new_version),
+            tag_name=args.tag_name.format(new_version=new_version),
             should_tag=not args.no_tag,
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bump-anything-2.0.0b2/pyproject.toml` & `bump-anything-2.0.0b3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "bump-anything"
-version = "2.0.0-beta.2"
+version = "2.0.0-beta.3"
 description = "A CLI utility for bumping the version of any file type"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
-    { name = "Caleb Evans", email = "caleb@calebevans.me" }
+    {name = "Caleb Evans", email = "caleb@calebevans.me"}
 ]
 maintainers = [
     {name = 'Caleb Evans', email = 'caleb@calebevans.me'}
 ]
 license = {file = 'LICENSE.txt'}
 keywords = ["semver", "semantic", "version", "versioning", "bump", "increment"]
 dependencies=[
@@ -19,12 +19,30 @@
 [project.urls]
 homepage = "https://github.com/caleb531/bump-anything"
 documentation = "https://github.com/caleb531/bump-anything#readme"
 repository = "https://github.com/caleb531/bump-anything"
 changelog = "https://github.com/caleb531/bump-anything/releases"
 
 [project.scripts]
-bump = "bump_anything.__main__:main"
-bump-anything = "bump_anything.__main__:main"
+bump = "bumpanything.__main__:main"
+bump-anything = "bumpanything.__main__:main"
 
 [build-system]
 requires = ["setuptools", "wheel"]
+
+# Configuration for coverage.py (https://pypi.python.org/pypi/coverage)
+
+[tool.coverage.run]
+# Enable branch coverage
+branch = true
+
+[tool.coverage.report]
+# Regexes for lines to exclude from consideration
+exclude_lines = [
+    "pragma: no cover",
+    # Ignore non-runnable code
+    "if __name__ == .__main__.:",
+    "pass",
+]
+
+# Only check coverage for source files
+include = ["bumpanything/*.py"]
```

