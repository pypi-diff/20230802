# Comparing `tmp/aws-step-functions-pydantic-0.0.3.tar.gz` & `tmp/aws-step-functions-pydantic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-step-functions-pydantic-0.0.3.tar", last modified: Tue Aug  1 15:29:10 2023, max compression
+gzip compressed data, was "aws-step-functions-pydantic-0.0.4.tar", last modified: Wed Aug  2 11:18:32 2023, max compression
```

## Comparing `aws-step-functions-pydantic-0.0.3.tar` & `aws-step-functions-pydantic-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/.github/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3226 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.github/CONTRIBUTING.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/.github/workflows/
--rw-rw-r--   0 louis     (1000) louis     (1000)     3587 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.github/workflows/master.yml
--rw-rw-r--   0 louis     (1000) louis     (1000)      203 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.gitignore
--rw-rw-r--   0 louis     (1000) louis     (1000)      749 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 louis     (1000) louis     (1000)      327 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/.readthedocs.yml
--rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)     2899 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     1692 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)      187 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/codecov.yml
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/codegen/
--rwxrwxr-x   0 louis     (1000) louis     (1000)     1060 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/codegen/generate_pydantic_models.sh
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/docs/
--rw-rw-r--   0 louis     (1000) louis     (1000)      634 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/Makefile
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.445027 aws-step-functions-pydantic-0.0.3/docs/_static/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/docs/_static/css/
--rw-rw-r--   0 louis     (1000) louis     (1000)       70 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/_static/css/style.css
--rw-rw-r--   0 louis     (1000) louis     (1000)      122 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/api.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)     3799 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/conf.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      485 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/index.rst
--rw-rw-r--   0 louis     (1000) louis     (1000)      795 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/docs/make.bat
--rw-rw-r--   0 louis     (1000) louis     (1000)      354 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/mypy.ini
--rw-rw-r--   0 louis     (1000) louis     (1000)      355 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/pyproject.toml
--rw-rw-r--   0 louis     (1000) louis     (1000)       25 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/requirements-generate.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       19 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     3155 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/setup.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.445027 aws-step-functions-pydantic-0.0.3/src/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/
--rw-rw-r--   0 louis     (1000) louis     (1000)      471 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/__init__.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/
--rw-rw-r--   0 louis     (1000) louis     (1000)       58 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      510 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/define.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      916 2023-08-01 15:28:39.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/sfn.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)    10298 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/base_state_machine.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/utils/
--rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/utils/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/utils/boto.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     2899 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)     1056 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      227 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       17 2023-08-01 15:29:10.000000 aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/tests/
--rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tests/__init__.py
--rw-rw-r--   0 louis     (1000) louis     (1000)      108 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tests/core_test.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.445027 aws-step-functions-pydantic-0.0.3/tools/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-01 15:29:10.449027 aws-step-functions-pydantic-0.0.3/tools/github/
--rw-rw-r--   0 louis     (1000) louis     (1000)      353 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tools/github/install_miniconda.sh
--rw-rw-r--   0 louis     (1000) louis     (1000)     1194 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.3/tox.ini
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.548659 aws-step-functions-pydantic-0.0.4/.github/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3226 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/.github/CONTRIBUTING.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.548659 aws-step-functions-pydantic-0.0.4/.github/workflows/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3566 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/.github/workflows/master.yml
+-rw-rw-r--   0 louis     (1000) louis     (1000)      203 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/.gitignore
+-rw-rw-r--   0 louis     (1000) louis     (1000)      755 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 louis     (1000) louis     (1000)      327 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/.readthedocs.yml
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2653 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1446 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)      187 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/codecov.yml
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.548659 aws-step-functions-pydantic-0.0.4/codegen/
+-rwxrwxr-x   0 louis     (1000) louis     (1000)     1060 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/codegen/generate_pydantic_models.sh
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/docs/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      634 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/docs/Makefile
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.548659 aws-step-functions-pydantic-0.0.4/docs/_static/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/docs/_static/css/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       70 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/docs/_static/css/style.css
+-rw-rw-r--   0 louis     (1000) louis     (1000)      121 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/docs/api.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3799 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/docs/conf.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      485 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/docs/index.rst
+-rw-rw-r--   0 louis     (1000) louis     (1000)      795 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/docs/make.bat
+-rw-rw-r--   0 louis     (1000) louis     (1000)      354 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/mypy.ini
+-rw-rw-r--   0 louis     (1000) louis     (1000)      355 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/pyproject.toml
+-rw-rw-r--   0 louis     (1000) louis     (1000)       25 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/requirements-generate.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       19 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.4/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3155 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.4/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.548659 aws-step-functions-pydantic-0.0.4/src/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      471 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/__init__.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/api/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       58 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/api/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      510 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/api/define.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      916 2023-08-01 15:28:39.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/api/sfn.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/generated/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/generated/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)    10298 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/generated/base_state_machine.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/utils/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       51 2023-08-01 15:21:20.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/utils/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      127 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/utils/boto.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     2653 2023-08-02 11:18:32.000000 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1056 2023-08-02 11:18:32.000000 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-02 11:18:32.000000 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-08-02 11:18:32.000000 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      227 2023-08-02 11:18:32.000000 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       17 2023-08-02 11:18:32.000000 aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/tests/
+-rw-rw-r--   0 louis     (1000) louis     (1000)        0 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/tests/__init__.py
+-rw-rw-r--   0 louis     (1000) louis     (1000)      126 2023-08-02 11:17:53.000000 aws-step-functions-pydantic-0.0.4/tests/core_test.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.548659 aws-step-functions-pydantic-0.0.4/tools/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-08-02 11:18:32.552659 aws-step-functions-pydantic-0.0.4/tools/github/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      353 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/tools/github/install_miniconda.sh
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1194 2023-08-01 12:42:25.000000 aws-step-functions-pydantic-0.0.4/tox.ini
```

### Comparing `aws-step-functions-pydantic-0.0.3/.github/CONTRIBUTING.md` & `aws-step-functions-pydantic-0.0.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/.github/workflows/master.yml` & `aws-step-functions-pydantic-0.0.4/.github/workflows/master.yml`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
           python -m coverage xml
         if: "contains(env.USING_COVERAGE, matrix.python-version)"
         continue-on-error: true
       - name: Upload coverage to Codecov
         if: "contains(env.USING_COVERAGE, matrix.python-version)"
         uses: "codecov/codecov-action@v1"
         with:
-          fail_ci_if_error: true
+          fail_ci_if_error: false
 
   package:
     name: "Build & verify package"
     runs-on: "ubuntu-20.04"
 
     defaults:
       run:
@@ -120,8 +120,8 @@
       - name: "Install in dev mode"
         run: |
           echo "CONDA=$CONDA"
           echo "python=$(which python)"
           echo "conda=$(which conda)"
           python -m pip install -e .[dev]
       - name: "Import package"
-        run: "python -c 'import aws_step_functions_pydantic; print(aws_step_functions_pydantic)'"
+        run: "python -c 'import aws_sfn_pydantic; print(aws_sfn_pydantic)'"
```

### Comparing `aws-step-functions-pydantic-0.0.3/.pre-commit-config.yaml` & `aws-step-functions-pydantic-0.0.4/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ---
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         language_version: python3.10
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.9.2
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.1.0
     hooks:
       - id: flake8
-        args: ["--max-line-length=88", "--extend-ignore=E203,E501"]
+        args: ["--max-line-length=88", "--extend-ignore=E203,E501,F722"]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude: ^data/
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: check-ast
```

### Comparing `aws-step-functions-pydantic-0.0.3/LICENSE` & `aws-step-functions-pydantic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/PKG-INFO` & `aws-step-functions-pydantic-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-step-functions-pydantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydantic models for AWS step functions
 Home-page: https://github.com/lmmx/aws-step-functions-pydantic
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
@@ -27,24 +27,21 @@
 Provides-Extra: boto3
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
 
 # aws-step-functions-pydantic
 
-[![Documentation](https://readthedocs.org/projects/aws-step-functions-pydantic/badge/?version=latest)](https://aws-step-functions-pydantic.readthedocs.io/en/latest/)
 [![CI Status](https://github.com/lmmx/aws-step-functions-pydantic/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/aws-step-functions-pydantic/actions/workflows/master.yml)
 [![Coverage](https://codecov.io/gh/lmmx/aws-step-functions-pydantic/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/aws-step-functions-pydantic)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Pydantic models for AWS step functions
 
-[Read The Docs](https://aws-step-functions-pydantic.readthedocs.io/en/latest/)
-
 ## Usage
 
 ### From Step Function ARN
 
 Use the `from_arn()` class constructor
 
 ```py
```

### Comparing `aws-step-functions-pydantic-0.0.3/README.md` & `aws-step-functions-pydantic-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # aws-step-functions-pydantic
 
-[![Documentation](https://readthedocs.org/projects/aws-step-functions-pydantic/badge/?version=latest)](https://aws-step-functions-pydantic.readthedocs.io/en/latest/)
 [![CI Status](https://github.com/lmmx/aws-step-functions-pydantic/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/aws-step-functions-pydantic/actions/workflows/master.yml)
 [![Coverage](https://codecov.io/gh/lmmx/aws-step-functions-pydantic/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/aws-step-functions-pydantic)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Pydantic models for AWS step functions
 
-[Read The Docs](https://aws-step-functions-pydantic.readthedocs.io/en/latest/)
-
 ## Usage
 
 ### From Step Function ARN
 
 Use the `from_arn()` class constructor
 
 ```py
```

### Comparing `aws-step-functions-pydantic-0.0.3/codegen/generate_pydantic_models.sh` & `aws-step-functions-pydantic-0.0.4/codegen/generate_pydantic_models.sh`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/docs/Makefile` & `aws-step-functions-pydantic-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/docs/conf.py` & `aws-step-functions-pydantic-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/docs/make.bat` & `aws-step-functions-pydantic-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/setup.py` & `aws-step-functions-pydantic-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/api/sfn.py` & `aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/api/sfn.py`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/src/aws_sfn_pydantic/generated/base_state_machine.py` & `aws-step-functions-pydantic-0.0.4/src/aws_sfn_pydantic/generated/base_state_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,43 +62,43 @@
     TimestampLessThanEquals: Optional[str] = None
     TimestampLessThanEqualsPath: Optional[AslPath] = None
     IsTimestamp: Optional[bool] = None
 
 
 class Fail(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Fail']
+    Type: Literal["Fail"]
     Comment: Optional[str] = None
     Cause: Optional[str] = None
     Error: Optional[str] = None
 
 
 class Errors(RootModel):
     root: Union[
         str,
-        Literal['States.ALL'],
-        Literal['States.HeartbeatTimeout'],
-        Literal['States.Timeout'],
-        Literal['States.TaskFailed'],
-        Literal['States.Permissions'],
-        Literal['States.ResultPathMatchFailure'],
-        Literal['States.ParameterPathFailure'],
-        Literal['States.BranchFailed'],
-        Literal['States.NoChoiceMatched'],
-        Literal['States.IntrinsicFailure'],
-    ] = Field(..., description='https://states-language.net/#appendix-a')
+        Literal["States.ALL"],
+        Literal["States.HeartbeatTimeout"],
+        Literal["States.Timeout"],
+        Literal["States.TaskFailed"],
+        Literal["States.Permissions"],
+        Literal["States.ResultPathMatchFailure"],
+        Literal["States.ParameterPathFailure"],
+        Literal["States.BranchFailed"],
+        Literal["States.NoChoiceMatched"],
+        Literal["States.IntrinsicFailure"],
+    ] = Field(..., description="https://states-language.net/#appendix-a")
 
 
 class Succeed(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Succeed']
+    Type: Literal["Succeed"]
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
 
 
 class ResourceItem(BaseModel):
     Ref: Optional[str] = None
@@ -115,64 +115,64 @@
     ErrorEquals: List[Errors]
     Next: str
     ResultPath: Optional[AslRefPath] = None
 
 
 class Wait(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Wait']
+    Type: Literal["Wait"]
     Next: Optional[str] = None
     End: Optional[Literal[True]] = None
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
     Seconds: Optional[confloat(ge=0.0)] = None
     Timestamp: Optional[str] = None
     SecondsPath: Optional[AslRefPath] = None
     TimestampPath: Optional[AslRefPath] = None
 
 
 class ReaderConfig(BaseModel):
     model_config = ConfigDict(
-        extra='allow',
+        extra="allow",
     )
     MaxItems: Optional[conint(ge=1)] = None
     MaxItemsPath: Optional[AslRefPath] = None
 
 
 class ProcessorConfigItem(BaseModel):
-    Mode: Literal['INLINE']
+    Mode: Literal["INLINE"]
 
 
 class ExecutionType(Enum):
-    EXPRESS = 'EXPRESS'
-    STANDARD = 'STANDARD'
+    EXPRESS = "EXPRESS"
+    STANDARD = "STANDARD"
 
 
 class ProcessorConfigItem1(BaseModel):
-    Mode: Literal['DISTRIBUTED']
+    Mode: Literal["DISTRIBUTED"]
     ExecutionType: ExecutionType
 
 
 class CatchItem2(BaseModel):
     ErrorEquals: List[Errors]
     Next: str
 
 
 class Choice1(Operator):
     Next: str
 
 
 class Choice(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Choice']
+    Type: Literal["Choice"]
     Next: Optional[str] = None
     End: Optional[Literal[True]] = None
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
     Choices: List[Choice1]
     Default: Optional[str] = None
@@ -183,26 +183,26 @@
     Next: str
     ResultPath: Optional[AslRefPath] = None
 
 
 class Model(BaseModel):
     Comment: Optional[str] = None
     StartAt: str
-    States: Dict[constr(pattern=r'^.{1,80}$'), State]
+    States: Dict[constr(pattern=r"^.{1,80}$"), State]
 
 
 class State(RootModel):
     root: Union[Choice, Fail, Parallel, Pass, Succeed, Task, Wait, Map]
 
 
 class FieldPayloadTemplateObject(RootModel):
     root: Union[
-        Dict[constr(pattern=r'^.+\.\$$'), str],
+        Dict[constr(pattern=r"^.+\.\$$"), str],
         Dict[
-            constr(pattern=r'^.+(([^.][^$])|([^.][$]))$'),
+            constr(pattern=r"^.+(([^.][^$])|([^.][$]))$"),
             Union[
                 Optional[Union[float, bool, str]],
                 List[AslPayloadTemplate],
                 FieldPayloadTemplateObject,
             ],
         ],
     ]
@@ -212,17 +212,17 @@
     root: Union[
         FieldPayloadTemplateObject, List[AslPayloadTemplate], Union[str, bool, float]
     ]
 
 
 class Parallel(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Parallel']
+    Type: Literal["Parallel"]
     Parameters: Optional[AslPayloadTemplate] = None
     ResultSelector: Optional[AslPayloadTemplate] = None
     Next: Optional[str] = None
     End: Optional[Literal[True]] = None
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
@@ -230,49 +230,49 @@
     Branches: List[StateMachine]
     Retry: Optional[List[RetryItem]] = None
     Catch: Optional[List[CatchItem]] = None
 
 
 class StateMachine(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
     Comment: Optional[str] = None
     StartAt: str
-    States: Dict[constr(pattern=r'^.{1,80}$'), State]
+    States: Dict[constr(pattern=r"^.{1,80}$"), State]
     Version: Optional[str] = None
     TimeoutSeconds: Optional[conint(ge=0)] = None
 
 
 class Pass(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Pass']
+    Type: Literal["Pass"]
     Next: Optional[str] = None
     End: Optional[Literal[True]] = None
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
     ResultPath: Optional[AslRefPath] = None
     Parameters: Optional[AslPayloadTemplate] = None
     Result: Optional[Any] = None
 
 
 class Task(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Task']
+    Type: Literal["Task"]
     Next: Optional[str] = None
     End: Optional[Literal[True]] = None
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
-    Resource: Union[str, constr(pattern=r'^\$\{[^\}]+\}$'), ResourceItem]
+    Resource: Union[str, constr(pattern=r"^\$\{[^\}]+\}$"), ResourceItem]
     ResultPath: Optional[AslRefPath] = None
     Retry: Optional[List[RetryItem]] = None
     Catch: Optional[List[CatchItem1]] = None
     TimeoutSeconds: Optional[confloat(ge=1.0)] = None
     TimeoutSecondsPath: Optional[AslRefPath] = None
     HeartbeatSeconds: Optional[confloat(ge=1.0)] = None
     HeartbeatSecondsPath: Optional[AslRefPath] = None
@@ -293,17 +293,17 @@
     MaxInputBytesPerBatch: Optional[confloat(ge=0.0, le=262144.0)] = None
     MaxInputBytesPerBatchPath: Optional[AslRefPath] = None
     BatchInput: Optional[AslPayloadTemplate] = None
 
 
 class Map(BaseModel):
     model_config = ConfigDict(
-        extra='forbid',
+        extra="forbid",
     )
-    Type: Literal['Map']
+    Type: Literal["Map"]
     Next: Optional[str] = None
     End: Optional[Literal[True]] = None
     Comment: Optional[str] = None
     OutputPath: Optional[AslPath] = None
     InputPath: Optional[AslPath] = None
     ResultPath: Optional[AslRefPath] = None
     ItemsPath: Optional[AslRefPath] = None
```

### Comparing `aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/PKG-INFO` & `aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-step-functions-pydantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydantic models for AWS step functions
 Home-page: https://github.com/lmmx/aws-step-functions-pydantic
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
@@ -27,24 +27,21 @@
 Provides-Extra: boto3
 Provides-Extra: tests
 Provides-Extra: dev
 License-File: LICENSE
 
 # aws-step-functions-pydantic
 
-[![Documentation](https://readthedocs.org/projects/aws-step-functions-pydantic/badge/?version=latest)](https://aws-step-functions-pydantic.readthedocs.io/en/latest/)
 [![CI Status](https://github.com/lmmx/aws-step-functions-pydantic/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/aws-step-functions-pydantic/actions/workflows/master.yml)
 [![Coverage](https://codecov.io/gh/lmmx/aws-step-functions-pydantic/branch/master/graph/badge.svg)](https://codecov.io/github/lmmx/aws-step-functions-pydantic)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Pydantic models for AWS step functions
 
-[Read The Docs](https://aws-step-functions-pydantic.readthedocs.io/en/latest/)
-
 ## Usage
 
 ### From Step Function ARN
 
 Use the `from_arn()` class constructor
 
 ```py
```

### Comparing `aws-step-functions-pydantic-0.0.3/src/aws_step_functions_pydantic.egg-info/SOURCES.txt` & `aws-step-functions-pydantic-0.0.4/src/aws_step_functions_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-step-functions-pydantic-0.0.3/tox.ini` & `aws-step-functions-pydantic-0.0.4/tox.ini`

 * *Files identical despite different names*

