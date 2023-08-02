# Comparing `tmp/cmdcomp-2.0.4.tar.gz` & `tmp/cmdcomp-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.0.4.tar", max compression
+gzip compressed data, was "cmdcomp-2.0.5.tar", max compression
```

## Comparing `cmdcomp-2.0.4.tar` & `cmdcomp-2.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2425 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/README.md
--rw-r--r--   0        0        0       79 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2289 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/app.py
--rw-r--r--   0        0        0      573 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/completion.py
--rw-r--r--   0        0        0      734 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/config.py
--rw-r--r--   0        0        0      444 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/exception.py
--rw-r--r--   0        0        0      115 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/main.py
--rw-r--r--   0        0        0      115 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      535 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     3358 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2164 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1888 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1469 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      535 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0     6844 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      789 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      744 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      601 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1668 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/command/argument/values_argument.py
--rw-r--r--   0        0        0      808 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/config.py
--rw-r--r--   0        0        0     4371 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     2731 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1696 2023-08-02 04:59:56.266762 cmdcomp-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2425 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/README.md
+-rw-r--r--   0        0        0       79 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2289 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/completion.py
+-rw-r--r--   0        0        0      734 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/config.py
+-rw-r--r--   0        0        0      444 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2164 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1888 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1469 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6844 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      808 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4371 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2785 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-08-02 05:58:17.383214 cmdcomp-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.5/PKG-INFO
```

### Comparing `cmdcomp-2.0.4/README.md` & `cmdcomp-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/app.py` & `cmdcomp-2.0.5/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/completion.py` & `cmdcomp-2.0.5/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/config.py` & `cmdcomp-2.0.5/cmdcomp/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v1/app_info.py` & `cmdcomp-2.0.5/cmdcomp/v1/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.0.5/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v1/completion.py` & `cmdcomp-2.0.5/cmdcomp/v1/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.0.5/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.0.5/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/app_info.py` & `cmdcomp-2.0.5/cmdcomp/v2/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/command/__init__.py` & `cmdcomp-2.0.5/cmdcomp/v2/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.0.5/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.0.5/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.0.5/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/command/argument/values_argument.py` & `cmdcomp-2.0.5/cmdcomp/v2/command/argument/values_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/completion.py` & `cmdcomp-2.0.5/cmdcomp/v2/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.0.5/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.4/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.0.5/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,16 @@
   local cmd_name={{ app_name }}
 
   case $cmd_name in
 {%- for cmd_name, command in commands.items() recursive %}
 {%- set scope = scope + "_" + cmd_name %}
     {{ ([cmd_name] + command.aliases)|join("|") }})
 {%- if command.has_subcommands %}
-      local -a _{{ scope }}_subcmds
-      _{{ scope }}_subcmds=(
+      local -a _{{ scope|replace("-", "_") }}_subcmds
+      _{{ scope|replace("-", "_") }}_subcmds=(
 {%- for subcmd_name, subcommand in command.subcommands.items() %}
         {{ candidate(subcmd_name, subcommand) }}'{{ description(subcommand) }}'
 {%- endfor %}
       )
 {% endif %}
       _arguments -C \
 {%- for kwd_name, keyword in command.keyword_arguments.items() %}
@@ -57,15 +57,15 @@
 {%- endfor %}
 {%- for pos_name, positional in command.positional_arguments.items() %}
         '{{ pos_name }}{{ contents(pos_name, positional) }}' \
 {%- endfor %}
 {%- if command.has_positional_wildcard_argument %}
         '*{{ contents("*", command.positional_wildcard_argument) }}' \
 {%- elif command.has_subcommands %}
-        '1: :_values "subcommand" ${_{{ scope }}_subcmds[@]}' \
+        '1: :_values "subcommand" ${_{{ scope|replace("-", "_") }}_subcmds[@]}' \
         '*:: :->args' \
 {%- endif %}
         && ret=0
 {%- if command.has_subcommands %}
 
       cmd_name=$words[1]
       case $state in
```

### Comparing `cmdcomp-2.0.4/pyproject.toml` & `cmdcomp-2.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.0.4"
+version = "2.0.5"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-2.0.4/PKG-INFO` & `cmdcomp-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 2.0.4
+Version: 2.0.5
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.4 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.5 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

