# Comparing `tmp/niconico.py-1.2.3.tar.gz` & `tmp/niconico.py-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niconico.py-1.2.3.tar", last modified: Fri Feb 11 07:32:04 2022, max compression
+gzip compressed data, was "niconico.py-1.2.4.tar", last modified: Wed Aug  2 18:19:35 2023, max compression
```

## Comparing `niconico.py-1.2.3.tar` & `niconico.py-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 07:32:04.562679 niconico.py-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-02-11 07:31:55.000000 niconico.py-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-02-11 07:32:04.562679 niconico.py-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-02-11 07:31:55.000000 niconico.py-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 07:32:04.562679 niconico.py-1.2.3/niconico/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/cookies.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/niconico.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 07:32:04.562679 niconico.py-1.2.3/niconico/objects/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/objects/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/objects/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/objects/video.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16516 2022-02-11 07:31:55.000000 niconico.py-1.2.3/niconico/video.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 07:32:04.562679 niconico.py-1.2.3/niconico.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-02-11 07:32:04.000000 niconico.py-1.2.3/niconico.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-11 07:32:04.000000 niconico.py-1.2.3/niconico.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 07:32:04.000000 niconico.py-1.2.3/niconico.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-11 07:32:04.000000 niconico.py-1.2.3/niconico.py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-11 07:32:04.000000 niconico.py-1.2.3/niconico.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-11 07:32:04.000000 niconico.py-1.2.3/niconico.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-11 07:32:04.562679 niconico.py-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-02-11 07:31:55.000000 niconico.py-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:19:35.218928 niconico.py-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 18:19:27.000000 niconico.py-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-02 18:19:35.218928 niconico.py-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-02 18:19:27.000000 niconico.py-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:19:35.218928 niconico.py-1.2.4/niconico/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/niconico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:19:35.218928 niconico.py-1.2.4/niconico/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/objects/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/objects/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/objects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/objects/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-08-02 18:19:27.000000 niconico.py-1.2.4/niconico/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:19:35.218928 niconico.py-1.2.4/niconico.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-02 18:19:35.000000 niconico.py-1.2.4/niconico.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-02 18:19:35.000000 niconico.py-1.2.4/niconico.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:19:35.000000 niconico.py-1.2.4/niconico.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 18:19:35.000000 niconico.py-1.2.4/niconico.py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 18:19:35.000000 niconico.py-1.2.4/niconico.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 18:19:35.000000 niconico.py-1.2.4/niconico.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-02 18:19:27.000000 niconico.py-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:19:35.218928 niconico.py-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 18:19:27.000000 niconico.py-1.2.4/setup.py
```

### Comparing `niconico.py-1.2.3/LICENSE` & `niconico.py-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `niconico.py-1.2.3/PKG-INFO` & `niconico.py-1.2.4/niconico/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,98 @@
-Metadata-Version: 2.1
-Name: niconico.py
-Version: 1.2.3
-Summary: ニコニコスクレイピングライブラリ
-Home-page: https://github.com/tasuren/niconico.py
-Author: tasuren
-Author-email: tasuren@aol.com
-License: MIT
-Project-URL: Documentation, https://niconico-py.readthedocs.io/
-Description: [![PyPI](https://img.shields.io/pypi/v/niconico.py)](https://pypi.org/project/niconico.py/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/niconico.py) ![PyPI - Downloads](https://img.shields.io/pypi/dm/niconico.py) ![PyPI - License](https://img.shields.io/pypi/l/niconico.py) [![Documentation Status](https://readthedocs.org/projects/niconico-py/badge/?version=latest)](https://niconico-py.readthedocs.io/ja/latest/?badge=latest) [![Discord](https://img.shields.io/discord/777430548951728149?label=chat&logo=discord)](https://discord.gg/kfMwZUyGFG) [![Buy Me a Coffee](https://img.shields.io/badge/-tasuren-E9EEF3?label=Buy%20Me%20a%20Coffee&logo=buymeacoffee)](https://www.buymeacoffee.com/tasuren)
-        # niconico.py
-        niconico.pyはニコニコにあるコンテンツを取得するためのライブラリです。  
-        これを使うことでニコニコ動画の動画のダウンロードができます。  
-        また、自分のアカウントを使用して動画情報の取得も可能です。
-        
-        **Warning!**  
-        現在は開発されたばかりで使用者が予期できない変更やバグがある可能性があります。
-        
-        ## Installation
-        pipを使用してインストールすることができます。  
-        `pip install niconico.py`
-        
-        ## Example
-        ### ニコニコ動画
-        #### ダウンロード
-        ```python
-        from niconico import NicoNico
-        
-        client = NicoNico()
-        
-        with client.video.get_video("https://www.nicovideo.jp/watch/sm37658498") as video:
-            video.download(f"{video.video.id}.mp4")
-        ```
-        #### マイリスト
-        ```python
-        from niconico import NicoNico
-        
-        URL = "https://www.nicovideo.jp/user/85641805/mylist/63403141"
-        
-        client = NicoNico()
-        for mylist in client.video.get_mylist(URL):
-            print(f"取り出したマイリスト: %s (%s)" % (mylist.name, mylist.id))
-        ```
-        
-        ## コンソールからの使用
-        `niconico help`で使用方法を確認可能です。  
-        注意：コマンドの使用方法は後日変更される予定です。
-        
-        ## ToDo
-        * [x] 動画のダウンロード
-        * [x] マイリストの読み込み
-        * [ ] 検索
-        * [ ] ニコニコ大百科
-        * [ ] ニコニコ静画
-        * [ ] 非同期版 (できれば)
-        * [ ] etc
-        
-        ## Documentation
-        ドキュメンテーションは[こちら](https://niconico-py.readthedocs.io/ja/latest/)から閲覧が可能です。  
-        テーマに[pydata-sphinx-theme](https://github.com/pydata/pydata-sphinx-theme/blob/master/LICENSE)を使用しています。
-        
-        ## Contributing
-        リポジトリ内の`contributing.md`をご覧ください。
-        
-        ## License
-        MITライセンスの下で使用が可能です。
-        
-Keywords: video download niconico ニコニコ動画
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
+# niconico.py - Base
+
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Generic, TypeVar, Type, Optional
+
+if TYPE_CHECKING:
+    from .niconico import NicoNico
+
+
+__all__ = ("DictFromAttribute", "BaseClient")
+
+
+SuperT = TypeVar("SuperT")
+class DictFromAttribute(Generic[SuperT]):
+    """辞書を属性からアクセスできるようにするものです。
+    属性からアクセスされた際に返すものもこのクラスのインスタンスです。
+    niconico.pyでのほとんどのニコニコのデータはこのクラスのインスタンスに格納されます。
+
+    Parameters
+    ----------
+    data : dict
+        属性でアクセスされた際に返すべき値がある辞書です。
+    super_ : SuperT
+        属性からアクセスされた際に返すインスタンスに渡すものです。
+
+    Attributes
+    ----------
+    __data__ : dict
+        インスタンス化時に引数の ``data`` に渡された辞書が入っています。
+
+        Notes
+        -----
+        データに属性からではない方法でアクセスしたい場合はこれを使用しましょう。
+        また、生のデータを取得したい場合はこちらを使用してください。
+    __super__ : SuperT
+        インスタンス化時に引数の ``super_`` に渡されたオブジェクトです。
+        ニコニコのデータの場合はそのデータの提供元(例：ニコニコ動画)のクライアント用クラスのインスタンスが入ります。"""
+
+    __dfa_class__: Type[DictFromAttribute]
+
+    def __init__(self, data: dict, super_: SuperT):
+        self.__data__, self.__super__ = data, super_
+
+    @staticmethod
+    def _get_extends(cls) -> dict[str, Type[DictFromAttribute]]:
+        return getattr(cls, "__extends__", {})
+
+    @classmethod
+    def _from_data(cls, data, super_: SuperT, key: str):
+        cls = cls._get_extends(cls).get(key, cls)
+        if isinstance(data, dict):
+            try:
+                return cls(data, super_)
+            except TypeError:
+                return cls.__dfa_class__(data, super_)
+        elif isinstance(data, list):
+            return [cls._from_data(item, super_, key) for item in data]
+        else:
+            return data
+
+    def __getattr__(self, key: str):
+        if key in self.__data__:
+            return self._from_data(self.__data__[key], self.__super__, key)
+        else:
+            raise AttributeError(
+                f"class '{self.__class__.__name__}' has no attributre '{key}'"
+            )
+
+
+class BaseClient:
+    """クライアントクラスのベースクラスです。  
+    ここでいうベースクラスはニコニコの各サービスのために用意するクライアントに使われるもので、 :class:`niconico.niconico.NicoNico` では使われません。
+
+    Parameters
+    ----------
+    cookies : Cookies, optional
+        リクエストを行う際に使用するクッキーです。
+        指定しない場合は :func:`niconico.cookies.Cookies.guest` を実行して返ってきたものが使われます。"""
+
+    if TYPE_CHECKING:
+        niconico: NicoNico
+
+    def log(self, type_: str, content: str, *args, **kwargs):
+        """クラスの名前を使ってログ出力を行います。
+        :attr:`niconico.niconico.NicoNico.logger` が使用されます。
+        普通これは開発者が使います。
+
+        Parameters
+        ----------
+        type_ : str
+        content : str
+        *args
+        **kwargs"""
+        return getattr(self.niconico.logger, type_)(content, *args, **kwargs)
+
+    def __init__(self, niconico: NicoNico):
+        self.niconico = niconico
```

### Comparing `niconico.py-1.2.3/niconico/__main__.py` & `niconico.py-1.2.4/niconico/__main__.py`

 * *Files identical despite different names*

### Comparing `niconico.py-1.2.3/niconico/cookies.py` & `niconico.py-1.2.4/niconico/cookies.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,25 @@
 
 
 __all__ = ("Cookies",)
 FORMAT = "%a, %d-%b-%Y %X"
 
 
 class Cookies(SimpleCookie):
+    @staticmethod
+    def _make_cookie_tuple(name: str, cookie: str, domain: Optional[str] = ".nicovideo.jp"):
+        cookies = Cookies()
+        cookies[name] = cookie
+        for key, value in (
+            ("domain", domain), ("path", "/"),
+            ("expires", (datetime.now() + timedelta(days=365)).strftime(FORMAT))
+        ):
+            cookies[name][key] = value
+        return cookies
+
     @classmethod
     def from_file(cls, path: str):
         """Netscapeのクッキーファイルフォーマットに準拠したテキストファイルからクッキーが格納されたクラスを作成します。  
         なので、ChromeやEdgeで使用可能な `Get cookies.txt <https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid>`_ のような拡張機能を使って作ったクッキーのテキストファイルを読み込むことができます。
         もし自分のアカウントでニコニコ動画のコンテンツを取得したい場合はこれを使用しましょう。
 
         Parameters
@@ -41,23 +52,26 @@
             ):
                 if key:
                     cookies[item[5]][key] = (
                         datetime.fromtimestamp(float(item[index])).strftime(FORMAT)
                         if key == "expires" else item[index]
                     )
         return cookies
+    
+    @classmethod
+    def from_string(cls, user_session: str):
+        """ニコニコ動画上での認証済みのクッキーの値を直接指定しクラスを作成します。
+
+        Parameters
+        ----------
+        user_session : str
+            ユーザーセッションです。"""
+        return cls._make_cookie_tuple("user_session", user_session)
 
     @classmethod
     def guest(cls, nicosid: Optional[str] = None):
         """ニコニコのゲストアカウントのクッキーを生成します。  
 
         Notes
         -----
         これはニコニコ動画にアクセスして作成するクッキーではなく、開発者がクッキーを見て予想して作った再現物です。"""
-        cookies = cls()
-        cookies["nicosid"] = nicosid or str(time())
-        for key, value in (
-            ("domain", ".nicovideo.jp"), ("path", "/"),
-            ("expires", (datetime.now() + timedelta(days=365)).strftime(FORMAT))
-        ):
-            cookies["nicosid"][key] = value
-        return cookies
+        return cls._make_cookie_tuple("nicosid", nicosid or str(time()))
```

### Comparing `niconico.py-1.2.3/niconico/niconico.py` & `niconico.py-1.2.4/niconico/niconico.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # niconico.py - Client
 
 from __future__ import annotations
 
 from typing import Optional
 
 from logging import getLogger
+import re
 
 import requests
 
 from .video import Client as VideoClient
+from .search import SearchClient
 from .cookies import Cookies
 
+from .exceptions import LoginFailureException
+
 
 __all__ = ("adjust_cookies", "NicoNico", "logger")
 Response = requests.Response
 logger = getLogger("niconico.py")
 "``logging`` の ``Logger`` です。"
 
 
@@ -39,14 +43,15 @@
     video: VideoClient
     "ニコニコ動画用のクライアントクラスのインスタンスです。"
     cookies: Optional[Cookies]
     "リクエスト時に使用するクッキーです。"
 
     def __init__(self, cookies: Optional[Cookies] = None):
         self.video = VideoClient(self)
+        self.searchclient = SearchClient(self)
         self.cookies = cookies
         self.logger = logger
 
     def request(self, method: str, url: str, *args, **kwargs) -> requests.Response:
         """``requests.request`` を使用して設定されているクッキーでリクエストを行います。
         引数は ``requests.request`` と同じです。
 
@@ -78,8 +83,43 @@
                 self.logger.debug("使用予定の%s: %s" % (value, kwargs[key]))
 
         # リクエストをする。
         response = requests.request(method, url, *args, **kwargs)
         if save_default:
             self.cookies = Cookies(response.cookies.get_dict())
         response.raise_for_status()
-        return response
+        return response
+
+    def login(self, mail: str, password: str) -> NicoNico:
+        """メールアドレスとパスワードを用いてログインを行います。
+        二段階認証が有効になっているアカウントではログインすることができません。
+        クッキーの中身を直接置き換える方法で認証をしてください。
+
+        Parameters
+        ----------
+        mail : str
+            ログインする際のメールアドレスもしくは電話番号です。
+        password : str
+            ログインする際のパスワードです。
+
+        Raises
+        ------
+        LoginFailureException"""
+        session = requests.session()
+        
+        res = session.post(
+            "https://secure.nicovideo.jp/secure/login?site=niconico",
+            params={
+                "mail": mail,
+                "password": password
+            })
+        
+        if res.headers.get("x-niconico-authflag") == ('1' or '3'):
+            self.cookies = Cookies.from_string(session.cookies.get("user_session"))
+            return self
+        else:
+            title_ptn = re.compile('<title>(.*?)</title>')
+            title = title_ptn.search(res.text)
+            if title:
+                if "2段階認証" in title.group(1):
+                    raise LoginFailureException("Two-step verification is not supported.")
+        raise LoginFailureException("Login failed.")
```

### Comparing `niconico.py-1.2.3/niconico/objects/video.py` & `niconico.py-1.2.4/niconico/objects/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # niconico.py - Video # TODO: middleが何なのか調べる。
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypedDict, Literal, Optional, List, Any
 
 from ..base import DictFromAttribute
-from .__init__ import Unknown
 
 if TYPE_CHECKING:
     from ..video import Client as VideoClient, Video as RealVideo
 
 
 __all__ = (
     "NicoDic", "Phrase", "EasyComment", "TagEdit", "TagItem", "Tag", "Counter", "Thumbnail",
     "Rating", "ViewerLike", "Viewer", "AbcOwner", "AbcVideo", "Video", "VideoOwner",
+    "CommentServer","NvCommentID","NvCommentParams","NvComment","Comment",
     "MyListOwner", "MyListItemVideo", "MyListItem", "MyList"
 )
 
 
 # easyComment
 class NicoDic(DictFromAttribute):
     "ニコニコ大百科での簡易データです。"
@@ -200,14 +200,49 @@
     "クライアントのデータです。"
     watchableUserTypeForPayment: str # TODO: ここに入る文字列は決まっている、なのでLiteralにしたい。
     "不明"
     commentableUserTypeForPayment: str # TODO: 上記と同じ。
     "不明"
 
 
+class CommentServer(DictFromAttribute):
+    "コメントサーバーに関するデータです。"
+
+    url: str
+    "コメントサーバーのURLです。"
+
+
+class NvCommentID(DictFromAttribute):
+    "コメントデータ取得に関するデータです。"
+
+    id: str
+    fork: str
+
+
+class NvCommentParams(DictFromAttribute):
+    "コメントデータ取得に関するデータです。"
+
+    targets: List[NvCommentID]
+    language: str
+
+class NvComment(DictFromAttribute):
+    "コメントデータ取得に関するデータです。"
+
+    threadKey: str
+    server: str
+    params: NvCommentParams
+
+
+class Comment(DictFromAttribute):
+    "コメントに関するデータです。"
+
+    server: CommentServer
+    nvComment: NvComment
+
+
 class MyListOwner(AbcOwner):
     "マイリストのオーナーのデータです。"
 
     ownerType: str
     "不明"
```

### Comparing `niconico.py-1.2.3/niconico/video.py` & `niconico.py-1.2.4/niconico/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from json import loads
 
 from .base import DictFromAttribute, BaseClient
 from .exceptions import ExtractFailed
 from .enums import VideoDownloadMode
 from .utils import parse_link
 
-from .objects.video import EasyComment, Tag, VideoOwner, Video as AbcVideo, MyList as AbcMyList
+from .objects.video import Comment, EasyComment, Tag, VideoOwner, Video as AbcVideo, MyList as AbcMyList
+from .objects.comment import Comments, MovieChat
 
 if TYPE_CHECKING:
     from .niconico import Response
 
 
 __all__ = ("HEADERS", "Video", "Client")
 BASES = {
@@ -116,14 +117,16 @@
     "動画の投稿者です。"
     thread: Optional[Thread] = None
     "ハートビートを動かすスレッドです。"
     url: str
     "動画のURLです。"
     client: Client
     "動画取得用のクライアントのインスタンスです。"
+    comment: Comment
+    "コメントのデータです。"
 
     def __init__(self, client: Client, url: str, data: dict):
         self.client, self.url, self.__data__ = client, url, data
         self._heartbeat_running = Event()
         self._download_log: Optional[Callable[[Any], None]] = None
         super().__init__(self.__data__, self)
 
@@ -342,36 +345,92 @@
         }
         data["client_info"] = {
             "player_id": session["playerId"]
         }
         del session
 
         return {"session": data}
+    
+    def get_comments(self, fork: str, num: Optional[int] = 1000, when: Optional[int] = None) -> Comments:
+        """動画のコメントを取得します。
+
+        Parameters
+        ----------
+        fork : str
+            コメントの種類です。"main","owner","easy","channel"が指定可能です。
+        num : int, default 1000
+            1度に取得する数です。1000が最大です。
+        when: Optional[int]
+            過去ログをUNIXタイムで指定できます。何も指定しない場合は最新のコメントを取得します。"""
+        fork_id = "0"
+        if fork == "main":
+            fork_id = "0"
+        elif fork == "owner":
+            fork_id = "1"
+        elif fork == "easy":
+            fork_id = "2"
+        r = self.client.niconico.request(
+            "GET", f"{self.comment.nvComment.server}/legacy/api.json/thread", headers=HEADERS["normal"],
+            params={
+                "fork": fork_id,
+                "nicoru": "3",
+                "scores": "1",
+                "res_from": f"-{num}",
+                "thread": next(
+                    x for x in self.comment.nvComment.params.targets if x.fork == fork).id,
+                "version": "20090904",
+                "with_global": "1",
+                "when": when or ""
+            }
+        ).json()
+
+        comments = Comments()
+        comments.fork = fork
+        for obj in r:
+            if "thread" in obj:
+                if obj["thread"]["resultcode"] == 1:
+                    raise Exception("コメントの取得に失敗しました。")
+                comments.thread = obj["thread"]["thread"]
+                comments.ticket = obj["thread"].get("ticket")
+                comments.last_res = obj["thread"].get("last_res")
+                comments.when = when or obj["thread"]["server_time"]
+            if "leaf" in obj:
+                comments.count = obj["leaf"]["count"]
+            if "global_num_res" in obj:
+                comments.num_res = obj["global_num_res"]["num_res"]
+            if "chat" in obj:
+                comments.chats.append(MovieChat(obj["chat"]))
+
+        return comments
 
 
 class Client(BaseClient):
     """ニコニコ動画用のクライアントです。
     普通 :class:`niconico.niconico.NicoNico` から使います。"""
 
     def get_video(self, url: str) -> Video:
         """ニコニコ動画から指定された動画を取得します。
 
         Parameters
         ----------
         url : str
-            動画のURLです。。
+            動画のURLです。(ex. https://www.nicovideo.jp/watch/sm9)
+            動画IDでも指定できます。(ex. sm9)
 
         Raises
         ------
         ExtractFailed"""
         # 短縮やスマホ用のURLであれば元に戻す。
         if "nico.ms" in url:
             url = url.replace("nico.ms/", "www.nicovideo.jp/watch/")
         url = parse_link(url)
 
+        if "watch" not in url:
+            url = "https://www.nicovideo.jp/watch/" + url
+
         # 動画情報を取得する。
         data = BeautifulSoup(
             self.niconico.request("GET", url, headers=HEADERS["normal"]).text, "html.parser"
         ).find(
             "div", {"id": "js-initial-watch-data"}
         ).get("data-api-data")
         video = Video(self, url, data)
```

### Comparing `niconico.py-1.2.3/niconico.py.egg-info/SOURCES.txt` & `niconico.py-1.2.4/niconico.py.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 niconico/__init__.py
 niconico/__main__.py
 niconico/base.py
 niconico/cookies.py
 niconico/enums.py
 niconico/exceptions.py
 niconico/niconico.py
 niconico/py.typed
+niconico/search.py
 niconico/utils.py
 niconico/video.py
 niconico.py.egg-info/PKG-INFO
 niconico.py.egg-info/SOURCES.txt
 niconico.py.egg-info/dependency_links.txt
 niconico.py.egg-info/entry_points.txt
 niconico.py.egg-info/requires.txt
 niconico.py.egg-info/top_level.txt
 niconico/objects/__init__.py
+niconico/objects/comment.py
 niconico/objects/dictionary.py
 niconico/objects/py.typed
 niconico/objects/video.py
```

### Comparing `niconico.py-1.2.3/setup.py` & `niconico.py-1.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 
 
 NAME = "niconico.py"
 DESCRIPTION = "ニコニコスクレイピングライブラリ"
 
 
 if exists("README.md"):
-    with open("README.md", "r") as f:
+    with open("README.md", "r", encoding="utf-8") as f:
         long_description = f.read()
 else:
     long_description = DESCRIPTION
 
 
-with open(f"{NAME[:-3]}/__init__.py", "r") as f:
+with open(f"{NAME[:-3]}/__init__.py", "r", encoding="utf-8") as f:
     text = f.read()
     version = text.split('__version__ = "')[1].split('"')[0]
     author = text.split('__author__ = "')[1].split('"')[0]
 
 
 setup(
     name=NAME,
     version=version,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url=f'https://github.com/tasuren/{NAME}',
+    url=f'https://github.com/niconicolibs/{NAME}',
     project_urls={
         "Documentation": f"https://{NAME.replace('.', '-')}.readthedocs.io/"
     },
     entry_points={
         "console_scripts": [
             "niconico = niconico.__main__:main"
         ]
@@ -49,8 +49,8 @@
     python_requires='>=3.8.0',
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Typing :: Typed'
     ]
-)
+)
```

