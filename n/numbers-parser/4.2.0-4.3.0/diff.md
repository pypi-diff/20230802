# Comparing `tmp/numbers_parser-4.2.0.tar.gz` & `tmp/numbers_parser-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.2.0.tar", max compression
+gzip compressed data, was "numbers_parser-4.3.0.tar", max compression
```

## Comparing `numbers_parser-4.2.0.tar` & `numbers_parser-4.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.2.0/LICENSE.rst
--rw-r--r--   0        0        0    21100 2023-07-21 16:51:45.519938 numbers_parser-4.2.0/README.md
--rw-r--r--   0        0        0     2112 2023-07-21 16:52:35.915547 numbers_parser-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.2.0/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4336 2023-07-23 15:54:51.161098 numbers_parser-4.2.0/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.2.0/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.2.0/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    22973 2023-07-27 06:57:17.175853 numbers_parser-4.2.0/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    29536 2023-07-23 15:54:51.340254 numbers_parser-4.2.0/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1823 2023-07-25 11:49:15.661140 numbers_parser-4.2.0/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.2.0/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0   134819 2022-07-21 08:13:02.000000 numbers_parser-4.2.0/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    18786 2023-07-28 10:14:11.778889 numbers_parser-4.2.0/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.2.0/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.2.0/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.2.0/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.2.0/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.2.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.2.0/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.2.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.2.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.2.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.2.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.2.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.2.0/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.2.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.2.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.2.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.2.0/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.2.0/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.2.0/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.2.0/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.2.0/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    87056 2023-07-28 10:51:47.125210 numbers_parser-4.2.0/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.2.0/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    22277 1970-01-01 00:00:00.000000 numbers_parser-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.3.0/LICENSE.rst
+-rw-r--r--   0        0        0    23133 2023-08-02 18:06:36.519270 numbers_parser-4.3.0/README.md
+-rw-r--r--   0        0        0     2130 2023-08-02 18:04:07.008254 numbers_parser-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.3.0/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4336 2023-08-02 13:30:28.000000 numbers_parser-4.3.0/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.3.0/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.3.0/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    24971 2023-08-02 17:34:50.770915 numbers_parser-4.3.0/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    28441 2023-08-02 17:30:54.921525 numbers_parser-4.3.0/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1875 2023-08-02 06:59:20.616439 numbers_parser-4.3.0/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.3.0/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.3.0/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    20435 2023-08-02 13:27:23.000000 numbers_parser-4.3.0/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.3.0/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.3.0/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.3.0/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.3.0/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.3.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.3.0/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.3.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.3.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.3.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.3.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.3.0/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.3.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.3.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.3.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.3.0/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.3.0/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.3.0/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.3.0/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.3.0/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    90563 2023-08-02 13:27:31.000000 numbers_parser-4.3.0/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.3.0/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    24349 1970-01-01 00:00:00.000000 numbers_parser-4.3.0/PKG-INFO
```

### Comparing `numbers_parser-4.2.0/LICENSE.rst` & `numbers_parser-4.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/README.md` & `numbers_parser-4.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Formula evaluation relies on Numbers storing current values which should usually be the case. Formulas themselves rather than the computed values can optionally be extracted. [Style support](#styles) is somewhat limited, but has grown significantly as of version 4.0.
 
 ## API changes in version 4.0
 
 To better partition cell styles, background image data which was supported in earlier versions through the methods `image_data` and `image_filename` is now part of the new `cell_style` property. Using the deprecated methods `image_data` and `image_filename` will issue a `DeprecationWarning` if used.The legacy methods will be removed in a future version of numbers-parser.
 
-`NumberCell` cell types return [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html) types rather than `float`. These are created in a [decimal128](https://en.wikipedia.org/wiki/Decimal128_floating-point_format) context to preserve the precision used by Numbers. Previously, using float resulted in rounding errors in unpacking internal numbers.
+`NumberCell` cell values are now limited to 15 significant figues to match the implementation of floating point numbers in Apple Numbers. For example, the value `1234567890123456` is rounded to `1234567890123460` in the same was as in Numbers. Previously, using native `float` with no checking resulted in rounding errors in unpacking internal numbers. Attempting to write a number with too many significant digits results in a `RuntimeWarning`.
 
 ## Installation
 
 ``` bash
 python3 -m pip install numbers-parser
 ```
 
@@ -102,18 +102,15 @@
 print("Cell A1 contains", table.cell(0, 0))
 # Excel/Numbers-style cell references
 print("Cell C2 contains", table.cell("C2"))
 ```
 
 ### Merged cells
 
-When extracting data using ```rows()``` merged cells are ignored since only text values
-are returned. The ```cell()``` method of ```Table``` objects returns a ```Cell``` type
-object which is typed by the type of cell in the Numbers table. ```MergeCell``` objects
-indicates cells removed in a merge.
+When extracting data using `rows()` merged cells are ignored since only text values are returned. The `cell()` method of `Table` objects returns a `Cell` type object which is typed by the type of cell in the Numbers table. `MergeCell` objects indicates cells removed in a merge. The remaining `Cell` has a `bool` property `is_merged` which is `True` if the cell is the result of a merge. Such cells return a `tuple` for their `size` property indicating the number of rows and columns in the merged cell. Unmerged cells return a `size` of `None`.
 
 ``` python
 doc = Document("my-spreadsheet.numbers")
 sheets = doc.sheets
 tables = sheets["Sheet 1"].tables
 table = tables["Table 1"]
 
@@ -218,14 +215,41 @@
 
 ``` python
 cell = table.cell("B1")
 with open (cell.style.bg_image.filename, "wb") as f:
     f.write(cell.style.bg_image.data)
 ```
 
+### Borders
+
+`numbers-parser` supports reading and writing cell borders, though the interface for each differs. Individual cells can have each of their four borders tested, but when drawing new borders, these are set for the table to allow for drawing borders across multiple cells. Setting the border of merged cells is not possible unless the edge of the cells is at the end of the merged region.
+
+Borders are represeted using the `Border` class that can be initialised with line width, color and line style:
+
+``` python
+border = Border(4.0, RGB(0, 162, 255), "solid"))
+```
+
+Valid values for the line `style` parameter are `"solid"`, `"dashes"`, `"dots"` and `"none"`.
+
+#### Reading Cell Borders
+
+Cells have a property `border` which itself has the properties `top`, `right`, `bottom` and `left`, each of which is a `Border` class representing the line type for that cell. Cells with no border set at all, and merged cells which are inside the range of the merge return `None` for these cells. The absence of a specified border is different from no border in Numbers which is a valid `Border` class with `style="none"`.
+
+#### Writing Cell Borders
+
+The `Table` method `set_cell_border()` sets the border for a cell edge or a range of cells:
+
+``` python
+table.set_cell_border("C1", ["top", "left"], Border(0.0, RGB(0, 0, 0), "none"))
+table.set_cell_border(0, 4, "right", Border(1.0, RGB(0, 0, 0), "solid"), 3)
+```
+
+The last positional parameter specifies the length of the border and defaults to 1. A single call to `set_cell_border()` can set the borders to one or more sides of the cell as above. Like `Table.write()`, `set_cell_border()` supports both row/column and Excel-style cell references.
+
 ## Writing Numbers files
 
 Whilst support for writing numbers files has been stable since version 3.4.0, you are highly recommened not to overwrite working Numbers files and instead save data to a new file.
 
 ### Limitations
 
 Current limitations to write support are:
```

### Comparing `numbers_parser-4.2.0/pyproject.toml` & `numbers_parser-4.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.2.0"
+version = "4.3.0"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
 pendulum = "^2.1.2"
 protobuf = "^4.21.1"
 python = "^3.8"
 python-snappy = "^0.6.1"
 regex = "^2022.9.13"
 roman = "^3.3"
+sigfig = "^1.3.2"
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^22.10.0", allow-prereleases = true}
 pylama = "^8.4.1"
 pytest = "^7.2.0"
 pytest-check = "^1.0.10"
 pytest-console-scripts = "^1.3.1"
```

### Comparing `numbers_parser-4.2.0/src/numbers_parser/__init__.py` & `numbers_parser-4.3.0/src/numbers_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.3.0/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.3.0/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/bullets.py` & `numbers_parser-4.3.0/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/cell.py` & `numbers_parser-4.3.0/src/numbers_parser/cell.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-import warnings
+import sigfig
 
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
 from numbers_parser.generated.TSWPArchives_pb2 import (
     ParagraphStylePropertiesArchive as ParagraphStyle,
 )
 from numbers_parser.exceptions import UnsupportedError, UnsupportedWarning
 from numbers_parser.cell_storage import CellType, CellStorage
@@ -12,22 +12,25 @@
     DEFAULT_FONT,
     DEFAULT_FONT_SIZE,
     DEFAULT_ALIGNMENT,
     DEFAULT_TEXT_INSET,
     DEFAULT_BORDER_WIDTH,
     DEFAULT_BORDER_COLOR,
     DEFAULT_BORDER_STYLE,
+    MAX_SIGNIFICANT_DIGITS,
 )
 
-from dataclasses import dataclass
 from collections import namedtuple
+from dataclasses import dataclass
+from datetime import datetime as builtin_datetime, timedelta as builtin_timedelta
 from enum import IntEnum
 from functools import lru_cache
-from pendulum import duration, Duration, DateTime
+from pendulum import duration, Duration, DateTime, instance as pendulum_instance
 from typing import Any, List, Tuple, Union
+from warnings import warn
 
 
 class BackgroundImage:
     def __init__(self, image_data: bytes = None, filename: str = None):
         self._data = image_data
         self._filename = filename
 
@@ -350,103 +353,152 @@
     def left(self, value):
         if self._left is None:
             self._left = value
         elif value._order > self._left._order:
             self._left = value
 
 
+class MergeReference:
+    """Cell reference for cells eliminated by a merge"""
+
+    def __init__(self, row_start: int, col_start: int, row_end: int, col_end: int):
+        self.rect = (row_start, col_start, row_end, col_end)
+
+
+class MergeAnchor:
+    """Cell reference for the merged cell"""
+
+    def __init__(self, size: Tuple):
+        self.size = size
+
+
 class Cell:
     @classmethod
     def empty_cell(cls, table_id: int, row_num: int, col_num: int, model: object):
-        row_col = (row_num, col_num)
-        merge_cells = model.merge_cell_ranges(table_id)
-        is_merged = row_col in merge_cells
-
-        if is_merged and merge_cells[row_col]["merge_type"] == "ref":
-            cell = MergedCell(*merge_cells[row_col]["rect"], row_num, col_num)
-        else:
-            cell = EmptyCell(row_num, col_num)
-        cell.size = None
+        cell = EmptyCell(row_num, col_num)
         cell._model = model
         cell._table_id = table_id
-        cell._style = None
+        merge_cells = model.merge_cells(table_id)
+        cell._set_merge(merge_cells.get((row_num, col_num)))
+
         return cell
 
     @classmethod
-    def from_storage(cls, cell_storage: CellStorage):  # noqa: C901
-        row_col = (cell_storage.row_num, cell_storage.col_num)
-        merge_cells = cell_storage.model.merge_cell_ranges(cell_storage.table_id)
-        is_merged = row_col in merge_cells
+    def merged_cell(cls, table_id: int, row_num: int, col_num: int, model: object):
+        cell = MergedCell(row_num, col_num)
+        cell._model = model
+        cell._table_id = table_id
+        merge_cells = model.merge_cells(table_id)
+        cell._set_merge(merge_cells.get((row_num, col_num)))
+        return cell
 
+    @classmethod
+    def from_storage(cls, cell_storage: CellStorage):
         if cell_storage.type == CellType.EMPTY:
             cell = EmptyCell(cell_storage.row_num, cell_storage.col_num)
         elif cell_storage.type == CellType.NUMBER:
-            cell = NumberCell(*row_col, cell_storage.value)
+            cell = NumberCell(cell_storage.row_num, cell_storage.col_num, cell_storage.value)
         elif cell_storage.type == CellType.TEXT:
-            cell = TextCell(*row_col, cell_storage.value)
+            cell = TextCell(cell_storage.row_num, cell_storage.col_num, cell_storage.value)
         elif cell_storage.type == CellType.DATE:
-            cell = DateCell(*row_col, cell_storage.value)
+            cell = DateCell(cell_storage.row_num, cell_storage.col_num, cell_storage.value)
         elif cell_storage.type == CellType.BOOL:
-            cell = BoolCell(*row_col, cell_storage.value)
+            cell = BoolCell(cell_storage.row_num, cell_storage.col_num, cell_storage.value)
         elif cell_storage.type == CellType.DURATION:
             value = duration(seconds=cell_storage.value)
-            cell = DurationCell(*row_col, value)
+            cell = DurationCell(cell_storage.row_num, cell_storage.col_num, value)
         elif cell_storage.type == CellType.ERROR:
-            cell = ErrorCell(*row_col)
+            cell = ErrorCell(cell_storage.row_num, cell_storage.col_num)
         elif cell_storage.type == CellType.RICH_TEXT:
-            cell = RichTextCell(*row_col, cell_storage.value)
+            cell = RichTextCell(cell_storage.row_num, cell_storage.col_num, cell_storage.value)
         else:
             raise UnsupportedError(
                 f"Unsupported cell type {cell_storage.type} "
                 + f"@:({cell_storage.row_num},{cell_storage.col_num})"
             )
 
         cell._table_id = cell_storage.table_id
         cell._model = cell_storage.model
         cell._storage = cell_storage
         cell._formula_key = cell_storage.formula_id
-        cell._style = None
+        merge_cells = cell_storage.model.merge_cells(cell_storage.table_id)
+        cell._set_merge(merge_cells.get((cell_storage.row_num, cell_storage.col_num)))
+        return cell
 
-        if is_merged and merge_cells[row_col]["merge_type"] == "source":
-            cell.is_merged = True
-            cell.size = merge_cells[row_col]["size"]
-            right_merged = cell.size[0] > 1
-            bottom_merged = cell.size[1] > 1
-            cell._border = CellBorder(False, right_merged, bottom_merged, False)
+    @classmethod
+    def from_value(cls, row_num: int, col_num: int, value):
+        # TODO: write needs to retain/init the border
+        if isinstance(value, str):
+            return TextCell(row_num, col_num, value)
+        elif isinstance(value, bool):
+            return BoolCell(row_num, col_num, value)
+        elif isinstance(value, int):
+            return NumberCell(row_num, col_num, value)
+        elif isinstance(value, float):
+            rounded_value = sigfig.round(value, sigfigs=MAX_SIGNIFICANT_DIGITS, warn=False)
+            if rounded_value != value:
+                warn(
+                    f"'{value}' rounded to {MAX_SIGNIFICANT_DIGITS} significant digits",
+                    RuntimeWarning,
+                )
+            return NumberCell(row_num, col_num, rounded_value)
+        elif isinstance(value, builtin_datetime) or isinstance(value, DateTime):
+            return DateCell(row_num, col_num, pendulum_instance(value))
+        elif isinstance(value, builtin_timedelta) or isinstance(value, Duration):
+            return DurationCell(row_num, col_num, value)
         else:
-            cell._border = CellBorder()
-
-        return cell
+            raise ValueError("Can't determine cell type from type " + type(value).__name__)
 
     def __init__(self, row_num: int, col_num: int, value):
         self._value = value
         self.row = row_num
         self.col = col_num
-        self.size = (1, 1)
-        self.is_merged = False
         self.is_bulleted = False
         self._formula_key = None
         self._storage = None
         self._style = None
 
+    def _set_merge(self, merge_ref):
+        if isinstance(merge_ref, MergeAnchor):
+            self.is_merged = True
+            self.size = merge_ref.size
+            self._border = CellBorder()
+        elif isinstance(merge_ref, MergeReference):
+            self.is_merged = False
+            self.size = None
+            self.row_start = merge_ref.rect[0]
+            self.col_start = merge_ref.rect[1]
+            self.row_end = merge_ref.rect[2]
+            self.col_end = merge_ref.rect[3]
+            self.merge_range = xl_range(*merge_ref.rect)
+            top_merged = self.row > self.row_start
+            right_merged = self.col < self.col_end
+            bottom_merged = self.row < self.row_end
+            left_merged = self.col > self.col_start
+            self._border = CellBorder(top_merged, right_merged, bottom_merged, left_merged)
+        else:
+            self.is_merged = False
+            self.size = (1, 1)
+            self._border = CellBorder()
+
     @property
     def image_filename(self):
-        warnings.warn(
+        warn(
             "image_filename is deprecated and will be removed in the future. "
             + "Please use the style property",
             DeprecationWarning,
         )
         if self.style is not None and self.style.bg_image is not None:
             return self.style.bg_image.filename
         else:
             return None
 
     @property
     def image_data(self):
-        warnings.warn(
+        warn(
             "image_data is deprecated and will be removed in the future. "
             + "Please use the style property",
             DeprecationWarning,
         )
         if self.style is not None and self.style.bg_image is not None:
             return self.style.bg_image.data
         else:
@@ -482,26 +534,27 @@
                 self._model, self._table_id, EMPTY_STORAGE_BUFFER, self.row, self.col
             )
         if self._style is None:
             self._style = Style.from_storage(self._storage, self._model)
         return self._style
 
     @style.setter
-    def style(self, style):
-        self._style = style
+    def style(self, _):
+        warn("cell style cannot be set; use Table.set_cell_style() instead", UnsupportedWarning)
 
     @property
     def border(self):
         self._model.extract_strokes(self._table_id)
         return self._border
 
     @border.setter
     def border(self, _):
-        warnings.warn(
-            "cell border values cannot be set; use Table.add_border() instead", UnsupportedWarning
+        warn(
+            "cell border values cannot be set; use Table.set_cell_border() instead",
+            UnsupportedWarning,
         )
 
 
 class NumberCell(Cell):
     def __init__(self, row_num: int, col_num: int, value: float):
         self._type = TSTArchives.numberCellType
         super().__init__(row_num, col_num, value)
@@ -558,15 +611,14 @@
     pass
 
 
 class EmptyCell(Cell):
     def __init__(self, row_num: int, col_num: int):
         super().__init__(row_num, col_num, None)
         self._type = None
-        self._border = CellBorder()
 
     @property
     def value(self):
         return None
 
 
 class BoolCell(Cell):
@@ -607,30 +659,20 @@
 
     @property
     def value(self):
         return None
 
 
 class MergedCell(Cell):
-    def __init__(
-        self, row_start: int, col_start: int, row_end: int, col_end: int, row_num: int, col_num: int
-    ):
+    def __init__(self, row_num: int, col_num: int):
         super().__init__(row_num, col_num, None)
-        self.value = None
-        self.row_start = row_start
-        self.row_end = row_end
-        self.col_start = col_start
-        self.col_end = col_end
-        self.is_merged = False
-        self.merge_range = xl_range(row_start, col_start, row_end, col_end)
-        top_merged = row_num > row_start
-        right_merged = col_num < col_end
-        bottom_merged = row_num < row_end
-        left_merged = col_num > col_start
-        self._border = CellBorder(top_merged, right_merged, bottom_merged, left_merged)
+
+    @property
+    def value(self):
+        return None
 
 
 # Cell reference conversion from  https://github.com/jmcnamara/XlsxWriter
 # Copyright (c) 2013-2021, John McNamara <jmcnamara@cpan.org>
 range_parts = re.compile(r"(\$?)([A-Z]{1,3})(\$?)(\d+)")
```

### Comparing `numbers_parser-4.2.0/src/numbers_parser/cell_storage.py` & `numbers_parser-4.3.0/src/numbers_parser/cell_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,42 @@
-import decimal
 import logging
 import math
 import re
+import sigfig
 
 from collections import OrderedDict
-
 from fractions import Fraction
 from functools import lru_cache
 from pendulum import datetime, duration
 from struct import unpack
 from typing import Tuple
 from warnings import warn
 
 from numbers_parser import __name__ as numbers_parser_name
-from numbers_parser.experimental import _experimental_features
 from numbers_parser.constants import (
     EPOCH,
     PACKAGE_ID,
     DECIMAL_PLACES_AUTO,
     CellType,
     CellPadding,
     DurationStyle,
     DurationUnits,
     FormatType,
     SECONDS_IN_HOUR,
     SECONDS_IN_DAY,
     SECONDS_IN_WEEK,
+    MAX_SIGNIFICANT_DIGITS,
 )
 from numbers_parser.exceptions import UnsupportedError, UnsupportedWarning
 from numbers_parser.numbers_uuid import NumbersUUID
 from numbers_parser.generated import TSTArchives_pb2 as TSTArchives
 
 logger = logging.getLogger(numbers_parser_name)
 debug = logger.debug
 
-DECIMAL128_CONTEXT = decimal.Context(
-    prec=34,
-    rounding=decimal.ROUND_HALF_EVEN,
-    Emin=-6143,
-    Emax=6144,
-    capitals=1,
-    clamp=1,
-    flags=[],
-    traps=[],
-)
-
 DATETIME_FIELD_MAP = OrderedDict(
     [
         ("a", lambda x: x.strftime("%p").lower()),
         ("EEEE", "%A"),
         ("EEE", "%a"),
         ("yyyy", "%Y"),
         ("yy", "%y"),
@@ -151,15 +139,15 @@
         # self.comment_id = None
         # self.import_warning_id = None
 
         if buffer is None:
             return
 
         version = buffer[0]
-        if version != 5:  # pragma: no cover
+        if version != 5:
             raise UnsupportedError(f"Cell storage version {version} is unsupported")
 
         offset = 12
         flags = unpack("<i", buffer[8:12])[0]
 
         if flags & 0x1:
             self.d128 = unpack_decimal128(buffer[offset : offset + 16])
@@ -288,28 +276,23 @@
     @property
     @lru_cache(maxsize=None)
     def image_data(self) -> Tuple[bytes, str]:
         """Return the background image data for a cell or None if no image"""
         if self.cell_style_id is None:
             return None
         style = self.model.table_style(self.table_id, self.cell_style_id)
-        if not style.cell_properties.cell_fill.HasField("image"):  # pragma: no cover
+        if not style.cell_properties.cell_fill.HasField("image"):
             return None
 
         image_id = style.cell_properties.cell_fill.image.imagedata.identifier
         datas = self.model.objects[PACKAGE_ID].datas
-        image_file_names = [x.file_name for x in datas if x.identifier == image_id]
-        if len(image_file_names) == 0:  # pragma: no cover
-            warn(f"No image found with ID {image_id}", UnsupportedWarning)
-            return None
-
-        image_path_name = [
-            x for x in self.model.objects.file_store.keys() if x == f"Data/{image_file_names[0]}"
-        ][0]
-        return (self.model.objects.file_store[image_path_name], image_file_names[0])
+        image_filename = [x.file_name for x in datas if x.identifier == image_id][0]
+        all_paths = self.model.objects.file_store.keys()
+        image_pathname = [x for x in all_paths if x == f"Data/{image_filename}"][0]
+        return (self.model.objects.file_store[image_pathname], image_filename)
 
     def custom_format(self) -> str:
         if self.text_format_id is not None and self.type == CellType.TEXT:
             format = self.model.table_format(self.table_id, self.text_format_id)
         elif self.currency_format_id is not None:
             format = self.model.table_format(self.table_id, self.currency_format_id)
         elif self.num_format_id is not None:
@@ -330,25 +313,18 @@
                 else:
                     formatted_value = float_to_fraction(self.d128, accuracy)
             elif custom_format.format_type == FormatType.CUSTOM_TEXT:
                 formatted_value = decode_text_format(
                     custom_format,
                     self.model.table_string(self.table_id, self.string_id),
                 )
-            elif (
-                custom_format.format_type == FormatType.CUSTOM_NUMBER
-                or custom_format.format_type == FormatType.CUSTOM_CURRENCY
-            ):
+            else:
                 formatted_value = decode_number_format(
                     custom_format, self.d128, format_map[format_uuid].name
                 )
-            else:
-                raise UnsupportedError(  # pragma: no cover
-                    f"Unexpected custom format type {custom_format.format_type}"
-                )
         elif format.format_type == FormatType.DECIMAL:
             return format_decimal(self.d128, format)
         elif format.format_type == FormatType.BOOLEAN:
             return "TRUE" if self.value else "FALSE"
         else:
             formatted_value = str(self.value)
         return formatted_value
@@ -358,16 +334,19 @@
         if format.HasField("custom_uid"):
             format_uuid = NumbersUUID(format.custom_uid).hex
             format_map = self.model.custom_format_map()
             custom_format = format_map[format_uuid].default_format
             custom_format_string = custom_format.custom_format_string
             if custom_format.format_type == FormatType.CUSTOM_DATE:
                 formatted_value = decode_date_format(custom_format_string, self.datetime)
-            else:  # pragma: no cover
-                raise UnsupportedError(f"Unexpected custom format type {custom_format.format_type}")
+            else:
+                warn(
+                    f"Unexpected custom format type {custom_format.format_type}", UnsupportedWarning
+                )
+                return ""
         else:
             formatted_value = decode_date_format(format.date_time_format, self.datetime)
         return formatted_value
 
     def duration_format(self) -> str:  # noqa: C901
         format = self.model.table_format(self.table_id, self.duration_format_id)
 
@@ -437,36 +416,23 @@
         if duration_style == DurationStyle.COMPACT:
             duration_str = re.sub(r":(\d\d\d)$", r".\1", duration_str)
 
         return duration_str
 
 
 def unpack_decimal128(buffer: bytearray) -> float:
-    if _experimental_features():
-        with decimal.localcontext(DECIMAL128_CONTEXT) as ctx:  # noqa: W0612
-            mantissa = decimal.Decimal(buffer[14] & 1)
-            exp = (((buffer[15] & 0x7F) << 7) | (buffer[14] >> 1)) - 0x1820
-            for i in range(13, -1, -1):
-                mantissa = mantissa * 256 + buffer[i]
-            sign = 1 if buffer[15] & 0x80 else 0
-            if sign == 1:
-                mantissa = -mantissa
-            value = mantissa * decimal.Decimal(10) ** decimal.Decimal(exp)
-            return value
-    else:
-        exp = (((buffer[15] & 0x7F) << 7) | (buffer[14] >> 1)) - 0x1820
-        mantissa = buffer[14] & 1
-        mantissa = buffer[14] & 1
-        for i in range(13, -1, -1):
-            mantissa = mantissa * 256 + buffer[i]
-        sign = 1 if buffer[15] & 0x80 else 0
-        if sign == 1:
-            mantissa = -mantissa
-        value = mantissa * 10**exp
-        return float(value)
+    exp = (((buffer[15] & 0x7F) << 7) | (buffer[14] >> 1)) - 0x1820
+    mantissa = buffer[14] & 1
+    for i in range(13, -1, -1):
+        mantissa = mantissa * 256 + buffer[i]
+    sign = 1 if buffer[15] & 0x80 else 0
+    if sign == 1:
+        mantissa = -mantissa
+    value = mantissa * 10**exp
+    return float(value)
 
 
 def days_occurred_in_month(value: datetime) -> str:
     """Return how many times the day of the datetime value has fallen in the month"""
     n_days = int((value - value.replace(day=1)).days / 7) + 1
     return str(n_days)
 
@@ -474,16 +440,17 @@
 def decode_date_format_field(field: str, value: datetime) -> str:
     if field in DATETIME_FIELD_MAP:
         s = DATETIME_FIELD_MAP[field]
         if callable(s):
             return s(value)
         else:
             return value.strftime(s)
-    else:  # pragma: no cover
-        raise UnsupportedError(f"Unsupported field code '{field}'")
+    else:
+        warn(f"Unsupported field code '{field}'", UnsupportedWarning)
+        return ""
 
 
 def decode_date_format(format, value):
     """Parse a custom date format string and return a formatted datetime value"""
     chars = [*format]
     index = 0
     in_string = False
@@ -572,17 +539,15 @@
 
     if format.currency_code != "":
         # Replace currency code with symbol and no-break space
         custom_format_string = custom_format_string.replace(
             "\u00a4", format.currency_code + "\u00a0"
         )
 
-    if (
-        match := re.search(r"([#0.,]+(E[+]\d+)?)", custom_format_string)
-    ) is None:  # pragma: no cover
+    if (match := re.search(r"([#0.,]+(E[+]\d+)?)", custom_format_string)) is None:
         warn(
             f"Can't parse format string '{custom_format_string}'; skipping",
             UnsupportedWarning,
         )
         return custom_format_string
     format_spec = match.group(1)
     scientific_spec = match.group(2)
@@ -641,17 +606,14 @@
         else:
             int_pad = CellPadding.SPACE
             int_width = len(int_part)
     else:
         int_pad = None
         int_width = num_integers
 
-    # if num_integers == 0 and dec_pad == CellPadding.SPACE:
-    #     dec_pad = CellPadding.ZERO
-
     # Formatting integer zero:
     #   Blank (padded if needed) if int_pad is SPACE and no decimals
     #   No leading zero if:
     #     int_pad is NONE, dec_pad is SPACE
     #     int_pad is SPACE, dec_pad is SPACE
     #     int_pad is SPACE, dec_pad is ZERO
     #     int_pad is SPACE, dec_pad is NONE if num decimals < decimals length
@@ -683,45 +645,53 @@
             formatted_value = f"{integer:,}"
         else:
             formatted_value = str(integer)
 
     if num_decimals:
         if dec_pad == CellPadding.ZERO:
             formatted_value += "." + f"{decimal:,.{dec_width}f}"[2:]
-        # elif dec_pad == CellPadding.SPACE and decimal == 0:
-        #     formatted_value += ".".ljust(dec_width + 1)
         elif dec_pad == CellPadding.SPACE:
             decimal_str = str(decimal)[2:]
             formatted_value += "." + decimal_str.ljust(dec_width)
         elif decimal or num_integers == 0:
             formatted_value += "." + str(decimal)[2:]
 
     formatted_value = custom_format_string.replace(format_spec, formatted_value)
     return expand_quotes(formatted_value)
 
 
-def format_decimal(value, format):
+def format_decimal(value: float, format) -> str:
     if value < 0 and format.negative_style == 1:
         accounting_style = False
         value = -value
     elif value < 0 and format.negative_style >= 2:
         accounting_style = True
         value = -value
     else:
         accounting_style = False
     if format.show_thousands_separator:
         thousands = ","
     else:
         thousands = ""
+
     if value.is_integer() and format.decimal_places >= DECIMAL_PLACES_AUTO:
         formatted_value = f"{int(value):{thousands}}"
-    elif format.decimal_places >= DECIMAL_PLACES_AUTO:
-        formatted_value = f"{value:{thousands}}"
     else:
-        formatted_value = f"{value:{thousands}.{format.decimal_places}f}"
+        if format.decimal_places >= DECIMAL_PLACES_AUTO:
+            formatted_value = str(sigfig.round(value, MAX_SIGNIFICANT_DIGITS, warn=False))
+        else:
+            formatted_value = sigfig.round(value, MAX_SIGNIFICANT_DIGITS, type=str, warn=False)
+            formatted_value = sigfig.round(
+                formatted_value, decimals=format.decimal_places, type=str
+            )
+        if format.show_thousands_separator:
+            formatted_value = sigfig.round(formatted_value, spacer=",", spacing=3, type=str)
+            (integer, decimal) = formatted_value.split(".")
+            formatted_value = integer + "." + decimal.replace(",", "")
+
     if accounting_style:
         return f"({formatted_value})"
     else:
         return formatted_value
 
 
 def float_to_fraction(value: float, denominator: int) -> str:
```

### Comparing `numbers_parser-4.2.0/src/numbers_parser/constants.py` & `numbers_parser-4.3.0/src/numbers_parser/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from enum import IntEnum
 from pendulum import datetime
 from pkg_resources import resource_filename
 
 # New document defaults
 DEFAULT_DOCUMENT = resource_filename(__name__, os.path.join("data", "empty.numbers"))
-DEFAULT_COLUMN_COUNT = 5
+DEFAULT_COLUMN_COUNT = 8
 DEFAULT_COLUMN_WIDTH = 98.0
 DEFAULT_PRE_BNC_BYTES = "🤠".encode("utf-8")  # Yes, really!
-DEFAULT_ROW_COUNT = 10
+DEFAULT_ROW_COUNT = 12
 DEFAULT_ROW_HEIGHT = 20.0
+DEFAULT_NUM_HEADERS = 1
 DEFAULT_TABLE_OFFSET = 80.0
 DEFAULT_TILE_SIZE = 256
 
 # Style defaults
 DEFAULT_ALIGNMENT = ("auto", "top")
 DEFAULT_BORDER_WIDTH = 0.35
 DEFAULT_BORDER_COLOR = (0, 0, 0)
@@ -25,14 +26,15 @@
 EMPTY_STORAGE_BUFFER = b"\x05\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
 
 # Numbers limits
 MAX_TILE_SIZE = 256
 MAX_ROW_COUNT = 1000000
 MAX_COL_COUNT = 1000
 MAX_HEADER_COUNT = 5
+MAX_SIGNIFICANT_DIGITS = 15
 
 # Root object IDs
 DOCUMENT_ID = 1
 PACKAGE_ID = 2
 
 # System constants
 EPOCH = datetime(2001, 1, 1)
```

### Comparing `numbers_parser-4.2.0/src/numbers_parser/containers.py` & `numbers_parser-4.3.0/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/document.py` & `numbers_parser-4.3.0/src/numbers_parser/document.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,79 @@
-from datetime import datetime as builtin_datetime, timedelta as builtin_timedelta
 from functools import lru_cache
-from pendulum import DateTime, Duration, instance as pendulum_instance
 from typing import Union, Generator, Tuple
+from warnings import warn
 
 from numbers_parser.containers import ItemsList
 from numbers_parser.model import _NumbersModel
 from numbers_parser.file import write_numbers_file
-from numbers_parser.constants import MAX_ROW_COUNT, MAX_COL_COUNT, MAX_HEADER_COUNT
+from numbers_parser.constants import (
+    MAX_ROW_COUNT,
+    MAX_COL_COUNT,
+    MAX_HEADER_COUNT,
+    DEFAULT_NUM_HEADERS,
+    DEFAULT_COLUMN_COUNT,
+    DEFAULT_ROW_COUNT,
+)
 from numbers_parser.cell import (
-    EmptyCell,
-    BoolCell,
-    NumberCell,
-    TextCell,
-    DurationCell,
-    DateCell,
     Cell,
     MergedCell,
     xl_cell_to_rowcol,
-    xl_range,
     Style,
     Border,
 )
 from numbers_parser.cell_storage import CellStorage
-from numbers_parser.constants import DEFAULT_COLUMN_COUNT, DEFAULT_ROW_COUNT
 
 
 class Document:
-    def __init__(self, filename=None):
+    def __init__(
+        self,
+        filename: str = None,
+        sheet_name: str = None,
+        table_name: str = None,
+        num_header_rows: int = None,
+        num_header_cols: int = None,
+        num_rows: int = None,
+        num_cols: int = None,
+    ):
+        if filename is not None and (
+            (sheet_name is not None)
+            or (table_name is not None)
+            or (num_header_rows is not None)
+            or (num_header_cols is not None)
+            or (num_rows is not None)
+            or (num_cols is not None)
+        ):
+            warn("can't set table/sheet attributes on load of existing document", RuntimeWarning)
+
         self._model = _NumbersModel(filename)
         refs = self._model.sheet_ids()
         self._sheets = ItemsList(self._model, refs, Sheet)
 
+        if filename is None:
+            if sheet_name is not None:
+                self.sheets[0].name = sheet_name
+            table = self.sheets[0].tables[0]
+            if table_name is not None:
+                table.name = table_name
+
+            if num_header_rows is None:
+                num_header_rows = DEFAULT_NUM_HEADERS
+            if num_header_cols is None:
+                num_header_cols = DEFAULT_NUM_HEADERS
+            if num_rows is None:
+                num_rows = DEFAULT_ROW_COUNT
+            if num_cols is None:
+                num_cols = DEFAULT_COLUMN_COUNT
+
+            # Table starts as 1x1 with no headers
+            table.add_row(num_rows - 1)
+            table.num_header_rows = num_header_rows
+            table.add_column(num_cols - 1)
+            table.num_header_cols = num_header_cols
+
     @property
     def sheets(self) -> list:
         """Return a list of all sheets in the document"""
         return self._sheets
 
     @property
     def styles(self) -> list:
@@ -156,20 +195,25 @@
         self._table_id = table_id
         self.num_rows = self._model.number_of_rows(self._table_id)
         self.num_cols = self._model.number_of_columns(self._table_id)
         # Cache all data now to facilite write(). Performance impact
         # of computing all cells is minimal compared to file IO
         self._data = []
         self._model.set_table_data(table_id, self._data)
+        merge_cells = self._model.merge_cells(table_id)
+
         for row_num in range(self.num_rows):
             self._data.append([])
             for col_num in range(self.num_cols):
                 cell_storage = model.table_cell_decode(table_id, row_num, col_num)
                 if cell_storage is None:
-                    cell = Cell.empty_cell(table_id, row_num, col_num, model)
+                    if merge_cells.is_merge_reference((row_num, col_num)):
+                        cell = Cell.merged_cell(table_id, row_num, col_num, model)
+                    else:
+                        cell = Cell.empty_cell(table_id, row_num, col_num, model)
                 else:
                     cell = Cell.from_storage(cell_storage)
                 self._data[row_num].append(cell)
 
     @property
     def name(self) -> str:
         """Return the table's name"""
@@ -186,15 +230,15 @@
         return self._model.num_header_rows(self._table_id)
 
     @num_header_rows.setter
     def num_header_rows(self, num_headers: int):
         """Return the number of header rows"""
         if num_headers < 0:
             raise ValueError("Number of headers cannot be negative")
-        elif num_headers > self.num_cols:
+        elif num_headers > self.num_rows:
             raise ValueError("Number of headers cannot exceed the number of rows")
         elif num_headers > MAX_HEADER_COUNT:
             raise ValueError(f"Number of headers cannot exceed {MAX_HEADER_COUNT} rows")
         return self._model.num_header_rows(self._table_id, num_headers)
 
     @property
     def num_header_cols(self) -> int:
@@ -251,20 +295,19 @@
             return rows
         else:
             return self._data
 
     @property
     @lru_cache(maxsize=None)
     def merge_ranges(self) -> list:
-        merge_cells = self._model.merge_cell_ranges(self._table_id)
-        ranges = [xl_range(*r["rect"]) for r in merge_cells.values()]
-        return sorted(set(list(ranges)))
+        merge_cells = self._model.merge_cells(self._table_id).merge_cell_names()
+        return sorted(set(list(merge_cells)))
 
     def cell(self, *args) -> Union[Cell, MergedCell]:
-        if type(args[0]) == str:
+        if isinstance(args[0], str):
             (row_num, col_num) = xl_cell_to_rowcol(args[0])
         elif len(args) != 2:
             raise IndexError("invalid cell reference " + str(args))
         else:
             (row_num, col_num) = args
 
         if row_num >= self.num_rows or row_num < 0:
@@ -365,15 +408,15 @@
                 yield tuple(row[col_num].value for row in rows[min_row : max_row + 1])
             else:
                 yield tuple(row[col_num] for row in rows[min_row : max_row + 1])
 
     def _validate_cell_coords(self, *args):
         """Check first arguments are value cell references and pad
         the table with empty cells if outside current bounds"""
-        if type(args[0]) == str:
+        if isinstance(args[0], str):
             (row_num, col_num) = xl_cell_to_rowcol(args[0])
             values = args[1:]
         elif len(args) < 2:
             raise IndexError("invalid cell reference " + str(args))
         else:
             (row_num, col_num) = args[0:2]
             values = args[2:]
@@ -388,33 +431,24 @@
 
         for row in range(self.num_cols, col_num + 1):
             self.add_column()
 
         return (row_num, col_num) + tuple(values)
 
     def write(self, *args, style=None):
+        # TODO: write needs to retain/init the border
         (row_num, col_num, value) = self._validate_cell_coords(*args)
-
-        if type(value) == str:
-            self._data[row_num][col_num] = TextCell(row_num, col_num, value)
-        elif type(value) == int or type(value) == float:
-            self._data[row_num][col_num] = NumberCell(row_num, col_num, value)
-        elif type(value) == bool:
-            self._data[row_num][col_num] = BoolCell(row_num, col_num, value)
-        elif type(value) == builtin_datetime or type(value) == DateTime:
-            self._data[row_num][col_num] = DateCell(row_num, col_num, pendulum_instance(value))
-        elif type(value) == builtin_timedelta or type(value) == Duration:
-            self._data[row_num][col_num] = DurationCell(row_num, col_num, value)
-        else:
-            raise ValueError("Can't determine cell type from type " + type(value).__name__)
+        self._data[row_num][col_num] = Cell.from_value(row_num, col_num, value)
         self._data[row_num][col_num]._storage = CellStorage(
             self._model, self._table_id, None, row_num, col_num
         )
+        merge_cells = self._model.merge_cells(self._table_id)
         self._data[row_num][col_num]._table_id = self._table_id
         self._data[row_num][col_num]._model = self._model
+        self._data[row_num][col_num]._set_merge(merge_cells.get((row_num, col_num)))
 
         if style is not None:
             self.set_cell_style(row_num, col_num, style)
 
     def set_cell_style(self, *args):
         (row_num, col_num, style) = self._validate_cell_coords(*args)
         if isinstance(style, Style):
@@ -423,52 +457,58 @@
             if style not in self._model.styles:
                 raise IndexError(f"style '{style}' does not exist")
             self._data[row_num][col_num]._style = self._model.styles[style]
         else:
             raise TypeError("style must be a Style object or style name")
 
     def add_row(self, num_rows=1):
-        row = [EmptyCell(self.num_rows - 1, col_num) for col_num in range(self.num_cols)]
+        row = [
+            Cell.empty_cell(self._table_id, self.num_rows - 1, col_num, self._model)
+            for col_num in range(self.num_cols)
+        ]
         for _ in range(num_rows):
             self._data.append(row.copy())
             self.num_rows += 1
             self._model.number_of_rows(self._table_id, self.num_rows)
 
     def add_column(self, num_cols=1):
         for _ in range(num_cols):
             for row_num in range(self.num_rows):
-                self._data[row_num].append(EmptyCell(row_num, self.num_cols - 1))
+                self._data[row_num].append(
+                    Cell.empty_cell(self._table_id, row_num, self.num_cols - 1, self._model)
+                )
             self.num_cols += 1
             self._model.number_of_columns(self._table_id, self.num_cols)
 
     def merge_cells(self, cell_range):
+        """Convert a cell range or list of cell ranges into merged cells"""
         if isinstance(cell_range, list):
             for x in cell_range:
                 self.merge_cells(x)
         else:
             (start_cell_ref, end_cell_ref) = cell_range.split(":")
             (row_start, col_start) = xl_cell_to_rowcol(start_cell_ref)
             (row_end, col_end) = xl_cell_to_rowcol(end_cell_ref)
             num_rows = row_end - row_start + 1
             num_cols = col_end - col_start + 1
 
-            merge_ranges = self._model._merge_cells[self._table_id]
-            merge_ranges[(row_start, col_start)] = {
-                "merge_type": "source",
-                "size": (num_rows, num_cols),
-            }
+            merge_cells = self._model.merge_cells(self._table_id)
+            merge_cells.add_anchor(row_start, col_start, (num_rows, num_cols))
             for row_num in range(row_start + 1, row_end + 1):
                 for col_num in range(col_start + 1, col_end + 1):
-                    merge_ranges[(row_num, col_num)] = {
-                        "merge_type": "ref",
-                        "rect": (row_start, col_start, row_end, col_end),
-                        "size": (num_rows, num_cols),
-                    }
+                    self._data[row_num][col_num] = MergedCell(row_num, col_num)
+                    merge_cells.add_reference(
+                        row_num, col_num, (row_start, col_start, row_end, col_end)
+                    )
+
+            for row_num, row in enumerate(self._data):
+                for col_num, cell in enumerate(row):
+                    cell._set_merge(merge_cells.get((row_num, col_num)))
 
-    def add_border(self, *args):
+    def set_cell_border(self, *args):
         (row_num, col_num, *args) = self._validate_cell_coords(*args)
         if len(args) == 2:
             (side, border_value) = args
             length = 1
         elif len(args) == 3:
             (side, border_value, length) = args
         else:
@@ -476,14 +516,25 @@
 
         if not isinstance(border_value, Border):
             raise TypeError("border value must be a Border object")
 
         if not isinstance(length, int):
             raise TypeError("border length must be an int")
 
+        if isinstance(side, list):
+            for s in side:
+                self.set_cell_border(row_num, col_num, s, border_value, length)
+            return
+
+        if self._data[row_num][col_num].is_merged and side in ["bottom", "right"]:
+            warn(f"cell [{row_num},{col_num}] is merged; {side} border not set", RuntimeWarning)
+            return
+
+        self._model.extract_strokes(self._table_id)
+
         if side == "top" or side == "bottom":
             for border_col_num in range(col_num, col_num + length):
                 self._model.set_cell_border(
                     self._table_id, row_num, border_col_num, side, border_value
                 )
         elif side == "left" or side == "right":
             for border_row_num in range(row_num, row_num + length):
```

### Comparing `numbers_parser-4.2.0/src/numbers_parser/exceptions.py` & `numbers_parser-4.3.0/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/file.py` & `numbers_parser-4.3.0/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/formula.py` & `numbers_parser-4.3.0/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.3.0/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/iwafile.py` & `numbers_parser-4.3.0/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/mapping.py` & `numbers_parser-4.3.0/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/src/numbers_parser/model.py` & `numbers_parser-4.3.0/src/numbers_parser/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 import re
 
 from array import array
+from collections import defaultdict
 from functools import lru_cache
 from struct import pack
 from typing import Dict, List, Tuple, Union
 from warnings import warn
 
 from numbers_parser.containers import ObjectStore
 from numbers_parser.iwafile import find_extension
@@ -21,28 +22,31 @@
     DOCUMENT_ID,
     PACKAGE_ID,
     MAX_TILE_SIZE,
 )
 from numbers_parser.cell import (
     xl_rowcol_to_cell,
     xl_col_to_name,
+    xl_range,
     BoolCell,
     DateCell,
     DurationCell,
     EmptyCell,
     MergedCell,
     NumberCell,
     TextCell,
     Style,
     Alignment,
     HorizontalJustification,
     VerticalJustification,
     RGB,
     Border,
     BorderType,
+    MergeReference,
+    MergeAnchor,
 )
 from numbers_parser.exceptions import UnsupportedError, UnsupportedWarning
 from numbers_parser.formula import TableFormulas
 from numbers_parser.bullets import (
     BULLET_PREFIXES,
     BULLET_CONVERTION,
     BULLET_SUFFIXES,
@@ -74,14 +78,53 @@
             new_font_map[v] = k
     return new_font_map
 
 
 FONT_FAMILY_TO_NAME = create_font_name_map(FONT_NAME_TO_FAMILY)
 
 
+class MergeCells:
+    def __init__(self):
+        self._references = defaultdict(lambda: False)
+
+    def add_reference(self, row_num: int, col_num: int, rect: Tuple):
+        self._references[(row_num, col_num)] = MergeReference(*rect)
+
+    def add_anchor(self, row_num: int, col_num: int, size: Tuple):
+        self._references[(row_num, col_num)] = MergeAnchor(size)
+
+    def is_merge_reference(self, row_col: Tuple) -> bool:
+        return isinstance(self._references[row_col], MergeReference)
+
+    def is_merge_anchor(self, row_col: Tuple) -> bool:
+        return isinstance(self._references[row_col], MergeAnchor)
+
+    def get(self, row_col: Tuple) -> Union[MergeAnchor, MergeReference]:
+        return self._references[row_col]
+
+    def size(self, row_col: Tuple) -> Tuple:
+        return self._references[row_col].size
+
+    def rect(self, row_col: Tuple) -> Tuple:
+        return self._references[row_col].rect
+
+    def merge_cell_names(self):
+        ranges = [
+            xl_range(*v.rect) for k, v in self._references.items() if self.is_merge_reference(k)
+        ]
+        return ranges
+
+    def merge_cells(self):
+        ranges = [k for k, v in self._references.items() if self.is_merge_anchor(k)]
+        return ranges
+
+    def __len__(self):
+        return len(self._references.keys())
+
+
 class DataLists:
     """Model for TST.DataList with caching and key generation for new values"""
 
     def __init__(self, model: object, datalist_name: str, value_attr: str = None):
         self._model = model
         self._datalists = {}
         self._value_attr = value_attr
@@ -161,23 +204,28 @@
     Not to be used in application code.
     """
 
     def __init__(self, filename):
         if filename is None:
             filename = DEFAULT_DOCUMENT
         self.objects = ObjectStore(filename)
-        self._merge_cells = {}
+        self._merge_cells = defaultdict(MergeCells)
         self._row_heights = {}
         self._col_widths = {}
         self._table_formats = DataLists(self, "format_table")
         self._table_styles = DataLists(self, "styleTable", "reference")
         self._table_strings = DataLists(self, "stringTable", "string")
         self._table_data = {}
         self._styles = None
-        self._max_stroke_order = 0
+        self._strokes = {
+            "top": defaultdict(),
+            "right": defaultdict(),
+            "bottom": defaultdict(),
+            "left": defaultdict(),
+        }
 
     @property
     def file_store(self):
         return self.objects.file_store
 
     def find_refs(self, ref: str) -> list:
         return self.objects.find_refs(ref)
@@ -398,73 +446,65 @@
         """Return the CalculationEngine object for the current document"""
         ce_id = self.calc_engine_id()
         if ce_id == 0:
             return None
         else:
             return self.objects[ce_id]
 
+    @lru_cache(maxsize=None)
     def calculate_merge_cell_ranges(self, table_id):
         """Exract all the merge cell ranges for the Table."""
         # https://github.com/masaccio/numbers-parser/blob/main/doc/Numbers.md#merge-ranges
         owner_id_map = self.owner_id_map()
         table_base_id = self.table_base_id(table_id)
 
-        merge_cells = {}
         range_table_ids = self.find_refs("RangePrecedentsTileArchive")
         for range_id in range_table_ids:
             o = self.objects[range_id]
             to_owner_id = o.to_owner_id
             if owner_id_map[to_owner_id] == table_base_id:
                 for from_to_range in o.from_to_range:
                     rect = from_to_range.refers_to_rect
                     row_start = rect.origin.row
                     row_end = row_start + rect.size.num_rows - 1
                     col_start = rect.origin.column
                     col_end = col_start + rect.size.num_columns - 1
+                    size = (row_end - row_start + 1, col_end - col_start + 1)
                     for row_num in range(row_start, row_end + 1):
                         for col_num in range(col_start, col_end + 1):
-                            merge_cells[(row_num, col_num)] = {
-                                "merge_type": "ref",
-                                "rect": (row_start, col_start, row_end, col_end),
-                                "size": (rect.size.num_rows, rect.size.num_columns),
-                            }
-                    merge_cells[(row_start, col_start)]["merge_type"] = "source"
-        self._merge_cells[table_id] = merge_cells
+                            self._merge_cells[table_id].add_reference(
+                                row_num, col_num, (row_start, col_start, row_end, col_end)
+                            )
+                    self._merge_cells[table_id].add_anchor(row_start, col_start, size)
 
-        bds = self.objects[table_id].base_data_store
-        if bds.merge_region_map.identifier != 0:
-            cell_range = self.objects[bds.merge_region_map.identifier]
-        else:
-            return merge_cells
+        base_data_store = self.objects[table_id].base_data_store
+        if base_data_store.merge_region_map.identifier == 0:
+            return
 
+        cell_range = self.objects[base_data_store.merge_region_map.identifier]
         for cell_range in cell_range.cell_range:
             (col_start, row_start) = (
                 cell_range.origin.packedData >> 16,
                 cell_range.origin.packedData & 0xFFFF,
             )
             (num_columns, num_rows) = (
                 cell_range.size.packedData >> 16,
                 cell_range.size.packedData & 0xFFFF,
             )
             row_end = row_start + num_rows - 1
             col_end = col_start + num_columns - 1
             for row_num in range(row_start, row_end + 1):
                 for col_num in range(col_start, col_end + 1):
-                    merge_cells[(row_num, col_num)] = {
-                        "merge_type": "ref",
-                        "rect": (row_start, col_start, row_end, col_end),
-                        "size": (num_rows, num_columns),
-                    }
-        merge_cells[(row_start, col_start)]["merge_type"] = "source"
-
-        return merge_cells
+                    self._merge_cells[table_id].add_reference(
+                        row_num, col_num, (row_start, col_start, row_end, col_end)
+                    )
+            self._merge_cells[table_id].add_anchor(row_start, col_start, (num_rows, num_columns))
 
-    def merge_cell_ranges(self, table_id):
-        if table_id not in self._merge_cells:
-            self._merge_cells[table_id] = self.calculate_merge_cell_ranges(table_id)
+    def merge_cells(self, table_id):
+        self.calculate_merge_cell_ranges(table_id)
         return self._merge_cells[table_id]
 
     def table_id_to_sheet_id(self, table_id: int) -> int:
         for sheet_id in self.sheet_ids():  # pragma: no branch
             if table_id in self.table_ids(sheet_id):
                 return sheet_id
 
@@ -566,14 +606,16 @@
 
     @lru_cache(maxsize=None)
     def storage_buffer(self, table_id: int, row_num: int, col_num: int) -> bytes:
         row_offset = self.row_storage_map(table_id)[row_num]
         if row_offset is None:
             return None
         storage_buffers = self.storage_buffers(table_id)
+        if len(storage_buffers) == 0:
+            return None
         if col_num >= len(storage_buffers[row_offset]):
             return None
         return storage_buffers[row_offset][col_num]
 
     def recalculate_row_headers(self, table_id: int, data: List):
         base_data_store = self.objects[table_id].base_data_store
         buckets = self.objects[base_data_store.rowHeaders.buckets[0].identifier]
@@ -610,30 +652,29 @@
                 width = current_column_widths[col_num]
             header = TSTArchives.HeaderStorageBucket.Header(
                 index=col_num, numberOfCells=num_rows, size=width, hidingState=0
             )
             buckets.headers.append(header)
 
     def recalculate_merged_cells(self, table_id: int):
-        merge_cells = self.merge_cell_ranges(table_id)
+        merge_cells = self.merge_cells(table_id)
         if len(merge_cells) == 0:
             return
 
         merge_map_id, merge_map = self.objects.create_object_from_dict(
             "CalculationEngine", {}, TSTArchives.MergeRegionMapArchive
         )
 
-        for merge_cell, merge_data in merge_cells.items():
-            if merge_data["merge_type"] == "source":
-                cell_id = TSTArchives.CellID(packedData=(merge_cell[1] << 16 | merge_cell[0]))
-                table_size = TSTArchives.TableSize(
-                    packedData=(merge_data["size"][1] << 16 | merge_data["size"][0])
-                )
-                cell_range = TSTArchives.CellRange(origin=cell_id, size=table_size)
-                merge_map.cell_range.append(cell_range)
+        merge_cells = self.merge_cells(table_id)
+        for row_col in merge_cells.merge_cells():
+            size = merge_cells.size(row_col)
+            cell_id = TSTArchives.CellID(packedData=(row_col[1] << 16 | row_col[0]))
+            table_size = TSTArchives.TableSize(packedData=(size[1] << 16 | size[0]))
+            cell_range = TSTArchives.CellRange(origin=cell_id, size=table_size)
+            merge_map.cell_range.append(cell_range)
 
         base_data_store = self.objects[table_id].base_data_store
         base_data_store.merge_region_map.CopyFrom(TSPMessages.Reference(identifier=merge_map_id))
 
     def recalculate_row_info(
         self, table_id: int, data: List, tile_row_offset: int, row_num: int
     ) -> TSTArchives.TileRowInfo:
@@ -1481,20 +1522,34 @@
             flags |= 0x200
             length += 4
             storage += pack("<i", cell._storage.formula_id)
         if cell._storage.num_format_id is not None:
             flags |= 0x2000
             length += 4
             storage += pack("<i", cell._storage.num_format_id)
-            storage[4:6] = pack("<h", 2)
-            storage[6:8] = pack("<h", 1)
+        if cell._storage.currency_format_id is not None:
+            flags |= 0x4000
+            length += 4
+            storage += pack("<i", cell._storage.currency_format_id)
+        if cell._storage.date_format_id is not None:
+            flags |= 0x8000
+            length += 4
+            storage += pack("<i", cell._storage.date_format_id)
+        if cell._storage.duration_format_id is not None:
+            flags |= 0x10000
+            length += 4
+            storage += pack("<i", cell._storage.duration_format_id)
         if cell._storage.text_format_id is not None:
             flags |= 0x20000
             length += 4
             storage += pack("<i", cell._storage.text_format_id)
+        if cell._storage.bool_format_id is not None:
+            flags |= 0x40000
+            length += 4
+            storage += pack("<i", cell._storage.bool_format_id)
 
         storage[8:12] = pack("<i", flags)
         if len(storage) < 32:
             storage += bytearray(32 - length)
 
         return storage[0:length]
 
@@ -1753,35 +1808,27 @@
         data = self._table_data[table_id]
         if row_num < 0 or col_num < 0:
             return None
         if row_num >= len(data) or col_num >= len(data[row_num]):
             return None
         cell = self._table_data[table_id][row_num][col_num]
         if isinstance(cell, MergedCell):
-            if side == "top":
-                if row_num == cell.row_start:
-                    return cell
-                else:
-                    return None
-            elif side == "right":
-                if col_num == cell.col_end:
-                    return cell
-                else:
-                    return None
-            elif side == "bottom":
-                if row_num == cell.row_end:
-                    return cell
-                else:
-                    return None
-            else:  # left
-                if col_num == cell.col_start:
-                    return cell
-                else:
-                    return None
-        return cell
+            if (
+                (side == "top" and row_num == cell.row_start)
+                or (side == "right" and col_num == cell.col_end)
+                or (side == "bottom" and row_num == cell.row_end)
+                or (side == "left" and col_num == cell.col_start)
+            ):
+                return cell
+        elif cell.is_merged:
+            if side == "top" or side == "left":
+                return cell
+        else:
+            return cell
+        return None
 
     def set_cell_border(
         self, table_id: int, row_num: int, col_num: int, side: str, border_value: Border
     ):
         """Set the 2 borders adjacent to a stroke if within the table range"""
         if side == "top":
             if (cell := self.cell_for_stroke(table_id, "top", row_num, col_num)) is not None:
@@ -1804,16 +1851,14 @@
             if (cell := self.cell_for_stroke(table_id, "right", row_num, col_num - 1)) is not None:
                 cell._border.right = border_value
 
     def extract_strokes_in_layers(self, table_id: int, layer_ids: List, side: str):
         for layer_id in layer_ids:
             stroke_layer = self.objects[layer_id.identifier]
             for stroke_run in stroke_layer.stroke_runs:
-                if stroke_run.order > self._max_stroke_order:
-                    self._max_stroke_order = stroke_run.order
                 border_value = Border(
                     width=round(stroke_run.stroke.width, 2),
                     color=rgb(stroke_run.stroke.color),
                     style=self.stroke_type(stroke_run),
                     _order=stroke_run.order,
                 )
                 if side in ["top", "bottom"]:
@@ -1833,15 +1878,14 @@
         sidecar_obj = self.objects[table_obj.stroke_sidecar.identifier]
         self.extract_strokes_in_layers(table_id, sidecar_obj.top_row_stroke_layers, "top")
         self.extract_strokes_in_layers(table_id, sidecar_obj.left_column_stroke_layers, "left")
         self.extract_strokes_in_layers(table_id, sidecar_obj.right_column_stroke_layers, "right")
         self.extract_strokes_in_layers(table_id, sidecar_obj.bottom_row_stroke_layers, "bottom")
 
     def create_stroke(self, origin: int, length: int, border_value: Border):
-        self._max_stroke_order += 1
         line_cap = TSDArchives.StrokeArchive.LineCap.ButtCap
         line_join = TSDArchives.LineJoin.MiterJoin
         if border_value.style == BorderType.SOLID:
             pattern = TSDArchives.StrokePatternArchive(
                 type=StrokePattern.StrokePatternType.TSDSolidPattern,
                 phase=0.0,
                 count=0,
@@ -1890,15 +1934,15 @@
                 b=border_value.color.b / 255,
                 a=1.0,
             )
             width = border_value.width
         return TSTArchives.StrokeLayerArchive.StrokeRunArchive(
             origin=origin,
             length=length,
-            order=self._max_stroke_order,
+            order=border_value._order,
             stroke=TSDArchives.StrokeArchive(
                 color=color,
                 width=width,
                 cap=line_cap,
                 join=line_join,
                 miter_limit=4.0,
                 pattern=pattern,
@@ -1912,14 +1956,18 @@
         col_num: int,
         side: str,
         border_value: Border,
         length: int,
     ):
         table_obj = self.objects[table_id]
         sidecar_obj = self.objects[table_obj.stroke_sidecar.identifier]
+        sidecar_obj.max_order += 1
+        sidecar_obj.row_count = table_obj.number_of_rows
+        sidecar_obj.column_count = table_obj.number_of_columns
+        border_value._order = sidecar_obj.max_order
 
         if side == "top":
             layer_ids = sidecar_obj.top_row_stroke_layers
             row_column_index = row_num
             origin = col_num
         elif side == "right":
             layer_ids = sidecar_obj.right_column_stroke_layers
@@ -1935,15 +1983,42 @@
             origin = row_num
 
         stroke_layer = None
         for layer_id in layer_ids:
             if self.objects[layer_id.identifier].row_column_index == row_column_index:
                 stroke_layer = self.objects[layer_id.identifier]
         if stroke_layer is not None:
-            stroke_layer.append(self.create_stroke(origin, length, border_value))
+            stroke_patched = False
+            for stroke_run in stroke_layer.stroke_runs:
+                stroke_start = stroke_run.origin
+                stroke_end = stroke_run.origin + stroke_run.length
+                stroke_range = range(stroke_start, stroke_end)
+                if origin <= stroke_start and (origin + length) >= stroke_end:
+                    # New stroke overwrites all of existing stroke
+                    stroke_run.CopyFrom(self.create_stroke(origin, length, border_value))
+                    stroke_patched = True
+                elif origin == stroke_start and length < stroke_run.length:
+                    # New stroke writes to start of existing stroke
+                    stroke_run.origin = origin + length
+                    stroke_run.length = stroke_run.length - length
+                elif origin in stroke_range and (origin + length) == stroke_end:
+                    # New stoke writes to end of existing stroke
+                    stroke_run.length = stroke_run.length - length
+                elif origin in stroke_range and (origin + length) in stroke_range:
+                    # New stroke in middle of existing stroke
+                    stroke_run.length = origin - stroke_start
+                    stroke_layer.stroke_runs.append(
+                        TSTArchives.StrokeLayerArchive.StrokeRunArchive()
+                    )
+                    stroke_layer.stroke_runs[-1].CopyFrom(stroke_run)
+                    stroke_layer.stroke_runs[-1].origin = origin + length
+                    stroke_layer.stroke_runs[-1].length = stroke_end - origin - length
+            if not stroke_patched:
+                stroke_layer.stroke_runs.append(self.create_stroke(origin, length, border_value))
+            stroke_layer.stroke_runs.sort(key=lambda x: x.origin)
         else:
             stroke_layer_id, stroke_layer = self.objects.create_object_from_dict(
                 "CalculationEngine",
                 {
                     "row_column_index": row_column_index,
                 },
                 TSTArchives.StrokeLayerArchive,
```

### Comparing `numbers_parser-4.2.0/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.3.0/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.2.0/PKG-INFO` & `numbers_parser-4.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.2.0
+Version: 4.3.0
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Requires-Dist: compact-json (>=1.1.3,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: protobuf (>=4.21.1,<5.0.0)
 Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
 Requires-Dist: regex (>=2022.9.13,<2023.0.0)
 Requires-Dist: roman (>=3.3,<4.0)
+Requires-Dist: sigfig (>=1.3.2,<2.0.0)
 Project-URL: Documentation, https://github.com/masaccio/numbers-parser/blob/main/README.md
 Project-URL: Repository, https://github.com/masaccio/numbers-parser
 Description-Content-Type: text/markdown
 
 # numbers-parser
 
 [![build:](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml/badge.svg)](https://github.com/masaccio/numbers-parser/actions/workflows/run-all-tests.yml)
@@ -40,15 +41,15 @@
 
 Formula evaluation relies on Numbers storing current values which should usually be the case. Formulas themselves rather than the computed values can optionally be extracted. [Style support](#styles) is somewhat limited, but has grown significantly as of version 4.0.
 
 ## API changes in version 4.0
 
 To better partition cell styles, background image data which was supported in earlier versions through the methods `image_data` and `image_filename` is now part of the new `cell_style` property. Using the deprecated methods `image_data` and `image_filename` will issue a `DeprecationWarning` if used.The legacy methods will be removed in a future version of numbers-parser.
 
-`NumberCell` cell types return [`decimal.Decimal`](https://docs.python.org/3/library/decimal.html) types rather than `float`. These are created in a [decimal128](https://en.wikipedia.org/wiki/Decimal128_floating-point_format) context to preserve the precision used by Numbers. Previously, using float resulted in rounding errors in unpacking internal numbers.
+`NumberCell` cell values are now limited to 15 significant figues to match the implementation of floating point numbers in Apple Numbers. For example, the value `1234567890123456` is rounded to `1234567890123460` in the same was as in Numbers. Previously, using native `float` with no checking resulted in rounding errors in unpacking internal numbers. Attempting to write a number with too many significant digits results in a `RuntimeWarning`.
 
 ## Installation
 
 ``` bash
 python3 -m pip install numbers-parser
 ```
 
@@ -130,18 +131,15 @@
 print("Cell A1 contains", table.cell(0, 0))
 # Excel/Numbers-style cell references
 print("Cell C2 contains", table.cell("C2"))
 ```
 
 ### Merged cells
 
-When extracting data using ```rows()``` merged cells are ignored since only text values
-are returned. The ```cell()``` method of ```Table``` objects returns a ```Cell``` type
-object which is typed by the type of cell in the Numbers table. ```MergeCell``` objects
-indicates cells removed in a merge.
+When extracting data using `rows()` merged cells are ignored since only text values are returned. The `cell()` method of `Table` objects returns a `Cell` type object which is typed by the type of cell in the Numbers table. `MergeCell` objects indicates cells removed in a merge. The remaining `Cell` has a `bool` property `is_merged` which is `True` if the cell is the result of a merge. Such cells return a `tuple` for their `size` property indicating the number of rows and columns in the merged cell. Unmerged cells return a `size` of `None`.
 
 ``` python
 doc = Document("my-spreadsheet.numbers")
 sheets = doc.sheets
 tables = sheets["Sheet 1"].tables
 table = tables["Table 1"]
 
@@ -246,14 +244,41 @@
 
 ``` python
 cell = table.cell("B1")
 with open (cell.style.bg_image.filename, "wb") as f:
     f.write(cell.style.bg_image.data)
 ```
 
+### Borders
+
+`numbers-parser` supports reading and writing cell borders, though the interface for each differs. Individual cells can have each of their four borders tested, but when drawing new borders, these are set for the table to allow for drawing borders across multiple cells. Setting the border of merged cells is not possible unless the edge of the cells is at the end of the merged region.
+
+Borders are represeted using the `Border` class that can be initialised with line width, color and line style:
+
+``` python
+border = Border(4.0, RGB(0, 162, 255), "solid"))
+```
+
+Valid values for the line `style` parameter are `"solid"`, `"dashes"`, `"dots"` and `"none"`.
+
+#### Reading Cell Borders
+
+Cells have a property `border` which itself has the properties `top`, `right`, `bottom` and `left`, each of which is a `Border` class representing the line type for that cell. Cells with no border set at all, and merged cells which are inside the range of the merge return `None` for these cells. The absence of a specified border is different from no border in Numbers which is a valid `Border` class with `style="none"`.
+
+#### Writing Cell Borders
+
+The `Table` method `set_cell_border()` sets the border for a cell edge or a range of cells:
+
+``` python
+table.set_cell_border("C1", ["top", "left"], Border(0.0, RGB(0, 0, 0), "none"))
+table.set_cell_border(0, 4, "right", Border(1.0, RGB(0, 0, 0), "solid"), 3)
+```
+
+The last positional parameter specifies the length of the border and defaults to 1. A single call to `set_cell_border()` can set the borders to one or more sides of the cell as above. Like `Table.write()`, `set_cell_border()` supports both row/column and Excel-style cell references.
+
 ## Writing Numbers files
 
 Whilst support for writing numbers files has been stable since version 3.4.0, you are highly recommened not to overwrite working Numbers files and instead save data to a new file.
 
 ### Limitations
 
 Current limitations to write support are:
```

