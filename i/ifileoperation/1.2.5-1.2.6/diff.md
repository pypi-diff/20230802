# Comparing `tmp/ifileoperation-1.2.5.tar.gz` & `tmp/ifileoperation-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifileoperation-1.2.5.tar", last modified: Thu Jul  6 00:30:45 2023, max compression
+gzip compressed data, was "ifileoperation-1.2.6.tar", last modified: Wed Aug  2 04:01:28 2023, max compression
```

## Comparing `ifileoperation-1.2.5.tar` & `ifileoperation-1.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.171008 ifileoperation-1.2.5/
--rw-rw-rw-   0        0        0     1514 2023-01-21 01:14:44.000000 ifileoperation-1.2.5/LICENSE
--rw-rw-rw-   0        0        0    10719 2023-07-06 00:30:45.171008 ifileoperation-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     9745 2023-02-06 21:24:02.000000 ifileoperation-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.142041 ifileoperation-1.2.5/ifileoperation/
--rw-rw-rw-   0        0        0      118 2023-07-06 00:19:55.000000 ifileoperation-1.2.5/ifileoperation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.163850 ifileoperation-1.2.5/ifileoperation/com/
--rw-rw-rw-   0        0        0      123 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-05-16 01:33:55.000000 ifileoperation-1.2.5/ifileoperation/com/common.py
--rw-rw-rw-   0        0        0      354 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/fileoperation.py
--rw-rw-rw-   0        0        0     9918 2023-01-24 21:26:33.000000 ifileoperation-1.2.5/ifileoperation/com/fileoperationprogresssink.py
--rw-rw-rw-   0        0        0     2168 2023-07-06 00:14:05.000000 ifileoperation-1.2.5/ifileoperation/com/filesysbinddata.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.168851 ifileoperation-1.2.5/ifileoperation/com/interfaces/
--rw-rw-rw-   0        0        0      130 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3311 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperation.py
--rw-rw-rw-   0        0        0     4293 2023-01-24 21:26:33.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperationprogresssink.py
--rw-rw-rw-   0        0        0      798 2023-01-23 23:38:57.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ifilesysbinddata.py
--rw-rw-rw-   0        0        0     1185 2023-01-24 21:26:34.000000 ifileoperation-1.2.5/ifileoperation/com/interfaces/ishellitem.py
--rw-rw-rw-   0        0        0     1903 2023-05-16 01:33:55.000000 ifileoperation-1.2.5/ifileoperation/errors.py
--rw-rw-rw-   0        0        0    11034 2023-05-16 01:45:06.000000 ifileoperation-1.2.5/ifileoperation/fileoperator.py
--rw-rw-rw-   0        0        0    12219 2023-05-16 01:33:55.000000 ifileoperation-1.2.5/ifileoperation/flags.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.159109 ifileoperation-1.2.5/ifileoperation.egg-info/
--rw-rw-rw-   0        0        0    10719 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 00:30:45.000000 ifileoperation-1.2.5/ifileoperation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1714 2023-01-24 21:00:56.000000 ifileoperation-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 00:30:45.171008 ifileoperation-1.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 00:30:45.169851 ifileoperation-1.2.5/tests/
--rw-rw-rw-   0        0        0      849 2023-05-16 01:34:17.000000 ifileoperation-1.2.5/tests/test_ifileoperation.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:01:28.335760 ifileoperation-1.2.6/
+-rw-rw-rw-   0        0        0     1514 2023-01-21 01:14:44.000000 ifileoperation-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0    10879 2023-08-02 04:01:28.335760 ifileoperation-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9903 2023-08-02 03:55:16.000000 ifileoperation-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 04:01:28.291773 ifileoperation-1.2.6/ifileoperation/
+-rw-rw-rw-   0        0        0      118 2023-08-02 03:55:16.000000 ifileoperation-1.2.6/ifileoperation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:01:28.322249 ifileoperation-1.2.6/ifileoperation/com/
+-rw-rw-rw-   0        0        0      123 2023-01-23 23:38:57.000000 ifileoperation-1.2.6/ifileoperation/com/__init__.py
+-rw-rw-rw-   0        0        0     2796 2023-08-01 21:39:30.000000 ifileoperation-1.2.6/ifileoperation/com/common.py
+-rw-rw-rw-   0        0        0      354 2023-01-23 23:38:57.000000 ifileoperation-1.2.6/ifileoperation/com/fileoperation.py
+-rw-rw-rw-   0        0        0     9918 2023-01-24 21:26:33.000000 ifileoperation-1.2.6/ifileoperation/com/fileoperationprogresssink.py
+-rw-rw-rw-   0        0        0     2835 2023-08-02 03:55:16.000000 ifileoperation-1.2.6/ifileoperation/com/filesysbinddata.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:01:28.328251 ifileoperation-1.2.6/ifileoperation/com/interfaces/
+-rw-rw-rw-   0        0        0      130 2023-01-23 23:38:57.000000 ifileoperation-1.2.6/ifileoperation/com/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-01-23 23:38:57.000000 ifileoperation-1.2.6/ifileoperation/com/interfaces/ifileoperation.py
+-rw-rw-rw-   0        0        0     4293 2023-01-24 21:26:33.000000 ifileoperation-1.2.6/ifileoperation/com/interfaces/ifileoperationprogresssink.py
+-rw-rw-rw-   0        0        0      798 2023-01-23 23:38:57.000000 ifileoperation-1.2.6/ifileoperation/com/interfaces/ifilesysbinddata.py
+-rw-rw-rw-   0        0        0     1185 2023-01-24 21:26:34.000000 ifileoperation-1.2.6/ifileoperation/com/interfaces/ishellitem.py
+-rw-rw-rw-   0        0        0     1903 2023-05-16 01:33:55.000000 ifileoperation-1.2.6/ifileoperation/errors.py
+-rw-rw-rw-   0        0        0    11409 2023-08-02 03:55:16.000000 ifileoperation-1.2.6/ifileoperation/fileoperator.py
+-rw-rw-rw-   0        0        0    12219 2023-05-16 01:33:55.000000 ifileoperation-1.2.6/ifileoperation/flags.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:01:28.316583 ifileoperation-1.2.6/ifileoperation.egg-info/
+-rw-rw-rw-   0        0        0    10879 2023-08-02 04:01:28.000000 ifileoperation-1.2.6/ifileoperation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-08-02 04:01:28.000000 ifileoperation-1.2.6/ifileoperation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:01:28.000000 ifileoperation-1.2.6/ifileoperation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-08-02 04:01:28.000000 ifileoperation-1.2.6/ifileoperation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-02 04:01:28.000000 ifileoperation-1.2.6/ifileoperation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1714 2023-01-24 21:00:56.000000 ifileoperation-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:01:28.336760 ifileoperation-1.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 04:01:28.334761 ifileoperation-1.2.6/tests/
+-rw-rw-rw-   0        0        0      849 2023-05-16 01:34:17.000000 ifileoperation-1.2.6/tests/test_ifileoperation.py
```

### Comparing `ifileoperation-1.2.5/LICENSE` & `ifileoperation-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/PKG-INFO` & `ifileoperation-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifileoperation
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python wrapper for using Win32's IFileOperation for manipulating the filesystem.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: Homepage, https://github.com/lojack5/IFileOperation
 Project-URL: Bug Tracker, https://github.com/lojack5/IFileOperation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -145,15 +145,17 @@
   the new file, without its directory.  However, if you're used to other file
   APIs that let you "rename" a file into a different directory, `rename_file`
   supports this as well.  When `allow_move` is `True`, if it is detected that
   `new_name` is actually a path resolving to a different directory, this will
   automatically be transformed into a `move_file` operation instead.
 - `rename_files(sources: Iterable[StrPath], new_name: str)`:  Renames the given
   files to have the new name.  Unlike `rename_file`, you cannot rename files
-  into files in different directories.
+  into files in different directories. If multiple source files are in the same
+  directory, you probably want to include `FileOperationFlags.RENAMEONCOLLISION` to
+  prevent errors while renaming.
 - `delete_file(source: StrPath)`: Deletes the target file.
 - `delete_files(sources: Iterable[StrPath])`: Deletes the target files.
 - `commit()`: Cause all the queue operations to be performed.
 
 ### Post-commit attributes
 After a `commit`, additional attributes are available on the `FileOperator` instance:
 - `return_code`: The `HRESULT` return code from the overall operation. This is usually
```

### Comparing `ifileoperation-1.2.5/README.md` & `ifileoperation-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,17 @@
   the new file, without its directory.  However, if you're used to other file
   APIs that let you "rename" a file into a different directory, `rename_file`
   supports this as well.  When `allow_move` is `True`, if it is detected that
   `new_name` is actually a path resolving to a different directory, this will
   automatically be transformed into a `move_file` operation instead.
 - `rename_files(sources: Iterable[StrPath], new_name: str)`:  Renames the given
   files to have the new name.  Unlike `rename_file`, you cannot rename files
-  into files in different directories.
+  into files in different directories. If multiple source files are in the same
+  directory, you probably want to include `FileOperationFlags.RENAMEONCOLLISION` to
+  prevent errors while renaming.
 - `delete_file(source: StrPath)`: Deletes the target file.
 - `delete_files(sources: Iterable[StrPath])`: Deletes the target files.
 - `commit()`: Cause all the queue operations to be performed.
 
 ### Post-commit attributes
 After a `commit`, additional attributes are available on the `FileOperator` instance:
 - `return_code`: The `HRESULT` return code from the overall operation. This is usually
```

### Comparing `ifileoperation-1.2.5/ifileoperation/com/common.py` & `ifileoperation-1.2.6/ifileoperation/com/common.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/com/fileoperationprogresssink.py` & `ifileoperation-1.2.6/ifileoperation/com/fileoperationprogresssink.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/com/filesysbinddata.py` & `ifileoperation-1.2.6/ifileoperation/com/filesysbinddata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 __all__ = [
     'FOLDER_BIND_CTX',
-    'parse_filename',
+    'filename_to_IShellItem',
+    'filenames_to_IShellItemArray',
 ]
+import os
+from collections.abc import Iterable
 from ctypes import byref
 from ctypes.wintypes import DWORD, WIN32_FIND_DATAW
-from os import PathLike, fspath
 from typing import TypeAlias
 
 import pythoncom
 import pywintypes
 from comtypes import COMObject
 from comtypes.hresult import S_OK
 from win32com.shell import shell  # type: ignore (module *does* exist)
 
 from ..flags import FileAttributeFlags
 from .common import com_ptr
 from .interfaces import IFileSysBindData
 
-StrPath: TypeAlias = str | PathLike[str]
+StrPath: TypeAlias = str | os.PathLike[str]
 
 
 class FileSysBindData(COMObject):
     """Implement the IFileSysBindData interface"""
 
     _com_interfaces_ = [IFileSysBindData]
 
@@ -46,26 +48,39 @@
 
 FOLDER_BIND_CTX = create_bind_ctx(WIN32_FIND_DATAW(DWORD(FileAttributeFlags.DIRECTORY)))
 
 
 E_FILE_NOT_FOUND = (-2147024894, -2147024893)
 
 
-def parse_filename(path: StrPath, force: bool = False):
-    """Parse a filename into an IShellItem2 instance. If `force` is True, then
-    an IShellItem2 instance will be returned even if the file does not exist.
+def filename_to_IShellItem(path: StrPath, force: bool = False):
+    """Parse a filename into an IShellItem instance. If `force` is True, then an
+    IShellItem instance will be returned even if the file does not exist.
     """
-    path = fspath(path)
+    path = os.path.abspath(os.fspath(path))
+    ctx = FOLDER_BIND_CTX if force else None
     try:
         return shell.SHCreateItemFromParsingName(
-            path, None, shell.IID_IShellItem2  # type: ignore
+            path, ctx, shell.IID_IShellItem  # type: ignore
         )
     except pywintypes.com_error as e:
         if e.hresult in E_FILE_NOT_FOUND:  # type: ignore
-            if force:
-                return shell.SHCreateItemFromParsingName(
-                    path, FOLDER_BIND_CTX, shell.IID_IShellItem2
-                )
-            else:
+            raise FileNotFoundError(path) from None
+        raise
+
+
+def filenames_to_IShellItemArray(paths: Iterable[StrPath]):
+    """Parse an iterable (list, etc) of filenames into an IShellItemArray, for use with
+    the plural forms of IFileOperation methods. If not filenames are passed, None is
+    returned (and indicates the operation would fail).
+    """
+    idls = []
+    for path in paths:
+        path = os.path.abspath(os.fspath(path))
+        try:
+            idl = shell.SHParseDisplayName(path, 0, None)[0]
+        except pywintypes.com_error as e:
+            if e.hresult in E_FILE_NOT_FOUND:  # type: ignore
                 raise FileNotFoundError(path) from None
-        else:
             raise
+        idls.append(idl)
+    return None if not idls else shell.SHCreateShellItemArrayFromIDLists(idls)
```

### Comparing `ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperation.py` & `ifileoperation-1.2.6/ifileoperation/com/interfaces/ifileoperation.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/com/interfaces/ifileoperationprogresssink.py` & `ifileoperation-1.2.6/ifileoperation/com/interfaces/ifileoperationprogresssink.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/com/interfaces/ifilesysbinddata.py` & `ifileoperation-1.2.6/ifileoperation/com/interfaces/ifilesysbinddata.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/com/interfaces/ishellitem.py` & `ifileoperation-1.2.6/ifileoperation/com/interfaces/ishellitem.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/errors.py` & `ifileoperation-1.2.6/ifileoperation/errors.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation/fileoperator.py` & `ifileoperation-1.2.6/ifileoperation/fileoperator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 import pythoncom
 
 from .com import (
     FileOperation,
     FileOperationProgressSink,
     convert_exceptions,
-    parse_filename,
+    filename_to_IShellItem,
+    filenames_to_IShellItemArray,
 )
 from .errors import IFileOperationError, UnexpectedError
 from .flags import FileOperationFlags, FileOperationResult, TransferSourceFlags
 
 StrPath: TypeAlias = str | PathLike[str]
 
 
@@ -108,14 +109,16 @@
         | FileOperationFlags.NO_CONFIRM_MKDIR
         | FileOperationFlags.SHOWELEVATIONPROMPT
     )
     """Flags to suppress all dialogs (as if Yes to All was selected), except for a UAC
     prompt if necessary.  If errors occur, the operation will fail immediately.
     """
 
+    results: dict[str, str]
+
     def __init__(
         self,
         parent=None,
         flags: FileOperationFlags | None = DEFAULT_FLAGS,
         *,
         commit_on_exit: bool = False,
     ):
@@ -136,14 +139,15 @@
             try:
                 parent = parent.GetHandle()  # wx.Window
             except AttributeError:
                 pass
         self._parent = parent
         self._flags = flags
         self.commit_on_exit = commit_on_exit
+        self.results = {}
 
     @convert_exceptions
     def __enter__(self):
         if self.entered:
             raise IFileOperationError(f'{type(self).__name__} is not reentrant')
         else:
             self.entered = True
@@ -179,28 +183,32 @@
         drive as a copy and delete.
 
         :param source: The file to be moved.
         :param destination: The destination *directory* to move to.
         :param new_name: The new name for the file if desired.
         """
         self.ifo.MoveItem(
-            parse_filename(source), parse_filename(destination, True), new_name
+            filename_to_IShellItem(source),
+            filename_to_IShellItem(destination, True),
+            new_name,
         )
         self._operations_queued = True
 
     @convert_exceptions
     def move_files(self, sources: Iterable[StrPath], destination: StrPath) -> None:
         """Schedule to move the files `sources` to `destination`. NOTE: Windows performs
         a move to a different logical drive as a copy and delete.
 
         :param sources: And iterable of filenames to be moved.
         :param destination: The destination *directory* to move to.
         """
-        srcs = [parse_filename(s) for s in sources]
-        self.ifo.MoveItems(srcs, parse_filename(destination, True))
+        srcs = filenames_to_IShellItemArray(sources)
+        if not srcs:
+            return
+        self.ifo.MoveItems(srcs, filename_to_IShellItem(destination, True))
         self._operations_queued = True
 
     @convert_exceptions
     def rename_file(
         self, source: StrPath, new_name: str, allow_move: bool = True
     ) -> None:
         """Schedule to rename `source` to `new_name`.  If `allow_move` is True and the
@@ -222,26 +230,28 @@
                 # instead
                 self.move_file(source, dest_path.parent, dest_path.name)
                 return
             else:
                 # new_name includes the directory, but it's the same directory, so a
                 # rename is fine
                 new_name = dest_path.name
-        self.ifo.RenameItem(parse_filename(source), new_name)
+        self.ifo.RenameItem(filename_to_IShellItem(source), new_name)
         self._operations_queued = True
 
     @convert_exceptions
     def rename_files(self, sources: Iterable[StrPath], new_name: StrPath) -> None:
         """Schedule to rename the files `sources` to `new_name`.  All files will be
         renamed to the new name.
 
         :param sources: An iterable of filenames to be renamed.
         :param new_name: The new name of the files.
         """
-        srcs = [parse_filename(s) for s in sources]
+        srcs = filenames_to_IShellItemArray(sources)
+        if not srcs:
+            return
         self.ifo.RenameItems(srcs, fspath(new_name))
         self._operations_queued = True
 
     @convert_exceptions
     def copy_file(
         self, source: StrPath, destination: StrPath, new_name: str | None = None
     ) -> None:
@@ -249,45 +259,51 @@
         file in the process.
 
         :param source: The file to be copied.
         :param destination: The destination *directory* to copy to.
         :param new_name: Optional new name of the file.
         """
         self.ifo.CopyItem(
-            parse_filename(source), parse_filename(destination, True), new_name
+            filename_to_IShellItem(source),
+            filename_to_IShellItem(destination, True),
+            new_name,
         )
         self._operations_queued = True
 
     @convert_exceptions
     def copy_files(self, sources: Iterable[StrPath], destination: StrPath) -> None:
         """Schedule to copy the files `sources` to `destination`.
 
         :param sources: An iterable of filenames to be copied.
         :param destination: The destination *directory* to copy to.
         """
-        srcs = [parse_filename(s) for s in sources]
-        self.ifo.CopyItems(srcs, parse_filename(destination, True))
+        srcs = filenames_to_IShellItemArray(sources)
+        if not srcs:
+            return
+        self.ifo.CopyItems(srcs, filename_to_IShellItem(destination, True))
         self._operations_queued = True
 
     @convert_exceptions
     def delete_file(self, source: StrPath) -> None:
         """Schedule to delete a file.
 
         :param source: The file to be deleted.
         """
-        self.ifo.DeleteItem(parse_filename(source))
+        self.ifo.DeleteItem(filename_to_IShellItem(source))
         self._operations_queued = True
 
     @convert_exceptions
     def delete_files(self, sources: Iterable[StrPath]) -> None:
         """Schedule to delete the files `sources`.
 
         :param sources: An iterable of filenames to be deleted.
         """
-        srcs = [parse_filename(s) for s in sources]
+        srcs = filenames_to_IShellItemArray(sources)
+        if not srcs:
+            return
         self.ifo.DeleteItems(srcs)
         self._operations_queued = True
 
     @convert_exceptions
     def _perform_operations(self):
         self.return_code = self.ifo.PerformOperations()
```

### Comparing `ifileoperation-1.2.5/ifileoperation/flags.py` & `ifileoperation-1.2.6/ifileoperation/flags.py`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/ifileoperation.egg-info/PKG-INFO` & `ifileoperation-1.2.6/ifileoperation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifileoperation
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python wrapper for using Win32's IFileOperation for manipulating the filesystem.
 Author: lojack5
 License: BSD 3-Clause
 Project-URL: Homepage, https://github.com/lojack5/IFileOperation
 Project-URL: Bug Tracker, https://github.com/lojack5/IFileOperation/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -145,15 +145,17 @@
   the new file, without its directory.  However, if you're used to other file
   APIs that let you "rename" a file into a different directory, `rename_file`
   supports this as well.  When `allow_move` is `True`, if it is detected that
   `new_name` is actually a path resolving to a different directory, this will
   automatically be transformed into a `move_file` operation instead.
 - `rename_files(sources: Iterable[StrPath], new_name: str)`:  Renames the given
   files to have the new name.  Unlike `rename_file`, you cannot rename files
-  into files in different directories.
+  into files in different directories. If multiple source files are in the same
+  directory, you probably want to include `FileOperationFlags.RENAMEONCOLLISION` to
+  prevent errors while renaming.
 - `delete_file(source: StrPath)`: Deletes the target file.
 - `delete_files(sources: Iterable[StrPath])`: Deletes the target files.
 - `commit()`: Cause all the queue operations to be performed.
 
 ### Post-commit attributes
 After a `commit`, additional attributes are available on the `FileOperator` instance:
 - `return_code`: The `HRESULT` return code from the overall operation. This is usually
```

### Comparing `ifileoperation-1.2.5/ifileoperation.egg-info/SOURCES.txt` & `ifileoperation-1.2.6/ifileoperation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/pyproject.toml` & `ifileoperation-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ifileoperation-1.2.5/tests/test_ifileoperation.py` & `ifileoperation-1.2.6/tests/test_ifileoperation.py`

 * *Files identical despite different names*

