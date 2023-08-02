# Comparing `tmp/thipster-0.23.3.tar.gz` & `tmp/thipster-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.23.3.tar", last modified: Wed Jul 12 09:15:15 2023, max compression
+gzip compressed data, was "thipster-0.23.5.tar", last modified: Wed Aug  2 07:13:30 2023, max compression
```

## Comparing `thipster-0.23.3.tar` & `thipster-0.23.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-07-12 09:15:11.000000 thipster-0.23.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-12 09:15:11.000000 thipster-0.23.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5376 2023-07-12 09:15:15.130450 thipster-0.23.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4544 2023-07-12 09:15:11.000000 thipster-0.23.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-07-12 09:15:11.000000 thipster-0.23.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-12 09:15:11.000000 thipster-0.23.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 09:15:15.130450 thipster-0.23.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1848 2023-07-12 09:15:12.000000 thipster-0.23.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/engine/
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    18947 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_dslparser.py
--rw-r--r--   0 root         (0) root         (0)    14360 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     5314 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/test_parserfactory.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/parser/test_yamlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/tests/repository/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/test_github_repository.py
--rw-r--r--   0 root         (0) root         (0)     6375 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/test_local_repository.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/repository/test_resourcemodel.py
--rw-r--r--   0 root         (0) root         (0)     3525 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     8033 2023-07-12 09:15:11.000000 thipster-0.23.3/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6551 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6285 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4646 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13040 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     5311 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14699 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     3283 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    24598 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.130450 thipster-0.23.3/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26119 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-07-12 09:15:11.000000 thipster-0.23.3/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:15:15.126450 thipster-0.23.3/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1957 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-12 09:15:15.000000 thipster-0.23.3/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.013070 thipster-0.23.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 07:13:08.000000 thipster-0.23.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-02 07:13:08.000000 thipster-0.23.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-02 07:13:30.013070 thipster-0.23.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-02 07:13:08.000000 thipster-0.23.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-02 07:13:08.000000 thipster-0.23.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 07:13:08.000000 thipster-0.23.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:13:30.013070 thipster-0.23.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-02 07:13:09.000000 thipster-0.23.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.993069 thipster-0.23.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.993069 thipster-0.23.5/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/engine/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.993069 thipster-0.23.5/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.997069 thipster-0.23.5/tests/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18947 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/test_parsedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/test_parserfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/parser/test_yamlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.997069 thipster-0.23.5/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/test_github_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/test_local_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/repository/test_resourcemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-02 07:13:08.000000 thipster-0.23.5/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:29.997069 thipster-0.23.5/thipster/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.001069 thipster-0.23.5/thipster/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/auth/google.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.001069 thipster-0.23.5/thipster/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/i_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/parsed_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/engine/resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.005069 thipster-0.23.5/thipster/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.005069 thipster-0.23.5/thipster/parser/dsl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24598 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/parser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.009070 thipster-0.23.5/thipster/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/repository/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.013070 thipster-0.23.5/thipster/terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/terraform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26119 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/terraform/cdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-02 07:13:08.000000 thipster-0.23.5/thipster/terraform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:13:30.001069 thipster-0.23.5/thipster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 07:13:29.000000 thipster-0.23.5/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.23.3/LICENSE` & `thipster-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/PKG-INFO` & `thipster-0.23.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.3
+Version: 0.23.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.3 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.5 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.23.3/README.md` & `thipster-0.23.5/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/pyproject.toml` & `thipster-0.23.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,53 @@
 
 testpaths = [
     "tests",
     "integration",
 ]
 
 [tool.semantic_release]
-version_variable = "setup.py:__version__"
-branch = "main"
-commit_parser = "semantic_release.history.emoji_parser"
-
-major_emoji = ":boom:"
-minor_emoji = ":sparkles:"
-patch_emoji = ":ambulance:,:bug:,:adhesive_bandage:,:lock:,:arrow_up:,:arrow_down:,:heavy_plus_sign:,:heavy_minus_sign:,:rotating_light:,:zap:,:recycle:,:wrench:,:loud_sound:,:mute:,:goal_net:,:wastebasket:,:coffin:,:chart_with_upwards_trend:,:globe_with_meridians:,:alien:,:wheelchair:,:children_crossing:,:bricks:"
-
-repository_url = "https://upload.pypi.org/legacy/"
+version_variables = [
+    "setup.py:__version__"
+]
+commit_parser = "emoji"
 
-commit_subject = ":bookmark: {version} [skip ci]"
+commit_message = ":bookmark: {version} [skip ci]"
 major_on_zero = false
 
+[tool.semantic_release.commit_parser_options]
+major_tags = [":boom:"]
+minor_tags = [
+    ":sparkles:",
+]
+patch_tags = [
+    ":ambulance:",
+    ":bug:",
+    ":adhesive_bandage:",
+    ":lock:",
+    ":arrow_up:",
+    ":arrow_down:",
+    ":heavy_plus_sign:",
+    ":heavy_minus_sign:",
+    ":rotating_light:",
+    ":zap:",
+    ":recycle:",
+    ":wrench:",
+    ":loud_sound:",
+    ":mute:",
+    ":goal_net:",
+    ":wastebasket:",
+    ":coffin:",
+    ":chart_with_upwards_trend:",
+    ":globe_with_meridians:",
+    ":alien:",
+    ":wheelchair:",
+    ":children_crossing:",
+    ":bricks:",
+]
+
 [pytest]
 mock_use_standalone_module = true
 
 [tool.ruff]
 exclude = ["__init__.py"]
 select = [
     "F",
```

### Comparing `thipster-0.23.3/setup.py` & `thipster-0.23.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('requirements').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.23.3'
+__version__ = '0.23.5'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as rm:
     readme = rm.read()
```

### Comparing `thipster-0.23.3/tests/engine/test_engine.py` & `thipster-0.23.5/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/engine/test_generation.py` & `thipster-0.23.5/tests/engine/test_generation.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/dsl_parser/test_ast.py` & `thipster-0.23.5/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/dsl_parser/test_dslparser.py` & `thipster-0.23.5/tests/parser/dsl_parser/test_dslparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.23.5/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/dsl_parser/test_token.py` & `thipster-0.23.5/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.23.5/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/test_parsedfile.py` & `thipster-0.23.5/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/test_parserfactory.py` & `thipster-0.23.5/tests/parser/test_parserfactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/parser/test_yamlparser.py` & `thipster-0.23.5/tests/parser/test_yamlparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/repository/test_github_repository.py` & `thipster-0.23.5/tests/repository/test_github_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/repository/test_local_repository.py` & `thipster-0.23.5/tests/repository/test_local_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/repository/test_resourcemodel.py` & `thipster-0.23.5/tests/repository/test_resourcemodel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/test_e2e.py` & `thipster-0.23.5/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/tests/test_tools.py` & `thipster-0.23.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/auth/google.py` & `thipster-0.23.5/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/engine/engine.py` & `thipster-0.23.5/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/engine/i_parser.py` & `thipster-0.23.5/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/engine/i_repository.py` & `thipster-0.23.5/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/engine/i_terraform.py` & `thipster-0.23.5/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/engine/parsed_file.py` & `thipster-0.23.5/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/engine/resource_model.py` & `thipster-0.23.5/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/helpers.py` & `thipster-0.23.5/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/ast.py` & `thipster-0.23.5/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.23.5/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.23.5/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/lexer.py` & `thipster-0.23.5/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.23.5/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/parser.py` & `thipster-0.23.5/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/token.py` & `thipster-0.23.5/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.23.5/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/exceptions.py` & `thipster-0.23.5/thipster/parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/parser_factory.py` & `thipster-0.23.5/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/parser/yaml_parser.py` & `thipster-0.23.5/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/repository/exceptions.py` & `thipster-0.23.5/thipster/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/repository/github.py` & `thipster-0.23.5/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/repository/json.py` & `thipster-0.23.5/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/repository/local.py` & `thipster-0.23.5/thipster/repository/local.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/terraform/cdk.py` & `thipster-0.23.5/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster/terraform/exceptions.py` & `thipster-0.23.5/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.23.3/thipster.egg-info/PKG-INFO` & `thipster-0.23.5/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.23.3
+Version: 0.23.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.23.3 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.23.5 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.23.3/thipster.egg-info/SOURCES.txt` & `thipster-0.23.5/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

