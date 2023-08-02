# Comparing `tmp/flask-openapi3-2.4.0rc1.tar.gz` & `tmp/flask-openapi3-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-openapi3-2.4.0rc1.tar", last modified: Wed May 31 09:01:07 2023, max compression
+gzip compressed data, was "flask-openapi3-2.5.0.tar", last modified: Wed Aug  2 02:43:24 2023, max compression
```

## Comparing `flask-openapi3-2.4.0rc1.tar` & `flask-openapi3-2.5.0.tar`

### file list

```diff
@@ -1,75 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/api_blueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/api_view_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/async_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/custom_ui_templates_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/enum_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/header_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/image_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/init_oauth_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/just_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/nested_apiblueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/openapi_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/orjson_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/pydantic_custom_root_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/response_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/rest_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/servers_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/upload_file_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/models/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.884657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/swagger-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.892657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/swagger.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.892657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.886635 flask-openapi3-2.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/api_blueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/api_view_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/async_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/custom_ui_templates_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/enum_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/header_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/image_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/init_oauth_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/just_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/openapi_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/openapi_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/orjson_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/pydantic_custom_root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/response_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/rest_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/servers_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/examples/upload_file_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.886635 flask-openapi3-2.5.0/flask_openapi3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/oauth_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/oauth_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/parameter_in_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/security_scheme_in_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/server_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/style_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/models/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24248 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.882635 flask-openapi3-2.5.0/flask_openapi3/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/css/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.890635 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/apidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/rapidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/redoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/images/swagger.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/rapidoc-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/redoc.standalone.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/flask_openapi3/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:43:24.886635 flask-openapi3-2.5.0/flask_openapi3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 02:43:24.000000 flask-openapi3-2.5.0/flask_openapi3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 02:43:24.894635 flask-openapi3-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-02 02:43:16.000000 flask-openapi3-2.5.0/setup.py
```

### Comparing `flask-openapi3-2.4.0rc1/CHANGELOG.md` & `flask-openapi3-2.5.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,28 @@
-## v2.4.0 2023-??-??
+## v2.5.0 2023-08-02
+
+- [#79](https://github.com/luolingchun/flask-openapi3/discussions/79) Support `by_alias` in Model Config. Thanks, @candleindark.
+- [#82](https://github.com/luolingchun/flask-openapi3/issues/82) Fix parameter in url_prefix. Thanks, @riedgar-ms.
+- [#83](https://github.com/luolingchun/flask-openapi3/pull/83) Be able to change 422 validation errors to other http response status. Thanks, @CostcoFanboy.
+- [#86](https://github.com/luolingchun/flask-openapi3/issues/86) Responses key supports both string, int, and HTTPStatus. Thanks, @CostcoFanboy.
+
+## v2.4.0 2023-06-04
 
 - [#72](https://github.com/luolingchun/flask-openapi3/pull/72) security_schemes(SecurityScheme) supports a json format.
 - [#68](https://github.com/luolingchun/flask-openapi3/pull/68) feat: Add operation_id_callback. Thanks, @BoyanYK.
-- Add DeprecationWarning to APIKey, HTTPBase, OAuth2, OpenIdConnect, HTTPBearer that will be deprecated in v3.0.
+- [#64](https://github.com/luolingchun/flask-openapi3/pull/64) Explains the usage of flask openapi command more clearly. Thanks, @candleindark.
+- [#75](https://github.com/luolingchun/flask-openapi3/pull/75) Init view_class and pass view_kwargs. Thanks, @stufisher.
+- [#70](https://github.com/luolingchun/flask-openapi3/issues/70) Support for Specification Extensions in OpenAPI Object and Operation Object. Thanks, @simonblund.
+- [#73](https://github.com/luolingchun/flask-openapi3/issues/73) BaseModel Config support openapi_extra.
+- Merge `extra_responses` to `responses` and deprecate `extra_responses`.
+
+**DeprecationWarning:**
+
+- Add DeprecationWarning to `APIKey`, `HTTPBase`, `OAuth2`, `OpenIdConnect`, `HTTPBearer` that will be deprecated in v3.0.
+- Add DeprecationWarning to `extra_form`, `extra_body` and `extra_responses` that will be deprecated in v3.0.
 
 
 ## v2.3.2 2023-04-03
 
 - [#61](https://github.com/luolingchun/flask-openapi3/issues/61) Fix headers with pydantic alias
 
 ## v2.3.1 2023-02-13
```

### Comparing `flask-openapi3-2.4.0rc1/CONTRIBUTING.md` & `flask-openapi3-2.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/LICENSE.rst` & `flask-openapi3-2.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/PKG-INFO` & `flask-openapi3-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.4.0rc1
+Version: 2.5.0
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,16 +34,16 @@
              width="60%" height="auto" alt="logo">
     </a>
 </div>
 <p align="center">
     <em>Generate REST API and OpenAPI documentation for your Flask project.</em>
 </p>
 <p align="center">
-    <a href="https://github.com/luolingchun/flask-openapi3/actions/workflows/test.yml" target="_blank">
-        <img class="off-glb" src="https://img.shields.io/github/actions/workflow/status/luolingchun/flask-openapi3/test.yml?branch=master" alt="test">
+    <a href="https://github.com/luolingchun/flask-openapi3/actions/workflows/tests.yml" target="_blank">
+        <img class="off-glb" src="https://img.shields.io/github/actions/workflow/status/luolingchun/flask-openapi3/tests.yml?branch=master" alt="test">
     </a>
     <a href="https://pypi.org/project/flask-openapi3/" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/v/flask-openapi3" alt="pypi">
     </a>
     <a href="https://pypistats.org/packages/flask-openapi3" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/dm/flask-openapi3" alt="pypistats">
     </a>
```

### Comparing `flask-openapi3-2.4.0rc1/README.md` & `flask-openapi3-2.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
              width="60%" height="auto" alt="logo">
     </a>
 </div>
 <p align="center">
     <em>Generate REST API and OpenAPI documentation for your Flask project.</em>
 </p>
 <p align="center">
-    <a href="https://github.com/luolingchun/flask-openapi3/actions/workflows/test.yml" target="_blank">
-        <img class="off-glb" src="https://img.shields.io/github/actions/workflow/status/luolingchun/flask-openapi3/test.yml?branch=master" alt="test">
+    <a href="https://github.com/luolingchun/flask-openapi3/actions/workflows/tests.yml" target="_blank">
+        <img class="off-glb" src="https://img.shields.io/github/actions/workflow/status/luolingchun/flask-openapi3/tests.yml?branch=master" alt="test">
     </a>
     <a href="https://pypi.org/project/flask-openapi3/" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/v/flask-openapi3" alt="pypi">
     </a>
     <a href="https://pypistats.org/packages/flask-openapi3" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/dm/flask-openapi3" alt="pypistats">
     </a>
```

### Comparing `flask-openapi3-2.4.0rc1/examples/api_blueprint_demo.py` & `flask-openapi3-2.5.0/examples/api_blueprint_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 @api.get('/book', doc_ui=False)
 def get_book():
     return {"code": 0, "message": "ok"}
 
 
-@api.post('/book', extra_responses={"200": {"content": {"text/csv": {"schema": {"type": "string"}}}}})
+@api.post('/book', responses={200: {"content": {"text/csv": {"schema": {"type": "string"}}}}})
 def create_book(body: BookBody):
     assert body.age == 3
     return {"code": 0, "message": "ok"}
 
 
 @api.put('/book/<int:bid>', operation_id='update')
 def update_book(path: Path, body: BookBody):
```

### Comparing `flask-openapi3-2.4.0rc1/examples/api_view_demo.py` & `flask-openapi3-2.5.0/examples/api_view_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/async_demo.py` & `flask-openapi3-2.5.0/examples/async_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/custom_ui_templates_demo.py` & `flask-openapi3-2.5.0/examples/custom_ui_templates_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/enum_demo.py` & `flask-openapi3-2.5.0/examples/enum_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/header_demo.py` & `flask-openapi3-2.5.0/examples/header_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/init_oauth_demo.py` & `flask-openapi3-2.5.0/examples/init_oauth_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/nested_apiblueprint_demo.py` & `flask-openapi3-2.5.0/examples/nested_apiblueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/openapi_extensions.py` & `flask-openapi3-2.5.0/examples/openapi_extensions.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/orjson_demo.py` & `flask-openapi3-2.5.0/examples/orjson_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/pydantic_custom_root_types.py` & `flask-openapi3-2.5.0/examples/pydantic_custom_root_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 class SelloutDict3(BaseModel):
     class Config:
         extra: Extra = Extra.allow
 
 
 @app.post('/api/v1/sellouts',
           tags=[Tag(name='Sellout', description='Loren.')],
-          responses={'200': SelloutList}
+          responses={200: SelloutList}
           )
 def post_sellout(body: SelloutList):
     print(body)
     return body.json()
 
 
 @app.post('/api/v2/sellouts',
           tags=[Tag(name='Sellout', description='Loren.')],
-          responses={'200': SelloutDict}
+          responses={200: SelloutDict}
           )
 def post_sellout2(body: SelloutDict):
     print(body)
     return body.json()
 
 
 @app.post('/api/v3/sellouts',
```

### Comparing `flask-openapi3-2.4.0rc1/examples/response_demo.py` & `flask-openapi3-2.5.0/examples/response_demo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 # -*- coding: utf-8 -*-
-# @Author  : [martinatseequent](https://github.com/martinatseequent)
+# @Author  : llc
 # @Time    : 2021/6/22 9:32
 
 import json
 from http import HTTPStatus
 
 from flask import make_response
 from pydantic import BaseModel, Field
 
 from flask_openapi3 import Info
 from flask_openapi3 import OpenAPI, APIBlueprint
 
-app = OpenAPI(__name__, info=Info(title="Hello API", version="1.0.0"), )
+app = OpenAPI(__name__, info=Info(title="Hello API", version="1.0.0"))
 
 bp = APIBlueprint("Hello BP", __name__)
 
 
 class HelloPath(BaseModel):
     name: str = Field(..., description="The name")
 
 
 class Message(BaseModel):
     message: str = Field(..., description="The message")
 
+    class Config:
+        openapi_extra = {
+            # "example": {"message": "aaa"},
+            "examples": {
+                "example1": {
+                    "summary": "example1 summary",
+                    "value": {
+                        "message": "bbb"
+                    }
+                },
+                "example2": {
+                    "summary": "example2 summary",
+                    "value": {
+                        "message": "ccc"
+                    }
+                }
+            }
+        }
 
-@bp.get("/hello/<string:name>", responses={"200": Message})
+
+@bp.get("/hello/<string:name>",
+        responses={HTTPStatus.OK: Message, "201": {"content": {"text/csv": {"schema": {"type": "string"}}}}})
 def hello(path: HelloPath):
     message = {"message": f"""Hello {path.name}!"""}
 
     response = make_response(json.dumps(message), HTTPStatus.OK)
     # response = make_response("sss", HTTPStatus.OK)
     response.mimetype = "application/json"
     return response
 
 
-@bp.get("/hello_no_response/<string:name>", responses={"204": None})
+@bp.get("/hello_no_response/<string:name>", responses={204: None})
 def hello_no_response(path: HelloPath):
     message = {"message": f"""Hello {path.name}!"""}
 
     # This message will never be returned because the http code (NO_CONTENT) doesn't return anything
     response = make_response(message, HTTPStatus.NO_CONTENT)
     response.mimetype = "application/json"
     return response
```

### Comparing `flask-openapi3-2.4.0rc1/examples/rest_demo.py` & `flask-openapi3-2.5.0/examples/rest_demo.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # @Author  : llc
 # @Time    : 2021/4/28 11:24
 from http import HTTPStatus
 from typing import Optional, List
 
 from pydantic import BaseModel, Field
 
-from flask_openapi3 import ExternalDocumentation, ExtraRequestBody, Example
+from flask_openapi3 import ExternalDocumentation
 from flask_openapi3 import Info, Tag, Server
 from flask_openapi3 import OpenAPI
 
 info = Info(title='book API', version='1.0.0')
 
 # Basic Authentication Sample
 basic = {
@@ -46,15 +46,15 @@
 
 
 class NotFoundResponse(BaseModel):
     code: int = Field(-1, description="Status Code")
     message: str = Field("Resource not found!", description="Exception Information")
 
 
-app = OpenAPI(__name__, info=info, security_schemes=security_schemes, responses={"404": NotFoundResponse})
+app = OpenAPI(__name__, info=info, security_schemes=security_schemes, responses={404: NotFoundResponse})
 
 book_tag = Tag(name='book', description='Some Book')
 security = [
     {"jwt": []},
     {"oauth2": ["write:pets", "read:pets"]},
     {"basic": []}
 ]
@@ -91,17 +91,15 @@
     tags=[book_tag],
     summary='new summary',
     description='new description',
     operation_id="get_book_id",
     external_docs=ExternalDocumentation(
         url="https://www.openapis.org/",
         description="Something great got better, get excited!"),
-
-    responses={"200": BookResponse},
-    extra_responses={"200": {"content": {"text/csv": {"schema": {"type": "string"}}}}},
+    responses={200: BookResponse},
     security=security,
     servers=[Server(url="https://www.openapis.org/", description="openapi")]
 )
 def get_book(path: BookPath):
     """Get a book
     to Get some book by id, like:
     http://localhost:5000/book/3
@@ -124,40 +122,15 @@
         "data": [
             {"bid": 1, "age": query.age, "author": 'a1'},
             {"bid": 2, "age": query.age, "author": 'a2'}
         ]
     }
 
 
-extra_body = ExtraRequestBody(
-    description="This is post RequestBody",
-    required=True,
-    example="ttt",
-    examples={
-        "example1": Example(
-            summary="example summary1",
-            description="example description1",
-            value={
-                "age": 24,
-                "author": "author1"
-            }
-        ),
-        "example2": Example(
-            summary="example summary2",
-            description="example description2",
-            value={
-                "age": 48,
-                "author": "author2"
-            }
-        )
-    }
-)
-
-
-@app.post('/book', tags=[book_tag], responses={"200": BookResponse}, extra_body=extra_body)
+@app.post('/book', tags=[book_tag], responses={200: BookResponse})
 def create_book(body: BookBody):
     print(body)
     return {"code": 0, "message": "ok"}, HTTPStatus.OK
 
 
 @app.put('/book/<int:bid>', tags=[book_tag])
 def update_book(path: BookPath, body: BookBody):
```

### Comparing `flask-openapi3-2.4.0rc1/examples/servers_demo.py` & `flask-openapi3-2.5.0/examples/servers_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/simple_demo.py` & `flask-openapi3-2.5.0/examples/simple_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/examples/upload_file_demo.py` & `flask-openapi3-2.5.0/examples/upload_file_demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # @Author  : llc
 # @Time    : 2021/5/11 14:03
 
 from typing import List
 
 from pydantic import BaseModel, Field
 
-from flask_openapi3 import OpenAPI, FileStorage, ExtraRequestBody
-from flask_openapi3 import Encoding
+from flask_openapi3 import OpenAPI, FileStorage
 
 app = OpenAPI(__name__)
 
 
 class UploadFileForm(BaseModel):
     file: FileStorage
     file_type: str = Field(None, description="File Type")
@@ -19,31 +18,23 @@
 
 class UploadFilesForm(BaseModel):
     files: List[FileStorage]
     str_list: List[str]
     int_list: List[int]
 
 
-extra_form = ExtraRequestBody(
-    description="This is form RequestBody",
-    required=True,
-    # replace style (default to form)
-    encoding={"str_list": Encoding(style="simple")}
-)
-
-
 @app.post('/upload/file')
 def upload_file(form: UploadFileForm):
     print(form.file.filename)
     print(form.file_type)
     form.file.save('test.jpg')
     return {"code": 0, "message": "ok"}
 
 
-@app.post('/upload/files', extra_form=extra_form)
+@app.post('/upload/files')
 def upload_files(form: UploadFilesForm):
     print(form.files)
     print(form.str_list)
     print(form.int_list)
     return {"code": 0, "message": "ok"}
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/blueprint.py` & `flask-openapi3-2.5.0/flask_openapi3/blueprint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,179 +1,199 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2022/4/1 16:54
-import re
 from copy import deepcopy
-from typing import Optional, List, Dict, Any, Type, Callable, Tuple
+from typing import Optional, List, Dict, Any, Callable
 
 from flask import Blueprint
-from pydantic import BaseModel
 
-from .http import HTTPMethod
-from .models import Tag, ExternalDocumentation
-from .models.common import ExtraRequestBody
-from .models.server import Server
+from ._http import HTTPMethod
+from .models import ExternalDocumentation
+from .models import ExtraRequestBody
+from .models import Server
+from .models import Tag
 from .scaffold import APIScaffold
-from .utils import get_operation, get_responses, parse_and_store_tags, parse_parameters, parse_method, \
-    get_operation_id_for_path
+from .types import ParametersTuple
+from .types import ResponseDict
+from .utils import convert_responses_key_to_string
+from .utils import get_operation
+from .utils import get_operation_id_for_path
+from .utils import get_responses
+from .utils import parse_and_store_tags
+from .utils import parse_method
+from .utils import parse_parameters
+from .utils import parse_rule
 
 
 class APIBlueprint(APIScaffold, Blueprint):
     def __init__(
             self,
             name: str,
             import_name: str,
             *,
             abp_tags: Optional[List[Tag]] = None,
             abp_security: Optional[List[Dict[str, List[str]]]] = None,
-            abp_responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            abp_responses: Optional[ResponseDict] = None,
             doc_ui: bool = True,
             operation_id_callback: Callable = get_operation_id_for_path,
             **kwargs: Any
     ) -> None:
         """
         Based on Flask Blueprint
 
         Arguments:
             name: The name of the blueprint. It Will be prepared to each endpoint name.
-            import_name: The name of the blueprint package, usually
-                         ``__name__``. This helps locate the ``root_path`` for the blueprint.
-            abp_tags: APIBlueprint tags for every api
-            abp_security: APIBlueprint security for every api
-            abp_responses: APIBlueprint response model
-            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            import_name: The name of the blueprint package, usually ``__name__``.
+                         This helps locate the ``root_path`` for the blueprint.
+            abp_tags: APIBlueprint tags for every API.
+            abp_security: APIBlueprint security for every API.
+            abp_responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            doc_ui: Enable OpenAPI document UI (Swagger UI, Redoc, and Rapidoc). Defaults to True.
             operation_id_callback: Callback function for custom operation_id generation.
-                Receives name (str), path (str) and method (str) parameters.
-                Defaults to `get_operation_id_for_path` from utils
+                                   Receives name (str), path (str) and method (str) parameters.
+                                   Defaults to `get_operation_id_for_path` from utils
             **kwargs: Flask Blueprint kwargs
         """
         super(APIBlueprint, self).__init__(name, import_name, **kwargs)
+
+        # Initialize instance variables
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.tags: List[Tag] = []
         self.tag_names: List[str] = []
 
+        # Set values from arguments or default values
         self.abp_tags = abp_tags or []
         self.abp_security = abp_security or []
-        self.abp_responses = abp_responses or {}
+
+        abp_responses = abp_responses or {}
+        # Convert key to string
+        self.abp_responses = convert_responses_key_to_string(abp_responses)
+
         self.doc_ui = doc_ui
+
+        # Set the operation ID callback function
         self.operation_id_callback: Callable = operation_id_callback
 
     def register_api(self, api: "APIBlueprint") -> None:
         """Register a nested APIBlueprint"""
+
+        # Check if the APIBlueprint is being registered on itself
         if api is self:
             raise ValueError("Cannot register a api blueprint on itself")
 
+        # Merge tags from the nested APIBlueprint
         for tag in api.tags:
             if tag.name not in self.tag_names:
                 self.tags.append(tag)
 
+        # Merge paths from the nested APIBlueprint
         for path_url, path_item in api.paths.items():
-            trail_slash = path_url.endswith("/")
-            # merge url_prefix and new api blueprint path url
-            uri = self.url_prefix.rstrip("/") + "/" + path_url.lstrip("/") if self.url_prefix else path_url
-            # strip the right slash
-            if not trail_slash:
-                uri = uri.rstrip("/")
+            # Parse rule: merge url_prefix and format rule from /pet/<petId> to /pet/{petId}
+            uri = parse_rule(path_url, url_prefix=self.url_prefix)
+
             self.paths[uri] = path_item
 
+        # Merge component schemas from the nested APIBlueprint
         self.components_schemas.update(**api.components_schemas)
 
+        # Register the nested APIBlueprint as a blueprint
         self.register_blueprint(api)
 
     def _do_decorator(
             self,
             rule: str,
             func: Callable,
             *,
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, Dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
-    ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
+    ) -> ParametersTuple:
         """
-        Collect openapi specification information
+        Collects OpenAPI specification information for Flask routes and view functions.
+
         Arguments:
             rule: Flask route
             func: Flask view_func
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
         if self.doc_ui is True and doc_ui is True:
             if responses is None:
-                responses = {}
+                new_responses = {}
+            else:
+                # Convert key to string
+                new_responses = convert_responses_key_to_string(responses)
             if extra_responses is None:
                 extra_responses = {}
-            # global response combine api responses
+            # Global response: combine API responses
             combine_responses = deepcopy(self.abp_responses)
-            combine_responses.update(**responses)
-            # create operation
+            combine_responses.update(**new_responses)
+            # Create operation
             operation = get_operation(
                 func,
                 summary=summary,
                 description=description,
                 openapi_extensions=openapi_extensions
             )
-            # set external docs
+            # Set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
             operation.operationId = operation_id or self.operation_id_callback(
                 name=func.__name__, path=rule, method=method
             )
-            # only set `deprecated` if True otherwise leave it as None
+            # Only set `deprecated` if True, otherwise leave it as None
             operation.deprecated = deprecated
-            # add security
+            # Add security
             if security is None:
                 security = []
             operation.security = security + self.abp_security or None
-            # add servers
+            # Add servers
             operation.servers = servers
-            # store tags
+            # Store tags
             tags = tags + self.abp_tags if tags else self.abp_tags
             parse_and_store_tags(tags, self.tags, self.tag_names, operation)
-            # parse parameters
+            # Parse parameters
             header, cookie, path, query, form, body = parse_parameters(
                 func,
                 extra_form=extra_form,
                 extra_body=extra_body,
                 components_schemas=self.components_schemas,
                 operation=operation
             )
-            # parse response
+            # Parse response
             get_responses(combine_responses, extra_responses, self.components_schemas, operation)
-            # /pet/<petId> --> /pet/{petId}
-            uri = re.sub(r"<([^<:]+:)?", "{", rule).replace(">", "}")
-            trail_slash = uri.endswith("/")
-            # merge url_prefix and uri
-            uri = self.url_prefix.rstrip("/") + "/" + uri.lstrip("/") if self.url_prefix else uri
-            if not trail_slash:
-                uri = uri.rstrip("/")
-            # parse method
+
+            # Parse rule: merge url_prefix and format rule from /pet/<petId> to /pet/{petId}
+            uri = parse_rule(rule, url_prefix=self.url_prefix)
+
+            # Parse method
             parse_method(uri, method, self.paths, operation)
             return header, cookie, path, query, form, body
         else:
-            # parse parameters
+            # Parse parameters
             header, cookie, path, query, form, body = parse_parameters(func, doc_ui=False)
             return header, cookie, path, query, form, body
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/commands.py` & `flask-openapi3-2.5.0/flask_openapi3/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,33 +6,39 @@
 from flask import current_app
 from flask.cli import click
 from flask.cli import with_appcontext
 
 from .markdown import openapi_to_markdown
 
 
-@click.command(name='openapi')
-@click.option('--output', '-o', type=click.Path(), help='The output file path.')
-@click.option('--format', '-f', type=click.Choice(['json', 'yaml', 'markdown']), help='The output file format.')
-@click.option('--indent', '-i', type=int, help='The indentation for JSON dumps.')
-@click.option('--ensure_ascii', '-a', is_flag=True, help='Ensure ASCII characters or not. Defaults to False.')
+@click.command(name="openapi")
+@click.option("--output", "-o", type=click.Path(), help="The output file path.")
+@click.option("--format", "-f", type=click.Choice(["json", "yaml", "markdown"]), help="The output file format.")
+@click.option("--indent", "-i", type=int, help="The indentation for JSON dumps.")
+@click.option("--ensure_ascii", "-a", is_flag=True, help="Ensure ASCII characters or not. Defaults to False.")
 @with_appcontext
 def openapi_command(output, format, indent, ensure_ascii):
     """Export the OpenAPI Specification to console or a file"""
-    if hasattr(current_app, 'api_doc'):
+
+    # Check if the current app has an api_doc attribute
+    if hasattr(current_app, "api_doc"):
         obj = current_app.api_doc
-        if format == 'yaml':
+
+        # Generate the OpenAPI Specification based on the specified format
+        if format == "yaml":
             try:
                 import yaml  # type: ignore
             except ImportError:
                 raise ImportError("pyyaml must be installed.")
             openapi = yaml.safe_dump(obj, allow_unicode=True)
-        elif format == 'markdown':
+        elif format == "markdown":
             openapi = openapi_to_markdown(obj)
         else:
             openapi = json.dumps(obj, indent=indent, ensure_ascii=ensure_ascii)
+
+        # Save the OpenAPI Specification to a file if the output path is provided
         if output:
-            with open(output, 'w', encoding='utf8') as f:
+            with open(output, "w", encoding="utf8") as f:
                 f.write(openapi)
             click.echo(f"Saved to {output}.")
         else:
             click.echo(openapi)
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/markdown.py` & `flask-openapi3-2.5.0/flask_openapi3/markdown.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/models/component.py` & `flask-openapi3-2.5.0/flask_openapi3/models/components.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
-# @Time    : 2021/4/30 11:45
-from typing import Optional, Dict, Union, Any
+# @Time    : 2023/7/4 9:36
+from typing import Dict, Optional, Union, Any
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
-from .common import Schema, Reference, Example, Header
-from .path import Response, Parameter, RequestBody, Link, PathItem
-from .security import SecurityScheme
+from .callback import Callback
+from .example import Example
+from .header import Header
+from .link import Link
+from .parameter import Parameter
+from .path_item import PathItem
+from .reference import Reference
+from .request_body import RequestBody
+from .response import Response
+from .schema import Schema
+from .security_scheme import SecurityScheme
 
 
 class Components(BaseModel):
-    """https://spec.openapis.org/oas/v3.0.3#components-object"""
-    schemas: Optional[Dict[str, Union[Schema, Reference]]] = None
+    """
+    https://spec.openapis.org/oas/v3.0.3#components-object
+    """
+
+    schemas: Optional[Dict[str, Union[Reference, Schema]]] = Field(None)
     responses: Optional[Dict[str, Union[Response, Reference]]] = None
     parameters: Optional[Dict[str, Union[Parameter, Reference]]] = None
     examples: Optional[Dict[str, Union[Example, Reference]]] = None
     requestBodies: Optional[Dict[str, Union[RequestBody, Reference]]] = None
     headers: Optional[Dict[str, Union[Header, Reference]]] = None
     securitySchemes: Optional[Dict[str, Union[SecurityScheme, Dict[str, Any]]]] = None
     links: Optional[Dict[str, Union[Link, Reference]]] = None
-    callbacks: Optional[Dict[str, Union[Dict[str, PathItem], Reference, Any]]] = None
+    callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
+    pathItems: Optional[Dict[str, Union[PathItem, Reference]]] = None
 
     class Config:
         extra = "allow"
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/models/file.py` & `flask-openapi3-2.5.0/flask_openapi3/models/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,18 +16,12 @@
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
-        field_schema.update(
-            format="binary",
-            type="string"
-        )
+        field_schema.update(format="binary", type="string")
 
     @classmethod
-    def validate(cls, value: Any) -> '_FileStorage':
-        if not isinstance(value, _FileStorage):
-            raise TypeError('werkzeug.datastructures.FileStorage required')
-
+    def validate(cls, value: Any) -> "_FileStorage":
         return value
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/models/info.py` & `flask-openapi3-2.5.0/flask_openapi3/models/info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2021/4/28 10:58
 from typing import Optional
 
 from pydantic import BaseModel
 
-
-class Contact(BaseModel):
-    name: Optional[str] = None
-    url: Optional[str] = None
-    email: Optional[str] = None
-
-    class Config:
-        extra = "allow"
-
-
-class License(BaseModel):
-    name: str
-    url: Optional[str] = None
-
-    class Config:
-        extra = "allow"
+from .contact import Contact
+from .license import License
 
 
 class Info(BaseModel):
-    """https://spec.openapis.org/oas/v3.0.3#info-object"""
+    """
+    https://spec.openapis.org/oas/v3.0.3#info-object
+    """
+
     title: str
+    summary: Optional[str] = None
     description: Optional[str] = None
     termsOfService: Optional[str] = None
     contact: Optional[Contact] = None
     license: Optional[License] = None
     version: str
 
     class Config:
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/models/oauth.py` & `flask-openapi3-2.5.0/flask_openapi3/models/link.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
-# @Time    : 2021/11/12 14:14
-
-
-from typing import Dict, Optional
+# @Time    : 2023/7/4 9:45
+from typing import Any, Dict, Optional
 
 from pydantic import BaseModel
 
+from .server import Server
+
 
-class OAuthConfig(BaseModel):
+class Link(BaseModel):
     """
-    More information go to: https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/oauth2.md
+    https://spec.openapis.org/oas/v3.0.3#link-object
     """
-    clientId: Optional[str] = None
-    clientSecret: Optional[str] = None
-    realm: Optional[str] = None
-    appName: Optional[str] = None
-    scopeSeparator: Optional[str] = None
-    scopes: Optional[str] = None
-    additionalQueryStringParams: Optional[Dict[str, str]] = None
-    useBasicAuthenticationWithAccessCodeGrant: Optional[bool] = False
-    usePkceWithAuthorizationCodeGrant: Optional[bool] = False
+
+    operationRef: Optional[str] = None
+    operationId: Optional[str] = None
+    parameters: Optional[Dict[str, Any]] = None
+    requestBody: Optional[Any] = None
+    description: Optional[str] = None
+    server: Optional[Server] = None
+
+    class Config:
+        extra = "allow"
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/models/security.py` & `flask-openapi3-2.5.0/flask_openapi3/models/security.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/models/validation_error.py` & `flask-openapi3-2.5.0/flask_openapi3/models/validation_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 # @Author  : llc
 # @Time    : 2021/5/10 14:51
 from typing import List, Dict, Any, Optional
 
 from pydantic import BaseModel, Field
 
 
-class UnprocessableEntity(BaseModel):
-    # More information: https://pydantic-docs.helpmanual.io/usage/models/#error-handling
+class ValidationErrorModel(BaseModel):
+    # More information: https://docs.pydantic.dev/1.10/usage/models/#error-handling
     loc: Optional[List[str]] = Field(None, title="Location", description="the error's location as a list. ")
     msg: Optional[str] = Field(None, title="Message", description="a computer-readable identifier of the error type.")
     type_: Optional[str] = Field(None, title="Error Type", description="a human readable explanation of the error.")
     ctx: Optional[Dict[str, Any]] = Field(
         None,
         title="Error context",
         description="an optional object which contains values required to render the error message."
     )
+
+
+# backward compatibility
+UnprocessableEntity = ValidationErrorModel
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/scaffold.py` & `flask-openapi3-2.5.0/flask_openapi3/scaffold.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2022/8/30 9:40
 import functools
 import inspect
 import sys
+import warnings
 from abc import ABC
 from functools import wraps
-from typing import Callable, List, Optional, Dict, Type, Any, Tuple
+from typing import Callable, List, Optional, Dict, Any
 
 from flask.scaffold import Scaffold
-from flask.wrappers import Response
-from pydantic import BaseModel
+from flask.wrappers import Response as FlaskResponse
 
-from .http import HTTPMethod
+from ._http import HTTPMethod
 from .models import ExternalDocumentation
-from .models.common import ExtraRequestBody
-from .models.server import Server
-from .models.tag import Tag
+from .models import ExtraRequestBody
+from .models import Server
+from .models import Tag
 from .request import _do_request
+from .types import ParametersTuple
+from .types import ResponseDict
 
 if sys.version_info >= (3, 8):
     iscoroutinefunction = inspect.iscoroutinefunction
 else:
     def iscoroutinefunction(func: Any) -> bool:
         while inspect.ismethod(func):
             func = func.__func__
 
         while isinstance(func, functools.partial):
             func = func.func
 
         return inspect.iscoroutinefunction(func)
 
+warnings.simplefilter("once")
+
 
 class APIScaffold(Scaffold, ABC):
     def _do_decorator(
             self,
             rule: str,
             func: Callable,
             *,
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
-    ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
+    ) -> ParametersTuple:
         raise NotImplementedError
 
     def register_api(self, api) -> None:
         raise NotImplementedError
 
     @staticmethod
     def create_view_func(
@@ -70,65 +74,61 @@
             body,
             view_class=None,
             view_kwargs=None
     ):
         is_coroutine_function = iscoroutinefunction(func)
         if is_coroutine_function:
             @wraps(func)
-            async def view_func(**kwargs) -> Response:
-                result = _do_request(
+            async def view_func(**kwargs) -> FlaskResponse:
+                func_kwargs = _do_request(
                     header=header,
                     cookie=cookie,
                     path=path,
                     query=query,
                     form=form,
                     body=body,
-                    **kwargs
+                    path_kwargs=kwargs
                 )
-                if isinstance(result, Response):
-                    # 422
-                    return result
+
                 # handle async request
                 if view_class:
                     signature = inspect.signature(view_class.__init__)
                     parameters = signature.parameters
                     if parameters.get("view_kwargs"):
                         view_object = view_class(view_kwargs=view_kwargs)
                     else:
                         view_object = view_class()
-                    response = await func(view_object, **result)
+                    response = await func(view_object, **func_kwargs)
                 else:
-                    response = await func(**result)
+                    response = await func(**func_kwargs)
                 return response
         else:
             @wraps(func)
-            def view_func(**kwargs) -> Response:
-                result = _do_request(
+            def view_func(**kwargs) -> FlaskResponse:
+                func_kwargs = _do_request(
                     header=header,
                     cookie=cookie,
                     path=path,
                     query=query,
                     form=form,
                     body=body,
-                    **kwargs
+                    path_kwargs=kwargs
                 )
-                if isinstance(result, Response):
-                    # 422
-                    return result
+
                 # handle request
                 if view_class:
                     signature = inspect.signature(view_class.__init__)
                     parameters = signature.parameters
                     if parameters.get("view_kwargs"):
                         view_object = view_class(view_kwargs=view_kwargs)
                     else:
                         view_object = view_class()
-                    response = func(view_object, **result)
+                    response = func(view_object, **func_kwargs)
                 else:
-                    response = func(**result)
+                    response = func(**func_kwargs)
                 return response
 
         if not hasattr(func, "view"):
             func.view = view_func
 
         return func.view
 
@@ -139,45 +139,58 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for rest api, like: app.route(methods=["GET"])
+        Decorator for defining a REST API endpoint with the HTTP GET method.
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
 
+        if extra_form is not None:
+            warnings.warn(
+                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_body is not None:
+            warnings.warn(
+                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_responses is not None:
+            warnings.warn(
+                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
+                DeprecationWarning)
+
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
                     summary=summary,
@@ -211,44 +224,56 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for rest api, like: app.route(methods=["POST"])
+        Decorator for defining a REST API endpoint with the HTTP POST method.
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
+        if extra_form is not None:
+            warnings.warn(
+                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_body is not None:
+            warnings.warn(
+                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_responses is not None:
+            warnings.warn(
+                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
+                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
@@ -283,44 +308,56 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for rest api, like: app.route(methods=["PUT"])
+        Decorator for defining a REST API endpoint with the HTTP PUT method.
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
+        if extra_form is not None:
+            warnings.warn(
+                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_body is not None:
+            warnings.warn(
+                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_responses is not None:
+            warnings.warn(
+                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
+                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
@@ -355,44 +392,56 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for rest api, like: app.route(methods=["DELETE"])
+        Decorator for defining a REST API endpoint with the HTTP DELETE method.
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
+        if extra_form is not None:
+            warnings.warn(
+                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_body is not None:
+            warnings.warn(
+                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_responses is not None:
+            warnings.warn(
+                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
+                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
@@ -427,44 +476,56 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
-        Decorator for rest api, like: app.route(methods=["PATCH"])
+        Decorator for defining a REST API endpoint with the HTTP PATCH method.
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
             rule: The URL rule string.
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
+        if extra_form is not None:
+            warnings.warn(
+                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_body is not None:
+            warnings.warn(
+                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_responses is not None:
+            warnings.warn(
+                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
+                DeprecationWarning)
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
                     tags=tags,
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/__init__.py` & `flask-openapi3-2.5.0/flask_openapi3/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/swagger-ui.css` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/apidoc.svg` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/apidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/rapidoc.svg` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/rapidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/redoc.svg` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/redoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/swagger.svg` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/rapidoc-min.js` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/rapidoc-min.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/redoc.standalone.js` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-bundle.js` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js` & `flask-openapi3-2.5.0/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/utils.py` & `flask-openapi3-2.5.0/flask_openapi3/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,196 +1,245 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2021/5/1 21:34
 
 import inspect
 import re
+from http import HTTPStatus
 from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional, Any
 
-from pydantic import BaseModel
-
-from .http import HTTP_STATUS, HTTPMethod
-from .models import OPENAPI3_REF_TEMPLATE, OPENAPI3_REF_PREFIX, Tag
-from .models.common import Schema, MediaType, Encoding, ExtraRequestBody
-from .models.path import Operation, RequestBody, PathItem, Response
-from .models.path import ParameterInType, Parameter
-from .models.validation_error import UnprocessableEntity
+from flask import make_response, current_app
+from flask.wrappers import Response as FlaskResponse
+from pydantic import BaseModel, ValidationError
+
+from ._http import HTTP_STATUS, HTTPMethod
+from .models import Encoding
+from .models import ExtraRequestBody
+from .models import MediaType
+from .models import OPENAPI3_REF_PREFIX
+from .models import OPENAPI3_REF_TEMPLATE
+from .models import Operation
+from .models import Parameter
+from .models import ParameterInType
+from .models import PathItem
+from .models import RequestBody
+from .models import Response
+from .models import Schema
+from .models import Tag
+from .types import ParametersTuple
+from .types import ResponseDict
+from .types import ResponseStrKeyDict
 
 
 def get_operation(
         func: Callable, *,
         summary: Optional[str] = None,
         description: Optional[str] = None,
         openapi_extensions: Optional[Dict[str, Any]] = None,
 ) -> Operation:
-    """Return an Operation object with summary and description."""
+    """
+    Return an Operation object with the specified summary and description.
+
+    Arguments:
+        func: The function or method for which the operation is being defined.
+        summary: A short summary of what the operation does.
+        description: A verbose explanation of the operation behavior.
+        openapi_extensions: Additional extensions to the OpenAPI Schema.
+
+    Returns:
+        An Operation object representing the operation.
+
+    """
+    # Get the docstring of the function
     doc = inspect.getdoc(func) or ""
     doc = doc.strip()
     lines = doc.split("\n")
     doc_summary = lines[0] or None
+
+    # Determine the summary and description based on provided arguments or docstring
     if summary is None:
         doc_description = lines[0] if len(lines) == 0 else "</br>".join(lines[1:]) or None
     else:
         doc_description = "</br>".join(lines) or None
 
+    # Create the operation dictionary with summary and description
     operation_dict = dict(
         summary=summary or doc_summary,
         description=description or doc_description
     )
-    # update openapi_extensions
+
+    # Add any additional openapi_extensions to the operation dictionary
     openapi_extensions = openapi_extensions or {}
     operation_dict.update(**openapi_extensions)
 
+    # Create and return the Operation object
     operation = Operation(**operation_dict)
 
     return operation
 
 
 def get_operation_id_for_path(*, name: str, path: str, method: str) -> str:
+    """
+    Generate a unique operation ID based on the name, path, and method.
+
+    Arguments:
+        name: The name or identifier for the operation.
+        path: The URL path for the operation.
+        method: The HTTP method for the operation.
+
+    Returns:
+        A unique operation ID generated based on the provided name, path, and method.
+
+    """
     operation_id = name + path
+    # Replace non-word characters with underscores
     operation_id = re.sub(r"\W", "_", operation_id)
     operation_id = operation_id + "_" + method.lower()
     return operation_id
 
 
-def get_schema(obj: Type[BaseModel]) -> dict:
-    """Pydantic model conversion to openapi schema"""
-    assert inspect.isclass(obj) and issubclass(obj, BaseModel), \
-        f"{obj} is invalid `pydantic.BaseModel`"
+def get_model_schema(model: Type[BaseModel]) -> dict:
+    """Converts a Pydantic model to an OpenAPI schema."""
 
-    return obj.schema(ref_template=OPENAPI3_REF_TEMPLATE)
+    assert inspect.isclass(model) and issubclass(model, BaseModel), \
+        f"{model} is invalid `pydantic.BaseModel`"
+
+    model_config = model.Config
+    by_alias = getattr(model_config, "by_alias", True)
+
+    return model.schema(by_alias=by_alias, ref_template=OPENAPI3_REF_TEMPLATE)
 
 
 def parse_header(header: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parse header model"""
-    schema = get_schema(header)
+    """Parses a header model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(header)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
-            "in": ParameterInType.header,
+            "in": ParameterInType.HEADER,
             "description": value.get("description"),
             "required": name in schema.get("required", []),
             "schema": Schema(**value)
         }
-        # parse extra values
+        # Parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # parse definitions
+    # Parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_cookie(cookie: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parse cookie model"""
-    schema = get_schema(cookie)
+    """Parses a cookie model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(cookie)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
-            "in": ParameterInType.cookie,
+            "in": ParameterInType.COOKIE,
             "description": value.get("description"),
             "required": name in schema.get("required", []),
             "schema": Schema(**value)
         }
-        # parse extra values
+        # Parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # parse definitions
+    # Parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_path(path: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parse path model"""
-    schema = get_schema(path)
+    """Parses a path model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(path)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
-            "in": ParameterInType.path,
+            "in": ParameterInType.PATH,
             "description": value.get("description"),
             "required": True,
             "schema": Schema(**value)
         }
-        # parse extra values
+        # Parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # parse definitions
+    # Parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_query(query: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parse query model"""
-    schema = get_schema(query)
+    """Parses a query model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(query)
     parameters = []
     components_schemas: Dict = dict()
     properties = schema.get("properties", {})
 
     for name, value in properties.items():
         data = {
             "name": name,
-            "in": ParameterInType.query,
+            "in": ParameterInType.QUERY,
             "description": value.get("description"),
             "required": name in schema.get("required", []),
             "schema": Schema(**value)
         }
-        # parse extra values
+        # Parse extra values
         data.update(**value)
         parameters.append(Parameter(**data))
 
-    # parse definitions
+    # Parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return parameters, components_schemas
 
 
 def parse_form(
         form: Type[BaseModel],
         extra_form: Optional[ExtraRequestBody] = None,
 ) -> Tuple[Dict[str, MediaType], dict]:
-    """Parse form model"""
-    schema = get_schema(form)
+    """Parses a form model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(form)
     components_schemas = dict()
     properties = schema.get("properties", {})
 
     assert properties, f"{form.__name__}'s properties cannot be empty."
 
-    title = schema.get("title")
+    title = schema.get("title") or form.__name__
     components_schemas[title] = Schema(**schema)
     encoding = {}
     for k, v in properties.items():
         if v.get("type") == "array":
             encoding[k] = Encoding(style="form")
     if extra_form:
-        # update encoding
+        # Update encoding
         if extra_form.encoding:
             encoding.update(**extra_form.encoding)
         content = {
             "multipart/form-data": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
                 example=extra_form.example,
                 examples=extra_form.examples,
@@ -201,31 +250,31 @@
         content = {
             "multipart/form-data": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
                 encoding=encoding or None
             )
         }
 
-    # parse definitions
+    # Parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return content, components_schemas
 
 
 def parse_body(
         body: Type[BaseModel],
         extra_body: Optional[ExtraRequestBody] = None,
 ) -> Tuple[Dict[str, MediaType], dict]:
-    """Parse body model"""
-    schema = get_schema(body)
+    """Parses a body model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(body)
     components_schemas = dict()
 
-    title = schema.get("title")
+    title = schema.get("title") or body.__name__
     components_schemas[title] = Schema(**schema)
     if extra_body:
         content = {
             "application/json": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
                 example=extra_body.example,
                 examples=extra_body.examples,
@@ -235,85 +284,67 @@
     else:
         content = {
             "application/json": MediaType(
                 schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"})
             )
         }
 
-    # parse definitions
+    # Parse definitions
     definitions = schema.get("definitions", {})
     for name, value in definitions.items():
         components_schemas[name] = Schema(**value)
 
     return content, components_schemas
 
 
 def get_responses(
-        responses: dict,
+        responses: ResponseStrKeyDict,
         extra_responses: Dict[str, dict],
         components_schemas: dict,
         operation: Operation
 ) -> None:
-    """
-    :param responses: Dict[str, BaseModel]
-    :param extra_responses: Dict[str, dict]
-    :param components_schemas: `models.component.py` `Components.schemas`
-    :param operation: `models.path.py` Operation
-    """
-    if responses is None:
-        responses = {}
     _responses = {}
     _schemas = {}
-    if not responses.get("422"):
-        _responses["422"] = Response(
-            description=HTTP_STATUS["422"],
-            content={
-                "application/json": MediaType(
-                    **{
-                        "schema": Schema(
-                            **{
-                                "type": "array",
-                                "items": {"$ref": f"{OPENAPI3_REF_PREFIX}/{UnprocessableEntity.__name__}"}
-                            }
-                        )
-                    }
-                )
-            }
-        )
-        _schemas[UnprocessableEntity.__name__] = Schema(**UnprocessableEntity.schema())
+
     for key, response in responses.items():
-        # Verify that the response is a class and that class is a subclass of `pydantic.BaseModel`
-        if inspect.isclass(response) and issubclass(response, BaseModel):
-            schema = response.schema(ref_template=OPENAPI3_REF_TEMPLATE)
+        if response is None:
+            # If the response is None, it means HTTP status code "204" (No Content)
+            _responses[key] = Response(description=HTTP_STATUS.get(key, ""))
+        elif isinstance(response, dict):
+            _responses[key] = Response(**response)
+        else:
+            schema = get_model_schema(response)
             _responses[key] = Response(
                 description=HTTP_STATUS.get(key, ""),
                 content={
                     "application/json": MediaType(
-                        **{
-                            "schema": Schema(
-                                **{
-                                    "$ref": f"{OPENAPI3_REF_PREFIX}/{response.__name__}"
-                                }
-                            )
-                        }
-                    )
-                }
-            )
+                        schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{response.__name__}"})
+                    )})
+
+            model_config = response.Config
+            openapi_extra = getattr(model_config, "openapi_extra", None)
+            if openapi_extra is not None:
+                # Add additional information from model_config to the response
+                _responses[key].description = openapi_extra.get("description")
+                _responses[key].headers = openapi_extra.get("headers")
+                _responses[key].links = openapi_extra.get("links")
+                _content = _responses[key].content
+                if _content is not None:
+                    _content["application/json"].example = openapi_extra.get("example")
+                    _content["application/json"].examples = openapi_extra.get("examples")
+                    _content["application/json"].encoding = openapi_extra.get("encoding")
+                    _content.update(openapi_extra.get("content", {}))
+
             _schemas[response.__name__] = Schema(**schema)
             definitions = schema.get("definitions")
             if definitions:
+                # Add schema definitions to _schemas
                 for name, value in definitions.items():
                     _schemas[name] = Schema(**value)
-        # Verify that if the response is None, because http status code "204" means return "No Content"
-        elif response is None:
-            _responses[key] = Response(
-                description=HTTP_STATUS.get(key, ""),
-            )
-        else:
-            raise TypeError(f"{response} is invalid `pydantic.BaseModel`.")
+
     # handle extra_responses
     for key, value in extra_responses.items():
         # key "200" value {"content":{"text/csv":{"schema":{"type": "string"}}}}
         new_response = Response(
             # Best effort to ensure there is always a description
             description=value.pop("description", HTTP_STATUS.get(key, "")),
             **value
@@ -326,116 +357,170 @@
 
 def parse_and_store_tags(
         new_tags: List[Tag],
         old_tags: List[Tag],
         old_tag_names: List[str],
         operation: Operation
 ) -> None:
-    """Store tags
-    :param new_tags: api tag
-    :param old_tags: openapi doc tags
-    :param old_tag_names: openapi doc tag names
-    :param operation: `models.path.py` Operation
     """
-    if new_tags is None:
-        new_tags = []
+    Parses new tags, stores them in an old_tags list if they are not already present,
+    and updates the tags attribute of the operation object.
+
+    Arguments:
+        new_tags: A list of new Tag objects to be parsed and stored.
+        old_tags: The list of existing Tag objects.
+        old_tag_names: The list that names of existing tags.
+        operation: The operation object whose tag attribute needs to be updated.
+
+    Returns:
+        None
+    """
+    # Iterate over each tag in new_tags
     for tag in new_tags:
         if tag.name not in old_tag_names:
             old_tag_names.append(tag.name)
             old_tags.append(tag)
+
+    # Set the tags attribute of the operation object to a list of unique tag names from new_tags
+    # If the resulting list is empty, set it to None
     operation.tags = list(set([tag.name for tag in new_tags])) or None
 
 
 def parse_parameters(
         func: Callable,
         *,
         extra_form: Optional[ExtraRequestBody] = None,
         extra_body: Optional[ExtraRequestBody] = None,
         components_schemas: Optional[Dict] = None,
         operation: Optional[Operation] = None,
         doc_ui: bool = True,
-) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
+) -> ParametersTuple:
     """
-    :param func: Flask view func
-    :param extra_form: Extra information describing the request body(application/form).
-    :param extra_body: Extra information describing the request body(application/json).
-    :param components_schemas: `models.component.py` Components.schemas
-    :param operation: `models.path.py` Operation
-    :param doc_ui: add openapi document UI(swagger and redoc). Defaults to True.
+    Parses the parameters of a given function and returns the types for header, cookie, path,
+    query, form, and body parameters. Also populates the Operation object with the parsed parameters.
+
+    Arguments:
+        func: The function to parse the parameters from.
+        extra_form: Additional form data for the request body (default: None).
+        extra_body: Additional body data for the request body (default: None).
+        components_schemas: Dictionary to store the parsed components schemas (default: None).
+        operation: Operation object to populate with parsed parameters (default: None).
+        doc_ui: Flag indicating whether to return types for documentation UI (default: True).
+
+    Returns:
+        Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
+        The types for header, cookie, path, query, form, and body parameters respectively.
+
     """
-    annotations = get_type_hints(func)
+    # Get the type hints from the function
+    annotations: Dict[str, Type[BaseModel]] = get_type_hints(func)
+
+    # Get the types for header, cookie, path, query, form, and body parameters
     header = annotations.get("header")
     cookie = annotations.get("cookie")
     path = annotations.get("path")
     query = annotations.get("query")
     form = annotations.get("form")
     body = annotations.get("body")
+
+    # If doc_ui is False, return the types without further processing
     if doc_ui is False:
-        return header, cookie, path, query, form, body  # type: ignore
+        return header, cookie, path, query, form, body
+
     parameters = []
+
+    # If components_schemas is None, initialize it as an empty dictionary
     if components_schemas is None:
         components_schemas = dict()
+
+    # If operation is None, initialize it as an Operation object
     if operation is None:
         operation = Operation()
+
     if header:
         _parameters, _components_schemas = parse_header(header)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
+
     if cookie:
         _parameters, _components_schemas = parse_cookie(cookie)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
+
     if path:
-        # get args from a route path
         _parameters, _components_schemas = parse_path(path)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
+
     if query:
-        # get args from route query
         _parameters, _components_schemas = parse_query(query)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
+
     if form:
         _content, _components_schemas = parse_form(form, extra_form)
         components_schemas.update(**_components_schemas)
         if extra_form:
             request_body = RequestBody(
                 description=extra_form.description,
                 content=_content,
                 required=extra_form.required
             )
         else:
-            request_body = RequestBody(**{
-                "content": _content,
-            })
+            request_body = RequestBody(content=_content)
+        model_config = form.Config
+        openapi_extra = getattr(model_config, "openapi_extra", None)
+        if openapi_extra:
+            request_body.description = openapi_extra.get("description")
+            request_body.content["multipart/form-data"].example = openapi_extra.get("example")
+            request_body.content["multipart/form-data"].examples = openapi_extra.get("examples")
+            if openapi_extra.get("encoding"):
+                request_body.content["multipart/form-data"].encoding = openapi_extra.get("encoding")
         operation.requestBody = request_body
+
     if body:
         _content, _components_schemas = parse_body(body, extra_body)
         components_schemas.update(**_components_schemas)
         if extra_body:
             request_body = RequestBody(
                 description=extra_body.description,
                 content=_content,
                 required=extra_body.required
             )
         else:
             request_body = RequestBody(content=_content)
+        model_config = body.Config
+        openapi_extra = getattr(model_config, "openapi_extra", None)
+        if openapi_extra:
+            request_body.description = openapi_extra.get("description")
+            request_body.content["application/json"].example = openapi_extra.get("example")
+            request_body.content["application/json"].examples = openapi_extra.get("examples")
+            request_body.content["application/json"].encoding = openapi_extra.get("encoding")
         operation.requestBody = request_body
+
+    # Set the parsed parameters in the operation object
     operation.parameters = parameters if parameters else None
 
-    return header, cookie, path, query, form, body  # type: ignore
+    return header, cookie, path, query, form, body
 
 
 def parse_method(uri: str, method: str, paths: dict, operation: Operation) -> None:
     """
-    :param uri: api route path
-    :param method: get post put delete patch
-    :param paths: openapi doc paths
-    :param operation: `models.path.py` Operation
+    Parses the HTTP method and updates the corresponding PathItem object in the paths' dictionary.
+
+    Arguments:
+        uri: The URI of the API endpoint.
+        method: The HTTP method for the API endpoint.
+        paths: A dictionary containing the API paths and their corresponding PathItem objects.
+        operation: The Operation object to assign to the PathItem.
+
+    Returns:
+        None
     """
+    # Check the HTTP method and update the PathItem object in the path dictionary
     if method == HTTPMethod.GET:
         if not paths.get(uri):
             paths[uri] = PathItem(get=operation)
         else:
             paths[uri].get = operation
     elif method == HTTPMethod.POST:
         if not paths.get(uri):
@@ -453,7 +538,51 @@
         else:
             paths[uri].patch = operation
     elif method == HTTPMethod.DELETE:
         if not paths.get(uri):
             paths[uri] = PathItem(delete=operation)
         else:
             paths[uri].delete = operation
+
+
+def make_validation_error_response(e: ValidationError) -> FlaskResponse:
+    """
+    Create a Flask response for a validation error.
+
+    Args:
+        e: The ValidationError object containing the details of the error.
+
+    Returns:
+        FlaskResponse: A Flask Response object with the JSON representation of the error.
+    """
+    response = make_response(e.json())
+    response.headers["Content-Type"] = "application/json"
+    response.status_code = getattr(current_app, "validation_error_status", 422)
+    return response
+
+
+def parse_rule(rule: str, url_prefix=None) -> str:
+    trail_slash = rule.endswith("/")
+
+    # Merge url_prefix and uri
+    uri = url_prefix.rstrip("/") + "/" + rule.lstrip("/") if url_prefix else rule
+
+    if not trail_slash:
+        uri = uri.rstrip("/")
+
+    # Convert route parameter format from /pet/<petId> to /pet/{petId}
+    uri = re.sub(r"<([^<:]+:)?", "{", uri).replace(">", "}")
+
+    return uri
+
+
+def convert_responses_key_to_string(responses: ResponseDict) -> ResponseStrKeyDict:
+    """Convert key to string"""
+    _responses = {}
+    for key, value in responses.items():
+        if isinstance(key, HTTPStatus):
+            key = str(key.value)
+        elif isinstance(key, int):
+            key = str(key)
+        _responses[key] = value
+
+    return _responses
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3/view.py` & `flask-openapi3-2.5.0/flask_openapi3/view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2022/10/14 16:09
-import re
 import typing
+import warnings
+from copy import deepcopy
+from typing import Optional, List, Dict, Any, Callable
+
+from ._http import HTTPMethod
+from .models import ExternalDocumentation
+from .models import ExtraRequestBody
+from .models import Server
+from .models import Tag
+from .types import ResponseDict
+from .utils import convert_responses_key_to_string
+from .utils import get_operation
+from .utils import get_operation_id_for_path
+from .utils import get_responses
+from .utils import parse_and_store_tags
+from .utils import parse_method
+from .utils import parse_parameters
+from .utils import parse_rule
 
 if typing.TYPE_CHECKING:
     from .openapi import OpenAPI
 
-from copy import deepcopy
-from typing import Optional, List, Dict, Type, Any, Callable
-
-from pydantic import BaseModel
-
-from .http import HTTPMethod
-from .models.common import ExternalDocumentation, ExtraRequestBody
-from .models.server import Server
-from .models.tag import Tag
-from .utils import get_operation, parse_and_store_tags, parse_parameters, get_responses, parse_method, \
-    get_operation_id_for_path
+warnings.simplefilter("once")
 
 
 class APIView:
     def __init__(
             self,
             url_prefix: Optional[str] = None,
             view_tags: Optional[List[Tag]] = None,
             view_security: Optional[List[Dict[str, List[str]]]] = None,
-            view_responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            view_responses: Optional[ResponseDict] = None,
             doc_ui: bool = True,
             operation_id_callback: Callable = get_operation_id_for_path,
     ):
         """
         Create a class-based view
 
         Arguments:
             url_prefix: A path to prepend to all the APIView's urls
-            view_tags: APIView tags for every api
-            view_security: APIView security for every api
-            view_responses: APIView response models
-            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            view_tags: APIView tags for every API.
+            view_security: APIView security for every API.
+            view_responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            doc_ui: Enable OpenAPI document UI (Swagger UI and Redoc). Defaults to True.
             operation_id_callback: Callback function for custom operation_id generation.
-                Receives name (str), path (str) and method (str) parameters.
-                Defaults to `get_operation_id_for_path` from utils
+                                   Receives name (str), path (str) and method (str) parameters.
+                                   Defaults to `get_operation_id_for_path` from utils
         """
         self.url_prefix = url_prefix
         self.view_tags = view_tags or []
         self.view_security = view_security or []
-        self.view_responses = view_responses or {}
+
+        view_responses = view_responses or {}
+        # Convert key to string
+        self.view_responses = convert_responses_key_to_string(view_responses)
+
         self.doc_ui = doc_ui
         self.operation_id_callback: Callable = operation_id_callback
 
         self.views: Dict = dict()
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.tags: List[Tag] = []
@@ -59,40 +70,38 @@
     def route(self, rule: str):
         """Decorator for view class"""
 
         def wrapper(cls):
             if self.views.get(rule):
                 raise ValueError(f"malformed url rule: {rule!r}")
             methods = []
-            # /pet/<petId> --> /pet/{petId}
-            uri = re.sub(r"<([^<:]+:)?", "{", rule).replace(">", "}")
-            trail_slash = uri.endswith("/")
-            # merge url_prefix and uri
-            uri = self.url_prefix.rstrip("/") + "/" + uri.lstrip("/") if self.url_prefix else uri
-            if not trail_slash:
-                uri = uri.rstrip("/")
+
+            # Parse rule: merge url_prefix and format rule from /pet/<petId> to /pet/{petId}
+            uri = parse_rule(rule, url_prefix=self.url_prefix)
+
             for method in HTTPMethod:
                 cls_method = getattr(cls, method.lower(), None)
                 if not cls_method:
                     continue
                 methods.append(method)
                 if self.doc_ui is False:
                     continue
                 if not getattr(cls_method, "operation", None):
                     continue
-                # parse method
+                # Parse method
                 parse_method(uri, method, self.paths, cls_method.operation)
-                # update operation_id
+                # Update operation_id
                 if not cls_method.operation.operationId:
                     cls_method.operation.operationId = self.operation_id_callback(
                         name=cls_method.__qualname__,
                         path=rule,
                         method=method
                     )
-            # /pet/{petId} --> /pet/<petId>
+
+            # Convert route parameters from {param} to <param>
             _rule = uri.replace("{", "<").replace("}", ">")
             self.views[_rule] = (cls, methods)
 
             return cls
 
         return wrapper
 
@@ -102,15 +111,15 @@
             tags: Optional[List[Tag]] = None,
             summary: Optional[str] = None,
             description: Optional[str] = None,
             external_docs: Optional[ExternalDocumentation] = None,
             operation_id: Optional[str] = None,
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
-            responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
+            responses: Optional[ResponseDict] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
             openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True
     ) -> Callable:
@@ -120,75 +129,98 @@
 
         Arguments:
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
-            extra_form: Extra information describing the request body(application/form).
-            extra_body: Extra information describing the request body(application/json).
-            responses: response's model must be pydantic BaseModel.
-            extra_responses: Extra information for responses.
+            extra_form: **Deprecated in v3.x**. Extra information describing the request body(application/form).
+            extra_body: **Deprecated in v3.x**. Extra information describing the request body(application/json).
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            extra_responses: **Deprecated in v3.x**. Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            doc_ui: Declares this operation to be shown. Default to True.
         """
 
+        if extra_form is not None:
+            warnings.warn(
+                """`extra_form` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_body is not None:
+            warnings.warn(
+                """`extra_body` will be deprecated in v3.x, please use `openapi_extra` instead.""",
+                DeprecationWarning)
+        if extra_responses is not None:
+            warnings.warn(
+                """`extra_responses` will be deprecated in v3.x, please use `responses` instead.""",
+                DeprecationWarning)
+
         if responses is None:
-            responses = {}
+            new_responses = {}
+        else:
+            # Convert key to string
+            new_responses = convert_responses_key_to_string(responses)
         if extra_responses is None:
             extra_responses = {}
         if security is None:
             security = []
         tags = tags + self.view_tags if tags else self.view_tags
 
         def decorator(func):
             if self.doc_ui is False or doc_ui is False:
                 return
-            # global response combine api responses
+            # Global response combines API responses
             combine_responses = deepcopy(self.view_responses)
-            combine_responses.update(**responses)
-            # create operation
+            combine_responses.update(**new_responses)
+            # Create operation
             operation = get_operation(
                 func,
                 summary=summary,
                 description=description,
                 openapi_extensions=openapi_extensions
             )
-            # set external docs
+            # Set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
             operation.operationId = operation_id
-            # only set `deprecated` if True otherwise leave it as None
+            # Only set `deprecated` if True, otherwise leave it as None
             operation.deprecated = deprecated
-            # add security
+            # Add security
             operation.security = security + self.view_security or None
-            # add servers
+            # Add servers
             operation.servers = servers
-            # store tags
+            # Store tags
             parse_and_store_tags(tags, self.tags, self.tag_names, operation)
-            # parse parameters
+            # Parse parameters
             parse_parameters(
                 func,
                 extra_form=extra_form,
                 extra_body=extra_body,
                 components_schemas=self.components_schemas,
                 operation=operation
             )
-            # parse response
+            # Parse response
             get_responses(combine_responses, extra_responses, self.components_schemas, operation)
             func.operation = operation
 
             return func
 
         return decorator
 
     def register(self, app: "OpenAPI", view_kwargs: Optional[Dict[Any, Any]] = None):
+        """
+        Register the API views with the given OpenAPI app.
+
+        Args:
+            app: An instance of the OpenAPI app.
+            view_kwargs: Additional keyword arguments to pass to the API views.
+        """
         if view_kwargs is None:
             view_kwargs = {}
         for rule, (cls, methods) in self.views.items():
             for method in methods:
                 func = getattr(cls, method.lower())
                 header, cookie, path, query, form, body = parse_parameters(func, doc_ui=False)
                 view_func = app.create_view_func(
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/PKG-INFO` & `flask-openapi3-2.5.0/flask_openapi3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.4.0rc1
+Version: 2.5.0
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,16 +34,16 @@
              width="60%" height="auto" alt="logo">
     </a>
 </div>
 <p align="center">
     <em>Generate REST API and OpenAPI documentation for your Flask project.</em>
 </p>
 <p align="center">
-    <a href="https://github.com/luolingchun/flask-openapi3/actions/workflows/test.yml" target="_blank">
-        <img class="off-glb" src="https://img.shields.io/github/actions/workflow/status/luolingchun/flask-openapi3/test.yml?branch=master" alt="test">
+    <a href="https://github.com/luolingchun/flask-openapi3/actions/workflows/tests.yml" target="_blank">
+        <img class="off-glb" src="https://img.shields.io/github/actions/workflow/status/luolingchun/flask-openapi3/tests.yml?branch=master" alt="test">
     </a>
     <a href="https://pypi.org/project/flask-openapi3/" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/v/flask-openapi3" alt="pypi">
     </a>
     <a href="https://pypistats.org/packages/flask-openapi3" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/dm/flask-openapi3" alt="pypistats">
     </a>
```

### Comparing `flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/SOURCES.txt` & `flask-openapi3-2.5.0/flask_openapi3.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,49 +12,77 @@
 examples/enum_demo.py
 examples/header_demo.py
 examples/image_demo.py
 examples/init_oauth_demo.py
 examples/just_flask.py
 examples/nested_apiblueprint_demo.py
 examples/openapi_extensions.py
+examples/openapi_extra.py
 examples/orjson_demo.py
 examples/pydantic_custom_root_types.py
 examples/response_demo.py
 examples/rest_demo.py
 examples/servers_demo.py
 examples/simple_demo.py
 examples/upload_file_demo.py
 flask_openapi3/__init__.py
 flask_openapi3/__version__.py
+flask_openapi3/_http.py
 flask_openapi3/blueprint.py
 flask_openapi3/commands.py
-flask_openapi3/http.py
 flask_openapi3/markdown.py
 flask_openapi3/openapi.py
 flask_openapi3/request.py
 flask_openapi3/scaffold.py
+flask_openapi3/types.py
 flask_openapi3/utils.py
 flask_openapi3/view.py
 flask_openapi3.egg-info/PKG-INFO
 flask_openapi3.egg-info/SOURCES.txt
 flask_openapi3.egg-info/dependency_links.txt
 flask_openapi3.egg-info/not-zip-safe
 flask_openapi3.egg-info/requires.txt
 flask_openapi3.egg-info/top_level.txt
 flask_openapi3/models/__init__.py
-flask_openapi3/models/common.py
-flask_openapi3/models/component.py
+flask_openapi3/models/callback.py
+flask_openapi3/models/components.py
+flask_openapi3/models/contact.py
+flask_openapi3/models/data_type.py
+flask_openapi3/models/discriminator.py
+flask_openapi3/models/encoding.py
+flask_openapi3/models/example.py
+flask_openapi3/models/external_documentation.py
 flask_openapi3/models/file.py
+flask_openapi3/models/header.py
 flask_openapi3/models/info.py
-flask_openapi3/models/oauth.py
-flask_openapi3/models/path.py
+flask_openapi3/models/license.py
+flask_openapi3/models/link.py
+flask_openapi3/models/media_type.py
+flask_openapi3/models/oauth_flow.py
+flask_openapi3/models/oauth_flows.py
+flask_openapi3/models/operation.py
+flask_openapi3/models/parameter.py
+flask_openapi3/models/parameter_in_type.py
+flask_openapi3/models/path_item.py
+flask_openapi3/models/paths.py
+flask_openapi3/models/reference.py
+flask_openapi3/models/request_body.py
+flask_openapi3/models/response.py
+flask_openapi3/models/responses.py
+flask_openapi3/models/schema.py
 flask_openapi3/models/security.py
+flask_openapi3/models/security_requirement.py
+flask_openapi3/models/security_scheme.py
+flask_openapi3/models/security_scheme_in_type.py
 flask_openapi3/models/server.py
+flask_openapi3/models/server_variable.py
+flask_openapi3/models/style_values.py
 flask_openapi3/models/tag.py
 flask_openapi3/models/validation_error.py
+flask_openapi3/models/xml.py
 flask_openapi3/templates/__init__.py
 flask_openapi3/templates/static/css/swagger-ui.css
 flask_openapi3/templates/static/images/apidoc.svg
 flask_openapi3/templates/static/images/rapidoc.svg
 flask_openapi3/templates/static/images/redoc.svg
 flask_openapi3/templates/static/images/swagger.svg
 flask_openapi3/templates/static/js/rapidoc-min.js
```

### Comparing `flask-openapi3-2.4.0rc1/setup.py` & `flask-openapi3-2.5.0/setup.py`

 * *Files identical despite different names*

