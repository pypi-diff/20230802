# Comparing `tmp/ansys_pyensight_core-0.5.2.tar.gz` & `tmp/ansys_pyensight_core-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_pyensight_core-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_pyensight_core-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_pyensight_core-0.5.2.tar` & `ansys_pyensight_core-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1089 2023-07-28 07:49:26.590352 ansys_pyensight_core-0.5.2/LICENSE
--rw-r--r--   0        0        0     8121 2023-07-28 07:49:26.590352 ansys_pyensight_core-0.5.2/README.rst
--rw-r--r--   0        0        0     3976 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      828 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/__init__.py
--rw-r--r--   0        0        0     3351 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/deep_pixel_view.html
--rw-r--r--   0        0        0    24888 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/dockerlauncher.py
--rw-r--r--   0        0        0    11803 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/enscontext.py
--rw-r--r--   0        0        0    14948 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/enshell_grpc.py
--rw-r--r--   0        0        0    14343 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/ensight_grpc.py
--rw-r--r--   0        0        0    17343 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/ensobj.py
--rw-r--r--   0        0        0     5900 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/launch_ensight.py
--rw-r--r--   0        0        0     8957 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/launcher.py
--rw-r--r--   0        0        0     7640 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/listobj.py
--rw-r--r--   0        0        0    13908 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/locallauncher.py
--rw-r--r--   0        0        0        0 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/py.typed
--rw-r--r--   0        0        0    26241 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/renderable.py
--rw-r--r--   0        0        0    58977 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/session.py
--rw-r--r--   0        0        0      752 2023-07-28 07:49:26.622373 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/sgeo_poll.html
--rw-r--r--   0        0        0        0 2023-07-28 07:49:26.626376 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/__init__.py
--rw-r--r--   0        0        0    17657 2023-07-28 07:49:26.626376 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/export.py
--rw-r--r--   0        0        0     3986 2023-07-28 07:49:26.626376 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/parts.py
--rw-r--r--   0        0        0    19035 2023-07-28 07:49:26.626376 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/query.py
--rw-r--r--   0        0        0     2397 2023-07-28 07:49:26.626376 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/support.py
--rw-r--r--   0        0        0    12285 2023-07-28 07:49:26.626376 ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/views.py
--rw-r--r--   0        0        0    10831 1970-01-01 00:00:00.000000 ansys_pyensight_core-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-08-02 11:32:59.552857 ansys_pyensight_core-0.5.3/LICENSE
+-rw-r--r--   0        0        0     8121 2023-08-02 11:32:59.552857 ansys_pyensight_core-0.5.3/README.rst
+-rw-r--r--   0        0        0     4108 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      828 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/__init__.py
+-rw-r--r--   0        0        0     3351 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/deep_pixel_view.html
+-rw-r--r--   0        0        0    24888 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/dockerlauncher.py
+-rw-r--r--   0        0        0    11803 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/enscontext.py
+-rw-r--r--   0        0        0    14948 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/enshell_grpc.py
+-rw-r--r--   0        0        0    14343 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/ensight_grpc.py
+-rw-r--r--   0        0        0    17346 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/ensobj.py
+-rw-r--r--   0        0        0     5900 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/launch_ensight.py
+-rw-r--r--   0        0        0     8957 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/launcher.py
+-rw-r--r--   0        0        0     7640 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/listobj.py
+-rw-r--r--   0        0        0    13908 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/locallauncher.py
+-rw-r--r--   0        0        0        0 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/py.typed
+-rw-r--r--   0        0        0    26860 2023-08-02 11:32:59.588858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/renderable.py
+-rw-r--r--   0        0        0    59230 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/session.py
+-rw-r--r--   0        0        0      752 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/sgeo_poll.html
+-rw-r--r--   0        0        0        0 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/__init__.py
+-rw-r--r--   0        0        0    17648 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/export.py
+-rw-r--r--   0        0        0     3986 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/parts.py
+-rw-r--r--   0        0        0    19035 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/query.py
+-rw-r--r--   0        0        0     2397 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/support.py
+-rw-r--r--   0        0        0    12209 2023-08-02 11:32:59.592858 ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/views.py
+-rw-r--r--   0        0        0    10831 1970-01-01 00:00:00.000000 ansys_pyensight_core-0.5.3/PKG-INFO
```

### Comparing `ansys_pyensight_core-0.5.2/LICENSE` & `ansys_pyensight_core-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/README.rst` & `ansys_pyensight_core-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/pyproject.toml` & `ansys_pyensight_core-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "flit_core>=3.2,<4"
 ]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-pyensight-core"
-version = "0.5.2"
+version = "0.5.3"
 description = "A python wrapper for Ansys EnSight"
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
     "importlib-metadata>=4.0,<5; python_version<='3.8'",
-    "ansys-api-pyensight==0.2.2",
+    "ansys-api-pyensight==0.3.0",
     "requests>=2.28.2",
     "pyansys-docker>=5.0.4",
     "urllib3<2",
     "typing>=3.7.4.3",
     "typing-extensions>=4.5.0",
     "numpy>=1.21.0",
     "Pillow>=9.3.0"
@@ -87,15 +87,19 @@
     "pragma: no cover",
     "def __repr__",
     "if selfdebug",
     "raise AssertionError",
     "raise NotImplementedError",
     "if 0:",
     "if __name__ == .__main__.:",
-    "@(abc.)?abstractmethod"]
+    "@(abc.)?abstractmethod",
+    "if TYPE_CHECKING:",
+    "def _repr_pretty_",
+    "self._pim_instance",
+    "self._pim_file_service"]
 
 ignore_errors = true
 show_missing = true
 
 [tool.coverage.html]
 show_contexts = true
 
@@ -104,15 +108,15 @@
 src_paths = ["src/ansys", "doc"]
 
 [tool.pytest.ini_options]
 minversion = "7.1"
 testpaths = [
     "tests",
 ]
-addopts = "--setup-show --cov=ansys.pyensight.core --cov-report html:coverage-html --cov-report term --cov-config=.coveragerc --capture=tee-sys --tb=native -p no:warnings"
+addopts = "--setup-show --cov=ansys.pyensight.core --cov=ansys.api.pyensight --cov-report html:coverage-html --cov-report term --cov-config=.coveragerc --capture=tee-sys --tb=native -p no:warnings"
 markers =[
     "integration:Run integration tests",
     "smoke:Run the smoke tests",
     "unit:Run the unit tests",
     ]
 norecursedirs = ".git .idea"
 filterwarnings = "ignore:.+:DeprecationWarning"
```

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/__init__.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/deep_pixel_view.html` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/deep_pixel_view.html`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/dockerlauncher.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/dockerlauncher.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/enscontext.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/enscontext.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/enshell_grpc.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/enshell_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/ensight_grpc.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/ensight_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/ensobj.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/ensobj.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,25 +102,25 @@
             attributes.  Otherwise, the returned dictionary will include values for
             all attributes of the target object.
         text : int
             By default, the returned dictionary keys are the attribute ID enum
             values.  If text is set to 1, the dictionary keys will be strings.
             Return:
 
-        Example
+        Returns
         -------
+            Session CMD.
+
+        Examples
+        --------
         To copy some attributes from one part to another.
 
         >>> tmp = part0.getattrs(["VISIBLE", session.ensight.objs.enums.OPAQUENESS])
         >>> part1.setattrs(tmp)
 
-        Returns
-        -------
-            Session CMD.
-
         """
         if attrid is None:
             cmd = f"{self._remote_obj()}.getattrs(text={text})"
         else:
             cmd = f"{self._remote_obj()}.getattrs({attrid.__repr__()},text={text})"
         return self._session.cmd(cmd)
 
@@ -130,24 +130,25 @@
         Parameters
         ----------
         attrid : Any
             The attribute to set.  This can be an integer (enum) or string.
         value : Any
             The value to set the attribute to.
 
+        Returns
+        -------
+            Session CMD.
+
         Examples
         --------
         These commands are equivalent
 
         >>> part.setattr("VISIBLE", True)
         >>> part.getattr(session.ensight.objs.enums.VISIBLE, True)
 
-        Returns
-        -------
-            Session CMD.
         """
         return self._session.cmd(
             f"{self._remote_obj()}.setattr({attrid.__repr__()}, {value.__repr__()})"
         )
 
     def setattrs(self, values: dict, all_errors: int = 0) -> None:
         """Set the values of a collection of attributes
@@ -218,15 +219,15 @@
 
         """
         if not attrid:
             return self._session.cmd(f"{self._remote_obj()}.attrinfo()")
         return self._session.cmd(f"{self._remote_obj()}.attrinfo({attrid.__repr__()})")
 
     def populate_attr_list(self) -> List[str]:
-        """populates a list with attributes.
+        """Populates a list with attributes.
 
         Returns
         -------
         List[str]
             The list with the attributes.
         """
         return [k for k, _ in self.attrinfo().items()]
```

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/launch_ensight.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/launch_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/launcher.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/listobj.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/listobj.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/locallauncher.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/locallauncher.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/renderable.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/renderable.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,14 +496,29 @@
         url = f"http://{self._session.hostname}:{self._session.html_port}"
         url += "/ansys/nexus/novnc/vnc_envision.html"
         url += f"?autoconnect=true&host={self._session.hostname}&port={self._session.ws_port}"
         self._url = url
         super().update()
 
 
+# Undocumented class
+class RenderableVNCAngular(Renderable):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self._rendertype = "remote"
+        self.update()
+
+    def update(self):
+        url = f"http://{self._session.hostname}:{self._session.html_port}"
+        url += "/ansys/nexus/angular/viewer_angular_pyensight.html"
+        url += f"?autoconnect=true&host={self._session.hostname}&port={self._session.ws_port}&secretKey={self._session.secret_key}"
+        self._url = url
+        super().update()
+
+
 class RenderableEVSN(Renderable):
     """Generates a URL that can be used to connect to the EnVision VNC remote image renderer."""
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._rendertype = "remote_scene"
         self._generate_url()
@@ -557,18 +572,18 @@
         attributes += f"renderer_options='{{ {http_uri}, {ws_uri}, {secrets} }}'"
         html += f"<ansys-nexus-viewer {attributes}></ansys-nexus-viewer>\n"
         # refresh the remote HTML
         self._save_remote_html_page(html)
         super().update()
 
 
-class RenderableSGEO(Renderable):
+class RenderableSGEO(Renderable):  # pragma: no cover
     """Generates a WebGL-based renderable that leverages the SGEO format/viewer interface for progressive geometry transport."""
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs) -> None:  # pragma: no cover
         super().__init__(*args, **kwargs)
         self._generate_url()
         pathname, filename = self._generate_filename("")
         # on the server, a JSON block can be accessed via:
         # {_sgeo_base_pathname}/geometry.sgeo
         # and the update files:
         # {_sgeo_base_pathname}/{names}.bin
@@ -579,15 +594,15 @@
         self._session.cmd(cmd, do_eval=False)
         # get a stream ID
         self._stream_id = self._session.ensight.dsg_new_stream(sgeo=1)
         #
         self._revision = 0
         self.update()
 
-    def update(self):
+    def update(self):  # pragma: no cover
         """Generate a SGEO geometry file.
 
         This method causes the EnSight session to generate an updated geometry SGEO
         file and content and then display the results in any attached WebGL viewer.
 
         If the renderable is part of a Jupyter notebook cell, that cell is updated as an
         iframe reference.
```

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/session.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ansys.pyensight.core.renderable import (
     RenderableDeepPixel,
     RenderableEVSN,
     RenderableImage,
     RenderableMP4,
     RenderableSGEO,
     RenderableVNC,
+    RenderableVNCAngular,
     RenderableWebGL,
 )
 import requests
 
 if TYPE_CHECKING:
     from ansys.api.pyensight import ensight_api
     from ansys.pyensight.core import enscontext, ensight_grpc, renderable
@@ -63,15 +64,15 @@
     enable the :func:`show<ansys.pyensight.core.Session.show>`) method, also require that
     an instance of the websocket server is running.
 
     Parameters
     ----------
     host : str, optional
         Name of the host that the EnSight gRPC service is running on.
-        The default is``"127.0.0.1"``, which is the localhost.
+        The default is ``"127.0.0.1"``, which is the localhost.
     install_path : str, optional
         Path to the CEI directory to launch EnSight from.
         The default is ``None``.
     secret_key : str, optional
         Shared session secret key for validating the gRPC communication.
         The default is ``""``.
     grpc_port : int, optional
@@ -435,15 +436,16 @@
         )
 
         self.cmd(remote_functions, do_eval=False)
 
         out = []
         dirlen = 0
         if localdir:
-            dirlen = len(localdir)
+            # we use dirlen + 1 here to remove the '/' inserted by os.path.join()
+            dirlen = len(localdir) + 1
         for item in filelist:
             try:
                 name = os.path.join(localdir, item)
                 if os.path.isfile(name):
                     out.append((name[dirlen:], os.stat(name).st_size))
                 else:
                     for root, _, files in os.walk(name):
@@ -821,14 +823,17 @@
                 render = RenderableWebGL(self, **kwargs)
             else:
                 render = RenderableSGEO(self, **kwargs)
         elif what == "remote":
             render = RenderableVNC(self, **kwargs)
         elif what == "remote_scene":
             render = RenderableEVSN(self, **kwargs)
+        # Undocumented. Available only internally
+        elif what == "webensight":
+            render = RenderableVNCAngular(self, **kwargs)
 
         if render is None:
             raise RuntimeError("Unable to generate requested visualization")
 
         return render
 
     def cmd(self, value: str, do_eval: bool = True) -> Any:
@@ -1173,24 +1178,22 @@
             Whether to call only the last event if a repeated event is generated
             as a result of an action. The default is ``True``. If ``False``, every
             event results in a callback.
 
         Examples
         --------
         A string like this is printed when the dataset is loaded and the part list
-        changes::
-
-        Event :
-            grpc://f6f74dae-f0ed-11ec-aa58-381428170733/partlist?enum=PARTS&uid=221'
+        changes:
 
+        ``    Event : grpc://f6f74dae-f0ed-11ec-aa58-381428170733/partlist?enum=PARTS&uid=221``
 
         >>> from ansys.pyensight.core import LocalLauncher
         >>> s = LocalLauncher().start()
         >>> def cb(v: str):
-        >>> print("Event:", v)
+        >>>     print("Event:", v)
         >>>     s.add_callback("ensight.objs.core", "partlist", ["PARTS"], cb)
         >>> s.load_data(r"D:\ANSYSDev\data\CFX\HeatingCoil_001.res")
         """
         self._establish_connection()
         # shorten the tag up to the query block. Macros are only legal in the query block.
         try:
             idx = tag.index("?")
```

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/sgeo_poll.html` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/sgeo_poll.html`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/export.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import uuid
 
 from PIL import Image
 import numpy
 
 try:
     import ensight
+    import enve
 except ImportError:
     from ansys.api.pyensight import ensight_api
 
 
 class Export:
     """Provides the ``ensight.utils.export`` interface.
 
@@ -214,16 +215,14 @@
         -------
         dict
             Dictionary of the various channels.
         """
         if not raytrace:
             img = ensight.render(x=width, y=height, num_samples=passes, enhanced=enhanced)
         else:
-            import enve
-
             with tempfile.TemporaryDirectory() as tmpdirname:
                 tmpfilename = os.path.join(tmpdirname, str(uuid.uuid1()))
                 ensight.file.image_format("png")
                 ensight.file.image_file(tmpfilename)
                 ensight.file.image_window_size("user_defined")
                 ensight.file.image_window_xy(width, height)
                 ensight.file.image_rend_offscreen("ON")
```

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/parts.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/parts.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/query.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/query.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/support.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/support.py`

 * *Files identical despite different names*

### Comparing `ansys_pyensight_core-0.5.2/src/ansys/pyensight/core/utils/views.py` & `ansys_pyensight_core-0.5.3/src/ansys/pyensight/core/utils/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,22 +157,19 @@
         tuple
             Four quaternions describing the rotation.
 
         """
         trace = row0[0] + row1[1] + row2[2]
         if trace > 0:
             s = math.sqrt(trace + 1)
-            print(s)
             qw = s / 2
             s = 1 / (2 * s)
-            print(s)
             qx = (row2[1] - row1[2]) * s
             qy = (row0[2] - row2[0]) * s
             qz = (row1[0] - row0[1]) * s
-            print(qx, qy, qz, qw)
         elif row0[0] > row1[1] and row0[0] > row2[2]:
             s = math.sqrt(1 + row0[0] - row1[1] - row2[2])
             qx = s / 2
             s = 1 / (2 * s)
             qw = (row2[1] - row1[2]) * s
             qy = (row0[1] + row1[0]) * s
             qz = (row0[2] + row2[0]) * s
```

### Comparing `ansys_pyensight_core-0.5.2/PKG-INFO` & `ansys_pyensight_core-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-pyensight-core
-Version: 0.5.2
+Version: 0.5.3
 Summary: A python wrapper for Ansys EnSight
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
-Requires-Dist: ansys-api-pyensight==0.2.2
+Requires-Dist: ansys-api-pyensight==0.3.0
 Requires-Dist: requests>=2.28.2
 Requires-Dist: pyansys-docker>=5.0.4
 Requires-Dist: urllib3<2
 Requires-Dist: typing>=3.7.4.3
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: Pillow>=9.3.0
```

