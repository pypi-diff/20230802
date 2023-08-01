# Comparing `tmp/equation-sampler-0.0.1.tar.gz` & `tmp/equation-sampler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equation-sampler-0.0.1.tar", last modified: Tue Aug  1 22:12:23 2023, max compression
+gzip compressed data, was "equation-sampler-0.0.2.tar", last modified: Tue Aug  1 22:22:02 2023, max compression
```

## Comparing `equation-sampler-0.0.1.tar` & `equation-sampler-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.280479 equation-sampler-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.276479 equation-sampler-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.276479 equation-sampler-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-01 22:12:23.280479 equation-sampler-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.276479 equation-sampler-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.276479 equation-sampler-0.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.276479 equation-sampler-0.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:12:23.280479 equation-sampler-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.276479 equation-sampler-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.280479 equation-sampler-0.0.1/src/equation_sampler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-01 22:12:23.000000 equation-sampler-0.0.1/src/equation_sampler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 22:12:23.000000 equation-sampler-0.0.1/src/equation_sampler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:12:23.000000 equation-sampler-0.0.1/src/equation_sampler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 22:12:23.000000 equation-sampler-0.0.1/src/equation_sampler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 22:12:23.000000 equation-sampler-0.0.1/src/equation_sampler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19615 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/src/equation_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:23.280479 equation-sampler-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/tests/test_equation_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-01 22:12:12.000000 equation-sampler-0.0.1/tests/test_equation_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.936308 equation-sampler-0.0.2/src/equation_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/src/equation_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19615 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/src/equation_sampler/equation_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/src/equation_sampler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 22:22:02.000000 equation-sampler-0.0.2/src/equation_sampler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:22:02.940309 equation-sampler-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/test_equation_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-01 22:21:48.000000 equation-sampler-0.0.2/tests/test_equation_tree.py
```

### Comparing `equation-sampler-0.0.1/.github/pull_request_template.md` & `equation-sampler-0.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/.github/workflows/python-publish.yml` & `equation-sampler-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/.gitignore` & `equation-sampler-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/.pre-commit-config.yaml` & `equation-sampler-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/PKG-INFO` & `equation-sampler-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equation-sampler
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool to sample equations
 Author-email: Ioana Marinescu <ioanam@princeton.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic-generator-equation-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `equation-sampler-0.0.1/README.md` & `equation-sampler-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/docs/Additional Example.ipynb` & `equation-sampler-0.0.2/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/docs/Basic Usage.ipynb` & `equation-sampler-0.0.2/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/docs/index.md` & `equation-sampler-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/mkdocs/base.yml` & `equation-sampler-0.0.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/pyproject.toml` & `equation-sampler-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/src/__init__.py` & `equation-sampler-0.0.2/src/equation_sampler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     n = len(infix)
     char_stack = []
     output = []
     i = 0
     while i < n:
         # Check if the character is alphabet or digit
         if infix[i].isdigit() and infix[i + 1] == "_":
-            output.append(infix[i: i + 3][::-1])
+            output.append(infix[i : i + 3][::-1])
             i += 2
         elif infix[i].isdigit():
             output.append(infix[i])
 
         # If the character is '(' push it in the stack
         elif infix[i] == "(":
             char_stack.append(infix[i])
@@ -61,17 +61,17 @@
         elif infix[i] == ")":
             while char_stack[-1] != "(":
                 output.append(char_stack.pop())
             char_stack.pop()
         # Found an operator
         else:
             if (
-                    char_stack[-1] in function_space
-                    or char_stack[-1] in operation_space
-                    or char_stack[-1] in [")", "("]
+                char_stack[-1] in function_space
+                or char_stack[-1] in operation_space
+                or char_stack[-1] in [")", "("]
             ):
                 if infix[i] == "^":
                     while get_priority(infix[i]) <= get_priority(char_stack[-1]):
                         output.append(char_stack.pop())
                     char_stack.append(infix[i])
                 elif infix[i].isalpha():
                     fct = ""
@@ -110,33 +110,33 @@
     prefix = infix_to_postfix(infix, function_space, operation_space)
     prefix = prefix[::-1]
 
     return prefix
 
 
 def sample_equations(
-        num_samples: int,
-        max_depth: int,
-        max_num_variables: int,
-        max_num_constants: int,
-        function_space: list,
-        operation_space: list,
-        without_replacement: bool = True,
-        fix_num_variables_to_max: bool = False,
-        include_zero_as_constant=False,
-        min_input_value: float = -1,
-        max_input_value: float = 1,
-        min_constant_value: float = -1,
-        max_constant_value: float = 1,
-        num_input_points: int = 100,
-        num_constant_points: int = 100,
-        num_evaluation_samples: int = 100,
-        max_iter: int = 1000000,
-        require_simplify=True,
-        verbose=True,
+    num_samples: int,
+    max_depth: int,
+    max_num_variables: int,
+    max_num_constants: int,
+    function_space: list,
+    operation_space: list,
+    without_replacement: bool = True,
+    fix_num_variables_to_max: bool = False,
+    include_zero_as_constant=False,
+    min_input_value: float = -1,
+    max_input_value: float = 1,
+    min_constant_value: float = -1,
+    max_constant_value: float = 1,
+    num_input_points: int = 100,
+    num_constant_points: int = 100,
+    num_evaluation_samples: int = 100,
+    max_iter: int = 1000000,
+    require_simplify=True,
+    verbose=True,
 ):
     """
     Generate data for the equation generator.
 
     Arguments:
         num_samples: Number of samples to generate.
         max_depth: Maximum depth of the equation tree.
@@ -227,16 +227,16 @@
                 continue
 
             # if tree has too many variables or constants, continue
             if tree.num_x > max_num_variables or tree.num_c > max_num_constants:
                 continue
 
             if (
-                    fix_num_variables_to_max
-                    and len(np.unique(tree.variables)) < max_num_variables
+                fix_num_variables_to_max
+                and len(np.unique(tree.variables)) < max_num_variables
             ):
                 continue
 
             # now we evaluate each node in the tree for a grid of inputs and constants
             crossings = create_crossings(
                 tree.num_x,
                 tree.num_c,
@@ -286,23 +286,23 @@
         evaluation_list[idx] = evaluation.T
 
     print("all equations generated")
     return equation_list, evaluation_list
 
 
 def create_crossings(
-        num_inputs,
-        num_constants,
-        min_input_value: float = -1,
-        max_input_value: float = 1,
-        min_constant_value: float = -1,
-        max_constant_value: float = 1,
-        num_input_points: int = 100,
-        num_constant_points: int = 100,
-        num_evaluation_samples: int = 100,
+    num_inputs,
+    num_constants,
+    min_input_value: float = -1,
+    max_input_value: float = 1,
+    min_constant_value: float = -1,
+    max_constant_value: float = 1,
+    num_input_points: int = 100,
+    num_constant_points: int = 100,
+    num_evaluation_samples: int = 100,
 ):
     grids = []
 
     for variable in range(num_inputs):
         # Create an evenly spaced grid for each variable
         grid = np.linspace(min_input_value, max_input_value, num_input_points)
         grids.append(grid)
@@ -322,20 +322,20 @@
         )
         crossings = crossings[indices]
 
     return crossings
 
 
 def get_evaluation(
-        crossings,
-        tree,
-        num_evaluation_samples=100,
-        include_zero_as_constant=False,
-        max_nodes_for_evaluation=None,
-        transpose=False,
+    crossings,
+    tree,
+    num_evaluation_samples=100,
+    include_zero_as_constant=False,
+    max_nodes_for_evaluation=None,
+    transpose=False,
 ):
     evaluation = np.zeros((num_evaluation_samples, len(tree.expr)))
 
     # get all the x labels
     x_labels = list()
     for element in tree.expr:
         # if element in feature_space:
```

### Comparing `equation-sampler-0.0.1/src/equation_sampler.egg-info/PKG-INFO` & `equation-sampler-0.0.2/src/equation_sampler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equation-sampler
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool to sample equations
 Author-email: Ioana Marinescu <ioanam@princeton.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic-generator-equation-sampler
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `equation-sampler-0.0.1/src/equation_sampler.egg-info/SOURCES.txt` & `equation-sampler-0.0.2/src/equation_sampler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 .github/workflows/python-publish.yml
 docs/Additional Example.ipynb
 docs/Basic Usage.ipynb
 docs/index.md
 docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
-src/__init__.py
-src/equation_tree.py
+src/equation_sampler/__init__.py
+src/equation_sampler/equation_tree.py
 src/equation_sampler.egg-info/PKG-INFO
 src/equation_sampler.egg-info/SOURCES.txt
 src/equation_sampler.egg-info/dependency_links.txt
 src/equation_sampler.egg-info/requires.txt
 src/equation_sampler.egg-info/top_level.txt
 tests/README.md
 tests/__init__.py
```

### Comparing `equation-sampler-0.0.1/src/equation_tree.py` & `equation-sampler-0.0.2/src/equation_sampler/equation_tree.py`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/tests/README.md` & `equation-sampler-0.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `equation-sampler-0.0.1/tests/test_equation_sampler.py` & `equation-sampler-0.0.2/tests/test_equation_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from src import infix_to_prefix, prefix_to_infix, simplify
+from equation_sampler import infix_to_prefix, prefix_to_infix, simplify
 
 
 def test_simplification():
     np.random.seed(42)
     function_space = ["sin", "cos", "tan", "exp", "log", "sqrt", "abs"]
     operation_space = ["+", "-", "*", "/"]
     tree = ["*", "sqrt", "x_1", "x_1"]
```

### Comparing `equation-sampler-0.0.1/tests/test_equation_tree.py` & `equation-sampler-0.0.2/tests/test_equation_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from src.equation_tree import EquationTree
+from equation_sampler.equation_tree import EquationTree
 
 
 def test_equation_sampler():
     np.random.seed(42)
     tree_structure = [0, 1, 2, 3, 2, 1]
     operation_space = ["+", "-", "*", "/"]
     function_space = ["sin", "cos", "tan", "exp", "log", "sqrt", "abs"]
```

