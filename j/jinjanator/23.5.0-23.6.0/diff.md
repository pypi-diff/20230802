# Comparing `tmp/jinjanator-23.5.0.tar.gz` & `tmp/jinjanator-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 24 20:08:03 2023, max compression
+gzip compressed data, last modified: Tue Aug  1 22:16:33 2023, max compression
```

## Comparing `jinjanator-23.5.0.tar` & `jinjanator-23.6.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
--rw-r--r--   0        0        0     2056 2023-07-24 20:08:03.000000 jinjanator-23.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     9172 2023-07-24 20:08:03.000000 jinjanator-23.5.0/README.md
--rw-r--r--   0        0        0       81 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/__init__.py
--rw-r--r--   0        0        0     9612 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/cli.py
--rw-r--r--   0        0        0      727 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/context.py
--rw-r--r--   0        0        0     1186 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/filters.py
--rw-r--r--   0        0        0     3520 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/formats.py
--rw-r--r--   0        0        0        0 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/py.typed
--rw-r--r--   0        0        0      162 2023-07-24 20:08:03.000000 jinjanator-23.5.0/src/jinjanator/version.py
--rw-r--r--   0        0        0     1614 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/__init__.py
--rw-r--r--   0        0        0      675 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1582 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_argparse.py
--rw-r--r--   0        0        0     1274 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_cli.py
--rw-r--r--   0        0        0     2723 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_env.py
--rw-r--r--   0        0        0      248 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_extension.py
--rw-r--r--   0        0        0      840 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_invalid_data.py
--rw-r--r--   0        0        0     3461 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_nginx_config.py
--rw-r--r--   0        0        0      780 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_output_file.py
--rw-r--r--   0        0        0      435 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_template_not_found.py
--rw-r--r--   0        0        0      501 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_undefined.py
--rw-r--r--   0        0        0      728 2023-07-24 20:08:03.000000 jinjanator-23.5.0/tests/test_unicode.py
--rw-r--r--   0        0        0       58 2023-07-24 20:08:03.000000 jinjanator-23.5.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-24 20:08:03.000000 jinjanator-23.5.0/LICENSE.apache-2.0
--rw-r--r--   0        0        0     1321 2023-07-24 20:08:03.000000 jinjanator-23.5.0/LICENSE.bsd-2-clause
--rw-r--r--   0        0        0     6482 2023-07-24 20:08:03.000000 jinjanator-23.5.0/pyproject.toml
--rw-r--r--   0        0        0     7811 2023-07-24 20:08:03.000000 jinjanator-23.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2694 2023-08-01 22:16:33.000000 jinjanator-23.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10144 2023-08-01 22:16:33.000000 jinjanator-23.6.0/README.md
+-rw-r--r--   0        0        0       81 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/__init__.py
+-rw-r--r--   0        0        0    12032 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/cli.py
+-rw-r--r--   0        0        0      692 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/context.py
+-rw-r--r--   0        0        0     1186 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/filters.py
+-rw-r--r--   0        0        0     6858 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/formats.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/py.typed
+-rw-r--r--   0        0        0      162 2023-08-01 22:16:33.000000 jinjanator-23.6.0/src/jinjanator/version.py
+-rw-r--r--   0        0        0     1614 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      675 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1683 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_argparse.py
+-rw-r--r--   0        0        0     2819 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2723 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_env.py
+-rw-r--r--   0        0        0      248 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_extension.py
+-rw-r--r--   0        0        0     1101 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_format_options.py
+-rw-r--r--   0        0        0      842 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_invalid_data.py
+-rw-r--r--   0        0        0     1886 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_json_input.py
+-rw-r--r--   0        0        0     3461 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_nginx_config.py
+-rw-r--r--   0        0        0      780 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_output_file.py
+-rw-r--r--   0        0        0      435 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_template_not_found.py
+-rw-r--r--   0        0        0      501 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_undefined.py
+-rw-r--r--   0        0        0      728 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_unicode.py
+-rw-r--r--   0        0        0     1912 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_yaml_input.py
+-rw-r--r--   0        0        0     1541 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_plugin/jinjanator_test_plugin.py
+-rw-r--r--   0        0        0      544 2023-08-01 22:16:33.000000 jinjanator-23.6.0/tests/test_plugin/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-08-01 22:16:33.000000 jinjanator-23.6.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-08-01 22:16:33.000000 jinjanator-23.6.0/LICENSE.apache-2.0
+-rw-r--r--   0        0        0     1321 2023-08-01 22:16:33.000000 jinjanator-23.6.0/LICENSE.bsd-2-clause
+-rw-r--r--   0        0        0     6877 2023-08-01 22:16:33.000000 jinjanator-23.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9407 2023-08-01 22:16:33.000000 jinjanator-23.6.0/PKG-INFO
```

### Comparing `jinjanator-23.5.0/CHANGELOG.md` & `jinjanator-23.6.0/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -24,14 +24,34 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.6.0](https://github.com/kpfleming/jinjanator/tree/23.6.0) - 2023-08-01
+
+### Backwards-incompatible Changes
+
+- Upgraded to plugins API 23.4.
+  
+
+
+### Additions
+
+- Added support for 'sequence' data in YAML-format input.
+  [#14](https://github.com/kpfleming/jinjanator/issues/14)
+- Added support for 'array' data in JSON-format input.
+  [#15](https://github.com/kpfleming/jinjanator/issues/15)
+- Added list of discovered plugins to '--version' output.
+  [#16](https://github.com/kpfleming/jinjanator/issues/16)
+- Options-related errors from format parsers are now handled.
+  [#17](https://github.com/kpfleming/jinjanator/issues/17)
+
+
 ## [23.5.0](https://github.com/kpfleming/jinjanator/tree/23.5.0) - 2023-07-24
 
 ### Additions
 
 - Added link to Ansible plugin.
```

### Comparing `jinjanator-23.5.0/README.md` & `jinjanator-23.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -187,15 +187,21 @@
 
     $ jinjanate --format=env config.j2 - < data.env
 
 
 ## Data Formats
 
 ### dotenv
-Data input from environment variables. This format does not support any options.
+Data input from environment variables.
+
+#### Options
+
+This format does not support any options.
+
+#### Usage
 
 Render directly from the current environment variable values:
 
     $ jinjanate config.j2
 
 Or alternatively, read the values from a dotenv file:
 
@@ -215,15 +221,21 @@
 
 If you're going to pipe a dotenv file into `jinjanate`, you'll need to
 use "-" as the second argument:
 
     $ jinjanate config.j2 - < data.env
 
 ### INI
-INI data input format. This format does not support any options.
+INI data input format.
+
+#### Options
+
+This format does not support any options.
+
+#### Usage
 
 data.ini:
 
 ```
 [nginx]
 hostname=localhost
 webroot=/var/www/project
@@ -235,15 +247,27 @@
     $ jinjanate config.j2 data.ini
 
 Or:
 
     $ cat data.ini | jinjanate --format=ini config.j2
 
 ### JSON
-JSON data input format. This format does not support any options.
+JSON data input format.
+
+#### Options
+
+* `array-name`: accepts a single string (e.g. `array-name=foo`), which
+  must be a valid Python identifier and not a Python keyword. If this
+  option is specified, and the JSON data provided is an `array`
+  (sequence, list), the specified name will be used to make the data
+  available to the Jinja2 template. Errors will be generated if
+  `array` data is provided and this option is not specified, or if
+  this option is specified and the data provided is an `object`.
+
+#### Usage
 
 data.json:
 
 ```
 {
     "nginx":{
         "hostname": "localhost",
@@ -258,15 +282,27 @@
     $ jinjanate config.j2 data.json
 
 Or:
 
     $ cat data.json | jinjanate --format=ini config.j2
 
 ### YAML
-YAML data input format. This format does not support any options.
+YAML data input format.
+
+#### Options
+
+* `sequence-name`: accepts a single string (e.g. `sequence-name=foo`),
+  which must be a valid Python identifier and not a Python keyword. If
+  this option is specified, and the YAML data provided is a `sequence`
+  (array, list), the specified name will be used to make the data
+  available to the Jinja2 template. Errors will be generated if
+  `sequence` data is provided and this option is not specified, or if
+  this option is specified and the data provided is a `mapping`.
+
+#### Usage
 
 data.yaml:
 
 ```
 nginx:
   hostname: localhost
   webroot: /var/www/project
```

#### html2text {}

```diff
@@ -64,51 +64,63 @@
 jinjanate config.j2 data.ini Render using JSON data source: $ jinjanate
 config.j2 data.json Render using YAML data source: $ jinjanate config.j2
 data.yaml Render using JSON data on stdin: $ curl http://example.com/
 service.json | jinjanate --format=json config.j2 - Render using environment
 variables: $ jinjanate config.j2 Or use environment variables from a file: $
 jinjanate config.j2 data.env Or pipe it: (note that you'll have to use "-" in
 this particular case): $ jinjanate --format=env config.j2 - < data.env ## Data
-Formats ### dotenv Data input from environment variables. This format does not
-support any options. Render directly from the current environment variable
-values: $ jinjanate config.j2 Or alternatively, read the values from a dotenv
-file: ``` NGINX_HOSTNAME=localhost NGINX_WEBROOT=/var/www/project NGINX_LOGS=/
-var/log/nginx/ ``` And render with: $ jinjanate config.j2 data.env Or: $ env |
-jinjanate --format=env config.j2 If you're going to pipe a dotenv file into
-`jinjanate`, you'll need to use "-" as the second argument: $ jinjanate
-config.j2 - < data.env ### INI INI data input format. This format does not
-support any options. data.ini: ``` [nginx] hostname=localhost webroot=/var/www/
-project logs=/var/log/nginx ``` Usage: $ jinjanate config.j2 data.ini Or: $ cat
-data.ini | jinjanate --format=ini config.j2 ### JSON JSON data input format.
-This format does not support any options. data.json: ``` { "nginx":
-{ "hostname": "localhost", "webroot": "/var/www/project", "logs": "/var/log/
-nginx" } } ``` Usage: $ jinjanate config.j2 data.json Or: $ cat data.json |
-jinjanate --format=ini config.j2 ### YAML YAML data input format. This format
-does not support any options. data.yaml: ``` nginx: hostname: localhost
-webroot: /var/www/project logs: /var/log/nginx ``` Usage: $ jinjanate config.j2
-data.yml Or: $ cat data.yml | jinjanate --format=yaml config.j2 ## Filters ###
-`env(varname, default=None)` Use an environment variable's value in the
-template. This filter is available even when your data source is something
-other than the environment. Example: ```jinja2 User: {{ user_login }} Pass: {
-{ "USER_PASSWORD" | env }} ``` You can provide a default value: ```jinja2 Pass:
-{{ "USER_PASSWORD" | env("-none-") }} ``` For your convenience, it's also
-available as a global function: ```jinja2 User: {{ user_login }} Pass: {{ env
-("USER_PASSWORD") }} ``` Notice that there must be quotes around the
-environment variable name when it is a literal string.  ## Chat If you'd like
-to chat with the Jinjanator community, join us on [Matrix](https://matrix.to/#/
-#jinjanator:km6g.us)! ## Credits This tool was created from [j2cli](https://
-github.com/kolypto/j2cli), which itself was created from [jinja2-cli](https://
-github.com/mattrobenolt/jinja2-cli). It was created to bring the project up to
-'modern' Python coding, packaging, and project-management standards, and to
-support plugins to provide extensibility. ["Standing on the shoulders of
-giants"](https://en.wikipedia.org/wiki/Standing_on_the_shoulders_of_giants)
-could not be more true than it is in the Python community; this project relies
-on many wonderful tools and libraries produced by the global open source
-software community, in addition to Python itself. I've listed many of them
-below, but if I've overlooked any please do not be offended :-) * [Attrs]
-(https://github.com/python-attrs/attrs) * [Black](https://github.com/psf/black)
-* [Hatch-Fancy-PyPI-Readme](https://github.com/hynek/hatch-fancy-pypi-readme) *
-[Hatch](https://github.com/pypa/hatch) * [Jinja2](https://github.com/pallets/
-jinja/) * [Mypy](https://github.com/python/mypy) * [Pluggy](https://github.com/
-pytest-dev/pluggy) * [Pytest](https://github.com/pytest-dev/pytest) * [Ruff]
-(https://github.com/astral-sh/ruff) * [Towncrier](https://github.com/twisted/
-towncrier)
+Formats ### dotenv Data input from environment variables. #### Options This
+format does not support any options. #### Usage Render directly from the
+current environment variable values: $ jinjanate config.j2 Or alternatively,
+read the values from a dotenv file: ``` NGINX_HOSTNAME=localhost
+NGINX_WEBROOT=/var/www/project NGINX_LOGS=/var/log/nginx/ ``` And render with:
+$ jinjanate config.j2 data.env Or: $ env | jinjanate --format=env config.j2 If
+you're going to pipe a dotenv file into `jinjanate`, you'll need to use "-" as
+the second argument: $ jinjanate config.j2 - < data.env ### INI INI data input
+format. #### Options This format does not support any options. #### Usage
+data.ini: ``` [nginx] hostname=localhost webroot=/var/www/project logs=/var/
+log/nginx ``` Usage: $ jinjanate config.j2 data.ini Or: $ cat data.ini |
+jinjanate --format=ini config.j2 ### JSON JSON data input format. #### Options
+* `array-name`: accepts a single string (e.g. `array-name=foo`), which must be
+a valid Python identifier and not a Python keyword. If this option is
+specified, and the JSON data provided is an `array` (sequence, list), the
+specified name will be used to make the data available to the Jinja2 template.
+Errors will be generated if `array` data is provided and this option is not
+specified, or if this option is specified and the data provided is an `object`.
+#### Usage data.json: ``` { "nginx":{ "hostname": "localhost", "webroot": "/
+var/www/project", "logs": "/var/log/nginx" } } ``` Usage: $ jinjanate config.j2
+data.json Or: $ cat data.json | jinjanate --format=ini config.j2 ### YAML YAML
+data input format. #### Options * `sequence-name`: accepts a single string
+(e.g. `sequence-name=foo`), which must be a valid Python identifier and not a
+Python keyword. If this option is specified, and the YAML data provided is a
+`sequence` (array, list), the specified name will be used to make the data
+available to the Jinja2 template. Errors will be generated if `sequence` data
+is provided and this option is not specified, or if this option is specified
+and the data provided is a `mapping`. #### Usage data.yaml: ``` nginx:
+hostname: localhost webroot: /var/www/project logs: /var/log/nginx ``` Usage: $
+jinjanate config.j2 data.yml Or: $ cat data.yml | jinjanate --format=yaml
+config.j2 ## Filters ### `env(varname, default=None)` Use an environment
+variable's value in the template. This filter is available even when your data
+source is something other than the environment. Example: ```jinja2 User: {
+{ user_login }} Pass: {{ "USER_PASSWORD" | env }} ``` You can provide a default
+value: ```jinja2 Pass: {{ "USER_PASSWORD" | env("-none-") }} ``` For your
+convenience, it's also available as a global function: ```jinja2 User: {
+{ user_login }} Pass: {{ env("USER_PASSWORD") }} ``` Notice that there must be
+quotes around the environment variable name when it is a literal string.  ##
+Chat If you'd like to chat with the Jinjanator community, join us on [Matrix]
+(https://matrix.to/#/#jinjanator:km6g.us)! ## Credits This tool was created
+from [j2cli](https://github.com/kolypto/j2cli), which itself was created from
+[jinja2-cli](https://github.com/mattrobenolt/jinja2-cli). It was created to
+bring the project up to 'modern' Python coding, packaging, and project-
+management standards, and to support plugins to provide extensibility.
+["Standing on the shoulders of giants"](https://en.wikipedia.org/wiki/
+Standing_on_the_shoulders_of_giants) could not be more true than it is in the
+Python community; this project relies on many wonderful tools and libraries
+produced by the global open source software community, in addition to Python
+itself. I've listed many of them below, but if I've overlooked any please do
+not be offended :-) * [Attrs](https://github.com/python-attrs/attrs) * [Black]
+(https://github.com/psf/black) * [Hatch-Fancy-PyPI-Readme](https://github.com/
+hynek/hatch-fancy-pypi-readme) * [Hatch](https://github.com/pypa/hatch) *
+[Jinja2](https://github.com/pallets/jinja/) * [Mypy](https://github.com/python/
+mypy) * [Pluggy](https://github.com/pytest-dev/pluggy) * [Pytest](https://
+github.com/pytest-dev/pytest) * [Ruff](https://github.com/astral-sh/ruff) *
+[Towncrier](https://github.com/twisted/towncrier)
```

### Comparing `jinjanator-23.5.0/src/jinjanator/cli.py` & `jinjanator-23.6.0/src/jinjanator/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import argparse
+import importlib
 import os
 import sys
 
 from pathlib import Path
 from typing import (
     Any,
     Callable,
+    Iterable,
     Mapping,
     Sequence,
     TextIO,
     cast,
 )
 
 import jinja2
@@ -102,30 +104,73 @@
     ) -> None:
         if self.already_seen and option_string:
             parser.error(option_string + " cannot be specified more than once.")
         setattr(namespace, self.dest, values)
         self.already_seen = True
 
 
+def print_version_info(
+    stream: TextIO = sys.stderr, *, plugin_identities: Iterable[str]
+) -> None:
+    print(
+        f"{Path(sys.argv[0]).name} {version}, Jinja2"
+        f" {importlib.metadata.version('jinja2')}",
+        file=stream,
+    )
+    header_printed = False
+    for plugin in plugin_identities:
+        if not header_printed:
+            print("Plugins:", file=stream)
+            header_printed = True
+
+        print(f"   {plugin}", file=stream)
+
+
+class VersionAction(argparse.Action):
+    def __init__(  # noqa: PLR0913
+        self,
+        option_strings: list[str],
+        plugin_identities: Iterable[str],
+        dest: str = argparse.SUPPRESS,
+        default: str = argparse.SUPPRESS,
+        help: str = "",  # noqa: A002
+    ):
+        super().__init__(
+            option_strings=option_strings, dest=dest, default=default, nargs=0, help=help
+        )
+        self.plugin_identities = plugin_identities
+
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,  # noqa: ARG002
+        values: str | Sequence[Any] | None,  # noqa: ARG002
+        option_string: str | None = None,  # noqa: ARG002
+    ) -> None:
+        print_version_info(sys.stdout, plugin_identities=self.plugin_identities)
+        parser.exit()
+
+
 def parse_args(
-    formats: Mapping[str, jinjanator_plugins.Format],
+    formats: Mapping[str, type[jinjanator_plugins.Format]],
+    plugin_identities: Iterable[str],
     argv: Sequence[str] | None = None,
 ) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="j2",
+        prog="jinjanate",
         description="Command-line interface to Jinja2 for templating in shell scripts.",
         epilog="",
     )
 
     parser.add_argument(
         "-v",
         "--version",
-        action="version",
-        version=f"jinjanate {version}, Jinja2 {jinja2.__version__}",
-        help="display version of this program",
+        action=VersionAction,
+        help="display version of this program and any installed plugins",
+        plugin_identities=plugin_identities,
     )
 
     parser.add_argument(
         "-f",
         "--format",
         action=UniqueStore,
         default="?",
@@ -195,47 +240,63 @@
     pm.add_hookspecs(jinjanator_plugins.PluginHooks)
     pm.register(filters)
     pm.register(formats)
     pm.load_setuptools_entrypoints("jinjanator")
     return cast(jinjanator_plugins.PluginHookCallers, pm.hook)
 
 
+def validate_format_options(
+    fmt: type[jinjanator_plugins.Format], options: Sequence[str] | None
+) -> jinjanator_plugins.Format:
+    if options:
+        if not fmt.option_names:
+            raise jinjanator_plugins.FormatOptionUnknownError(fmt, options[0])
+
+        for opt in options:
+            if opt.split("=")[0] not in fmt.option_names:
+                raise jinjanator_plugins.FormatOptionUnknownError(fmt, opt)
+
+    return fmt(options)
+
+
 def render_command(
     cwd: Path,
     environ: Mapping[str, str],
     stdin: TextIO | None,
     argv: Sequence[str],
 ) -> str:
     plugin_hook_callers = get_hook_callers()
 
-    available_formats: dict[str, jinjanator_plugins.Format] = {}
+    available_formats: dict[str, type[jinjanator_plugins.Format]] = {}
 
     for plugin_formats in plugin_hook_callers.plugin_formats():
         available_formats.update(plugin_formats)
 
-    args = parse_args(available_formats, argv[1:])
+    plugin_identities = plugin_hook_callers.plugin_identities()
+
+    args = parse_args(available_formats, plugin_identities, argv[1:])
 
     if not args.quiet:
-        print(
-            f"{Path(argv[0]).name} {version}, Jinja2 {jinja2.__version__}",
-            file=sys.stderr,
-        )
+        print_version_info(plugin_identities=plugin_identities)
 
     if args.format == "?":
         if args.data is None or str(args.data) == "-":
             args.format = "env"
         else:
             suffix = args.data.suffix
             for k, v in available_formats.items():
-                if suffix in v.suffixes:
+                if v.suffixes and suffix in v.suffixes:
                     args.format = k
                     break
             if args.format == "?":
-                msg = f"no format which can read '{suffix}' files available"
-                raise SystemExit(msg)
+                print(
+                    f"No format which can read '{suffix}' files available",
+                    file=sys.stderr,
+                )
+                raise SystemExit(1)
 
     # We always expect a file;
     # unless the user wants 'env', and there's no input file provided.
     if args.format == "env":
         """
         With the "env" format, if no dotenv filename is provided,
         we have two options: 1. The user wants to use the current
@@ -259,23 +320,24 @@
         else:
             input_data_f = args.data.open()
     else:
         input_data_f = (
             stdin if args.data is None or str(args.data) == "-" else args.data.open()
         )
 
+    fmt = validate_format_options(available_formats[args.format], args.format_options)
+
     if args.format == "env" and input_data_f is None:
         context = environ
     else:
         context = read_context_data(
-            available_formats[args.format],
+            fmt,
             input_data_f,
             environ,
             args.import_env,
-            args.format_options,
         )
 
     renderer = Jinja2TemplateRenderer(
         cwd,
         args.undefined,
         j2_env_params={},
         plugin_hook_callers=plugin_hook_callers,
@@ -314,13 +376,25 @@
 
 def main(args: list[str] | None = None) -> int | None:
     try:
         if args is None:  # pragma: no cover
             args = sys.argv
 
         output = render_command(Path.cwd(), os.environ, sys.stdin, args)
-    except SystemExit:
+    except jinjanator_plugins.FormatOptionUnknownError as exc:
+        print(str(exc), file=sys.stderr)
+        return 2
+    except jinjanator_plugins.FormatOptionUnsupportedError as exc:
+        print(str(exc), file=sys.stderr)
+        return 3
+    except jinjanator_plugins.FormatOptionValueError as exc:
+        print(str(exc), file=sys.stderr)
+        return 4
+    except SystemExit as exc:
+        if isinstance(exc.code, int):
+            return exc.code
+
         return 1
 
     sys.stdout.write(output)
 
     return None
```

### Comparing `jinjanator-23.5.0/src/jinjanator/context.py` & `jinjanator-23.6.0/src/jinjanator/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Mapping, TextIO
 
 
 if TYPE_CHECKING:  # pragma: no cover
-    from jinjanator_plugins import Format
+    from jinjanator_plugins import (
+        Format,
+    )
 
 
 def read_context_data(
     fmt: Format,
     f: TextIO | None,
     environ: Mapping[str, str],
     import_env: str | None = None,
-    format_options: list[str] | None = None,
 ) -> Mapping[str, Any]:
     if not f:
         msg = "no input supplied"
         raise ValueError(msg)
 
     context: dict[str, Any] = {}
 
-    context.update(fmt.parser(f.read(), format_options))
+    result = fmt.parse(f.read())
+
+    context.update(result)
 
     if import_env is not None:
         if import_env == "":
             context.update(environ)
         else:
             context[import_env] = environ
 
-    # Done
     return context
```

### Comparing `jinjanator-23.5.0/src/jinjanator/filters.py` & `jinjanator-23.6.0/src/jinjanator/filters.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/tests/__init__.py` & `jinjanator-23.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/tests/conftest.py` & `jinjanator-23.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/tests/test_argparse.py` & `jinjanator-23.6.0/tests/test_argparse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from __future__ import annotations
 
-from typing import Any, Mapping
+from typing import Iterable, Mapping
 
 import pytest
 
-from jinjanator_plugins import Format
-
 from jinjanator.cli import parse_args
 
 
-def fake_env_parser(
-    data: str, options: list[str] | None = None  # noqa: ARG001
-) -> Mapping[str, Any]:
-    return {"foo": "bar"}
-
-
-fake_env_format = Format(parser=fake_env_parser, suffixes=["env"])
+class FakeFormat:
+    name = "env"
+    suffixes: Iterable[str] | None = (".env",)
+    option_names: Iterable[str] | None = ()
+
+    def __init__(self, options: Iterable[str] | None) -> None:
+        pass
+
+    def parse(
+        self,
+        data_string: str,  # noqa: ARG002
+    ) -> Mapping[str, str]:
+        return {"foo": "bar"}
 
 
 def test_invalid_arg() -> None:
     """Ensure that an invalid argument is not accepted."""
     with pytest.raises(SystemExit):
-        parse_args({}, ["--test-invalid-arg"])
+        parse_args({}, [], ["--test-invalid-arg"])
 
 
 @pytest.mark.parametrize(
     "args",
     [
         ["--format", "env"],
         ["--format-option", "opt"],
@@ -36,28 +40,28 @@
         ["-e", "env"],
         ["-f", "env"],
         ["-o", "output"],
     ],
 )
 def test_args(args: list[str]) -> None:
     """Ensure that known arguments are accepted."""
-    parse_args({"env": fake_env_format}, [*args, "template"])
+    parse_args({"env": FakeFormat}, [], [*args, "template"])
 
 
 def test_version() -> None:
     """Ensure that '--version' argument is accepted and program exits without an error."""
     with pytest.raises(SystemExit) as excinfo:
-        parse_args({}, ["--version"])
+        parse_args({}, [], ["--version"])
     assert 0 == excinfo.value.code
 
 
 @pytest.mark.xfail()
 @pytest.mark.parametrize(
     "args",
     [
         ["--format", "env", "-f", "env"],
         ["--import-env", "env", "-e", "env"],
     ],
 )
 def test_duplicate_args(args: list[str]) -> None:
     """Ensure that duplicate arguments are not accepted."""
-    parse_args({"env": fake_env_format}, [*args, "template"])
+    parse_args({"env": FakeFormat}, [], [*args, "template"])
```

### Comparing `jinjanator-23.5.0/tests/test_cli.py` & `jinjanator-23.6.0/tests/test_json_input.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 from __future__ import annotations
 
-from typing import Any
-
+import jinjanator_plugins
 import pytest
 
-import jinjanator.cli
-
 from . import (
     FilePairFactory,
     render_file,
 )
 
 
-def test_quiet(make_file_pair: FilePairFactory, capsys: Any) -> None:
-    files = make_file_pair("Hello {{name}}!", "name=Blart", "env")
-    render_file(files, ["--quiet"])
-    captured = capsys.readouterr()
-    assert 0 == len(captured.err)
-
-
-def test_unavailable_suffix(make_file_pair: FilePairFactory) -> None:
-    files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
-    with pytest.raises(
-        SystemExit,
-        match="no format which can read '.xyz' files available",
-    ):
-        render_file(files, [])
-
-
-def test_main_normal(make_file_pair: FilePairFactory, capsys: Any) -> None:
-    files = make_file_pair("Hello {{name}}!", "name=Blart", "env")
-    assert (
-        jinjanator.cli.main(["--quiet", str(files.template_file), str(files.data_file)])
-        is None
-    )
-    captured = capsys.readouterr()
-    assert "Hello Blart!" == captured.out
-
-
-def test_main_failure(make_file_pair: FilePairFactory) -> None:
-    files = make_file_pair("Hello {{name}}!", "name=Blart", "xyz")
-    assert 1 == jinjanator.cli.main(
-        ["--quiet", str(files.template_file), str(files.data_file)]
-    )
+def test_mapping_normal(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ foo }}", '{"foo": "bar"}', "json")
+
+    assert "bar" == render_file(files, [])
+
+
+def test_mapping_with_array_name_option(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ foo }}", '{"foo": "bar"}', "json")
+
+    with pytest.raises(jinjanator_plugins.FormatOptionUnsupportedError):
+        assert render_file(files, ["--format-option", "array-name=seq"])
+
+
+def test_array_normal(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ seq[0] }}", "[1,2,3]", "json")
+
+    assert "1" == render_file(files, ["--format-option", "array-name=seq"])
+
+
+def test_array_without_array_name_option(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ seq[0] }}", "[1,2,3]", "json")
+
+    with pytest.raises(jinjanator_plugins.FormatOptionUnsupportedError):
+        assert render_file(files, [])
+
+
+def test_array_invalid_name(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ seq[0] }}", "[1,2,3]", "json")
+
+    with pytest.raises(jinjanator_plugins.FormatOptionValueError):
+        render_file(files, ["--format-option", "array-name=334seq"])
+
+
+def test_array_invalid_value(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ seq[0] }}", "[1,2,3]", "json")
+
+    with pytest.raises(jinjanator_plugins.FormatOptionValueError):
+        render_file(files, ["--format-option", "array-name=abc=def"])
+
+
+def test_array_keyword_name(make_file_pair: FilePairFactory) -> None:
+    files = make_file_pair("{{ seq[0] }}", "[1,2,3]", "json")
+
+    with pytest.raises(jinjanator_plugins.FormatOptionValueError):
+        render_file(files, ["--format-option", "array-name=raise"])
```

### Comparing `jinjanator-23.5.0/tests/test_env.py` & `jinjanator-23.6.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/tests/test_invalid_data.py` & `jinjanator-23.6.0/tests/test_invalid_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     FilePairFactory,
     render_env,
     render_file,
 )
 
 
 def test_invalid_json(make_file_pair: FilePairFactory) -> None:
-    files = make_file_pair("", '["one", "two"]', "json")
+    files = make_file_pair("", "midge", "json")
 
-    with pytest.raises(TypeError, match="JSON input does not contain an object"):
+    with pytest.raises(TypeError, match="JSON input is neither an object nor an array"):
         assert render_file(files, [])
 
 
 def test_invalid_yaml(make_file_pair: FilePairFactory) -> None:
-    files = make_file_pair("", "-one\n-two", "yaml")
+    files = make_file_pair("", "midge", "yaml")
 
-    with pytest.raises(TypeError, match="YAML input does not contain a mapping"):
+    with pytest.raises(TypeError, match="YAML input is neither a mapping nor a sequence"):
         assert render_file(files, [])
 
 
 def test_no_input_data(make_file_pair: FilePairFactory) -> None:
     files = make_file_pair("", "", "yaml")
 
     with pytest.raises(ValueError, match="no input supplied"):
```

### Comparing `jinjanator-23.5.0/tests/test_nginx_config.py` & `jinjanator-23.6.0/tests/test_nginx_config.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/tests/test_output_file.py` & `jinjanator-23.6.0/tests/test_output_file.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/tests/test_unicode.py` & `jinjanator-23.6.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/LICENSE.apache-2.0` & `jinjanator-23.6.0/LICENSE.apache-2.0`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/LICENSE.bsd-2-clause` & `jinjanator-23.6.0/LICENSE.bsd-2-clause`

 * *Files identical despite different names*

### Comparing `jinjanator-23.5.0/pyproject.toml` & `jinjanator-23.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 dynamic = [
   "readme",
   "version",
 ]
 dependencies = [
   "attrs",
   "jinja2>=2.7.2",
-  "jinjanator-plugins==23.1.*",
+  "jinjanator-plugins==23.4.*",
   "PyYAML",
   "typing-extensions",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator"
 [project.scripts]
@@ -134,18 +134,21 @@
 "3.11",
 "3.12",
 ]
 
 [tool.hatch.envs.ci.scripts]
 ci = [
     "rm -f .coverage",
-    # run tests
-    "pytest --verbose --cov-append  --cov-branch --cov-fail-under=97 --cov=jinjanator",
-    # produce a coverage report with 'missing' lines indicated
-    "coverage report -m",
+    # run tests for 'no plugin' mode
+    "pip uninstall --yes jinjanator-test-plugin",
+    "pytest -m 'noplugin' --verbose  --cov-branch --cov=jinjanator",
+    # run tests for 'plugin' mode
+    "pip install ./tests/test_plugin",
+    "pytest -m 'not noplugin' --verbose --cov-append  --cov-branch --cov=jinjanator",
+    "coverage report --show-missing --fail-under=98",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
@@ -209,14 +212,17 @@
 "src/jinjanator/cli.py" = ["T201"]
 "tests/*" = [
   "PLC1901", # empty strings are falsey, but are less specific in tests
   "PT005",   # we use always underscores and explicit names
   "S101",    # assert
   "SIM300",  # Yoda rocks in tests
 ]
+"tests/test_plugin/*" = [
+  "INP001",  # we don't care that these are in implicit namespace packages
+]
 
 [tool.ruff.isort]
 lines-between-types = 1
 lines-after-imports = 2
 
 [tool.pytest.ini_options]
 minversion = "6.0"
@@ -224,14 +230,17 @@
 testpaths = [
     "tests",
 ]
 addopts = [
     "-ra",
     "--strict-markers",
 ]
+markers = [
+    "noplugin: tests which must run without plugins installed",
+]
 
 [tool.mypy]
 python_version = 3.8
 namespace_packages = true
 explicit_package_bases = true
 check_untyped_defs = true
 disallow_any_generics = true
@@ -243,14 +252,15 @@
 follow_imports = "normal"
 no_implicit_optional = true
 strict_equality = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_ignores = true
+exclude = ['tests/test_plugin/build']
 
 [tool.towncrier]
 name = "jinjanator"
 package = "jinjanator"
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
```

### Comparing `jinjanator-23.5.0/PKG-INFO` & `jinjanator-23.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator
-Version: 23.5.0
+Version: 23.6.0
 Summary: Command-line interface to Jinja2 for templating in shell scripts.
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>, Mark Vartanyan <kolypto@gmail.com>
 License: Apache-2.0
 License-File: LICENSE.apache-2.0
 License-File: LICENSE.bsd-2-clause
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs
 Requires-Dist: jinja2>=2.7.2
-Requires-Dist: jinjanator-plugins==23.1.*
+Requires-Dist: jinjanator-plugins==23.4.*
 Requires-Dist: pyyaml
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # *jinjanator*: CLI tool for rendering Jinja2 templates
 
 
@@ -198,15 +198,21 @@
 
     $ jinjanate --format=env config.j2 - < data.env
 
 
 ## Data Formats
 
 ### dotenv
-Data input from environment variables. This format does not support any options.
+Data input from environment variables.
+
+#### Options
+
+This format does not support any options.
+
+#### Usage
 
 Render directly from the current environment variable values:
 
     $ jinjanate config.j2
 
 Or alternatively, read the values from a dotenv file:
 
@@ -226,15 +232,21 @@
 
 If you're going to pipe a dotenv file into `jinjanate`, you'll need to
 use "-" as the second argument:
 
     $ jinjanate config.j2 - < data.env
 
 ### INI
-INI data input format. This format does not support any options.
+INI data input format.
+
+#### Options
+
+This format does not support any options.
+
+#### Usage
 
 data.ini:
 
 ```
 [nginx]
 hostname=localhost
 webroot=/var/www/project
@@ -246,15 +258,27 @@
     $ jinjanate config.j2 data.ini
 
 Or:
 
     $ cat data.ini | jinjanate --format=ini config.j2
 
 ### JSON
-JSON data input format. This format does not support any options.
+JSON data input format.
+
+#### Options
+
+* `array-name`: accepts a single string (e.g. `array-name=foo`), which
+  must be a valid Python identifier and not a Python keyword. If this
+  option is specified, and the JSON data provided is an `array`
+  (sequence, list), the specified name will be used to make the data
+  available to the Jinja2 template. Errors will be generated if
+  `array` data is provided and this option is not specified, or if
+  this option is specified and the data provided is an `object`.
+
+#### Usage
 
 data.json:
 
 ```
 {
     "nginx":{
         "hostname": "localhost",
@@ -269,15 +293,27 @@
     $ jinjanate config.j2 data.json
 
 Or:
 
     $ cat data.json | jinjanate --format=ini config.j2
 
 ### YAML
-YAML data input format. This format does not support any options.
+YAML data input format.
+
+#### Options
+
+* `sequence-name`: accepts a single string (e.g. `sequence-name=foo`),
+  which must be a valid Python identifier and not a Python keyword. If
+  this option is specified, and the YAML data provided is a `sequence`
+  (array, list), the specified name will be used to make the data
+  available to the Jinja2 template. Errors will be generated if
+  `sequence` data is provided and this option is not specified, or if
+  this option is specified and the data provided is a `mapping`.
+
+#### Usage
 
 data.yaml:
 
 ```
 nginx:
   hostname: localhost
   webroot: /var/www/project
@@ -319,22 +355,27 @@
 User: {{ user_login }}
 Pass: {{ env("USER_PASSWORD") }}
 ```
 
 Notice that there must be quotes around the environment variable name
 when it is a literal string.
 ## Release Information
-### Additions
+### Backwards-incompatible Changes
 
-- Added link to Ansible plugin.
+- Upgraded to plugins API 23.4.
   
 
 
-### Fixes
+### Additions
 
-- Corrected content of LICENSE file.
-  
-- Corrected formatting of README on PyPI.
+- Added support for 'sequence' data in YAML-format input.
+  [[#14](https://github.com/kpfleming/jinjanator/issues/14)](https://github.com/kpfleming/jinjanator/issues/14)
+- Added support for 'array' data in JSON-format input.
+  [[#15](https://github.com/kpfleming/jinjanator/issues/15)](https://github.com/kpfleming/jinjanator/issues/15)
+- Added list of discovered plugins to '--version' output.
+  [[#16](https://github.com/kpfleming/jinjanator/issues/16)](https://github.com/kpfleming/jinjanator/issues/16)
+- Options-related errors from format parsers are now handled.
+  [[#17](https://github.com/kpfleming/jinjanator/issues/17)](https://github.com/kpfleming/jinjanator/issues/17)
 
 
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator/blob/main/CHANGELOG.md)
```

