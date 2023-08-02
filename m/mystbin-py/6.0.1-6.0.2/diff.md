# Comparing `tmp/mystbin_py-6.0.1.tar.gz` & `tmp/mystbin_py-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystbin_py-6.0.1.tar", max compression
+gzip compressed data, was "mystbin_py-6.0.2.tar", max compression
```

## Comparing `mystbin_py-6.0.1.tar` & `mystbin_py-6.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1063 2023-07-21 11:45:52.554451 mystbin_py-6.0.1/LICENSE
--rwxr-xr-x   0        0        0     2886 2023-07-25 03:47:26.738429 mystbin_py-6.0.1/README.md
--rwxr-xr-x   0        0        0     1547 2023-07-25 03:53:45.475988 mystbin_py-6.0.1/mystbin/__init__.py
--rwxr-xr-x   0        0        0     6403 2023-07-25 03:47:11.270202 mystbin_py-6.0.1/mystbin/client.py
--rwxr-xr-x   0        0        0     1738 2023-07-21 11:50:11.686218 mystbin_py-6.0.1/mystbin/errors.py
--rwxr-xr-x   0        0        0    10885 2023-07-23 18:21:32.231992 mystbin_py-6.0.1/mystbin/http.py
--rwxr-xr-x   0        0        0     4787 2023-07-25 03:45:21.648593 mystbin_py-6.0.1/mystbin/paste.py
--rwxr-xr-x   0        0        0        0 2023-07-21 11:45:52.554451 mystbin_py-6.0.1/mystbin/py.typed
--rwxr-xr-x   0        0        0     1149 2023-07-21 11:45:52.554451 mystbin_py-6.0.1/mystbin/types/__init__.py
--rwxr-xr-x   0        0        0     1689 2023-07-25 03:42:26.222018 mystbin_py-6.0.1/mystbin/types/responses.py
--rwxr-xr-x   0        0        0     2263 2023-07-21 11:45:52.558451 mystbin_py-6.0.1/mystbin/utils.py
--rwxr-xr-x   0        0        0     2147 2023-07-25 03:53:34.339825 mystbin_py-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 mystbin_py-6.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1063 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/LICENSE
+-rwxr-xr-x   0        0        0     2886 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/README.md
+-rwxr-xr-x   0        0        0     1547 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/__init__.py
+-rwxr-xr-x   0        0        0     7111 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/client.py
+-rwxr-xr-x   0        0        0     1738 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/errors.py
+-rwxr-xr-x   0        0        0    10885 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/http.py
+-rwxr-xr-x   0        0        0     4798 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/paste.py
+-rwxr-xr-x   0        0        0        0 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/py.typed
+-rwxr-xr-x   0        0        0     1149 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/types/__init__.py
+-rwxr-xr-x   0        0        0     1773 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/types/responses.py
+-rwxr-xr-x   0        0        0     2263 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/mystbin/utils.py
+-rwxr-xr-x   0        0        0     2160 2023-08-02 18:59:28.173666 mystbin_py-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 mystbin_py-6.0.2/PKG-INFO
```

### Comparing `mystbin_py-6.0.1/LICENSE` & `mystbin_py-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.1/README.md` & `mystbin_py-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.1/mystbin/__init__.py` & `mystbin_py-6.0.2/mystbin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=6, minor=0, micro=1, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=6, minor=0, micro=2, releaselevel="final", serial=0)
```

### Comparing `mystbin_py-6.0.1/mystbin/client.py` & `mystbin_py-6.0.2/mystbin/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 import datetime
-from typing import List, Optional, Sequence, overload
+from typing import List, Literal, Optional, Sequence, Union, overload
 
 import aiohttp
 
 from .http import HTTPClient
 from .paste import File, Paste
 from .utils import require_authentication
 
@@ -170,27 +170,47 @@
         Parameters
         -----------
         paste_ids: List[:class:`str`]
             The pastes to delete.
         """
         await self.http.delete_pastes(paste_ids=paste_ids)
 
-    async def get_paste(self, paste_id: str, *, password: Optional[str] = None) -> Paste:
+    @overload
+    async def get_paste(self, paste_id: str, *, password: Optional[str] = ..., raw: Literal[False]) -> Paste:
+        ...
+
+    @overload
+    async def get_paste(self, paste_id: str, *, password: Optional[str] = ..., raw: Literal[True]) -> list[str]:
+        ...
+
+    async def get_paste(
+        self, paste_id: str, *, password: Optional[str] = None, raw: bool = False
+    ) -> Union[Paste, list[str]]:
         """|coro|
 
         Fetch a paste.
 
         Parameters
         -----------
         paste_id: :class:`str`
             The paste id to fetch.
         password: Optional[:class:`str`]
             The password of the paste, if any.
+        raw: :class:`bool`
+            Whether to return the raw file(s) content or a :class:`~mystbin.Paste` instance.
+            Defaults to ``False``.
+
+        Returns
+        --------
+        Union[:class:`~mystbin.Paste`, List[:class:`str`]]
+            The paste data returned.
         """
         data = await self.http.get_paste(paste_id=paste_id, password=password)
+        if raw:
+            return [item["content"] for item in data["files"]]
         return Paste.from_data(data)
 
     @require_authentication
     async def get_user_pastes(self, *, limit: int = 100) -> List[Paste]:
         """|coro|
 
         Get all pastes belonging to the current authenticated user.
```

### Comparing `mystbin_py-6.0.1/mystbin/errors.py` & `mystbin_py-6.0.2/mystbin/errors.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.1/mystbin/http.py` & `mystbin_py-6.0.2/mystbin/http.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.1/mystbin/paste.py` & `mystbin_py-6.0.2/mystbin/paste.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         "filename",
         "content",
         "attachment_url",
         "_lines_of_code",
         "_character_count",
     )
 
-    def __init__(self, *, filename: str, content: str, attachment_url: Optional[str]) -> None:
+    def __init__(self, *, filename: str, content: str, attachment_url: Optional[str] = None) -> None:
         self.filename: str = filename
         self.content: str = content
         self.attachment_url: Optional[str] = attachment_url
 
     @property
     def lines_of_code(self) -> int:
         return self._lines_of_code
@@ -143,15 +143,15 @@
         return self._views
 
     @classmethod
     def from_data(cls, payload: PasteResponse, /) -> Self:
         files = [File.from_data(data) for data in payload["files"]]
         self = cls(id=payload["id"], created_at=payload["created_at"], files=files, notice=payload["notice"])
         self._views = payload.get("views")
-        last_edited = payload["last_edited"]
+        last_edited = payload.get("last_edited")
         if last_edited:
             self._last_edited = datetime.datetime.fromisoformat(last_edited)
         else:
             self._last_edited = None
 
         expires = payload["expires"]
         if expires:
```

### Comparing `mystbin_py-6.0.1/mystbin/types/__init__.py` & `mystbin_py-6.0.2/mystbin/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.1/mystbin/types/responses.py` & `mystbin_py-6.0.2/mystbin/types/responses.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import List, Optional, TypedDict
+from typing import TYPE_CHECKING, List, Optional, TypedDict
+
+
+if TYPE_CHECKING:
+    from typing_extensions import NotRequired
 
 
 __all__ = (
     "FileResponse",
     "PasteResponse",
 )
 
@@ -41,15 +45,15 @@
 
 
 class PasteResponse(TypedDict):
     id: str
     author_id: Optional[int]
     created_at: str
     expires: Optional[str]
-    last_edited: Optional[str]
+    last_edited: NotRequired[str]
     files: List[FileResponse]
     notice: Optional[str]
 
 
 class EditPasteResponse(TypedDict):
     id: str
     expires: Optional[datetime]
```

### Comparing `mystbin_py-6.0.1/mystbin/utils.py` & `mystbin_py-6.0.2/mystbin/utils.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.1/pyproject.toml` & `mystbin_py-6.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 [tool.poetry]
 name = "mystbin-py"
-version = "6.0.1"
+version = "6.0.2"
 description = "A small simple wrapper around the mystb.in API."
-authors = ["AbstractUmbra <Umbra@AbstractUmbra.dev>"]
+authors = ["AbstractUmbra <umbra@abstractumbra.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/PythonistaGuild/mystbin.py"
 repository = "https://github.com/PythonistaGuild/mystbin.py"
-keywords = ["mystbin",  "paste"]
+keywords = ["mystbin", "paste"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
-include = [
-    "LICENSE"
-]
+include = ["LICENSE"]
 packages = [
     { include = "mystbin" },
     { include = "mystbin/**/*.py" },
-    { include = "mystbin/py.typed" }
+    { include = "mystbin/py.typed" },
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/PythonistaGuild/mystbin.py/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = [
     { version = "^3.8" },
-    { version = "^3.8", markers = "extra == 'speed'", extras= ["speedups"]},
+    { version = "^3.8", markers = "extra == 'speed'", extras = [
+        "speedups",
+    ] },
 ]
 
 sphinx = { version = "^4.0.0", optional = true }
 sphinxcontrib-trio = { version = "*", optional = true }
 furo = { version = "*", optional = true }
-pytz = { version = "*", optional = true, python="<3.9" }
+pytz = { version = "*", optional = true, python = "<3.9" }
 
 [tool.poetry.extras]
 speed = ["aiohttp"]
 docs = ["sphinx", "sphinxcontrib-trio", "furo"]
 
 [tool.poetry.group.speedups.dependencies]
 aiohttp = { version = "^3.8", extras = ["speedups"] }
```

### Comparing `mystbin_py-6.0.1/PKG-INFO` & `mystbin_py-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mystbin-py
-Version: 6.0.1
+Version: 6.0.2
 Summary: A small simple wrapper around the mystb.in API.
 Home-page: https://github.com/PythonistaGuild/mystbin.py
 License: MIT
 Keywords: mystbin,paste
 Author: AbstractUmbra
-Author-email: Umbra@AbstractUmbra.dev
+Author-email: umbra@abstractumbra.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: mystbin-py Version: 6.0.1 Summary: A small simple
+Metadata-Version: 2.1 Name: mystbin-py Version: 6.0.2 Summary: A small simple
 wrapper around the mystb.in API. Home-page: https://github.com/PythonistaGuild/
 mystbin.py License: MIT Keywords: mystbin,paste Author: AbstractUmbra Author-
-email: Umbra@AbstractUmbra.dev Requires-Python: >=3.8,<4.0 Classifier: Intended
+email: umbra@abstractumbra.dev Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Internet
 Classifier: Typing :: Typed Provides-Extra: docs Provides-Extra: speed
```

