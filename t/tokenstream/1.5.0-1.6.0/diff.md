# Comparing `tmp/tokenstream-1.5.0.tar.gz` & `tmp/tokenstream-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenstream-1.5.0.tar", max compression
+gzip compressed data, was "tokenstream-1.6.0.tar", max compression
```

## Comparing `tokenstream-1.5.0.tar` & `tokenstream-1.6.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-01-05 00:36:24.184512 tokenstream-1.5.0/LICENSE
--rw-r--r--   0        0        0     7512 2023-01-05 00:36:24.184512 tokenstream-1.5.0/README.md
--rw-r--r--   0        0        0     1542 2023-01-05 00:38:29.469610 tokenstream-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      334 2023-01-05 00:38:29.441609 tokenstream-1.5.0/tokenstream/__init__.py
--rw-r--r--   0        0        0     3916 2023-01-05 00:36:24.188512 tokenstream-1.5.0/tokenstream/error.py
--rw-r--r--   0        0        0     3398 2023-01-05 00:36:24.188512 tokenstream-1.5.0/tokenstream/location.py
--rw-r--r--   0        0        0        0 2023-01-05 00:36:24.188512 tokenstream-1.5.0/tokenstream/py.typed
--rw-r--r--   0        0        0    37394 2023-01-05 00:36:24.188512 tokenstream-1.5.0/tokenstream/stream.py
--rw-r--r--   0        0        0     2729 2023-01-05 00:36:24.188512 tokenstream-1.5.0/tokenstream/token.py
--rw-r--r--   0        0        0     8366 1970-01-01 00:00:00.000000 tokenstream-1.5.0/setup.py
--rw-r--r--   0        0        0     8225 1970-01-01 00:00:00.000000 tokenstream-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-02 18:51:55.545993 tokenstream-1.6.0/LICENSE
+-rw-r--r--   0        0        0     7512 2023-08-02 18:51:55.545993 tokenstream-1.6.0/README.md
+-rw-r--r--   0        0        0     1542 2023-08-02 18:52:44.786665 tokenstream-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-08-02 18:52:44.762665 tokenstream-1.6.0/tokenstream/__init__.py
+-rw-r--r--   0        0        0     3916 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/error.py
+-rw-r--r--   0        0        0     3398 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/location.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/py.typed
+-rw-r--r--   0        0        0    37644 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/stream.py
+-rw-r--r--   0        0        0     2729 2023-08-02 18:51:55.549993 tokenstream-1.6.0/tokenstream/token.py
+-rw-r--r--   0        0        0     8225 1970-01-01 00:00:00.000000 tokenstream-1.6.0/PKG-INFO
```

### Comparing `tokenstream-1.5.0/LICENSE` & `tokenstream-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenstream-1.5.0/README.md` & `tokenstream-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tokenstream-1.5.0/pyproject.toml` & `tokenstream-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tokenstream"
-version = "1.5.0"
+version = "1.6.0"
 description = "A versatile token stream for handwritten parsers"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/vberlier/tokenstream"
 repository = "https://github.com/vberlier/tokenstream"
 documentation = "https://github.com/vberlier/tokenstream"
```

### Comparing `tokenstream-1.5.0/tokenstream/error.py` & `tokenstream-1.6.0/tokenstream/error.py`

 * *Files identical despite different names*

### Comparing `tokenstream-1.5.0/tokenstream/location.py` & `tokenstream-1.6.0/tokenstream/location.py`

 * *Files identical despite different names*

### Comparing `tokenstream-1.5.0/tokenstream/stream.py` & `tokenstream-1.6.0/tokenstream/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "CheckpointCommit",
     "BAKED_REGEX_CACHE",
 ]
 
 import re
 from contextlib import contextmanager
 from dataclasses import dataclass, field
-from typing import Any, ContextManager, Iterable, Iterator, TypeVar, overload
+from typing import Any, Callable, ContextManager, Iterable, Iterator, TypeVar, overload
 
 from .error import InvalidSyntax, UnexpectedEOF, UnexpectedToken
 from .location import SourceLocation, set_location
 from .token import Token, TokenPattern
 
 T = TypeVar("T")
 
@@ -64,14 +64,17 @@
     source
         The input string.
 
         >>> stream = TokenStream("hello world")
         >>> stream.source
         'hello world'
 
+    token_handler
+        A callback for modifying tokens before they're emitted.
+
     syntax_rules
         A tuple of ``(token_type, pattern)`` pairs that define the recognizable tokens.
 
         >>> stream = TokenStream("hello world")
         >>> with stream.syntax(word=r"[a-z]+"):
         ...     print(stream.syntax_rules)
         (('word', '[a-z]+'),)
@@ -136,14 +139,15 @@
 
     regex_cache
         A cache that keeps a reference to the compiled regular expression associated
         to each set of syntax rules.
     """
 
     source: str
+    token_handler: Callable[[Token], Token] | None = extra_field(default=None)
     syntax_rules: SyntaxRules = extra_field(default=())
     regex: re.Pattern[str] = extra_field()
 
     location: SourceLocation = extra_field()
 
     index: int = extra_field(default=-1)
     tokens: list[Token] = extra_field(default_factory=list)
@@ -478,14 +482,17 @@
         token = Token(
             type=token_type,
             value=value,
             location=self.location,
             end_location=SourceLocation(end_pos, end_lineno, end_colno),
         )
 
+        if self.token_handler:
+            token = self.token_handler(token)
+
         self.location = token.end_location
         self.tokens.append(token)
 
         self.index = len(self.tokens) - 1
 
         return token
```

### Comparing `tokenstream-1.5.0/tokenstream/token.py` & `tokenstream-1.6.0/tokenstream/token.py`

 * *Files identical despite different names*

### Comparing `tokenstream-1.5.0/setup.py` & `tokenstream-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,235 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tokenstream
+Version: 1.6.0
+Summary: A versatile token stream for handwritten parsers
+Home-page: https://github.com/vberlier/tokenstream
+License: MIT
+Keywords: parsing,tokenizer,lexer,recursive-descent-parser,token-stream
+Author: Valentin Berlier
+Author-email: berlier.v@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Documentation, https://github.com/vberlier/tokenstream
+Project-URL: Repository, https://github.com/vberlier/tokenstream
+Description-Content-Type: text/markdown
 
-packages = \
-['tokenstream']
+# tokenstream
 
-package_data = \
-{'': ['*']}
+[![GitHub Actions](https://github.com/vberlier/tokenstream/workflows/CI/badge.svg)](https://github.com/vberlier/tokenstream/actions)
+[![PyPI](https://img.shields.io/pypi/v/tokenstream.svg)](https://pypi.org/project/tokenstream/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tokenstream.svg)](https://pypi.org/project/tokenstream/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
-setup_kwargs = {
-    'name': 'tokenstream',
-    'version': '1.5.0',
-    'description': 'A versatile token stream for handwritten parsers',
-    'long_description': '# tokenstream\n\n[![GitHub Actions](https://github.com/vberlier/tokenstream/workflows/CI/badge.svg)](https://github.com/vberlier/tokenstream/actions)\n[![PyPI](https://img.shields.io/pypi/v/tokenstream.svg)](https://pypi.org/project/tokenstream/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tokenstream.svg)](https://pypi.org/project/tokenstream/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n> A versatile token stream for handwritten parsers.\n\n```python\nfrom tokenstream import TokenStream\n\ndef parse_sexp(stream: TokenStream):\n    """A basic S-expression parser."""\n    with stream.syntax(brace=r"\\(|\\)", number=r"\\d+", name=r"\\w+"):\n        brace, number, name = stream.expect(("brace", "("), "number", "name")\n        if brace:\n            return [parse_sexp(stream) for _ in stream.peek_until(("brace", ")"))]\n        elif number:\n            return int(number.value)\n        elif name:\n            return name.value\n\nprint(parse_sexp(TokenStream("(hello (world 42))")))  # [\'hello\', [\'world\', 42]]\n```\n\n## Introduction\n\nWriting recursive-descent parsers by hand can be quite elegant but it\'s often a bit more verbose than expected, especially when it comes to handling indentation and reporting proper syntax errors. This package provides a powerful general-purpose token stream that addresses these issues and more.\n\n### Features\n\n- Define the set of recognizable tokens dynamically with regular expressions\n- Transparently skip over irrelevant tokens\n- Expressive API for matching, collecting, peeking, and expecting tokens\n- Clean error reporting with line numbers and column numbers\n- Contextual support for indentation-based syntax\n- Checkpoints for backtracking parsers\n- Works well with Python 3.10+ match statements\n\nCheck out the [`examples`](https://github.com/vberlier/tokenstream/tree/main/examples) directory for practical examples.\n\n## Installation\n\nThe package can be installed with `pip`.\n\n```bash\npip install tokenstream\n```\n\n## Getting started\n\nYou can define tokens with the `syntax()` method. The keyword arguments associate regular expression patterns to token types. The method returns a context manager during which the specified tokens will be recognized.\n\n```python\nstream = TokenStream("hello world")\n\nwith stream.syntax(word=r"\\w+"):\n    print([token.value for token in stream])  # [\'hello\', \'world\']\n```\n\nCheck out the full [API reference](https://vberlier.github.io/tokenstream/api_reference/) for more details.\n\n### Expecting tokens\n\nThe token stream is iterable and will yield all the extracted tokens one after the other. You can also retrieve tokens from the token stream one at a time by using the `expect()` method.\n\n```python\nstream = TokenStream("hello world")\n\nwith stream.syntax(word=r"\\w+"):\n    print(stream.expect().value)  # "hello"\n    print(stream.expect().value)  # "world"\n```\n\nThe `expect()` method lets you ensure that the extracted token matches a specified type and will raise an exception otherwise.\n\n```python\nstream = TokenStream("hello world")\n\nwith stream.syntax(number=r"\\d+", word=r"\\w+"):\n    print(stream.expect("word").value)  # "hello"\n    print(stream.expect("number").value)  # UnexpectedToken: Expected number but got word \'world\'\n```\n\n### Filtering the stream\n\nNewlines and whitespace are ignored by default. You can reject interspersed whitespace by intercepting the built-in `newline` and `whitespace` tokens.\n\n```python\nstream = TokenStream("hello world")\n\nwith stream.syntax(word=r"\\w+"), stream.intercept("newline", "whitespace"):\n    print(stream.expect("word").value)  # "hello"\n    print(stream.expect("word").value)  # UnexpectedToken: Expected word but got whitespace \' \'\n```\n\nThe opposite of the `intercept()` method is `ignore()`. It allows you to ignore tokens and handle comments pretty easily.\n\n```python\nstream = TokenStream(\n    """\n    # this is a comment\n    hello # also a comment\n    world\n    """\n)\n\nwith stream.syntax(word=r"\\w+", comment=r"#.+$"), stream.ignore("comment"):\n    print([token.value for token in stream])  # [\'hello\', \'world\']\n```\n\n### Indentation\n\nTo enable indentation you can use the `indent()` method. The stream will now yield balanced pairs of `indent` and `dedent` tokens when the indentation changes.\n\n```python\nsource = """\nhello\n    world\n"""\nstream = TokenStream(source)\n\nwith stream.syntax(word=r"\\w+"), stream.indent():\n    stream.expect("word")\n    stream.expect("indent")\n    stream.expect("word")\n    stream.expect("dedent")\n```\n\nTo prevent some tokens from triggering unwanted indentation changes you can use the `skip` argument.\n\n```python\nsource = """\nhello\n        # some comment\n    world\n"""\nstream = TokenStream(source)\n\nwith stream.syntax(word=r"\\w+", comment=r"#.+$"), stream.indent(skip=["comment"]):\n    stream.expect("word")\n    stream.expect("comment")\n    stream.expect("indent")\n    stream.expect("word")\n    stream.expect("dedent")\n```\n\n### Checkpoints\n\nThe `checkpoint()` method returns a context manager that resets the stream to the current token at the end of the `with` statement. You can use the returned `commit()` function to keep the state of the stream at the end of the `with` statement.\n\n```python\nstream = TokenStream("hello world")\n\nwith stream.syntax(word=r"\\w+"):\n    with stream.checkpoint():\n        print([token.value for token in stream])  # [\'hello\', \'world\']\n    with stream.checkpoint() as commit:\n        print([token.value for token in stream])  # [\'hello\', \'world\']\n        commit()\n    print([token.value for token in stream])  # []\n```\n\n### Match statements\n\nMatch statements make it very intuitive to process tokens extracted from the token stream. If you\'re using Python 3.10+ give it a try and see if you like it.\n\n```python\nfrom tokenstream import TokenStream, Token\n\ndef parse_sexp(stream: TokenStream):\n    """A basic S-expression parser that uses Python 3.10+ match statements."""\n    with stream.syntax(brace=r"\\(|\\)", number=r"\\d+", name=r"\\w+"):\n        match stream.expect_any(("brace", "("), "number", "name"):\n            case Token(type="brace"):\n                return [parse_sexp(stream) for _ in stream.peek_until(("brace", ")"))]\n            case Token(type="number") as number :\n                return int(number.value)\n            case Token(type="name") as name:\n                return name.value\n```\n\n## Contributing\n\nContributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org/).\n\n```bash\n$ poetry install\n```\n\nYou can run the tests with `poetry run pytest`.\n\n```bash\n$ poetry run pytest\n```\n\nThe project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you\'re using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.\n\n```bash\n$ npm run watch\n$ npm run check\n$ npm run verifytypes\n```\n\nThe code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).\n\n```bash\n$ poetry run isort tokenstream examples tests\n$ poetry run black tokenstream examples tests\n$ poetry run black --check tokenstream examples tests\n```\n\n---\n\nLicense - [MIT](https://github.com/vberlier/tokenstream/blob/main/LICENSE)\n',
-    'author': 'Valentin Berlier',
-    'author_email': 'berlier.v@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/vberlier/tokenstream',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
+> A versatile token stream for handwritten parsers.
 
+```python
+from tokenstream import TokenStream
+
+def parse_sexp(stream: TokenStream):
+    """A basic S-expression parser."""
+    with stream.syntax(brace=r"\(|\)", number=r"\d+", name=r"\w+"):
+        brace, number, name = stream.expect(("brace", "("), "number", "name")
+        if brace:
+            return [parse_sexp(stream) for _ in stream.peek_until(("brace", ")"))]
+        elif number:
+            return int(number.value)
+        elif name:
+            return name.value
+
+print(parse_sexp(TokenStream("(hello (world 42))")))  # ['hello', ['world', 42]]
+```
+
+## Introduction
+
+Writing recursive-descent parsers by hand can be quite elegant but it's often a bit more verbose than expected, especially when it comes to handling indentation and reporting proper syntax errors. This package provides a powerful general-purpose token stream that addresses these issues and more.
+
+### Features
+
+- Define the set of recognizable tokens dynamically with regular expressions
+- Transparently skip over irrelevant tokens
+- Expressive API for matching, collecting, peeking, and expecting tokens
+- Clean error reporting with line numbers and column numbers
+- Contextual support for indentation-based syntax
+- Checkpoints for backtracking parsers
+- Works well with Python 3.10+ match statements
+
+Check out the [`examples`](https://github.com/vberlier/tokenstream/tree/main/examples) directory for practical examples.
+
+## Installation
+
+The package can be installed with `pip`.
+
+```bash
+pip install tokenstream
+```
+
+## Getting started
+
+You can define tokens with the `syntax()` method. The keyword arguments associate regular expression patterns to token types. The method returns a context manager during which the specified tokens will be recognized.
+
+```python
+stream = TokenStream("hello world")
+
+with stream.syntax(word=r"\w+"):
+    print([token.value for token in stream])  # ['hello', 'world']
+```
+
+Check out the full [API reference](https://vberlier.github.io/tokenstream/api_reference/) for more details.
+
+### Expecting tokens
+
+The token stream is iterable and will yield all the extracted tokens one after the other. You can also retrieve tokens from the token stream one at a time by using the `expect()` method.
+
+```python
+stream = TokenStream("hello world")
+
+with stream.syntax(word=r"\w+"):
+    print(stream.expect().value)  # "hello"
+    print(stream.expect().value)  # "world"
+```
+
+The `expect()` method lets you ensure that the extracted token matches a specified type and will raise an exception otherwise.
+
+```python
+stream = TokenStream("hello world")
+
+with stream.syntax(number=r"\d+", word=r"\w+"):
+    print(stream.expect("word").value)  # "hello"
+    print(stream.expect("number").value)  # UnexpectedToken: Expected number but got word 'world'
+```
+
+### Filtering the stream
+
+Newlines and whitespace are ignored by default. You can reject interspersed whitespace by intercepting the built-in `newline` and `whitespace` tokens.
+
+```python
+stream = TokenStream("hello world")
+
+with stream.syntax(word=r"\w+"), stream.intercept("newline", "whitespace"):
+    print(stream.expect("word").value)  # "hello"
+    print(stream.expect("word").value)  # UnexpectedToken: Expected word but got whitespace ' '
+```
+
+The opposite of the `intercept()` method is `ignore()`. It allows you to ignore tokens and handle comments pretty easily.
+
+```python
+stream = TokenStream(
+    """
+    # this is a comment
+    hello # also a comment
+    world
+    """
+)
+
+with stream.syntax(word=r"\w+", comment=r"#.+$"), stream.ignore("comment"):
+    print([token.value for token in stream])  # ['hello', 'world']
+```
+
+### Indentation
+
+To enable indentation you can use the `indent()` method. The stream will now yield balanced pairs of `indent` and `dedent` tokens when the indentation changes.
+
+```python
+source = """
+hello
+    world
+"""
+stream = TokenStream(source)
+
+with stream.syntax(word=r"\w+"), stream.indent():
+    stream.expect("word")
+    stream.expect("indent")
+    stream.expect("word")
+    stream.expect("dedent")
+```
+
+To prevent some tokens from triggering unwanted indentation changes you can use the `skip` argument.
+
+```python
+source = """
+hello
+        # some comment
+    world
+"""
+stream = TokenStream(source)
+
+with stream.syntax(word=r"\w+", comment=r"#.+$"), stream.indent(skip=["comment"]):
+    stream.expect("word")
+    stream.expect("comment")
+    stream.expect("indent")
+    stream.expect("word")
+    stream.expect("dedent")
+```
+
+### Checkpoints
+
+The `checkpoint()` method returns a context manager that resets the stream to the current token at the end of the `with` statement. You can use the returned `commit()` function to keep the state of the stream at the end of the `with` statement.
+
+```python
+stream = TokenStream("hello world")
+
+with stream.syntax(word=r"\w+"):
+    with stream.checkpoint():
+        print([token.value for token in stream])  # ['hello', 'world']
+    with stream.checkpoint() as commit:
+        print([token.value for token in stream])  # ['hello', 'world']
+        commit()
+    print([token.value for token in stream])  # []
+```
+
+### Match statements
+
+Match statements make it very intuitive to process tokens extracted from the token stream. If you're using Python 3.10+ give it a try and see if you like it.
+
+```python
+from tokenstream import TokenStream, Token
+
+def parse_sexp(stream: TokenStream):
+    """A basic S-expression parser that uses Python 3.10+ match statements."""
+    with stream.syntax(brace=r"\(|\)", number=r"\d+", name=r"\w+"):
+        match stream.expect_any(("brace", "("), "number", "name"):
+            case Token(type="brace"):
+                return [parse_sexp(stream) for _ in stream.peek_until(("brace", ")"))]
+            case Token(type="number") as number :
+                return int(number.value)
+            case Token(type="name") as name:
+                return name.value
+```
+
+## Contributing
+
+Contributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org/).
+
+```bash
+$ poetry install
+```
+
+You can run the tests with `poetry run pytest`.
+
+```bash
+$ poetry run pytest
+```
+
+The project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you're using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.
+
+```bash
+$ npm run watch
+$ npm run check
+$ npm run verifytypes
+```
+
+The code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).
+
+```bash
+$ poetry run isort tokenstream examples tests
+$ poetry run black tokenstream examples tests
+$ poetry run black --check tokenstream examples tests
+```
+
+---
+
+License - [MIT](https://github.com/vberlier/tokenstream/blob/main/LICENSE)
 
-setup(**setup_kwargs)
```

