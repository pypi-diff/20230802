# Comparing `tmp/bump-anything-1.0.4.tar.gz` & `tmp/bump-anything-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bump-anything-1.0.4.tar", last modified: Wed Feb 13 23:25:07 2019, max compression
+gzip compressed data, was "bump-anything-2.0.0b2.tar", last modified: Wed Aug  2 02:21:56 2023, max compression
```

## Comparing `bump-anything-1.0.4.tar` & `bump-anything-2.0.0b2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxr-xr-x   0 Caleb      (501) staff       (20)        0 2019-02-13 23:25:06.000000 bump-anything-1.0.4/
--rw-r--r--   0 Caleb      (501) staff       (20)     2118 2019-02-13 23:25:06.000000 bump-anything-1.0.4/PKG-INFO
--rw-r--r--   0 Caleb      (501) staff       (20)     1292 2019-02-10 23:49:22.000000 bump-anything-1.0.4/README.md
--rw-r--r--   0 Caleb      (501) staff       (20)     4296 2019-02-13 23:20:50.000000 bump-anything-1.0.4/bump.py
-drwxr-xr-x   0 Caleb      (501) staff       (20)        0 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/
--rw-r--r--   0 Caleb      (501) staff       (20)     2118 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/PKG-INFO
--rw-r--r--   0 Caleb      (501) staff       (20)      250 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/SOURCES.txt
--rw-r--r--   0 Caleb      (501) staff       (20)        1 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/dependency_links.txt
--rw-r--r--   0 Caleb      (501) staff       (20)       36 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/entry_points.txt
--rw-r--r--   0 Caleb      (501) staff       (20)       13 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/requires.txt
--rw-r--r--   0 Caleb      (501) staff       (20)        5 2019-02-13 23:25:06.000000 bump-anything-1.0.4/bump_anything.egg-info/top_level.txt
--rw-r--r--   0 Caleb      (501) staff       (20)       38 2019-02-13 23:25:06.000000 bump-anything-1.0.4/setup.cfg
--rw-r--r--   0 Caleb      (501) staff       (20)      892 2019-02-13 23:22:35.000000 bump-anything-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/bump_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/file_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/bump_anything/git.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:21:56.313640 bump-anything-2.0.0b2/bump_anything.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 02:21:56.000000 bump-anything-2.0.0b2/bump_anything.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 02:21:56.317640 bump-anything-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 02:21:41.000000 bump-anything-2.0.0b2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bump-anything-1.0.4/README.md` & `bump-anything-2.0.0b2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 # Bump Anything
 
-*Copyright 2019 Caleb Evans*  
+*Copyright 2019-2023 Caleb Evans*  
 *Released under the MIT license*
 
 Bump Anything is a command-line utility for incrementing the version  It serves
 as a more-flexible alternative to `npm version` and similar tools because
 Bump Anything can handle any arbitrary text file and has built-in support for
 different types of projects.
 
 ## Features
 
 - Bump the version number in any arbitrary file
-- Supports most project types (if no paths are supplied, automatically detects `package.json` in Node, `setup.py` in Python, WordPress themes, etc.)
+- Supports most project types (if no paths are supplied, automatically detects
+  `package.json` in Node, `setup.py` or `pyproject.toml` in Python, `style.css`
+  for WordPress themes, etc.)
 
 ## Installation
 
-Bump Anything requires Python 3.4 or newer to run, so please ensure you have it
+Bump Anything requires Python 3.9 or newer to run, so please ensure you have it
 installed.
 
 ```sh
 pip3 install bump-anything
 ```
 
 ## Usage
 
-Bump Anything exposes a `bump` command to your shell. The only required argument
-is a keyword indicating how you want to increment each version. It can be either
-`major`, `minor`, or `patch`.
+Bump Anything exposes to your shell a `bump-anything` command (also aliased to
+`bump`). The only required argument is a keyword indicating how you want to
+increment each version. It can be either `major`, `minor`, or `patch`.
 
 
-```
-bump major
+```sh
+bump major # 1.2.3 -> 2.0.0
 ```
 
-```
-bump minor
+```sh
+bump minor # 1.2.3 -> 1.3.0
 ```
 
+```sh
+bump patch # 1.2.3 -> 1.2.4
 ```
-bump patch
+
+```sh
+bump prerelease # 1.2.3-beta.1 -> 1.2.3-beta.2
 ```
 
 With this syntax, Bump Anything will do its best to find the relevant files to
 bump. However, Bump Anything can also accept an optional list of one or more
 file paths whose versions to bump. Only the first occurrence of the version
 field in each file will be updated.
 
 ```
-bump minor subdir/myfile1.txt subdir/myfile2.txt
+bump minor subdir/myfile1.json subdir/myfile2.toml
 ```
+
+## Auto-Detected Files
+
+- `package.json` (Node)
+- `package-lock.json` (Node)
+- `setup.py` (Python)
+- `pyproject.toml` (Python)
+- `style.css` (WordPress Theme)
+- `<cwd name>.php` (WordPress Plugin)
```

