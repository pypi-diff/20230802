# Comparing `tmp/formulite-0.0.1.tar.gz` & `tmp/formulite-0.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formulite-0.0.1.tar", last modified: Wed Aug  2 02:40:48 2023, max compression
+gzip compressed data, was "formulite-0.0.1.dev0.tar", last modified: Tue Aug  1 15:01:26 2023, max compression
```

## Comparing `formulite-0.0.1.tar` & `formulite-0.0.1.dev0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:40:48.551761 formulite-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-08-02 02:35:43.000000 formulite-0.0.1/LICENSE.MIT
--rw-rw-rw-   0        0        0      821 2023-08-02 02:40:48.548946 formulite-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-08-02 02:38:59.000000 formulite-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 02:40:48.540012 formulite-0.0.1/formulite/
--rw-rw-rw-   0        0        0      112 2023-08-01 13:35:03.000000 formulite-0.0.1/formulite/__init__.py
--rw-rw-rw-   0        0        0    14407 2023-08-02 02:19:42.000000 formulite-0.0.1/formulite/calc_parser.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:40:48.547963 formulite-0.0.1/formulite.egg-info/
--rw-rw-rw-   0        0        0      821 2023-08-02 02:40:48.000000 formulite-0.0.1/formulite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-08-02 02:40:48.000000 formulite-0.0.1/formulite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 02:40:48.000000 formulite-0.0.1/formulite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 02:40:48.000000 formulite-0.0.1/formulite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 02:40:48.551761 formulite-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-08-02 02:34:49.000000 formulite-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.640467 formulite-0.0.1.dev0/
+-rw-rw-rw-   0        0        0      301 2023-08-01 15:01:26.637841 formulite-0.0.1.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-01 13:35:39.000000 formulite-0.0.1.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.628006 formulite-0.0.1.dev0/formulite/
+-rw-rw-rw-   0        0        0      112 2023-08-01 13:35:03.000000 formulite-0.0.1.dev0/formulite/__init__.py
+-rw-rw-rw-   0        0        0    14403 2023-07-28 00:52:13.000000 formulite-0.0.1.dev0/formulite/calc_parser.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.633856 formulite-0.0.1.dev0/formulite.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-01 15:01:26.000000 formulite-0.0.1.dev0/formulite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 15:01:26.640467 formulite-0.0.1.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-08-01 15:00:50.000000 formulite-0.0.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 15:01:26.635847 formulite-0.0.1.dev0/test/
+-rw-rw-rw-   0        0        0        0 2023-08-01 13:20:13.000000 formulite-0.0.1.dev0/test/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-08-01 13:28:02.000000 formulite-0.0.1.dev0/test/main.py
```

### Comparing `formulite-0.0.1/formulite/calc_parser.py` & `formulite-0.0.1.dev0/formulite/calc_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
         return formula_tree(
             funcname,
             Elem_type.FUNCTION,
             [self.resolve_util(i)[0] for i in funcdata[1:]]
         )
 
     def resolve(self):
-        return self.resolve_util(self.code)[0]
+        return self.resolve_util(self.code)
     def priority(self,vec:list[str])->int|None:
         #配列内にある最も優先順位が低い演算子を探します
         #返り値はindexです
         """
         実装されている計算規則
         rankの数字が低いものほど計算順位も低い
         同一のランクが並列に続く場合、式の右に行く程計算順位が低い
@@ -422,19 +422,19 @@
     "sin(x)",
     "(1)+2",
     "3.14",
     "-8+6"
     ]
     """
     texts = [
-        "f(x)+g(x,y,z)*5"
+        "main(a,b,c)"
     ]
     for i in texts:
         par=parser(i)
-        print(par.resolve())
+        print(par.resolve()[0])
     el = elem("-sin(x)")
     print(el.elemtype)
     #print(
     #    elem.new(" sin(x) ").elemtype
     #)
```

### Comparing `formulite-0.0.1/setup.py` & `formulite-0.0.1.dev0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup,find_packages
 
 with open("README.md",encoding="utf-8",mode="r")as f:
     long_description = f.read()
 
 setup(
     name="formulite",
-    version="0.0.1",
+    version="0.0.1.dev0",
     description='Simple Formula Parser',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Tom0427',
     author_email='tom.ipynb@gmail.com',
     license='MIT',
     keywords='parser, formula, formulite',
     python_requires='>=3',
-    packages=find_packages(),
-    url="https://github.com/Tom-game-project/formulite"
+    packages=find_packages()
 )
```

