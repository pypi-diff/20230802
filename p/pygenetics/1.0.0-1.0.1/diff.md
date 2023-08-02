# Comparing `tmp/pygenetics-1.0.0.tar.gz` & `tmp/pygenetics-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygenetics-1.0.0.tar", last modified: Sat Aug  3 16:54:46 2019, max compression
+gzip compressed data, was "pygenetics-1.0.1.tar", last modified: Wed Aug  2 21:19:19 2023, max compression
```

## Comparing `pygenetics-1.0.0.tar` & `pygenetics-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2019-08-03 16:54:46.000000 pygenetics-1.0.0/
--rw-rw-rw-   0        0        0      314 2019-08-03 16:54:46.000000 pygenetics-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9089 2019-08-03 16:53:27.000000 pygenetics-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics/
--rw-rw-rw-   0        0        0      176 2019-08-03 16:53:27.000000 pygenetics-1.0.0/pygenetics/__init__.py
--rw-rw-rw-   0        0        0     1621 2019-08-03 16:53:27.000000 pygenetics-1.0.0/pygenetics/member.py
--rw-rw-rw-   0        0        0     3007 2019-08-03 16:53:27.000000 pygenetics-1.0.0/pygenetics/parameter.py
--rw-rw-rw-   0        0        0     8498 2019-08-03 16:53:27.000000 pygenetics-1.0.0/pygenetics/population.py
--rw-rw-rw-   0        0        0     3765 2019-08-03 16:53:27.000000 pygenetics-1.0.0/pygenetics/utils.py
-drwxrwxrwx   0        0        0        0 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics.egg-info/
--rw-rw-rw-   0        0        0      314 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2019-08-03 16:54:46.000000 pygenetics-1.0.0/pygenetics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2019-08-03 16:54:46.000000 pygenetics-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      429 2019-08-03 16:53:27.000000 pygenetics-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:19:19.338805 pygenetics-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 21:19:08.000000 pygenetics-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-08-02 21:19:19.338805 pygenetics-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-08-02 21:19:08.000000 pygenetics-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:19:19.338805 pygenetics-1.0.1/pygenetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 21:19:08.000000 pygenetics-1.0.1/pygenetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-02 21:19:08.000000 pygenetics-1.0.1/pygenetics/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-02 21:19:08.000000 pygenetics-1.0.1/pygenetics/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-08-02 21:19:08.000000 pygenetics-1.0.1/pygenetics/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-08-02 21:19:08.000000 pygenetics-1.0.1/pygenetics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:19:19.338805 pygenetics-1.0.1/pygenetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-08-02 21:19:19.000000 pygenetics-1.0.1/pygenetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-02 21:19:19.000000 pygenetics-1.0.1/pygenetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:19:19.000000 pygenetics-1.0.1/pygenetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 21:19:19.000000 pygenetics-1.0.1/pygenetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 21:19:08.000000 pygenetics-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:19:19.338805 pygenetics-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:19:19.338805 pygenetics-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-02 21:19:08.000000 pygenetics-1.0.1/tests/test_all.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pygenetics-1.0.0/README.md` & `pygenetics-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,253 +1,241 @@
-# PyGenetics: Genetic Algorithm for Tuning Function Parameters
-
-[![GitHub version](https://badge.fury.io/gh/tjkessler%2FPyGenetics.svg)](https://badge.fury.io/gh/tjkessler%2FPyGenetics)
-[![PyPI version](https://badge.fury.io/py/pygenetics.svg)](https://badge.fury.io/py/pygenetics)
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/TJKessler/PyGenetics/master/LICENSE.txt)
-[![Build Status](https://dev.azure.com/travisjkessler/personal-repos/_apis/build/status/tjkessler.PyGenetics?branchName=master)](https://dev.azure.com/travisjkessler/personal-repos/_build/latest?definitionId=7&branchName=master)
-
-PyGenetics is an open source Python package used to tune parameters for user-supplied functions. Inspired by [genetic algorithms](https://www.researchgate.net/profile/Darrell_Whitley2/publication/2425017_A_Genetic_Algorithm_Tutorial/links/563214a108ae506cea68fd96/A-Genetic-Algorithm-Tutorial.pdf), PyGenetics is able to optimize variables in a multidimensional search space to minimize a "cost" (e.g. an error value returned by the user-supplied function).
-
-<p align="center">
-  <img align="center" src="docs/img/demo.gif" width="75%" height="75%">
-</p>
-
-# Installation:
-
-### Prerequisites:
-- Have Python 3.X installed
-- Have the ability to install Python packages
-
-### Method 1: pip
-If you are working in a Linux/Mac environment:
-```
-sudo pip install pygenetics
-```
-
-Alternatively, in a Windows or virtualenv environment:
-```
-pip install pygenetics
-```
-
-To update your version of PyGenetics to the latest version, use:
-```
-pip install --upgrade pygenetics
-```
-
-Note: if multiple Python releases are installed on your system (e.g. 2.7 and 3.7), you may need to execute the correct version of pip. For Python 3.7, change **"pip install pygenetics"** to **"pip3 install pygenetics"**.
-
-### Method 2: From source
-Download the PyGenetics repository, navigate to the download location on the command line/terminal, and execute:
-```
-python setup.py install
-```
-
-There are currently no additional dependencies for PyGenetics.
-
-# Usage:
-
-To start using PyGenetics, you need a couple items:
-- a cost function (objective function) to optimize
-- parameters used by the cost function
-
-For example, let's define a cost function to minimize the sum of three integers:
-
-```python
-def minimize_integers(integers):
-
-    return sum(integers)
-
-```
-
-Your cost function must accept a **list** from PyGenetics. The list values represent the current solution, i.e. parameter values, being evaluated by a population member
-
-Now that we have our cost function, let's import the Population object from PyGenetics, initialize the population, and add our parameters/genes:
-
-```python
-from pygenetics import Population
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-pop = Population(10, minimize_integers)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-```
-
-Here we initialize the population with 10 population members, supply our cost function and add our parameters/genes. Parameters are added with minimum/maximum values for its search space. By default, parameter mutations (searching a neighboring solution) will not exceed the specified parameter bounds [min_val, max_val]; if this limitation is not desired, supply the "restrict=False" argument:
-
-```python
-pop.add_param(0, 10, restrict=False)
-```
-
-Once we have created our population and added our parameters/genes, we then need to "initialize" the population's members:
-
-```python
-from pygenetics import Population
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-pop = Population(10, minimize_integers)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.initialize()
-```
-
-Initializing the population's members (in this example, 10 members) deploys them to random solutions/chromosomes (a random parameter/gene set is created), and their fitness is evaluated (in this example, lowest sum is better).
-
-We then compute a pre-determined number of generations, each derived from the previous generation's members:
-
-```python
-from pygenetics import Population
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-pop = Population(10, minimize_integers)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.initialize()
-for _ in range(10):
-    pop.next_generation()
-```
-
-Computing the next generation consists of:
-
-- **1.** Select a chromosome (parameter/gene set) from the population based on fitness (a higher fitness score results in a higher chance of being chosen)
-
-- **2a.** Perform crossover with probability _p<sub>c</sub>_ (default of 0.5, 50%); if crossover is not performed, perform step (2b)
-
-    - Select a different chromosome per method in (1)
-    - Select a crossover point between 1 and L-1 (random index in chromosomes' genes) with uniform probability
-    - Recombine chromosomes to form two offspring
-    - Perform mutation on each gene with probability _p<sub>m</sub>_ (default of 0.01, 1%)
-    - Place both offspring in the next generation
-    
-- **2b.** Crossover not performed, perform mutation on each gene of the chromosome with probability _p<sub>m</sub>_ (default of 0.01, 1%), place chromosome in the next generation
-
-- **3.** If the next generation is not full (less than total population size), continue from step (1)
-
-Both _p<sub>c</sub>_ and _p<sub>m</sub>_ can be adjusted when the next generation is created:
-
-```python
-pop.next_generation(p_crossover=0.75, p_mutation=0.05)
-```
-
-We can access the populations's average fitness score, average objective function return value, best fitness score, best objective function return value and best parameters at any time:
-
-```python
-print(pop.average_fitness)
-print(pop.average_ret_val)
-print(pop.best_fitness)
-print(pop.best_ret_val)
-print(pop.best_params)
-```
-
-PyGenetics can utilize multiple CPU cores for concurrent processing:
-
-```python
-pop = Population(10, minimize_integers, num_processes=8)
-```
-
-Tying everything together, we have:
-
-```python
-from pygenetics import Population
-
-def minimize_integers(integers):
-
-    return sum(integers)
-
-pop = Population(10, minimize_integers)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.add_param(0, 10)
-pop.initialize()
-for _ in range(10):
-    pop.next_generation()
-    print('Average fitness: {}'.format(pop.average_fitness))
-    print('Average obj. fn. return value: {}'.format(pop.average_ret_val))
-    print('Best fitness score: {}'.format(pop.best_fitness))
-    print('Best obj. fn. return value: {}'.format(pop.best_ret_val))
-    print('Best parameters: {}\n'.format(pop.best_params))
-```
-
-Running this script produces:
-
-```
-Average fitness: 0.11519380797455661
-Average obj. fn. return value: 9.545454545454545
-Best fitness score: 0.25
-Best obj. fn. return value: 3
-Best parameters: [1, 0, 2]
-
-Average fitness: 0.16551587301587303
-Average obj. fn. return value: 5.6
-Best fitness score: 0.25
-Best obj. fn. return value: 3
-Best parameters: [1, 0, 2]
-
-Average fitness: 0.1694047619047619
-Average obj. fn. return value: 5.5
-Best fitness score: 0.25
-Best obj. fn. return value: 3
-Best parameters: [1, 0, 2]
-
-Average fitness: 0.18857142857142856
-Average obj. fn. return value: 4.9
-Best fitness score: 0.25
-Best obj. fn. return value: 3
-Best parameters: [1, 2, 0]
-
-Average fitness: 0.19935064935064933
-Average obj. fn. return value: 5.0
-Best fitness score: 0.5
-Best obj. fn. return value: 1
-Best parameters: [1, 0, 0]
-
-Average fitness: 0.2946969696969697
-Average obj. fn. return value: 3.1818181818181817
-Best fitness score: 0.5
-Best obj. fn. return value: 1
-Best parameters: [1, 0, 0]
-
-Average fitness: 0.29416666666666663
-Average obj. fn. return value: 3.2
-Best fitness score: 0.5
-Best obj. fn. return value: 1
-Best parameters: [1, 0, 0]
-
-Average fitness: 0.25844155844155847
-Average obj. fn. return value: 3.5454545454545454
-Best fitness score: 0.5
-Best obj. fn. return value: 1
-Best parameters: [1, 0, 0]
-
-Average fitness: 0.3538961038961039
-Average obj. fn. return value: 2.727272727272727
-Best fitness score: 0.5
-Best obj. fn. return value: 1
-Best parameters: [1, 0, 0]
-
-Average fitness: 0.4772727272727273
-Average obj. fn. return value: 1.1818181818181819
-Best fitness score: 0.5
-Best obj. fn. return value: 1
-Best parameters: [1, 0, 0]
-```
-
-To run this script yourself, head over to our [examples](https://github.com/tjkessler/PyGenetics/tree/master/examples) directory.
-
-# Contributing, Reporting Issues and Other Support:
-
-To contribute to PyGenetics, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
-
-To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
-
-For additional support/questions, contact Travis Kessler (travis.j.kessler@gmail.com).
+# PyGenetics: Genetic Algorithm for Tuning Function Parameters
+
+[![GitHub version](https://badge.fury.io/gh/tjkessler%2FPyGenetics.svg)](https://badge.fury.io/gh/tjkessler%2FPyGenetics)
+[![PyPI version](https://badge.fury.io/py/pygenetics.svg)](https://badge.fury.io/py/pygenetics)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/TJKessler/PyGenetics/master/LICENSE.txt)
+[![Build Status](https://dev.azure.com/travisjkessler/personal-repos/_apis/build/status/tjkessler.PyGenetics?branchName=master)](https://dev.azure.com/travisjkessler/personal-repos/_build/latest?definitionId=7&branchName=master)
+
+PyGenetics is an open source Python package used to tune parameters for user-supplied functions. Inspired by [genetic algorithms](https://www.researchgate.net/profile/Darrell_Whitley2/publication/2425017_A_Genetic_Algorithm_Tutorial/links/563214a108ae506cea68fd96/A-Genetic-Algorithm-Tutorial.pdf), PyGenetics is able to optimize variables in a multidimensional search space to minimize a "cost" (e.g. an error value returned by the user-supplied function).
+
+<p align="center">
+  <img align="center" src="docs/img/demo.gif" width="75%" height="75%">
+</p>
+
+# Installation:
+
+### Method 1: pip
+```
+pip install pygenetics
+```
+
+To update your version of PyGenetics to the latest version, use:
+```
+pip install --upgrade pygenetics
+```
+
+### Method 2: From source
+Download the PyGenetics repository, navigate to the download location on the command line/terminal, and execute:
+```
+pip install .
+```
+
+There are currently no additional dependencies for PyGenetics.
+
+# Usage:
+
+To start using PyGenetics, you need a couple items:
+- a cost function (objective function) to optimize
+- parameters used by the cost function
+
+For example, let's define a cost function to minimize the sum of three integers:
+
+```python
+def minimize_integers(integers):
+
+    return sum(integers)
+
+```
+
+Your cost function must accept a **list** from PyGenetics. The list values represent the current solution, i.e. parameter values, being evaluated by a population member
+
+Now that we have our cost function, let's import the Population object from PyGenetics, initialize the population, and add our parameters/genes:
+
+```python
+from pygenetics import Population
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+pop = Population(10, minimize_integers)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+```
+
+Here we initialize the population with 10 population members, supply our cost function and add our parameters/genes. Parameters are added with minimum/maximum values for its search space. By default, parameter mutations (searching a neighboring solution) will not exceed the specified parameter bounds [min_val, max_val]; if this limitation is not desired, supply the "restrict=False" argument:
+
+```python
+pop.add_param(0, 10, restrict=False)
+```
+
+Once we have created our population and added our parameters/genes, we then need to "initialize" the population's members:
+
+```python
+from pygenetics import Population
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+pop = Population(10, minimize_integers)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.initialize()
+```
+
+Initializing the population's members (in this example, 10 members) deploys them to random solutions/chromosomes (a random parameter/gene set is created), and their fitness is evaluated (in this example, lowest sum is better).
+
+We then compute a pre-determined number of generations, each derived from the previous generation's members:
+
+```python
+from pygenetics import Population
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+pop = Population(10, minimize_integers)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.initialize()
+for _ in range(10):
+    pop.next_generation()
+```
+
+Computing the next generation consists of:
+
+- **1.** Select a chromosome (parameter/gene set) from the population based on fitness (a higher fitness score results in a higher chance of being chosen)
+
+- **2a.** Perform crossover with probability _p<sub>c</sub>_ (default of 0.5, 50%); if crossover is not performed, perform step (2b)
+
+    - Select a different chromosome per method in (1)
+    - Select a crossover point between 1 and L-1 (random index in chromosomes' genes) with uniform probability
+    - Recombine chromosomes to form two offspring
+    - Perform mutation on each gene with probability _p<sub>m</sub>_ (default of 0.01, 1%)
+    - Place both offspring in the next generation
+    
+- **2b.** Crossover not performed, perform mutation on each gene of the chromosome with probability _p<sub>m</sub>_ (default of 0.01, 1%), place chromosome in the next generation
+
+- **3.** If the next generation is not full (less than total population size), continue from step (1)
+
+Both _p<sub>c</sub>_ and _p<sub>m</sub>_ can be adjusted when the next generation is created:
+
+```python
+pop.next_generation(p_crossover=0.75, p_mutation=0.05)
+```
+
+We can access the populations's average fitness score, average objective function return value, best fitness score, best objective function return value and best parameters at any time:
+
+```python
+print(pop.average_fitness)
+print(pop.average_ret_val)
+print(pop.best_fitness)
+print(pop.best_ret_val)
+print(pop.best_params)
+```
+
+PyGenetics can utilize multiple CPU cores for concurrent processing:
+
+```python
+pop = Population(10, minimize_integers, num_processes=8)
+```
+
+Tying everything together, we have:
+
+```python
+from pygenetics import Population
+
+def minimize_integers(integers):
+
+    return sum(integers)
+
+pop = Population(10, minimize_integers)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.add_param(0, 10)
+pop.initialize()
+for _ in range(10):
+    pop.next_generation()
+    print('Average fitness: {}'.format(pop.average_fitness))
+    print('Average obj. fn. return value: {}'.format(pop.average_ret_val))
+    print('Best fitness score: {}'.format(pop.best_fitness))
+    print('Best obj. fn. return value: {}'.format(pop.best_ret_val))
+    print('Best parameters: {}\n'.format(pop.best_params))
+```
+
+Running this script produces:
+
+```
+Average fitness: 0.11519380797455661
+Average obj. fn. return value: 9.545454545454545
+Best fitness score: 0.25
+Best obj. fn. return value: 3
+Best parameters: [1, 0, 2]
+
+Average fitness: 0.16551587301587303
+Average obj. fn. return value: 5.6
+Best fitness score: 0.25
+Best obj. fn. return value: 3
+Best parameters: [1, 0, 2]
+
+Average fitness: 0.1694047619047619
+Average obj. fn. return value: 5.5
+Best fitness score: 0.25
+Best obj. fn. return value: 3
+Best parameters: [1, 0, 2]
+
+Average fitness: 0.18857142857142856
+Average obj. fn. return value: 4.9
+Best fitness score: 0.25
+Best obj. fn. return value: 3
+Best parameters: [1, 2, 0]
+
+Average fitness: 0.19935064935064933
+Average obj. fn. return value: 5.0
+Best fitness score: 0.5
+Best obj. fn. return value: 1
+Best parameters: [1, 0, 0]
+
+Average fitness: 0.2946969696969697
+Average obj. fn. return value: 3.1818181818181817
+Best fitness score: 0.5
+Best obj. fn. return value: 1
+Best parameters: [1, 0, 0]
+
+Average fitness: 0.29416666666666663
+Average obj. fn. return value: 3.2
+Best fitness score: 0.5
+Best obj. fn. return value: 1
+Best parameters: [1, 0, 0]
+
+Average fitness: 0.25844155844155847
+Average obj. fn. return value: 3.5454545454545454
+Best fitness score: 0.5
+Best obj. fn. return value: 1
+Best parameters: [1, 0, 0]
+
+Average fitness: 0.3538961038961039
+Average obj. fn. return value: 2.727272727272727
+Best fitness score: 0.5
+Best obj. fn. return value: 1
+Best parameters: [1, 0, 0]
+
+Average fitness: 0.4772727272727273
+Average obj. fn. return value: 1.1818181818181819
+Best fitness score: 0.5
+Best obj. fn. return value: 1
+Best parameters: [1, 0, 0]
+```
+
+To run this script yourself, head over to our [examples](https://github.com/tjkessler/PyGenetics/tree/master/examples) directory.
+
+# Contributing, Reporting Issues and Other Support:
+
+To contribute to PyGenetics, make a pull request. Contributions should include tests for new features added, as well as extensive documentation.
+
+To report problems with the software or feature requests, file an issue. When reporting problems, include information such as error messages, your OS/environment and Python version.
+
+For additional support/questions, contact Travis Kessler (travis.j.kessler@gmail.com).
```

### Comparing `pygenetics-1.0.0/pygenetics/member.py` & `pygenetics-1.0.1/pygenetics/member.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# pygenetics/member.py
-# v.1.0.0
-# Developed in 2019 by Travis Kessler <travis.j.kessler@gmail.com>
-#
-# Contains the Member object
-#
-
-from typing import Union
-
-
-class Member:
-
-    def __init__(self, params: list, obj_fn_val: Union[int, float]):
-        ''' Member object: houses information about a population member's
-        currently-used parameters, the return value of the objective function
-        using these parameters, and the fitness score resulting from this
-        return value
-
-        Args:
-            params (list): currently-used parameter values
-            obj_fn_val (int, float): value returned by the user-supplied
-                objective function
-        '''
-
-        self._params = params
-        self._obj_fn_val = obj_fn_val
-        self._fitness_score = self.calc_fitness(obj_fn_val)
-
-    @staticmethod
-    def calc_fitness(obj_fn_val: Union[int, float]) -> float:
-        ''' Static method: Member.calc_fitness: Calculates fitness score based on
-        objective function value, using the equation:
-
-        fitness = 1 / (1 + ofv)     if ofv >= 0
-        fitness = 1 + abs(ofv)      if ofv < 0
-
-        Where `ofv` is the objective function value and `fitness` is the
-        resulting fitness score
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
+from typing import Union
+
+
+class Member:
+
+    def __init__(self, params: list, obj_fn_val: Union[int, float]):
+        ''' Member object: houses information about a population member's
+        currently-used parameters, the return value of the objective function
+        using these parameters, and the fitness score resulting from this
+        return value
+
+        Args:
+            params (list): currently-used parameter values
+            obj_fn_val (int, float): value returned by the user-supplied
+                objective function
+        '''
+
+        self._params = params
+        self._obj_fn_val = obj_fn_val
+        self._fitness_score = self.calc_fitness(obj_fn_val)
+
+    @staticmethod
+    def calc_fitness(obj_fn_val: Union[int, float]) -> float:
+        ''' Static method: Member.calc_fitness: Calculates fitness score based
+        on objective function value, using the equation:
+
+        fitness = 1 / (1 + ofv)     if ofv >= 0
+        fitness = 1 + abs(ofv)      if ofv < 0
+
+        Where `ofv` is the objective function value and `fitness` is the
+        resulting fitness score
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
```

### Comparing `pygenetics-1.0.0/pygenetics/parameter.py` & `pygenetics-1.0.1/pygenetics/parameter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,81 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# pygenetics/parameter.py
-# v.1.0.0
-# Developed in 2019 by Travis Kessler <travis.j.kessler@gmail.com>
-#
-# Contains the Parameter object
-#
-
-from random import uniform
-from typing import Union
-
-
-class Parameter:
-
-    def __init__(self, min_val: Union[int, float], max_val: Union[int, float],
-                 restrict: bool=True):
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
-        '''
-
-        if type(min_val) != type(max_val):
-            raise ValueError('Supplied min_val is not the same type as '
-                             'supplied max_val: {}, {}'.format(
-                                 type(min_val), type(max_val)
-                             ))
-
-        if type(min_val) not in [int, float]:
-            raise ValueError('Unsupported data type for Parameter, {}; use {}'
-                             .format(type(min_val), [int, float]))
-
-        self._min_val = min_val
-        self._max_val = max_val
-        self._dtype = type(min_val)
-        self._restrict = restrict
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
+from random import uniform
+from typing import Union
+
+
+class Parameter:
+
+    def __init__(self, min_val: Union[int, float], max_val: Union[int, float],
+                 restrict: bool = True):
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
+        '''
+
+        if type(min_val) != type(max_val):
+            raise ValueError('Supplied min_val is not the same type as '
+                             'supplied max_val: {}, {}'.format(
+                                 type(min_val), type(max_val)
+                             ))
+
+        if type(min_val) not in [int, float]:
+            raise ValueError('Unsupported data type for Parameter, {}; use {}'
+                             .format(type(min_val), [int, float]))
+
+        self._min_val = min_val
+        self._max_val = max_val
+        self._dtype = type(min_val)
+        self._restrict = restrict
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

### Comparing `pygenetics-1.0.0/pygenetics/population.py` & `pygenetics-1.0.1/pygenetics/population.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,239 +1,230 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# pygenetics/population.py
-# v.1.0.0
-# Developed in 2019 by Travis Kessler <travis.j.kessler@gmail.com>
-#
-# Contains the Population object
-#
-
-from bisect import bisect
-from multiprocessing import Pool
-from random import random, uniform
-from typing import Callable, Union
-from warnings import warn
-
-from pygenetics.member import Member
-from pygenetics.parameter import Parameter
-from pygenetics.utils import calc_cdf_vals, call_obj_fn,\
-    determine_best_member, mutate_params, perform_crossover
-
-
-class Population:
-
-    def __init__(self, pop_size: int,
-                 objective_fn: Callable[[list], Union[int, float]],
-                 obj_fn_args: dict={}, num_processes: int=1):
-        ''' Population object: initializes a genetic algorithm population with
-        user-specified population size, objective function and any additional
-        immutable objects to pass to the objective function
-
-        Args:
-            pop_size (int): size of the population
-            objective_fn (callable): function for optimization
-            obj_fn_args (dict): immutable arguments to pass to objective_fn
-            num_processes (int): number of concurrent processes to utilize
-        '''
-
-        if not callable(objective_fn):
-            raise ReferenceError('Supplied objective function is not callable')
-
-        if pop_size <= 1:
-            raise ValueError('`pop_size` must be >= 2: {}'.format(pop_size))
-
-        self._obj_fn = objective_fn
-        self._obj_fn_args = obj_fn_args
-        self._pop_size = pop_size
-        self._num_processes = num_processes
-        self._members = []
-        self._params = []
-
-    @property
-    def best_fitness(self) -> float:
-        ''' Returns fitness score from best-performing member '''
-
-        if len(self._members) == 0:
-            return None
-        return determine_best_member(self._members)[0]
-
-    @property
-    def best_ret_val(self) -> Union[int, float]:
-        ''' Returns objective_fn return value from best-performing member '''
-
-        if len(self._members) == 0:
-            return None
-        return determine_best_member(self._members)[1]
-
-    @property
-    def best_params(self) -> list:
-        ''' Returns parameters from best-performing member '''
-
-        if len(self._members) == 0:
-            return None
-        return determine_best_member(self._members)[2]
-
-    @property
-    def average_fitness(self) -> float:
-        ''' Returns average fitness score for population '''
-
-        if len(self._members) == 0:
-            return None
-        return (sum(m._fitness_score for m in self._members) /
-                len(self._members))
-
-    @property
-    def average_ret_val(self) -> float:
-        ''' Returns average objective_fn return value for population '''
-
-        if len(self._members) == 0:
-            return None
-        return (sum(m._obj_fn_val for m in self._members) / len(self._members))
-
-    def add_param(self, min_val: Union[int, float], max_val: Union[int, float],
-                  restrict: bool=True):
-        ''' Population.add_param: adds a parameter to be processed by the user-
-        supplied objective function
-
-        Args:
-            min_val (int, float): minimum value allowed for the parameter's
-                initialization
-            max_val (int, float): maximum value allowed for the parameter's
-                initialization
-            restrict (bool): if `True`, parameter mutations must be within
-                [min_val, max_val], `False` allows out-of-bounds mutation
-        '''
-
-        if len(self._members) > 0:
-            raise RuntimeError(
-                'Cannot add another parameter after population is created'
-            )
-
-        self._params.append(Parameter(min_val, max_val, restrict))
-
-    def initialize(self):
-        ''' Population.initialize: generates random paramter values for each
-        population member, evaluates fitness for each
-        '''
-
-        if len(self._params) == 0:
-            raise RuntimeError(
-                'No parameters have been added, cannot initialize'
-            )
-
-        if len(self._members) > 0:
-            warn('initialize() called again: overwriting current population',
-                 RuntimeWarning)
-
-        self._members = []
-
-        if self._num_processes > 1:
-            mp_pool = Pool(processes=self._num_processes)
-        member_results = []
-
-        for _ in range(self._pop_size):
-
-            params = [p.rand_val for p in self._params]
-            if self._num_processes > 1:
-                member_results.append(mp_pool.apply_async(
-                    call_obj_fn, [params, self._obj_fn, self._obj_fn_args]
-                ))
-            else:
-                member_results.append(call_obj_fn(
-                    params, self._obj_fn, self._obj_fn_args
-                ))
-
-        if self._num_processes > 1:
-
-            mp_pool.close()
-            mp_pool.join()
-            member_results = [r.get() for r in member_results]
-
-        for result in member_results:
-
-            self._members.append(Member(result[0], result[1]))
-
-    def next_generation(self, p_crossover: float=0.5, p_mutation: float=0.01):
-        ''' Population.next_generation: generates the next generation of
-        population members; members are chosen proportionally based on their
-        fitness, where a higher fitness results in a higher chance to be
-        chosen for the next generation; included is a chance for crossover
-        between two members and a chance for mutation within a member's
-        parameter/chromosome
-
-        Args:
-            p_crossover (float): [0, 1], probability a member is subjected to
-                crossover after selection for the next generation; default
-                value of 0.5 (50%)
-            p_mutation (float): [0, 1], probability a chosen member's
-                parameters are subject to mutation; default value of 0.01 (1%)
-        '''
-
-        if len(self._members) == 0:
-            raise RuntimeError(
-                'initilize() must be called before next_generation()'
-            )
-
-        if p_crossover < 0 or p_crossover > 1:
-            raise ValueError('`p_crossover` must be within [0, 1]: {}'.format(
-                p_crossover
-            ))
-
-        if p_mutation < 0 or p_mutation > 1:
-            raise ValueError('`p_mutation` must be within [0, 1]: {}'.format(
-                p_mutation
-            ))
-
-        new_param_vals = []
-        cdf_vals = calc_cdf_vals(self._members)
-
-        while len(new_param_vals) < self._pop_size:
-
-            chosen_member = self._members[bisect(cdf_vals, random())]
-
-            if len(self._params) > 1 and uniform(0, 1) < p_crossover:
-
-                mate = self._members[bisect(cdf_vals, random())]
-                while chosen_member == mate:
-                    mate = self._members[bisect(cdf_vals, random())]
-                new_params_1, new_params_2 = perform_crossover(
-                    chosen_member._params, mate._params
-                )
-                new_param_vals.append(mutate_params(
-                    new_params_1, self._params, p_mutation
-                ))
-                new_param_vals.append(mutate_params(
-                    new_params_2, self._params, p_mutation
-                ))
-
-            else:
-
-                new_param_vals.append(mutate_params(
-                    chosen_member._params, self._params, p_mutation
-                ))
-
-        if self._num_processes > 1:
-            mp_pool = Pool(processes=self._num_processes)
-        new_member_results = []
-
-        for vals in new_param_vals:
-
-            if self._num_processes > 1:
-                new_member_results.append(mp_pool.apply_async(
-                    call_obj_fn, [vals, self._obj_fn, self._obj_fn_args]
-                ))
-            else:
-                new_member_results.append(call_obj_fn(
-                    vals, self._obj_fn, self._obj_fn_args
-                ))
-
-        if self._num_processes > 1:
-
-            mp_pool.close()
-            mp_pool.join()
-            new_member_results = [r.get() for r in new_member_results]
-
-        self._members = []
-        for result in new_member_results:
-
-            self._members.append(Member(result[0], result[1]))
+from bisect import bisect
+from multiprocessing import Pool
+from random import random, uniform
+from typing import Callable, Union
+from warnings import warn
+
+from pygenetics.member import Member
+from pygenetics.parameter import Parameter
+from pygenetics.utils import calc_cdf_vals, call_obj_fn,\
+    determine_best_member, mutate_params, perform_crossover
+
+
+class Population:
+
+    def __init__(self, pop_size: int,
+                 objective_fn: Callable[[list], Union[int, float]],
+                 obj_fn_args: dict = {}, num_processes: int = 1):
+        ''' Population object: initializes a genetic algorithm population with
+        user-specified population size, objective function and any additional
+        immutable objects to pass to the objective function
+
+        Args:
+            pop_size (int): size of the population
+            objective_fn (callable): function for optimization
+            obj_fn_args (dict): immutable arguments to pass to objective_fn
+            num_processes (int): number of concurrent processes to utilize
+        '''
+
+        if not callable(objective_fn):
+            raise ReferenceError('Supplied objective function is not callable')
+
+        if pop_size <= 1:
+            raise ValueError('`pop_size` must be >= 2: {}'.format(pop_size))
+
+        self._obj_fn = objective_fn
+        self._obj_fn_args = obj_fn_args
+        self._pop_size = pop_size
+        self._num_processes = num_processes
+        self._members = []
+        self._params = []
+
+    @property
+    def best_fitness(self) -> float:
+        ''' Returns fitness score from best-performing member '''
+
+        if len(self._members) == 0:
+            return None
+        return determine_best_member(self._members)[0]
+
+    @property
+    def best_ret_val(self) -> Union[int, float]:
+        ''' Returns objective_fn return value from best-performing member '''
+
+        if len(self._members) == 0:
+            return None
+        return determine_best_member(self._members)[1]
+
+    @property
+    def best_params(self) -> list:
+        ''' Returns parameters from best-performing member '''
+
+        if len(self._members) == 0:
+            return None
+        return determine_best_member(self._members)[2]
+
+    @property
+    def average_fitness(self) -> float:
+        ''' Returns average fitness score for population '''
+
+        if len(self._members) == 0:
+            return None
+        return (sum(m._fitness_score for m in self._members) /
+                len(self._members))
+
+    @property
+    def average_ret_val(self) -> float:
+        ''' Returns average objective_fn return value for population '''
+
+        if len(self._members) == 0:
+            return None
+        return (sum(m._obj_fn_val for m in self._members) / len(self._members))
+
+    def add_param(self, min_val: Union[int, float], max_val: Union[int, float],
+                  restrict: bool = True):
+        ''' Population.add_param: adds a parameter to be processed by the user-
+        supplied objective function
+
+        Args:
+            min_val (int, float): minimum value allowed for the parameter's
+                initialization
+            max_val (int, float): maximum value allowed for the parameter's
+                initialization
+            restrict (bool): if `True`, parameter mutations must be within
+                [min_val, max_val], `False` allows out-of-bounds mutation
+        '''
+
+        if len(self._members) > 0:
+            raise RuntimeError(
+                'Cannot add another parameter after population is created'
+            )
+
+        self._params.append(Parameter(min_val, max_val, restrict))
+
+    def initialize(self):
+        ''' Population.initialize: generates random paramter values for each
+        population member, evaluates fitness for each
+        '''
+
+        if len(self._params) == 0:
+            raise RuntimeError(
+                'No parameters have been added, cannot initialize'
+            )
+
+        if len(self._members) > 0:
+            warn('initialize() called again: overwriting current population',
+                 RuntimeWarning)
+
+        self._members = []
+
+        if self._num_processes > 1:
+            mp_pool = Pool(processes=self._num_processes)
+        member_results = []
+
+        for _ in range(self._pop_size):
+
+            params = [p.rand_val for p in self._params]
+            if self._num_processes > 1:
+                member_results.append(mp_pool.apply_async(
+                    call_obj_fn, [params, self._obj_fn, self._obj_fn_args]
+                ))
+            else:
+                member_results.append(call_obj_fn(
+                    params, self._obj_fn, self._obj_fn_args
+                ))
+
+        if self._num_processes > 1:
+
+            mp_pool.close()
+            mp_pool.join()
+            member_results = [r.get() for r in member_results]
+
+        for result in member_results:
+
+            self._members.append(Member(result[0], result[1]))
+
+    def next_generation(self, p_crossover: float = 0.5,
+                        p_mutation: float = 0.01):
+        ''' Population.next_generation: generates the next generation of
+        population members; members are chosen proportionally based on their
+        fitness, where a higher fitness results in a higher chance to be
+        chosen for the next generation; included is a chance for crossover
+        between two members and a chance for mutation within a member's
+        parameter/chromosome
+
+        Args:
+            p_crossover (float): [0, 1], probability a member is subjected to
+                crossover after selection for the next generation; default
+                value of 0.5 (50%)
+            p_mutation (float): [0, 1], probability a chosen member's
+                parameters are subject to mutation; default value of 0.01 (1%)
+        '''
+
+        if len(self._members) == 0:
+            raise RuntimeError(
+                'initilize() must be called before next_generation()'
+            )
+
+        if p_crossover < 0 or p_crossover > 1:
+            raise ValueError('`p_crossover` must be within [0, 1]: {}'.format(
+                p_crossover
+            ))
+
+        if p_mutation < 0 or p_mutation > 1:
+            raise ValueError('`p_mutation` must be within [0, 1]: {}'.format(
+                p_mutation
+            ))
+
+        new_param_vals = []
+        cdf_vals = calc_cdf_vals(self._members)
+
+        while len(new_param_vals) < self._pop_size:
+
+            chosen_member = self._members[bisect(cdf_vals, random())]
+
+            if len(self._params) > 1 and uniform(0, 1) < p_crossover:
+
+                mate = self._members[bisect(cdf_vals, random())]
+                while chosen_member == mate:
+                    mate = self._members[bisect(cdf_vals, random())]
+                new_params_1, new_params_2 = perform_crossover(
+                    chosen_member._params, mate._params
+                )
+                new_param_vals.append(mutate_params(
+                    new_params_1, self._params, p_mutation
+                ))
+                new_param_vals.append(mutate_params(
+                    new_params_2, self._params, p_mutation
+                ))
+
+            else:
+
+                new_param_vals.append(mutate_params(
+                    chosen_member._params, self._params, p_mutation
+                ))
+
+        if self._num_processes > 1:
+            mp_pool = Pool(processes=self._num_processes)
+        new_member_results = []
+
+        for vals in new_param_vals:
+
+            if self._num_processes > 1:
+                new_member_results.append(mp_pool.apply_async(
+                    call_obj_fn, [vals, self._obj_fn, self._obj_fn_args]
+                ))
+            else:
+                new_member_results.append(call_obj_fn(
+                    vals, self._obj_fn, self._obj_fn_args
+                ))
+
+        if self._num_processes > 1:
+
+            mp_pool.close()
+            mp_pool.join()
+            new_member_results = [r.get() for r in new_member_results]
+
+        self._members = []
+        for result in new_member_results:
+
+            self._members.append(Member(result[0], result[1]))
```

### Comparing `pygenetics-1.0.0/pygenetics/utils.py` & `pygenetics-1.0.1/pygenetics/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,115 +1,105 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# pygenetics/utils.py
-# v.1.0.0
-# Developed in 2019 by Travis Kessler <travis.j.kessler@gmail.com>
-#
-# Contains function utilized by PyGenetics classes
-#
-
-from random import randint, uniform
-
-
-def calc_cdf_vals(members: list) -> list:
-    ''' calc_cdf_vals: calculates the cumulative distribution of population
-    member selection probabilities (i.e. members w/ higher fitness more likely
-    to be chosen for next generation)
-
-    Args:
-        members (list): list of pygenetics.Member objects
-
-    Returns:
-        list: CDF values w/ parallel indices to supplied Members
-    '''
-
-    fitness_sum = sum(m._fitness_score for m in members)
-    selection_probs = [m._fitness_score / fitness_sum for m in members]
-    cdf_vals = []
-    cumsum = 0
-    for p in selection_probs:
-        cumsum += p
-        cdf_vals.append(cumsum)
-    return cdf_vals
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
-def determine_best_member(members: list) -> tuple:
-    ''' determine_best_member: returns the fitness score, objective function
-    return value, and paramters for the best-performing population member
-
-    Args:
-        members (list): list of pygenetics.Member objects
-
-    Returns:
-        tuple: (best fitness, best return value, best parameters)
-    '''
-
-    best_fitness = members[0]._fitness_score
-    best_ret_val = members[0]._obj_fn_val
-    best_params = members[0]._params
-    for m in members[1:]:
-        if m._fitness_score > best_fitness:
-            best_fitness = m._fitness_score
-            best_ret_val = m._obj_fn_val
-            best_params = m._params
-    return (best_fitness, best_ret_val, best_params)
-
-
-def mutate_params(curr_params: list, params: list, p_mutation: float) -> list:
-    ''' mutate_parameters: based on supplied mutation rate, mutates parameters
-    supplied by the user
-
-    Args:
-        curr_params (list): current parameter values, int or float
-        params (list): list of pygenetics.Parameter objects
-        p_mutation (float): [0, 1], probability of mutation on any parameter
-
-    Returns:
-        list: mutated parameters
-    '''
-
-    new_params = []
-    for idx, param in enumerate(curr_params):
-        if uniform(0, 1) < p_mutation:
-            new_params.append(params[idx].mutate(param))
-        else:
-            new_params.append(param)
-    return new_params
-
-
-def perform_crossover(params_1: list, params_2: list) -> tuple:
-    ''' perform_crossover: performs a crossover of two parameter lists, using
-    a random crossover point, and returns the resulting parameter lists
-
-    Args:
-        params_1 (list): first set of parameter values
-        params_2 (list): second set of paramter values
-
-    Returns:
-        tuple: (crossed 1, crossed 2)
-    '''
-
-    cross_pt = randint(1, len(params_1) - 1)
-    first_params = params_1[:cross_pt]
-    first_params.extend(params_2[cross_pt:])
-    second_params = params_2[:cross_pt]
-    second_params.extend(params_1[cross_pt:])
-    return (first_params, second_params)
+from random import randint, uniform
+
+
+def calc_cdf_vals(members: list) -> list:
+    ''' calc_cdf_vals: calculates the cumulative distribution of population
+    member selection probabilities (i.e. members w/ higher fitness more likely
+    to be chosen for next generation)
+
+    Args:
+        members (list): list of pygenetics.Member objects
+
+    Returns:
+        list: CDF values w/ parallel indices to supplied Members
+    '''
+
+    fitness_sum = sum(m._fitness_score for m in members)
+    selection_probs = [m._fitness_score / fitness_sum for m in members]
+    cdf_vals = []
+    cumsum = 0
+    for p in selection_probs:
+        cumsum += p
+        cdf_vals.append(cumsum)
+    return cdf_vals
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
+def determine_best_member(members: list) -> tuple:
+    ''' determine_best_member: returns the fitness score, objective function
+    return value, and paramters for the best-performing population member
+
+    Args:
+        members (list): list of pygenetics.Member objects
+
+    Returns:
+        tuple: (best fitness, best return value, best parameters)
+    '''
+
+    best_fitness = members[0]._fitness_score
+    best_ret_val = members[0]._obj_fn_val
+    best_params = members[0]._params
+    for m in members[1:]:
+        if m._fitness_score > best_fitness:
+            best_fitness = m._fitness_score
+            best_ret_val = m._obj_fn_val
+            best_params = m._params
+    return (best_fitness, best_ret_val, best_params)
+
+
+def mutate_params(curr_params: list, params: list, p_mutation: float) -> list:
+    ''' mutate_parameters: based on supplied mutation rate, mutates parameters
+    supplied by the user
+
+    Args:
+        curr_params (list): current parameter values, int or float
+        params (list): list of pygenetics.Parameter objects
+        p_mutation (float): [0, 1], probability of mutation on any parameter
+
+    Returns:
+        list: mutated parameters
+    '''
+
+    new_params = []
+    for idx, param in enumerate(curr_params):
+        if uniform(0, 1) < p_mutation:
+            new_params.append(params[idx].mutate(param))
+        else:
+            new_params.append(param)
+    return new_params
+
+
+def perform_crossover(params_1: list, params_2: list) -> tuple:
+    ''' perform_crossover: performs a crossover of two parameter lists, using
+    a random crossover point, and returns the resulting parameter lists
+
+    Args:
+        params_1 (list): first set of parameter values
+        params_2 (list): second set of paramter values
+
+    Returns:
+        tuple: (crossed 1, crossed 2)
+    '''
+
+    cross_pt = randint(1, len(params_1) - 1)
+    first_params = params_1[:cross_pt]
+    first_params.extend(params_2[cross_pt:])
+    second_params = params_2[:cross_pt]
+    second_params.extend(params_1[cross_pt:])
+    return (first_params, second_params)
```

