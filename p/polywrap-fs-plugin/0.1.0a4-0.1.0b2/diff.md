# Comparing `tmp/polywrap_fs_plugin-0.1.0a4.tar.gz` & `tmp/polywrap_fs_plugin-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_fs_plugin-0.1.0a4.tar", max compression
+gzip compressed data, was "polywrap_fs_plugin-0.1.0b2.tar", max compression
```

## Comparing `polywrap_fs_plugin-0.1.0a4.tar` & `polywrap_fs_plugin-0.1.0b2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1002 2023-06-28 18:33:02.542686 polywrap_fs_plugin-0.1.0a4/README.md
--rw-r--r--   0        0        0     3816 2023-06-28 18:33:02.542686 polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:02.542686 polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/py.typed
--rw-r--r--   0        0        0      163 2023-06-28 18:33:22.198920 polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/__init__.py
--rw-r--r--   0        0        0     2771 2023-06-28 18:33:22.198920 polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/module.py
--rw-r--r--   0        0        0     1186 2023-06-28 18:33:22.198920 polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/types.py
--rw-r--r--   0        0        0     7225 2023-06-28 18:33:22.198920 polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/wrap_info.py
--rw-r--r--   0        0        0     1430 2023-06-28 18:33:02.542686 polywrap_fs_plugin-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-29 08:59:38.308066 polywrap_fs_plugin-0.1.0b2/README.md
+-rw-r--r--   0        0        0     3768 2023-07-29 16:10:14.336638 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 08:59:38.307747 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/py.typed
+-rw-r--r--   0        0        0      163 2023-08-02 15:42:01.043847 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/__init__.py
+-rw-r--r--   0        0        0     2771 2023-08-02 15:42:01.043985 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/module.py
+-rw-r--r--   0        0        0     1186 2023-08-02 15:42:01.044066 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/types.py
+-rw-r--r--   0        0        0     7225 2023-08-02 15:42:01.044177 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1511 2023-08-02 15:41:49.405508 polywrap_fs_plugin-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0b2/setup.py
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_fs_plugin-0.1.0a4/README.md` & `polywrap_fs_plugin-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/__init__.py` & `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 
 from .wrap import *
 
 
 class FileSystemPlugin(Module[None]):
     """Defines the Filesystem plugin."""
 
-    def read_file(
-        self, args: ArgsReadFile, client: InvokerClient, env: None
-    ) -> bytes:
-        """Read a file from the filesystem and return its contents as bytes. """
+    def read_file(self, args: ArgsReadFile, client: InvokerClient, env: None) -> bytes:
+        """Read a file from the filesystem and return its contents as bytes."""
         with open(args["path"], "rb") as f:
             return f.read()
 
     def read_file_as_string(
         self,
         args: ArgsReadFileAsString,
         client: InvokerClient,
@@ -50,66 +48,57 @@
         if encoding == "BASE64URL":
             return base64.urlsafe_b64encode(content).decode("ascii").rstrip("=")
         if encoding == "HEX":
             return content.hex()
 
         raise ValueError(f"Unsupported encoding: {encoding}")
 
-    def exists(
-        self, args: ArgsExists, client: InvokerClient, env: None
-    ) -> bool:
+    def exists(self, args: ArgsExists, client: InvokerClient, env: None) -> bool:
         """Check if a file or directory exists."""
         return os.path.exists(args["path"])
 
-    def write_file(
-        self, args: ArgsWriteFile, client: InvokerClient, env: None
-    ) -> bool:
+    def write_file(self, args: ArgsWriteFile, client: InvokerClient, env: None) -> bool:
         """Write data to a file on the filesystem."""
         with open(args["path"], "wb") as f:
             f.write(args["data"])
         return True
 
-
     def mkdir(self, args: ArgsMkdir, client: InvokerClient, env: None):
         """Create directories on the filesystem."""
         path = args["path"]
         if args.get("recursive", False):
             os.makedirs(path, exist_ok=True)
         else:
             parent_dir = os.path.dirname(path)
             if not os.path.exists(parent_dir):
-                raise FileNotFoundError(f"Parent directory does not exist: {parent_dir}")
+                raise FileNotFoundError(
+                    f"Parent directory does not exist: {parent_dir}"
+                )
             os.mkdir(path)
 
-
-    def rm(
-        self, args: ArgsRm, client: InvokerClient, env: None
-    ) -> bool:
+    def rm(self, args: ArgsRm, client: InvokerClient, env: None) -> bool:
         """Remove a file or directory from the filesystem."""
         if os.path.isdir(args["path"]):
             if args.get("force", False) and args.get("recursive", False):
+
                 def force_remove(action: Any, name: str, exc: Exception) -> None:
                     os.chmod(name, stat.S_IWRITE)
                     os.remove(name)
 
                 shutil.rmtree(args["path"], onerror=force_remove)
             elif args.get("recursive", False):
                 shutil.rmtree(args["path"])
             else:
                 os.rmdir(args["path"])
         else:
             os.remove(args["path"])
         return True
 
-    def rmdir(
-        self, args: ArgsRmdir, client: InvokerClient, env: None
-    ) -> bool:
+    def rmdir(self, args: ArgsRmdir, client: InvokerClient, env: None) -> bool:
         """Remove an empty directory from the filesystem."""
         os.rmdir(args["path"])
         return True
 
 
 def file_system_plugin() -> PluginPackage[None]:
     """Create a Polywrap plugin instance for interacting with EVM networks."""
-    return PluginPackage(
-        module=FileSystemPlugin(None), manifest=manifest
-    )
+    return PluginPackage(module=FileSystemPlugin(None), manifest=manifest)
```

### Comparing `polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/module.py` & `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/types.py` & `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0a4/polywrap_fs_plugin/wrap/wrap_info.py` & `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0a4/pyproject.toml` & `polywrap_fs_plugin-0.1.0b2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-fs-plugin"
-version = "0.1.0a4"
+version = "0.1.0b2"
 description = ""
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_fs_plugin"}]
 include = ["polywrap_fs_plugin/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-plugin = "0.1.0a35"
-polywrap-core = "0.1.0a35"
-polywrap-msgpack = "0.1.0a35"
-polywrap-manifest = "0.1.0a35"
+polywrap-plugin = "^0.1.0b2"
+polywrap-core = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b2"
+polywrap-manifest = "^0.1.0b2"
 
 [tool.poetry.group.dev.dependencies]
-polywrap-client = "0.1.0a35"
+polywrap-client = {path = "../../polywrap-client", develop = true}
+polywrap-uri-resolvers = {path = "../../polywrap-uri-resolvers", develop = true}
+polywrap-client-config-builder = {path = "../../polywrap-client-config-builder", develop = true}
 black = "^23.1.0"
 pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
 isort = "^5.12.0"
 bandit = "^1.7.4"
 pyright = "^1.1.296"
 pylint = "^2.16.3"
-polywrap-uri-resolvers = "0.1.0a35"
-polywrap-client-config-builder = "0.1.0a35"
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 pytest-mock = "^3.10.0"
 pydocstyle = "^6.3.0"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
-exclude = [
-    "polywrap_fs_plugin/wrap"
-]
+exclude = "polywrap_fs_plugin/wrap/*"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportShadowedImports = false
 exclude = [
     "**/wrap/"
 ]
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
 
 [tool.pylint]
 disable = [
     "too-many-return-statements",
```

### Comparing `polywrap_fs_plugin-0.1.0a4/PKG-INFO` & `polywrap_fs_plugin-0.1.0b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: polywrap-fs-plugin
-Version: 0.1.0a4
+Version: 0.1.0b2
 Summary: 
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (==0.1.0a35)
-Requires-Dist: polywrap-manifest (==0.1.0a35)
-Requires-Dist: polywrap-msgpack (==0.1.0a35)
-Requires-Dist: polywrap-plugin (==0.1.0a35)
+Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-plugin (>=0.1.0b2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-fs-plugin
 
 The Filesystem plugin enables wraps running within the Polywrap client to interact with the local filesystem.
 
 ## Interface
```

