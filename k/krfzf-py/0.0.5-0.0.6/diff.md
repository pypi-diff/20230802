# Comparing `tmp/krfzf_py-0.0.5.tar.gz` & `tmp/krfzf_py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krfzf_py-0.0.5.tar", max compression
+gzip compressed data, was "krfzf_py-0.0.6.tar", max compression
```

## Comparing `krfzf_py-0.0.5.tar` & `krfzf_py-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/LICENSE
--rw-r--r--   0        0        0       77 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/fzf/__init__.py
--rw-r--r--   0        0        0     6522 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/fzf/options.py
--rw-r--r--   0        0        0     4203 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/fzf/process.py
--rw-r--r--   0        0        0      433 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 11:21:02.353387 krfzf_py-0.0.5/readme.txt
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 krfzf_py-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-02 12:50:56.064195 krfzf_py-0.0.6/LICENSE
+-rw-r--r--   0        0        0       77 2023-08-02 12:50:56.064195 krfzf_py-0.0.6/fzf/__init__.py
+-rw-r--r--   0        0        0     6522 2023-08-02 12:50:56.064195 krfzf_py-0.0.6/fzf/options.py
+-rw-r--r--   0        0        0     5182 2023-08-02 12:50:56.064195 krfzf_py-0.0.6/fzf/process.py
+-rw-r--r--   0        0        0      411 2023-08-02 12:50:56.068194 krfzf_py-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 krfzf_py-0.0.6/PKG-INFO
```

### Comparing `krfzf_py-0.0.5/LICENSE` & `krfzf_py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `krfzf_py-0.0.5/fzf/options.py` & `krfzf_py-0.0.6/fzf/options.py`

 * *Files identical despite different names*

### Comparing `krfzf_py-0.0.5/fzf/process.py` & `krfzf_py-0.0.6/fzf/process.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,114 @@
 import importlib
 import shutil
 import subprocess
 import typing
 
+T = typing.TypeVar("T")
+
+
 get_opts = importlib.import_module(".options", __package__).get_opts
 
 EXECUTABLE = "fzf"
 
-has_fzf = lambda: shutil.which(EXECUTABLE) is not None
-
 
 def ensure_stdin_available(f):
     def __inner__(self, *args, **kwargs):
         if self.process.stdin.closed:
             return
 
         return f(self, *args, **kwargs)
 
     return __inner__
 
 
 class Fzf:
     fetch_options = staticmethod(get_opts)
 
-    def __init__(self, opts=[], *, encoding="utf-8", encoding_errors="strict"):
-        if not has_fzf():
+    def __init__(
+        self,
+        executable=EXECUTABLE,
+        opts=None,
+        disable_env: bool = False,
+        *,
+        encoding="utf-8",
+        encoding_errors="strict"
+    ):
+        opts = opts or []
+
+        if shutil.which(executable) is None:
             raise RuntimeError(
                 "fzf was not found in PATH. Please ensure that the process can access fzf."
             )
 
         self.process = subprocess.Popen(
             [EXECUTABLE, *opts],
             stdout=subprocess.PIPE,
             stdin=subprocess.PIPE,
+            env={} if disable_env else None,
         )
         self.encoding_options = {
             "encoding": encoding,
             "errors": encoding_errors,
         }
 
     @classmethod
-    def load_with_options(cls, *, encoding="utf-8", encoding_errors="strict", **opts):
+    def load_with_options(
+        cls,
+        *,
+        executable=EXECUTABLE,
+        encoding="utf-8",
+        encoding_errors="strict",
+        **opts
+    ):
         return cls(
-            Fzf.fetch_options(**opts),
+            executable=executable,
+            opts=Fzf.fetch_options(**opts),
             encoding=encoding,
             encoding_errors=encoding_errors,
         )
 
     @ensure_stdin_available
-    def add_lines(self, lines: typing.Iterable, flush_last: bool = True):
+    def add_lines(self, lines: typing.Iterable[str], flush_last: bool = True):
         for line in lines:
             if not self.to_stdin(
                 data=line.encode(**self.encoding_options) + b"\n", flush=not flush_last
             ):
                 return
 
         if flush_last:
             self.to_stdin(flush=True)
 
+    @property
+    def is_alive(self):
+        return self.process.poll() is None
+
     def close(self):
         try:
             if not self.process.stdin.closed:
                 self.process.stdin.close()
         except OSError:
             pass
 
-    def to_stdin(self, data=None, flush=True):
+    def to_stdin(self, data: typing.Optional[typing.AnyStr] = None, flush: bool = True):
         try:
             if data is not None:
                 self.process.stdin.write(data)
             if flush:
                 self.process.stdin.flush()
-        except BrokenPipeError:
+
+        except (BrokenPipeError, OSError):
             return False
 
         return True
 
     @ensure_stdin_available
-    def pipe_from_stream(self, stream, flush_last: bool = True):
+    def pipe_from_stream(
+        self, stream: typing.IO[typing.AnyStr], flush_last: bool = True
+    ):
         for line in stream:
             if not self.to_stdin(line, flush=not flush_last):
                 return
 
         if flush_last:
             self.to_stdin(flush=True)
 
@@ -102,36 +129,46 @@
         return self
 
     def __exit__(self, *_):
         self.close()
 
 
 def fzf_prompt(
-    components,
-    processor=None,
-    escape_output=True,
-    encoding="utf-8",
-    encoding_errors="strict",
-    flush_last=False,
+    components: typing.Iterable[T],
+    processor: typing.Optional[typing.Callable[[T], str]] = None,
+    escape_output: bool = True,
+    encoding: str = "utf-8",
+    encoding_errors: str = "strict",
+    duplication_treatment: typing.Callable[[str], str] = lambda value: value + "*",
+    flush_last: bool = False,
+    *,
+    executable=EXECUTABLE,
     **opts
-):
+) -> typing.Union[T, typing.List[T]]:
     with Fzf.load_with_options(
-        encoding=encoding, encoding_errors=encoding_errors, **opts
+        executable=executable,
+        encoding=encoding,
+        encoding_errors=encoding_errors,
+        **opts
     ) as fzf:
         if escape_output:
-            output_escape = lambda value: repr(value)[1:-1]
+            output_escape = lambda value: repr(value)[
+                1:-1
+            ]  # type: typing.Callable[[str], str]
         else:
-            output_escape = lambda value: value
+            output_escape = lambda value: value  # type: typing.Callable[[str], str]
 
         if processor:
             shallow_copy = {}
 
-            def raw_process_save(value, processed_value):
+            def raw_process_save(value: str, processed_value: str):
                 if processed_value in shallow_copy:
-                    return raw_process_save(value, processed_value + "*")
+                    return raw_process_save(
+                        value, duplication_treatment(processed_value)
+                    )
 
                 shallow_copy.update(
                     {
                         processed_value: value,
                     }
                 )
                 return processed_value
@@ -152,10 +189,10 @@
             return [shallow_copy[value] for value in output]
 
         return shallow_copy[output]
 
     return output
 
 
-def get_fzf_version():
-    with Fzf(["--version"]) as fzf:
+def get_fzf_version(executable=EXECUTABLE):
+    with Fzf(executable, ["--version"]) as fzf:
         return fzf.get_output()
```

