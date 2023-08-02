# Comparing `tmp/ecabc-3.0.0.tar.gz` & `tmp/ecabc-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ecabc-3.0.0.tar", last modified: Mon Oct  5 18:59:55 2020, max compression
+gzip compressed data, was "ecabc-3.0.1.tar", last modified: Wed Aug  2 03:20:52 2023, max compression
```

## Comparing `ecabc-3.0.0.tar` & `ecabc-3.0.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2020-10-05 18:59:55.000000 ecabc-3.0.0/
--rw-rw-rw-   0        0        0      394 2020-10-05 18:59:55.000000 ecabc-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10490 2020-10-05 18:10:52.000000 ecabc-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc/
--rw-rw-rw-   0        0        0      136 2020-10-05 18:05:28.000000 ecabc-3.0.0/ecabc/__init__.py
--rw-rw-rw-   0        0        0    11300 2020-10-05 18:05:28.000000 ecabc-3.0.0/ecabc/abc.py
--rw-rw-rw-   0        0        0     3263 2020-10-05 18:05:28.000000 ecabc-3.0.0/ecabc/bee.py
--rw-rw-rw-   0        0        0     3319 2020-10-05 18:05:28.000000 ecabc-3.0.0/ecabc/parameter.py
--rw-rw-rw-   0        0        0     3040 2020-10-05 18:05:28.000000 ecabc-3.0.0/ecabc/utils.py
-drwxrwxrwx   0        0        0        0 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc.egg-info/
--rw-rw-rw-   0        0        0      394 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2020-10-05 18:59:55.000000 ecabc-3.0.0/ecabc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-10-05 18:59:55.000000 ecabc-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      526 2020-10-05 18:05:28.000000 ecabc-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:20:52.051891 ecabc-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 03:20:42.000000 ecabc-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-08-02 03:20:52.051891 ecabc-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-08-02 03:20:42.000000 ecabc-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:20:52.051891 ecabc-3.0.1/ecabc/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-02 03:20:42.000000 ecabc-3.0.1/ecabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-08-02 03:20:42.000000 ecabc-3.0.1/ecabc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-02 03:20:42.000000 ecabc-3.0.1/ecabc/bee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-08-02 03:20:42.000000 ecabc-3.0.1/ecabc/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-08-02 03:20:42.000000 ecabc-3.0.1/ecabc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:20:52.051891 ecabc-3.0.1/ecabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-08-02 03:20:52.000000 ecabc-3.0.1/ecabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 03:20:52.000000 ecabc-3.0.1/ecabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 03:20:52.000000 ecabc-3.0.1/ecabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 03:20:52.000000 ecabc-3.0.1/ecabc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:20:52.051891 ecabc-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-02 03:20:42.000000 ecabc-3.0.1/examples/minimize_integers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-02 03:20:42.000000 ecabc-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 03:20:52.051891 ecabc-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:20:52.051891 ecabc-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-08-02 03:20:42.000000 ecabc-3.0.1/tests/test_all.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ecabc-3.0.0/README.md` & `ecabc-3.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,244 +1,257 @@
-[![UML Energy & Combustion Research Laboratory](http://faculty.uml.edu/Hunter_Mack/uploads/9/7/1/3/97138798/1481826668_2.png)](http://faculty.uml.edu/Hunter_Mack/)
-
-# ECabc: optimization algorithm for tuning user-defined parametric functions 
-[![GitHub version](https://badge.fury.io/gh/ECRL%2FECabc.svg)](https://badge.fury.io/gh/ECRL%2FECabc)
-[![PyPI version](https://badge.fury.io/py/ecabc.svg)](https://badge.fury.io/py/ecabc)
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ECRL/ecabc/blob/master/LICENSE)
-[![DOI](http://joss.theoj.org/papers/10.21105/joss.01420/status.svg)](https://doi.org/10.21105/joss.01420)
-[![Build Status](https://dev.azure.com/uml-ecrl/package-management/_apis/build/status/ECRL.ecabc?branchName=master)](https://dev.azure.com/uml-ecrl/package-management/_build/latest?definitionId=5&branchName=master)
-
-**ECabc** is an open source Python package used to tune parameters for user-supplied functions based on the [Artificial Bee Colony by D. Karaboğa](http://scholarpedia.org/article/Artificial_bee_colony_algorithm). ECabc optimizes user supplied functions, or **fitness function**s, using a set of variables that exist within a search space. The bee colony consists of three types of bees: employers, onlookers and scouts. An **employer bee** exploits a solution comprised of a permutation of the variables in the search space, and evaluates the viability of the solution. An **onlooker bee** chooses an employer bee with an optimal solution and searches for new solutions near them. The **scout bee**, a variant of the employer bee, will search for a new solution if it has stayed too long at its current solution.
-
-<p align="center">
-  <img align="center" src="docs/img/abc_visual_convergence.gif" width="75%" height="75%">
-</p>
-
-### Research applications
-While it has several applications, ECabc has been successfully used by the Energy and Combustion Research Laboratory (ECRL) at the University of Massachusetts Lowell to tune the hyperparameters of ECNet, an open source Python package tailored to predicting fuel properties. ECNet provides scientists an open source tool for predicting key fuel properties of potential next-generation biofuels, reducing the need for costly fuel synthesis and experimentation. By increasing the accuracy of ECNet and similar models efficiently, ECabc helps to provide a higher degree of confidence in discovering new, optimal fuels. A single run of ECabc on ECNet yielded a lower average root mean square error (RMSE) for cetane number (CN) and yield sooting index (YSI) when compared to the RMSE generated by a year of manual tuning. While the manual tuning generated an RMSE of 10.13, the ECabc was able to yield an RMSE of 8.06 in one run of 500 iterations.
-
-# Installation
-
-### Prerequisites:
-- Have python 3.X installed
-- Have the ability to install python packages
-
-### Method 1: pip
-If you are working in a Linux/Mac environment:
-```
-sudo pip install ecabc
-```
-
-Alternatively, in a Windows or virtualenv environment:
-```
-pip install ecabc
-```
-
-To update your version of ECabc to the latest release version, use
-```
-pip install --upgrade ecabc
-```
-
-Note: if multiple Python releases are installed on your system (e.g. 2.7 and 3.7), you may need to execute the correct version of pip. For Python 3.X, change **"pip install ecabc"** to **"pip3 install ecabc"**.
-
-### Method 2: From source
-- Download the ECabc repository, navigate to the download location on the command line/terminal, and execute:
-```
-python setup.py install
-```
-
-There are currently no additional dependencies for ECabc.
-
-# Usage
-
-To start using ECabc, you need a couple items:
-- a fitness function (cost function) to optimize
-- parameters used by the fitness function
-
-For example, let's define a fitness function to minimize the sum of three integers:
-
-```python
-def minimize_integers(integers):
-
-    return sum(integers)
-
-```
-
-Your fitness function must accept a **list** from ECabc. The list values represent the current "food source", i.e. parameter values, being exploited by a given bee.
-
-Now that we have our fitness function, let's import the ABC object from ECabc, initialize the artificial bee colony, and add our parameters:
-
-```python
-from ecabc import ABC
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-abc = ABC(10, minimize_integers)
-abc.add_param(0, 10, name='Int_1')
-abc.add_param(0, 10, name='Int_2')
-abc.add_param(0, 10, name='Int_3')
-```
-
-Here we initialize the colony with 10 employer bees, supply our fitness function, and add our parameters. Parameters are added with minimum/maximum values for its search space and optionally a name. By default, parameter mutations (searching a neighboring food source) will not exceed the specified parameter bounds [min_val, max_val]; if this limitation is not desired, supply the "restrict=False" argument:
-
-```python
-abc.add_param(0, 10, restrict=False, name='Int_1')
-```
-
-Once we have created our colony and added our parameters, we then need to "initialize" the colony's bees:
-
-```python
-from ecabc import ABC
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-abc = ABC(10, minimize_integers)
-abc.add_param(0, 10, name='Int_1')
-abc.add_param(0, 10, name='Int_2')
-abc.add_param(0, 10, name='Int_3')
-abc.initialize()
-```
-
-Initializing the colony's bees deploys employer bees (in this example, 10 bees) to random food sources (random parameter values are generated), their fitness is evaluated (in this example, lowest sum is better), and onlooker bees (equal to the number of employers) are deployed proportionally to neighboring food sources of well-performing bees.
-
-We then send the colony through a predetermined of "search cycles":
-
-```python
-from ecabc import ABC
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-abc = ABC(10, minimize_integers)
-abc.add_param(0, 10, name='Int_1')
-abc.add_param(0, 10, name='Int_2')
-abc.add_param(0, 10, name='Int_3')
-abc.initialize()
-for _ in range(10):
-    abc.search()
-```
-
-A search cycle consists of:
-- each bee searches a neighboring food source (performs a mutation on one parameter)
-- if the food source produces a better fitness than the bee's current food source, move there
-- otherwise, the bee stays at its current food source
-    - if the bee has stayed for (NE * D) cycles (NE = number of employers, D = dimension of the function, 3 in our example), abandon the food source
-        - if the bee is an employer, go to a new random food source
-        - if the bee is an onlooker, go to a food source neighboring a well-performing bee
-
-We can access the colony's average fitness score, average fitness function return value, best fitness score, best fitness function return value and best parameters at any time:
-
-```python
-print(abc.average_fitness)
-print(abc.average_ret_val)
-print(abc.best_fitness)
-print(abc.best_ret_val)
-print(abc.best_params)
-```
-
-ECabc can utilize multiple CPU cores for concurrent processing:
-
-```python
-abc = ABC(10, minimize_integers, num_processes=8)
-```
-
-Tying everything together, we have:
-
-```python
-from ecabc import ABC
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-abc = ABC(10, minimize_integers)
-abc.add_param(0, 10, name='Int_1')
-abc.add_param(0, 10, name='Int_2')
-abc.add_param(0, 10, name='Int_3')
-abc.initialize()
-for _ in range(10):
-    abc.search()
-    print('Average fitness: {}'.format(abc.average_fitness))
-    print('Average obj. fn. return value: {}'.format(abc.average_ret_val))
-    print('Best fitness score: {}'.format(abc.best_fitness))
-    print('Best obj. fn. return value: {}'.format(abc.best_ret_val))
-    print('Best parameters: {}\n'.format(abc.best_params))
-```
-
-Running this script produces:
-
-```
-Average fitness: 0.08244866244866243
-Average obj. fn. return value: 11.65
-Best fitness score: 0.125
-Best obj. fn. return value: 7
-Best parameters: {'Int_1': 4, 'Int_2': 3, 'Int_3': 0}
-
-Average fitness: 0.0885855117105117
-Average obj. fn. return value: 10.8
-Best fitness score: 0.125
-Best obj. fn. return value: 7
-Best parameters: {'Int_1': 4, 'Int_2': 3, 'Int_3': 0}
-
-Average fitness: 0.10361832611832611
-Average obj. fn. return value: 9.4
-Best fitness score: 0.16666666666666666
-Best obj. fn. return value: 5
-Best parameters: {'Int_1': 2, 'Int_2': 3, 'Int_3': 0}
-
-Average fitness: 0.11173502151443326
-Average obj. fn. return value: 8.8
-Best fitness score: 0.2
-Best obj. fn. return value: 4
-Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 4}
-
-Average fitness: 0.12448879551820731
-Average obj. fn. return value: 7.95
-Best fitness score: 0.2
-Best obj. fn. return value: 4
-Best parameters: {'Int_1': 1, 'Int_2': 3, 'Int_3': 0}
-
-Average fitness: 0.1767694805194805
-Average obj. fn. return value: 6.7
-Best fitness score: 1.0
-Best obj. fn. return value: 0
-Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
-
-Average fitness: 0.183255772005772
-Average obj. fn. return value: 6.3
-Best fitness score: 1.0
-Best obj. fn. return value: 0
-Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
-
-Average fitness: 0.20172799422799423
-Average obj. fn. return value: 5.65
-Best fitness score: 1.0
-Best obj. fn. return value: 0
-Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
-
-Average fitness: 0.23827561327561328
-Average obj. fn. return value: 4.95
-Best fitness score: 1.0
-Best obj. fn. return value: 0
-Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
-
-Average fitness: 0.28456349206349213
-Average obj. fn. return value: 4.35
-Best fitness score: 1.0
-Best obj. fn. return value: 0
-Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
-```
-
-To run this script yourself, head over to our [examples](https://github.com/ecrl/ecabc/tree/master/examples) directory.
-
-# Contributing, Reporting Issues and Other Support:
-
-To contribute to ECabc, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
-
-To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
-
-For additional support/questions, contact Sanskriti Sharma (Sanskriti_Sharma@student.uml.edu), Hernan Gelaf-Romer (Hernan_Gelafromer@student.uml.edu), or Travis Kessler (Travis_Kessler@student.uml.edu).
+Metadata-Version: 2.1
+Name: ecabc
+Version: 3.0.1
+Summary: Artificial bee colony for function parameter optimization
+Author-email: Sanskriti Sharma <Sanskriti_Sharma@student.uml.edu>, Hernan Gelaf-Romer <Hernan_Gelafromer@student.uml.edu>, Travis Kessler <travis.j.kessler@gmail.com>
+Project-URL: Homepage, https://github.com/ecrl/ecabc
+Project-URL: Bug Tracker, https://github.com/ecrl/ecabc/issues
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
+
+# ECabc: optimization algorithm for tuning user-defined parametric functions 
+[![GitHub version](https://badge.fury.io/gh/ECRL%2FECabc.svg)](https://badge.fury.io/gh/ECRL%2FECabc)
+[![PyPI version](https://badge.fury.io/py/ecabc.svg)](https://badge.fury.io/py/ecabc)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ECRL/ecabc/blob/master/LICENSE)
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.01420/status.svg)](https://doi.org/10.21105/joss.01420)
+
+**ECabc** is an open source Python package used to tune parameters for user-supplied functions based on the [Artificial Bee Colony by D. Karaboğa](http://scholarpedia.org/article/Artificial_bee_colony_algorithm). ECabc optimizes user supplied functions, or **fitness function**s, using a set of variables that exist within a search space. The bee colony consists of three types of bees: employers, onlookers and scouts. An **employer bee** exploits a solution comprised of a permutation of the variables in the search space, and evaluates the viability of the solution. An **onlooker bee** chooses an employer bee with an optimal solution and searches for new solutions near them. The **scout bee**, a variant of the employer bee, will search for a new solution if it has stayed too long at its current solution.
+
+<p align="center">
+  <img align="center" src="docs/img/abc_visual_convergence.gif" width="75%" height="75%">
+</p>
+
+### Research applications
+While it has several applications, ECabc has been successfully used by the Energy and Combustion Research Laboratory (ECRL) at the University of Massachusetts Lowell to tune the hyperparameters of ECNet, an open source Python package tailored to predicting fuel properties. ECNet provides scientists an open source tool for predicting key fuel properties of potential next-generation biofuels, reducing the need for costly fuel synthesis and experimentation. By increasing the accuracy of ECNet and similar models efficiently, ECabc helps to provide a higher degree of confidence in discovering new, optimal fuels. A single run of ECabc on ECNet yielded a lower average root mean square error (RMSE) for cetane number (CN) and yield sooting index (YSI) when compared to the RMSE generated by a year of manual tuning. While the manual tuning generated an RMSE of 10.13, the ECabc was able to yield an RMSE of 8.06 in one run of 500 iterations.
+
+# Installation
+
+### Prerequisites:
+- Have python 3.X installed
+- Have the ability to install python packages
+
+### Method 1: pip
+If you are working in a Linux/Mac environment:
+```
+sudo pip install ecabc
+```
+
+Alternatively, in a Windows or virtualenv environment:
+```
+pip install ecabc
+```
+
+To update your version of ECabc to the latest release version, use
+```
+pip install --upgrade ecabc
+```
+
+Note: if multiple Python releases are installed on your system (e.g. 2.7 and 3.7), you may need to execute the correct version of pip. For Python 3.X, change **"pip install ecabc"** to **"pip3 install ecabc"**.
+
+### Method 2: From source
+- Download the ECabc repository, navigate to the download location on the command line/terminal, and execute:
+```
+pip install .
+```
+
+There are currently no additional dependencies for ECabc.
+
+# Usage
+
+To start using ECabc, you need a couple items:
+- a fitness function (cost function) to optimize
+- parameters used by the fitness function
+
+For example, let's define a fitness function to minimize the sum of three integers:
+
+```python
+def minimize_integers(integers):
+
+    return sum(integers)
+
+```
+
+Your fitness function must accept a **list** from ECabc. The list values represent the current "food source", i.e. parameter values, being exploited by a given bee.
+
+Now that we have our fitness function, let's import the ABC object from ECabc, initialize the artificial bee colony, and add our parameters:
+
+```python
+from ecabc import ABC
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+abc = ABC(10, minimize_integers)
+abc.add_param(0, 10, name='Int_1')
+abc.add_param(0, 10, name='Int_2')
+abc.add_param(0, 10, name='Int_3')
+```
+
+Here we initialize the colony with 10 employer bees, supply our fitness function, and add our parameters. Parameters are added with minimum/maximum values for its search space and optionally a name. By default, parameter mutations (searching a neighboring food source) will not exceed the specified parameter bounds [min_val, max_val]; if this limitation is not desired, supply the "restrict=False" argument:
+
+```python
+abc.add_param(0, 10, restrict=False, name='Int_1')
+```
+
+Once we have created our colony and added our parameters, we then need to "initialize" the colony's bees:
+
+```python
+from ecabc import ABC
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+abc = ABC(10, minimize_integers)
+abc.add_param(0, 10, name='Int_1')
+abc.add_param(0, 10, name='Int_2')
+abc.add_param(0, 10, name='Int_3')
+abc.initialize()
+```
+
+Initializing the colony's bees deploys employer bees (in this example, 10 bees) to random food sources (random parameter values are generated), their fitness is evaluated (in this example, lowest sum is better), and onlooker bees (equal to the number of employers) are deployed proportionally to neighboring food sources of well-performing bees.
+
+We then send the colony through a predetermined of "search cycles":
+
+```python
+from ecabc import ABC
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+abc = ABC(10, minimize_integers)
+abc.add_param(0, 10, name='Int_1')
+abc.add_param(0, 10, name='Int_2')
+abc.add_param(0, 10, name='Int_3')
+abc.initialize()
+for _ in range(10):
+    abc.search()
+```
+
+A search cycle consists of:
+- each bee searches a neighboring food source (performs a mutation on one parameter)
+- if the food source produces a better fitness than the bee's current food source, move there
+- otherwise, the bee stays at its current food source
+    - if the bee has stayed for (NE * D) cycles (NE = number of employers, D = dimension of the function, 3 in our example), abandon the food source
+        - if the bee is an employer, go to a new random food source
+        - if the bee is an onlooker, go to a food source neighboring a well-performing bee
+
+We can access the colony's average fitness score, average fitness function return value, best fitness score, best fitness function return value and best parameters at any time:
+
+```python
+print(abc.average_fitness)
+print(abc.average_ret_val)
+print(abc.best_fitness)
+print(abc.best_ret_val)
+print(abc.best_params)
+```
+
+ECabc can utilize multiple CPU cores for concurrent processing:
+
+```python
+abc = ABC(10, minimize_integers, num_processes=8)
+```
+
+Tying everything together, we have:
+
+```python
+from ecabc import ABC
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+abc = ABC(10, minimize_integers)
+abc.add_param(0, 10, name='Int_1')
+abc.add_param(0, 10, name='Int_2')
+abc.add_param(0, 10, name='Int_3')
+abc.initialize()
+for _ in range(10):
+    abc.search()
+    print('Average fitness: {}'.format(abc.average_fitness))
+    print('Average obj. fn. return value: {}'.format(abc.average_ret_val))
+    print('Best fitness score: {}'.format(abc.best_fitness))
+    print('Best obj. fn. return value: {}'.format(abc.best_ret_val))
+    print('Best parameters: {}\n'.format(abc.best_params))
+```
+
+Running this script produces:
+
+```
+Average fitness: 0.08244866244866243
+Average obj. fn. return value: 11.65
+Best fitness score: 0.125
+Best obj. fn. return value: 7
+Best parameters: {'Int_1': 4, 'Int_2': 3, 'Int_3': 0}
+
+Average fitness: 0.0885855117105117
+Average obj. fn. return value: 10.8
+Best fitness score: 0.125
+Best obj. fn. return value: 7
+Best parameters: {'Int_1': 4, 'Int_2': 3, 'Int_3': 0}
+
+Average fitness: 0.10361832611832611
+Average obj. fn. return value: 9.4
+Best fitness score: 0.16666666666666666
+Best obj. fn. return value: 5
+Best parameters: {'Int_1': 2, 'Int_2': 3, 'Int_3': 0}
+
+Average fitness: 0.11173502151443326
+Average obj. fn. return value: 8.8
+Best fitness score: 0.2
+Best obj. fn. return value: 4
+Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 4}
+
+Average fitness: 0.12448879551820731
+Average obj. fn. return value: 7.95
+Best fitness score: 0.2
+Best obj. fn. return value: 4
+Best parameters: {'Int_1': 1, 'Int_2': 3, 'Int_3': 0}
+
+Average fitness: 0.1767694805194805
+Average obj. fn. return value: 6.7
+Best fitness score: 1.0
+Best obj. fn. return value: 0
+Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
+
+Average fitness: 0.183255772005772
+Average obj. fn. return value: 6.3
+Best fitness score: 1.0
+Best obj. fn. return value: 0
+Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
+
+Average fitness: 0.20172799422799423
+Average obj. fn. return value: 5.65
+Best fitness score: 1.0
+Best obj. fn. return value: 0
+Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
+
+Average fitness: 0.23827561327561328
+Average obj. fn. return value: 4.95
+Best fitness score: 1.0
+Best obj. fn. return value: 0
+Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
+
+Average fitness: 0.28456349206349213
+Average obj. fn. return value: 4.35
+Best fitness score: 1.0
+Best obj. fn. return value: 0
+Best parameters: {'Int_1': 0, 'Int_2': 0, 'Int_3': 0}
+```
+
+To run this script yourself, head over to our [examples](https://github.com/ecrl/ecabc/tree/master/examples) directory.
+
+# Contributing, Reporting Issues and Other Support:
+
+To contribute to ECabc, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
+
+To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
+
+For additional support/questions, contact Sanskriti Sharma (Sanskriti_Sharma@student.uml.edu), Hernan Gelaf-Romer (Hernan_Gelafromer@student.uml.edu), or Travis Kessler (Travis_Kessler@student.uml.edu).
```

### Comparing `ecabc-3.0.0/ecabc/abc.py` & `ecabc-3.0.1/ecabc/abc.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,315 +1,315 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-#  ecabc/abc.py
-#  v.3.0.0
-#
-#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
-#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
-#  <Travis_Kessler@student.uml.edu>
-#
-#  abc.py: contains ABC object, handling the initialization and runtime of the
-#  artificial bee colony
-#
-
-# Stdlib. imports
-from multiprocessing import Pool
-from random import randint
-from typing import Callable, Any, Union
-from warnings import warn
-
-# ECabc imports
-from ecabc.bee import Bee
-from ecabc.parameter import Parameter
-from ecabc.utils import apply_mutation, call_obj_fn, choose_bee,\
-    determine_best_bee
-
-
-class ABC:
-
-    def __init__(self, num_employers: int,
-                 objective_fn: Callable[[list], float], obj_fn_args: dict = {},
-                 num_processes: int = 1):
-        ''' ABC object: optimizes parameters for user-supplied function
-
-        Args:
-            num_employers (int): number of employer bees in the colony
-            objective_fn (callable): function to optimize; accepts list of
-                ints/floats, returns float (fitness)
-            obj_fn_args (dict): non-tunable kwargs to pass to objective_fn
-            num_processes (int): number of concurrent processes to utilize
-        '''
-
-        if not callable(objective_fn):
-            raise ReferenceError('Supplied objective function not callable')
-        self._obj_fn = objective_fn
-        self._obj_fn_args = obj_fn_args
-        self._num_employers = num_employers
-        self._num_processes = num_processes
-        self._params = []
-        self._bees = []
-
-    @property
-    def best_fitness(self) -> float:
-        ''' Returns fitness score from best-performing bee '''
-
-        return determine_best_bee(self._bees)[0]
-
-    @property
-    def best_ret_val(self) -> Union[int, float]:
-        ''' Returns objective_fn return value from best-performing bee '''
-
-        return determine_best_bee(self._bees)[1]
-
-    @property
-    def best_params(self) -> dict:
-        ''' Returns parameters from best-performing bee '''
-
-        vals = determine_best_bee(self._bees)[2]
-        ret_val = {}
-        for idx, param in enumerate(self._params):
-            if param._name is None:
-                ret_val['P{}'.format(idx)] = vals[idx]
-            else:
-                ret_val[param._name] = vals[idx]
-        return ret_val
-
-    @property
-    def average_fitness(self) -> float:
-        ''' Returns average fitness score for bee population '''
-
-        if len(self._bees) == 0:
-            return None
-        return (sum(b._fitness_score for b in self._bees) / len(self._bees))
-
-    @property
-    def average_ret_val(self) -> Union[int, float]:
-        ''' Returns average objective_fn return value for bee population '''
-
-        if len(self._bees) == 0:
-            return None
-        return (sum(b._obj_fn_val for b in self._bees) / len(self._bees))
-
-    def add_param(self, min_val: Union[int, float], max_val: Union[int, float],
-                  restrict: bool = True, name: str = None):
-        ''' ABC.add_param: adds a parameter to be processed by the user-
-        supplied objective function
-
-        Args:
-            min_val (int, float): minimum value allowed for the parameter's
-                initialization
-            max_val (int, float): maximum value allowed for the parameter's
-                initialization
-            restrict (bool): if `True`, parameter mutations must be within
-                [min_val, max_val], `False` allows out-of-bounds mutation
-            name (str): name of parameter, optional
-        '''
-
-        if len(self._bees) > 0:
-            raise RuntimeError(
-                'Cannot add another parameter after bee initialization'
-            )
-        self._params.append(Parameter(min_val, max_val, restrict, name))
-
-    def initialize(self):
-        ''' ABC.initialize: creates `num_employers` employer bees and
-        `num_employers` onlooker bees
-        '''
-
-        if len(self._bees) > 0:
-            warn('initialize() called again: overwriting bee population',
-                 RuntimeWarning)
-
-        self._bees = []
-
-        if self._num_processes > 1:
-            employer_pool = Pool(processes=self._num_processes)
-        employer_results = []
-
-        for _ in range(self._num_employers):
-
-            params = [p.rand_val for p in self._params]
-            if self._num_processes > 1:
-                employer_results.append(employer_pool.apply_async(
-                    call_obj_fn, [params, self._obj_fn, self._obj_fn_args]
-                ))
-            else:
-                employer_results.append(call_obj_fn(
-                    params, self._obj_fn, self._obj_fn_args
-                ))
-
-        if self._num_processes > 1:
-
-            employer_pool.close()
-            employer_pool.join()
-            employer_results = [r.get() for r in employer_results]
-
-        for result in employer_results:
-
-            self._bees.append(Bee(
-                result[0],
-                result[1],
-                len(self._params) * self._num_employers,
-                True
-            ))
-
-        if self._num_processes > 1:
-            onlooker_pool = Pool(processes=self._num_processes)
-        onlooker_results = []
-
-        for _ in range(self._num_employers):
-
-            chosen_employer = choose_bee(self._bees)
-            neighbor_food = apply_mutation(
-                chosen_employer._params, self._params
-            )
-
-            if self._num_processes > 1:
-                onlooker_results.append(onlooker_pool.apply_async(
-                    call_obj_fn,
-                    [neighbor_food, self._obj_fn, self._obj_fn_args]
-                ))
-            else:
-                onlooker_results.append(call_obj_fn(
-                    neighbor_food, self._obj_fn, self._obj_fn_args
-                ))
-
-        if self._num_processes > 1:
-
-            onlooker_pool.close()
-            onlooker_pool.join()
-            onlooker_results = [r.get() for r in onlooker_results]
-
-        for result in onlooker_results:
-
-            self._bees.append(Bee(
-                result[0],
-                result[1],
-                len(self._params) * self._num_employers,
-            ))
-
-    def search(self):
-        ''' ABC.search: performs one "search cycle" for all bees in the
-        colony; a search cycle consists of:
-
-        for all bees:
-            if bee has exhausted its current food source:
-                if bee is an employer, find a new random food source
-                if bee is an onlooker, travel to a food source near a well-
-                    performing bee's food source
-            if bee has not exhausted its current food source:
-                mutate one parameter value, move to food source if better;
-                    else, stay at current food source
-        bees = updated bee states
-
-        Exhaustion is defined as the maximum number of search cycles a bee is
-        allowed to stay at its current food source, given by EX = NE * D, where
-        NE is the number of employers and D is the dimensionality of the
-        problem (number of parameters)
-        '''
-
-        if len(self._bees) == 0:
-            raise RuntimeError('search() cannot be called before initialize()')
-
-        if self._num_processes > 1:
-            bee_pool = Pool(processes=self._num_processes)
-        new_employer_results = []
-        new_onlooker_results = []
-        new_position_results = []
-        current_positions = []
-
-        for bee in self._bees:
-
-            if bee.abandon:
-
-                if bee._is_employer:
-
-                    new_params = [p.rand_val for p in self._params]
-                    if self._num_processes > 1:
-                        new_employer_results.append(bee_pool.apply_async(
-                            call_obj_fn,
-                            [new_params, self._obj_fn, self._obj_fn_args]
-                        ))
-                    else:
-                        new_employer_results.append(call_obj_fn(
-                            new_params, self._obj_fn, self._obj_fn_args
-                        ))
-
-                else:
-
-                    chosen_bee = choose_bee(self._bees)
-                    neighbor_food = apply_mutation(
-                        chosen_bee._params, self._params
-                    )
-                    if self._num_processes > 1:
-                        new_onlooker_results.append(bee_pool.apply_async(
-                            call_obj_fn,
-                            [neighbor_food, self._obj_fn, self._obj_fn_args]
-                        ))
-                    else:
-                        new_onlooker_results.append(call_obj_fn(
-                            neighbor_food, self._obj_fn, self._obj_fn_args
-                        ))
-
-            else:
-
-                current_positions.append(bee)
-                neighbor_food = apply_mutation(bee._params, self._params)
-                if self._num_processes > 1:
-                    new_position_results.append(bee_pool.apply_async(
-                        call_obj_fn,
-                        [neighbor_food, self._obj_fn, self._obj_fn_args]
-                    ))
-                else:
-                    new_position_results.append(call_obj_fn(
-                        neighbor_food, self._obj_fn, self._obj_fn_args
-                    ))
-
-        if self._num_processes > 1:
-
-            bee_pool.close()
-            bee_pool.join()
-            new_employer_results = [r.get() for r in new_employer_results]
-            new_onlooker_results = [r.get() for r in new_onlooker_results]
-            new_position_results = [r.get() for r in new_position_results]
-
-        next_bee_generation = []
-
-        for result in new_employer_results:
-
-            next_bee_generation.append(Bee(
-                result[0],
-                result[1],
-                len(self._params) * self._num_employers,
-                True
-            ))
-
-        for result in new_onlooker_results:
-
-            next_bee_generation.append(Bee(
-                result[0],
-                result[1],
-                len(self._params) * self._num_employers
-            ))
-
-        for idx, result in enumerate(new_position_results):
-
-            bee_to_compare = current_positions[idx]
-            if bee_to_compare.is_better_food(result[1]):
-                if bee._is_employer:
-                    next_bee_generation.append(Bee(
-                        result[0],
-                        result[1],
-                        len(self._params) * self._num_employers,
-                        True
-                    ))
-                else:
-                    next_bee_generation.append(Bee(
-                        result[0],
-                        result[1],
-                        len(self._params) * self._num_employers
-                    ))
-            else:
-                next_bee_generation.append(bee_to_compare)
-
-        self._bees = next_bee_generation
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+#  ecabc/abc.py
+#  v.3.0.0
+#
+#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
+#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
+#  <Travis_Kessler@student.uml.edu>
+#
+#  abc.py: contains ABC object, handling the initialization and runtime of the
+#  artificial bee colony
+#
+
+# Stdlib. imports
+from multiprocessing import Pool
+from random import randint
+from typing import Callable, Any, Union
+from warnings import warn
+
+# ECabc imports
+from ecabc.bee import Bee
+from ecabc.parameter import Parameter
+from ecabc.utils import apply_mutation, call_obj_fn, choose_bee,\
+    determine_best_bee
+
+
+class ABC:
+
+    def __init__(self, num_employers: int,
+                 objective_fn: Callable[[list], float], obj_fn_args: dict = {},
+                 num_processes: int = 1):
+        ''' ABC object: optimizes parameters for user-supplied function
+
+        Args:
+            num_employers (int): number of employer bees in the colony
+            objective_fn (callable): function to optimize; accepts list of
+                ints/floats, returns float (fitness)
+            obj_fn_args (dict): non-tunable kwargs to pass to objective_fn
+            num_processes (int): number of concurrent processes to utilize
+        '''
+
+        if not callable(objective_fn):
+            raise ReferenceError('Supplied objective function not callable')
+        self._obj_fn = objective_fn
+        self._obj_fn_args = obj_fn_args
+        self._num_employers = num_employers
+        self._num_processes = num_processes
+        self._params = []
+        self._bees = []
+
+    @property
+    def best_fitness(self) -> float:
+        ''' Returns fitness score from best-performing bee '''
+
+        return determine_best_bee(self._bees)[0]
+
+    @property
+    def best_ret_val(self) -> Union[int, float]:
+        ''' Returns objective_fn return value from best-performing bee '''
+
+        return determine_best_bee(self._bees)[1]
+
+    @property
+    def best_params(self) -> dict:
+        ''' Returns parameters from best-performing bee '''
+
+        vals = determine_best_bee(self._bees)[2]
+        ret_val = {}
+        for idx, param in enumerate(self._params):
+            if param._name is None:
+                ret_val['P{}'.format(idx)] = vals[idx]
+            else:
+                ret_val[param._name] = vals[idx]
+        return ret_val
+
+    @property
+    def average_fitness(self) -> float:
+        ''' Returns average fitness score for bee population '''
+
+        if len(self._bees) == 0:
+            return None
+        return (sum(b._fitness_score for b in self._bees) / len(self._bees))
+
+    @property
+    def average_ret_val(self) -> Union[int, float]:
+        ''' Returns average objective_fn return value for bee population '''
+
+        if len(self._bees) == 0:
+            return None
+        return (sum(b._obj_fn_val for b in self._bees) / len(self._bees))
+
+    def add_param(self, min_val: Union[int, float], max_val: Union[int, float],
+                  restrict: bool = True, name: str = None):
+        ''' ABC.add_param: adds a parameter to be processed by the user-
+        supplied objective function
+
+        Args:
+            min_val (int, float): minimum value allowed for the parameter's
+                initialization
+            max_val (int, float): maximum value allowed for the parameter's
+                initialization
+            restrict (bool): if `True`, parameter mutations must be within
+                [min_val, max_val], `False` allows out-of-bounds mutation
+            name (str): name of parameter, optional
+        '''
+
+        if len(self._bees) > 0:
+            raise RuntimeError(
+                'Cannot add another parameter after bee initialization'
+            )
+        self._params.append(Parameter(min_val, max_val, restrict, name))
+
+    def initialize(self):
+        ''' ABC.initialize: creates `num_employers` employer bees and
+        `num_employers` onlooker bees
+        '''
+
+        if len(self._bees) > 0:
+            warn('initialize() called again: overwriting bee population',
+                 RuntimeWarning)
+
+        self._bees = []
+
+        if self._num_processes > 1:
+            employer_pool = Pool(processes=self._num_processes)
+        employer_results = []
+
+        for _ in range(self._num_employers):
+
+            params = [p.rand_val for p in self._params]
+            if self._num_processes > 1:
+                employer_results.append(employer_pool.apply_async(
+                    call_obj_fn, [params, self._obj_fn, self._obj_fn_args]
+                ))
+            else:
+                employer_results.append(call_obj_fn(
+                    params, self._obj_fn, self._obj_fn_args
+                ))
+
+        if self._num_processes > 1:
+
+            employer_pool.close()
+            employer_pool.join()
+            employer_results = [r.get() for r in employer_results]
+
+        for result in employer_results:
+
+            self._bees.append(Bee(
+                result[0],
+                result[1],
+                len(self._params) * self._num_employers,
+                True
+            ))
+
+        if self._num_processes > 1:
+            onlooker_pool = Pool(processes=self._num_processes)
+        onlooker_results = []
+
+        for _ in range(self._num_employers):
+
+            chosen_employer = choose_bee(self._bees)
+            neighbor_food = apply_mutation(
+                chosen_employer._params, self._params
+            )
+
+            if self._num_processes > 1:
+                onlooker_results.append(onlooker_pool.apply_async(
+                    call_obj_fn,
+                    [neighbor_food, self._obj_fn, self._obj_fn_args]
+                ))
+            else:
+                onlooker_results.append(call_obj_fn(
+                    neighbor_food, self._obj_fn, self._obj_fn_args
+                ))
+
+        if self._num_processes > 1:
+
+            onlooker_pool.close()
+            onlooker_pool.join()
+            onlooker_results = [r.get() for r in onlooker_results]
+
+        for result in onlooker_results:
+
+            self._bees.append(Bee(
+                result[0],
+                result[1],
+                len(self._params) * self._num_employers,
+            ))
+
+    def search(self):
+        ''' ABC.search: performs one "search cycle" for all bees in the
+        colony; a search cycle consists of:
+
+        for all bees:
+            if bee has exhausted its current food source:
+                if bee is an employer, find a new random food source
+                if bee is an onlooker, travel to a food source near a well-
+                    performing bee's food source
+            if bee has not exhausted its current food source:
+                mutate one parameter value, move to food source if better;
+                    else, stay at current food source
+        bees = updated bee states
+
+        Exhaustion is defined as the maximum number of search cycles a bee is
+        allowed to stay at its current food source, given by EX = NE * D, where
+        NE is the number of employers and D is the dimensionality of the
+        problem (number of parameters)
+        '''
+
+        if len(self._bees) == 0:
+            raise RuntimeError('search() cannot be called before initialize()')
+
+        if self._num_processes > 1:
+            bee_pool = Pool(processes=self._num_processes)
+        new_employer_results = []
+        new_onlooker_results = []
+        new_position_results = []
+        current_positions = []
+
+        for bee in self._bees:
+
+            if bee.abandon:
+
+                if bee._is_employer:
+
+                    new_params = [p.rand_val for p in self._params]
+                    if self._num_processes > 1:
+                        new_employer_results.append(bee_pool.apply_async(
+                            call_obj_fn,
+                            [new_params, self._obj_fn, self._obj_fn_args]
+                        ))
+                    else:
+                        new_employer_results.append(call_obj_fn(
+                            new_params, self._obj_fn, self._obj_fn_args
+                        ))
+
+                else:
+
+                    chosen_bee = choose_bee(self._bees)
+                    neighbor_food = apply_mutation(
+                        chosen_bee._params, self._params
+                    )
+                    if self._num_processes > 1:
+                        new_onlooker_results.append(bee_pool.apply_async(
+                            call_obj_fn,
+                            [neighbor_food, self._obj_fn, self._obj_fn_args]
+                        ))
+                    else:
+                        new_onlooker_results.append(call_obj_fn(
+                            neighbor_food, self._obj_fn, self._obj_fn_args
+                        ))
+
+            else:
+
+                current_positions.append(bee)
+                neighbor_food = apply_mutation(bee._params, self._params)
+                if self._num_processes > 1:
+                    new_position_results.append(bee_pool.apply_async(
+                        call_obj_fn,
+                        [neighbor_food, self._obj_fn, self._obj_fn_args]
+                    ))
+                else:
+                    new_position_results.append(call_obj_fn(
+                        neighbor_food, self._obj_fn, self._obj_fn_args
+                    ))
+
+        if self._num_processes > 1:
+
+            bee_pool.close()
+            bee_pool.join()
+            new_employer_results = [r.get() for r in new_employer_results]
+            new_onlooker_results = [r.get() for r in new_onlooker_results]
+            new_position_results = [r.get() for r in new_position_results]
+
+        next_bee_generation = []
+
+        for result in new_employer_results:
+
+            next_bee_generation.append(Bee(
+                result[0],
+                result[1],
+                len(self._params) * self._num_employers,
+                True
+            ))
+
+        for result in new_onlooker_results:
+
+            next_bee_generation.append(Bee(
+                result[0],
+                result[1],
+                len(self._params) * self._num_employers
+            ))
+
+        for idx, result in enumerate(new_position_results):
+
+            bee_to_compare = current_positions[idx]
+            if bee_to_compare.is_better_food(result[1]):
+                if bee._is_employer:
+                    next_bee_generation.append(Bee(
+                        result[0],
+                        result[1],
+                        len(self._params) * self._num_employers,
+                        True
+                    ))
+                else:
+                    next_bee_generation.append(Bee(
+                        result[0],
+                        result[1],
+                        len(self._params) * self._num_employers
+                    ))
+            else:
+                next_bee_generation.append(bee_to_compare)
+
+        self._bees = next_bee_generation
```

### Comparing `ecabc-3.0.0/ecabc/bee.py` & `ecabc-3.0.1/ecabc/bee.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-#  ecabc/bee.py
-#  v.3.0.0
-#
-#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
-#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
-#  <Travis_Kessler@student.uml.edu>
-#
-#  bee.py: contains Bee object, which houses information relevant to a
-#  specific solution being investigated by an individual bee
-#
-
-# Stdlib. imports
-from typing import Union
-
-
-class Bee:
-
-    def __init__(self, params: list, obj_fn_val: Union[int, float],
-                 stay_limit: int, is_employer: bool = False):
-        ''' Bee object: houses bee-specific information such as its current
-        set of parameters, the objective function value resulting from its,
-        current parameters, maximum number of cycles it can stay at its
-        current food source, and whether it is an employer bee or not
-
-        Args:
-            params (list): list of current set of parameters, int or float
-            obj_fn_val (int, float): value returned by objective function when
-                supplied parameters are supplied
-            stay_limit (int): maximum number of cycles the bee can stay at its
-                current food source
-            is_employer (bool): `True` if employer, `False` if onlooker
-        '''
-
-        self._params = params
-        self._obj_fn_val = obj_fn_val
-        self._fitness_score = self.calc_fitness(obj_fn_val)
-        self._stay_limit = stay_limit
-        self._stay_count = 0
-        self._is_employer = is_employer
-
-    @property
-    def abandon(self) -> bool:
-        ''' When called, increment how many times the bee has stayed at its
-        current food source; if reached stay limit, return `True` else `False`
-        '''
-
-        self._stay_count += 1
-        if self._stay_count >= self._stay_limit:
-            return True
-        else:
-            return False
-
-    @staticmethod
-    def calc_fitness(obj_fn_val: Union[int, float]) -> float:
-        ''' Static method: Bee.calc_fitness: Calculates fitness score based on
-        objective function value, using the equation:
-
-        fitness = 1 / (1 + ofv)     if ofv >= 0
-        fitness = 1 + abs(ofv)      if ofv < 0
-
-        Where ofv is the objective function value and fitness is the resulting
-        fitness score
-
-        Args:
-            obj_fn_val (int, float): value obtained from objective function
-
-        Returns:
-            float: resulting fitness score
-        '''
-
-        if obj_fn_val >= 0:
-            return 1 / (obj_fn_val + 1)
-        else:
-            return 1 + abs(obj_fn_val)
-
-    def is_better_food(self, obj_fn_val: Union[int, float]) -> bool:
-        ''' Bee.is_better_food: determines if objective function value
-        resulting from a new food source is better than the bee's current food
-        source
-
-        Args:
-            obj_fn_val (int, float): value resulting from objective function
-                with new food
-
-        Returns:
-            bool: `True` if better food source else `False`
-        '''
-
-        if self.calc_fitness(obj_fn_val) > self._fitness_score:
-            return True
-        else:
-            return False
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+#  ecabc/bee.py
+#  v.3.0.0
+#
+#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
+#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
+#  <Travis_Kessler@student.uml.edu>
+#
+#  bee.py: contains Bee object, which houses information relevant to a
+#  specific solution being investigated by an individual bee
+#
+
+# Stdlib. imports
+from typing import Union
+
+
+class Bee:
+
+    def __init__(self, params: list, obj_fn_val: Union[int, float],
+                 stay_limit: int, is_employer: bool = False):
+        ''' Bee object: houses bee-specific information such as its current
+        set of parameters, the objective function value resulting from its,
+        current parameters, maximum number of cycles it can stay at its
+        current food source, and whether it is an employer bee or not
+
+        Args:
+            params (list): list of current set of parameters, int or float
+            obj_fn_val (int, float): value returned by objective function when
+                supplied parameters are supplied
+            stay_limit (int): maximum number of cycles the bee can stay at its
+                current food source
+            is_employer (bool): `True` if employer, `False` if onlooker
+        '''
+
+        self._params = params
+        self._obj_fn_val = obj_fn_val
+        self._fitness_score = self.calc_fitness(obj_fn_val)
+        self._stay_limit = stay_limit
+        self._stay_count = 0
+        self._is_employer = is_employer
+
+    @property
+    def abandon(self) -> bool:
+        ''' When called, increment how many times the bee has stayed at its
+        current food source; if reached stay limit, return `True` else `False`
+        '''
+
+        self._stay_count += 1
+        if self._stay_count >= self._stay_limit:
+            return True
+        else:
+            return False
+
+    @staticmethod
+    def calc_fitness(obj_fn_val: Union[int, float]) -> float:
+        ''' Static method: Bee.calc_fitness: Calculates fitness score based on
+        objective function value, using the equation:
+
+        fitness = 1 / (1 + ofv)     if ofv >= 0
+        fitness = 1 + abs(ofv)      if ofv < 0
+
+        Where ofv is the objective function value and fitness is the resulting
+        fitness score
+
+        Args:
+            obj_fn_val (int, float): value obtained from objective function
+
+        Returns:
+            float: resulting fitness score
+        '''
+
+        if obj_fn_val >= 0:
+            return 1 / (obj_fn_val + 1)
+        else:
+            return 1 + abs(obj_fn_val)
+
+    def is_better_food(self, obj_fn_val: Union[int, float]) -> bool:
+        ''' Bee.is_better_food: determines if objective function value
+        resulting from a new food source is better than the bee's current food
+        source
+
+        Args:
+            obj_fn_val (int, float): value resulting from objective function
+                with new food
+
+        Returns:
+            bool: `True` if better food source else `False`
+        '''
+
+        if self.calc_fitness(obj_fn_val) > self._fitness_score:
+            return True
+        else:
+            return False
```

### Comparing `ecabc-3.0.0/ecabc/parameter.py` & `ecabc-3.0.1/ecabc/parameter.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-#  ecabc/parameter.py
-#  v.3.0.0
-#
-#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
-#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
-#  <Travis_Kessler@student.uml.edu>
-#
-#  parameter.py: contains Parameter object, defining the search space for an
-#  individual function variable
-#
-
-# Stdlib. imports
-from random import uniform
-from typing import Union
-
-
-class Parameter:
-
-    def __init__(self, min_val: Union[int, float], max_val: Union[int, float],
-                 restrict: bool = True, name: str = None):
-        ''' Parameter object: houses information about a user-supplied
-        parameter including data type, minimum/maximum initialization values,
-        and whether the parameter is limited to [min_val, max_val] when
-        mutating
-
-        Args:
-            min_val (int, float): minimum value allowed for the parameter's
-                initialization
-            max_val (int, float): maximum value allowed for the parameter's
-                initialization
-            restrict (bool): if `True`, parameter mutations must be within
-                [min_val, max_val]
-            name (str): name of parameter, optional
-        '''
-
-        if type(min_val) != type(max_val):
-            raise ValueError('Supplied min_val is not the same type is '
-                             'supplied max_val: {}, {}'.format(
-                                 type(min_val), type(max_val)
-                             ))
-
-        self._dtype = type(min_val + max_val)
-        if self._dtype not in [int, float]:
-            raise ValueError('Unsupported data type for Parameter: use {}'
-                             .format([int, float]))
-
-        self._min_val = min_val
-        self._max_val = max_val
-        self._restrict = restrict
-        self._name = name
-
-    @property
-    def rand_val(self) -> Union[int, float]:
-        ''' Returns a random value X in range [min_val, max_val] using the
-        equation:
-
-        X = min_val + rand(0, 1) * (max_val - min_val)
-        '''
-
-        return self._dtype(self._min_val + uniform(0, 1) *
-                           (self._max_val - self._min_val))
-
-    def mutate(self, curr_value: Union[int, float]) -> Union[int, float]:
-        ''' Parameter.mutate: mutates current parameter value by using the
-        equation:
-
-        V = X + rand(-1, 1) * (X - Xrand)
-
-        Where V is the new value, X is the current value and Xrand is a random
-        parameter value
-
-        Args:
-            curr_value (int, float): current parameter value
-
-        Returns:
-            int, float: mutated parameter value
-        '''
-
-        new_value = self._dtype(
-            curr_value + uniform(-1, 1) * (curr_value - self.rand_val)
-        )
-
-        if self._restrict:
-            if new_value > self._max_val:
-                new_value = self._max_val
-            elif new_value < self._min_val:
-                new_value = self._min_val
-
-        if new_value == curr_value:
-            if self._dtype is int and self._max_val - self._min_val <= 2:
-                pass
-            else:
-                return self.mutate(curr_value)
-
-        return new_value
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+#  ecabc/parameter.py
+#  v.3.0.0
+#
+#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
+#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
+#  <Travis_Kessler@student.uml.edu>
+#
+#  parameter.py: contains Parameter object, defining the search space for an
+#  individual function variable
+#
+
+# Stdlib. imports
+from random import uniform
+from typing import Union
+
+
+class Parameter:
+
+    def __init__(self, min_val: Union[int, float], max_val: Union[int, float],
+                 restrict: bool = True, name: str = None):
+        ''' Parameter object: houses information about a user-supplied
+        parameter including data type, minimum/maximum initialization values,
+        and whether the parameter is limited to [min_val, max_val] when
+        mutating
+
+        Args:
+            min_val (int, float): minimum value allowed for the parameter's
+                initialization
+            max_val (int, float): maximum value allowed for the parameter's
+                initialization
+            restrict (bool): if `True`, parameter mutations must be within
+                [min_val, max_val]
+            name (str): name of parameter, optional
+        '''
+
+        if type(min_val) != type(max_val):
+            raise ValueError('Supplied min_val is not the same type is '
+                             'supplied max_val: {}, {}'.format(
+                                 type(min_val), type(max_val)
+                             ))
+
+        self._dtype = type(min_val + max_val)
+        if self._dtype not in [int, float]:
+            raise ValueError('Unsupported data type for Parameter: use {}'
+                             .format([int, float]))
+
+        self._min_val = min_val
+        self._max_val = max_val
+        self._restrict = restrict
+        self._name = name
+
+    @property
+    def rand_val(self) -> Union[int, float]:
+        ''' Returns a random value X in range [min_val, max_val] using the
+        equation:
+
+        X = min_val + rand(0, 1) * (max_val - min_val)
+        '''
+
+        return self._dtype(self._min_val + uniform(0, 1) *
+                           (self._max_val - self._min_val))
+
+    def mutate(self, curr_value: Union[int, float]) -> Union[int, float]:
+        ''' Parameter.mutate: mutates current parameter value by using the
+        equation:
+
+        V = X + rand(-1, 1) * (X - Xrand)
+
+        Where V is the new value, X is the current value and Xrand is a random
+        parameter value
+
+        Args:
+            curr_value (int, float): current parameter value
+
+        Returns:
+            int, float: mutated parameter value
+        '''
+
+        new_value = self._dtype(
+            curr_value + uniform(-1, 1) * (curr_value - self.rand_val)
+        )
+
+        if self._restrict:
+            if new_value > self._max_val:
+                new_value = self._max_val
+            elif new_value < self._min_val:
+                new_value = self._min_val
+
+        if new_value == curr_value:
+            if self._dtype is int and self._max_val - self._min_val <= 2:
+                pass
+            else:
+                return self.mutate(curr_value)
+
+        return new_value
```

### Comparing `ecabc-3.0.0/ecabc/utils.py` & `ecabc-3.0.1/ecabc/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-#  ecabc/utils.py
-#  v.3.0.0
-#
-#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
-#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
-#  <Travis_Kessler@student.uml.edu>
-#
-#  utils.py: contains various utility functions used by the artificial bee
-#  colony
-#
-
-# Stdlib. imports
-from bisect import bisect
-from random import randint, random
-
-
-def apply_mutation(curr_params: list, all_params: list) -> list:
-    ''' apply_mutation: alters the value of one parameter in supplied list of
-    values
-
-    Args:
-        curr_params (list): current parameter values, ints or floats
-        all_params (list): list of Parameter objects
-
-    Returns:
-        list: parameter values with one value mutation
-    '''
-
-    to_change = randint(0, len(curr_params) - 1)
-    new_params = curr_params[:]
-    new_params[to_change] = all_params[to_change].mutate(new_params[to_change])
-    return new_params
-
-
-def call_obj_fn(params: list, obj_fn: callable, obj_fn_args: dict) -> tuple:
-    ''' call_obj_fn: calls supplied objective function, evaluating using
-    supplied parameters; callable in single- and multi-processed configurations
-
-    Args:
-        params (list): list of ints or floats corresponding to current bee
-            parameter values
-        obj_fn (callable): function to accept list of paramters, returns a
-            quantitative measurement of fitness
-        obj_fn_args (dict): non-tunable kwargs to pass to objective function
-
-    Returns:
-        tuple: (params, objective function return value)
-    '''
-
-    return (params, obj_fn(params, **obj_fn_args))
-
-
-def choose_bee(bees: list) -> 'Bee':
-    ''' choose_bee: choose a bee based on probabilities a given bee will be
-    chosen; probabilities based on fitness score (higher fitness score ==
-    higher probability of being chosen)
-
-    Args:
-        bees (list): list of Bee objects
-
-    Returns:
-        Bee: chosen Bee
-    '''
-
-    fitness_sum = sum(b._fitness_score for b in bees)
-    probabilities = [b._fitness_score / fitness_sum for b in bees]
-    cdf_vals = []
-    cumsum = 0
-    for p in probabilities:
-        cumsum += p
-        cdf_vals.append(cumsum)
-    idx = bisect(cdf_vals, random())
-    return bees[idx]
-
-
-def determine_best_bee(bees: list) -> tuple:
-    ''' determine_best_bee: return highest fitness score w/ corresponding
-    objective function return value and parameters given a list of bees
-
-    Args:
-        bees (list): list of Bee objects
-
-    Returns:
-        tuple: (best fitness score, best return value, best parameters)
-    '''
-
-    best_fitness = 0
-    best_ret_val = None
-    best_params = None
-    for bee in bees:
-        if bee._fitness_score > best_fitness:
-            best_fitness = bee._fitness_score
-            best_ret_val = bee._obj_fn_val
-            best_params = bee._params
-    return (best_fitness, best_ret_val, best_params)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+#  ecabc/utils.py
+#  v.3.0.0
+#
+#  Developed in 2019 by Sanskriti Sharma <sanskriti_sharma@student.uml.edu>,
+#  Hernan Gelaf-Romer <hernan_gelafromer@student.uml.edu>, and Travis Kessler
+#  <Travis_Kessler@student.uml.edu>
+#
+#  utils.py: contains various utility functions used by the artificial bee
+#  colony
+#
+
+# Stdlib. imports
+from bisect import bisect
+from random import randint, random
+
+
+def apply_mutation(curr_params: list, all_params: list) -> list:
+    ''' apply_mutation: alters the value of one parameter in supplied list of
+    values
+
+    Args:
+        curr_params (list): current parameter values, ints or floats
+        all_params (list): list of Parameter objects
+
+    Returns:
+        list: parameter values with one value mutation
+    '''
+
+    to_change = randint(0, len(curr_params) - 1)
+    new_params = curr_params[:]
+    new_params[to_change] = all_params[to_change].mutate(new_params[to_change])
+    return new_params
+
+
+def call_obj_fn(params: list, obj_fn: callable, obj_fn_args: dict) -> tuple:
+    ''' call_obj_fn: calls supplied objective function, evaluating using
+    supplied parameters; callable in single- and multi-processed configurations
+
+    Args:
+        params (list): list of ints or floats corresponding to current bee
+            parameter values
+        obj_fn (callable): function to accept list of paramters, returns a
+            quantitative measurement of fitness
+        obj_fn_args (dict): non-tunable kwargs to pass to objective function
+
+    Returns:
+        tuple: (params, objective function return value)
+    '''
+
+    return (params, obj_fn(params, **obj_fn_args))
+
+
+def choose_bee(bees: list) -> 'Bee':
+    ''' choose_bee: choose a bee based on probabilities a given bee will be
+    chosen; probabilities based on fitness score (higher fitness score ==
+    higher probability of being chosen)
+
+    Args:
+        bees (list): list of Bee objects
+
+    Returns:
+        Bee: chosen Bee
+    '''
+
+    fitness_sum = sum(b._fitness_score for b in bees)
+    probabilities = [b._fitness_score / fitness_sum for b in bees]
+    cdf_vals = []
+    cumsum = 0
+    for p in probabilities:
+        cumsum += p
+        cdf_vals.append(cumsum)
+    idx = bisect(cdf_vals, random())
+    return bees[idx]
+
+
+def determine_best_bee(bees: list) -> tuple:
+    ''' determine_best_bee: return highest fitness score w/ corresponding
+    objective function return value and parameters given a list of bees
+
+    Args:
+        bees (list): list of Bee objects
+
+    Returns:
+        tuple: (best fitness score, best return value, best parameters)
+    '''
+
+    best_fitness = 0
+    best_ret_val = None
+    best_params = None
+    for bee in bees:
+        if bee._fitness_score > best_fitness:
+            best_fitness = bee._fitness_score
+            best_ret_val = bee._obj_fn_val
+            best_params = bee._params
+    return (best_fitness, best_ret_val, best_params)
```

