# Comparing `tmp/cmdcomp-2.0.5.tar.gz` & `tmp/cmdcomp-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.0.5.tar", max compression
+gzip compressed data, was "cmdcomp-2.0.6.tar", max compression
```

## Comparing `cmdcomp-2.0.5.tar` & `cmdcomp-2.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2425 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/README.md
--rw-r--r--   0        0        0       79 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2289 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/app.py
--rw-r--r--   0        0        0      573 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/completion.py
--rw-r--r--   0        0        0      734 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/config.py
--rw-r--r--   0        0        0      444 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/exception.py
--rw-r--r--   0        0        0      115 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/main.py
--rw-r--r--   0        0        0      115 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      535 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     3358 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2164 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1888 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1469 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      535 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0     6844 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      789 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      744 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      601 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1668 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/command/argument/values_argument.py
--rw-r--r--   0        0        0      808 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/config.py
--rw-r--r--   0        0        0     4371 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     2785 2023-08-02 05:58:17.379214 cmdcomp-2.0.5/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1696 2023-08-02 05:58:17.383214 cmdcomp-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2425 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/README.md
+-rw-r--r--   0        0        0       79 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2289 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/completion.py
+-rw-r--r--   0        0        0      734 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/config.py
+-rw-r--r--   0        0        0      444 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2164 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-08-02 14:16:53.412526 cmdcomp-2.0.6/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1888 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1469 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6844 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      888 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4338 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2949 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-08-02 14:16:53.416526 cmdcomp-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 cmdcomp-2.0.6/PKG-INFO
```

### Comparing `cmdcomp-2.0.5/README.md` & `cmdcomp-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/app.py` & `cmdcomp-2.0.6/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/completion.py` & `cmdcomp-2.0.6/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/config.py` & `cmdcomp-2.0.6/cmdcomp/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v1/app_info.py` & `cmdcomp-2.0.6/cmdcomp/v1/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.0.6/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v1/completion.py` & `cmdcomp-2.0.6/cmdcomp/v1/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.0.6/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.0.6/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/app_info.py` & `cmdcomp-2.0.6/cmdcomp/v2/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/command/__init__.py` & `cmdcomp-2.0.6/cmdcomp/v2/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.0.6/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.0.6/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.0.6/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/command/argument/values_argument.py` & `cmdcomp-2.0.6/cmdcomp/v2/command/argument/values_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/completion.py` & `cmdcomp-2.0.6/cmdcomp/v2/completion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import re
 from pathlib import Path
 from typing import Any
 
 from cmdcomp import __version__
 from cmdcomp.shell import ShellType
 from cmdcomp.v2.config import V2Config
 
 
 def generate_v2(shell: ShellType, config: V2Config) -> str:
     from jinja2 import Environment, FileSystemLoader
 
     env = Environment(
         loader=FileSystemLoader(Path(__file__).parent / "templates"),
     )
+    env.filters["ident"] = lambda x: re.sub(r"[\*\.,-]", "_", str(x))
     template = env.get_template(f"{shell.value}.sh.jinja")
 
     return template.render(
         app_name=config.app.name,
         app_aliases=config.app.aliases + config.root.aliases,
         commands={config.app.name: config.root},
         append_key_tag=_append_key_tag,
```

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.0.6/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set func_name = "_" + app_name|replace("-","_") -%}
+{%- set func_name = "_" + app_name|ident -%}
 {%- set scope = "" -%}
 
 {#- macro def -#}
 {%- macro argument_completion(argument) -%}
 {% if argument.type == "values" -%}
 if [ $cur -eq $COMP_CWORD ] ; then
   COMPREPLY=( $(compgen -W "{{ argument.values|join(" ") }}" -- "$cur") )
@@ -113,15 +113,15 @@
   for word in ${COMP_WORDS[@]}; do
     case "${cmd},${word}" in
       ",$1")
         cmd="{{ func_name }}"
         cur=$(( cur + opts_cur + 1 ))
         ;;
 {% for (tag, command_name), subcommand in append_key_tag(commands[app_name].subcommands, func_name).items() recursive %}
-      {%- set new_tag = tag + "_" + command_name|replace("-","_") %}
+      {%- set new_tag = tag + "_" + command_name|ident %}
       {{ tag }},{{ command_name }}
 {%- for alias in subcommand.aliases -%}
       |{{ tag }},{{ alias }}
 {%- endfor -%})
         cmd="{{ new_tag }}"
         cur=$(( cur + opts_cur + 1 ))
         ;;
@@ -136,15 +136,15 @@
   case "${cmd}" in
     {{ func_name }})
       {{ command_completion(commands[app_name], 1)|indent(6) }}
 
       return 0
       ;;
 {% for (tag, command_name), subcommand in append_key_tag(commands[app_name].subcommands, func_name).items() recursive %}
-{%- set new_tag = tag + "_" + command_name|replace("-","_") %}
+{%- set new_tag = tag + "_" + command_name|ident %}
     {{ new_tag }})
       {{ command_completion(subcommand, loop.depth + 1)|indent(6) }}
 
       return 0
       ;;
 {{ loop(append_key_tag(subcommand.subcommands, new_tag).items()) -}}
 {% endfor %}
```

### Comparing `cmdcomp-2.0.5/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.0.6/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set func_name = "_" + app_name|replace("-","_") -%}
+{%- set func_name = "_" + app_name|ident -%}
 {%- set scope = "" -%}
 
 {#- macro def -#}
 {%- macro candidate(target_name, target) -%}
   {% if target.aliases|length == 0 -%}
     {{ target_name }}
   {%- else -%}
@@ -18,15 +18,15 @@
 {#- macro def -#}
 {%- macro contents(arg_name, argument) -%}
   {%- if argument.type == 'values' -%}
           :values:{{ "(" + argument.values|map("string")|join(" ") + ")" }}
   {%- elif argument.type == 'file' -%}
           :file:_files{%- if argument.base_path is not none %} -W "{{ argument.base_path }}"{%- endif -%}
   {%- elif argument.type == 'command' -%}
-          :command:_values '{{ arg_name|trim("-") }}' $({{ argument.execute }})
+          :command:_values '{{ arg_name|ident }}' '"$_{{ arg_name|ident }}_execute_result"'
   {%- elif argument.type == 'flag' -%}
   {%- endif -%}
 {%- endmacro -%}
 
 #!/bin/zsh
 #
 # Code generated by cmdcomp "{{ version }}". DO NOT EDIT.
@@ -40,32 +40,37 @@
   local cmd_name={{ app_name }}
 
   case $cmd_name in
 {%- for cmd_name, command in commands.items() recursive %}
 {%- set scope = scope + "_" + cmd_name %}
     {{ ([cmd_name] + command.aliases)|join("|") }})
 {%- if command.has_subcommands %}
-      local -a _{{ scope|replace("-", "_") }}_subcmds
-      _{{ scope|replace("-", "_") }}_subcmds=(
+      local -a _{{ scope|ident }}_subcmds
+      _{{ scope|ident }}_subcmds=(
 {%- for subcmd_name, subcommand in command.subcommands.items() %}
         {{ candidate(subcmd_name, subcommand) }}'{{ description(subcommand) }}'
 {%- endfor %}
       )
 {% endif %}
+{%- for arg_name, argument in command.arguments.items() -%}
+{%- if argument.type == "command" %}
+      local _{{ arg_name|ident }}_execute_result=$({{ argument.execute }})
+{%- endif %}
+{%- endfor %}
       _arguments -C \
 {%- for kwd_name, keyword in command.keyword_arguments.items() %}
         {{ candidate(kwd_name, keyword) }}'{{ description(keyword) }}{{ contents(kwd_name, keyword) }}' \
 {%- endfor %}
 {%- for pos_name, positional in command.positional_arguments.items() %}
         '{{ pos_name }}{{ contents(pos_name, positional) }}' \
 {%- endfor %}
 {%- if command.has_positional_wildcard_argument %}
         '*{{ contents("*", command.positional_wildcard_argument) }}' \
 {%- elif command.has_subcommands %}
-        '1: :_values "subcommand" ${_{{ scope|replace("-", "_") }}_subcmds[@]}' \
+        '1: :_values "subcommand" ${_{{ scope|ident }}_subcmds[@]}' \
         '*:: :->args' \
 {%- endif %}
         && ret=0
 {%- if command.has_subcommands %}
 
       cmd_name=$words[1]
       case $state in
```

### Comparing `cmdcomp-2.0.5/pyproject.toml` & `cmdcomp-2.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.0.5"
+version = "2.0.6"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-2.0.5/PKG-INFO` & `cmdcomp-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 2.0.5
+Version: 2.0.6
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
-Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.5 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.6 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

