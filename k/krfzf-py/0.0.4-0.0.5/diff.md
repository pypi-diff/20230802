# Comparing `tmp/krfzf_py-0.0.4.tar.gz` & `tmp/krfzf_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krfzf_py-0.0.4.tar", max compression
+gzip compressed data, was "krfzf_py-0.0.5.tar", max compression
```

## Comparing `krfzf_py-0.0.4.tar` & `krfzf_py-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-01-15 14:43:28.929222 krfzf_py-0.0.4/LICENSE
--rw-r--r--   0        0        0       77 2023-01-15 14:43:28.929222 krfzf_py-0.0.4/fzf/__init__.py
--rw-r--r--   0        0        0     6218 2023-01-15 14:43:28.929222 krfzf_py-0.0.4/fzf/options.py
--rw-r--r--   0        0        0     4112 2023-01-15 14:43:28.929222 krfzf_py-0.0.4/fzf/process.py
--rw-r--r--   0        0        0      433 2023-01-15 14:43:28.929222 krfzf_py-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 14:43:28.929222 krfzf_py-0.0.4/readme.txt
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 krfzf_py-0.0.4/setup.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 krfzf_py-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/LICENSE
+-rw-r--r--   0        0        0       77 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/fzf/__init__.py
+-rw-r--r--   0        0        0     6522 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/fzf/options.py
+-rw-r--r--   0        0        0     4203 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/fzf/process.py
+-rw-r--r--   0        0        0      433 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/readme.txt
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 krfzf_py-0.0.5/PKG-INFO
```

### Comparing `krfzf_py-0.0.4/LICENSE` & `krfzf_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `krfzf_py-0.0.4/fzf/options.py` & `krfzf_py-0.0.5/fzf/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,100 @@
 import enum
+from typing import Optional
 
 
 class Algorithm(enum.Enum):
     V1 = "v1"
     V2 = "v2"
 
 
 class TiebreakSetting(enum.Enum):
-
     LENGTH = "length"
     BEGIN = "begin"
     END = "end"
     INDEX = "index"
 
 
 class Layout(enum.Enum):
-
     DEFAULT = "default"
     REVERSE = "reverse"
     REVERSE_LIST = "reverse-list"
 
 
 class BorderStyle(enum.Enum):
-
     ROUNDED = "rounded"
     SHARP = "sharp"
     HORIZONTAL = "horizontal"
     VERTICAL = "vertical"
     TOP = "top"
     BOTTOM = "bottom"
     LEFT = "left"
     RIGHT = "right"
     NONE = "none"
 
 
 class InfoStyle(enum.Enum):
-
     DEFAULT = "default"
     INLINE = "inline"
     HIDDEN = "hidden"
 
 
 def get_opts(
     extended: bool = True,
     match_exact: bool = False,
     case_insensitive: bool = True,
     normalise_literals: bool = True,
     algo_type: Algorithm = Algorithm.V2,
-    field_index_expressions: str = None,
-    with_field_index_expressions: str = None,
-    delimiter: str = None,
+    field_index_expressions: Optional[str] = None,
+    with_field_index_expressions: Optional[str] = None,
+    delimiter: Optional[str] = None,
     disable_search: bool = False,
     sort_results: bool = True,
     reverse_results: bool = False,
-    tiebreak_settings: TiebreakSetting = None,
+    tiebreak_settings: Optional[TiebreakSetting] = None,
     multi=False,
     mouse=True,
-    keybinds: str = None,
+    keybinds: Optional[str] = None,
     cycle=False,
     keep_right=False,
-    scroll_off_lines: int = None,
+    scroll_off_lines: Optional[int] = None,
     disable_horizontal_scroll=False,
     filepath_word=False,
-    jump_labels: str = None,
-    height: str = None,
-    minimum_height: str = None,
-    layout: Layout = None,
+    jump_labels: Optional[str] = None,
+    height: Optional[str] = None,
+    minimum_height: Optional[str] = None,
+    layout: Optional[Layout] = None,
     reversed_layout: bool = False,
-    border_style: BorderStyle = None,
+    border_style: Optional[BorderStyle] = None,
     only_ascii_borders: bool = False,
-    margin: str = None,
-    padding: str = None,
-    info_style: InfoStyle = None,
+    margin: Optional[str] = None,
+    padding: Optional[str] = None,
+    info_style: Optional[InfoStyle] = None,
     hide_info: bool = False,
-    prompt_string: str = None,
-    pointer_string: str = None,
-    selected_string: str = None,
-    header: str = None,
-    header_lines: int = None,
+    prompt_string: Optional[str] = None,
+    pointer_string: Optional[str] = None,
+    selected_string: Optional[str] = None,
+    header: Optional[str] = None,
+    header_lines: Optional[int] = None,
     header_first: bool = False,
     ansi: bool = False,
-    tab_character_number: int = None,
-    color: str = None,
+    tab_character_number: Optional[int] = None,
+    color: Optional[str] = None,
     bold_off: bool = False,
     use_black_background: bool = False,
-    history_file: str = None,
-    history_size: int = None,
-    preview: str = None,
-    preview_window_settings: str = None,
-    query: str = None,
+    history_file: Optional[str] = None,
+    history_size: Optional[int] = None,
+    preview: Optional[str] = None,
+    preview_window_settings: Optional[str] = None,
+    query: Optional[str] = None,
     select_first: bool = False,
     exit_when_empty: bool = False,
-    filter_mode: str = None,
+    filter_mode: Optional[str] = None,
     print_query: bool = False,
-    expect_keys: str = None,
+    expect_keys: Optional[str] = None,
     read0: bool = False,
     print0: bool = False,
     clear_screen: bool = True,
     sync: bool = False,
 ):
     opts = ()
```

### Comparing `krfzf_py-0.0.4/fzf/process.py` & `krfzf_py-0.0.5/fzf/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 
         return f(self, *args, **kwargs)
 
     return __inner__
 
 
 class Fzf:
-
     fetch_options = staticmethod(get_opts)
 
     def __init__(self, opts=[], *, encoding="utf-8", encoding_errors="strict"):
-
         if not has_fzf():
             raise RuntimeError(
                 "fzf was not found in PATH. Please ensure that the process can access fzf."
             )
 
         self.process = subprocess.Popen(
             [EXECUTABLE, *opts],
@@ -47,27 +45,24 @@
             Fzf.fetch_options(**opts),
             encoding=encoding,
             encoding_errors=encoding_errors,
         )
 
     @ensure_stdin_available
     def add_lines(self, lines: typing.Iterable, flush_last: bool = True):
-
         for line in lines:
-
             if not self.to_stdin(
                 data=line.encode(**self.encoding_options) + b"\n", flush=not flush_last
             ):
                 return
 
         if flush_last:
             self.to_stdin(flush=True)
 
     def close(self):
-
         try:
             if not self.process.stdin.closed:
                 self.process.stdin.close()
         except OSError:
             pass
 
     def to_stdin(self, data=None, flush=True):
@@ -87,15 +82,14 @@
             if not self.to_stdin(line, flush=not flush_last):
                 return
 
         if flush_last:
             self.to_stdin(flush=True)
 
     def get_output(self):
-
         self.process.wait()
 
         stdout = self.process.stdout.read().decode(**self.encoding_options)
 
         if not stdout:
             return None
 
@@ -119,25 +113,23 @@
     encoding_errors="strict",
     flush_last=False,
     **opts
 ):
     with Fzf.load_with_options(
         encoding=encoding, encoding_errors=encoding_errors, **opts
     ) as fzf:
-
         if escape_output:
             output_escape = lambda value: repr(value)[1:-1]
         else:
             output_escape = lambda value: value
 
         if processor:
             shallow_copy = {}
 
             def raw_process_save(value, processed_value):
-
                 if processed_value in shallow_copy:
                     return raw_process_save(value, processed_value + "*")
 
                 shallow_copy.update(
                     {
                         processed_value: value,
                     }
@@ -152,14 +144,17 @@
             generator = (output_escape(value) for value in components)
 
         fzf.add_lines(lines=generator, flush_last=flush_last)
 
     output = fzf.get_output()
 
     if processor and output is not None:
+        if isinstance(output, list):
+            return [shallow_copy[value] for value in output]
+
         return shallow_copy[output]
 
     return output
 
 
 def get_fzf_version():
     with Fzf(["--version"]) as fzf:
```

