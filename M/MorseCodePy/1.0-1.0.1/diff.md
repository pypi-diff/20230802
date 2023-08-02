# Comparing `tmp/MorseCodePy-1.0.tar.gz` & `tmp/MorseCodePy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MorseCodePy-1.0.tar", last modified: Tue Aug  1 12:16:26 2023, max compression
+gzip compressed data, was "MorseCodePy-1.0.1.tar", last modified: Wed Aug  2 19:51:12 2023, max compression
```

## Comparing `MorseCodePy-1.0.tar` & `MorseCodePy-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:16:26.551752 MorseCodePy-1.0/
-drwxrwxrwx   0        0        0        0 2023-08-01 12:16:26.544753 MorseCodePy-1.0/MorseCodePy/
--rw-rw-rw-   0        0        0     2209 2023-08-01 12:12:50.000000 MorseCodePy-1.0/MorseCodePy/MorseCodePy.py
--rw-rw-rw-   0        0        0       28 2023-08-01 11:44:29.000000 MorseCodePy-1.0/MorseCodePy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:16:26.549752 MorseCodePy-1.0/MorseCodePy.egg-info/
--rw-rw-rw-   0        0        0      278 2023-08-01 12:16:26.000000 MorseCodePy-1.0/MorseCodePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-08-01 12:16:26.000000 MorseCodePy-1.0/MorseCodePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:16:26.000000 MorseCodePy-1.0/MorseCodePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-01 12:16:26.000000 MorseCodePy-1.0/MorseCodePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      278 2023-08-01 12:16:26.550752 MorseCodePy-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-08-01 11:45:54.000000 MorseCodePy-1.0/README.md
--rw-rw-rw-   0        0        0     1069 2023-08-01 10:56:06.000000 MorseCodePy-1.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 12:16:26.551752 MorseCodePy-1.0/setup.cfg
--rw-rw-rw-   0        0        0      276 2023-08-01 12:16:13.000000 MorseCodePy-1.0/setup.py
+drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 19:51:12.876990 MorseCodePy-1.0.1/
+drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 19:51:12.876225 MorseCodePy-1.0.1/MorseCodePy/
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     2218 2023-08-02 19:31:31.000000 MorseCodePy-1.0.1/MorseCodePy/MorseCodePy.py
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)       28 2023-08-01 11:44:30.000000 MorseCodePy-1.0.1/MorseCodePy/__init__.py
+drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-08-02 19:51:12.876683 MorseCodePy-1.0.1/MorseCodePy.egg-info/
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1397 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/PKG-INFO
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)      221 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)        1 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)       12 2023-08-02 19:51:12.000000 MorseCodePy-1.0.1/MorseCodePy.egg-info/top_level.txt
+-rw-r--r--   0 artemkarpenko   (501) staff       (20)     1397 2023-08-02 19:51:12.876873 MorseCodePy-1.0.1/PKG-INFO
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1138 2023-08-02 19:50:24.000000 MorseCodePy-1.0.1/README.md
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)     1069 2023-08-01 10:56:08.000000 MorseCodePy-1.0.1/license.txt
+-rw-r--r--   0 artemkarpenko   (501) staff       (20)       38 2023-08-02 19:51:12.877031 MorseCodePy-1.0.1/setup.cfg
+-rwxrwxrwx   0 artemkarpenko   (501) staff       (20)      581 2023-08-02 19:49:56.000000 MorseCodePy-1.0.1/setup.py
```

### Comparing `MorseCodePy-1.0/MorseCodePy/MorseCodePy.py` & `MorseCodePy-1.0.1/MorseCodePy/MorseCodePy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 codes: dict = {  # Dictionary of characters and their translations into Morse code
     # English
     'a': '01', 'b': '1000', 'c': '1010', 'd': '100', 'e': '0', 'f': '0010', 'g': '110', 'h': '0000',
     'i': '00', 'j': '0111', 'k': '101', 'l': '0100', 'm': '11', 'n': '10', 'o': '111', 'p': '0110',
-    'q': '1101', 'r': '010', 's': '111', 't': '1', 'u': '001', 'v': '0001', 'w': '011', 'x': '1001',
+    'q': '1101', 'r': '010', 's': '000', 't': '1', 'u': '001', 'v': '0001', 'w': '011', 'x': '1001',
     'y': '1011', 'z': '1100',
     # Russian
     'а': '01', 'б': '1000', 'в': '011', 'г': '110', 'д': '100', 'е': '0', 'ё': '0', 'ж': '0001',
     'з': '1100', 'и': '00', 'й': '0111', 'к': '101', 'л': '0001', 'м': '11', 'н': '10', 'о': '111',
     'п': '0110', 'р': '010', 'с': '000', 'т': '1', 'у': '001', 'ф': '0010', 'х': '0000', 'ц': '1010',
     'ч': '1110', 'ш': '1111', 'щ': '1101', 'ъ': '11011', 'ы': '1011', 'ь': '1001', 'э': '00100',
     'ю': '0011', 'я': '0101',
@@ -19,21 +19,23 @@
     '\"': '010010', '$': '0001001', '+': '01010', '-': '100001', '=': '10001', '_': '001101',
     # Other letters
     'ґ': '110', 'і': '00', 'є': '00100', 'ї': '01110', 'à': '01101', 'ç': '10100', 'è': '01001', 'é': '00100',
     'â': '01101', 'ê': '10010', 'ë': '00100', 'ï': '10011', 'ü': '0011', 'á': '01101', 'ó': '1110',
     'ñ': '11011'
 }
 
-def encode(string: str, dit_symbol: chr = '·', dash_symbol: chr = '-') -> str:
+def encode(string: str, dit: chr = '·', dash: chr = '-') -> str:
     """
     This function translates your string into Morse code.
     You can customize dits and dashes
     """
 
-    t_string = str()  # New string that hold translated text (result)
+    t_string = str()  # New string that will hold translated text
     for char in string:
         try:
-            t_string += codes[char.lower()].replace('0', dit_symbol).replace('1', dash_symbol) + ' '
+            t_string += codes[char.lower()].replace('0', dit).replace('1', dash) + ' '
         except:
-            t_string += '* '  # If character is not is dictionary "codes", it will return...
+            t_string += '* '  # If character isn't is dictionary "codes", it will return...
 
     return t_string.strip()
+
+print(encode("Bye!", dit='0', dash='1'))
```

### Comparing `MorseCodePy-1.0/license.txt` & `MorseCodePy-1.0.1/license.txt`

 * *Files identical despite different names*

