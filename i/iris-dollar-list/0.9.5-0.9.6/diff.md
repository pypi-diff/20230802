# Comparing `tmp/iris-dollar-list-0.9.5.tar.gz` & `tmp/iris-dollar-list-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris-dollar-list-0.9.5.tar", last modified: Mon Nov 14 16:24:15 2022, max compression
+gzip compressed data, was "iris-dollar-list-0.9.6.tar", last modified: Wed Aug  2 12:10:49 2023, max compression
```

## Comparing `iris-dollar-list-0.9.5.tar` & `iris-dollar-list-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 1252422112 1252422112        0 2022-11-14 16:24:15.192723 iris-dollar-list-0.9.5/
--rw-r--r--   0 1252422112 1252422112     1075 2022-10-23 14:57:21.000000 iris-dollar-list-0.9.5/LICENSE
--rw-r--r--   0 1252422112 1252422112     7031 2022-11-14 16:24:15.190238 iris-dollar-list-0.9.5/PKG-INFO
--rw-r--r--   0 1252422112 1252422112     6236 2022-11-03 14:01:19.000000 iris-dollar-list-0.9.5/README.md
--rw-r--r--   0 1252422112 1252422112       38 2022-11-14 16:24:15.195400 iris-dollar-list-0.9.5/setup.cfg
--rw-r--r--   0 1252422112 1252422112     1639 2022-11-14 16:23:23.000000 iris-dollar-list-0.9.5/setup.py
-drwxr-xr-x   0 1252422112 1252422112        0 2022-11-14 16:24:15.102740 iris-dollar-list-0.9.5/src/
-drwxr-xr-x   0 1252422112 1252422112        0 2022-11-14 16:24:15.138551 iris-dollar-list-0.9.5/src/iris_dollar_list/
--rw-r--r--   0 1252422112 1252422112      124 2022-10-23 16:36:47.000000 iris-dollar-list-0.9.5/src/iris_dollar_list/__init__.py
--rw-r--r--   0 1252422112 1252422112    20713 2022-11-14 16:02:31.000000 iris-dollar-list-0.9.5/src/iris_dollar_list/dollar_list.py
-drwxr-xr-x   0 1252422112 1252422112        0 2022-11-14 16:24:15.181706 iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/
--rw-r--r--   0 1252422112 1252422112     7031 2022-11-14 16:24:14.000000 iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/PKG-INFO
--rw-r--r--   0 1252422112 1252422112      318 2022-11-14 16:24:14.000000 iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/SOURCES.txt
--rw-r--r--   0 1252422112 1252422112        1 2022-11-14 16:24:14.000000 iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/dependency_links.txt
--rw-r--r--   0 1252422112 1252422112       59 2022-11-14 16:24:14.000000 iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/entry_points.txt
--rw-r--r--   0 1252422112 1252422112       17 2022-11-14 16:24:14.000000 iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-08-02 12:10:49.664168 iris-dollar-list-0.9.6/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1075 2022-10-23 14:57:21.000000 iris-dollar-list-0.9.6/LICENSE
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     7031 2023-08-02 12:10:49.662967 iris-dollar-list-0.9.6/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     6236 2022-11-03 14:01:19.000000 iris-dollar-list-0.9.6/README.md
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-08-02 12:10:49.664515 iris-dollar-list-0.9.6/setup.cfg
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1499 2023-08-02 10:33:41.000000 iris-dollar-list-0.9.6/setup.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-08-02 12:10:49.644768 iris-dollar-list-0.9.6/src/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-08-02 12:10:49.653285 iris-dollar-list-0.9.6/src/iris_dollar_list/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      124 2022-10-23 16:36:47.000000 iris-dollar-list-0.9.6/src/iris_dollar_list/__init__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20973 2023-08-02 10:32:38.000000 iris-dollar-list-0.9.6/src/iris_dollar_list/dollar_list.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-08-02 12:10:49.660931 iris-dollar-list-0.9.6/src/iris_dollar_list.egg-info/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     7031 2023-08-02 12:10:49.000000 iris-dollar-list-0.9.6/src/iris_dollar_list.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      271 2023-08-02 12:10:49.000000 iris-dollar-list-0.9.6/src/iris_dollar_list.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-08-02 12:10:49.000000 iris-dollar-list-0.9.6/src/iris_dollar_list.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       17 2023-08-02 12:10:49.000000 iris-dollar-list-0.9.6/src/iris_dollar_list.egg-info/top_level.txt
```

### Comparing `iris-dollar-list-0.9.5/LICENSE` & `iris-dollar-list-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iris-dollar-list-0.9.5/PKG-INFO` & `iris-dollar-list-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-dollar-list
-Version: 0.9.5
+Version: 0.9.6
 Summary: iris-dollar-list
 Home-page: https://github.com/grongierisc/iris-dollar-list
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris-dollar-list
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris-dollar-list-0.9.5/README.md` & `iris-dollar-list-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `iris-dollar-list-0.9.5/setup.py` & `iris-dollar-list-0.9.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     # Do the setup
     setup(
         name='iris-dollar-list',
         description='iris-dollar-list',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='0.9.5',
+        version='0.9.6',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris-dollar-list',
         url='https://github.com/grongierisc/iris-dollar-list',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
@@ -34,17 +34,11 @@
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Topic :: Utilities'
         ],
         package_dir={'': 'src'},
         packages=['iris_dollar_list'],
-        entry_points={
-            'console_scripts': [
-                'iris-dollar-list = dollar_list.main:main'
-            ]
-        }
     )
 
-
 if __name__ == '__main__':
     main()
```

### Comparing `iris-dollar-list-0.9.5/src/iris_dollar_list/dollar_list.py` & `iris-dollar-list-0.9.6/src/iris_dollar_list/dollar_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from dataclasses import dataclass
 from enum import Enum
 import struct
 from typing import Any,List
 import decimal
 
-class Dollartype(Enum):
+class DollarType(Enum):
     ITEM_UNDEF = -1
     ITEM_PLACEHOLDER = 0
     ITEM_ASCII = 1
     ITEM_UNICODE = 2
     ITEM_POSINT = 4
     ITEM_NEGINT = 5
     ITEM_POSNUM = 6
@@ -24,15 +24,15 @@
 
 @dataclass
 class DollarItem:
     """
     A class that represents a dollar item
     """
     # type of the item
-    dollar_type: Dollartype = Dollartype.ITEM_UNDEF
+    dollar_type: DollarType = DollarType.ITEM_UNDEF
     # value of the item
     value: Any = None
     # raw data of the item
     raw_value: bytes = b''
     # raw data of the item + meta data
     buffer: bytes = b''
     # offset of the item in the list buffer
@@ -124,29 +124,29 @@
         if typ is None:
             typ = self.get_item_type(
                     offset=offset,
                     meta_offset=meta_offset
                 )
         if raw_value is None:
             raw_value = self.get_item_raw_value(offset,meta_offset,length)
-        if typ == Dollartype.ITEM_ASCII.value:
+        if typ == DollarType.ITEM_ASCII.value:
             val = self.get_ascii(raw_value)
-        elif typ == Dollartype.ITEM_UNICODE.value:
+        elif typ == DollarType.ITEM_UNICODE.value:
             val = raw_value.decode('utf-16')
-        elif typ == Dollartype.ITEM_POSINT.value:
+        elif typ == DollarType.ITEM_POSINT.value:
             val = self.get_posint(raw_value)
-        elif typ == Dollartype.ITEM_NEGINT.value:
+        elif typ == DollarType.ITEM_NEGINT.value:
             val = self.get_negint(raw_value)
-        elif typ == Dollartype.ITEM_POSNUM.value:
+        elif typ == DollarType.ITEM_POSNUM.value:
             val = self.get_posnum(raw_value)
-        elif typ == Dollartype.ITEM_NEGNUM.value:
+        elif typ == DollarType.ITEM_NEGNUM.value:
             val = self.get_negnum(raw_value)
-        elif typ == Dollartype.ITEM_DOUBLE.value:
+        elif typ == DollarType.ITEM_DOUBLE.value:
             val = struct.unpack('<d',raw_value)[0]
-        elif typ == Dollartype.ITEM_COMPACT_DOUBLE.value:
+        elif typ == DollarType.ITEM_COMPACT_DOUBLE.value:
             val = struct.unpack('<f',raw_value)[0]
         else:
             val = None
         return val
 
     def get_ascii(self,raw_value):
         """
@@ -235,15 +235,15 @@
         """
         rsp = None
         if isinstance(item,DollarItem):
             rsp = item
         elif isinstance(item,DollarList):
             rsp = DollarItem(value=item,dollar_type=0,raw_value=item.to_bytes()
             ,buffer=self.get_meta_value_length(item.to_bytes())+
-                Dollartype.ITEM_ASCII.value.to_bytes(1, "little")+
+                DollarType.ITEM_ASCII.value.to_bytes(1, "little")+
                 item.to_bytes())
         elif isinstance(item,str) or item is None:
             rsp = self.create_from_string(item)
         elif isinstance(item,int):
             rsp = self.create_from_int(item)
         elif isinstance(item,float):
             rsp = self.create_from_float(item)
@@ -273,33 +273,33 @@
     def create_null_item(self):
         """
         Create a DollarItem with a null value
         """
         raw_value = b''
         item_value = None
         lenght = b'\x02'
-        buffer = lenght + Dollartype.ITEM_ASCII.value.to_bytes(1, "little") + raw_value
+        buffer = lenght + DollarType.ITEM_ASCII.value.to_bytes(1, "little") + raw_value
         return DollarItem(
             value=item_value,
             raw_value=raw_value,
             buffer=buffer,
-            dollar_type=Dollartype.ITEM_ASCII.value,
+            dollar_type=DollarType.ITEM_ASCII.value,
         )
 
     def create_from_ascii(self,item,locale):
         """
         Create a DollarItem from a string
         """
         raw_value = item.encode(locale)
         item_value = item
         lenght = self.get_meta_value_length(raw_value)
         if locale != 'utf-16':
-            typ = Dollartype.ITEM_ASCII.value
+            typ = DollarType.ITEM_ASCII.value
         else:
-            typ = Dollartype.ITEM_UNICODE.value
+            typ = DollarType.ITEM_UNICODE.value
         buffer = lenght + typ.to_bytes(1, "little") + raw_value
         return DollarItem(
             value=item_value,
             raw_value=raw_value,
             buffer=buffer,
             dollar_type=typ,
         )
@@ -318,32 +318,32 @@
     def create_negint(self,item):
         """
         Create a DollarItem from a negative integer
         """
         raw_value = item.to_bytes((item.bit_length() + 7) // 8, "little",signed=True)
         item_value = item
         lenght = self.get_meta_value_length(raw_value)
-        buffer = lenght + Dollartype.ITEM_NEGINT.value.to_bytes(1, "little") + raw_value
+        buffer = lenght + DollarType.ITEM_NEGINT.value.to_bytes(1, "little") + raw_value
         return DollarItem(
-            dollar_type=Dollartype.ITEM_NEGINT.value,
+            dollar_type=DollarType.ITEM_NEGINT.value,
             value=item_value,
             raw_value=raw_value,
             buffer=buffer
         )
 
     def create_posint(self,item):
         """
         Create a DollarItem from a positive integer
         """
         raw_value = item.to_bytes((item.bit_length() + 7) // 8, "little")
         item_value = item
         lenght = self.get_meta_value_length(raw_value)
-        buffer = lenght + Dollartype.ITEM_POSINT.value.to_bytes(1, "little") + raw_value
+        buffer = lenght + DollarType.ITEM_POSINT.value.to_bytes(1, "little") + raw_value
         return DollarItem(
-            dollar_type=Dollartype.ITEM_POSINT.value,
+            dollar_type=DollarType.ITEM_POSINT.value,
             value=item_value,
             raw_value=raw_value,
             buffer=buffer
         )
 
     def create_from_float(self,item):
         """
@@ -364,21 +364,22 @@
         # 1.2345 -> 12345 with scale 4
 
         # get the scale
         scale = len(str(item).split('.')[1]) * -1
         # convert to int
         num = int(item * (10 ** (scale * -1)))
         # create the item
-        raw_value = scale.to_bytes(1, "little",signed=True)+num.to_bytes((num.bit_length() + 7) // 8, "little",signed=True)
+        raw_value = (scale.to_bytes(1, "little",signed=True)
+                    +num.to_bytes((num.bit_length() + 7) // 8, "little",signed=True))
 
         item_value = item
         lenght = self.get_meta_value_length(raw_value)
-        buffer = lenght + Dollartype.ITEM_NEGNUM.value.to_bytes(1, "little") + raw_value
+        buffer = lenght + DollarType.ITEM_NEGNUM.value.to_bytes(1, "little") + raw_value
         return DollarItem(
-            dollar_type=Dollartype.ITEM_NEGNUM.value,
+            dollar_type=DollarType.ITEM_NEGNUM.value,
             value=item_value,
             raw_value=raw_value,
             buffer=buffer
         )
 
     def create_posnum(self,item):
         """
@@ -388,21 +389,22 @@
         # 1.2345 -> 12345 with scale 4
 
         # get the scale
         scale = len(str(item).split('.')[1]) * -1
         # convert to int
         num = int(item * (10 ** (scale * -1)))
         # create the item
-        raw_value = scale.to_bytes(1, "little",signed=True)+num.to_bytes((num.bit_length() + 7) // 8, "little")
+        raw_value = (scale.to_bytes(1, "little",signed=True)
+                    +num.to_bytes((num.bit_length() + 7) // 8, "little"))
 
         item_value = item
         lenght = self.get_meta_value_length(raw_value)
-        buffer = lenght + Dollartype.ITEM_POSNUM.value.to_bytes(1, "little") + raw_value
+        buffer = lenght + DollarType.ITEM_POSNUM.value.to_bytes(1, "little") + raw_value
         return DollarItem(
-            dollar_type=Dollartype.ITEM_POSNUM.value,
+            dollar_type=DollarType.ITEM_POSNUM.value,
             value=item_value,
             raw_value=raw_value,
             buffer=buffer
         )
 
     def get_meta_value_length(self,raw_value):
         """
@@ -424,14 +426,18 @@
         return response
 
 class DollarList:
 
     items: List[DollarItem] = []
 
     def __init__(self, value=None):
+        """
+        Create a DollarList
+        """
+        self.items = []
         if value is not None:
             if isinstance(value, bytes):
                 for item in self.from_bytes(value):
                     self.items.append(item)
             elif isinstance(value, list):
                 for item in self.from_list(value):
                     self.items.append(item)
@@ -552,22 +558,22 @@
     def _str_(cls,items):
         """
         Return a string representation of the list.
         Like the dollar list representation with $lb"""
         response = "$lb("
         for item in items:
 
-            if item.dollar_type in (Dollartype.ITEM_ASCII.value,
-                                    Dollartype.ITEM_UNICODE.value):
+            if item.dollar_type in (DollarType.ITEM_ASCII.value,
+                                    DollarType.ITEM_UNICODE.value):
                 if item.value is None:
                     response += '""' # way of iris to represent null string
                 else:
                     response += f'"{item.value}"'
 
-            elif item.dollar_type == Dollartype.ITEM_PLACEHOLDER.value:
+            elif item.dollar_type == DollarType.ITEM_PLACEHOLDER.value:
                 response += cls._str_(item.value.items)
             else:
                 response += f'{item.value}'
             response += ","
         if len(items) > 0:
             response = response[:-1]
         if len(items) == 0:
@@ -607,15 +613,18 @@
     def __delitem__(self, index):
         del self.items[index]
 
     def __contains__(self, item):
         return DollarListWriter().create_dollar_item(item) in self.items
 
     def __eq__(self, other):
-        return self.items == other.items
+        # check if the other object is a DollarList
+        # and if the items are the same
+        if isinstance(other, DollarList):
+            return self.items == other.items
 
     def __ne__(self, other):
         return self.items != other.items
 
     def __add__(self, other):
         result = self.items + other.items
         return DollarList(result)
```

### Comparing `iris-dollar-list-0.9.5/src/iris_dollar_list.egg-info/PKG-INFO` & `iris-dollar-list-0.9.6/src/iris_dollar_list.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-dollar-list
-Version: 0.9.5
+Version: 0.9.6
 Summary: iris-dollar-list
 Home-page: https://github.com/grongierisc/iris-dollar-list
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris-dollar-list
 Classifier: Development Status :: 5 - Production/Stable
```

