# Comparing `tmp/imap_structure-0.1.5.tar.gz` & `tmp/imap_structure-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_structure-0.1.5.tar", max compression
+gzip compressed data, was "imap_structure-0.2.0.tar", max compression
```

## Comparing `imap_structure-0.1.5.tar` & `imap_structure-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       44 2023-05-18 03:04:19.021602 imap_structure-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-18 03:04:19.021602 imap_structure-0.1.5/imap_structure/__init__.py
--rw-r--r--   0        0        0    10965 2023-05-22 07:56:02.884600 imap_structure-0.1.5/imap_structure/body_structure.py
--rw-r--r--   0        0        0     5084 2023-05-18 08:39:35.872324 imap_structure-0.1.5/imap_structure/metadata.py
--rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.021602 imap_structure-0.1.5/imap_structure/parser.py
--rw-r--r--   0        0        0      540 2023-05-22 07:56:19.594593 imap_structure-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.5/setup.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-05-18 03:04:19.000000 imap_structure-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 03:04:19.000000 imap_structure-0.2.0/imap_structure/__init__.py
+-rw-r--r--   0        0        0    12316 2023-08-02 12:20:06.952016 imap_structure-0.2.0/imap_structure/body_structure.py
+-rw-r--r--   0        0        0     5084 2023-05-18 08:39:35.000000 imap_structure-0.2.0/imap_structure/metadata.py
+-rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.000000 imap_structure-0.2.0/imap_structure/parser.py
+-rw-r--r--   0        0        0      603 2023-08-02 12:20:41.819426 imap_structure-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 imap_structure-0.2.0/setup.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 imap_structure-0.2.0/PKG-INFO
```

### Comparing `imap_structure-0.1.5/imap_structure/body_structure.py` & `imap_structure-0.2.0/imap_structure/body_structure.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+import collections.abc
+import logging
 from dataclasses import dataclass
 from email import _header_value_parser as parser
 from functools import cached_property
 from typing import NamedTuple, Optional
 
 from pyparsing import (
     Literal,
-    ParseResults,
     Word,
     alphanums,
     nested_expr,
     nums,
     quoted_string,
     remove_quotes,
     replace_with,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def get_bs_parser():
     """
     Create a pyparsing parser that can parse RFC 9051 response into AST
     """
     NIL = Literal("NIL").set_parse_action(replace_with(None))
     integer = Word(nums).set_parse_action(lambda s, loc, toks: int(toks[0]))  # type: ignore
@@ -34,15 +37,15 @@
 
 
 bodystructure_parser = get_bs_parser()
 
 
 class MimeTree(NamedTuple):
     mime_type: list[str]
-    children: list[ParseResults]
+    children: list[collections.abc.Sequence]
 
 
 @dataclass
 class BodyPart:
     section: str
     mime_type: list[str]
     children: list["BodyPart"]
@@ -51,49 +54,53 @@
 @dataclass
 class BodyPartNonMultipart(BodyPart):
     # Basic fields
     # https://datatracker.ietf.org/doc/html/rfc9051#section-7.5.2-4.18.3
 
     body_type: str
     body_subtype: str
-    body_parameters: ParseResults
+    body_parameters: collections.abc.Sequence
     body_id: Optional[str]
     body_description: Optional[str]
     body_encoding: str
     body_size: int
 
     # Type-specific fields
     # https://datatracker.ietf.org/doc/html/rfc9051#section-7.5.2-4.32.2
 
-    message_rfc822_envelope: Optional[ParseResults] = None
+    message_rfc822_envelope: Optional[collections.abc.Sequence] = None
     text_lines: Optional[int] = None
 
     # Extension fields
     # https://datatracker.ietf.org/doc/html/rfc9051#section-7.5.2-4.32.5
 
     body_md5: Optional[str] = None
-    body_disposition: Optional[ParseResults] = None
-    body_language: Optional[str | ParseResults] = None
+    body_disposition: Optional[collections.abc.Sequence] = None
+    body_language: Optional[str | collections.abc.Sequence] = None
     body_location: Optional[str] = None
 
 
 @dataclass
 class BodyPartMultipart(BodyPart):
-    body_parameters: Optional[ParseResults] = None
-    body_disposition: Optional[ParseResults] = None
-    body_language: Optional[str | ParseResults] = None
+    body_parameters: Optional[collections.abc.Sequence] = None
+    body_disposition: Optional[collections.abc.Sequence] = None
+    body_language: Optional[str | collections.abc.Sequence] = None
     body_location: Optional[str] = None
 
 
 class BodyStructure:
     _raw: Optional[str]
-    parse_results: ParseResults
+    parse_results: collections.abc.Sequence
 
-    def __init__(self, parse_results: ParseResults, raw: Optional[str] = None):
+    def __init__(
+        self, parse_results: collections.abc.Sequence, raw: Optional[str] = None
+    ):
         self._raw = raw
+        if len(parse_results) == 0:
+            raise ValueError("parse_results must not be empty")
         self.parse_results = parse_results
 
     @cached_property
     def mime_tree(self) -> MimeTree:
         return extract_mime_tree(self.parse_results)
 
     @cached_property
@@ -106,53 +113,57 @@
 
     def attachments(self):
         for part in self.body_part.children:
             if not isinstance(part, BodyPartNonMultipart):
                 continue
             if part.body_disposition is None:
                 continue
-            disposition = part.body_disposition.as_list()
+            disposition = part.body_disposition
             if "attachment" not in disposition:
                 continue
-            if len(disposition) > 1 and isinstance(disposition[1], list):
+            if len(disposition) > 1 and isinstance(
+                disposition[1], collections.abc.Sequence
+            ):
                 filename_idx = disposition[1].index("filename")
                 if len(disposition[1]) > filename_idx + 1:
                     filename = disposition[1][filename_idx + 1]
                     # Should be parse_content_disposition_header but we use get_unstructured
                     yield str(parser.get_unstructured(filename))
 
     @cached_property
     def has_attachment(self) -> bool:
         return any(
             isinstance(part, BodyPartNonMultipart)
             and part.body_disposition is not None
-            and "attachment" in part.body_disposition.as_list()
+            and "attachment" in part.body_disposition
             for part in self.body_part.children
         )
 
 
 def parse_body_structure(body_structure: str) -> BodyStructure:
     """
     Parse BODYSTRUCTURE into AST.
     The body structure follows RFC 9051:
     https://www.rfc-editor.org/rfc/rfc9051.html#section-7.5.2-4.9
     """
     # parse it
     parsed_structure = bodystructure_parser.parse_string(body_structure)
+    parsed_structure = parsed_structure.as_list()
+    # as we actually use the parse result like if it's list
+    # we will convert it to nested list to avoid complicated ducktype check
 
     assert len(parsed_structure) == 1
     parsed_structure = parsed_structure[0]
 
-    assert isinstance(parsed_structure, ParseResults)
-
+    assert isinstance(parsed_structure, collections.abc.Sequence)
     return BodyStructure(parsed_structure, raw=body_structure)
 
 
 def extract_mime_tree(
-    parsed_structure: ParseResults,
+    parsed_structure: collections.abc.Sequence,
 ) -> MimeTree:
     """
     Extract body structure information from a parsed result.
 
     :returns: a tuple of (MIME type, children)
     """
     assert len(parsed_structure) > 0
@@ -161,14 +172,22 @@
         if len(parsed_structure) > 1:
             if isinstance(parsed_structure[1], str):
                 return (parsed_structure[:2], [])  # type: ignore
                 # Extension data may exists, which is ignored by us for now
                 # https://www.rfc-editor.org/rfc/rfc9051.html#section-7.5.2-4.10.7
         return (parsed_structure[:1], [])  # type: ignore
 
+    # For result from imapclient, the parts before MIME type is already collected as a list
+    if isinstance(parsed_structure, tuple) and isinstance(parsed_structure[0], list):
+        mime = parsed_structure[1]
+        if isinstance(mime, str):
+            return MimeTree([mime], parsed_structure[0])
+        if isinstance(mime, bytes):
+            raise NotImplementedError("all bytes should be decoded before parsing")
+    # For result from email.message_from_bytes, the parts before MIME type is flattened with rest of the structure
     result = []
     for part in parsed_structure:
         if isinstance(part, str):
             return MimeTree([part], result)
         result.append(part)
     return MimeTree([], result)
 
@@ -181,24 +200,24 @@
         section = f"{index + 1}"
     else:
         section = f"{prefix}.{index + 1}"
     return section
 
 
 def extract_non_multipart(
-    section: str, mime: list[str], parsed_structure: ParseResults
+    section: str, mime: list[str], parsed_structure: collections.abc.Sequence
 ):
     index = 0
 
     body_type, body_subtype = parsed_structure[index : index + 2]
     assert isinstance(body_type, str) and isinstance(body_subtype, str)
     index += 2
 
     body_parameters = parsed_structure[index]
-    assert isinstance(body_parameters, ParseResults)
+    assert isinstance(body_parameters, collections.abc.Sequence)
     index += 1
 
     body_id = parsed_structure[index]
     assert isinstance(body_id, str) or body_id is None
     index += 1
 
     body_description = parsed_structure[index]
@@ -266,92 +285,103 @@
     return result
 
 
 def extract_multipart(
     section: str,
     mime: list[str],
     children: list[BodyPart],
-    parsed_structure: ParseResults,
+    parsed_structure: collections.abc.Sequence,
 ) -> BodyPartMultipart:
     """
     Generate a tree for the body part of the message
     """
-    li = parsed_structure.as_list()
+    li = parsed_structure
     index = li.index(mime[-1])
     assert index > 0
 
     result = BodyPartMultipart(
         section=section,
         mime_type=mime,
         children=children,
     )
 
     if len(parsed_structure) <= index:
         return result
 
     body_parameters = parsed_structure[index]
-    assert isinstance(body_parameters, ParseResults)
+    assert isinstance(body_parameters, collections.abc.Sequence)
     result.body_parameters = body_parameters
     index += 1
     if len(parsed_structure) <= index:
         return result
 
     body_disposition = parsed_structure[index]
-    assert isinstance(body_disposition, ParseResults)
+    assert (
+        isinstance(body_disposition, collections.abc.Sequence)
+        or body_disposition is None
+    )
     result.body_disposition = body_disposition
     index += 1
     if len(parsed_structure) <= index:
         return result
 
     body_language = parsed_structure[index]
-    assert isinstance(body_language, ParseResults) or isinstance(body_language, str)
+    assert (
+        isinstance(body_language, collections.abc.Sequence)
+        or isinstance(body_language, str)
+        or body_language is None
+    )
     result.body_language = body_language
     index += 1
     if len(parsed_structure) <= index:
         return result
 
     body_location = parsed_structure[index]
     assert isinstance(body_location, str) or body_location is None
     result.body_location = body_location
     index += 1
 
     return result
 
 
-def extract_body_part(parsed_structure: ParseResults, section: str = "") -> BodyPart:
+def extract_body_part(
+    parsed_structure: collections.abc.Sequence, section: str = ""
+) -> BodyPart:
     """
     Generate a tree for the body part of the message
     """
     mime, parts = extract_mime_tree(parsed_structure)
     if len(parts) == 0:
         try:
             return extract_non_multipart(section, mime, parsed_structure)
         except:
+            logger.exception("Failed to extract non-multipart")
             return BodyPart(section, mime, [])
 
     children = [
         extract_body_part(part, section=child_section(section, i))
         for i, part in enumerate(parts)
     ]
 
     try:
         return extract_multipart(section, mime, children, parsed_structure)
     except:
+        logger.exception("Failed to extract multipart")
         return BodyPart(section, mime, children)
 
 
-def extract_text_sections(parsed_structure: BodyPart) -> list[tuple[str, str]]:
+def extract_text_sections(body_part: BodyPart) -> list[tuple[str, str]]:
     """
     Select text sections from given MIME structure
 
     :returns: a list of (section, text MIME subtype) tuples
     """
-    section = parsed_structure.section
-    mime = parsed_structure.mime_type
-    children = parsed_structure.children
+    section = body_part.section
+    mime = body_part.mime_type
+    children = body_part.children
 
     if mime[0] == "TEXT":
         return [(section, mime[1])]
 
     if len(children) == 0:
         return []
```

### Comparing `imap_structure-0.1.5/imap_structure/metadata.py` & `imap_structure-0.2.0/imap_structure/metadata.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.5/imap_structure/parser.py` & `imap_structure-0.2.0/imap_structure/parser.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.5/setup.py` & `imap_structure-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['pyparsing>=3.0.9,<4.0.0']
 
 setup_kwargs = {
     'name': 'imap-structure',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': 'IMAP BODYSTRUCTURE parser',
     'long_description': '# imap-structure\n\nIMAP BODYSTRUCTURE parser\n',
     'author': 'Kiruya Momochi',
     'author_email': '65301509+kiruyamomochi@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/KiruyaMomochi/pyimap-structure',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

