# Comparing `tmp/changelog-parser-0.0.2.tar.gz` & `tmp/changelog-parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog-parser-0.0.2.tar", last modified: Mon Jul 31 16:42:35 2023, max compression
+gzip compressed data, was "changelog-parser-0.0.3.tar", last modified: Wed Aug  2 16:34:53 2023, max compression
```

## Comparing `changelog-parser-0.0.2.tar` & `changelog-parser-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/.github/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)      425 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.github/workflows/deploy.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      552 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1909 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/changelog_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7673 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/test/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/test/projects/example/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/test/projects/example/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.661889 changelog-parser-0.0.3/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.661889 changelog-parser-0.0.3/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.github/workflows/publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2371 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.github/workflows/pull_request_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/changelog_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 16:34:53.000000 changelog-parser-0.0.3/changelog_parser.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8846 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1205 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.661889 changelog-parser-0.0.3/test/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:53.665889 changelog-parser-0.0.3/test/projects/example/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/test/projects/example/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5078 2023-08-02 16:34:42.000000 changelog-parser-0.0.3/test/test_load.py
```

### Comparing `changelog-parser-0.0.2/.gitignore` & `changelog-parser-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.2/CHANGELOG.md` & `changelog-parser-0.0.3/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.0.2]
+## [0.0.3] - 2023-08-01
 
-### Changing
+### Fixed
+
+- Error message regarding version/data separation in titles
+
+## [0.0.2] - 2023-07-31
+
+### Changed
 
 - `*_no` ChangelogParsingError properties to `line_number` and `column_number`
 
-## [0.0.1]
+## [0.0.1] - 2023-07-28
 
 ### Fixed
 
 - Some links
 
-## [0.0.0]
+## [0.0.0] - 2023-07-28
 
 ### Added
 
 - Load function to convert a CHANGELOG.md to a python object
 - Error to specify line/column of parsing problems
 - Some basic testing
```

### Comparing `changelog-parser-0.0.2/LICENSE` & `changelog-parser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.2/Makefile` & `changelog-parser-0.0.3/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 VENV_LOCATION ?= venv
 
 $(VENV_LOCATION):
 	$(if $(filter 0,$(shell python3 --version >/dev/null 2>&1; echo $$?)),$\
-		python3 -m venv --clea $@,$\
+		python3 -m venv --clear $@,$\
 		$(if $(filter 0,$(shell python --version >/dev/null 2>&1; echo $$?)),$\
 			python -m venv --clear $@,$\
 			$(error Unable to determine a way to invoke python to create a venv)))
 
 .PHONY: install
 $(VENV_LOCATION)/bin/pytest: $(VENV_LOCATION)
 	$</bin/python -m pip install -e .[test]
 install-test: $(VENV_LOCATION)/bin/test-changelog;
 
 .PHONY: test
 test: $(VENV_LOCATION)/bin/pytest
 	$<
+
+cover: $(VENV_LOCATION)/bin/pytest
+	$(VENV_LOCATION)/bin/coverage run -m pytest -n auto
+	$(VENV_LOCATION)/bin/coverage html --directory $@
```

### Comparing `changelog-parser-0.0.2/PKG-INFO` & `changelog-parser-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Parses changelog files
 Author-email: Jason Stiefel <Jason.R.Stiefel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 JasonStiefel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,24 +62,24 @@
    ```js
    {
      "$schema": "https://json-schema.org/draft-07/schema#",
      "title": "Loaded Changelog",
      "type": "object",
      "properties": {
        "version": {
-         "OneOf": [ {
-           "const": "Unreleased",
-           "description": "Case Insensitive"
+         "oneOf": [ {
+           "type": "string",
+           "pattern": "^[Uu][Nn][Rr][Ee][Ll][Ee][Aa][Ss][Ee][Dd]$"
          }, {
            "type": "semver.Version",
            "description": "Python object from https://pypi.org/project/semver/"
          } ]
        },
        "date": {
-         "OneOf": [ {
+         "oneOf": [ {
            "const": null
          }, {
            "type": "datetime.date",
            "description": "Python object from https://docs.python.org/3/library/datetime.html#date-objects; parsed using \"fromisoformat\""
          } ]
        },
        "yanked": {
```

### Comparing `changelog-parser-0.0.2/README.md` & `changelog-parser-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,24 @@
    ```js
    {
      "$schema": "https://json-schema.org/draft-07/schema#",
      "title": "Loaded Changelog",
      "type": "object",
      "properties": {
        "version": {
-         "OneOf": [ {
-           "const": "Unreleased",
-           "description": "Case Insensitive"
+         "oneOf": [ {
+           "type": "string",
+           "pattern": "^[Uu][Nn][Rr][Ee][Ll][Ee][Aa][Ss][Ee][Dd]$"
          }, {
            "type": "semver.Version",
            "description": "Python object from https://pypi.org/project/semver/"
          } ]
        },
        "date": {
-         "OneOf": [ {
+         "oneOf": [ {
            "const": null
          }, {
            "type": "datetime.date",
            "description": "Python object from https://docs.python.org/3/library/datetime.html#date-objects; parsed using \"fromisoformat\""
          } ]
        },
        "yanked": {
```

### Comparing `changelog-parser-0.0.2/changelog_parser.egg-info/PKG-INFO` & `changelog-parser-0.0.3/changelog_parser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: Parses changelog files
 Author-email: Jason Stiefel <Jason.R.Stiefel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 JasonStiefel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,24 +62,24 @@
    ```js
    {
      "$schema": "https://json-schema.org/draft-07/schema#",
      "title": "Loaded Changelog",
      "type": "object",
      "properties": {
        "version": {
-         "OneOf": [ {
-           "const": "Unreleased",
-           "description": "Case Insensitive"
+         "oneOf": [ {
+           "type": "string",
+           "pattern": "^[Uu][Nn][Rr][Ee][Ll][Ee][Aa][Ss][Ee][Dd]$"
          }, {
            "type": "semver.Version",
            "description": "Python object from https://pypi.org/project/semver/"
          } ]
        },
        "date": {
-         "OneOf": [ {
+         "oneOf": [ {
            "const": null
          }, {
            "type": "datetime.date",
            "description": "Python object from https://docs.python.org/3/library/datetime.html#date-objects; parsed using \"fromisoformat\""
          } ]
        },
        "yanked": {
```

### Comparing `changelog-parser-0.0.2/pyproject.toml` & `changelog-parser-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,21 @@
 
 [tool.setuptools.dynamic]
 version = { attr = "changelog.__version__" }
 
 [project.optional-dependencies]
 test = [
   "pytest",
+  "coverage",
   "pytest-xdist"
 ]
 
 [tool.pytest.ini_options]
 log_cli_level = "info"
 testpaths = [ "test" ]
 
+[tool.coverage.run]
+branch = true
+source_pkgs = [ "changelog" ]
+
 [tool.setuptools.package-dir]
 changelog = "src"
```

### Comparing `changelog-parser-0.0.2/src/__init__.py` & `changelog-parser-0.0.3/src/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 # SPDX-License-Identifier: MIT
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 import re
 from datetime import date
 from semver import Version
 from typing import ( Optional, Any )
 from io import ( IOBase, StringIO )
 
-class ChangelogParsingError(Exception):
+class ChangelogParsingError( Exception ):
     @property
     def line_number( self )-> Optional[ int ]:
+        """
+        Parse the line number from the error message, if defined
+        """
         if ( match := re.search( r' \(at line (\d+)(?:, column \d+)?\)$', str( self ) ) ):
             return int( match.group( 1 ) )
 
     @property
     def column_number( self )-> Optional[ int ]:
+        """
+        Parse the column number from the error message, if defined
+        """
         if ( match := re.search( r' \(at (?:line \d+, )?column (\d+)\)$', str( self ) ) ):
             return int( match.group( 1 ) )
 
     def __init__( self, msg: str, line_number: Optional[ int ] = None, column_number: Optional[ int ] = None ):
         specifications = (
             *( ( f'line { line_number }', ) if isinstance( line_number, int ) else () ),
             *( ( f'column { column_number }', ) if isinstance( column_number, int ) else () )
         )
         super().__init__( msg + ( f' (at { ", ".join( specifications ) })' if specifications else '' ) )
 
-def load( fp: IOBase, encoding: str = 'utf-8' )-> dict[ str, Any ]:
+def load( fp: IOBase, encoding: str = 'utf-8' )-> list[ dict[ str, Any ] ]:
+    """
+    Parse changelog data from a stream
+
+    :param input: a stream that outputs changelog data (eg. a file opened for reading)
+    :param encoding: if the stream outputs binary data, decode it using this encoding
+    :return: a list of dictionaries with changelog data (see README.md for structure)
+    """
     line_no, changes, section, in_compare_urls = 0, [], None, False
 
     while ( line := fp.readline() ):
         line_no += 1
         if isinstance( line, bytes ):
             try:
                 line = line.decode( encoding )
@@ -67,14 +80,20 @@
                 changes[ -1 ][ "yanked" ] = False
 
             if line.rstrip() != line:
                 raise ChangelogParsingError( "Extra space(s) after date", line_no, len( line.rstrip() ) + 1 )
             line, sep, change_date = line.partition( ' - ' )
             if change_date.lstrip() != change_date:
                 raise ChangelogParsingError( "Extra space(s) before date", line_no, len( line + sep ) + 1 )
+            if "]" in line and not line.rstrip().endswith( "]" ):
+                raise ChangelogParsingError(
+                    msg = 'Version and date must be separated by " - "',
+                    line_number = line_no,
+                    column_number = line.find( "]" ) + 2
+                )
             if sep:
                 try:
                     changes[ -1 ][ "date" ] = date.fromisoformat( change_date )
                 except Exception as e:
                     raise ChangelogParsingError(
                         msg = f'Unable to parse changelog entry date, "{ change_date }"; { e }',
                         line_number = line_no,
@@ -110,20 +129,20 @@
             if section is not None and changes[ -1 ][ section ]:
                 changes[ -1 ][ section ][ -1 ] = changes[ -1 ][ section ][ -1 ].rstrip()
 
             line = line.removeprefix( '### ' )
             if line not in ( 'Added', 'Changed', 'Deprecated', 'Removed', 'Fixed', 'Security' ):
                 raise ChangelogParsingError( f'Invalid change type, "{ line }"', line_no, 5 )
             if line.lower() in changes[ -1 ]:
-                raise ChangelogParsingError( f'Multiple "{ line }" sections found', line_no, 4 )
+                raise ChangelogParsingError( f'Multiple "{ line }" sections found', line_no, 5 )
             changes[ -1 ][ ( section := line.lower() ) ] = []
 
         elif line.startswith( '- ' ) or line.startswith( '* ' ):
             if section is None:
-                raise ChangelogParsingError( 'Change not under a category section', line_no, 0 )
+                raise ChangelogParsingError( 'Change not under a category section', line_no )
             changes[ -1 ][ section ].append( line[ 2 : ] )
 
         elif ( line.startswith( "  " ) or not line ) and section is not None and changes[ -1 ][ section ]:
             changes[ -1 ][ section ][ -1 ] += "\n" + line.removeprefix( "  " )
 
         elif ( match := re.fullmatch( r'\[([^\]]+)\]: (https?:\/\/.*)', line ) ):
             if match.group( 1 ).lower() == "unreleased":
@@ -168,9 +187,26 @@
             raise ChangelogParsingError( f'Unrecognized line pattern, "{ line }"', line_no )
 
     if section is not None and changes[ -1 ][ section ]:
         changes[ -1 ][ section ][ -1 ] = changes[ -1 ][ section ][ -1 ].rstrip()
 
     return changes
 
-def loads( input: str ):
+def loads( input: str )-> list[ dict[ str, Any ] ]:
+    """
+    Parse data from a changelog provided as a string
+
+    :param input: the string parse as a changelog
+    :return: a list of dictionaries with changelog data (see README.md for structure)
+    """
     return load( StringIO( input ) )
+
+
+__all__ = [
+    '__version__',
+    'ChangelogParsingError',
+    'load',
+    'loads'
+]
+
+def __dir__() -> list[str]:
+    return __all__
```

### Comparing `changelog-parser-0.0.2/test/projects/example/CHANGELOG.md` & `changelog-parser-0.0.3/test/projects/example/CHANGELOG.md`

 * *Files identical despite different names*

