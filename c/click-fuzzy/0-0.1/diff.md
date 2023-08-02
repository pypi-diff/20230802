# Comparing `tmp/click_fuzzy-0.tar.gz` & `tmp/click_fuzzy-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_fuzzy-0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "click_fuzzy-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `click_fuzzy-0.tar` & `click_fuzzy-0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0      171 2023-08-02 06:19:31.025111 click_fuzzy-0/.flake8
--rw-r--r--   0        0        0     1799 2023-08-02 06:19:31.025444 click_fuzzy-0/.gitignore
--rw-r--r--   0        0        0     5483 2023-08-02 06:20:06.656301 click_fuzzy-0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      626 2023-08-02 06:20:06.656500 click_fuzzy-0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1066 2023-08-02 06:20:06.656663 click_fuzzy-0/LICENSE
--rw-r--r--   0        0        0      492 2023-08-02 06:20:06.656817 click_fuzzy-0/README.md
--rw-r--r--   0        0        0      174 2023-08-02 06:20:06.656944 click_fuzzy-0/click_fuzzy/__init__.py
--rw-r--r--   0        0        0      131 2023-08-02 06:21:26.497203 click_fuzzy-0/click_fuzzy/__main__.py
--rw-r--r--   0        0        0      152 2023-08-02 06:19:31.025780 click_fuzzy-0/click_fuzzy/__version__.py
--rw-r--r--   0        0        0      507 2023-08-02 06:20:06.657246 click_fuzzy-0/makefile
--rw-r--r--   0        0        0      856 2023-08-02 06:20:06.657383 click_fuzzy-0/pyproject.toml
--rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 click_fuzzy-0/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-08-02 06:19:31.025111 click_fuzzy-0.1/.flake8
+-rw-r--r--   0        0        0     1818 2023-08-02 08:15:25.067426 click_fuzzy-0.1/.gitignore
+-rw-r--r--   0        0        0      405 2023-08-02 08:45:35.195780 click_fuzzy-0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5483 2023-08-02 06:20:06.656301 click_fuzzy-0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      626 2023-08-02 06:20:06.656500 click_fuzzy-0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1066 2023-08-02 06:20:06.656663 click_fuzzy-0.1/LICENSE
+-rw-r--r--   0        0        0      818 2023-08-02 08:25:00.951978 click_fuzzy-0.1/README.md
+-rw-r--r--   0        0        0      250 2023-08-02 08:15:50.446889 click_fuzzy-0.1/click_fuzzy/__init__.py
+-rw-r--r--   0        0        0      154 2023-08-02 08:45:35.202096 click_fuzzy-0.1/click_fuzzy/__version__.py
+-rw-r--r--   0        0        0     1784 2023-08-02 08:44:05.415223 click_fuzzy-0.1/click_fuzzy/core.py
+-rw-r--r--   0        0        0       90 2023-08-02 08:15:50.445502 click_fuzzy-0.1/click_fuzzy/tests/__init__.py
+-rw-r--r--   0        0        0     4089 2023-08-02 08:44:01.041472 click_fuzzy-0.1/click_fuzzy/tests/smoke.py
+-rw-r--r--   0        0        0      547 2023-08-02 08:16:53.978712 click_fuzzy-0.1/makefile
+-rw-r--r--   0        0        0      834 2023-08-02 08:29:00.507605 click_fuzzy-0.1/pyproject.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 click_fuzzy-0.1/PKG-INFO
```

### Comparing `click_fuzzy-0/.gitignore` & `click_fuzzy-0.1/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -97,14 +97,17 @@
 # Celery stuff
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
+# VSCode
+.vscode/
+
 # Environments
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
```

### Comparing `click_fuzzy-0/CODE_OF_CONDUCT.md` & `click_fuzzy-0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0/CONTRIBUTING.md` & `click_fuzzy-0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0/LICENSE` & `click_fuzzy-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0/pyproject.toml` & `click_fuzzy-0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 name = "click-fuzzy"
 readme = "README.md"
 authors = [
     {name="Amethyst Reese", email="amethyst@n7.gg"},
 ]
 license = {file="LICENSE"}
 dynamic = ["version", "description"]
-requires-python = ">=3.10"
-dependencies = []
+requires-python = ">=3.8"
+dependencies = [
+    "click >= 8",
+    "editdistance >= 0.6",
+]
 
 [project.optional-dependencies]
 dev = [
     "attribution==1.6.2",
     "black==23.3.0",
     "flake8==6.0.0",
     "flit==3.8.0",
     "mypy==1.2.0",
     "ufmt==2.0.1",
     "usort==1.0.6",
 ]
 
-[project.scripts]
-click-fuzzy = "click_fuzzy.__main__:main"
-
 [project.urls]
 Home = "https://github.com/amyreese/click-fuzzy"
 
 [tool.flit.sdist]
 exclude = [
     ".github/",
 ]
 
 [tool.attribution]
-name = "Click Fuzzy Commands"
+name = "Fuzzy Commands"
 package = "click_fuzzy"
 version_file = true
 ignored_authors = ["dependabot[bot]"]
 signed_tags = true
 
 [tool.mypy]
 strict = true
```

